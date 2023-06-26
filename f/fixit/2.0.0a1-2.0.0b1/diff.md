# Comparing `tmp/fixit-2.0.0a1.tar.gz` & `tmp/fixit-2.0.0b1.tar.gz`

## Comparing `fixit-2.0.0a1.tar` & `fixit-2.0.0b1.tar`

### file list

```diff
@@ -1,95 +1,96 @@
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.editorconfig
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.flake8
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.mailmap
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.pyre_configuration
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.readthedocs.yml
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.watchmanconfig
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 fixit-2.0.0a1/CHANGELOG.md
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fixit-2.0.0a1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 fixit-2.0.0a1/CONTRIBUTING.md
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fixit-2.0.0a1/makefile
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/api.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/changelog.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/code-of-conduct.rst
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/conf.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/contributing.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide.rst
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/index.rst
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/proposals.rst
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/why.rst
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/custom.css
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/fbopensource.png
--rw-r--r--   0        0        0    21530 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/opensource.png
--rw-r--r--   0        0        0    22163 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/icon.png
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/icon.svg
--rw-r--r--   0        0        0    21638 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/icon_whilte.png
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/icon_white.svg
--rw-r--r--   0        0        0    37225 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/logo.png
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/logo.svg
--rw-r--r--   0        0        0    36486 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/logo_whilte.png
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/logo_white.svg
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_templates/badges.html
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_templates/meta.html
--rw-r--r--   0        0        0    30722 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/builtins.rst
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/commands.rst
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/configuration.rst
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/integrations.rst
--rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/quickstart.rst
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/proposals/fp1.md
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/proposals/fp2.rst
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fixit-2.0.0a1/scripts/check_copyright.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 fixit-2.0.0a1/scripts/document_rules.py
--rwxr-xr-x   0        0        0     3360 2020-02-02 00:00:00.000000 fixit-2.0.0a1/scripts/migrate_rule_to_fixit2.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/__version__.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/api.py
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/cli.py
--rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/config.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/engine.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/ftypes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/py.typed
--rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rule.py
--rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/testing.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/util.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/local/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/__init__.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/avoid_or_in_except.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/chained_instance_check.py
--rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/cls_in_classmethod.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/compare_primitives_by_equal.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/compare_singleton_primitives_by_is.py
--rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/explicit_frozen_dataclass.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_assert_equals.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_assert_true_for_comparison.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_inherit_from_object.py
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_namedtuple.py
--rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_redundant_arguments_super.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_redundant_fstring.py
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_redundant_lambda.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_redundant_list_comprehension.py
--rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_static_if_condition.py
--rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_string_type_annotation.py
--rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/replace_union_with_optional.py
--rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/rewrite_to_comprehension.py
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/rewrite_to_literal.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/sorted_attributes_rule.py
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_assert_in.py
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_assert_is_not_none.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_classname_as_code.py
--rw-r--r--   0        0        0     9303 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_fstring.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_lint_fixme_comment.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_types_from_typing.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/__main__.py
--rw-r--r--   0        0        0    13344 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/config.py
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/ftypes.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/rule.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/smoke.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.gitignore
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 fixit-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 fixit-2.0.0a1/README.rst
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 fixit-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     7747 2020-02-02 00:00:00.000000 fixit-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.editorconfig
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.flake8
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.mailmap
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.pyre_configuration
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.readthedocs.yml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.watchmanconfig
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 fixit-2.0.0b1/CHANGELOG.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fixit-2.0.0b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 fixit-2.0.0b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fixit-2.0.0b1/makefile
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/api.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/changelog.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/code-of-conduct.rst
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/conf.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/contributing.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/guide.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/index.rst
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/proposals.rst
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/why.rst
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/custom.css
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/fbopensource.png
+-rw-r--r--   0        0        0    21530 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/opensource.png
+-rw-r--r--   0        0        0    22163 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/logo/icon.png
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/logo/icon.svg
+-rw-r--r--   0        0        0    21638 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/logo/icon_whilte.png
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/logo/icon_white.svg
+-rw-r--r--   0        0        0    37225 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/logo/logo.png
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/logo/logo.svg
+-rw-r--r--   0        0        0    36486 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/logo/logo_whilte.png
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_static/logo/logo_white.svg
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_templates/badges.html
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/_templates/meta.html
+-rw-r--r--   0        0        0    31543 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/guide/builtins.rst
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/guide/commands.rst
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/guide/configuration.rst
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/guide/integrations.rst
+-rw-r--r--   0        0        0     7534 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/guide/quickstart.rst
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/proposals/fp1.md
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 fixit-2.0.0b1/docs/proposals/fp2.rst
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fixit-2.0.0b1/scripts/check_copyright.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 fixit-2.0.0b1/scripts/document_rules.py
+-rwxr-xr-x   0        0        0     3360 2020-02-02 00:00:00.000000 fixit-2.0.0b1/scripts/migrate_rule_to_fixit2.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/__version__.py
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/api.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/cli.py
+-rw-r--r--   0        0        0    15013 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/config.py
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/engine.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/ftypes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/py.typed
+-rw-r--r--   0        0        0     8221 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rule.py
+-rw-r--r--   0        0        0     9568 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/testing.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/util.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/local/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/__init__.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/avoid_or_in_except.py
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/chained_instance_check.py
+-rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/cls_in_classmethod.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/compare_primitives_by_equal.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/compare_singleton_primitives_by_is.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/deprecated_unittest_asserts.py
+-rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/explicit_frozen_dataclass.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_assert_true_for_comparison.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_inherit_from_object.py
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_namedtuple.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_redundant_arguments_super.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_redundant_fstring.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_redundant_lambda.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_redundant_list_comprehension.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_static_if_condition.py
+-rw-r--r--   0        0        0     8629 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/no_string_type_annotation.py
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/replace_union_with_optional.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/rewrite_to_comprehension.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/rewrite_to_literal.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/sorted_attributes_rule.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/use_assert_in.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/use_assert_is_not_none.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/use_async_sleep_in_async_def.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/use_classname_as_code.py
+-rw-r--r--   0        0        0     9303 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/use_fstring.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/use_lint_fixme_comment.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/rules/use_types_from_typing.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/tests/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/tests/__main__.py
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/tests/config.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/tests/ftypes.py
+-rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/tests/rule.py
+-rw-r--r--   0        0        0     5322 2020-02-02 00:00:00.000000 fixit-2.0.0b1/src/fixit/tests/smoke.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 fixit-2.0.0b1/.gitignore
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 fixit-2.0.0b1/LICENSE
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 fixit-2.0.0b1/README.rst
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 fixit-2.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 fixit-2.0.0b1/PKG-INFO
```

### Comparing `fixit-2.0.0a1/.pre-commit-config.yaml` & `fixit-2.0.0b1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/CHANGELOG.md` & `fixit-2.0.0b1/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,34 @@
 # Changelog
 
