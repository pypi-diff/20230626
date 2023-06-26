# Comparing `tmp/swh.deposit-1.2.1.tar.gz` & `tmp/swh.deposit-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.deposit-1.2.1.tar", last modified: Thu Apr 13 09:27:38 2023, max compression
+gzip compressed data, was "swh.deposit-1.2.2.tar", last modified: Mon Jun 26 11:25:42 2023, max compression
```

## Comparing `swh.deposit-1.2.1.tar` & `swh.deposit-1.2.2.tar`

### file list

```diff
@@ -1,344 +1,344 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      970 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      375 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      831 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     4315 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     3366 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/bin/
--rw-r--r--   0 jenkins    (115) docker     (999)      959 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/Makefile
--rwxr-xr-x   0 jenkins    (115) docker     (999)      130 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/content.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      322 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/create_deposit.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      381 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/create_deposit_atom.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      492 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/create_deposit_with_metadata.sh
--rw-r--r--   0 jenkins    (115) docker     (999)       94 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/default-setup
--rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/download-deposit-archive.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)       60 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/home.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      551 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/replace-deposit-archive.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)       91 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/service-document.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      256 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/status.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      582 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/update-deposit-with-another-archive.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      252 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/bin/update-status.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      569 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       25 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      240 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     3366 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/_templates/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/api/
--rw-r--r--   0 jenkins    (115) docker     (999)     3230 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/api-documentation.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      181 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     8816 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/metadata.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     1504 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/register-account.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     8033 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/use-cases.rst
--rw-r--r--   0 jenkins    (115) docker     (999)    14875 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/api/user-manual.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      653 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      169 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/conf.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/endpoints/
--rw-r--r--   0 jenkins    (115) docker     (999)     3371 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/collection.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     1864 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/content.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     2342 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/service-document.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3488 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/status.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      996 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/update-media.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      884 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/endpoints/update-metadata.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/images/
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      179 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      687 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-authentication-basic.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      977 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-authentication-keycloak.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      929 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-create-chart.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1151 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-delete-chart.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1460 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-update-chart.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1005 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-workflow-checking.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1208 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-workflow-loading.uml
--rw-r--r--   0 jenkins    (115) docker     (999)     1139 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/deposit-workflow-reception.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      542 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/images/status.uml
--rw-r--r--   0 jenkins    (115) docker     (999)      372 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/index.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/internals/
--rw-r--r--   0 jenkins    (115) docker     (999)     1646 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/authentication.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3613 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/dev-environment.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      299 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3534 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/loading-workflow.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     4191 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/internals/prod-environment.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       60 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/metadata.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       69 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/spec-api.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/docs/specs/
--rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/blueprint.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      179 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     1216 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/metadata_example.xml
--rw-r--r--   0 jenkins    (115) docker     (999)    13782 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/protocol-reference.rst
--rw-r--r--   0 jenkins    (115) docker     (999)    26174 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/spec-loading.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/specs/spec-meta-deposit.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/docs/user-manual.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      846 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      396 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       57 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements-server.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      138 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements-swh-server.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       55 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      336 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       33 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/resources/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/resources/deposit/
--rw-r--r--   0 jenkins    (115) docker     (999)       46 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/resources/deposit/server.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2648 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/
--rw-r--r--   0 jenkins    (115) docker     (999)      414 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/api/
--rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9451 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/checks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6034 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/collection.py
--rw-r--r--   0 jenkins    (115) docker     (999)    46093 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1337 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/content.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1827 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5267 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/edit.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3085 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/edit_media.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/api/private/
--rw-r--r--   0 jenkins    (115) docker     (999)     2606 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7310 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/deposit_check.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7257 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/deposit_list.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7593 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/deposit_read.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/deposit_update_status.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2612 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/private/urls.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1455 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/service_document.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1575 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/state.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2987 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/sword_edit.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2328 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/urls.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1119 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/api/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)      362 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/apps.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6072 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/auth.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/cli/
--rw-r--r--   0 jenkins    (115) docker     (999)     1187 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/cli/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8348 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/cli/admin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20150 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/cli/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    28542 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4025 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6080 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/errors.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1345 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/exception.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/fixtures/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/fixtures/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      194 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/fixtures/deposit_data.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      456 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/gunicorn_config.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/loader/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1397 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/loader/checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)      657 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/loader/tasks.py
--rwxr-xr-x   0 jenkins    (115) docker     (999)     1748 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/manage.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/migrations/
--rw-r--r--   0 jenkins    (115) docker     (999)     5260 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (115) docker     (999)      552 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0002_depositrequest_archive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      705 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0003_temporaryarchive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      368 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0004_delete_temporaryarchive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      909 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0005_auto_20171019_1436.py
--rw-r--r--   0 jenkins    (115) docker     (999)      519 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0006_depositclient_url.py
--rw-r--r--   0 jenkins    (115) docker     (999)      451 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0007_auto_20171129_1609.py
--rw-r--r--   0 jenkins    (115) docker     (999)      918 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0008_auto_20171130_1513.py
--rw-r--r--   0 jenkins    (115) docker     (999)      610 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0009_deposit_parent.py
--rw-r--r--   0 jenkins    (115) docker     (999)      633 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0010_auto_20180110_0953.py
--rw-r--r--   0 jenkins    (115) docker     (999)      884 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0011_auto_20180115_1510.py
--rw-r--r--   0 jenkins    (115) docker     (999)      520 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0012_deposit_status_detail.py
--rw-r--r--   0 jenkins    (115) docker     (999)      463 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0013_depositrequest_raw_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)      818 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0014_auto_20180720_1221.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1360 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0015_depositrequest_typemigration.py
--rw-r--r--   0 jenkins    (115) docker     (999)      879 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0016_auto_20190507_1408.py
--rw-r--r--   0 jenkins    (115) docker     (999)      613 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0017_auto_20190925_0906.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12150 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0018_migrate_swhids.py
--rw-r--r--   0 jenkins    (115) docker     (999)      517 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0019_auto_20200519_1035.py
--rw-r--r--   0 jenkins    (115) docker     (999)      583 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0020_auto_20200929_0855.py
--rw-r--r--   0 jenkins    (115) docker     (999)      859 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1858 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/0022_auto_20220223_1542.py
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/migrations/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8440 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/models.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2367 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/parsers.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/settings/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3446 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1845 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/development.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3115 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/production.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1481 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/settings/testing.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/static/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/static/css/
--rw-r--r--   0 jenkins    (115) docker     (999)    16840 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/css/bootstrap-responsive.min.css
--rw-r--r--   0 jenkins    (115) docker     (999)     8833 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/css/style.css
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/static/img/
--rw-r--r--   0 jenkins    (115) docker     (999)      868 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/arrow-up-small.png
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/
--rw-r--r--   0 jenkins    (115) docker     (999)     1961 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-32x32.png
--rw-r--r--   0 jenkins    (115) docker     (999)    16114 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png
--rw-r--r--   0 jenkins    (115) docker     (999)    17138 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png
--rw-r--r--   0 jenkins    (115) docker     (999)    23808 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png
--rw-r--r--   0 jenkins    (115) docker     (999)    45250 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/swh-logo-deposit.png
--rw-r--r--   0 jenkins    (115) docker     (999)    11585 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/img/swh-logo-deposit.svg
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/static/robots.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      505 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/api.html
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      492 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/collection_list.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      840 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/content.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      274 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/deposit_info.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1249 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/deposit_receipt.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      414 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/error.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/service_document.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1501 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/deposit/state.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1507 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/homepage.html
--rw-r--r--   0 jenkins    (115) docker     (999)     3170 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/layout.html
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/templates/rest_framework/
--rw-r--r--   0 jenkins    (115) docker     (999)      168 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/templates/rest_framework/api.html
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2730 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)      921 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_basic_auth.py
--rw-r--r--   0 jenkins    (115) docker     (999)    39027 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_checks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3499 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5097 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_add_to_origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5083 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_list.py
--rw-r--r--   0 jenkins    (115) docker     (999)    29034 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_atom.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10077 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_binary.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14940 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_multipart.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9575 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_reuse_slug.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3860 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_delete.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7680 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_check.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12966 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_list.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4051 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_read_archive.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17497 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_read_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6857 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_update_status.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4175 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_schedule.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5193 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_state.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4695 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update.py
--rw-r--r--   0 jenkins    (115) docker     (999)    19861 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update_atom.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13738 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update_binary.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1781 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_exception.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2435 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_get_file.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_keycloak_auth.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3586 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_parsers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3051 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/api/test_service_document.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10494 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/test_admin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    38630 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/cli/test_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6908 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17877 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/archives/
--rw-r--r--   0 jenkins    (115) docker     (999)      102 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/archives/single-artifact-package.tar.gz
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/
--rw-r--r--   0 jenkins    (115) docker     (999)     3613 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/codemeta-sample.xml
--rw-r--r--   0 jenkins    (115) docker     (999)       73 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-badly-formatted.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1349 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml
--rw-r--r--   0 jenkins    (115) docker     (999)       74 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-empty-body.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      220 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-fail-metadata-functional-checks.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      208 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-ko.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      111 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-minimal.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      421 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-multiple-release-notes.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1107 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      158 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-parsing-error-prone.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      501 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin-no-prov.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      639 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      515 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-both-add-to-origin-and-external-id.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      601 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      449 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-metadata-provenance.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      459 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-origin-reference.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      413 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid-fail-metadata-functional-checks.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      463 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid-no-prov.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      630 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1229 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data0.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      998 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data1.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data2.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      617 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data3.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      695 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1021 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1469 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      449 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-only-create-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      263 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-update-in-place.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      346 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-cli.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     2060 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-decimal.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-external-identifier-and-create-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-external-identifier.xml
--rw-r--r--   0 jenkins    (115) docker     (999)      527 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml
--rw-r--r--   0 jenkins    (115) docker     (999)     1538 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/atom/metadata.xml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/
--rw-r--r--   0 jenkins    (115) docker     (999)     1209 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1164 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_test
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/
--rw-r--r--   0 jenkins    (115) docker     (999)     1212 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1469 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/
--rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1240 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test
--rw-r--r--   0 jenkins    (115) docker     (999)     1196 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media
--rw-r--r--   0 jenkins    (115) docker     (999)     1196 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata
--rw-r--r--   0 jenkins    (115) docker     (999)      792 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/
--rw-r--r--   0 jenkins    (115) docker     (999)     1218 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)      812 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/
--rw-r--r--   0 jenkins    (115) docker     (999)     1212 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1636 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/
--rw-r--r--   0 jenkins    (115) docker     (999)     1217 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument
--rw-r--r--   0 jenkins    (115) docker     (999)     1634 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom
--rw-r--r--   0 jenkins    (115) docker     (999)     1635 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status
--rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4190 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)      601 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/http_example.org/
--rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/http_example.org/hello.json
--rw-r--r--   0 jenkins    (115) docker     (999)       13 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/http_example.org/hello_you
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/
--rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_1_check
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_2_check
--rw-r--r--   0 jenkins    (115) docker     (999)     2146 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta
--rw-r--r--   0 jenkins    (115) docker     (999)   725946 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw
--rw-r--r--   0 jenkins    (115) docker     (999)        5 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_update
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_nowhere.org/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_check
--rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_metadata
--rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_raw
--rw-r--r--   0 jenkins    (115) docker     (999)     1233 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/test_checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7064 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/test_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2387 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/loader/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2466 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_backend.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7253 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_client_module.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1050 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1258 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2031 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_gunicorn_config.py
--rw-r--r--   0 jenkins    (115) docker     (999)      762 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5134 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_migrations.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7679 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests/test_utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/tests_migration/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/tests_migration/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1394 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/urls.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7713 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh/deposit/xsd/
--rw-r--r--   0 jenkins    (115) docker     (999)     3808 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/xsd/codemeta.xsd
--rw-r--r--   0 jenkins    (115) docker     (999)     2699 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/swh/deposit/xsd/swh.xsd
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     4315 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)    11801 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      162 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      690 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-04-13 09:27:38.000000 swh.deposit-1.2.1/swh.deposit.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1872 2023-04-13 09:27:36.000000 swh.deposit-1.2.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.854580 swh.deposit-1.2.2/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      970 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      375 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      831 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     4315 2023-06-26 11:25:42.854580 swh.deposit-1.2.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     3366 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.790579 swh.deposit-1.2.2/bin/
+-rw-r--r--   0 jenkins    (115) docker     (999)      959 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/Makefile
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      130 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/content.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      322 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/create_deposit.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      381 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/create_deposit_atom.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      492 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/create_deposit_with_metadata.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)       94 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/default-setup
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/download-deposit-archive.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)       60 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/home.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      551 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/replace-deposit-archive.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)       91 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/service-document.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      256 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/status.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      582 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/update-deposit-with-another-archive.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      252 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/bin/update-status.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      569 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.794579 swh.deposit-1.2.2/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       25 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      240 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     3366 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.794579 swh.deposit-1.2.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.794579 swh.deposit-1.2.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/_templates/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.794579 swh.deposit-1.2.2/docs/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3230 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/api/api-documentation.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      181 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/api/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     8816 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/api/metadata.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     1504 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/api/register-account.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     8033 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/api/use-cases.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)    14875 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/api/user-manual.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      653 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      169 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/conf.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.794579 swh.deposit-1.2.2/docs/endpoints/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3371 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/endpoints/collection.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     1864 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/endpoints/content.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     2342 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/endpoints/service-document.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3488 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/endpoints/status.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      996 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/endpoints/update-media.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      884 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/endpoints/update-metadata.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.794579 swh.deposit-1.2.2/docs/images/
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      179 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      687 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/deposit-authentication-basic.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      977 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/deposit-authentication-keycloak.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      929 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/deposit-create-chart.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1151 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/deposit-delete-chart.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1460 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/deposit-update-chart.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1005 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/deposit-workflow-checking.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1208 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/deposit-workflow-loading.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1139 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/deposit-workflow-reception.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      542 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/images/status.uml
+-rw-r--r--   0 jenkins    (115) docker     (999)      372 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/index.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.798579 swh.deposit-1.2.2/docs/internals/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1646 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/internals/authentication.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3613 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/internals/dev-environment.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      299 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/internals/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3534 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/internals/loading-workflow.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     4191 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/internals/prod-environment.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       60 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/metadata.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       69 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/spec-api.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.798579 swh.deposit-1.2.2/docs/specs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/specs/blueprint.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      179 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/specs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     1216 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/specs/metadata_example.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)    13782 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/specs/protocol-reference.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)    26174 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/specs/spec-loading.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     4108 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/specs/spec-meta-deposit.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/docs/user-manual.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      846 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      396 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       57 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/requirements-server.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      138 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/requirements-swh-server.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      166 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      336 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      155 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.782579 swh.deposit-1.2.2/resources/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.798579 swh.deposit-1.2.2/resources/deposit/
+-rw-r--r--   0 jenkins    (115) docker     (999)       46 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/resources/deposit/server.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-26 11:25:42.854580 swh.deposit-1.2.2/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2648 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.798579 swh.deposit-1.2.2/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.826579 swh.deposit-1.2.2/swh/deposit/
+-rw-r--r--   0 jenkins    (115) docker     (999)      414 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.826579 swh.deposit-1.2.2/swh/deposit/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9451 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/checks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6034 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/collection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    46093 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1337 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/content.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1827 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5267 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/edit.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3085 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/edit_media.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.830579 swh.deposit-1.2.2/swh/deposit/api/private/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2606 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/private/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7310 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/private/deposit_check.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7257 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/private/deposit_list.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7593 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/private/deposit_read.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3822 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/private/deposit_update_status.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2612 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/private/urls.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1455 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/service_document.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1575 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/state.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2987 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/sword_edit.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2328 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/urls.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1119 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/api/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      362 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/apps.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6072 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/auth.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.830579 swh.deposit-1.2.2/swh/deposit/cli/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1187 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8348 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/cli/admin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20150 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/cli/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    28542 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4025 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6080 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/errors.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1345 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/exception.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.830579 swh.deposit-1.2.2/swh/deposit/fixtures/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/fixtures/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      194 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/fixtures/deposit_data.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      456 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/gunicorn_config.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.830579 swh.deposit-1.2.2/swh/deposit/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)      245 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/loader/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1397 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/loader/checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      657 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/loader/tasks.py
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     1748 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/manage.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.834580 swh.deposit-1.2.2/swh/deposit/migrations/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5260 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      552 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0002_depositrequest_archive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      705 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0003_temporaryarchive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      368 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0004_delete_temporaryarchive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      909 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0005_auto_20171019_1436.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      519 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0006_depositclient_url.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      451 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0007_auto_20171129_1609.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      918 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0008_auto_20171130_1513.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      610 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0009_deposit_parent.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      633 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0010_auto_20180110_0953.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      884 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0011_auto_20180115_1510.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      520 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0012_deposit_status_detail.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      463 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0013_depositrequest_raw_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      818 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0014_auto_20180720_1221.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1360 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0015_depositrequest_typemigration.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      879 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0016_auto_20190507_1408.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      613 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0017_auto_20190925_0906.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12150 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0018_migrate_swhids.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      517 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0019_auto_20200519_1035.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      583 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0020_auto_20200929_0855.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      859 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1858 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/0022_auto_20220223_1542.py
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/migrations/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8440 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/models.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2367 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/parsers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.834580 swh.deposit-1.2.2/swh/deposit/settings/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/settings/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3446 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/settings/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1845 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/settings/development.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3115 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/settings/production.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1481 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/settings/testing.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.834580 swh.deposit-1.2.2/swh/deposit/static/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.834580 swh.deposit-1.2.2/swh/deposit/static/css/
+-rw-r--r--   0 jenkins    (115) docker     (999)    16840 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/css/bootstrap-responsive.min.css
+-rw-r--r--   0 jenkins    (115) docker     (999)     8833 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/css/style.css
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.834580 swh.deposit-1.2.2/swh/deposit/static/img/
+-rw-r--r--   0 jenkins    (115) docker     (999)      868 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/img/arrow-up-small.png
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.834580 swh.deposit-1.2.2/swh/deposit/static/img/icons/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1961 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/img/icons/swh-logo-32x32.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    16114 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    17138 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    23808 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    45250 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/img/swh-logo-deposit.png
+-rw-r--r--   0 jenkins    (115) docker     (999)    11585 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/img/swh-logo-deposit.svg
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/static/robots.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.834580 swh.deposit-1.2.2/swh/deposit/templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      505 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/api.html
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.838580 swh.deposit-1.2.2/swh/deposit/templates/deposit/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/deposit/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      492 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/deposit/collection_list.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      840 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/deposit/content.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      274 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/deposit/deposit_info.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1249 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/deposit/deposit_receipt.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      414 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/deposit/error.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/deposit/service_document.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1501 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/deposit/state.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1507 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/homepage.html
+-rw-r--r--   0 jenkins    (115) docker     (999)     3170 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/layout.html
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.838580 swh.deposit-1.2.2/swh/deposit/templates/rest_framework/
+-rw-r--r--   0 jenkins    (115) docker     (999)      168 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/templates/rest_framework/api.html
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.838580 swh.deposit-1.2.2/swh/deposit/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.842579 swh.deposit-1.2.2/swh/deposit/tests/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2730 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      921 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_basic_auth.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    39027 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_checks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3499 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_collection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5097 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_add_to_origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5083 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_list.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    29034 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_post_atom.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10077 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_post_binary.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14940 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_post_multipart.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9575 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_reuse_slug.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3860 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_delete.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7680 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_check.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12966 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_list.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4051 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_read_archive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17497 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_read_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6857 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_update_status.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4175 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_schedule.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5193 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_state.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4695 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_update.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    19861 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_update_atom.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13738 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_update_binary.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1781 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_exception.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2435 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_get_file.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_keycloak_auth.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3586 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_parsers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3051 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/api/test_service_document.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.842579 swh.deposit-1.2.2/swh/deposit/tests/cli/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/cli/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10494 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/cli/test_admin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    38630 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/cli/test_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6908 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17877 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.786579 swh.deposit-1.2.2/swh/deposit/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.842579 swh.deposit-1.2.2/swh/deposit/tests/data/archives/
+-rw-r--r--   0 jenkins    (115) docker     (999)      102 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/archives/single-artifact-package.tar.gz
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.846579 swh.deposit-1.2.2/swh/deposit/tests/data/atom/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3613 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/codemeta-sample.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)       73 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-badly-formatted.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1349 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)       74 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-empty-body.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      220 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-fail-metadata-functional-checks.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      208 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-ko.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      111 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-minimal.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      421 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-multiple-release-notes.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1107 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      158 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-parsing-error-prone.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      501 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-add-to-origin-no-prov.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      639 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      515 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-both-add-to-origin-and-external-id.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      601 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      449 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-metadata-provenance.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      459 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-origin-reference.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      413 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-swhid-fail-metadata-functional-checks.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      463 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-swhid-no-prov.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      630 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-swhid.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1229 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data0.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      998 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data1.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data2.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      617 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data3.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      695 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1021 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1469 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-list-deposits.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      449 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-only-create-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      263 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-update-in-place.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      346 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/error-cli.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     2060 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/error-with-decimal.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      512 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/error-with-external-identifier-and-create-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/error-with-external-identifier.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)      527 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1538 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/atom/metadata.xml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.846579 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.swh.test/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1209 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1164 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.swh.test/1_test
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.846579 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.list/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1212 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1469 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.850580 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1214 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1240 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test
+-rw-r--r--   0 jenkins    (115) docker     (999)     1196 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media
+-rw-r--r--   0 jenkins    (115) docker     (999)     1196 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata
+-rw-r--r--   0 jenkins    (115) docker     (999)      792 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.850580 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1218 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)      812 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.850580 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.status/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1212 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1636 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.850580 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1217 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument
+-rw-r--r--   0 jenkins    (115) docker     (999)     1634 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom
+-rw-r--r--   0 jenkins    (115) docker     (999)     1635 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status
+-rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.850580 swh.deposit-1.2.2/swh/deposit/tests/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4190 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      601 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.786579 swh.deposit-1.2.2/swh/deposit/tests/loader/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.850580 swh.deposit-1.2.2/swh/deposit/tests/loader/data/http_example.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)       20 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/http_example.org/hello.json
+-rw-r--r--   0 jenkins    (115) docker     (999)       13 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/http_example.org/hello_you
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.850580 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_1_check
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_2_check
+-rw-r--r--   0 jenkins    (115) docker     (999)     2146 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta
+-rw-r--r--   0 jenkins    (115) docker     (999)   725946 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw
+-rw-r--r--   0 jenkins    (115) docker     (999)        5 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_update
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.854580 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_nowhere.org/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_check
+-rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_metadata
+-rw-r--r--   0 jenkins    (115) docker     (999)       23 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_nowhere.org/1_private_test_1_raw
+-rw-r--r--   0 jenkins    (115) docker     (999)     1233 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/test_checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7064 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/test_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2387 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/loader/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2466 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/test_backend.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7253 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/test_client_module.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1050 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1258 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2031 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/test_gunicorn_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      762 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5134 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/test_migrations.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7679 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests/test_utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.854580 swh.deposit-1.2.2/swh/deposit/tests_migration/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/tests_migration/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1394 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/urls.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7713 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.854580 swh.deposit-1.2.2/swh/deposit/xsd/
+-rw-r--r--   0 jenkins    (115) docker     (999)     3808 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/xsd/codemeta.xsd
+-rw-r--r--   0 jenkins    (115) docker     (999)     2699 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/swh/deposit/xsd/swh.xsd
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-26 11:25:42.798579 swh.deposit-1.2.2/swh.deposit.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4315 2023-06-26 11:25:42.000000 swh.deposit-1.2.2/swh.deposit.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)    11801 2023-06-26 11:25:42.000000 swh.deposit-1.2.2/swh.deposit.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-26 11:25:42.000000 swh.deposit-1.2.2/swh.deposit.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      162 2023-06-26 11:25:42.000000 swh.deposit-1.2.2/swh.deposit.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      676 2023-06-26 11:25:42.000000 swh.deposit-1.2.2/swh.deposit.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-26 11:25:42.000000 swh.deposit-1.2.2/swh.deposit.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1872 2023-06-26 11:25:37.000000 swh.deposit-1.2.2/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `swh.deposit-1.2.1/.pre-commit-config.yaml` & `swh.deposit-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/CODE_OF_CONDUCT.md` & `swh.deposit-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/LICENSE` & `swh.deposit-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/Makefile.local` & `swh.deposit-1.2.2/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/PKG-INFO` & `swh.deposit-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.deposit
-Version: 1.2.1
+Version: 1.2.2
 Summary: Software Heritage Deposit Server
 Home-page: https://forge.softwareheritage.org/source/swh-deposit/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-deposit
```

