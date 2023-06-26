# Comparing `tmp/acondbs-0.4.7.tar.gz` & `tmp/acondbs-0.4.8.tar.gz`

## Comparing `acondbs-0.4.7.tar` & `acondbs-0.4.8.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/__about__.py
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/__init__.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/_logging.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/_warnings.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/auth/__init__.py
--rw-r--r--   0        0        0     3926 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/blueprint/__init__.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/blueprint/graphql_ide/__init__.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/blueprint/graphql_ide/graphiql_newer.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/blueprint/graphql_ide/graphql_playground.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/db/__init__.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/db/backup.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/db/cmds.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/db/conn.py
--rw-r--r--   0        0        0     8163 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/db/ops.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/db/sa.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/github/__init__.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/github/call.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/github/ops.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/github/query.py
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/migrations/README.md
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/migrations/alembic.ini
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/migrations/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/migrations/script.py.mako
--rw-r--r--   0        0        0    15506 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/migrations/versions/2023-06-14_14:41-2ed9841987be.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/misc/__init__.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/misc/cap.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/misc/gitb.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/misc/lock.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/__init__.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/funcs.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/account/__init__.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/account/account_admin.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/github/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/github/github_org.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/github/github_org_membership.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/github/github_token.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/github/github_user.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/misc/__init__.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/misc/log.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/__init__.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/attribute.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/field.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/product.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/product_file_path.py
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/product_relation.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/product_relation_type.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/product_type.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/product/type_field_association.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/web/__init__.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/models/web/web_config.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/__init__.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/field.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/log.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/misc.py
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/product.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/product_file_path.py
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/product_relation.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/product_relation_type.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/product_type.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/ops/web_config.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/connection.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/filter_.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/funcs.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/version.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/auth/__init__.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/auth/query.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/github/__init__.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/github/mutation.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/github/query.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/github/type_.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/misc/__init__.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/misc/mutation.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/misc/query.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/misc/type_.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/query.py
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/type_.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/mutation/__init__.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/mutation/field.py
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/mutation/product.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/mutation/product_file_path.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/mutation/product_relation.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/mutation/product_relation_type.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/product/mutation/product_type.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/web/__init__.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/web/mutation.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/web/query.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 acondbs-0.4.7/acondbs/schema/web/type_.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 acondbs-0.4.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 acondbs-0.4.7/LICENSE
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 acondbs-0.4.7/README.md
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 acondbs-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     4693 2020-02-02 00:00:00.000000 acondbs-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/__about__.py
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/__init__.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/_logging.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/_warnings.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/auth/__init__.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/blueprint/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/blueprint/graphql_ide/__init__.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/blueprint/graphql_ide/graphiql_newer.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/blueprint/graphql_ide/graphql_playground.py
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/db/__init__.py
+-rw-r--r--   0        0        0     3473 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/db/backup.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/db/cmds.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/db/conn.py
+-rw-r--r--   0        0        0     8521 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/db/ops.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/db/sa.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/github/__init__.py
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/github/call.py
+-rw-r--r--   0        0        0     7528 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/github/ops.py
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/github/query.py
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/migrations/README.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/migrations/alembic.ini
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/migrations/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/migrations/script.py.mako
+-rw-r--r--   0        0        0    15506 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/migrations/versions/2023-06-14_14:41-2ed9841987be.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/misc/__init__.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/misc/cap.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/misc/gitb.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/misc/lock.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/__init__.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/funcs.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/account/__init__.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/account/account_admin.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/github/__init__.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/github/github_org.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/github/github_org_membership.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/github/github_token.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/github/github_user.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/misc/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/misc/log.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/__init__.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/attribute.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/field.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/product.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/product_file_path.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/product_relation.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/product_relation_type.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/product_type.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/product/type_field_association.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/web/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/models/web/web_config.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/__init__.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/field.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/log.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/misc.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/product.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/product_file_path.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/product_relation.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/product_relation_type.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/product_type.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/ops/web_config.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/connection.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/filter_.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/funcs.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/version.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/auth/__init__.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/auth/query.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/github/__init__.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/github/mutation.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/github/query.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/github/type_.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/misc/__init__.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/misc/mutation.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/misc/query.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/misc/type_.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/__init__.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/query.py
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/type_.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/mutation/__init__.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/mutation/field.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/mutation/product.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/mutation/product_file_path.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/mutation/product_relation.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/mutation/product_relation_type.py
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/product/mutation/product_type.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/web/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/web/mutation.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/web/query.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 acondbs-0.4.8/acondbs/schema/web/type_.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 acondbs-0.4.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 acondbs-0.4.8/LICENSE
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 acondbs-0.4.8/README.md
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 acondbs-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 acondbs-0.4.8/PKG-INFO
```

### Comparing `acondbs-0.4.7/acondbs/__init__.py` & `acondbs-0.4.8/acondbs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 __all__ = [
     '__version__',
     'create_app',
 ]
 
 from pathlib import Path
+from typing import Any, Dict, Optional, Union
 
 from flask import Flask
 from flask_cors import CORS
 
 # This import prevents the error, ImportError: cannot import name
 # 'attach_enctype_error_multidict' from partially initialized module
 # 'flask.debughelpers' (most likely due to a circular import)
 from flask import debughelpers  # noqa: F401
 
 from . import _warnings  # noqa: F401
 from . import _logging
 
+from acondbs.__about__ import __version__
 