+## 2.0.0b1 - 2023-06-26
+
+### Beta Release
+
+This is a beta release of a major rework of Fixit. There are many breaking
+API changes since the `0.1.4` release – existing users should wait for a stable
+release before upgrading.
+
+Please see the new [User Guide][] for an overview of the new version.
+A migration guide is planned, but not yet available.
+
+[User Guide]: https://fixit.rtfd.io/en/latest/guide.html
+
+### Major Changes
+
+- New `test` command for validating local lint rules (#300)
+- Support for configurable target version and selection of applicable rules (#332)
+- Support for selecting and filtering rules by tags at runtime (#333)
+- Support for `# lint-ignore` and `# lint-fixme` directives (#334)
+
+### New Rules
+
+- Added `UseAsyncSleepInAsyncDefRule` (#297)
+- Added `DeprecatedUnittestAssertsRule` (#314)
+
 ## 2.0.0a1 - 2023-04-07
 
 ### Alpha Release
 
 This is an alpha release of a major rework of Fixit. There are many breaking
 API changes since the `0.1.4` release – existing users should wait for a stable
 release before upgrading.
```

### Comparing `fixit-2.0.0a1/CONTRIBUTING.md` & `fixit-2.0.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/api.rst` & `fixit-2.0.0b1/docs/api.rst`

 * *Files 12% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 .. autoclass:: LintViolation
 .. autoclass:: Result
 
 
 Advanced API
 ^^^^^^^^^^^^
 
-.. autoclass:: fixit.ftypes.FileContent
+.. autoclass:: fixit.FileContent
 
 .. autofunction:: fixit_bytes
 .. autoclass:: fixit.util.capture
 
 .. autoclass:: Config
+.. autoclass:: Options
 .. autoclass:: QualifiedRule
+.. autoclass:: Tags
```

### Comparing `fixit-2.0.0a1/docs/conf.py` & `fixit-2.0.0b1/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,28 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
+# -- Patch python domain signature regex to allow "foo-bar" style names ------
+
+import re
+# modified from sphinx/domains/python.py
+py_sig_re = re.compile(
+    r'''^ ([\w.]*\.)?            # class name(s)
+          ([\w-]+)  \s*             # thing name
+          (?: \(\s*(.*)\s*\)     # optional: arguments
+           (?:\s* -> \s* (.*))?  #           return annotation
+          )? $                   # and nothing more
+          ''', re.VERBOSE)
+
+from sphinx.domains import python
+python.py_sig_re = py_sig_re
 
 # -- Project information -----------------------------------------------------
 
 import datetime
 
 project = "Fixit"
 copyright = f" Copyright © Meta Platforms, Inc. and affiliates"
@@ -59,14 +73,15 @@
 autodoc_typehints = "description"
 autodoc_typehints_format = "short"
 
 # highlight_language = "python3"
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "libcst": ("https://libcst.rtfd.io/en/latest", None),
+    "packaging": ("https://packaging.pypa.io/en/latest", None),
 }
 master_doc = "index"
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
```

### Comparing `fixit-2.0.0a1/docs/index.rst` & `fixit-2.0.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/why.rst` & `fixit-2.0.0b1/docs/why.rst`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/custom.css` & `fixit-2.0.0b1/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/fbopensource.png` & `fixit-2.0.0b1/docs/_static/fbopensource.png`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/opensource.png` & `fixit-2.0.0b1/docs/_static/opensource.png`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/logo/icon.png` & `fixit-2.0.0b1/docs/_static/logo/icon.png`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/logo/icon.svg` & `fixit-2.0.0b1/docs/_static/logo/icon.svg`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/logo/icon_whilte.png` & `fixit-2.0.0b1/docs/_static/logo/icon_whilte.png`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/logo/icon_white.svg` & `fixit-2.0.0b1/docs/_static/logo/icon_white.svg`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/logo/logo.png` & `fixit-2.0.0b1/docs/_static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/logo/logo.svg` & `fixit-2.0.0b1/docs/_static/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/logo/logo_whilte.png` & `fixit-2.0.0b1/docs/_static/logo/logo_whilte.png`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_static/logo/logo_white.svg` & `fixit-2.0.0b1/docs/_static/logo/logo_white.svg`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/_templates/meta.html` & `fixit-2.0.0b1/docs/_templates/meta.html`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/guide/builtins.rst` & `fixit-2.0.0b1/docs/guide/builtins.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 These rules are all part of the :mod:`fixit.rules` package, and are enabled by default
 unless explicitly listed in the :attr:`disable` configuration option.
 
 - :class:`AvoidOrInExceptRule`
 - :class:`CollapseIsinstanceChecksRule`
 - :class:`ComparePrimitivesByEqualRule`
 - :class:`CompareSingletonPrimitivesByIsRule`
+- :class:`DeprecatedUnittestAssertsRule`
 - :class:`ExplicitFrozenDataclassRule`
-- :class:`NoAssertEqualsRule`
 - :class:`NoAssertTrueForComparisonsRule`
 - :class:`NoInheritFromObjectRule`
 - :class:`NoNamedTupleRule`
 - :class:`NoRedundantArgumentsSuperRule`
 - :class:`NoRedundantFStringRule`
 - :class:`NoRedundantLambdaRule`
 - :class:`NoRedundantListComprehensionRule`
@@ -28,14 +28,15 @@
 - :class:`NoStringTypeAnnotationRule`
 - :class:`ReplaceUnionWithOptionalRule`
 - :class:`RewriteToComprehensionRule`
 - :class:`RewriteToLiteralRule`
 - :class:`SortedAttributesRule`
 - :class:`UseAssertInRule`
 - :class:`UseAssertIsNotNoneRule`
+- :class:`UseAsyncSleepInAsyncDefRule`
 - :class:`UseClassNameAsCodeRule`
 - :class:`UseClsInClassmethodRule`
 - :class:`UseFstringRule`
 - :class:`UseLintFixmeCommentRule`
 - :class:`UseTypesFromTypingRule`
 
 .. class:: AvoidOrInExceptRule
@@ -232,14 +233,53 @@
         .. code:: python
 
             x != False
 
             # suggested fix
             x is not False
 
+.. class:: DeprecatedUnittestAssertsRule
+
+    Discourages the use of various deprecated unittest.TestCase functions
+
+    See https://docs.python.org/3/library/unittest.html#deprecated-aliases
+    
+
+    .. attribute:: MESSAGE
+
+        {deprecated} is deprecated, use {replacement} instead
+    .. attribute:: AUTOFIX
+        :type: Yes
+
+
+    .. attribute:: VALID
+
+        .. code:: python
+
+            self.assertEqual(a, b)
+        .. code:: python
+
+            self.assertNotEqual(a, b)
+
+    .. attribute:: INVALID
+
+        .. code:: python
+
+            self.assertEquals(a, b)
+
+            # suggested fix
+            self.assertEqual(a, b)
+
+        .. code:: python
+
+            self.assertNotEquals(a, b)
+
+            # suggested fix
+            self.assertNotEqual(a, b)
+
 .. class:: ExplicitFrozenDataclassRule
 
     Encourages the use of frozen dataclass objects by telling users to specify the
     kwarg.
 
     Without this lint rule, most users of dataclass won't know to use the kwarg, and
     may unintentionally end up with mutable objects.
@@ -288,43 +328,14 @@
             class Cls: pass
 
             # suggested fix
             from dataclasses import dataclass
             @dataclass(frozen=True)  # called as a function, no kwargs
             class Cls: pass
 
-.. class:: NoAssertEqualsRule
-
-    Discourages use of ``assertEquals`` as it is deprecated (see https://docs.python.org/2/library/unittest.html#deprecated-aliases
-    and https://bugs.python.org/issue9424). Use the standardized ``assertEqual`` instead.
-    
-
-    .. attribute:: MESSAGE
-
-        "assertEquals" is deprecated, use "assertEqual" instead.
-        See https://docs.python.org/2/library/unittest.html#deprecated-aliases and https://bugs.python.org/issue9424.
-    .. attribute:: AUTOFIX
-        :type: Yes
-
-
-    .. attribute:: VALID
-
-        .. code:: python
-
-            self.assertEqual(a, b)
-
-    .. attribute:: INVALID
-
-        .. code:: python
-
-            self.assertEquals(a, b)
-
-            # suggested fix
-            self.assertEqual(a, b)
-
 .. class:: NoAssertTrueForComparisonsRule
 
     Finds incorrect use of ``assertTrue`` when the intention is to compare two values.
     These calls are replaced with ``assertEqual``.
     Comparisons with True, False and None are replaced with one-argument
     calls to ``assertTrue``, ``assertFalse`` and ``assertIsNone``.
     
@@ -973,14 +984,48 @@
         .. code:: python
 
             self.assertTrue(not x is None)
 
             # suggested fix
             self.assertIsNotNone(x)
 
+.. class:: UseAsyncSleepInAsyncDefRule
+
+    Detect if asyncio.sleep is used in an async function
+    
+
+    .. attribute:: MESSAGE
+
+        Use asyncio.sleep in async function
+
+    .. attribute:: VALID
+
+        .. code:: python
+
+            import time
+            def func():
+                time.sleep(1)
+        .. code:: python
+
+            from time import sleep
+            def func():
+                sleep(1)
+
+    .. attribute:: INVALID
+
+        .. code:: python
+
+            import time
+            async def func():
+                time.sleep(1)
+        .. code:: python
+
+            from time import sleep
+            async def func():
+                sleep(1)
 .. class:: UseClassNameAsCodeRule
 
     Meta lint rule which checks that codes of lint rules are migrated to new format in lint rule class definitions.
     
 
     .. attribute:: MESSAGE
 
@@ -1174,21 +1219,24 @@
 
             (
              1,
              2,  # noqa
             )
 .. class:: UseTypesFromTypingRule
 
-    Enforces the use of types from the ``typing`` module in type annotations in place of ``builtins.{builtin_type}``
-    since the type system doesn't recognize the latter as a valid type.
+    Enforces the use of types from the ``typing`` module in type annotations in place
+    of ``builtins.{builtin_type}`` since the type system doesn't recognize the latter
+    as a valid type before Python ``3.10``.
     
 
     .. attribute:: AUTOFIX
         :type: Yes
 
+    .. attribute:: PYTHON_VERSION
+        :type: '< 3.10'
 
     .. attribute:: VALID
 
         .. code:: python
 
             def fuction(list: List[str]) -> None:
                 pass
```

### Comparing `fixit-2.0.0a1/docs/guide/configuration.rst` & `fixit-2.0.0b1/docs/guide/configuration.rst`

 * *Files 20% similar despite different names*

```diff
@@ -40,48 +40,84 @@
 .. attribute:: enable
     :type: list[str]
     :value: []
 
     List of modules or individual rules to enable when linting files covered
     by this configuration.
 
+    Rules bundled with Fixit, or available in the environment's site-packages,
+    can be referenced as a group by their fully-qualified package name, or
+    individually by adding a colon and the rule name:
+
+    .. code-block:: toml
+
+        enable = [
+            "fixit.rules",  # all lint rules in this package (non-recursive)
+            "fixit.rules:UseFstringRule",  # single lint rule by name
+        ]
+
+    Local rules, available only in the repo being linted, can be referenced by
+    their locally-qualified package names, as if they were being imported from
+    a Python module *relative to the configuration file specifying the rule*:
+
+    .. code-block:: toml
+
+        # teambread/fixit.toml
+        enable = [
+            ".rules",  # all rules in teambread/rules/ (non-recursive)
+            ".rules.hollywood",  # all rules in teambread/rules/hollywood.py
+            ".rules:HollywoodNameRule",  # single lint rule by name
+        ]
+
     Overrides disabled rules from any configuration further up the hierarchy.
 
-    If no rules are explicitly enabled, Fixit will enable the ``fixit.rules``
-    module by default.
+    Fixit will enable the built-in :mod:`fixit.rules` lint rules by default.
 
 .. attribute:: disable
     :type: list[str]
     :value: []
 
     List of modules or individual rules to disable when linting files covered
     by this configuration.
 
     Overrides enabled rules from this file, as well any configuration files
     further up the hierarchy.
 
+    See :attr:`enable` for details on referencing lint rules.
+
+.. attribute:: python-version
+    :type: str
+    :value: "3.10"
+
+    Python version to target when selecting lint rules. Rules with
+    :attr:`~fixit.LintRule.PYTHON_VERSION` specifiers that don't match this
+    target version will be automatically disabled during linting.
+    
+    Defaults to the currently active version of Python.
+    Set to empty string ``""`` to disable target version checking.
+
 
 ``[tool.fixit.options]``
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The ``options`` table allows setting options for individual lint rules,
 by mapping the fully-qualified rule name to a dictionary of key/value pairs:
 
 .. code-block:: toml
 
     [tool.fixit.options]
-    "fixit.rules.ExampleRule" = {greeting = "hello world"}
+    "fixit.rules:ExampleRule" = {greeting = "hello world"}
 
 Alternatively, for rules with a large number of options, the rule name can
 be included in the table name for easier usage. Note that the quotes in the
 table name are required for correctly specifying options:
 
 .. code-block:: toml
 
-    [tool.fixit.options."fixit.rules.ExampleRule"]
+    [tool.fixit.options."fixit.rules:ExampleRule"]
     greeting = "hello world"
     answer = 42
 
 
 .. _overrides:
 
 ``[[tool.fixit.overrides]]``
@@ -92,16 +128,16 @@
 `array of tables <https://toml.io/en/v1.0.0#array-of-tables>`_, with each table
 defining the subpath it applies to, along with any values from the tables above:
 
 .. code-block:: toml
 
     [[tool.fixit.overrides]]
     path = "foo/bar"
-    disable = ["fixit.rules.ExampleRule"]
+    disable = ["fixit.rules:ExampleRule"]
 
     [[tool.fixit.overrides.options]]
     # applies to the above override path only
-    "fixit.rules.Story" = {closing = "goodnight moon"}
+    "fixit.rules:Story" = {closing = "goodnight moon"}
 
     [[tool.fixit.overrides]]
     path = "fizz/buzz"
-    enable = ["plugin.SomethingNeat"]
+    enable = ["plugin:SomethingNeat"]
```

### Comparing `fixit-2.0.0a1/docs/guide/integrations.rst` & `fixit-2.0.0b1/docs/guide/integrations.rst`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/proposals/fp1.md` & `fixit-2.0.0b1/docs/proposals/fp1.md`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/docs/proposals/fp2.rst` & `fixit-2.0.0b1/docs/proposals/fp2.rst`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/scripts/check_copyright.py` & `fixit-2.0.0b1/scripts/check_copyright.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/scripts/document_rules.py` & `fixit-2.0.0b1/scripts/document_rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,18 @@
 {{ indent(rule.MESSAGE, "        ") }}
 {% endif %}
 {% if rule.AUTOFIX %}
     .. attribute:: AUTOFIX
         :type: Yes
 
 {% endif %}
+{% if rule.PYTHON_VERSION %}
+    .. attribute:: PYTHON_VERSION
+        :type: {{ repr(rule.PYTHON_VERSION) }}
+{% endif %}
 
     .. attribute:: VALID
 
 {% for case in rule.VALID[:2] %}
         .. code:: python
 
 {{ redent(case.code, "            ") }}
```

### Comparing `fixit-2.0.0a1/scripts/migrate_rule_to_fixit2.py` & `fixit-2.0.0b1/scripts/migrate_rule_to_fixit2.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/__init__.py` & `fixit-2.0.0b1/src/fixit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,16 +11,18 @@
 from .api import fixit_bytes, fixit_file, fixit_paths, print_result
 from .ftypes import (
     CodePosition,
     CodeRange,
     Config,
     FileContent,
     LintViolation,
+    Options,
     QualifiedRule,
     Result,
+    Tags,
 )
 from .rule import CSTLintRule, CstLintRule, LintRule
 from .testing import InvalidTestCase, ValidTestCase
 
 __all__ = [
     "__version__",
     "fixit_bytes",
@@ -31,12 +33,14 @@
     "CstLintRule",
     "LintRule",
     "LintViolation",
     "InvalidTestCase",
     "ValidTestCase",
     "Config",
     "FileContent",
+    "Options",
     "QualifiedRule",
     "Result",
+    "Tags",
     "CodeRange",
     "CodePosition",
 ]
```

### Comparing `fixit-2.0.0a1/src/fixit/api.py` & `fixit-2.0.0b1/src/fixit/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import click
 import trailrunner
 from moreorless.click import echo_color_precomputed_diff
 
 from .config import collect_rules, generate_config
 from .engine import LintRunner
-from .ftypes import Config, FileContent, LintViolation, Result
+from .ftypes import Config, FileContent, LintViolation, Options, Result
 
 LOG = logging.getLogger(__name__)
 
 
 def print_result(result: Result, show_diff: bool = False) -> int:
     """
     Print linting results in a simple format designed for human eyes.
@@ -79,15 +79,15 @@
     violations. Use ``generator.send(...)`` with a boolean value to apply individual
     fixes for each violation.
 
     If ``autofix`` is ``True``, all violations with replacements will be applied
     automatically, even if ``False`` is sent back to the generator.
     """
     try:
-        rules = collect_rules(config.enable, config.disable)
+        rules = collect_rules(config)
         runner = LintRunner(path, content)
         pending_fixes: List[LintViolation] = []
 
         clean = True
         for violation in runner.collect_violations(rules, config):
             clean = False
             fix = yield Result(path, violation)
@@ -109,14 +109,15 @@
     return None
 
 
 def fixit_file(
     path: Path,
     *,
     autofix: bool = False,
+    options: Optional[Options] = None,
 ) -> Generator[Result, bool, None]:
     """
     Lint a single file on disk, detecting and generating appropriate configuration.
 
     Generates a merged :ref:`configuration` based on all applicable config files.
     Reads file from disk as raw bytes, and uses :func:`fixit_bytes` to lint and apply
     any fixes to the content. Writes content back to disk if changes are detected.
@@ -125,38 +126,41 @@
     empty result if the file is clean.
     See :func:`fixit_bytes` for semantics.
     """
     path = path.resolve()
 
     try:
         content: FileContent = path.read_bytes()
-        config = generate_config(path)
+        config = generate_config(path, options=options)
 
         updated = yield from fixit_bytes(path, content, config=config, autofix=autofix)
         if updated and updated != content:
             LOG.info(f"{path}: writing changes to file")
             path.write_bytes(updated)
 
     except Exception as error:
         LOG.debug("Exception while fixit_file", exc_info=error)
         yield Result(path, violation=None, error=(error, traceback.format_exc()))
 
 
-def _fixit_file_wrapper(path: Path, *, autofix: bool = False) -> List[Result]:
+def _fixit_file_wrapper(
+    path: Path, *, autofix: bool = False, options: Optional[Options] = None
+) -> List[Result]:
     """
     Wrapper because generators can't be pickled or used directly via multiprocessing
     TODO: replace this with some sort of queue or whatever
     """
-    return list(fixit_file(path, autofix=autofix))
+    return list(fixit_file(path, autofix=autofix, options=options))
 
 
 def fixit_paths(
     paths: Iterable[Path],
     *,
     autofix: bool = False,
+    options: Optional[Options] = None,
     parallel: bool = True,
 ) -> Generator[Result, bool, None]:
     """
     Lint multiple files or directories, recursively expanding each path.
 
     Walks all paths given, obeying any ``.gitignore`` exclusions, finding Python source
     files. Lints each file found using :func:`fixit_file`, using a process pool when
@@ -177,12 +181,12 @@
 
     expanded_paths: List[Path] = []
     for path in paths:
         expanded_paths.extend(trailrunner.walk(path))
 
     if len(expanded_paths) == 1 or not parallel:
         for path in expanded_paths:
-            yield from fixit_file(path, autofix=autofix)
+            yield from fixit_file(path, autofix=autofix, options=options)
     else:
-        fn = partial(_fixit_file_wrapper, autofix=autofix)
+        fn = partial(_fixit_file_wrapper, autofix=autofix, options=options)
         for _, results in trailrunner.run_iter(expanded_paths, fn):
             yield from results
```

### Comparing `fixit-2.0.0a1/src/fixit/cli.py` & `fixit-2.0.0b1/src/fixit/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
 import sys
+import unittest
 from pathlib import Path
-from typing import Optional, Sequence, Set
+from typing import Dict, Optional, Sequence, Set, Type
 
 import click
 
 from fixit import __version__
 
 from .api import fixit_paths, print_result
-from .config import collect_rules, generate_config
-from .ftypes import Options
+from .config import collect_rules, generate_config, parse_rule
+from .ftypes import Config, Options, Tags
+from .rule import LintRule
+from .testing import generate_lint_rule_test_cases
 from .util import capture
 
 
 def splash(
     visited: Set[Path], dirty: Set[Path], autofixes: int = 0, fixed: int = 0
 ) -> None:
     def f(v: int) -> str:
@@ -53,27 +56,35 @@
 @click.option(
     "--config-file",
     "-c",
     type=click.Path(dir_okay=False, exists=True, path_type=Path),
     default=None,
     help="Override default config file search behavior",
 )
+@click.option(
+    "--tags",
+    type=str,
+    default="",
+    help="Select or filter rules by tags",
+)
 def main(
     ctx: click.Context,
     debug: Optional[bool],
     config_file: Optional[Path],
+    tags: str,
 ):
     level = logging.WARNING
     if debug is not None:
         level = logging.DEBUG if debug else logging.ERROR
     logging.basicConfig(level=level, stream=sys.stderr)
 
     ctx.obj = Options(
         debug=debug,
         config_file=config_file,
+        tags=Tags.parse(tags),
     )
 
 
 @main.command()
 @click.pass_context
 @click.option("--diff", "-d", is_flag=True, help="Show diff of suggested changes")
 @click.argument("paths", nargs=-1, type=click.Path(path_type=Path))
@@ -81,22 +92,24 @@
     ctx: click.Context,
     diff: bool,
     paths: Sequence[Path],
 ):
     """
     lint one or more paths and return suggestions
     """
+    options: Options = ctx.obj
+
     if not paths:
         paths = [Path.cwd()]
 
     exit_code = 0
     visited: Set[Path] = set()
     dirty: Set[Path] = set()
     autofixes = 0
-    for result in fixit_paths(paths):
+    for result in fixit_paths(paths, options=options):
         visited.add(result.path)
 
         if print_result(result, show_diff=diff):
             dirty.add(result.path)
             if result.violation:
                 exit_code |= 1
                 if result.violation.autofixable:
@@ -124,27 +137,31 @@
     interactive: bool,
     diff: bool,
     paths: Sequence[Path],
 ):
     """
     lint and autofix one or more files and return results
     """
+    options: Options = ctx.obj
+
     if not paths:
         paths = [Path.cwd()]
 
     autofix = not interactive
     exit_code = 0
 
     visited: Set[Path] = set()
     dirty: Set[Path] = set()
     autofixes = 0
     fixed = 0
 
     # TODO: make this parallel
-    generator = capture(fixit_paths(paths, autofix=autofix, parallel=False))
+    generator = capture(
+        fixit_paths(paths, autofix=autofix, options=options, parallel=False)
+    )
     for result in generator:
         visited.add(result.path)
         if print_result(result, show_diff=interactive or diff):
             dirty.add(result.path)
             if autofix and result.violation and result.violation.autofixable:
                 autofixes += 1
                 fixed += 1
@@ -161,28 +178,59 @@
 
     splash(visited, dirty, autofixes, fixed)
     ctx.exit(exit_code)
 
 
 @main.command()
 @click.pass_context
+@click.argument("rules", nargs=-1, required=True, type=str)
+def test(ctx: click.Context, rules: Sequence[str]):
+    """
+    test lint rules and their VALID/INVALID cases
+    """
+    qual_rules = [parse_rule(rule, Path.cwd().resolve()) for rule in rules]
+    lint_rules = collect_rules(
+        Config(enable=qual_rules, disable=[], python_version=None)
+    )
+    test_cases = generate_lint_rule_test_cases(lint_rules)
+
+    test_suite = unittest.TestSuite()
+    loader = unittest.TestLoader()
+    for test_case in test_cases:
+        test_suite.addTest(loader.loadTestsFromTestCase(test_case))
+
+    runner = unittest.TextTestRunner(verbosity=2)
+    result = runner.run(test_suite)
+    if not result.wasSuccessful():
+        ctx.exit(1)
+
+
+@main.command()
+@click.pass_context
 @click.argument("paths", nargs=-1, type=click.Path(exists=True, path_type=Path))
 def debug(ctx: click.Context, paths: Sequence[Path]):
     """
     print materialized configuration for paths
     """
+    options: Options = ctx.obj
+
     if not paths:
         paths = [Path.cwd()]
 
     try:
         from rich import print as pprint
     except ImportError:
         from pprint import pprint  # type: ignore
 
     for path in paths:
         path = path.resolve()
-        config = generate_config(path)
-        rules = collect_rules(config.enable, config.disable)
+        config = generate_config(path, options=options)
+        disabled: Dict[Type[LintRule], str] = {}
+        enabled = collect_rules(config, debug_reasons=disabled)
 
         pprint(">>> ", path)
         pprint(config)
-        pprint(rules)
+        pprint("enabled:", sorted(str(rule) for rule in enabled))
+        pprint(
+            "disabled:",
+            sorted(f"{rule()} ({reason})" for rule, reason in disabled.items()),
+        )
```

### Comparing `fixit-2.0.0a1/src/fixit/config.py` & `fixit-2.0.0b1/src/fixit/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import importlib
 import inspect
 import logging
 import pkgutil
+import platform
 import sys
 from contextlib import contextmanager
-from dataclasses import replace
 from pathlib import Path
 from types import ModuleType
 from typing import (
     Any,
     Collection,
     Dict,
     Iterable,
@@ -22,18 +22,23 @@
     Mapping,
     Optional,
     Sequence,
     Set,
     Type,
 )
 
+from packaging.specifiers import SpecifierSet
+
+from packaging.version import InvalidVersion, Version
+
 from .ftypes import (
     Config,
     is_collection,
     is_sequence,
+    Options,
     QualifiedRule,
     QualifiedRuleRegex,
     RawConfig,
     RuleOptionsTable,
     RuleOptionTypes,
     T,
 )
@@ -47,15 +52,15 @@
 FIXIT_CONFIG_FILENAMES = ("fixit.toml", ".fixit.toml", "pyproject.toml")
 FIXIT_LOCAL_MODULE = "fixit.local"
 
 log = logging.getLogger(__name__)
 
 
 class ConfigError(ValueError):
-    def __init__(self, msg: str, config: RawConfig):
+    def __init__(self, msg: str, config: Optional[RawConfig] = None):
         super().__init__(msg)
         self.config = config
 
 
 class CollectionError(RuntimeError):
     def __init__(self, msg: str, rule: QualifiedRule):
         super().__init__(msg)
@@ -182,30 +187,53 @@
                 mod = importlib.import_module(f".{module_name}", module.__name__)
                 rules.update(walk_module(mod))
 
     return rules
 
 
 def collect_rules(
-    enables: Collection[QualifiedRule], disables: Collection[QualifiedRule]
+    config: Config,
+    *,
+    # out-param to capture reasons when disabling rules for debugging
+    debug_reasons: Optional[Dict[Type[LintRule], str]] = None,
 ) -> Collection[LintRule]:
     """
     Import and return rules specified by `enables` and `disables`.
     """
 
-    final_rules: Set[Type[LintRule]] = set()
-    for qualified_rule in enables:
-        matched_rules = list(find_rules(qualified_rule))
-        final_rules.update(matched_rules)
-
-    for qualified_rule in disables:
-        matched_rules = list(find_rules(qualified_rule))
-        final_rules.difference_update(matched_rules)
+    all_rules: Set[Type[LintRule]] = set()
+    if debug_reasons is not None:
+        disabled_rules = debug_reasons
+    else:
+        disabled_rules = {}
+
+    for qualified_rule in config.enable:
+        all_rules |= set(find_rules(qualified_rule))
 
-    return [R() for R in final_rules]
+    for qualified_rule in config.disable:
+        disabled_rules.update({r: "disabled" for r in find_rules(qualified_rule)})
+        all_rules -= set(disabled_rules)
+
+    if config.tags:
+        disabled_rules.update(
+            {R: "tags" for R in all_rules if R.TAGS not in config.tags}
+        )
+        all_rules -= set(disabled_rules)
+
+    if config.python_version is not None:
+        disabled_rules.update(
+            {
+                R: "python_version"
+                for R in all_rules
+                if config.python_version not in SpecifierSet(R.PYTHON_VERSION)
+            }
+        )
+        all_rules -= set(disabled_rules)
+
+    return [R() for R in all_rules]
 
 
 def locate_configs(path: Path, root: Optional[Path] = None) -> List[Path]:
     """
     Given a file path, locate all relevant config files in priority order.
 
     Walking upward from target path, creates a list of candidate paths that exist
@@ -306,80 +334,106 @@
                 )
 
             rule_configs[rule_name][key] = value
 
     return rule_configs
 
 
+def parse_rule(
+    rule: str, root: Path, config: Optional[RawConfig] = None
+) -> QualifiedRule:
+    """
+    Given a raw rule string, parse and return a QualifiedRule object
+    """
+    if not (match := QualifiedRuleRegex.match(rule)):
+        raise ConfigError(f"invalid rule name {rule!r}", config=config)
+
+    group = match.groupdict()
+    module = group["module"]
+    name = group["name"]
+    local = group["local"]
+
+    if local:
+        return QualifiedRule(module, name, local, root)
+    else:
+        return QualifiedRule(module, name)
+
+
 def merge_configs(
     path: Path, raw_configs: List[RawConfig], root: Optional[Path] = None
 ) -> Config:
     """
     Given multiple raw configs, merge them in priority order.
 
     Assumes raw_configs are given in order from highest to lowest priority.
     """
 
     config: RawConfig
     enable_rules: Set[QualifiedRule] = {QualifiedRule("fixit.rules")}
     disable_rules: Set[QualifiedRule] = set()
     rule_options: RuleOptionsTable = {}
+    target_python_version: Optional[Version] = Version(platform.python_version())
 
     def process_subpath(
         subpath: Path,
         *,
         enable: Sequence[str] = (),
         disable: Sequence[str] = (),
         options: Optional[RuleOptionsTable] = None,
+        python_version: Any = None,
     ):
+        nonlocal target_python_version
+
         subpath = subpath.resolve()
         try:
             path.relative_to(subpath)
         except ValueError:  # not relative to subpath
             return
 
+        config_dir = config.path.parent
         for rule in enable:
-            if not (match := QualifiedRuleRegex.match(rule)):
-                raise ConfigError(f"invalid rule name {rule!r}", config=config)
-
-            group = match.groupdict()
-            qual_rule = QualifiedRule(module=group["module"], name=group["name"], local=group["local"])  # type: ignore
-
-            if qual_rule.local:
-                qual_rule = replace(qual_rule, root=subpath)
-
+            qual_rule = parse_rule(rule, config_dir, config)
             enable_rules.add(qual_rule)
             disable_rules.discard(qual_rule)
 
         for rule in disable:
-            if not (match := QualifiedRuleRegex.match(rule)):
-                raise ConfigError(f"invalid rule name {rule!r}", config=config)
-
-            group = match.groupdict()
-            qual_rule = QualifiedRule(module=group["module"], name=group["name"], local=group["local"])  # type: ignore
-
+            qual_rule = parse_rule(rule, config_dir, config)
             enable_rules.discard(qual_rule)
             disable_rules.add(qual_rule)
 
         if options:
             rule_options.update(options)
 
+        if python_version is not None:
+            if python_version:
+                try:
+                    target_python_version = Version(python_version)
+                except InvalidVersion:
+                    raise ConfigError(
+                        f"'python_version' {python_version!r} is not valid",
+                        config=config,
+                    )
+
+            else:  # disable versioning, aka python_version = ""
+                target_python_version = None
+
     for config in reversed(raw_configs):
         if root is None:
             root = config.path.parent
 
         data = config.data
         if data.pop("root", False):
             root = config.path.parent
 
         process_subpath(
             config.path.parent,
             enable=get_sequence(config, "enable"),
             disable=get_sequence(config, "disable"),
             options=get_options(config, "options"),
+            python_version=config.data.pop("python_version", None),
         )
 
         for override in get_sequence(config, "overrides"):
             if not isinstance(override, dict):
                 raise ConfigError("'overrides' requires array of tables", config=config)
 
             subpath = override.get("path", None)
@@ -390,33 +444,46 @@
 
             subpath = config.path.parent / subpath
             process_subpath(
                 subpath,
                 enable=get_sequence(config, "enable", data=override),
                 disable=get_sequence(config, "disable", data=override),
                 options=get_options(config, "options", data=override),
+                python_version=override.pop("python_version", None),
             )
 
         for key in data.keys():
             log.warning("unknown configuration option %r", key)
 
     return Config(
         path=path,
         root=root or Path(path.anchor),
         enable=sorted(enable_rules),
         disable=sorted(disable_rules),
         options=rule_options,
+        python_version=target_python_version,
     )
 
 
-def generate_config(path: Path, root: Optional[Path] = None) -> Config:
+def generate_config(
+    path: Path, root: Optional[Path] = None, *, options: Optional[Options] = None
+) -> Config:
     """
     Given a file path, walk upwards looking for and applying cascading configs
     """
     path = path.resolve()
 
     if root is not None:
         root = root.resolve()
 
-    config_paths = locate_configs(path, root=root)
+    if options and options.config_file:
+        config_paths = [options.config_file]
+    else:
+        config_paths = locate_configs(path, root=root)
+
     raw_configs = read_configs(config_paths)
-    return merge_configs(path, raw_configs, root=root)
+    config = merge_configs(path, raw_configs, root=root)
+
+    if options and options.tags:
+        config.tags = options.tags
+
+    return config
```

### Comparing `fixit-2.0.0a1/src/fixit/engine.py` & `fixit-2.0.0b1/src/fixit/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,19 +7,26 @@
 import time
 from collections import defaultdict
 from contextlib import contextmanager
 from dataclasses import replace
 from pathlib import Path
 from typing import Collection, Iterable, Iterator, Mapping, Optional, Set
 
-from libcst import Module, parse_module
+from libcst import CSTNode, CSTTransformer, Module, parse_module
 from libcst.metadata import FullRepoManager, MetadataWrapper, ProviderT
 from moreorless import unified_diff
 
-from .ftypes import Config, FileContent, LintViolation, Timings, TimingsHook
+from .ftypes import (
+    Config,
+    FileContent,
+    LintViolation,
+    NodeReplacement,
+    Timings,
+    TimingsHook,
+)
 from .rule import LintRule
 
 LOG = logging.getLogger(__name__)
 
 
 class LintRunner:
     def __init__(self, path: Path, source: FileContent) -> None:
@@ -101,13 +108,22 @@
 
         return count
 
     def apply_replacements(self, violations: Collection[LintViolation]) -> FileContent:
         """
         Apply any autofixes to the module, and return the resulting source code.
         """
-        for violation in violations:
-            if violation.replacement:
-                self.module = self.module.deep_replace(
-                    violation.node, violation.replacement  # type:ignore # LibCST#906
-                )
-        return self.module.bytes
+        replacements = {v.node: v.replacement for v in violations if v.replacement}
+
+        class ReplacementTransformer(CSTTransformer):
+            def on_visit(self, node: CSTNode) -> bool:
+                # don't visit children if we're going to replace the parent anyways
+                return node not in replacements
+
+            def on_leave(self, node: CSTNode, updated: CSTNode) -> NodeReplacement:
+                if node in replacements:
+                    new = replacements[node]
+                    return new
+                return updated
+
+        updated = self.module.visit(ReplacementTransformer())
+        return updated.bytes
```

### Comparing `fixit-2.0.0a1/src/fixit/ftypes.py` & `fixit-2.0.0b1/src/fixit/rules/replace_union_with_optional.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,173 +1,128 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-import re
-from dataclasses import dataclass, field
-from pathlib import Path
-from typing import (
-    Any,
-    Callable,
-    ContextManager,
-    Dict,
-    Iterable,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    TypedDict,
-    TypeVar,
-    Union,
-)
-
-from libcst import CSTNode, FlattenSentinel, RemovalSentinel
-from libcst._add_slots import add_slots
-from libcst.metadata import CodePosition as CodePosition, CodeRange as CodeRange
-
-T = TypeVar("T")
-
-CodeRange
-CodePosition
-
-FileContent = bytes
-RuleOptionTypes = (str, int, float)
-RuleOptions = Dict[str, Union[str, int, float]]
-RuleOptionsTable = Dict[str, RuleOptions]
-
-NodeReplacement = Union[CSTNode, FlattenSentinel, RemovalSentinel]
-
-Timings = Dict[str, int]
-TimingsHook = Callable[[Timings], None]
-
-VisitorMethod = Callable[[CSTNode], None]
-VisitHook = Callable[[str], ContextManager]
-
-
-@dataclass(frozen=True)
-class InvalidTestCase:
-    code: str
-    range: Optional[CodeRange] = None
-    expected_message: Optional[str] = None
-    expected_replacement: Optional[str] = None
-
-
-@dataclass(frozen=True)
-class ValidTestCase:
-    code: str
-
-
-QualifiedRuleRegex = re.compile(
-    r"""
-    ^
-    (?P<module>
-        (?P<local>\.)?
-        [a-zA-Z0-9_]+(\.[a-zA-Z0-9_]+)*
-    )
-    (?::(?P<name>[a-zA-Z0-9_]+))?
-    $
-    """,
-    re.VERBOSE,
-)
-
-
-class QualifiedRuleRegexResult(TypedDict):
-    module: str
-    name: Optional[str]
-    local: Optional[str]
-
-
-def is_sequence(value: Any) -> bool:
-    return isinstance(value, Sequence) and not isinstance(value, (str, bytes))
-
-
-def is_collection(value: Any) -> bool:
-    return isinstance(value, Iterable) and not isinstance(value, (str, bytes))
-
-
-@dataclass(frozen=True)
-class QualifiedRule:
-    module: str
-    name: Optional[str] = None
-    local: Optional[str] = None
-    root: Optional[Path] = field(default=None, hash=False, compare=False)
-
-    def __str__(self) -> str:
-        return self.module + (f":{self.name}" if self.name else "")
-
-    def __lt__(self, other: object) -> bool:
-        if isinstance(other, QualifiedRule):
-            return str(self) < str(other)
-        return NotImplemented
-
-
-@dataclass
-class Options:
-    """
-    Command-line options to affect runtime behavior
-    """
+import libcst as cst
+import libcst.matchers as m
 
-    debug: Optional[bool]
-    config_file: Optional[Path]
+from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
-@dataclass
-class Config:
+class ReplaceUnionWithOptionalRule(CstLintRule):
     """
-    Materialized configuration valid for processing a single file.
+    Enforces the use of ``Optional[T]`` over ``Union[T, None]`` and ``Union[None, T]``.
+    See https://docs.python.org/3/library/typing.html#typing.Optional to learn more about Optionals.
     """
 
-    path: Path = field(default_factory=Path)
-    root: Path = field(default_factory=Path.cwd)
-
-    enable: List[QualifiedRule] = field(
-        default_factory=lambda: [QualifiedRule("fixit.rules")]
+    MESSAGE: str = (
+        "`Optional[T]` is preferred over `Union[T, None]` or `Union[None, T]`. "
+        + "Learn more: https://docs.python.org/3/library/typing.html#typing.Optional"
     )
-    disable: List[QualifiedRule] = field(default_factory=list)
-    options: RuleOptionsTable = field(default_factory=dict)
-
-    def __post_init__(self):
-        self.path = self.path.resolve()
-        self.root = self.root.resolve()
-
-
-@dataclass
-class RawConfig:
-    path: Path
-    data: Dict[str, Any]
-
-    def __post_init__(self):
-        self.path = self.path.resolve()
-
-
-@add_slots
-@dataclass(frozen=True)
-class LintViolation:
-    """
-    An individual lint error, with an optional replacement and expected diff.
-    """
-
-    rule_name: str
-    range: CodeRange
-    message: str
-    node: CSTNode
-    replacement: Optional[NodeReplacement]
-    diff: str = ""
-
-    @property
-    def autofixable(self) -> bool:
-        """
-        Whether the violation includes a suggested replacement.
-        """
-        return bool(self.replacement)
-
-
-@dataclass
-class Result:
-    """
-    A single lint result for a given file and lint rule.
-    """
-
-    path: Path
-    violation: Optional[LintViolation]
-    error: Optional[Tuple[Exception, str]] = None
+    METADATA_DEPENDENCIES = (cst.metadata.ScopeProvider,)
+    VALID = [
+        Valid(
+            """
+            def func() -> Optional[str]:
+                pass
+            """
+        ),
+        Valid(
+            """
+            def func() -> Optional[Dict]:
+                pass
+            """
+        ),
+        Valid(
+            """
+            def func() -> Union[str, int, None]:
+                pass
+            """
+        ),
+    ]
+    INVALID = [
+        Invalid(
+            """
+            def func() -> Union[str, None]:
+                pass
+            """,
+        ),
+        Invalid(
+            """
+            from typing import Optional
+            def func() -> Union[Dict[str, int], None]:
+                pass
+            """,
+            expected_replacement="""
+            from typing import Optional
+            def func() -> Optional[Dict[str, int]]:
+                pass
+            """,
+        ),
+        Invalid(
+            """
+            from typing import Optional
+            def func() -> Union[str, None]:
+                pass
+            """,
+            expected_replacement="""
+            from typing import Optional
+            def func() -> Optional[str]:
+                pass
+            """,
+        ),
+        Invalid(
+            """
+            from typing import Optional
+            def func() -> Union[Dict, None]:
+                pass
+            """,
+            expected_replacement="""
+            from typing import Optional
+            def func() -> Optional[Dict]:
+                pass
+            """,
+        ),
+    ]
+
+    def leave_Annotation(self, original_node: cst.Annotation) -> None:
+        if self.contains_union_with_none(original_node):
+            scope = self.get_metadata(cst.metadata.ScopeProvider, original_node, None)
+            nones = 0
+            indexes = []
+            replacement = None
+            if scope is not None and "Optional" in scope:
+                for s in cst.ensure_type(original_node.annotation, cst.Subscript).slice:
+                    if m.matches(s, m.SubscriptElement(m.Index(m.Name("None")))):
+                        nones += 1
+                    else:
+                        indexes.append(s.slice)
+                if not (nones > 1) and len(indexes) == 1:
+                    replacement = original_node.with_changes(
+                        annotation=cst.Subscript(
+                            value=cst.Name("Optional"),
+                            slice=(cst.SubscriptElement(indexes[0]),),
+                        )
+                    )
+                    # TODO(T57106602) refactor lint replacement once extract exists
+            self.report(original_node, replacement=replacement)
+
+    def contains_union_with_none(self, node: cst.Annotation) -> bool:
+        return m.matches(
+            node,
+            m.Annotation(
+                m.Subscript(
+                    value=m.Name("Union"),
+                    slice=m.OneOf(
+                        [
+                            m.SubscriptElement(m.Index()),
+                            m.SubscriptElement(m.Index(m.Name("None"))),
+                        ],
+                        [
+                            m.SubscriptElement(m.Index(m.Name("None"))),
+                            m.SubscriptElement(m.Index()),
+                        ],
+                    ),
+                )
+            ),
+        )
```

### Comparing `fixit-2.0.0a1/src/fixit/testing.py` & `fixit-2.0.0b1/src/fixit/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,26 +4,15 @@
 # LICENSE file in the root directory of this source tree.
 
 import re
 import textwrap
 import unittest
 from dataclasses import dataclass
 from pathlib import Path
-from typing import (
-    Any,
-    Callable,
-    Collection,
-    Dict,
-    List,
-    Mapping,
-    Optional,
-    Sequence,
-    Type,
-    Union,
-)
+from typing import Any, Callable, Collection, Dict, List, Mapping, Sequence, Type, Union
 
 from moreorless import unified_diff
 
 from .engine import LintRunner
 from .ftypes import Config
 from .rule import InvalidTestCase, LintRule, ValidTestCase
 
@@ -131,17 +120,15 @@
             # make sure we generated a reasonable diff
             expected_diff = unified_diff(
                 source_code, expected_code, filename=path.name, n=1
             )
             self.assertEqual(expected_diff, report.diff)
 
 
-def _gen_test_methods_for_rule(
-    rule: LintRule, fixture_dir: Path, rules_package: str
-) -> TestCasePrecursor:
+def gen_test_methods_for_rule(rule: LintRule) -> TestCasePrecursor:
     """
     Aggregates all of the cases inside a single LintRule's VALID and INVALID
     attributes and maps them to altered names with a `test_` prefix so that 'unittest'
     can discover them later on and an index postfix so that individual tests can be
     selected from the command line.
     """
     valid_tcs = {}
@@ -167,39 +154,58 @@
     return TestCasePrecursor(
         rule=rule,
         test_methods={**valid_tcs, **invalid_tcs},
         fixture_paths=fixture_paths,
     )
 
 
-def _gen_all_test_methods(
-    rules: Collection[LintRule], fixture_dir: Path, rules_package: str
-) -> Sequence[TestCasePrecursor]:
+def gen_all_test_methods(rules: Collection[LintRule]) -> Sequence[TestCasePrecursor]:
     """
     Converts all passed-in lint rules to type `TestCasePrecursor` to ease further TestCase
     creation later on.
     """
     cases = []
     for rule in rules:
         if not isinstance(rule, LintRule):
             continue
-        test_cases_for_rule = _gen_test_methods_for_rule(
-            rule, fixture_dir, rules_package
-        )
+        test_cases_for_rule = gen_test_methods_for_rule(rule)
         cases.append(test_cases_for_rule)
     return cases
 
 
-def add_lint_rule_tests_to_module(
-    module_attrs: Dict[str, Any],
+def generate_lint_rule_test_cases(
     rules: Collection[LintRule],
-    test_case_type: Type[unittest.TestCase] = LintRuleTestCase,
-    custom_test_method_name: str = "_test_method",
-    fixture_dir: Optional[Path] = None,
-    rules_package: str = "",
+) -> List[Type[unittest.TestCase]]:
+    test_case_classes: List[Type[unittest.TestCase]] = []
+    for test_case in gen_all_test_methods(rules):
+        rule_name = type(test_case.rule).__name__
+        test_methods_to_add: Dict[str, Callable] = {}
+
+        for test_method_name, test_method_data in test_case.test_methods.items():
+
+            def test_method(
+                self: LintRuleTestCase,
+                data: Union[ValidTestCase, InvalidTestCase] = test_method_data,
+                rule: LintRule = test_case.rule,
+            ) -> None:
+                # instantiate a new rule for every test
+                rule_ty = type(rule)
+                return self._test_method(data, rule_ty())
+
+            test_method.__name__ = test_method_name
+            test_methods_to_add[test_method_name] = test_method
+
+        test_case_class = type(rule_name, (LintRuleTestCase,), test_methods_to_add)
+        test_case_classes.append(test_case_class)
+
+    return test_case_classes
+
+
+def add_lint_rule_tests_to_module(
+    module_attrs: Dict[str, Any], rules: Collection[LintRule]
 ) -> None:
     """
     Generates classes inheriting from `unittest.TestCase` from the data available in `rules` and adds these to module_attrs.
     The goal is to facilitate unit test discovery by Python's `unittest` framework. This will provide the capability of
     testing your lint rules by running commands such as `python -m unittest <your testing module name>`.
 
     module_attrs: A dictionary of attributes we want to add these test cases to. If adding to a module, you can pass `globals()` as the argument.
@@ -216,42 +222,17 @@
 
     fixture_dir: The directory in which fixture files for the passed rules live. Necessary only if any lint rules require fixture data for testing.
 
     rules_package: The name of the rules package. This will be used during the search for fixture files and provides insight into the structure of the fixture directory.
     The structure of the fixture directory is automatically assumed to mirror the structure of the rules package, eg: `<rules_package>.submodule.module.rule_class` should
     have fixture files in `<fixture_dir>/submodule/module/rule_class/`.
     """
-    if fixture_dir is not None or rules_package:
-        raise NotImplementedError("fixtures are not implemented in tests yet")
-    if fixture_dir is None:
-        fixture_dir = Path("")
-    test_case_classes: List[Type[unittest.TestCase]] = []
-    for test_case in _gen_all_test_methods(rules, fixture_dir, rules_package):
-        rule_name = type(test_case.rule).__name__
-        test_methods_to_add: Dict[str, Callable] = {}
-
-        for test_method_name, test_method_data in test_case.test_methods.items():
-            fixture_file = test_case.fixture_paths.get(test_method_name)
-
-            def test_method(
-                self: Type[unittest.TestCase],
-                data: Union[ValidTestCase, InvalidTestCase] = test_method_data,
-                rule: LintRule = test_case.rule,
-                fixture_file: Optional[Path] = fixture_file,
-            ) -> None:
-                # instantiate a new rule for every test
-                rule_ty = type(rule)
-                return getattr(self, custom_test_method_name)(data, rule_ty())
-
-            test_method.__name__ = test_method_name
-            test_methods_to_add[test_method_name] = test_method
-
-        test_case_class = type(rule_name, (test_case_type,), test_methods_to_add)
-        test_case_classes.append(test_case_class)
-        module_attrs[rule_name] = test_case_class
+    test_case_classes = generate_lint_rule_test_cases(rules)
+    for test_case_class in test_case_classes:
+        module_attrs[test_case_class.__name__] = test_case_class
 
     # Rewrite the module for each generated test case to match the location calling
     # this function. This enables better integration with test case discovery methods
     # that depend on listing test cases separately from running them.
     if "__package__" in module_attrs:
         test_module = module_attrs.get("__package__")
         assert isinstance(test_module, str)
```

### Comparing `fixit-2.0.0a1/src/fixit/util.py` & `fixit-2.0.0b1/src/fixit/util.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/avoid_or_in_except.py` & `fixit-2.0.0b1/src/fixit/rules/avoid_or_in_except.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/chained_instance_check.py` & `fixit-2.0.0b1/src/fixit/rules/chained_instance_check.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/cls_in_classmethod.py` & `fixit-2.0.0b1/src/fixit/rules/cls_in_classmethod.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/compare_primitives_by_equal.py` & `fixit-2.0.0b1/src/fixit/rules/compare_primitives_by_equal.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/compare_singleton_primitives_by_is.py` & `fixit-2.0.0b1/src/fixit/rules/compare_singleton_primitives_by_is.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/explicit_frozen_dataclass.py` & `fixit-2.0.0b1/src/fixit/rules/explicit_frozen_dataclass.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_assert_true_for_comparison.py` & `fixit-2.0.0b1/src/fixit/rules/no_assert_true_for_comparison.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_inherit_from_object.py` & `fixit-2.0.0b1/src/fixit/rules/no_inherit_from_object.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_namedtuple.py` & `fixit-2.0.0b1/src/fixit/rules/no_namedtuple.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_redundant_arguments_super.py` & `fixit-2.0.0b1/src/fixit/rules/no_redundant_arguments_super.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_redundant_fstring.py` & `fixit-2.0.0b1/src/fixit/rules/no_redundant_fstring.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_redundant_lambda.py` & `fixit-2.0.0b1/src/fixit/rules/no_redundant_lambda.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_redundant_list_comprehension.py` & `fixit-2.0.0b1/src/fixit/rules/no_redundant_list_comprehension.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_static_if_condition.py` & `fixit-2.0.0b1/src/fixit/rules/no_static_if_condition.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/no_string_type_annotation.py` & `fixit-2.0.0b1/src/fixit/rules/no_string_type_annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,11 +294,11 @@
             self.in_literal.remove(original_node)
 
     def visit_SimpleString(self, node: cst.SimpleString) -> None:
         if not self.has_future_annotations_import:
             return
         if self.in_annotation and not self.in_literal:
             # This is not allowed past Python3.7 since it's no longer necessary.
-            self.report(
-                node,
-                replacement=cst.parse_expression(node.evaluated_value),
-            )
+            value = node.evaluated_value
+            if isinstance(value, bytes):
+                value = value.decode("utf-8")
+            self.report(node, replacement=cst.parse_expression(value))
```

### Comparing `fixit-2.0.0a1/src/fixit/rules/replace_union_with_optional.py` & `fixit-2.0.0b1/src/fixit/rules/use_types_from_typing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,128 +1,154 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
-import libcst as cst
-import libcst.matchers as m
+from typing import Set
+
+import libcst
+from libcst.metadata import QualifiedNameProvider, ScopeProvider
 
 from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
-class ReplaceUnionWithOptionalRule(CstLintRule):
+REPLACE_BUILTIN_TYPE_ANNOTATION: str = (
+    "You are using builtins.{builtin_type} as a type annotation "
+    + "but the type system doesn't recognize it as a valid type."
+    + " You should use typing.{correct_type} instead."
+)
+
+BUILTINS_TO_REPLACE: Set[str] = {"dict", "list", "set", "tuple"}
+QUALIFIED_BUILTINS_TO_REPLACE: Set[str] = {f"builtins.{s}" for s in BUILTINS_TO_REPLACE}
+
+
+class UseTypesFromTypingRule(CstLintRule):
     """
-    Enforces the use of ``Optional[T]`` over ``Union[T, None]`` and ``Union[None, T]``.
-    See https://docs.python.org/3/library/typing.html#typing.Optional to learn more about Optionals.
+    Enforces the use of types from the ``typing`` module in type annotations in place
+    of ``builtins.{builtin_type}`` since the type system doesn't recognize the latter
+    as a valid type before Python ``3.10``.
     """
 
-    MESSAGE: str = (
-        "`Optional[T]` is preferred over `Union[T, None]` or `Union[None, T]`. "
-        + "Learn more: https://docs.python.org/3/library/typing.html#typing.Optional"
+    PYTHON_VERSION = "< 3.10"
+
+    METADATA_DEPENDENCIES = (
+        QualifiedNameProvider,
+        ScopeProvider,
     )
-    METADATA_DEPENDENCIES = (cst.metadata.ScopeProvider,)
     VALID = [
         Valid(
             """
-            def func() -> Optional[str]:
+            def fuction(list: List[str]) -> None:
                 pass
             """
         ),
         Valid(
             """
-            def func() -> Optional[Dict]:
-                pass
+            def function() -> None:
+                thing: Dict[str, str] = {}
             """
         ),
         Valid(
             """
-            def func() -> Union[str, int, None]:
-                pass
+            def function() -> None:
+                thing: Tuple[str]
+            """
+        ),
+        Valid(
+            """
+            from typing import Dict, List
+            def function() -> bool:
+                    return Dict == List
+            """
+        ),
+        Valid(
+            """
+            from typing import List as list
+            from graphene import List
+
+            def function(a: list[int]) -> List[int]:
+                    return []
             """
         ),
     ]
     INVALID = [
         Invalid(
             """
-            def func() -> Union[str, None]:
+            from typing import List
+            def whatever(list: list[str]) -> None:
+                pass
+            """,
+            expected_replacement="""
+            from typing import List
+            def whatever(list: List[str]) -> None:
                 pass
             """,
         ),
         Invalid(
             """
-            from typing import Optional
-            def func() -> Union[Dict[str, int], None]:
-                pass
-            """,
-            expected_replacement="""
-            from typing import Optional
-            def func() -> Optional[Dict[str, int]]:
+            def function(list: list[str]) -> None:
                 pass
             """,
         ),
         Invalid(
             """
-            from typing import Optional
-            def func() -> Union[str, None]:
-                pass
+            def func() -> None:
+                thing: dict[str, str] = {}
             """,
-            expected_replacement="""
-            from typing import Optional
-            def func() -> Optional[str]:
-                pass
+        ),
+        Invalid(
+            """
+            def func() -> None:
+                thing: tuple[str]
             """,
         ),
         Invalid(
             """
-            from typing import Optional
-            def func() -> Union[Dict, None]:
-                pass
+            from typing import Dict
+            def func() -> None:
+                thing: dict[str, str] = {}
             """,
             expected_replacement="""
-            from typing import Optional
-            def func() -> Optional[Dict]:
-                pass
+            from typing import Dict
+            def func() -> None:
+                thing: Dict[str, str] = {}
             """,
         ),
     ]
 
-    def leave_Annotation(self, original_node: cst.Annotation) -> None:
-        if self.contains_union_with_none(original_node):
-            scope = self.get_metadata(cst.metadata.ScopeProvider, original_node, None)
-            nones = 0
-            indexes = []
-            replacement = None
-            if scope is not None and "Optional" in scope:
-                for s in cst.ensure_type(original_node.annotation, cst.Subscript).slice:
-                    if m.matches(s, m.SubscriptElement(m.Index(m.Name("None")))):
-                        nones += 1
-                    else:
-                        indexes.append(s.slice)
-                if not (nones > 1) and len(indexes) == 1:
-                    replacement = original_node.with_changes(
-                        annotation=cst.Subscript(
-                            value=cst.Name("Optional"),
-                            slice=(cst.SubscriptElement(indexes[0]),),
-                        )
-                    )
-                    # TODO(T57106602) refactor lint replacement once extract exists
-            self.report(original_node, replacement=replacement)
-
-    def contains_union_with_none(self, node: cst.Annotation) -> bool:
-        return m.matches(
-            node,
-            m.Annotation(
-                m.Subscript(
-                    value=m.Name("Union"),
-                    slice=m.OneOf(
-                        [
-                            m.SubscriptElement(m.Index()),
-                            m.SubscriptElement(m.Index(m.Name("None"))),
-                        ],
-                        [
-                            m.SubscriptElement(m.Index(m.Name("None"))),
-                            m.SubscriptElement(m.Index()),
-                        ],
-                    ),
-                )
-            ),
+    def __init__(self) -> None:
+        super().__init__()
+        self.annotation_counter: int = 0
+
+    def visit_Annotation(self, node: libcst.Annotation) -> None:
+        self.annotation_counter += 1
+
+    def leave_Annotation(self, original_node: libcst.Annotation) -> None:
+        self.annotation_counter -= 1
+
+    def visit_Name(self, node: libcst.Name) -> None:
+        # Avoid a false-positive in this scenario:
+        #
+        # ```
+        # from typing import List as list
+        # from graphene import List
+        # ```
+        qualified_names = self.get_metadata(QualifiedNameProvider, node, set())
+
+        is_builtin_type = node.value in BUILTINS_TO_REPLACE and all(
+            qualified_name.name in QUALIFIED_BUILTINS_TO_REPLACE
+            for qualified_name in qualified_names
         )
+
+        if self.annotation_counter > 0 and is_builtin_type:
+            correct_type = node.value.title()
+            scope = self.get_metadata(ScopeProvider, node)
+            replacement = None
+            if scope is not None and correct_type in scope:
+                replacement = node.with_changes(value=correct_type)
+            self.report(
+                node,
+                REPLACE_BUILTIN_TYPE_ANNOTATION.format(
+                    builtin_type=node.value, correct_type=correct_type
+                ),
+                replacement=replacement,
+            )
```

### Comparing `fixit-2.0.0a1/src/fixit/rules/rewrite_to_comprehension.py` & `fixit-2.0.0b1/src/fixit/rules/rewrite_to_comprehension.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/rewrite_to_literal.py` & `fixit-2.0.0b1/src/fixit/rules/rewrite_to_literal.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/sorted_attributes_rule.py` & `fixit-2.0.0b1/src/fixit/rules/sorted_attributes_rule.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/use_assert_in.py` & `fixit-2.0.0b1/src/fixit/rules/use_assert_in.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/use_assert_is_not_none.py` & `fixit-2.0.0b1/src/fixit/rules/use_assert_is_not_none.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/use_classname_as_code.py` & `fixit-2.0.0b1/src/fixit/rules/use_classname_as_code.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/use_fstring.py` & `fixit-2.0.0b1/src/fixit/rules/use_fstring.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/rules/use_lint_fixme_comment.py` & `fixit-2.0.0b1/src/fixit/rules/use_lint_fixme_comment.py`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/src/fixit/tests/config.py` & `fixit-2.0.0b1/src/fixit/tests/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses import asdict
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from textwrap import dedent
 from unittest import TestCase
 
 from .. import config
-from ..ftypes import Config, QualifiedRule, RawConfig
+from ..ftypes import Config, QualifiedRule, RawConfig, Tags, Version
 
 
 class ConfigTest(TestCase):
     maxDiff = None
 
     def setUp(self):
         self.td = TemporaryDirectory()
@@ -27,20 +27,22 @@
         (self.tdp / "pyproject.toml").write_text(
             dedent(
                 """
                 [tool.fixit]
                 root = true
                 enable = ["more.rules"]
                 disable = ["fixit.rules.SomethingSpecific"]
+                python_version = "3.8"
 
                 [[tool.fixit.overrides]]
                 path = "other"
-                enable = ["other.stuff"]
+                enable = ["other.stuff", ".globalrules"]
                 disable = ["fixit.rules"]
                 options = {"other.stuff.Whatever"={key="value"}}
+                python_version = "3.10"
                 """
             )
         )
         (self.outer / ".fixit.toml").write_text(
             dedent(
                 """
                 [tool.fixit]
@@ -164,22 +166,24 @@
                     ),
                     RawConfig(
                         top,
                         {
                             "root": True,
                             "enable": ["more.rules"],
                             "disable": ["fixit.rules.SomethingSpecific"],
+                            "python_version": "3.8",
                             "overrides": [
                                 {
                                     "path": "other",
-                                    "enable": ["other.stuff"],
+                                    "enable": ["other.stuff", ".globalrules"],
                                     "disable": ["fixit.rules"],
                                     "options": {
                                         "other.stuff.Whatever": {"key": "value"}
                                     },
+                                    "python_version": "3.10",
                                 },
                             ],
                         },
                     ),
                 ],
             ),
             (
@@ -191,22 +195,24 @@
                     ),
                     RawConfig(
                         top,
                         {
                             "root": True,
                             "enable": ["more.rules"],
                             "disable": ["fixit.rules.SomethingSpecific"],
+                            "python_version": "3.8",
                             "overrides": [
                                 {
                                     "path": "other",
-                                    "enable": ["other.stuff"],
+                                    "enable": ["other.stuff", ".globalrules"],
                                     "disable": ["fixit.rules"],
                                     "options": {
                                         "other.stuff.Whatever": {"key": "value"}
                                     },
+                                    "python_version": "3.10",
                                 },
                             ],
                         },
                     ),
                 ],
             ),
             (
@@ -215,22 +221,24 @@
                 [
                     RawConfig(
                         top,
                         {
                             "root": True,
                             "enable": ["more.rules"],
                             "disable": ["fixit.rules.SomethingSpecific"],
+                            "python_version": "3.8",
                             "overrides": [
                                 {
                                     "path": "other",
-                                    "enable": ["other.stuff"],
+                                    "enable": ["other.stuff", ".globalrules"],
                                     "disable": ["fixit.rules"],
                                     "options": {
                                         "other.stuff.Whatever": {"key": "value"}
                                     },
+                                    "python_version": "3.10",
                                 },
                             ],
                         },
                     ),
                 ],
             ),
         ):
@@ -253,42 +261,52 @@
                 ),
             ),
             (
                 "single",
                 [
                     RawConfig(
                         (root / "fixit.toml"),
-                        {"enable": ["foo", "bar"], "disable": ["bar"]},
+                        {
+                            "enable": ["foo", "bar"],
+                            "disable": ["bar"],
+                        },
                     ),
                 ],
                 Config(
                     path=target,
                     root=root,
                     enable=[QualifiedRule("fixit.rules"), QualifiedRule("foo")],
                     disable=[QualifiedRule("bar")],
                 ),
             ),
             (
                 "without root",
                 [
-                    RawConfig((root / "a/b/c/fixit.toml"), {"enable": ["foo"]}),
+                    RawConfig(
+                        (root / "a/b/c/fixit.toml"),
+                        {"enable": ["foo"], "python_version": "3.10"},
+                    ),
                     RawConfig(
                         (root / "a/b/fixit.toml"),
                         {"enable": ["bar"], "disable": ["foo"]},
                     ),
-                    RawConfig((root / "a/fixit.toml"), {"enable": ["foo"]}),
+                    RawConfig(
+                        (root / "a/fixit.toml"),
+                        {"enable": ["foo"], "python_version": "3.8"},
+                    ),
                 ],
                 Config(
                     path=target,
                     root=(root / "a"),
                     enable=[
                         QualifiedRule("bar"),
                         QualifiedRule("fixit.rules"),
                         QualifiedRule("foo"),
                     ],
+                    python_version=Version("3.10"),
                 ),
             ),
             (
                 "with root",
                 [
                     RawConfig(
                         (root / "a/b/c/fixit.toml"),
@@ -342,14 +360,15 @@
                         QualifiedRule(".localrules", local=".", root=self.outer),
                         QualifiedRule("more.rules"),
                     ],
                     disable=[
                         QualifiedRule("fixit.rules"),
                         QualifiedRule("fixit.rules.SomethingSpecific"),
                     ],
+                    python_version=Version("3.8"),
                 ),
             ),
             (
                 "outer with root",
                 self.outer / "foo.py",
                 self.outer,
                 Config(
@@ -362,30 +381,126 @@
             (
                 "other",
                 self.tdp / "other" / "foo.py",
                 None,
                 Config(
                     path=self.tdp / "other" / "foo.py",
                     root=self.tdp,
-                    enable=[QualifiedRule("more.rules"), QualifiedRule("other.stuff")],
+                    enable=[
+                        QualifiedRule(".globalrules", local=".", root=self.tdp),
+                        QualifiedRule("more.rules"),
+                        QualifiedRule("other.stuff"),
+                    ],
                     disable=[
                         QualifiedRule("fixit.rules"),
                         QualifiedRule("fixit.rules.SomethingSpecific"),
                     ],
                     options={"other.stuff.Whatever": {"key": "value"}},
+                    python_version=Version("3.10"),
                 ),
             ),
             (
                 "root",
                 self.tdp / "foo.py",
                 None,
                 Config(
                     path=self.tdp / "foo.py",
                     root=self.tdp,
                     enable=[QualifiedRule("fixit.rules"), QualifiedRule("more.rules")],
                     disable=[QualifiedRule("fixit.rules.SomethingSpecific")],
+                    python_version=Version("3.8"),
                 ),
             ),
         ):
             with self.subTest(name):
                 actual = config.generate_config(path, root)
                 self.assertDictEqual(asdict(expected), asdict(actual))
+
+    def test_collect_rules(self):
+        from fixit.rules.avoid_or_in_except import AvoidOrInExceptRule
+        from fixit.rules.cls_in_classmethod import UseClsInClassmethodRule
+        from fixit.rules.no_namedtuple import NoNamedTupleRule
+        from fixit.rules.use_types_from_typing import UseTypesFromTypingRule
+
+        AvoidOrInExceptRule.TAGS = {"exceptions"}
+        UseTypesFromTypingRule.TAGS = {"typing"}
+        NoNamedTupleRule.TAGS = {"typing", "tuples"}
+
+        def collect_types(cfg):
+            return sorted([type(rule) for rule in config.collect_rules(cfg)], key=str)
+
+        with self.subTest("everything"):
+            rules = collect_types(
+                Config(
+                    python_version=None,
+                )
+            )
+            self.assertIn(UseClsInClassmethodRule, rules)
+            self.assertIn(UseTypesFromTypingRule, rules)
+
+        with self.subTest("opt-out"):
+            rules = collect_types(
+                Config(
+                    disable=[QualifiedRule("fixit.rules", "UseClsInClassmethodRule")],
+                    python_version=None,
+                )
+            )
+            self.assertNotIn(UseClsInClassmethodRule, rules)
+            self.assertIn(UseTypesFromTypingRule, rules)
+
+        with self.subTest("opt-in"):
+            rules = collect_types(
+                Config(
+                    enable=[QualifiedRule("fixit.rules", "UseClsInClassmethodRule")],
+                    python_version=None,
+                )
+            )
+            self.assertListEqual([UseClsInClassmethodRule], rules)
+
+        with self.subTest("version match"):
+            rules = collect_types(
+                Config(
+                    python_version="3.7",
+                )
+            )
+            self.assertIn(UseTypesFromTypingRule, rules)
+
+        with self.subTest("version mismatch"):
+            rules = collect_types(
+                Config(
+                    python_version="3.10",
+                )
+            )
+            self.assertNotIn(UseTypesFromTypingRule, rules)
+
+        with self.subTest("tag select"):
+            rules = collect_types(
+                Config(
+                    python_version=None,
+                    tags=Tags.parse("typing"),
+                )
+            )
+            self.assertListEqual(
+                [
+                    NoNamedTupleRule,
+                    UseTypesFromTypingRule,
+                ],
+                rules,
+            )
+
+        with self.subTest("tag filter"):
+            rules = collect_types(
+                Config(
+                    python_version=None,
+                    tags=Tags.parse("^exceptions"),
+                )
+            )
+            self.assertNotIn(AvoidOrInExceptRule, rules)
+
+        with self.subTest("tag select and filter"):
+            rules = collect_types(
+                Config(
+                    python_version=None,
+                    tags=Tags.parse("typing,^tuples"),
+                )
+            )
+            self.assertListEqual([UseTypesFromTypingRule], rules)
```

### Comparing `fixit-2.0.0a1/.gitignore` & `fixit-2.0.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/LICENSE` & `fixit-2.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `fixit-2.0.0a1/README.rst` & `fixit-2.0.0b1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 on `LibCST <https://libcst.rtfd.io>`_.
 
 Fixit makes it quick and easy to write new lint rules and offer suggested
 changes for any errors found, which can then be accepted automatically,
 or presented to the user for consideration.
 
 
-**Fixit has been rebuilt for better configuration and support for custom
+**Fixit 2.0 has been rebuilt for better configuration and support for custom
 lint rules.** If you are using Fixit 0.1.4 or older, take a look at the
 `legacy documentation <https://fixit.rtfd.io/en/v0.1.4/>`_
 or the `stable branch <https://github.com/Instagram/Fixit/tree/0.x>`_.
 
 For more details, see the `user guide`__.
 
 .. __: https://fixit.rtfd.io/en/latest/guide.html
```

### Comparing `fixit-2.0.0a1/pyproject.toml` & `fixit-2.0.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,34 +24,36 @@
 ]
 
 requires-python = ">=3.8"
 dependencies = [
     "click >= 8.0",
     "libcst >= 0.3.18",
     "moreorless >= 0.4.0",
+    "packaging >= 21",
     "tomli >= 2.0; python_version < '3.11'",
     "trailrunner >= 1.2",
 ]
 
 dynamic = ["version"]
 description = "A lint framework that writes better Python code for you."
 
 [project.optional-dependencies]
 docs = [
     "jinja2 == 3.1.2",
-    "sphinx == 6.1.3",
+    "sphinx == 7.0.1",
     "sphinx-mdinclude == 0.5.3",
 ]
 dev = [
+    "attribution == 1.6.2",
     "black == 23.3.0",
     "flake8 == 6.0.0",
-    "flake8-bugbear == 23.3.23",
-    "mypy == 1.1.1",
+    "flake8-bugbear == 23.6.5",
+    "mypy == 1.3.0",
     "ufmt == 2.1.0",
-    "usort == 1.0.6",
+    "usort == 1.0.7",
 ]
 pretty = [
     "rich >= 12.6.0",
 ]
 
 [project.scripts]
 fixit = "fixit.cli:main"
@@ -110,7 +112,19 @@
 enable = ["fixit.rules"]
 disable = [
     # We don't want everything to be frozen or have to set frozen=False
     "fixit.rules:ExplicitFrozenDataclassRule",
     # We need noqa for compat with flake8 until we jettison flake8
     "fixit.rules:UseLintFixmeCommentRule",
 ]
+python_version = "3.10"
+
+[[tool.fixit.overrides]]
+path = "examples"
+enable = [".examples.noop"]
+
+[tool.attribution]
+name = "Fixit"
+package = "fixit"
+signed_tags = true
+version_file = false
+ignored_authors = ["dependabot"]
```

### Comparing `fixit-2.0.0a1/PKG-INFO` & `fixit-2.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixit
-Version: 2.0.0a1
+Version: 2.0.0b1
 Summary: A lint framework that writes better Python code for you.
 Project-URL: Home, https://fixit.rtfd.io
 Project-URL: Github, https://github.com/Instagram/Fixit
 Project-URL: Changelog, https://github.com/Instagram/LibCST/blob/main/CHANGELOG.md
 Author: Meta Platforms, Inc, Amethyst Reese, Jimmy Lai, Zsolt Dollenstein
 License: MIT License
         
@@ -91,27 +91,29 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.8
 Requires-Dist: click>=8.0
 Requires-Dist: libcst>=0.3.18
 Requires-Dist: moreorless>=0.4.0
+Requires-Dist: packaging>=21
 Requires-Dist: tomli>=2.0; python_version < '3.11'
 Requires-Dist: trailrunner>=1.2
 Provides-Extra: dev
+Requires-Dist: attribution==1.6.2; extra == 'dev'
 Requires-Dist: black==23.3.0; extra == 'dev'
-Requires-Dist: flake8-bugbear==23.3.23; extra == 'dev'
+Requires-Dist: flake8-bugbear==23.6.5; extra == 'dev'
 Requires-Dist: flake8==6.0.0; extra == 'dev'
-Requires-Dist: mypy==1.1.1; extra == 'dev'
+Requires-Dist: mypy==1.3.0; extra == 'dev'
 Requires-Dist: ufmt==2.1.0; extra == 'dev'
-Requires-Dist: usort==1.0.6; extra == 'dev'
+Requires-Dist: usort==1.0.7; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: jinja2==3.1.2; extra == 'docs'
 Requires-Dist: sphinx-mdinclude==0.5.3; extra == 'docs'
-Requires-Dist: sphinx==6.1.3; extra == 'docs'
+Requires-Dist: sphinx==7.0.1; extra == 'docs'
 Provides-Extra: pretty
 Requires-Dist: rich>=12.6.0; extra == 'pretty'
 Description-Content-Type: text/x-rst
 
 .. image:: docs/_static/logo/logo.svg
    :width: 600 px
    :alt: Fixit
@@ -143,15 +145,15 @@
 on `LibCST <https://libcst.rtfd.io>`_.
 
 Fixit makes it quick and easy to write new lint rules and offer suggested
 changes for any errors found, which can then be accepted automatically,
 or presented to the user for consideration.
 
 
-**Fixit has been rebuilt for better configuration and support for custom
+**Fixit 2.0 has been rebuilt for better configuration and support for custom
 lint rules.** If you are using Fixit 0.1.4 or older, take a look at the
 `legacy documentation <https://fixit.rtfd.io/en/v0.1.4/>`_
 or the `stable branch <https://github.com/Instagram/Fixit/tree/0.x>`_.
 
 For more details, see the `user guide`__.
 
 .. __: https://fixit.rtfd.io/en/latest/guide.html
```

