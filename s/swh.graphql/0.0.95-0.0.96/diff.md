# Comparing `tmp/swh.graphql-0.0.95.tar.gz` & `tmp/swh.graphql-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.graphql-0.0.95.tar", last modified: Tue Jun  6 15:45:15 2023, max compression
+gzip compressed data, was "swh.graphql-0.0.96.tar", last modified: Mon Jun 26 13:08:50 2023, max compression
```

## Comparing `swh.graphql-0.0.95.tar` & `swh.graphql-0.0.96.tar`

### file list

```diff
@@ -1,134 +1,136 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/
--rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)      367 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/Dockerfile
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      216 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docker-compose-dev.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docker-compose-staging.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docker-compose.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      236 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      316 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/requirements-dev.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       32 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       52 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/setup.cfg
--rw-r--r--   0 jenkins    (115) docker     (999)     2287 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1916 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/app.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/backends/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/backends/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7570 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/backends/archive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      791 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/backends/search.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/client/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/client/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5116 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/client/explorer.html
--rw-r--r--   0 jenkins    (115) docker     (999)      747 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/client/view.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/config/
--rw-r--r--   0 jenkins    (115) docker     (999)      453 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/config/dev.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      506 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/config/staging.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/config/test.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/errors/
--rw-r--r--   0 jenkins    (115) docker     (999)      604 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/errors/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      873 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/errors/errors.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/errors/handlers.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/middlewares/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/middlewares/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1054 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/middlewares/logger.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/resolvers/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6228 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/base_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/base_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3768 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/content.py
--rw-r--r--   0 jenkins    (115) docker     (999)      984 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/content_data.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2147 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2544 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/directory_entry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2194 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1974 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/person.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1919 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/release.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5211 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/resolver_factory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11757 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/resolvers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3633 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/revision.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1209 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/scalars.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1369 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/search.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3435 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/snapshot.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4202 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/snapshot_branch.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1739 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/swhid.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3030 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/target.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2141 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/visit.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/visit_status.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/schema/
--rw-r--r--   0 jenkins    (115) docker     (999)    19943 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/schema/schema.graphql
--rw-r--r--   0 jenkins    (115) docker     (999)     4367 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/server.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2821 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8119 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/data.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8848 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_branch_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7427 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_content.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1798 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_content_data_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2666 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7115 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_directory_entry.py
--rw-r--r--   0 jenkins    (115) docker     (999)      618 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_errors.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3387 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_logger.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1647 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_origin_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4815 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_origin_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5388 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_pagination.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_query_cost.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5877 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_release_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6304 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_revision.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1740 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_search.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1668 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_snapshot_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_swhid_resolve.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5259 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_visit_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_visit_status.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1289 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/backends/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/backends/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/backends/test_archive.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/errors/
--rw-r--r--   0 jenkins    (115) docker     (999)     2022 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/errors/test_errors.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      874 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_resolver_factory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3270 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_resolvers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_scalars.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1056 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/test_server.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/utils/
--rw-r--r--   0 jenkins    (115) docker     (999)     2547 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/utils/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/utils/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2102 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/utils/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     3501 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      171 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1483 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/
+-rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)      367 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/Dockerfile
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      216 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docker-compose-dev.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docker-compose-staging.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docker-compose.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.652414 swh.graphql-0.0.96/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.652414 swh.graphql-0.0.96/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.652414 swh.graphql-0.0.96/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      236 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      316 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/requirements-dev.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       32 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       60 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/setup.cfg
+-rw-r--r--   0 jenkins    (115) docker     (999)     2287 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.652414 swh.graphql-0.0.96/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.652414 swh.graphql-0.0.96/swh/graphql/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1916 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/app.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.656414 swh.graphql-0.0.96/swh/graphql/backends/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7570 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/backends/archive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      791 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/backends/search.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.656414 swh.graphql-0.0.96/swh/graphql/client/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/client/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6892 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/client/explorer.html
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.656414 swh.graphql-0.0.96/swh/graphql/client/static/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2126 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/client/static/favicon.png
+-rw-r--r--   0 jenkins    (115) docker     (999)      747 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/client/view.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.656414 swh.graphql-0.0.96/swh/graphql/config/
+-rw-r--r--   0 jenkins    (115) docker     (999)      520 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/config/dev.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      506 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/config/staging.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/config/test.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.656414 swh.graphql-0.0.96/swh/graphql/errors/
+-rw-r--r--   0 jenkins    (115) docker     (999)      604 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/errors/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      873 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/errors/errors.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/errors/handlers.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.656414 swh.graphql-0.0.96/swh/graphql/middlewares/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/middlewares/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1054 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/middlewares/logger.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.660414 swh.graphql-0.0.96/swh/graphql/resolvers/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6228 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/base_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/base_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3768 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/content.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      984 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/content_data.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2147 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2544 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/directory_entry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2194 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1974 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/person.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1919 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/release.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5211 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/resolver_factory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11757 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/resolvers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3633 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/revision.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1209 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/scalars.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1369 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/search.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3435 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/snapshot.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4202 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/snapshot_branch.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1739 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/swhid.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3030 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/target.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2141 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/visit.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/resolvers/visit_status.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.660414 swh.graphql-0.0.96/swh/graphql/schema/
+-rw-r--r--   0 jenkins    (115) docker     (999)    19922 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/schema/schema.graphql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4590 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/server.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.660414 swh.graphql-0.0.96/swh/graphql/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2821 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8119 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/data.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/swh/graphql/tests/functional/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8848 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_branch_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7427 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_content.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1798 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_content_data_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2666 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7115 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_directory_entry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      618 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_errors.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3387 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_logger.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1647 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_origin_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4815 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_origin_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5388 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_pagination.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_query_cost.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5877 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_release_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6304 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_revision.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1740 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_search.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1668 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_snapshot_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_swhid_resolve.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5259 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_visit_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/test_visit_status.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1289 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/functional/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/swh/graphql/tests/unit/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/swh/graphql/tests/unit/backends/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/backends/test_archive.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/swh/graphql/tests/unit/errors/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2022 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/errors/test_errors.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/swh/graphql/tests/unit/resolvers/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/resolvers/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      874 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/resolvers/test_resolver_factory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3270 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/resolvers/test_resolvers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/resolvers/test_scalars.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1056 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/test_server.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/swh/graphql/tests/unit/utils/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2547 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.664414 swh.graphql-0.0.96/swh/graphql/utils/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/utils/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2102 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/swh/graphql/utils/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 13:08:50.652414 swh.graphql-0.0.96/swh.graphql.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-06-26 13:08:50.000000 swh.graphql-0.0.96/swh.graphql.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     3539 2023-06-26 13:08:50.000000 swh.graphql-0.0.96/swh.graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-26 13:08:50.000000 swh.graphql-0.0.96/swh.graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      179 2023-06-26 13:08:50.000000 swh.graphql-0.0.96/swh.graphql.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-26 13:08:50.000000 swh.graphql-0.0.96/swh.graphql.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1483 2023-06-26 13:08:45.000000 swh.graphql-0.0.96/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.graphql-0.0.95/.pre-commit-config.yaml` & `swh.graphql-0.0.96/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/CODE_OF_CONDUCT.md` & `swh.graphql-0.0.96/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/LICENSE` & `swh.graphql-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/Makefile.local` & `swh.graphql-0.0.96/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/PKG-INFO` & `swh.graphql-0.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.graphql
-Version: 0.0.95
+Version: 0.0.96
 Summary: Software Heritage GraphQL Apis
 Home-page: https://forge.softwareheritage.org/diffusion/DGQL
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-graphql
```

### Comparing `swh.graphql-0.0.95/README.md` & `swh.graphql-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/docs/README.rst` & `swh.graphql-0.0.96/docs/README.rst`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/setup.py` & `swh.graphql-0.0.96/setup.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/app.py` & `swh.graphql-0.0.96/swh/graphql/app.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/backends/archive.py` & `swh.graphql-0.0.96/swh/graphql/backends/archive.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/backends/search.py` & `swh.graphql-0.0.96/swh/graphql/backends/search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/client/view.py` & `swh.graphql-0.0.96/swh/graphql/client/view.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/errors/__init__.py` & `swh.graphql-0.0.96/swh/graphql/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/errors/errors.py` & `swh.graphql-0.0.96/swh/graphql/errors/errors.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/errors/handlers.py` & `swh.graphql-0.0.96/swh/graphql/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/middlewares/logger.py` & `swh.graphql-0.0.96/swh/graphql/middlewares/logger.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/base_connection.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/base_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/base_node.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/base_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/content.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/content.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/content_data.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/content_data.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/directory.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/directory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/directory_entry.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/directory_entry.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/origin.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/origin.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/person.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/person.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/release.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/release.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/resolver_factory.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/resolver_factory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/resolvers.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/resolvers.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/revision.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/revision.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/scalars.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/scalars.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/search.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/snapshot.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/snapshot.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/snapshot_branch.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/snapshot_branch.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/swhid.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/swhid.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/target.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/target.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/visit.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/visit.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/resolvers/visit_status.py` & `swh.graphql-0.0.96/swh/graphql/resolvers/visit_status.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/schema/schema.graphql` & `swh.graphql-0.0.96/swh/graphql/schema/schema.graphql`

 * *Files 0% similar despite different names*