-DEFAULT_CONFIG_DICT = dict(
+DEFAULT_CONFIG_DICT: Dict[str, Any] = dict(
     SECRET_KEY="dev",
     SQLALCHEMY_DATABASE_URI="sqlite:///:memory:",
     SQLALCHEMY_TRACK_MODIFICATIONS=False,
 )
 
 
-def create_app(config_path=None, **kwargs):
+def create_app(config_path: Optional[Union[Path, str]] = None, **kwargs: Any) -> Flask:
     _logging.configure_logging()
 
     app = Flask(__name__, instance_relative_config=False)
     app.config.from_mapping(**DEFAULT_CONFIG_DICT)
 
     if config_path is not None:
         config_path = Path(config_path)
@@ -41,15 +43,15 @@
             # either a) relative to the top directory of the app,
             # i.e., the directory in which this file is, if
             # `instance_relative_config` is `False`, or b) relative to
             # the "instance folder", a specific directory described in
             # https://flask.palletsprojects.com/en/1.1.x/config/#instance-folders),
             # if `instance_relative_config` is `True`.
 
-        app.config.from_pyfile(config_path, silent=False)
+        app.config.from_pyfile(str(config_path), silent=False)
 
     if kwargs:
         app.config.from_mapping(**kwargs)
 
     from . import db
 
     db.init_app(app)
@@ -62,10 +64,7 @@
 
     models.init_app(app)
 
     CORS(app, resources={r"/*": {"origins": "*"}})
 
     app.logger.info('"app" initialized')
     return app
-
-
-from acondbs.__about__ import __version__
```

### Comparing `acondbs-0.4.7/acondbs/_logging.py` & `acondbs-0.4.8/acondbs/_logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 # i.e., the one dir above the module path.
 # e.g., /home/username/venv/lib/python3.8/site-packages
 
 # https://docs.python.org/3/library/logging.html#logrecord-objects
 _old_factory = logging.getLogRecordFactory()
 
 
-def record_factory(*args, **kwargs):
+def record_factory(*args, **kwargs) -> logging.LogRecord:
     """replace the pathname (the full pathname of the source file) with
     the relative path of the source file in the package
 
     For example, replace
     "/home/username/venv/lib/python3.8/site-packages/acondbs/schema/auth.py"
     with
     "acondbs/schema/auth.py"
 
     """
 
     record = _old_factory(*args, **kwargs)
     try:
-        record.pathname = Path(record.pathname).resolve().relative_to(_module_path)
+        record.pathname = str(Path(record.pathname).resolve().relative_to(_module_path))
     except Exception:
         pass
     return record
 
 
 logging.setLogRecordFactory(record_factory)
 
 
-def configure_logging():
+def configure_logging() -> None:
     """configure logging
 
     This function needs to be called early in the program, i.e., in
     the beginning of create_app() before app.logger is accessed. (It
     seems fine to be called after "app" is created.)
 
     https://flask.palletsprojects.com/en/1.1.x/logging/#basic-configuration
```

### Comparing `acondbs-0.4.7/acondbs/auth/__init__.py` & `acondbs-0.4.8/acondbs/auth/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
+from typing import Optional
+
 from flask import request
 
-from ..models import AccountAdmin, GitHubToken, GitHubUser
+from acondbs.models import AccountAdmin, GitHubToken, GitHubUser
 
 
-def is_signed_in():
-    """ """
+def is_signed_in() -> bool:
     token = _get_token_from_http_headers()
     if not token:
         return False
 
     token_model = GitHubToken.query.filter_by(token=token).one_or_none()
     if not token_model:
         return False
 
     return True
 
 
-def is_admin():
-    """ """
-
+def is_admin() -> bool:
     if not is_signed_in():
         return False
 
     token = _get_token_from_http_headers()
     if not token:
         return False
 
@@ -41,15 +40,15 @@
 
     if not admin_model:
         return False
 
     return True
 
 
-def _get_token_from_http_headers():
+def _get_token_from_http_headers() -> Optional[str]:
     auth_header = request.headers.get('Authorization')
     # e.g., 'Bearer "xxxx"', "Bearer 'xxxx'",  or 'Bearer xxxx'
 
     if not auth_header:
         return None
 
     token = auth_header.split()[1].strip('"\'')
```

### Comparing `acondbs-0.4.7/acondbs/blueprint/__init__.py` & `acondbs-0.4.8/acondbs/blueprint/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import json
 import textwrap
 import traceback
+from typing import Mapping, Optional, Union
 
-from flask import Blueprint, current_app, request
+from flask import Blueprint, Flask, Response, current_app, request
 from flask_graphql import GraphQLView
+import graphene
+
+from acondbs import auth, ops, schema
 
-from .. import auth, ops, schema
 from .graphql_ide import GRAPHIQL_NEWER, GRAPHQL_PLAYGROUND
 
 
-def format_to_str(data_dict):
+def format_to_str(data_dict: Mapping[str, str]) -> str:
     format_item = textwrap.dedent(
         """
         - {key}:
         {value}
         """
     ).lstrip()
 
@@ -24,31 +27,31 @@
                 value=textwrap.indent(str(v), " " * 4).rstrip(),
             )
             for k, v in data_dict.items()
         ]
     )
 
 
-class GraphQLView(GraphQLView):
-    def dispatch_request(self):
+class GraphQLView(GraphQLView):  # type: ignore
+    def dispatch_request(self) -> Union[str, Response]:
         res = super().dispatch_request()
         # return res
 
         if isinstance(res, str):
             # e.g, GraphiQL
             return res
 
         try:
             self._log_response(res)
         except BaseException:
             traceback.print_exc()
         finally:
             return res
 
-    def _log_response(self, res):
+    def _log_response(self, res: Response) -> None:
         if res.status_code == 200:
             return
 
         level = "ERROR"
 
         try:
             msg = self._compose_message(res)
@@ -57,32 +60,32 @@
 
         # print(msg)
         # print()
 
         ops.create_log(level=level, message=msg)
         ops.commit()
 
-    def _compose_message(self, res):
+    def _compose_message(self, res: Response) -> str:
         content = {
             "Request": self._format_request_to_str(),
             "Response": self._format_response_to_str(res),
         }
         msg = format_to_str(content)
         return msg
 
-    def _format_request_to_str(self):
+    def _format_request_to_str(self) -> str:
         content = {
             "Header": str(request.headers),
             "Data": format_to_str(self.parse_body()),
         }
         msg = format_to_str(content)
         # print(msg)
         return msg
 
-    def _format_response_to_str(self, response):
+    def _format_response_to_str(self, response: Response) -> str:
         content = {
             "Status": str(response.status),
             "Data": textwrap.indent(
                 json.dumps(response.get_json(), indent=2),
                 " " * 4,
             ),
         }
@@ -124,28 +127,28 @@
         super().__init__(**kwargs)
 
 
 bp = Blueprint("graphql", __name__)
 bp.add_url_rule("/graphql", view_func=GraphQLViewW.as_view("graphql"))
 
 
-def init_app(app):
+def init_app(app: Flask) -> None:
     app.register_blueprint(bp)
 
 
-def _select_schema():
+def _select_schema() -> graphene.Schema:
     if auth.is_admin():
         return schema.schema_admin
     elif auth.is_signed_in():
         return schema.schema_private
     else:
         return schema.schema_public
 
 
-def _select_graphiql_template():
+def _select_graphiql_template() -> Optional[str]:
     template_no = current_app.config.get("ACONDBS_GRAPHIQL_TEMPLATE_NO", None)
     if template_no == 1:
         return GRAPHIQL_NEWER
     elif template_no == 2:
         return GRAPHQL_PLAYGROUND
     else:
         return None
```

### Comparing `acondbs-0.4.7/acondbs/blueprint/graphql_ide/graphiql_newer.py` & `acondbs-0.4.8/acondbs/blueprint/graphql_ide/graphiql_newer.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/blueprint/graphql_ide/graphql_playground.py` & `acondbs-0.4.8/acondbs/blueprint/graphql_ide/graphql_playground.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/db/__init__.py` & `acondbs-0.4.8/acondbs/db/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 related to SQLAlchemy and the DB except ORM model declarations.
 
 """
 
 
 from pathlib import Path
 
+from flask import Flask
 from flask_migrate import Migrate
 
 from .cmds import (
     backup_db_command,
     dump_db_command,
     export_csv_command,
     import_csv_command,
     init_db_command,
 )
 from .conn import close_db_connection
 from .sa import sa
 
 migrate = Migrate()
 
-_MIGRATIONS_DIR = Path(__file__).resolve().parent.parent.joinpath("migrations")
+_MIGRATIONS_DIR = str(Path(__file__).resolve().parent.parent / 'migrations')
 
 
-def init_app(app):
+def init_app(app: Flask) -> None:
     """Initialize the Flask application object
 
     This function is called by `create_app()` of Flask
 
     Parameters
     ----------
     app : Flask
```

### Comparing `acondbs-0.4.7/acondbs/db/backup.py` & `acondbs-0.4.8/acondbs/db/backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Backup DB
 """
 import atexit
 import subprocess
 import threading
 import warnings
 from pathlib import Path
+from typing import Collection, Optional, Union
 
 from flask import current_app
 
 from acondbs.db.ops import export_db_to_csv_files
 from acondbs.misc import gitb, lock
 from acondbs.misc.cap import cap_exec_rate
 
 
-def request_backup_db():
+def request_backup_db() -> None:
     """reqeust to take a backup of the DB."""
     global _lock
     global _capped_backup_func
     with _lock:
         if not _capped_backup_func:
             pause = current_app.config['ACONDBS_DB_BACKUP_PAUSE']
             _capped_backup_func = cap_exec_rate(
@@ -27,35 +28,37 @@
             # threading waits for the thread to join
             # before the function registered in atexist
             # is executed.
     _capped_backup_func()
 
 
 _lock = threading.Lock()
-_capped_backup_func = None
+_capped_backup_func: Optional[cap_exec_rate] = None
 
 
-def end_backup_thread():
+def end_backup_thread() -> None:
     global _lock
     global _capped_backup_func
     with _lock:
         if _capped_backup_func:
             _capped_backup_func.end()
         _capped_backup_func = None
 
 
-import multiprocessing.queues  # This import prevents the error described in
-
+# This import prevents the error described in
 # https://github.com/alphatwirl/atpbar/issues/4#issuecomment-473426630
+import multiprocessing.queues  # noqa: F401, E402
+
 
 atexit.register(end_backup_thread)
 
 
-def run_flask_backup_db():
+def run_flask_backup_db() -> None:
     proc = subprocess.run(['flask', 'backup-db'])
+    del proc
 
 
 def backup_db(exclude_csv=None):
     try:
         backup_db_to_github()
     except Exception as e:
         warnings.warn('An exception occurred in backup_db_to_github(): {}'.format(e))
@@ -64,49 +67,51 @@
         backup_db_as_csv_to_github(exclude=exclude_csv)
     except Exception as e:
         warnings.warn(
             'An exception occurred in backup_db_as_csv_to_github(): {}'.format(e)
         )
 
 
-def backup_db_to_github():
+def backup_db_to_github() -> None:
     repo_path = current_app.config['ACONDBS_DB_FOLDER']
     lock_path = current_app.config['ACONDBS_DB_BACKUP_LOCK']
     timeout = current_app.config['ACONDBS_DB_BACKUP_LOCK_TIMEOUT']
     try:
         with lock.lock(lock_path, timeout=timeout):
             backup_db_to_github_(repo_path)
     except lock.TimeOutAcquiringLock:
         warnings.warn(
             'Time out! unable to acquire the lock in {} seconds: {}'.format(
                 timeout, lock_path
             )
         )
 
 
-def backup_db_to_github_(repo_path):
+def backup_db_to_github_(repo_path: Union[str, Path]) -> None:
     gitb.commit(repo_path)
     gitb.push(repo_path)
 
 
-def backup_db_as_csv_to_github(exclude=None):
+def backup_db_as_csv_to_github(exclude: Optional[Collection[str]] = None) -> None:
     repo_path = current_app.config['ACONDBS_DB_BACKUP_CSV_GIT_FOLDER']
     lock_path = current_app.config['ACONDBS_DB_BACKUP_CSV_GIT_LOCK']
     timeout = current_app.config['ACONDBS_DB_BACKUP_CSV_GIT_LOCK_TIMEOUT']
     try:
         with lock.lock(lock_path, timeout=timeout):
             backup_db_as_csv_to_github_(repo_path, exclude)
     except lock.TimeOutAcquiringLock:
         warnings.warn(
             'Time out! unable to acquire the lock in {} seconds: {}'.format(
                 timeout, lock_path
             )
         )
 
 
-def backup_db_as_csv_to_github_(repo_path, exclude=None):
+def backup_db_as_csv_to_github_(
+    repo_path: Union[str, Path], exclude: Optional[Collection[str]] = None
+) -> None:
     repo_path = Path(repo_path)
     for csv_file in repo_path.glob('*.csv'):
         csv_file.unlink()
     export_db_to_csv_files(repo_path, exclude)
     gitb.commit(repo_path)
     gitb.push(repo_path)
```

### Comparing `acondbs-0.4.7/acondbs/db/cmds.py` & `acondbs-0.4.8/acondbs/db/cmds.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/db/conn.py` & `acondbs-0.4.8/acondbs/db/conn.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/db/ops.py` & `acondbs-0.4.8/acondbs/db/ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 context of Flask unless stated otherwise.
 
 """
 import ast
 import csv
 import datetime
 from pathlib import Path
+from typing import Any, Collection, Optional, TextIO, Union
 
 from sqlalchemy import MetaData
 from sqlalchemy.sql import sqltypes
 
 from .conn import get_db_connection
 from .sa import sa
 
 
-def define_tables():
+def define_tables() -> None:
     """Define DB tables from ORM models
 
     After dropping any existing tables, this function defines tables
     in the DB based on ORM models.
 
     """
 
@@ -36,48 +37,48 @@
         # '"beams", "maps"'
 
         msg = f"Dropped all tables: {tbl_names}"
 
         metadata.drop_all(bind=engine)
         print(msg)
 
-    if not sa.Model.metadata.tables:
+    if not sa.Model.metadata.tables:  # type: ignore
         msg = "No tables to be created are found!"
         print(msg)
         return
 
-    tbl_names = sa.Model.metadata.tables.keys()
+    tbl_names = sa.Model.metadata.tables.keys()  # type: ignore
     # ['maps', 'beams']
 
     tbl_names = ", ".join([f'"{t}"' for t in tbl_names])
     # '"beams", "maps"'
 
     msg = f"Created tables: {tbl_names}"
 
-    sa.Model.metadata.create_all(engine)
+    sa.Model.metadata.create_all(engine)  # type: ignore
 
     print(msg)
 
 
-def get_all_table_names():
+def get_all_table_names() -> list[str]:
     """returns the names of all tables in the DB.
 
     Returns
     -------
     list of str
         the names of all tables in the DB
 
     """
     engine = sa.engine
     metadata = MetaData()
     metadata.reflect(bind=engine)
     return [tbl.name for tbl in metadata.sorted_tables]
 
 
-def export_db_to_dict_of_dict_list():
+def export_db_to_dict_of_dict_list() -> dict[str, list[dict[str, Any]]]:
     """exports the DB to a dict of table names and lists of dicts for each row
 
     Returns
     -------
     dict
         dict with one entry for each table: the table name as the key
         and the value lists of dicts: one dict for each row: field
@@ -90,15 +91,15 @@
 
     """
     tbl_names = get_all_table_names()
     ret = {n: export_table_to_dict_list(n) for n in tbl_names}
     return ret
 
 
-def export_table_to_dict_list(tbl_name):
+def export_table_to_dict_list(tbl_name: str) -> list[dict[str, Any]]:
     """exports the table to a list of dicts
 
     Parameters
     ----------
     tbl_name : str
         the table name
 
@@ -114,15 +115,15 @@
             ]
 
     """
     result_proxy = get_resultproxy_of_select_all_rows(tbl_name)
     return [dict(r) for r in result_proxy]
 
 
-def get_resultproxy_of_select_all_rows(tbl_name):
+def get_resultproxy_of_select_all_rows(tbl_name: str):
     """returns ResultProxy with all rows of the table
 
     Parameters
     ----------
     tbl_name : str
         the table name
 
@@ -137,15 +138,15 @@
     engine = sa.engine
     metadata = MetaData()
     metadata.reflect(bind=engine)
     tbl = metadata.tables[tbl_name]
     return engine.execute(tbl.select())
 
 
-def import_tables_from_csv_files(csvdir):
+def import_tables_from_csv_files(csvdir: Union[str, Path]) -> None:
     """imports tables from CSV files into the DB
 
     The tables need to be already defined in the DB.
 
     The folder `csvdir` should contain CSV files with the table
     contents to be imported: one CSV file for one table with the file
     name <<table name>>.csv
@@ -170,15 +171,15 @@
             message = f'imported to "{tbl_name}" from {csv_path}'
         else:
             message = f'skipped "{tbl_name}". file not found: {csv_path}'
 
         print(message)
 
 
-def import_table_from_csv_file(tbl_name, path):
+def import_table_from_csv_file(tbl_name: str, path: Union[str, Path]) -> None:
     """import a table from a CSV file
 
     The table needs to be already defined in the DB.
 
     Parameters
     ----------
     tbl_name : str
@@ -212,22 +213,22 @@
         )
 
         ins = tbl.insert()
         connection = get_db_connection()
 
         # Unfortunately, it is not possible to insert from a
         # generator in the current version (1.4) of SQLAlchemy.