### Comparing `swh.deposit-1.2.1/README.rst` & `swh.deposit-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/bin/Makefile` & `swh.deposit-1.2.2/bin/Makefile`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/bin/replace-deposit-archive.sh` & `swh.deposit-1.2.2/bin/replace-deposit-archive.sh`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/bin/update-deposit-with-another-archive.sh` & `swh.deposit-1.2.2/bin/update-deposit-with-another-archive.sh`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/conftest.py` & `swh.deposit-1.2.2/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/README.rst` & `swh.deposit-1.2.2/docs/README.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/api/api-documentation.rst` & `swh.deposit-1.2.2/docs/api/api-documentation.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/api/metadata.rst` & `swh.deposit-1.2.2/docs/api/metadata.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/api/register-account.rst` & `swh.deposit-1.2.2/docs/api/register-account.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/api/use-cases.rst` & `swh.deposit-1.2.2/docs/api/use-cases.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/api/user-manual.rst` & `swh.deposit-1.2.2/docs/api/user-manual.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/cli.rst` & `swh.deposit-1.2.2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/endpoints/collection.rst` & `swh.deposit-1.2.2/docs/endpoints/collection.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/endpoints/content.rst` & `swh.deposit-1.2.2/docs/endpoints/content.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/endpoints/service-document.rst` & `swh.deposit-1.2.2/docs/endpoints/service-document.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/endpoints/status.rst` & `swh.deposit-1.2.2/docs/endpoints/status.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/endpoints/update-media.rst` & `swh.deposit-1.2.2/docs/endpoints/update-media.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/endpoints/update-metadata.rst` & `swh.deposit-1.2.2/docs/endpoints/update-metadata.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/deposit-authentication-basic.uml` & `swh.deposit-1.2.2/docs/images/deposit-authentication-basic.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/deposit-authentication-keycloak.uml` & `swh.deposit-1.2.2/docs/images/deposit-authentication-keycloak.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/deposit-create-chart.uml` & `swh.deposit-1.2.2/docs/images/deposit-create-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/deposit-delete-chart.uml` & `swh.deposit-1.2.2/docs/images/deposit-delete-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/deposit-update-chart.uml` & `swh.deposit-1.2.2/docs/images/deposit-update-chart.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/deposit-workflow-checking.uml` & `swh.deposit-1.2.2/docs/images/deposit-workflow-checking.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/deposit-workflow-loading.uml` & `swh.deposit-1.2.2/docs/images/deposit-workflow-loading.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/deposit-workflow-reception.uml` & `swh.deposit-1.2.2/docs/images/deposit-workflow-reception.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/images/status.uml` & `swh.deposit-1.2.2/docs/images/status.uml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/internals/authentication.rst` & `swh.deposit-1.2.2/docs/internals/authentication.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/internals/dev-environment.rst` & `swh.deposit-1.2.2/docs/internals/dev-environment.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/internals/loading-workflow.rst` & `swh.deposit-1.2.2/docs/internals/loading-workflow.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/internals/prod-environment.rst` & `swh.deposit-1.2.2/docs/internals/prod-environment.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/specs/metadata_example.xml` & `swh.deposit-1.2.2/docs/specs/metadata_example.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/specs/protocol-reference.rst` & `swh.deposit-1.2.2/docs/specs/protocol-reference.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/specs/spec-loading.rst` & `swh.deposit-1.2.2/docs/specs/spec-loading.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/docs/specs/spec-meta-deposit.rst` & `swh.deposit-1.2.2/docs/specs/spec-meta-deposit.rst`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/mypy.ini` & `swh.deposit-1.2.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/setup.py` & `swh.deposit-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/checks.py` & `swh.deposit-1.2.2/swh/deposit/api/checks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/collection.py` & `swh.deposit-1.2.2/swh/deposit/api/collection.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/common.py` & `swh.deposit-1.2.2/swh/deposit/api/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/content.py` & `swh.deposit-1.2.2/swh/deposit/api/content.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/converters.py` & `swh.deposit-1.2.2/swh/deposit/api/converters.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/edit.py` & `swh.deposit-1.2.2/swh/deposit/api/edit.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/edit_media.py` & `swh.deposit-1.2.2/swh/deposit/api/edit_media.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/private/__init__.py` & `swh.deposit-1.2.2/swh/deposit/api/private/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/private/deposit_check.py` & `swh.deposit-1.2.2/swh/deposit/api/private/deposit_check.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/private/deposit_list.py` & `swh.deposit-1.2.2/swh/deposit/api/private/deposit_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/private/deposit_read.py` & `swh.deposit-1.2.2/swh/deposit/api/private/deposit_read.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/private/deposit_update_status.py` & `swh.deposit-1.2.2/swh/deposit/api/private/deposit_update_status.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/private/urls.py` & `swh.deposit-1.2.2/swh/deposit/api/private/urls.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/service_document.py` & `swh.deposit-1.2.2/swh/deposit/api/service_document.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/state.py` & `swh.deposit-1.2.2/swh/deposit/api/state.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/sword_edit.py` & `swh.deposit-1.2.2/swh/deposit/api/sword_edit.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/urls.py` & `swh.deposit-1.2.2/swh/deposit/api/urls.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/api/utils.py` & `swh.deposit-1.2.2/swh/deposit/api/utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/auth.py` & `swh.deposit-1.2.2/swh/deposit/auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/cli/__init__.py` & `swh.deposit-1.2.2/swh/deposit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/cli/admin.py` & `swh.deposit-1.2.2/swh/deposit/cli/admin.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/cli/client.py` & `swh.deposit-1.2.2/swh/deposit/cli/client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/client.py` & `swh.deposit-1.2.2/swh/deposit/client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/config.py` & `swh.deposit-1.2.2/swh/deposit/config.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/errors.py` & `swh.deposit-1.2.2/swh/deposit/errors.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/exception.py` & `swh.deposit-1.2.2/swh/deposit/exception.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/loader/checker.py` & `swh.deposit-1.2.2/swh/deposit/loader/checker.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/loader/tasks.py` & `swh.deposit-1.2.2/swh/deposit/loader/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/manage.py` & `swh.deposit-1.2.2/swh/deposit/manage.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0001_initial.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0002_depositrequest_archive.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0002_depositrequest_archive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0003_temporaryarchive.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0003_temporaryarchive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0005_auto_20171019_1436.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0005_auto_20171019_1436.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0006_depositclient_url.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0006_depositclient_url.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0008_auto_20171130_1513.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0008_auto_20171130_1513.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0009_deposit_parent.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0009_deposit_parent.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0010_auto_20180110_0953.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0010_auto_20180110_0953.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0011_auto_20180115_1510.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0011_auto_20180115_1510.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0012_deposit_status_detail.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0012_deposit_status_detail.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0014_auto_20180720_1221.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0014_auto_20180720_1221.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0015_depositrequest_typemigration.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0015_depositrequest_typemigration.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0016_auto_20190507_1408.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0016_auto_20190507_1408.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0017_auto_20190925_0906.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0017_auto_20190925_0906.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0018_migrate_swhids.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0018_migrate_swhids.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0019_auto_20200519_1035.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0019_auto_20200519_1035.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0020_auto_20200929_0855.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0020_auto_20200929_0855.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0021_deposit_origin_url_20201124_1438.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/migrations/0022_auto_20220223_1542.py` & `swh.deposit-1.2.2/swh/deposit/migrations/0022_auto_20220223_1542.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/models.py` & `swh.deposit-1.2.2/swh/deposit/models.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/parsers.py` & `swh.deposit-1.2.2/swh/deposit/parsers.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/settings/common.py` & `swh.deposit-1.2.2/swh/deposit/settings/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/settings/development.py` & `swh.deposit-1.2.2/swh/deposit/settings/development.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/settings/production.py` & `swh.deposit-1.2.2/swh/deposit/settings/production.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/settings/testing.py` & `swh.deposit-1.2.2/swh/deposit/settings/testing.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/css/bootstrap-responsive.min.css` & `swh.deposit-1.2.2/swh/deposit/static/css/bootstrap-responsive.min.css`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/css/style.css` & `swh.deposit-1.2.2/swh/deposit/static/css/style.css`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/img/arrow-up-small.png` & `swh.deposit-1.2.2/swh/deposit/static/img/arrow-up-small.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-32x32.png` & `swh.deposit-1.2.2/swh/deposit/static/img/icons/swh-logo-32x32.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png` & `swh.deposit-1.2.2/swh/deposit/static/img/icons/swh-logo-deposit-180x180.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png` & `swh.deposit-1.2.2/swh/deposit/static/img/icons/swh-logo-deposit-192x192.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png` & `swh.deposit-1.2.2/swh/deposit/static/img/icons/swh-logo-deposit-270x270.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/img/swh-logo-deposit.png` & `swh.deposit-1.2.2/swh/deposit/static/img/swh-logo-deposit.png`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/static/img/swh-logo-deposit.svg` & `swh.deposit-1.2.2/swh/deposit/static/img/swh-logo-deposit.svg`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/templates/deposit/content.xml` & `swh.deposit-1.2.2/swh/deposit/templates/deposit/content.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/templates/deposit/deposit_receipt.xml` & `swh.deposit-1.2.2/swh/deposit/templates/deposit/deposit_receipt.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/templates/deposit/service_document.xml` & `swh.deposit-1.2.2/swh/deposit/templates/deposit/service_document.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/templates/deposit/state.xml` & `swh.deposit-1.2.2/swh/deposit/templates/deposit/state.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/templates/homepage.html` & `swh.deposit-1.2.2/swh/deposit/templates/homepage.html`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/templates/layout.html` & `swh.deposit-1.2.2/swh/deposit/templates/layout.html`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/conftest.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_basic_auth.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_basic_auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_checks.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_checks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_collection.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_add_to_origin.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_add_to_origin.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_list.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_atom.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_post_atom.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_binary.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_post_binary.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_post_multipart.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_post_multipart.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_collection_reuse_slug.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_collection_reuse_slug.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_converters.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_delete.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_delete.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_check.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_check.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_list.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_list.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_read_archive.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_read_archive.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_read_metadata.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_read_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_private_update_status.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_private_update_status.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_schedule.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_schedule.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_state.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_state.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_update.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update_atom.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_update_atom.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_deposit_update_binary.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_deposit_update_binary.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_exception.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_exception.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_get_file.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_get_file.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_keycloak_auth.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_keycloak_auth.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_parsers.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_parsers.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/api/test_service_document.py` & `swh.deposit-1.2.2/swh/deposit/tests/api/test_service_document.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/cli/test_admin.py` & `swh.deposit-1.2.2/swh/deposit/tests/cli/test_admin.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/cli/test_client.py` & `swh.deposit-1.2.2/swh/deposit/tests/cli/test_client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/common.py` & `swh.deposit-1.2.2/swh/deposit/tests/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/conftest.py` & `swh.deposit-1.2.2/swh/deposit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/codemeta-sample.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/codemeta-sample.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-deposit-binary.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-no-origin-url.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-add-to-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-both-add-to-origin-and-external-id.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-both-add-to-origin-and-external-id.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-both-create-origin-and-add-to-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data-with-swhid.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data-with-swhid.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data0.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data0.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data1.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data1.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data2.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data2.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-data3.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-data3.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-list-deposits-page1.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-list-deposits-page2.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/entry-list-deposits.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/entry-list-deposits.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-decimal.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/error-with-decimal.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-external-identifier-and-create-origin.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/error-with-external-identifier-and-create-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/error-with-reference-and-create-origin.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/atom/metadata.xml` & `swh.deposit-1.2.2/swh/deposit/tests/data/atom/metadata.xml`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.swh.test/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.swh.test/1_test` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.swh.test/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.list/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.list/1_test,page=1,page_size=10`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_media`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_metadata`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadata/1_test_666_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.metadataonly/1_test`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.status/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.status/1_test_1033_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_servicedocument`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_atom`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_123_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status` & `swh.deposit-1.2.2/swh/deposit/tests/data/https_deposit.test.updateswhid/1_test_321_status`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/loader/common.py` & `swh.deposit-1.2.2/swh/deposit/tests/loader/common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/loader/conftest.py` & `swh.deposit-1.2.2/swh/deposit/tests/loader/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta` & `swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_meta`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw` & `swh.deposit-1.2.2/swh/deposit/tests/loader/data/https_deposit.softwareheritage.org/1_private_test_999_raw`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/loader/test_checker.py` & `swh.deposit-1.2.2/swh/deposit/tests/loader/test_checker.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/loader/test_client.py` & `swh.deposit-1.2.2/swh/deposit/tests/loader/test_client.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/loader/test_tasks.py` & `swh.deposit-1.2.2/swh/deposit/tests/loader/test_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/test_backend.py` & `swh.deposit-1.2.2/swh/deposit/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/test_client_module.py` & `swh.deposit-1.2.2/swh/deposit/tests/test_client_module.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/test_common.py` & `swh.deposit-1.2.2/swh/deposit/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/test_config.py` & `swh.deposit-1.2.2/swh/deposit/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/test_gunicorn_config.py` & `swh.deposit-1.2.2/swh/deposit/tests/test_gunicorn_config.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/test_init.py` & `swh.deposit-1.2.2/swh/deposit/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/test_migrations.py` & `swh.deposit-1.2.2/swh/deposit/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/tests/test_utils.py` & `swh.deposit-1.2.2/swh/deposit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/urls.py` & `swh.deposit-1.2.2/swh/deposit/urls.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/utils.py` & `swh.deposit-1.2.2/swh/deposit/utils.py`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/xsd/codemeta.xsd` & `swh.deposit-1.2.2/swh/deposit/xsd/codemeta.xsd`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh/deposit/xsd/swh.xsd` & `swh.deposit-1.2.2/swh/deposit/xsd/swh.xsd`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh.deposit.egg-info/PKG-INFO` & `swh.deposit-1.2.2/swh.deposit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.deposit
-Version: 1.2.1
+Version: 1.2.2
 Summary: Software Heritage Deposit Server
 Home-page: https://forge.softwareheritage.org/source/swh-deposit/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-deposit
```

### Comparing `swh.deposit-1.2.1/swh.deposit.egg-info/SOURCES.txt` & `swh.deposit-1.2.2/swh.deposit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.deposit-1.2.1/swh.deposit.egg-info/requires.txt` & `swh.deposit-1.2.2/swh.deposit.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 click
 iso8601
 requests
 sentry-sdk
 swh.core[http]>=0.4
 swh.model>=4.4.0
-swh.scheduler
 
 [server]
 django
 djangorestframework
 psycopg2
 setuptools
 xmlschema
```

### Comparing `swh.deposit-1.2.1/tox.ini` & `swh.deposit-1.2.2/tox.ini`

 * *Files identical despite different names*