```diff
@@ -852,15 +852,15 @@
   The directory entry name
   """
   name: BinaryString
 
   """
   Directory entry target object
   """
-  target: DirectoryEntryTarget @cost(complexity: 1)
+  target: DirectoryEntryTarget
 }
 
 """
 Possible directory entry target nodes
 """
 union DirectoryEntryTargetNode = Directory | Content | Revision
```

### Comparing `swh.graphql-0.0.95/swh/graphql/server.py` & `swh.graphql-0.0.96/swh/graphql/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,16 @@
     AuthCredentials,
     AuthenticationBackend,
     UnauthenticatedUser,
 )
 from starlette.middleware import Middleware
 from starlette.middleware.authentication import AuthenticationMiddleware
 from starlette.middleware.cors import CORSMiddleware
-from starlette.routing import Route
+from starlette.routing import Mount, Route
+from starlette.staticfiles import StaticFiles
 
 from swh.auth.starlette.backends import BearerTokenAuthBackend
 from swh.core import config
 from swh.search import get_search as get_swh_search
 from swh.search.interface import SearchInterface
 from swh.storage import get_storage as get_swh_storage
 from swh.storage.interface import StorageInterface
@@ -134,11 +135,16 @@
     ]
 
     # Mount under a starlette application
     application = Starlette(
         routes=[
             Route("/", ariadne_app, methods=["POST"], name="graphql_api"),
             Route("/", explorer_page, methods=["GET"]),
+            Mount(
+                "/static",
+                app=StaticFiles(packages=[("swh.graphql.client", "static")]),
+                name="static",
+            ),
         ],
         middleware=middleware,
     )
     return application