-        data = list(data)
+        data = list(data)  # type: ignore
         if not data:
             return
 
         connection.execute(ins, data)
 
 
-def convert_data_type_for_insert(str_, type_):
+def convert_data_type_for_insert(str_: str, type_):
     """converts data type for insert
 
     This function converts the data type from str to a type relevant
     to insert in SQLAlchemy
 
     Parameters
     ----------
@@ -272,15 +273,17 @@
         try:
             return type_.python_type(ast.literal_eval(str_))
         except BaseException:
             return str_
     return None
 
 
-def export_db_to_csv_files(outdir, exclude=None):
+def export_db_to_csv_files(
+    outdir: Union[str, Path], exclude: Optional[Collection[str]] = None
+) -> None:
     """export all tables in the DB to CSV files
 
     The CSV files will be stored in the folder `csvdir`: one CSV file
     for one table with the file name <<table name>>.csv
 
     Parameters
     ----------
@@ -305,15 +308,15 @@
     for tbl_name in tbl_names:
         csv_filename = f"{tbl_name}.csv"
         csv_path = Path(outdir, csv_filename)
         with open(csv_path, "w", newline="") as f:
             export_table_to_csv_file(f, tbl_name)
 
 
-def export_table_to_csv_file(file_, tbl_name):
+def export_table_to_csv_file(file_: TextIO, tbl_name: str) -> None:
     """Export a tablesin the DB to aCSV file
 
     Parameters
     ----------
     file_ : obj
         a file object, e.g., an object returned by open()
     tbl_name : str
```

### Comparing `acondbs-0.4.7/acondbs/db/sa.py` & `acondbs-0.4.8/acondbs/db/sa.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/github/call.py` & `acondbs-0.4.8/acondbs/github/call.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 
 This module contains functions that actually access to GitHub APIs.
 Other modules in the sub-package access to GitHub APIs via functions
 in this module.
 
 """
 
+from typing import Any, Mapping, Optional, TypedDict
+
 import requests
 
 API_URL = 'https://api.github.com/graphql'
 
 
-def call_graphql_api(query, variables=None, token=None):
+def call_graphql_api(
+    query: str,
+    variables: Optional[Mapping[str, Any]] = None,
+    token: Optional[str] = None,
+) -> dict:
     """Call a GitHub GraphQL API
 
     Parameters
     ----------
     query : str
         A GraphQL query, e.g.,
         'query User($login: String!) { user(login: $login) { name } }'
@@ -37,30 +43,30 @@
         field "data."
     """
 
     headers = {}
     if token:
         headers['Authorization'] = 'token {}'.format(token)
 
-    json = {'query': query}
+    json: dict[str, Any] = {'query': query}
     if variables:
         json['variables'] = variables
 
     # example:
     #   headers = {'Authorization': 'token XXXXXXXXXXXXXXXXXXXX'}
     #   json = {
     #       'query': (
     #           'query User($login: String!) '
     #           '{ user(login: $login) { name } }'
     #       ),
     #       'variables': {"login": "octocat"}
     #   }
 
-    response = requests.post(API_URL, json=json, headers=headers)
-    response = response.json()
+    response_ = requests.post(API_URL, json=json, headers=headers)
+    response = response_.json()
     # examples:
     #   success:
     #     response = {"data": {"user": {"name": "The Octocat"} } }
     #
     #   error: (note: the 'data' field might not exist.)
     #     response = {
     #         "data": {"user": null},
@@ -85,15 +91,23 @@
 
     if 'data' not in response:
         raise Exception(response)
 
     return response['data']
 
 
-def exchange_code_for_token(code, token_url, client_id, client_secret, redirect_uri):
+class Token(TypedDict):
+    access_token: str
+    token_type: str
+    scope: str
+
+
+def exchange_code_for_token(
+    code: str, token_url: str, client_id: str, client_secret: str, redirect_uri: str
+) -> Token:
     """exchange a OAuth2 authorization code for an access token
 
     https://docs.github.com/en/free-pro-team@latest/developers/apps/authorizing-oauth-apps#2-users-are-redirected-back-to-your-site-by-github
 
     Parameters
     ----------
     code : str
@@ -128,24 +142,26 @@
         'code': code,
     }
 
     headers = {
         'Accept': "application/vnd.github.v3+json, application/json",
     }
 
-    response = requests.post(token_url, json=params, headers=headers)
-    response = response.json()  # dict
+    response_ = requests.post(token_url, json=params, headers=headers)
+    response = response_.json()  # dict
     # examples:
     #   success:
     #     response = {'access_token': 'XXXXXXXXXXXXXXXXXXXX', 'token_type': 'bearer', 'scope': 'user'}
     #
     #   error:
     #     response = {
     #         'error': 'bad_verification_code',
     #         'error_description': 'The code passed is incorrect or expired.',
     #         'error_uri': 'https://docs.github.com/apps/managing-oauth-apps/troubleshooting-oauth-app-access-token-request-errors/#bad-verification-code'
     #     }
 
     if 'access_token' not in response:
         raise Exception(response)
 
+    # TODO: verify if the response conforms Token
+
     return response
```

### Comparing `acondbs-0.4.7/acondbs/github/ops.py` & `acondbs-0.4.8/acondbs/github/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,60 @@
 """Operations on DB
 """
 
+from typing import TypedDict
+
 from flask import current_app
 
-from ..db.sa import sa
-from ..models import (
+from acondbs.db.sa import sa
+from acondbs.models import (
     AccountAdmin,
     GitHubOrg,
     GitHubOrgMembership,
     GitHubToken,
     GitHubUser,
 )
+
 from . import call, query
 
 
-def get_github_oauth_app_info():
+class GitHubOAuthAppInfo(TypedDict):
+    authorize_url: str
+    token_url: str
+    client_id: str
+    client_secret: str
+    redirect_uri: str
+
+
+def get_github_oauth_app_info() -> GitHubOAuthAppInfo:
     """Return GitHub OAuth App information
 
     Returns
     -------
     dict
         e.g.,
             {
                 'authorize_url': 'https://github.com/login/oauth/authorize',
                 'token_url': 'https://github.com/login/oauth/access_token',
                 'client_id': '2a868f8903ce767aa372',
                 'client_secret': 'a3b5c532fc28f6ceca8fd284635d915300beb7d3',
                 'redirect_uri': 'https://example.org/redirect'
             }
     """
-    ret = dict(
+    ret = GitHubOAuthAppInfo(
         authorize_url=current_app.config['GITHUB_AUTH_AUTHORIZE_URL'],
         token_url=current_app.config['GITHUB_AUTH_TOKEN_URL'],
         client_id=current_app.config['GITHUB_AUTH_CLIENT_ID'],
         client_secret=current_app.config['GITHUB_AUTH_CLIENT_SECRET'],
         redirect_uri=current_app.config['GITHUB_AUTH_REDIRECT_URI'],
     )
     return ret
 
 
-def exchange_code_for_token(code):
+def exchange_code_for_token(code: str):
     """Exchange an OAuth authentication code for a access token
 
     Parameters
     ----------
     code : str
         An OAuth authentication code, e.g, '7a31b6726dd2927b0af7'
 
@@ -64,51 +75,51 @@
         token_url=oauth_app_info['token_url'],
         client_id=oauth_app_info['client_id'],
         client_secret=current_app.config['GITHUB_AUTH_CLIENT_SECRET'],
         redirect_uri=current_app.config['GITHUB_AUTH_REDIRECT_URI'],
     )
 
 
-def add_org(login):
+def add_org(login: str) -> GitHubOrg:
     if GitHubOrg.query.filter_by(login=login).one_or_none() is not None:
         raise Exception(f'already exists: {login}')
     if not (tokens := GitHubToken.query.all()):
         raise Exception('No tokens available.')
     r = None
     for token in tokens:
         try:
             r = query.org(login, token.token)
-        except:
+        except Exception:
             continue
         break
     if r is None:
         raise Exception(f'Unable to find an org: {login}')
     model = GitHubOrg(
         login=login, git_hub_id=r['id'], avatar_url=r['avatarUrl'], url=r['url']
     )
     sa.session.add(model)
     sa.session.commit()
     return model
 
 
-def delete_org(login):
+def delete_org(login: str) -> None:
     if (model := GitHubOrg.query.filter_by(login=login).one_or_none()) is None:
         raise Exception(f'does not exist: {login}')
     sa.session.delete(model)
     sa.session.commit()
 
 
-def update_org_member_lists():
+def update_org_member_lists() -> None:
     if not (
         tokens := GitHubToken.query.filter(GitHubToken.scope.like('%read:org%')).all()
     ):
         raise Exception('No tokens with relevant scopes available.')
     if not (orgs := GitHubOrg.query.all()):
         raise Exception('No orgs found.')
-    with sa.session.no_autoflush:
+    with sa.session.no_autoflush:  # type: ignore
         memberships = GitHubOrgMembership.query.all()
         for membership in memberships:
             sa.session.delete(membership)
         for org in orgs:
             edges = None
             for token in tokens:
                 try:
@@ -145,15 +156,15 @@
                 member.avatar_url = node['avatarUrl']
                 member.url = node['url']
                 membership = GitHubOrgMembership(org=org, member=member)
                 sa.session.add(membership)
     sa.session.commit()
 
 
-def store_token_for_code(code):
+def store_token_for_code(code: str) -> None:
     token_dict = exchange_code_for_token(code)
     viewer = query.viewer(token_dict['access_token'])
     if (
         user_model := GitHubUser.query.filter_by(git_hub_id=viewer['id']).one_or_none()
     ) is None:
         user_model = GitHubUser(git_hub_id=viewer['id'])
     user_model.login = viewer['login']
@@ -163,15 +174,15 @@
     token_model = GitHubToken(
         token=token_dict['access_token'], scope=token_dict['scope'], user=user_model
     )
     sa.session.add(token_model)
     sa.session.commit()
 
 
-def authenticate(code):
+def authenticate(code: str) -> call.Token:
     """Authenticate a GitHub user with an OAuth authentication code
 
     This function authenticates a GitHub user with an OAuth
     authentication code. It also checks the membership of GitHub
     organizations and updates the DB.
 
     Parameters
@@ -218,11 +229,11 @@
         token=token_dict['access_token'], scope=token_dict['scope'], user=user_model
     )
     sa.session.add(token_model)
     sa.session.commit()
     return token_dict
 
 
-def get_user_for_token(token):
+def get_user_for_token(token: str):
     """ """
     user = GitHubUser.query.join(GitHubToken).filter(GitHubToken.token == token).one()
     return user
```

### Comparing `acondbs-0.4.7/acondbs/github/query.py` & `acondbs-0.4.8/acondbs/github/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Queries to GitHub API
 """
 
 import base64
+from typing import TypedDict
 
 from .call import call_graphql_api
 
 