```

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/conftest.py` & `swh.graphql-0.0.96/swh/graphql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/data.py` & `swh.graphql-0.0.96/swh/graphql/tests/data.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_branch_connection.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_branch_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_content.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_content.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_content_data_node.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_content_data_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_directory.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_directory_entry.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_directory_entry.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_errors.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_errors.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_logger.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_logger.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_origin_connection.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_origin_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_origin_node.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_origin_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_pagination.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_pagination.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_query_cost.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_query_cost.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
               }
             }
           }
         }
       }
     }
     """
-    # Total cost here is 157
+    # Total cost here is 207
     # 1 (snapshot) + 2 *50 (branches) + 50 * 1 (branch target)
     # + 50 * 1 (revision or Directory) +  3 * 2 = 207
     # parent multiplier is not applied when schema introspection is used
     # ie: directory entry connection cost is 3 * 2 and not 50 * 3 * 2
     errors = utils.get_error_response(
         client, query_str, swhid=str(get_snapshots()[0].swhid()), response_code=400
     )
```

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_release_node.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_release_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_revision.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_revision.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_search.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_snapshot_node.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_snapshot_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_swhid_resolve.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_swhid_resolve.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_visit_node.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_visit_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/test_visit_status.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/test_visit_status.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/functional/utils.py` & `swh.graphql-0.0.96/swh/graphql/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/unit/errors/test_errors.py` & `swh.graphql-0.0.96/swh/graphql/tests/unit/errors/test_errors.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_resolver_factory.py` & `swh.graphql-0.0.96/swh/graphql/tests/unit/resolvers/test_resolver_factory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_resolvers.py` & `swh.graphql-0.0.96/swh/graphql/tests/unit/resolvers/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_scalars.py` & `swh.graphql-0.0.96/swh/graphql/tests/unit/resolvers/test_scalars.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/unit/test_server.py` & `swh.graphql-0.0.96/swh/graphql/tests/unit/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/tests/unit/utils/test_utils.py` & `swh.graphql-0.0.96/swh/graphql/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh/graphql/utils/utils.py` & `swh.graphql-0.0.96/swh/graphql/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.95/swh.graphql.egg-info/PKG-INFO` & `swh.graphql-0.0.96/swh.graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.graphql
-Version: 0.0.95
+Version: 0.0.96
 Summary: Software Heritage GraphQL Apis
 Home-page: https://forge.softwareheritage.org/diffusion/DGQL
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-graphql
```

### Comparing `swh.graphql-0.0.95/swh.graphql.egg-info/SOURCES.txt` & `swh.graphql-0.0.96/swh.graphql.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 swh/graphql/server.py
 swh/graphql/backends/__init__.py
 swh/graphql/backends/archive.py
 swh/graphql/backends/search.py
 swh/graphql/client/__init__.py
 swh/graphql/client/explorer.html
 swh/graphql/client/view.py
+swh/graphql/client/static/favicon.png
 swh/graphql/config/dev.yml
 swh/graphql/config/staging.yml
 swh/graphql/config/test.yml
 swh/graphql/errors/__init__.py
 swh/graphql/errors/errors.py
 swh/graphql/errors/handlers.py
 swh/graphql/middlewares/__init__.py
```

### Comparing `swh.graphql-0.0.95/tox.ini` & `swh.graphql-0.0.96/tox.ini`

 * *Files identical despite different names*