-def org(login, token):
+def org(login: str, token):
     query = """
       query Organization($login: String!) {
         organization(login: $login) {
           id
           login
           avatarUrl
           url
@@ -31,15 +32,15 @@
 
     r['organization']['id'] = _decode_id(r['organization']['id'])
     # e.g., "012:Organization75631844"
 
     return r['organization']
 
 
-def org_members(org_login, token):
+def org_members(org_login: str, token: str):
     first = 100
 
     query = """
       query OrganizationMembers($org_login: String!, $first: Int!, $after: String) {
         organization(login: $org_login) {
           login
           membersWithRole(first: $first, after: $after) {
@@ -111,15 +112,23 @@
 
     for e in edges:
         e['node']['id'] = _decode_id(e['node']['id'])
 
     return edges
 
 
-def viewer(token):
+class Viewer(TypedDict):
+    id: str
+    login: str
+    name: str
+    avatarUrl: str
+    url: str
+
+
+def viewer(token: str) -> Viewer:
     """Return info about the GitHub user for a token
 
     Parameters
     ----------
     token : str
         An access token, e.g, '4d5dc8b74eccdf65859d6ac64358a3a98300c351'
 
@@ -150,14 +159,16 @@
     # }
 
     viewer = r['viewer']
 
     viewer['id'] = _decode_id(viewer['id'])
     # e.g., '04:User583231'
 
+    # TODO: verify TypedDict
+
     return viewer
 
 
 def _decode_id(id_):
     """Decode a GitHub user or organization ID returned from GitHub GraphQL API
 
     Parameters
```

### Comparing `acondbs-0.4.7/acondbs/migrations/README.md` & `acondbs-0.4.8/acondbs/migrations/README.md`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/migrations/alembic.ini` & `acondbs-0.4.8/acondbs/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/migrations/env.py` & `acondbs-0.4.8/acondbs/migrations/env.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/migrations/versions/2023-06-14_14:41-2ed9841987be.py` & `acondbs-0.4.8/acondbs/migrations/versions/2023-06-14_14:41-2ed9841987be.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/misc/cap.py` & `acondbs-0.4.8/acondbs/misc/cap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Throttle function executions
 """
 import functools
 import queue
 import threading
-import time
 from enum import Enum
+from typing import Any, Callable
 
 
 class cap_exec_rate:
     """cap the execution rate of a function
 
     This class prevents a function from being executed too often. This
     class executes a function in another thread. Once it executes a
@@ -38,162 +38,177 @@
         the function will be executed one last time if it has been
         called but not executed. If `True`, the thread can be abruptly
         stopped at the end of Python program; the function that has
         been called but not executed will not be executed.
 
     """
 
-    def __init__(self, func, pause_time=1.0, daemon=False):
+    def __init__(
+        self, func: Callable[[], Any], pause_time: float = 1.0, daemon: bool = False
+    ):
         self.func = func
         self.pause_time = pause_time
         self.daemon = daemon
 
-        self.queue = queue.Queue()
+        self.queue = queue.Queue[Message]()
         config = Config(func, self.queue, pause_time)
         self.machine = threading.Thread(
             target=state_machine, args=(config,), daemon=daemon
         )
         self.machine.start()
 
-    def __call__(self):
+    def __call__(self) -> None:
         """call the function
 
         The number of executions of the function is capped
         """
         self.queue.put(Message.FUNC_CALLED)
 
-    def end(self):
+    def end(self) -> None:
         """end using this class
 
         The function will be executed immediately if it is waiting for
         the timer. This method returns after the function is executed
         and the thread joins.
 
         """
         self.queue.put(Message.EXIT)
         self.machine.join()
 
 
-def state_machine(config):
-    """the entry function to be executed in a thread"""
-    state = Active(config)
-    while not state.end:
-        state = state()
-
-
 class Message(Enum):
     FUNC_CALLED = 1
     TIMER_GOES_OFF = 2
     EXIT = 3
 
 
 class Config:
     """Configuration of the state"""
 
-    def __init__(self, func, queue, pause_time):
+    def __init__(
+        self, func: Callable[[], Any], queue: queue.Queue[Message], pause_time: float
+    ):
         self.func = func
         self.queue = queue
         self.pause_time = pause_time
 
 
+def state_machine(config: Config) -> None:
+    """the entry function to be executed in a thread"""
+    state: State = Active(config)
+    while not state.end:
+        state = state()
+
+
 class State:
     """The base class of the states"""
 
-    def __init__(self, config):
+    end: bool = False
+
+    def __init__(self, config: Config):
         self.config = config
 
-    def __call__(self):
+    def __call__(self) -> 'State':
         message = self.config.queue.get()
         if message == Message.FUNC_CALLED:
             return self.func_called()
         elif message == Message.TIMER_GOES_OFF:
             return self.timer_goes_off()
         elif message == Message.EXIT:
             return self.exit_()
         else:
             raise ValueError('unknown message: {!r}'.format(message))
 
+    def func_called(self) -> 'State':
+        raise NotImplementedError
+
+    def timer_goes_off(self) -> 'State':
+        raise NotImplementedError
+
+    def exit_(self) -> 'State':
+        raise NotImplementedError
+
 
 class Active(State):
     """Active state
 
     The timer is not running. The function can be executed immediately
     if it is called.
     """
 
     end = False
 
-    def __init__(self, config):
+    def __init__(self, config: Config):
         super().__init__(config)
 
-    def func_called(self):
+    def func_called(self) -> State:
         self.config.func()
         return Pause(self.config)
 
-    def exit_(self):
+    def exit_(self) -> State:
         return Exit(self.config)
 
 
-def timer_end(queue):
+def timer_end(queue: queue.Queue[Message]) -> None:
     queue.put(Message.TIMER_GOES_OFF)
 
 
 class Pause(State):
     """Pause state. The function has not been called
 
     The timer is running. The function has not been called. It won't
     be executed immediately when it is called.
     """
 
     end = False
 
-    def __init__(self, config):
+    def __init__(self, config: Config):
         super().__init__(config)
         self.timer = threading.Timer(
             self.config.pause_time, functools.partial(timer_end, self.config.queue)
         )
         self.timer.start()
 
-    def func_called(self):
+    def func_called(self) -> State:
         return PauseCalled(self.config, self.timer)
 
-    def timer_goes_off(self):
+    def timer_goes_off(self) -> State:
         return Active(self.config)
 
-    def exit_(self):
+    def exit_(self) -> State:
         self.timer.cancel()
         return Exit(self.config)
 
 
 class PauseCalled(State):
     """Pause state. The function has been called
 
     The timer is running. The function has been called. The function
     won't be executed until the timer goes off.
     """
 
     end = False
 
-    def __init__(self, config, timer):
+    def __init__(self, config: Config, timer: threading.Timer):
         super().__init__(config)
         self.timer = timer
 
-    def func_called(self):
+    def func_called(self) -> State:
         return self
 
-    def timer_goes_off(self):
+    def timer_goes_off(self) -> State:
         self.config.func()
         return Pause(self.config)
 
-    def exit_(self):
+    def exit_(self) -> State:
         self.timer.cancel()
         self.config.func()
         return Exit(self.config)
 
 
 class Exit(State):
     """Exit state"""
 
     end = True
 
-    def __init__(self, config):
+    def __init__(self, config: Config):
         super().__init__(config)
```

### Comparing `acondbs-0.4.7/acondbs/misc/gitb.py` & `acondbs-0.4.8/acondbs/misc/gitb.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Git operations
 """
 import warnings
 from pathlib import Path
+from typing import Optional, Union
 
 import git
 
 
-def commit(path, message=None):
+def commit(path: Union[str, Path], message: Optional[str] = None) -> None:
     """commit all changes in a git repository to git
 
     If the path is not a git repository, unless it is empty, it will
     be initialized as a new repository.
 
     Parameters
     ----------
@@ -49,15 +50,15 @@
     repo.git.add(A=True)
 
     if not message:
         message = 'commit all'
     repo.index.commit(message)
 
 
-def pull(path):
+def pull(path: Union[str, Path]) -> None:
     """pull from a tracking branch
 
     Equivalent to execute "git pull" in the path.
 
     Parameters
     ----------
     path : str
@@ -90,15 +91,15 @@
     if not tracking_branch:
         raise ValueError("repo has no tracking branch: {}".format(path))
 
     remote = repo.remotes[tracking_branch.remote_name]
     remote.pull()
 
 
-def push(path):
+def push(path: Union[str, Path]) -> None:
     """push to a upstream branch
 
     Equivalent to execute "git push" in the path.
 
     Parameters
     ----------
     path : str
@@ -131,18 +132,18 @@
     if not tracking_branch:
         raise ValueError("repo has no tracking branch: {}".format(path))
 
     remote = repo.remotes[tracking_branch.remote_name]
     remote.push()
 
 
-def is_git_repo(path):
+def is_git_repo(path: Union[str, Path]) -> bool:
     """test if a folder is a git repository
 
     copied from https://stackoverflow.com/a/39956572/7309855
 
     """
     try:
         _ = git.Repo(path).git_dir
         return True
-    except git.exc.InvalidGitRepositoryError:
+    except git.exc.InvalidGitRepositoryError:  # type: ignore
         return False
```

### Comparing `acondbs-0.4.7/acondbs/misc/lock.py` & `acondbs-0.4.8/acondbs/misc/lock.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import contextlib
 import os
 import time
 from pathlib import Path
+from typing import Optional, Union
 
 
 class lock:
-    def __init__(self, path, timeout=None):
+    def __init__(self, path: Union[Path, str], timeout: Optional[float] = None):
         self.path = Path(path)
         self.timeout = timeout
         self.locked = False
 
-    def __enter__(self):
+    def __enter__(self) -> 'lock':
         self.acquire()
         return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
+    def __exit__(self, exc_type, exc_value, traceback) -> None:
         self.release()
 
-    def acquire(self):
+    def acquire(self) -> None:
         start_time = time.time()
         while True:
             if try_make_file(self.path):
                 break
             if self.timeout is not None:
                 if time.time() - start_time > self.timeout:
                     raise TimeOutAcquiringLock
             time.sleep(0.001)
         self.locked = True
 
-    def release(self):
+    def release(self) -> None:
         if not self.locked:
             return
 
         try:
             self.path.unlink()
         except FileNotFoundError:
             pass
         self.locked = False
 
 
 class TimeOutAcquiringLock(Exception):
     pass
 
 
-def try_make_file(path):
+def try_make_file(path: Union[str, Path]) -> bool:
     """try to create a file atomically
 
     http://stackoverflow.com/questions/33223564/atomically-creating-a-file-if-it-doesnt-exist-in-python
     """
     try:
         os.open(path, os.O_CREAT | os.O_EXCL)
         return True
```

### Comparing `acondbs-0.4.7/acondbs/models/__init__.py` & `acondbs-0.4.8/acondbs/models/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,67 +7,87 @@
 "Declaring Models" in Flask-SQLAlchemy doc:
 https://flask-sqlalchemy.palletsprojects.com/en/2.x/models/
 
 "Declare a Mapping" in SQLAlchemy doc:
 https://docs.sqlalchemy.org/en/14/orm/tutorial.html#declare-a-mapping
 
 """
-
-
-from .product import (  # noqa: F401
-    ProductType,
-    Product,
-    ProductFilePath,
-    ProductRelationType,
-    ProductRelation,
-    AttributeUnicodeText,
+__all__ = [
+    'AccountAdmin',
+    'GitHubOrg',
+    'GitHubOrgMembership',
+    'GitHubToken',
+    'GitHubUser',
+    'Log',
+    'FieldType',
+    'saEnumFieldType',
+    'AttributeBoolean',
+    'AttributeDate',
+    'AttributeDateTime',
+    'AttributeFloat',
+    'AttributeInteger',
+    'AttributeTime',
+    'AttributeUnicodeText',
+    'Field',
+    'Product',
+    'ProductFilePath',
+    'ProductRelation',
+    'ProductRelationType',
+    'ProductType',
+    'TypeFieldAssociation',
+    'WebConfig',
+    'init_app',
+]
+
+
+from flask import Flask
+
+from .account import AccountAdmin
+from .github import GitHubOrg, GitHubOrgMembership, GitHubToken, GitHubUser
+from .misc import Log
+from .product import FieldType  # enum
+from .product import saEnumFieldType  # SQLAlchemy Enum
+from .product import (
     AttributeBoolean,
-    AttributeInteger,
-    AttributeFloat,
     AttributeDate,
     AttributeDateTime,
+    AttributeFloat,
+    AttributeInteger,
     AttributeTime,
-    FieldType,  # enum
-    saEnumFieldType,  # SQLAlchemy Enum
+    AttributeUnicodeText,
     Field,
+    Product,
+    ProductFilePath,
+    ProductRelation,
+    ProductRelationType,
+    ProductType,
     TypeFieldAssociation,
 )
+from .web import WebConfig
 
-from .github import (  # noqa: F401
-    GitHubToken,
-    GitHubOrg,
-    GitHubUser,
-    GitHubOrgMembership,
-)
-
-from .account import AccountAdmin  # noqa: F401
-
-from .web import WebConfig  # noqa: F401
 
-from .misc import Log  # noqa: F401
-
-
-def init_app(app):
+def init_app(app: Flask) -> None:
     """Initialize the Flask application object
 
     This function is called by `create_app()` of Flask
 
     Parameters
     ----------
     app : Flask
         The Flask application object, an instance of `Flask`
     """
 
     _add_owners_to_db_as_admins(app)
     # remove_git_hub_tokens_with_invalid_decryption_key(app)
 
 
-def _add_owners_to_db_as_admins(app):
+def _add_owners_to_db_as_admins(app: Flask) -> None:
     import sqlalchemy
-    from ..db.sa import sa
+
+    from acondbs.db.sa import sa
 
     # Test if tables are defined. For example, tables are not defined
     # when a migration version is being created.
     with app.app_context():
         try:
             _ = AccountAdmin.query.all()
         except sqlalchemy.exc.OperationalError:
@@ -91,16 +111,16 @@
                 admin := AccountAdmin.query.filter_by(git_hub_login=owner).one_or_none()
             ) is None:
                 admin = AccountAdmin(git_hub_login=owner)
                 sa.session.add(admin)
         sa.session.commit()
 
 
-def remove_git_hub_tokens_with_invalid_decryption_key(app):
-    from ..db.sa import sa
+def remove_git_hub_tokens_with_invalid_decryption_key(app: Flask) -> None:
+    from acondbs.db.sa import sa
 
     with app.app_context():
         token_ids = [e[0] for e in sa.session.query(GitHubToken.token_id).all()]
         for token_id in token_ids:
             try:
                 token = GitHubToken.query.filter_by(  # noqa: F841
                     token_id=token_id
```

### Comparing `acondbs-0.4.7/acondbs/models/github/github_org_membership.py` & `acondbs-0.4.8/acondbs/models/github/github_org_membership.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from ...db.sa import sa
+from acondbs.db.sa import sa
 
 
-class GitHubOrgMembership(sa.Model):
+class GitHubOrgMembership(sa.Model):  # type: ignore
     __tablename__ = "github_org_memberships"
     entry_id = sa.Column(sa.Integer(), primary_key=True)
     org_id = sa.Column(sa.ForeignKey("github_orgs.org_id"), nullable=False)
     org = sa.relationship(
         "GitHubOrg",
         backref=sa.backref("memberships", cascade="all"),
     )
```

### Comparing `acondbs-0.4.7/acondbs/models/github/github_token.py` & `acondbs-0.4.8/acondbs/models/github/github_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
 
 from flask import current_app
 from sqlalchemy_utils import EncryptedType
 
-from ...db.sa import sa
+from acondbs.db.sa import sa
 
 
 def encription_key():
     return current_app.config["SECRET_KEY"]
 
 
-class GitHubToken(sa.Model):
+class GitHubToken(sa.Model):  # type: ignore
     __tablename__ = "github_tokens"
     token_id = sa.Column(sa.Integer(), primary_key=True)
     token = sa.Column(EncryptedType(sa.Text(), key=encription_key))
     scope = sa.Column(sa.Text())
     user_id = sa.Column(sa.ForeignKey("github_users.user_id"), nullable=False)
     user = sa.relationship(
         "GitHubUser",
```

### Comparing `acondbs-0.4.7/acondbs/models/product/attribute.py` & `acondbs-0.4.8/acondbs/models/product/attribute.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,63 @@
+# type: ignore
 from sqlalchemy.orm import declarative_mixin, declared_attr
 
-from ...db.sa import sa
+from acondbs.db.sa import sa
 
 
 @declarative_mixin
 class AttributeBase:
     iid = sa.Column(sa.Integer(), primary_key=True)
 
-    @declared_attr
+    @declared_attr  # type: ignore
     def product_id(self):
         return sa.Column(
             sa.Integer(),
             sa.ForeignKey("products.product_id"),
             nullable=False,
         )
 
-    @declared_attr
+    @declared_attr  # type: ignore
     def product(self):
         return sa.relationship(
             "Product",
             backref=sa.backref(
                 self.backref_column,
                 cascade="all, delete-orphan",
             ),
         )
 
-    @declared_attr
+    @declared_attr  # type: ignore
     def type_field_association_iid(self):
         return sa.Column(
             sa.Integer(),
             sa.ForeignKey("type_field_association.iid"),
             nullable=False,
         )
 
-    @declared_attr
+    @declared_attr  # type: ignore
     def type_field_association(self):
         return sa.relationship(
             "TypeFieldAssociation",
             backref=sa.backref(
                 self.backref_column,  # TODO: need to change
                 cascade="all, delete-orphan",
             ),
         )
 
-    @declared_attr
+    @declared_attr  # type: ignore
     def field_id(self):
         return sa.Column(
             sa.Integer(),
             sa.ForeignKey("field.field_id"),
             nullable=False,
         )
         # TODO: remove, replace with type_field_association_iid
 
-    @declared_attr
+    @declared_attr  # type: ignore
     def field(self):
         return sa.relationship(
             "Field",
             backref=sa.backref(
                 self.backref_column,
                 cascade="all, delete-orphan",
             ),
@@ -70,47 +71,47 @@
     def field_name(self):
         try:
             return self.field.name
         except BaseException:
             return self.field
 
 
-class AttributeUnicodeText(AttributeBase, sa.Model):
+class AttributeUnicodeText(AttributeBase, sa.Model):  # type: ignore
     __tablename__ = "attribute_unicode_text"
     backref_column = "attributes_unicode_text"
     value = sa.Column(sa.UnicodeText())
 
 
-class AttributeBoolean(AttributeBase, sa.Model):
+class AttributeBoolean(AttributeBase, sa.Model):  # type: ignore
     __tablename__ = "attribute_boolean"
     backref_column = "attributes_boolean"
     value = sa.Column(sa.Boolean())
 
 
-class AttributeInteger(AttributeBase, sa.Model):
+class AttributeInteger(AttributeBase, sa.Model):  # type: ignore
     __tablename__ = "attribute_integer"
     backref_column = "attributes_integer"
     value = sa.Column(sa.Integer())
 
 
-class AttributeFloat(AttributeBase, sa.Model):
+class AttributeFloat(AttributeBase, sa.Model):  # type: ignore
     __tablename__ = "attribute_float"
     backref_column = "attributes_float"
     value = sa.Column(sa.Float())
 
 
-class AttributeDate(AttributeBase, sa.Model):
+class AttributeDate(AttributeBase, sa.Model):  # type: ignore
     __tablename__ = "attribute_date"
     backref_column = "attributes_date"
     value = sa.Column(sa.Date())
 
 
-class AttributeDateTime(AttributeBase, sa.Model):
+class AttributeDateTime(AttributeBase, sa.Model):  # type: ignore
     __tablename__ = "attribute_date_time"
     backref_column = "attributes_date_time"
     value = sa.Column(sa.DateTime())
 
 
-class AttributeTime(AttributeBase, sa.Model):
+class AttributeTime(AttributeBase, sa.Model):  # type: ignore
     __tablename__ = "attribute_time"
     backref_column = "attributes_time"
     value = sa.Column(sa.Time())
```

### Comparing `acondbs-0.4.7/acondbs/models/product/field.py` & `acondbs-0.4.8/acondbs/models/product/field.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 
-from ...db.sa import sa
+from acondbs.db.sa import sa
+
 from . import attribute
 
 
 class FieldType(enum.Enum):
     # SQLAlchemy generic types: https://docs.sqlalchemy.org/en/14/core/type_basics.html#generic-types
     UnicodeText = 1
     Boolean = 2
@@ -29,15 +30,15 @@
     FieldType.Time: attribute.AttributeTime,
 }
 
 
 saEnumFieldType = sa.Enum(FieldType)  # to be imported in another module
 
 
-class Field(sa.Model):
+class Field(sa.Model):  # type: ignore
     __tablename__ = "field"
     field_id = sa.Column(sa.Integer(), primary_key=True)
     name = sa.Column(sa.UnicodeText(), nullable=False)
     type_ = sa.Column(saEnumFieldType, nullable=False)
 
     def __repr__(self):
         return f"<{self.__class__.__name__} {self.name!r} {self.type_name!r}>"
```

### Comparing `acondbs-0.4.7/acondbs/models/product/product.py` & `acondbs-0.4.8/acondbs/models/product/product.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
-from ...db.sa import sa
+from acondbs.db.sa import sa
 
 
-class Product(sa.Model):
+class Product(sa.Model):  # type: ignore
     # TODO: rename the class name to be more generic, e.g., "Entry"
     # TODO: use singular for the table name
     __tablename__ = "products"
     product_id = sa.Column(sa.Integer(), primary_key=True)
     type_id = sa.Column(sa.ForeignKey("product_types.type_id"), nullable=False)
     type_ = sa.relationship("ProductType", backref=sa.backref("products"))
     name = sa.Column(sa.Text(), nullable=False)
```

### Comparing `acondbs-0.4.7/acondbs/models/product/product_file_path.py` & `acondbs-0.4.8/acondbs/models/product/product_file_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from ...db.sa import sa
-from ..funcs import shorten
+from acondbs.db.sa import sa
+from acondbs.models.funcs import shorten
 
 
-class ProductFilePath(sa.Model):
+class ProductFilePath(sa.Model):  # type: ignore
     __tablename__ = "product_file_paths"
     path_id = sa.Column(sa.Integer(), primary_key=True)
     path = sa.Column(sa.Text())
     note = sa.Column(sa.Text())
     product_id = sa.Column(sa.ForeignKey("products.product_id"))
     product = sa.relationship(
         "Product", backref=sa.backref("paths", cascade="all, delete-orphan")
```

### Comparing `acondbs-0.4.7/acondbs/models/product/product_relation.py` & `acondbs-0.4.8/acondbs/models/product/product_relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy.event import listens_for
 
-from ...db.sa import sa
+from acondbs.db.sa import sa
 
 
-class ProductRelation(sa.Model):
+class ProductRelation(sa.Model):  # type: ignore
     __tablename__ = "product_relations"
     relation_id = sa.Column(sa.Integer(), primary_key=True)
     type_id = sa.Column(
         sa.Integer(),
         sa.ForeignKey("product_relation_types.type_id"),
         nullable=False,
     )
@@ -38,15 +38,15 @@
             "type_id",
             "self_product_id",
             "other_product_id",
             name="_type_id_self_product_id_other_product_id",
         ),
     )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__} {self.type_name!r}>"
 
     @property
     def type_name(self):
         # used in __repr__()
         try:
             return self.type_.name
```

### Comparing `acondbs-0.4.7/acondbs/models/product/product_relation_type.py` & `acondbs-0.4.8/acondbs/models/product/product_relation_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from sqlalchemy.event import listens_for
 
-from ...db.sa import sa
+from acondbs.db.sa import sa
 
 
-class ProductRelationType(sa.Model):
+class ProductRelationType(sa.Model):  # type: ignore
     __tablename__ = "product_relation_types"
     type_id = sa.Column(sa.Integer(), primary_key=True)
     name = sa.Column(
         sa.Text(), nullable=False, unique=True, index=True
     )  # TODO: set unique False
     reverse_type_id = sa.Column(sa.ForeignKey("product_relation_types.type_id"))
     reverse = sa.relationship(
```

### Comparing `acondbs-0.4.7/acondbs/models/product/type_field_association.py` & `acondbs-0.4.8/acondbs/models/product/type_field_association.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from ...db.sa import sa
+from acondbs.db.sa import sa
 
 
-class TypeFieldAssociation(sa.Model):
+class TypeFieldAssociation(sa.Model):  # type: ignore
     """Many-to-many relation between ProductType and Field
 
 
     This class defines which fields each product type has.
 
     When a product type is deleted, all related instances of this
     class will be automatically deleted ("delete-orphan").
```

### Comparing `acondbs-0.4.7/acondbs/ops/field.py` & `acondbs-0.4.8/acondbs/ops/field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..db.sa import sa
-from ..models import Field, FieldType
+from acondbs.db.sa import sa
+from acondbs.models import Field, FieldType
 
 
 def create_field(name, type_, field_id=None):
     """Instantiate SQLAlchemy ORM model "Field"
 
     Parameters
     ----------
```

### Comparing `acondbs-0.4.7/acondbs/ops/product.py` & `acondbs-0.4.8/acondbs/ops/product.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 
-from ..db.sa import sa
-from ..models import (
+from acondbs.db.sa import sa
+from acondbs.models import (
     FieldType,
     GitHubUser,
     Product,
     ProductFilePath,
     ProductRelation,
     ProductRelationType,
     ProductType,
```

### Comparing `acondbs-0.4.7/acondbs/ops/product_file_path.py` & `acondbs-0.4.8/acondbs/ops/product_file_path.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..db.sa import sa
-from ..models import ProductFilePath
+from acondbs.db.sa import sa
+from acondbs.models import ProductFilePath
 
 
 def create_product_file_path(**kwargs):
     model = ProductFilePath(**kwargs)
     sa.session.add(model)
     return model
```

### Comparing `acondbs-0.4.7/acondbs/ops/product_relation.py` & `acondbs-0.4.8/acondbs/ops/product_relation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..db.sa import sa
-from ..models import Product, ProductRelation, ProductRelationType
+from acondbs.db.sa import sa
+from acondbs.models import Product, ProductRelation, ProductRelationType
 
 
 def create_product_relation(type_id, self_product_id, other_product_id, **kwargs):
     type_ = ProductRelationType.query.filter_by(type_id=type_id).one()
     self_ = Product.query.filter_by(product_id=self_product_id).one()
     other = Product.query.filter_by(product_id=other_product_id).one()
     model = ProductRelation(type_=type_, self_=self_, other=other, **kwargs)
```

### Comparing `acondbs-0.4.7/acondbs/ops/product_relation_type.py` & `acondbs-0.4.8/acondbs/ops/product_relation_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..db.sa import sa
-from ..models import ProductRelationType
+from acondbs.db.sa import sa
+from acondbs.models import ProductRelationType
 
 
 def create_product_relation_type(type_, reverse=None, self_reverse=False):
     """Create a product relation type"""
 
     if self_reverse and reverse:
         raise ValueError('"reverse" is given when "self_reverse" is True')
```

### Comparing `acondbs-0.4.7/acondbs/ops/product_type.py` & `acondbs-0.4.8/acondbs/ops/product_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from ..db.sa import sa
-from ..models import Field, ProductType, TypeFieldAssociation
+from acondbs.db.sa import sa
+from acondbs.models import Field, ProductType, TypeFieldAssociation
 
 
 def create_product_type(field_ids=None, **kwargs):
     """Create a product type"""
     model = ProductType(**kwargs)
     if field_ids:
         with sa.session.no_autoflush:
```

### Comparing `acondbs-0.4.7/acondbs/schema/__init__.py` & `acondbs-0.4.8/acondbs/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/schema/connection.py` & `acondbs-0.4.8/acondbs/schema/connection.py`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/acondbs/schema/filter_.py` & `acondbs-0.4.8/acondbs/schema/filter_.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 example:
 https://github.com/art1415926535/graphene-sqlalchemy-filter/blob/1.10.2/examples/clients_and_records/filters.py
 
 """
 import graphene
 from graphene_sqlalchemy_filter import FilterableConnectionField, FilterSet
 
-from ..models import GitHubToken as GitHubTokenModel
-from ..models import GitHubUser as GitHubUserModel
-from ..models import Product as ProductModel
-from ..models import ProductType as ProductTypeModel
+from acondbs.models import GitHubToken as GitHubTokenModel
+from acondbs.models import GitHubUser as GitHubUserModel
+from acondbs.models import Product as ProductModel
+from acondbs.models import ProductType as ProductTypeModel
 
 
 class ProductFilter(FilterSet):
     type_name = graphene.String()
 
     class Meta:
         model = ProductModel
```

### Comparing `acondbs-0.4.7/acondbs/schema/version.py` & `acondbs-0.4.8/acondbs/schema/version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import graphene
 from alembic.migration import MigrationContext
 
-from ..db.conn import get_db_connection
+from acondbs.db.conn import get_db_connection
 
 
 def resolve_version(parent, info):
-    from .. import __version__
+    from acondbs.__about__ import __version__
 
     return __version__
 
 
 version_field = graphene.Field(
     graphene.String,
     description="The version of Acondbs",
```

### Comparing `acondbs-0.4.7/acondbs/schema/github/mutation.py` & `acondbs-0.4.8/acondbs/schema/github/mutation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 import graphene
 from graphql import GraphQLError
 
-from ...db.backup import request_backup_db
-from ...db.sa import sa
-from ...github.ops import (
+from acondbs.db.backup import request_backup_db
+from acondbs.db.sa import sa
+from acondbs.github.ops import (
     add_org,
     authenticate,
     delete_org,
     store_token_for_code,
     update_org_member_lists,
 )
-from ...models import GitHubToken as GitHubTokenModel
+from acondbs.models import GitHubToken as GitHubTokenModel
+
 from . import type_
 
 
 class AddGitHubOrg(graphene.Mutation):
     class Arguments:
         login = graphene.String(required=True)
 
     ok = graphene.Boolean()
     git_hub_org = graphene.Field(lambda: type_.GitHubOrg)
 
-    def mutate(root, info, login):
+    def mutate(root, info, login: str):
         model = add_org(login)
         ok = True
         # request_backup_db()
         return AddGitHubOrg(git_hub_org=model, ok=ok)
 
 
 class DeleteGitHubOrg(graphene.Mutation):
     class Arguments:
         login = graphene.String(required=True)
 
     ok = graphene.Boolean()
 
-    def mutate(root, info, login):
+    def mutate(root, info, login: str):
         delete_org(login)
         ok = True
         # request_backup_db()
         return DeleteGitHubOrg(ok=ok)
 
 
 class AuthenticateWithGitHub(graphene.Mutation):
```

### Comparing `acondbs-0.4.7/acondbs/schema/github/query.py` & `acondbs-0.4.8/acondbs/schema/github/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import graphene
 
-from ...github.ops import get_github_oauth_app_info
-from ..filter_ import PFilterableConnectionField
-from ..funcs import get_git_hub_viewer_from_info
+from acondbs.github.ops import get_github_oauth_app_info
+from acondbs.schema.filter_ import PFilterableConnectionField
+from acondbs.schema.funcs import get_git_hub_viewer_from_info
+
 from . import type_
 
 all_git_hub_orgs_field = PFilterableConnectionField(type_.GitHubOrg.connection)
 all_git_hub_users_field = PFilterableConnectionField(type_.GitHubUser.connection)
 all_git_hub_tokens_field = PFilterableConnectionField(type_.GitHubToken.connection)
```

### Comparing `acondbs-0.4.7/acondbs/schema/github/type_.py` & `acondbs-0.4.8/acondbs/schema/github/type_.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import graphene
 from graphene import relay
 from graphene_sqlalchemy import SQLAlchemyObjectType
 
-from ...models import GitHubOrg as GitHubOrgModel
-from ...models import GitHubOrgMembership as GitHubOrgMembershipModel
-from ...models import GitHubToken as GitHubTokenModel
-from ...models import GitHubUser as GitHubUserModel
-from ..connection import CountedConnection
-from ..filter_ import PFilterableConnectionField
+from acondbs.models import GitHubOrg as GitHubOrgModel
+from acondbs.models import GitHubOrgMembership as GitHubOrgMembershipModel
+from acondbs.models import GitHubToken as GitHubTokenModel
+from acondbs.models import GitHubUser as GitHubUserModel
+from acondbs.schema.connection import CountedConnection
+from acondbs.schema.filter_ import PFilterableConnectionField
 
 
 class GitHubOAuthAppInfo(graphene.ObjectType):
     client_id = graphene.String()
     authorize_url = graphene.String()
     redirect_uri = graphene.String()
```

### Comparing `acondbs-0.4.7/acondbs/schema/misc/mutation.py` & `acondbs-0.4.8/acondbs/schema/misc/mutation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import graphene
 
-from ... import ops
+from acondbs import ops
+
 from . import type_
 
 
 class CreateLogInput(graphene.InputObjectType):
     """Input to createLog()"""
 
     id_ = graphene.Int()
```

### Comparing `acondbs-0.4.7/acondbs/schema/product/query.py` & `acondbs-0.4.8/acondbs/schema/product/query.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import graphene
 
-from ...models import Field as FieldModel
-from ...models import Product as ProductModel
-from ...models import ProductRelation as ProductRelationModel
-from ...models import ProductRelationType as ProductRelationTypeModel
-from ...models import ProductType as ProductTypeModel
-from ..filter_ import PFilterableConnectionField
+from acondbs.models import Field as FieldModel
+from acondbs.models import Product as ProductModel
+from acondbs.models import ProductRelation as ProductRelationModel
+from acondbs.models import ProductRelationType as ProductRelationTypeModel
+from acondbs.models import ProductType as ProductTypeModel
+from acondbs.schema.filter_ import PFilterableConnectionField
+
 from . import type_
 
 all_products_field = PFilterableConnectionField(type_.Product.connection)
 all_product_types_field = PFilterableConnectionField(type_.ProductType.connection)  # fmt: skip
 all_product_relations_field = PFilterableConnectionField(type_.ProductRelation.connection)  # fmt: skip
 all_product_relation_types_field = PFilterableConnectionField(type_.ProductRelationType.connection)  # fmt: skip
 all_product_file_paths_field = PFilterableConnectionField(type_.ProductFilePath.connection)  # fmt: skip
```

### Comparing `acondbs-0.4.7/acondbs/schema/product/type_.py` & `acondbs-0.4.8/acondbs/schema/product/type_.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 import graphene
 from graphene import relay
 from graphene_sqlalchemy import SQLAlchemyObjectType
-
-from ..connection import CountedConnection
-from ...models import (
-    Product as ProductModel,
-    ProductType as ProductTypeModel,
-    ProductFilePath as ProductFilePathModel,
-    ProductRelation as ProductRelationModel,
-    ProductRelationType as ProductRelationTypeModel,
-    # FieldType as FieldTypeModel,  # enum
-    saEnumFieldType,  # SQLAlchemy Enum
-    Field as FieldModel,
-    TypeFieldAssociation as TypeFieldAssociationModel,
-    AttributeUnicodeText as AttributeUnicodeTextModel,
-    AttributeBoolean as AttributeBooleanModel,
-    AttributeInteger as AttributeIntegerModel,
-    AttributeFloat as AttributeFloatModel,
-    AttributeDate as AttributeDateModel,
-    AttributeDateTime as AttributeDateTimeModel,
-    AttributeTime as AttributeTimeModel,
-)
-from ..filter_ import PFilterableConnectionField
-
-
 from graphene_sqlalchemy.enums import _convert_sa_to_graphene_enum
 
+# from acondbs.models import FieldType as FieldTypeModel  # enum
+from acondbs.models import AttributeBoolean as AttributeBooleanModel
+from acondbs.models import AttributeDate as AttributeDateModel
+from acondbs.models import AttributeDateTime as AttributeDateTimeModel
+from acondbs.models import AttributeFloat as AttributeFloatModel
+from acondbs.models import AttributeInteger as AttributeIntegerModel
+from acondbs.models import AttributeTime as AttributeTimeModel
+from acondbs.models import AttributeUnicodeText as AttributeUnicodeTextModel
+from acondbs.models import Field as FieldModel
+from acondbs.models import Product as ProductModel
+from acondbs.models import ProductFilePath as ProductFilePathModel
+from acondbs.models import ProductRelation as ProductRelationModel
+from acondbs.models import ProductRelationType as ProductRelationTypeModel
+from acondbs.models import ProductType as ProductTypeModel
+from acondbs.models import TypeFieldAssociation as TypeFieldAssociationModel
+from acondbs.models import saEnumFieldType  # SQLAlchemy Enum
+from acondbs.schema.connection import CountedConnection
+from acondbs.schema.filter_ import PFilterableConnectionField
 
 # FieldType is an enum. It is manually converted to a graphene enum
 # here. An enum will be usually automatically converted. However, the
 # automatic conversion causes an error if the automatic conversion
 # of the same enum happens multiple times as described in
 # https://github.com/graphql-python/graphene-sqlalchemy/issues/211.
```

### Comparing `acondbs-0.4.7/acondbs/schema/product/mutation/field.py` & `acondbs-0.4.8/acondbs/schema/product/mutation/field.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import graphene
 
-from .... import ops
-from .. import type_
+from acondbs import ops
+from acondbs.schema.product import type_
 
 
 class CommonInputFields:
     name = graphene.String(
         required=True,
         description="The name of the field",
     )
```

### Comparing `acondbs-0.4.7/acondbs/schema/product/mutation/product.py` & `acondbs-0.4.8/acondbs/schema/product/mutation/product.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import graphene
 
-from .... import ops
-from ...funcs import get_git_hub_viewer_from_info
-from .. import type_
+from acondbs import ops
+from acondbs.schema.funcs import get_git_hub_viewer_from_info
+from acondbs.schema.product import type_
 
 
 def _reshape_arg_attributes(attributes):
     ret = {e["field_id"]: e["value"] for t, v in attributes.items() for e in v}
     return ret
```

### Comparing `acondbs-0.4.7/acondbs/schema/product/mutation/product_file_path.py` & `acondbs-0.4.8/acondbs/schema/product/mutation/product_file_path.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import graphene
 
-from .... import ops
-from .. import type_
+from acondbs import ops
+from acondbs.schema.product import type_
 
 
 class CommonInputFields:
     """Common input fields of mutations for creating and updating file paths"""
 
     path = graphene.String()
     note = graphene.String()
```

### Comparing `acondbs-0.4.7/acondbs/schema/product/mutation/product_relation.py` & `acondbs-0.4.8/acondbs/schema/product/mutation/product_relation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import graphene
 
-from .... import ops
-from .. import type_
+from acondbs import ops
+from acondbs.schema.product import type_
 
 
 class CreateProductRelationInput(graphene.InputObjectType):
     """An input to createProductRelation()"""
 
     type_id = graphene.Int(
         required=True,
```

### Comparing `acondbs-0.4.7/acondbs/schema/product/mutation/product_relation_type.py` & `acondbs-0.4.8/acondbs/schema/product/mutation/product_relation_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import graphene
 
-from .... import ops
-from .. import type_
+from acondbs import ops
+from acondbs.schema.product import type_
 
 
 class CommonInputFields:
     indef_article = graphene.String(
         description=(
             'The indefinite article placed before the singular noun "'
             'i.e., "a" or "an". '
```

### Comparing `acondbs-0.4.7/acondbs/schema/product/mutation/product_type.py` & `acondbs-0.4.8/acondbs/schema/product/mutation/product_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import graphene
 
-from .... import ops
-from .. import type_
+from acondbs import ops
+from acondbs.schema.product import type_
 
 
 class CommonInputFields:
     order = graphene.Int(
         description=(
             "The order in which the type is displayed, for example, "
             "in navigation bars."
```

### Comparing `acondbs-0.4.7/.gitignore` & `acondbs-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/LICENSE` & `acondbs-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `acondbs-0.4.7/README.md` & `acondbs-0.4.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-[![PyPI version](https://badge.fury.io/py/acondbs.svg)](https://badge.fury.io/py/acondbs) [![Test Status](https://github.com/simonsobs/acondbs/workflows/Test/badge.svg)](https://github.com/simonsobs/acondbs/actions?query=workflow%3ATest) [![codecov](https://codecov.io/gh/simonsobs/acondbs/branch/master/graph/badge.svg)](https://codecov.io/gh/simonsobs/acondbs)
+[![PyPI - Version](https://img.shields.io/pypi/v/acondbs.svg)](https://pypi.org/project/acondbs)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/acondbs.svg)](https://pypi.org/project/acondbs)
+[![Test Status](https://github.com/simonsobs/acondbs/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/acondbs/actions/workflows/unit-test.yml)
+[![codecov](https://codecov.io/gh/simonsobs/acondbs/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/acondbs)
 
 # Acondbs
 
-A GraphQL server for product DB
+ProductDB back-end API
 
 ## How to check out and run (for developers)
 
 ### Prepare environment
 
 Create a virtual environment
```

### Comparing `acondbs-0.4.7/pyproject.toml` & `acondbs-0.4.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 [build-system]
 requires = ["hatchling", "hatch-regex-commit"]
 build-backend = "hatchling.build"
 
 [project]
 name = "acondbs"
 dynamic = ["version"]
-description = "A GraphQL server for product DB"
+description = "ProductDB back-end API"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = "MIT"
 authors = [
     { name = "Simons Observatory", email = "so_software@simonsobservatory.org" },
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "a2wsgi>=1.4",
     "cryptography>=3.2",
     "Flask-Cors>=3.0",
     "Flask-GraphQL>=2.0",
-    "Flask-Migrate>=3.1,<4",
-    "Flask-SQLAlchemy>=2.5,<3",
+    "Flask-Migrate>=4.0",
+    "Flask-SQLAlchemy>=3.0",
     "Flask>=2.3",
     "gitpython>=3.1",
     "graphene-sqlalchemy-filter>=1.10",
     "graphene-sqlalchemy>=2.3",
     "requests>=2.24",
     "SQLAlchemy-Utils>=0.41",
-    "SQLAlchemy>=1.4,<3",
+    "SQLAlchemy[mypy]>=1.4,<2",
 ]
 
 [project.optional-dependencies]
 dev = ["black", "isort", "flake8", "mypy", "tox", "twine"]
 tests = [
     "async-asgi-testclient>=1.4.6",
     "pytest-asyncio>=0.14",
@@ -75,14 +75,30 @@
 norecursedirs = "acondbs/migrations docker build tests/sample"
 log_cli = false
 log_cli_level = "INFO"
 
 
 [tool.black]
 skip-string-normalization = true
-target_version = ['py38', 'py39', 'py310', 'py311']
+target_version = ['py39', 'py310', 'py311']
 exclude = '''(?x)(
    acondbs/migrations/versions/.*\.py$
 )'''
 
 [tool.isort]
 profile = "black"
+
+[tool.mypy]
+plugins = "sqlalchemy.ext.mypy.plugin"
+
+[[tool.mypy.overrides]]
+module = [
+    "graphene.*",
+    "sqlalchemy_utils.*",
+    "snapshottest",
+    "graphene_sqlalchemy.*",
+    "async_asgi_testclient",
+    "flask_graphql",
+    "graphene_sqlalchemy_filter",
+    "sqlparse",
+]
+ignore_missing_imports = true
```

### Comparing `acondbs-0.4.7/PKG-INFO` & `acondbs-0.4.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: acondbs
-Version: 0.4.7
-Summary: A GraphQL server for product DB
+Version: 0.4.8
+Summary: ProductDB back-end API
 Project-URL: Homepage, https://github.com/simonsobs/acondbs
 Project-URL: Issues, https://github.com/simonsobs/acondbs/issues
 Project-URL: Source, https://github.com/simonsobs/acondbs
 Author-email: Simons Observatory <so_software@simonsobservatory.org>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
 Requires-Dist: a2wsgi>=1.4
 Requires-Dist: cryptography>=3.2
 Requires-Dist: flask-cors>=3.0
 Requires-Dist: flask-graphql>=2.0
-Requires-Dist: flask-migrate<4,>=3.1
-Requires-Dist: flask-sqlalchemy<3,>=2.5
+Requires-Dist: flask-migrate>=4.0
+Requires-Dist: flask-sqlalchemy>=3.0
 Requires-Dist: flask>=2.3
 Requires-Dist: gitpython>=3.1
 Requires-Dist: graphene-sqlalchemy-filter>=1.10
 Requires-Dist: graphene-sqlalchemy>=2.3
 Requires-Dist: requests>=2.24
 Requires-Dist: sqlalchemy-utils>=0.41
-Requires-Dist: sqlalchemy<3,>=1.4
+Requires-Dist: sqlalchemy[mypy]<2,>=1.4
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: tox; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
@@ -40,19 +40,22 @@
 Requires-Dist: pytest-asyncio>=0.14; extra == 'tests'
 Requires-Dist: pytest-cov>=2.12; extra == 'tests'
 Requires-Dist: pytest>=6.2; extra == 'tests'
 Requires-Dist: snapshottest>=0.6; extra == 'tests'
 Requires-Dist: sqlparse; extra == 'tests'
 Description-Content-Type: text/markdown
 
-[![PyPI version](https://badge.fury.io/py/acondbs.svg)](https://badge.fury.io/py/acondbs) [![Test Status](https://github.com/simonsobs/acondbs/workflows/Test/badge.svg)](https://github.com/simonsobs/acondbs/actions?query=workflow%3ATest) [![codecov](https://codecov.io/gh/simonsobs/acondbs/branch/master/graph/badge.svg)](https://codecov.io/gh/simonsobs/acondbs)
+[![PyPI - Version](https://img.shields.io/pypi/v/acondbs.svg)](https://pypi.org/project/acondbs)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/acondbs.svg)](https://pypi.org/project/acondbs)
+[![Test Status](https://github.com/simonsobs/acondbs/actions/workflows/unit-test.yml/badge.svg)](https://github.com/simonsobs/acondbs/actions/workflows/unit-test.yml)
+[![codecov](https://codecov.io/gh/simonsobs/acondbs/branch/main/graph/badge.svg)](https://codecov.io/gh/simonsobs/acondbs)
 
 # Acondbs
 
-A GraphQL server for product DB
+ProductDB back-end API
 
 ## How to check out and run (for developers)
 
 ### Prepare environment
 
 Create a virtual environment
```

