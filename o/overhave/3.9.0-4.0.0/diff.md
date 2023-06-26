# Comparing `tmp/overhave-3.9.0.tar.gz` & `tmp/overhave-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overhave-3.9.0.tar", max compression
+gzip compressed data, was "overhave-4.0.0.tar", max compression
```

## Comparing `overhave-3.9.0.tar` & `overhave-4.0.0.tar`

### file list

```diff
@@ -1,236 +1,245 @@
--rw-r--r--   0        0        0    23315 2022-08-22 13:34:13.941154 overhave-3.9.0/README.rst
--rw-r--r--   0        0        0     3075 2022-08-22 13:34:13.953154 overhave-3.9.0/overhave/__init__.py
--rw-r--r--   0        0        0       63 2022-08-22 13:34:13.953154 overhave-3.9.0/overhave/admin/__init__.py
--rw-r--r--   0        0        0     5109 2022-08-22 13:34:13.953154 overhave-3.9.0/overhave/admin/app.py
--rw-r--r--   0        0        0   735118 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/files/ace-src/ace.js
--rw-r--r--   0        0        0     5426 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/files/ace-src/mode-gherkin.js
--rw-r--r--   0        0        0     1263 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/files/css/overhave.css
--rw-r--r--   0        0        0    38062 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/files/favicon.ico
--rw-r--r--   0        0        0      138 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/flask/__init__.py
--rw-r--r--   0        0        0     1819 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/flask/flask_admin.py
--rw-r--r--   0        0        0      459 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/flask/flask_app.py
--rw-r--r--   0        0        0      946 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/flask/login_manager.py
--rw-r--r--   0        0        0      187 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/templates/draft_detail.html
--rw-r--r--   0        0        0      405 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/templates/emulation.html
--rw-r--r--   0        0        0      194 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/templates/emulation_create.html
--rw-r--r--   0        0        0      190 2022-08-22 13:34:13.957154 overhave-3.9.0/overhave/admin/templates/emulation_edit.html
--rw-r--r--   0        0        0      860 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/emulation_run_detail.html
--rw-r--r--   0        0        0    10445 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/feature.html
--rw-r--r--   0        0        0      404 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/feature_create.html
--rw-r--r--   0        0        0      400 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/feature_edit.html
--rw-r--r--   0        0        0      177 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/index.html
--rw-r--r--   0        0        0     2414 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/login.html
--rw-r--r--   0        0        0      149 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/overhave_master.html
--rw-r--r--   0        0        0     1696 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_run.html
--rw-r--r--   0        0        0     1469 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_run_detail.html
--rw-r--r--   0        0        0      189 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_run_list.html
--rw-r--r--   0        0        0      606 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_user.html
--rw-r--r--   0        0        0      210 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_user_create.html
--rw-r--r--   0        0        0      208 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/templates/test_user_edit.html
--rw-r--r--   0        0        0      451 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/__init__.py
--rw-r--r--   0        0        0     1382 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/access.py
--rw-r--r--   0        0        0     2914 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/base.py
--rw-r--r--   0        0        0     1105 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/draft.py
--rw-r--r--   0        0        0     3441 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/emulation.py
--rw-r--r--   0        0        0     1620 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/emulation_run.py
--rw-r--r--   0        0        0     9557 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/feature.py
--rw-r--r--   0        0        0      306 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/formatters/__init__.py
--rw-r--r--   0        0        0     5169 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/formatters/formatters.py
--rw-r--r--   0        0        0      669 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/formatters/helpers.py
--rw-r--r--   0        0        0     1429 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/formatters/safe_formatter.py
--rw-r--r--   0        0        0       51 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/index/__init__.py
--rw-r--r--   0        0        0     1680 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/index/custom_page.py
--rw-r--r--   0        0        0     1536 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/index/login_form.py
--rw-r--r--   0        0        0     2658 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/index/view.py
--rw-r--r--   0        0        0     1794 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/scenario_test_run.py
--rw-r--r--   0        0        0     1378 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/tag.py
--rw-r--r--   0        0        0     3603 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/admin/views/testing_users.py
--rw-r--r--   0        0        0       52 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/__init__.py
--rw-r--r--   0        0        0     6002 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/app.py
--rw-r--r--   0        0        0      212 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/asgi.py
--rw-r--r--   0        0        0      143 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/auth/__init__.py
--rw-r--r--   0        0        0      348 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/auth/models.py
--rw-r--r--   0        0        0     1271 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/auth/regular.py
--rw-r--r--   0        0        0      902 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/auth/token.py
--rw-r--r--   0        0        0     1914 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/deps.py
--rw-r--r--   0        0        0      848 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/settings.py
--rw-r--r--   0        0        0      580 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/__init__.py
--rw-r--r--   0        0        0     1304 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/auth_views.py
--rw-r--r--   0        0        0      574 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/emulation_views.py
--rw-r--r--   0        0        0      586 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/extra_views.py
--rw-r--r--   0        0        0      491 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/feature_type_views.py
--rw-r--r--   0        0        0     1224 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/feature_views.py
--rw-r--r--   0        0        0      993 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/tags_views.py
--rw-r--r--   0        0        0     1816 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/testrun_views.py
--rw-r--r--   0        0        0     4383 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/api/views/testuser_views.py
--rw-r--r--   0        0        0     3802 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/base_settings.py
--rw-r--r--   0        0        0      164 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/__init__.py
--rw-r--r--   0        0        0      553 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/admin.py
--rw-r--r--   0        0        0      534 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/api.py
--rw-r--r--   0        0        0      643 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/consumers.py
--rw-r--r--   0        0        0       84 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/db_cmds/__init__.py
--rw-r--r--   0        0        0      830 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/db_cmds/group.py
--rw-r--r--   0        0        0     1520 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/db_cmds/regular.py
--rw-r--r--   0        0        0      358 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/group.py
--rw-r--r--   0        0        0     3048 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/s3.py
--rw-r--r--   0        0        0     1567 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/cli/synchronizer.py
--rw-r--r--   0        0        0      443 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/__init__.py
--rw-r--r--   0        0        0     2483 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/base.py
--rw-r--r--   0        0        0     1352 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/statuses.py
--rw-r--r--   0        0        0     9112 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/tables.py
--rw-r--r--   0        0        0     1051 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/users.py
--rw-r--r--   0        0        0     1239 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/db/utils.py
--rw-r--r--   0        0        0       46 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/emulation/__init__.py
--rw-r--r--   0        0        0     3629 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/emulation/emulator.py
--rw-r--r--   0        0        0      924 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/__init__.py
--rw-r--r--   0        0        0     1231 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/archiver.py
--rw-r--r--   0        0        0      247 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/__init__.py
--rw-r--r--   0        0        0      347 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/abstract.py
--rw-r--r--   0        0        0      497 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/base.py
--rw-r--r--   0        0        0      588 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/default.py
--rw-r--r--   0        0        0      116 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/ldap/__init__.py
--rw-r--r--   0        0        0     2928 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/ldap/manager.py
--rw-r--r--   0        0        0      198 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/ldap/settings.py
--rw-r--r--   0        0        0     1394 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/secret_mixin.py
--rw-r--r--   0        0        0     1289 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/auth_managers/simple.py
--rw-r--r--   0        0        0      169 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/feature/__init__.py
--rw-r--r--   0        0        0      455 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/feature/abstract.py
--rw-r--r--   0        0        0      221 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/feature/errors.py
--rw-r--r--   0        0        0     2839 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/feature/extractor.py
--rw-r--r--   0        0        0     1092 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/file_extractor.py
--rw-r--r--   0        0        0     1760 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/git_initializer.py
--rw-r--r--   0        0        0       55 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/language/__init__.py
--rw-r--r--   0        0        0     1288 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/language/prefixes.py
--rw-r--r--   0        0        0      102 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/report_manager/__init__.py
--rw-r--r--   0        0        0      447 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/report_manager/models.py
--rw-r--r--   0        0        0     5844 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/report_manager/report_manager.py
--rw-r--r--   0        0        0     7181 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/entities/settings.py
--rw-r--r--   0        0        0       54 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/extra/__init__.py
--rw-r--r--   0        0        0      386 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/extra/prefixes.py
--rw-r--r--   0        0        0      739 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/__init__.py
--rw-r--r--   0        0        0     7159 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/base_factory.py
--rw-r--r--   0        0        0      418 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/__init__.py
--rw-r--r--   0        0        0      306 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/abstract_consumer.py
--rw-r--r--   0        0        0     4135 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/admin_factory.py
--rw-r--r--   0        0        0      994 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/emulation_factory.py
--rw-r--r--   0        0        0     3691 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/publication_factory.py
--rw-r--r--   0        0        0      486 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/s3_init_factory.py
--rw-r--r--   0        0        0     2163 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/synchronizer_factory.py
--rw-r--r--   0        0        0     1623 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/components/test_execution_factory.py
--rw-r--r--   0        0        0     1659 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/consumer_factory.py
--rw-r--r--   0        0        0      550 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/__init__.py
--rw-r--r--   0        0        0     2974 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/admin_context.py
--rw-r--r--   0        0        0     3702 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/base_context.py
--rw-r--r--   0        0        0      538 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/emulation_context.py
--rw-r--r--   0        0        0     2085 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/publication_context.py
--rw-r--r--   0        0        0     1332 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/synchronizer_context.py
--rw-r--r--   0        0        0     2581 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/context/test_execution_context.py
--rw-r--r--   0        0        0      769 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/factory/getters.py
--rw-r--r--   0        0        0      342 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/__init__.py
--rw-r--r--   0        0        0      365 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/abstract_publisher.py
--rw-r--r--   0        0        0     4659 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/base_publisher.py
--rw-r--r--   0        0        0     5369 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/git_publisher.py
--rw-r--r--   0        0        0      224 2022-08-22 13:34:13.961154 overhave-3.9.0/overhave/publication/gitlab/__init__.py
--rw-r--r--   0        0        0     4742 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/gitlab_publisher.py
--rw-r--r--   0        0        0     1446 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/settings.py
--rw-r--r--   0        0        0      171 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/tokenizer/__init__.py
--rw-r--r--   0        0        0     2065 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/tokenizer/client.py
--rw-r--r--   0        0        0      894 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/gitlab/tokenizer/settings.py
--rw-r--r--   0        0        0      180 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/objects.py
--rw-r--r--   0        0        0      834 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/settings.py
--rw-r--r--   0        0        0      119 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/stash/__init__.py
--rw-r--r--   0        0        0     1697 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/stash/settings.py
--rw-r--r--   0        0        0     3814 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/publication/stash/stash_publisher.py
--rw-r--r--   0        0        0      371 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/__init__.py
--rw-r--r--   0        0        0     3584 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/config_injector.py
--rw-r--r--   0        0        0      827 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/deps.py
--rw-r--r--   0        0        0      530 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/__init__.py
--rw-r--r--   0        0        0      305 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/__init__.py
--rw-r--r--   0        0        0      952 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
--rw-r--r--   0        0        0     1111 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/links.py
--rw-r--r--   0        0        0     1276 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/severity.py
--rw-r--r--   0        0        0     2470 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
--rw-r--r--   0        0        0     1648 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/bdd_item.py
--rw-r--r--   0        0        0      994 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/parsed_info.py
--rw-r--r--   0        0        0     2900 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/helpers/tag_controller.py
--rw-r--r--   0        0        0     7321 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/plugin.py
--rw-r--r--   0        0        0     2274 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/plugin_resolver.py
--rw-r--r--   0        0        0     3957 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/pytest_plugin/proxy_manager.py
--rw-r--r--   0        0        0      498 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/__init__.py
--rw-r--r--   0        0        0      157 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/compiler/__init__.py
--rw-r--r--   0        0        0     5240 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/compiler/compiler.py
--rw-r--r--   0        0        0      631 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/compiler/settings.py
--rw-r--r--   0        0        0      150 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/file_manager/__init__.py
--rw-r--r--   0        0        0     3494 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/file_manager/file_manager.py
--rw-r--r--   0        0        0     2803 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/file_manager/settings.py
--rw-r--r--   0        0        0      230 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/parser/__init__.py
--rw-r--r--   0        0        0      918 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/parser/models.py
--rw-r--r--   0        0        0     8480 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/parser/parser.py
--rw-r--r--   0        0        0      263 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/parser/settings.py
--rw-r--r--   0        0        0      235 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/prefix_mixin.py
--rw-r--r--   0        0        0     2786 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/scenario/validator.py
--rw-r--r--   0        0        0     1229 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/__init__.py
--rw-r--r--   0        0        0     1214 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/api_auth_storage.py
--rw-r--r--   0        0        0     3694 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/converters.py
--rw-r--r--   0        0        0     4377 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/draft_storage.py
--rw-r--r--   0        0        0     6055 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/emulation_storage.py
--rw-r--r--   0        0        0     4729 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/feature_storage.py
--rw-r--r--   0        0        0     1802 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/feature_tag_storage.py
--rw-r--r--   0        0        0     2013 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/feature_type_storage.py
--rw-r--r--   0        0        0     2343 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/scenario_storage.py
--rw-r--r--   0        0        0      617 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/system_user_group_storage.py
--rw-r--r--   0        0        0     2896 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/system_user_storage.py
--rw-r--r--   0        0        0     2900 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/test_run_storage.py
--rw-r--r--   0        0        0     4560 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/storage/test_user_storage.py
--rw-r--r--   0        0        0      192 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/synchronization/__init__.py
--rw-r--r--   0        0        0      260 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/synchronization/abstract.py
--rw-r--r--   0        0        0     3737 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/synchronization/storage_manager.py
--rw-r--r--   0        0        0     6564 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/synchronization/synchronizer.py
--rw-r--r--   0        0        0      263 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/__init__.py
--rw-r--r--   0        0        0     4360 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/executor.py
--rw-r--r--   0        0        0      575 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/objects.py
--rw-r--r--   0        0        0     1596 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/settings.py
--rw-r--r--   0        0        0     3546 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/step_collector.py
--rw-r--r--   0        0        0     1672 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/test_execution/test_runner.py
--rw-r--r--   0        0        0      933 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/__init__.py
--rw-r--r--   0        0        0      658 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/__init__.py
--rw-r--r--   0        0        0      122 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/api_client/__init__.py
--rw-r--r--   0        0        0     1841 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/api_client/authenticator.py
--rw-r--r--   0        0        0      237 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/api_client/models.py
--rw-r--r--   0        0        0      485 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/api_client/settings.py
--rw-r--r--   0        0        0      208 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/__init__.py
--rw-r--r--   0        0        0      547 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/auth.py
--rw-r--r--   0        0        0     2282 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/client.py
--rw-r--r--   0        0        0      112 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/objects.py
--rw-r--r--   0        0        0      743 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/base_client/settings.py
--rw-r--r--   0        0        0      289 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/__init__.py
--rw-r--r--   0        0        0     1847 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/client.py
--rw-r--r--   0        0        0     1109 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/models.py
--rw-r--r--   0        0        0      144 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/objects.py
--rw-r--r--   0        0        0      409 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/settings.py
--rw-r--r--   0        0        0      707 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/gitlab_client/utils.py
--rw-r--r--   0        0        0      326 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/stash_client/__init__.py
--rw-r--r--   0        0        0     2115 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/stash_client/client.py
--rw-r--r--   0        0        0     2807 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/stash_client/models.py
--rw-r--r--   0        0        0      555 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/http/stash_client/settings.py
--rw-r--r--   0        0        0      109 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/ldap/__init__.py
--rw-r--r--   0        0        0     1936 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/ldap/authenticator.py
--rw-r--r--   0        0        0      420 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/ldap/settings.py
--rw-r--r--   0        0        0      336 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/__init__.py
--rw-r--r--   0        0        0     2672 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/consumer.py
--rw-r--r--   0        0        0     2335 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/objects.py
--rw-r--r--   0        0        0     1061 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/producer.py
--rw-r--r--   0        0        0     1396 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/runner.py
--rw-r--r--   0        0        0      435 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/redis/template.py
--rw-r--r--   0        0        0      132 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/__init__.py
--rw-r--r--   0        0        0     8513 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/manager.py
--rw-r--r--   0        0        0     2122 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/models.py
--rw-r--r--   0        0        0      181 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/objects.py
--rw-r--r--   0        0        0      913 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/transport/s3/settings.py
--rw-r--r--   0        0        0      103 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/utils/__init__.py
--rw-r--r--   0        0        0       84 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/utils/mocks.py
--rw-r--r--   0        0        0      139 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/utils/time.py
--rw-r--r--   0        0        0      179 2022-08-22 13:34:13.965154 overhave-3.9.0/overhave/utils/url.py
--rw-r--r--   0        0        0     3493 2022-08-22 13:34:13.969154 overhave-3.9.0/pyproject.toml
--rw-r--r--   0        0        0    27109 2022-08-22 13:36:02.605930 overhave-3.9.0/setup.py
--rw-r--r--   0        0        0    25560 2022-08-22 13:36:02.607434 overhave-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0    23136 2023-06-26 10:51:26.726732 overhave-4.0.0/README.rst
+-rw-r--r--   0        0        0     3193 2023-06-26 10:51:26.746732 overhave-4.0.0/overhave/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-26 10:51:26.746732 overhave-4.0.0/overhave/admin/__init__.py
+-rw-r--r--   0        0        0     5172 2023-06-26 10:51:26.746732 overhave-4.0.0/overhave/admin/app.py
+-rw-r--r--   0        0        0   735118 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/files/ace-src/ace.js
+-rw-r--r--   0        0        0     5426 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/files/ace-src/mode-gherkin.js
+-rw-r--r--   0        0        0     1263 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/files/css/overhave.css
+-rw-r--r--   0        0        0    38062 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/files/favicon.ico
+-rw-r--r--   0        0        0      138 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/flask/__init__.py
+-rw-r--r--   0        0        0     1819 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/flask/flask_admin.py
+-rw-r--r--   0        0        0      287 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/flask/flask_app.py
+-rw-r--r--   0        0        0     2134 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/flask/login_manager.py
+-rw-r--r--   0        0        0      187 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/draft_detail.html
+-rw-r--r--   0        0        0      405 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/emulation.html
+-rw-r--r--   0        0        0      194 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/emulation_create.html
+-rw-r--r--   0        0        0      190 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/emulation_edit.html
+-rw-r--r--   0        0        0      860 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/emulation_run_detail.html
+-rw-r--r--   0        0        0    10071 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/feature.html
+-rw-r--r--   0        0        0      404 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/feature_create.html
+-rw-r--r--   0        0        0      465 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/feature_edit.html
+-rw-r--r--   0        0        0      177 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/index.html
+-rw-r--r--   0        0        0     2414 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/login.html
+-rw-r--r--   0        0        0      149 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/overhave_master.html
+-rw-r--r--   0        0        0     1696 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/test_run.html
+-rw-r--r--   0        0        0     1535 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/test_run_detail.html
+-rw-r--r--   0        0        0      189 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/test_run_list.html
+-rw-r--r--   0        0        0      606 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/test_user.html
+-rw-r--r--   0        0        0      210 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/test_user_create.html
+-rw-r--r--   0        0        0      208 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/templates/test_user_edit.html
+-rw-r--r--   0        0        0      451 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/__init__.py
+-rw-r--r--   0        0        0     1386 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/access.py
+-rw-r--r--   0        0        0     2914 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/base.py
+-rw-r--r--   0        0        0     1105 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/draft.py
+-rw-r--r--   0        0        0     3407 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/emulation.py
+-rw-r--r--   0        0        0     1620 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/emulation_run.py
+-rw-r--r--   0        0        0    10224 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/feature.py
+-rw-r--r--   0        0        0      306 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/formatters/__init__.py
+-rw-r--r--   0        0        0     4997 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/formatters/formatters.py
+-rw-r--r--   0        0        0      631 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/formatters/helpers.py
+-rw-r--r--   0        0        0     1404 2023-06-26 10:51:26.750732 overhave-4.0.0/overhave/admin/views/formatters/safe_formatter.py
+-rw-r--r--   0        0        0       51 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/admin/views/index/__init__.py
+-rw-r--r--   0        0        0     1648 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/admin/views/index/custom_page.py
+-rw-r--r--   0        0        0     1578 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/admin/views/index/login_form.py
+-rw-r--r--   0        0        0     2645 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/admin/views/index/view.py
+-rw-r--r--   0        0        0     1794 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/admin/views/scenario_test_run.py
+-rw-r--r--   0        0        0     1378 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/admin/views/tag.py
+-rw-r--r--   0        0        0     3659 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/admin/views/testing_users.py
+-rw-r--r--   0        0        0       52 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/__init__.py
+-rw-r--r--   0        0        0     5977 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/app.py
+-rw-r--r--   0        0        0      216 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/asgi.py
+-rw-r--r--   0        0        0      143 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/auth/__init__.py
+-rw-r--r--   0        0        0      348 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/auth/models.py
+-rw-r--r--   0        0        0     1271 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/auth/regular.py
+-rw-r--r--   0        0        0      867 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/auth/token.py
+-rw-r--r--   0        0        0     2422 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/deps.py
+-rw-r--r--   0        0        0      848 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/settings.py
+-rw-r--r--   0        0        0      580 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/__init__.py
+-rw-r--r--   0        0        0     1304 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/auth_views.py
+-rw-r--r--   0        0        0      550 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/emulation_views.py
+-rw-r--r--   0        0        0      586 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/extra_views.py
+-rw-r--r--   0        0        0      461 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/feature_type_views.py
+-rw-r--r--   0        0        0     1184 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/feature_views.py
+-rw-r--r--   0        0        0      969 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/tags_views.py
+-rw-r--r--   0        0        0     2041 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/testrun_views.py
+-rw-r--r--   0        0        0     4486 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/api/views/testuser_views.py
+-rw-r--r--   0        0        0     4108 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/base_settings.py
+-rw-r--r--   0        0        0      164 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/__init__.py
+-rw-r--r--   0        0        0      557 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/admin.py
+-rw-r--r--   0        0        0      534 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/api.py
+-rw-r--r--   0        0        0      647 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/consumers.py
+-rw-r--r--   0        0        0       84 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/db_cmds/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/db_cmds/group.py
+-rw-r--r--   0        0        0     1755 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/db_cmds/regular.py
+-rw-r--r--   0        0        0      358 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/group.py
+-rw-r--r--   0        0        0     3048 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/s3.py
+-rw-r--r--   0        0        0     1573 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/cli/synchronizer.py
+-rw-r--r--   0        0        0      455 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/db/__init__.py
+-rw-r--r--   0        0        0     3283 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/db/base.py
+-rw-r--r--   0        0        0     1349 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/db/statuses.py
+-rw-r--r--   0        0        0     8141 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/db/tables.py
+-rw-r--r--   0        0        0      795 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/db/users.py
+-rw-r--r--   0        0        0     1249 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/db/utils.py
+-rw-r--r--   0        0        0       46 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/emulation/__init__.py
+-rw-r--r--   0        0        0     4103 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/emulation/emulator.py
+-rw-r--r--   0        0        0      897 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/__init__.py
+-rw-r--r--   0        0        0     1231 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/archiver.py
+-rw-r--r--   0        0        0      247 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/__init__.py
+-rw-r--r--   0        0        0      316 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/abstract.py
+-rw-r--r--   0        0        0      497 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/base.py
+-rw-r--r--   0        0        0      557 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/default.py
+-rw-r--r--   0        0        0      116 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/ldap/__init__.py
+-rw-r--r--   0        0        0     2891 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/ldap/manager.py
+-rw-r--r--   0        0        0      198 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/ldap/settings.py
+-rw-r--r--   0        0        0     1394 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/secret_mixin.py
+-rw-r--r--   0        0        0     1258 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/auth_managers/simple.py
+-rw-r--r--   0        0        0      169 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/feature/__init__.py
+-rw-r--r--   0        0        0      425 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/feature/abstract.py
+-rw-r--r--   0        0        0      221 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/feature/errors.py
+-rw-r--r--   0        0        0     2748 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/feature/extractor.py
+-rw-r--r--   0        0        0     1098 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/file_extractor.py
+-rw-r--r--   0        0        0     1760 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/git_initializer.py
+-rw-r--r--   0        0        0       55 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/language/__init__.py
+-rw-r--r--   0        0        0     1198 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/language/prefixes.py
+-rw-r--r--   0        0        0      102 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/report_manager/__init__.py
+-rw-r--r--   0        0        0      415 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/report_manager/models.py
+-rw-r--r--   0        0        0     5825 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/report_manager/report_manager.py
+-rw-r--r--   0        0        0     6633 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/entities/settings.py
+-rw-r--r--   0        0        0       54 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/extra/__init__.py
+-rw-r--r--   0        0        0      386 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/extra/prefixes.py
+-rw-r--r--   0        0        0      739 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/__init__.py
+-rw-r--r--   0        0        0     7209 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/base_factory.py
+-rw-r--r--   0        0        0      418 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/components/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/components/abstract_consumer.py
+-rw-r--r--   0        0        0     4555 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/components/admin_factory.py
+-rw-r--r--   0        0        0     1312 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/components/emulation_factory.py
+-rw-r--r--   0        0        0     3960 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/components/publication_factory.py
+-rw-r--r--   0        0        0      486 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/components/s3_init_factory.py
+-rw-r--r--   0        0        0     2184 2023-06-26 10:51:26.754732 overhave-4.0.0/overhave/factory/components/synchronizer_factory.py
+-rw-r--r--   0        0        0     1888 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/components/test_execution_factory.py
+-rw-r--r--   0        0        0     2045 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/consumer_factory.py
+-rw-r--r--   0        0        0      550 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/context/__init__.py
+-rw-r--r--   0        0        0     2950 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/context/admin_context.py
+-rw-r--r--   0        0        0     4028 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/context/base_context.py
+-rw-r--r--   0        0        0      506 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/context/emulation_context.py
+-rw-r--r--   0        0        0     2032 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/context/publication_context.py
+-rw-r--r--   0        0        0     1288 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/context/synchronizer_context.py
+-rw-r--r--   0        0        0     2519 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/context/test_execution_context.py
+-rw-r--r--   0        0        0      769 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/factory/getters.py
+-rw-r--r--   0        0        0      353 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/metrics/__init__.py
+-rw-r--r--   0        0        0      193 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/metrics/client/__init__.py
+-rw-r--r--   0        0        0     3140 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/metrics/client/container.py
+-rw-r--r--   0        0        0      983 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/metrics/getters.py
+-rw-r--r--   0        0        0      342 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/__init__.py
+-rw-r--r--   0        0        0      399 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/abstract_publisher.py
+-rw-r--r--   0        0        0     4126 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/base_publisher.py
+-rw-r--r--   0        0        0      532 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/errors.py
+-rw-r--r--   0        0        0     5036 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/git_publisher.py
+-rw-r--r--   0        0        0      224 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/gitlab/__init__.py
+-rw-r--r--   0        0        0     4316 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/gitlab/gitlab_publisher.py
+-rw-r--r--   0        0        0     1408 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/gitlab/settings.py
+-rw-r--r--   0        0        0      171 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/gitlab/tokenizer/__init__.py
+-rw-r--r--   0        0        0     2157 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/gitlab/tokenizer/client.py
+-rw-r--r--   0        0        0     1015 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/gitlab/tokenizer/settings.py
+-rw-r--r--   0        0        0      178 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/objects.py
+-rw-r--r--   0        0        0      877 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/settings.py
+-rw-r--r--   0        0        0      119 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/stash/__init__.py
+-rw-r--r--   0        0        0     1672 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/stash/settings.py
+-rw-r--r--   0        0        0     4431 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/publication/stash/stash_publisher.py
+-rw-r--r--   0        0        0      371 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0     3538 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/config_injector.py
+-rw-r--r--   0        0        0      827 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/deps.py
+-rw-r--r--   0        0        0      530 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/__init__.py
+-rw-r--r--   0        0        0      305 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
+-rw-r--r--   0        0        0     1102 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/links.py
+-rw-r--r--   0        0        0     1260 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/severity.py
+-rw-r--r--   0        0        0     2452 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
+-rw-r--r--   0        0        0     1638 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/bdd_item.py
+-rw-r--r--   0        0        0      981 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/parsed_info.py
+-rw-r--r--   0        0        0     2874 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/helpers/tag_controller.py
+-rw-r--r--   0        0        0     6192 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/plugin.py
+-rw-r--r--   0        0        0     2223 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/plugin_resolver.py
+-rw-r--r--   0        0        0     3945 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/pytest_plugin/proxy_manager.py
+-rw-r--r--   0        0        0      517 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/__init__.py
+-rw-r--r--   0        0        0      157 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/compiler/__init__.py
+-rw-r--r--   0        0        0     5173 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/compiler/compiler.py
+-rw-r--r--   0        0        0      631 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/compiler/settings.py
+-rw-r--r--   0        0        0      150 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/file_manager/__init__.py
+-rw-r--r--   0        0        0     3495 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/file_manager/file_manager.py
+-rw-r--r--   0        0        0     2820 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/file_manager/settings.py
+-rw-r--r--   0        0        0      230 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/parser/__init__.py
+-rw-r--r--   0        0        0      854 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/parser/models.py
+-rw-r--r--   0        0        0     8442 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/parser/parser.py
+-rw-r--r--   0        0        0      263 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/parser/settings.py
+-rw-r--r--   0        0        0      235 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/prefix_mixin.py
+-rw-r--r--   0        0        0       95 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/validator/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/validator/abstract.py
+-rw-r--r--   0        0        0     1441 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/validator/duplicate_id_mixin.py
+-rw-r--r--   0        0        0      510 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/validator/errors.py
+-rw-r--r--   0        0        0     2827 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/scenario/validator/validator.py
+-rw-r--r--   0        0        0     1226 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/storage/__init__.py
+-rw-r--r--   0        0        0     1180 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/storage/api_auth_storage.py
+-rw-r--r--   0        0        0     3271 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/storage/converters.py
+-rw-r--r--   0        0        0     6178 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/storage/draft_storage.py
+-rw-r--r--   0        0        0     5323 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/storage/emulation_storage.py
+-rw-r--r--   0        0        0     4947 2023-06-26 10:51:26.758732 overhave-4.0.0/overhave/storage/feature_storage.py
+-rw-r--r--   0        0        0     1566 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/storage/feature_tag_storage.py
+-rw-r--r--   0        0        0     2176 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/storage/feature_type_storage.py
+-rw-r--r--   0        0        0     1902 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/storage/scenario_storage.py
+-rw-r--r--   0        0        0      593 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/storage/system_user_group_storage.py
+-rw-r--r--   0        0        0     2464 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/storage/system_user_storage.py
+-rw-r--r--   0        0        0     3054 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/storage/test_run_storage.py
+-rw-r--r--   0        0        0     4451 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/storage/test_user_storage.py
+-rw-r--r--   0        0        0      192 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/synchronization/__init__.py
+-rw-r--r--   0        0        0      260 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/synchronization/abstract.py
+-rw-r--r--   0        0        0     3702 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/synchronization/storage_manager.py
+-rw-r--r--   0        0        0     6973 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/synchronization/synchronizer.py
+-rw-r--r--   0        0        0      307 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/test_execution/__init__.py
+-rw-r--r--   0        0        0     4256 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/test_execution/executor.py
+-rw-r--r--   0        0        0     1056 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/test_execution/objects.py
+-rw-r--r--   0        0        0     1750 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/test_execution/settings.py
+-rw-r--r--   0        0        0     4106 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/test_execution/step_collector.py
+-rw-r--r--   0        0        0     1617 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/test_execution/test_runner.py
+-rw-r--r--   0        0        0      983 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/__init__.py
+-rw-r--r--   0        0        0      623 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/__init__.py
+-rw-r--r--   0        0        0      122 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/api_client/__init__.py
+-rw-r--r--   0        0        0     1810 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/api_client/authenticator.py
+-rw-r--r--   0        0        0      237 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/api_client/models.py
+-rw-r--r--   0        0        0      499 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/api_client/settings.py
+-rw-r--r--   0        0        0      208 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/base_client/__init__.py
+-rw-r--r--   0        0        0      590 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/base_client/auth.py
+-rw-r--r--   0        0        0     2139 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/base_client/client.py
+-rw-r--r--   0        0        0      110 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/base_client/objects.py
+-rw-r--r--   0        0        0     1287 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/base_client/settings.py
+-rw-r--r--   0        0        0      258 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/gitlab_client/__init__.py
+-rw-r--r--   0        0        0     2003 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/gitlab_client/client.py
+-rw-r--r--   0        0        0      609 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/gitlab_client/models.py
+-rw-r--r--   0        0        0      144 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/gitlab_client/objects.py
+-rw-r--r--   0        0        0      377 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/gitlab_client/settings.py
+-rw-r--r--   0        0        0      741 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/gitlab_client/utils.py
+-rw-r--r--   0        0        0      326 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/stash_client/__init__.py
+-rw-r--r--   0        0        0     2115 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/stash_client/client.py
+-rw-r--r--   0        0        0     2757 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/stash_client/models.py
+-rw-r--r--   0        0        0      569 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/http/stash_client/settings.py
+-rw-r--r--   0        0        0      109 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/ldap/__init__.py
+-rw-r--r--   0        0        0     1896 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/ldap/authenticator.py
+-rw-r--r--   0        0        0      420 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/ldap/settings.py
+-rw-r--r--   0        0        0      430 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/redis/__init__.py
+-rw-r--r--   0        0        0     2937 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/redis/consumer.py
+-rw-r--r--   0        0        0     1661 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/redis/deps.py
+-rw-r--r--   0        0        0     2439 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/redis/objects.py
+-rw-r--r--   0        0        0     1319 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/redis/producer.py
+-rw-r--r--   0        0        0     1384 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/redis/runner.py
+-rw-r--r--   0        0        0     1674 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/redis/settings.py
+-rw-r--r--   0        0        0      132 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/s3/__init__.py
+-rw-r--r--   0        0        0     8494 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/s3/manager.py
+-rw-r--r--   0        0        0     2082 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/s3/models.py
+-rw-r--r--   0        0        0      181 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/s3/objects.py
+-rw-r--r--   0        0        0      885 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/transport/s3/settings.py
+-rw-r--r--   0        0        0      103 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/utils/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/utils/mocks.py
+-rw-r--r--   0        0        0      139 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/utils/time.py
+-rw-r--r--   0        0        0      148 2023-06-26 10:51:26.762732 overhave-4.0.0/overhave/utils/url.py
+-rw-r--r--   0        0        0     3522 2023-06-26 10:51:26.766732 overhave-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0    25392 1970-01-01 00:00:00.000000 overhave-4.0.0/PKG-INFO
```

### Comparing `overhave-3.9.0/README.rst` & `overhave-4.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -223,28 +223,19 @@
     Flask Admin and Login Manager plug-ins;
 * ```overhave_factory``` is a function for LRU cached instance of the **Overhave**
     factory ```ProxyFactory```; the instance has an access to application components,
     directly used in ```overhave_app```.
 * ```my_custom_context``` is an example of context configuration, see an
     example code in `context_example.rst`_.
 
-Enabling of injection
-^^^^^^^^^^^^^^^^^^^^^
-
-**Overhave** has it's own built-in `PyTest`_ plugin, which is used to enable
-and configure injection of prepared context into application core instance.
-The plugin provides one option:
-
-* `--enable-injection` - flag to enable context injection.
-
-The `PyTest` usage should be similar to:
-
-.. code-block:: bash
+Redis
+---------
+* **RedisSentinel** - redis connection through sentinel. To enable sentinel connection use env OVERHAVE_REDIS_SENTINEL_ENABLED=True
 
-    pytest --enable-injection
+* **Redis** - default redis connection without sentinel.
 
 Consumers
 ---------
 
 **Overhave** has `producer-consumer` architecture, based on Redis streams,
 and supported 3 consumer's types:
```

### Comparing `overhave-3.9.0/overhave/__init__.py` & `overhave-4.0.0/overhave/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from overhave.entities import (
     OverhaveAdminSettings,
     OverhaveDescriptionManagerSettings,
     OverhaveEmulationSettings,
     OverhaveFileSettings,
     OverhaveLanguageSettings,
     OverhaveLdapManagerSettings,
-    OverhaveRedisSettings,
     OverhaveStepContextSettings,
     StepPrefixesModel,
 )
 from overhave.factory import ConsumerFactory as OverhaveConsumerFactory
 from overhave.factory import IAdminFactory as OverhaveAdminFactory
 from overhave.factory import IEmulationFactory as OverhaveEmulationFactory
 from overhave.factory import IPublicationFactory as OverhavePublicationFactory
@@ -40,18 +39,25 @@
 from overhave.publication import PublicationSettings as OverhavePublicationSettings
 from overhave.pytest_plugin import IProxyManager as OverhaveProxyManager
 from overhave.pytest_plugin import get_description_manager, get_feature_info_from_item
 from overhave.pytest_plugin import get_proxy_manager as overhave_proxy_manager
 from overhave.scenario import FeatureInfo as OverhaveFeatureInfo
 from overhave.scenario import OverhaveProjectSettings, OverhaveScenarioCompilerSettings, OverhaveScenarioParserSettings
 from overhave.storage import FeatureTypeName as OverhaveFeatureName
-from overhave.storage import TestUserSpecification, TestUserStorage
-from overhave.test_execution import OverhaveAdminLinkSettings, OverhaveTestSettings
+from overhave.storage import ITestUserStorage, TestUserSpecification, TestUserStorage
+from overhave.test_execution import (
+    OverhaveAdminLinkSettings,
+    OverhaveStepCollectorSettings,
+    OverhaveTestSettings,
+    public_step,
+)
 from overhave.transport import (
     OverhaveApiAuthenticator,
     OverhaveApiAuthenticatorSettings,
     OverhaveGitlabClientSettings,
     OverhaveLdapClientSettings,
+    OverhaveRedisSentinelSettings,
+    OverhaveRedisSettings,
     OverhaveS3ManagerSettings,
     OverhaveStashClientSettings,
 )
 from overhave.transport import RedisStream as OverhaveRedisStream
```

### Comparing `overhave-3.9.0/overhave/admin/app.py` & `overhave-4.0.0/overhave/admin/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import flask
 import werkzeug
 
 from overhave import db
 from overhave.admin.flask import FlaskLoginManager, get_flask_admin, get_flask_app
 from overhave.factory import IAdminFactory, get_publication_factory
 from overhave.pytest_plugin import get_proxy_manager
-from overhave.storage import UniqueDraftCreationError
 from overhave.transport import PublicationData, PublicationTask
 
 logger = logging.getLogger(__name__)
 
 OverhaveAdminApp = typing.NewType("OverhaveAdminApp", flask.Flask)
 
 
@@ -44,15 +43,15 @@
     files_dir = current_dir / "files"
 
     _prepare_factory(factory)
     flask_app = _resolved_app(factory=factory, template_dir=template_dir)
     flask_app.config["FILES_DIR"] = files_dir
 
     @flask_app.teardown_request
-    def remove_session(exception: typing.Optional[BaseException]) -> None:
+    def remove_session(exception: BaseException | None) -> None:
         db.current_session.remove()
 
     @flask_app.route("/reports/<path:request>", methods=["GET", "POST"])
     def get_report(request: str) -> flask.Response:
         if flask.request.method == "POST":
             test_run_id = flask.request.form.get("run_id")
             if test_run_id is None:
@@ -66,32 +65,36 @@
                         flask.Response, flask.redirect(f"/reports/{request}", code=HTTPStatus.TEMPORARY_REDIRECT)
                     )
                 return flask.abort(HTTPStatus.NOT_FOUND)
         return flask.send_from_directory(factory.context.file_settings.tmp_reports_dir, request)
 
     @flask_app.route("/emulations/<path:url>")
     def go_to_emulation(url: str) -> werkzeug.Response:
-        return flask.redirect(factory.context.emulation_settings.get_emulation_url(url))
+        return flask.redirect(str(factory.context.emulation_settings.get_emulation_url(url)))
 
     @flask_app.route("/pull_request/<int:run_id>")
     def publish_feature(run_id: int) -> werkzeug.Response:
         published_by = flask.request.args.get("published_by")
         if not isinstance(published_by, str):
             flask.flash("Parameter 'published_by' should be specified for version's creation!", category="error")
             return flask.redirect(flask.url_for("testrun.details_view", id=run_id))
-        try:
-            draft_id = factory.draft_storage.save_draft(
-                test_run_id=run_id, published_by=published_by, status=db.DraftStatus.REQUESTED
-            )
-        except UniqueDraftCreationError:
-            logger.exception("Error while creation draft!")
-            flask.flash(
-                "Requested publication contains scenario which identical to the previous version!", category="warning"
-            )
+
+        draft_id: int | None = None
+        with db.create_session() as session:
+            test_run = session.get(db.TestRun, run_id)
+            if test_run is not None:
+                draft_id = factory.draft_storage.get_or_create_draft(
+                    session=session, test_run=test_run, published_by=published_by, status=db.DraftStatus.REQUESTED
+                )
+        if draft_id is None:
+            msg = "Not found TestRun.id="
+            logger.exception("%s%s!", msg, run_id)
+            flask.flash(f"{msg}{run_id}", category="error")
             return flask.redirect(flask.url_for("testrun.details_view", id=run_id))
+
         if not factory.context.admin_settings.consumer_based:
             factory.threadpool.apply_async(get_publication_factory().publisher.publish_version, args=(draft_id,))
         if factory.context.admin_settings.consumer_based and not factory.redis_producer.add_task(
             PublicationTask(data=PublicationData(draft_id=draft_id))
         ):
             flask.flash("Problems with Redis service! TestRunTask has not been sent.", category="error")
             return flask.redirect(flask.url_for("testrun.details_view", id=run_id))
```

### Comparing `overhave-3.9.0/overhave/admin/files/ace-src/ace.js` & `overhave-4.0.0/overhave/admin/files/ace-src/ace.js`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/files/ace-src/mode-gherkin.js` & `overhave-4.0.0/overhave/admin/files/ace-src/mode-gherkin.js`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/files/css/overhave.css` & `overhave-4.0.0/overhave/admin/files/css/overhave.css`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/files/favicon.ico` & `overhave-4.0.0/overhave/admin/files/favicon.ico`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/flask/flask_admin.py` & `overhave-4.0.0/overhave/admin/flask/flask_admin.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/templates/emulation_run_detail.html` & `overhave-4.0.0/overhave/admin/templates/emulation_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/templates/feature.html` & `overhave-4.0.0/overhave/admin/templates/feature.html`

 * *Files 4% similar despite different names*

```diff
@@ -52,32 +52,25 @@
 {% set bdd_fixtures = admin_view.get_bdd_steps %}
 
 {% macro render_editor() %}
     <script type='text/javascript' src="/files/ace-src/ace.js"></script>
     <link rel="stylesheet" href="https://ace.c9.io/api/resources/csses/ace_api.css">
     <script>
         function contains(target, pattern){
-            var value = 0;
-            pattern.forEach(function(word) {
-              value = value + target.includes(word);
-            });
-            return (value === 1)
+            var value = pattern.reduce((acc, curr) => acc + target.includes(curr), 0)
+            return value === 1
         }
         function with_double_indent(text) {
             return "\n\n".concat(text)
         }
         function with_new_line(text) {
             return "\n  ".concat(text)
         }
         function join_text(arr){
-            var value = "";
-            arr.forEach(function (text) {
-                value = value.concat(text);
-            });
-            return value
+            return arr.reduce((acc, curr) => acc + curr, "")
         }
         var scenario_prefixes = ['Scenario:', 'Сценарий:'];
         var scenario_outline_prefixes = ['Scenario Outline:', 'Структура сценария:'];
         var backround_prefixes = ['Background:', 'Предыстория:'];
         var given_type = "given";
         var when_type = "when";
         var then_type = "then";
@@ -123,26 +116,20 @@
                 var add_scenario_button = document.getElementById('scenario-button');
                 add_scenario_button.style.display = "none";
             });
         }
         function renderSteps() {
             actual_feature_type = $('#s2id_feature_type > a > span').text().toLowerCase();
             if (actual_feature_type.length !== 0){
-                // TODO
-                steps_container_elements = document.querySelectorAll('[id^="steps_container_"]');
-                for (let steps_container of steps_container_elements){
-                    element = $("#".concat(steps_container.id));
-                    search_result = steps_container.id.search(actual_feature_type);
-                    if (search_result === -1) {
-                        element.hide();
-                    }
-                    else {
-                        element.show();
-                    }
-                }
+                $('.steps_container').each(function (index) {
+                    if (this.id.search(actual_feature_type) === -1)
+                        $(this).hide();
+                    else 
+                        $(this).show();
+                });
             }
         }
         function observeStepsRendering() {
               var observer = new MutationObserver(function(mutations){
                   renderSteps();
                   for (var mutation of mutations){
                     for (var node of mutation.addedNodes){
@@ -200,15 +187,17 @@
     <div class="row">
         <div class="col-md-12">
             <h2 align="center">Script panel</h2>
         </div>
         <hr>
         <div class="col-md-8">
             {% macro extra() %}
-                <input type="submit" class="btn btn-info" value="Run test" name="run" formtarget="_blank">
+                {% if 'edit' in url_for(request.endpoint) %}
+                    <input type="submit" class="btn btn-info" value="Run test" name="run" formtarget="_blank">
+                {% endif %}
             {% endmacro %}
             {{ lib.render_form(form, return_url, extra(), form_opts) }}
 
             {% if model and model.versions %}
                 <hr><br>
             <h3 align="center">Published versions</h3>
             <table class="table" border="1" bordercolor="gray">
@@ -223,34 +212,33 @@
                     {{ drafts }}
                 </tbody>
             </table>
             {% endif %}
         </div>
         <div class="col-md-4" id="steps_container">
             {% for feature_type in bdd_fixtures %}
-                <div id="steps_container_{{ feature_type }}" style="display: none;">
+                <div id="steps_container_{{ feature_type }}" class="steps_container" style="display: none;">
                     {{ render_steps_container(feature_type) }}
                 </div>
             {% endfor %}
         </div>
     </div>
 {% endmacro %}
 
 {% macro render_steps_container(feature_type) %}
     {{ render_fixtures_table("Given steps", "given", feature_type) }}
     {{ render_fixtures_table("When steps", "when", feature_type) }}
     {{ render_fixtures_table("Then steps", "then", feature_type) }}
 {% endmacro %}
 
 {% macro render_fixtures_table(title, step_type, feature_type) %}
-    <!-- TODO -->
     <table style="width:100%;">
         <tbody>
         <tr onclick="$('#{{ feature_type }}_{{ step_type }}_steps').slideToggle('slow');">
-            <th style="width:10%;">
+            <th>
                 <a class="toggle-block">►</a>
             </th>
             <th class="text-center" title="Push for toggle">
                 <a class="toggle-block"><h4>{{ title }}</h4></a>
             </th>
         </tr>
         </tbody>
```

### Comparing `overhave-3.9.0/overhave/admin/templates/login.html` & `overhave-4.0.0/overhave/admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/templates/test_run.html` & `overhave-4.0.0/overhave/admin/templates/test_run.html`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/templates/test_run_detail.html` & `overhave-4.0.0/overhave/admin/templates/test_run_detail.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 {% extends 'admin/model/details.html' %}
 {% import 'test_run.html' as test_run_lib with context %}
 
+{% block title %}
+    Test run / {{ model.name }}
+{% endblock %}
+
 {% block tail %}
     {{ super() }}
     {{ test_run_lib.add_button_style() }}
     {% if model.status not in ['STARTED', 'RUNNING'] %}
         {{ render_edit_button(model) }}
     {% endif %}
     {% if model.report  %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends 'admin/model/details.html' %} {% import 'test_run.html' as
-test_run_lib with context %} {% block tail %} {{ super() }} {
-{ test_run_lib.add_button_style() }} {% if model.status not in ['STARTED',
-'RUNNING'] %} {{ render_edit_button(model) }} {% endif %} {% if model.report %}
-{% if model.status != 'INTERNAL_ERROR' and model.report != 'not_created' %} {
-{ render_allure_button(model) }} {% endif %} {% else %}
+test_run_lib with context %} {% block title %} Test run / {{ model.name }} {%
+endblock %} {% block tail %} {{ super() }} {{ test_run_lib.add_button_style()
+}} {% if model.status not in ['STARTED', 'RUNNING'] %} {{ render_edit_button
+(model) }} {% endif %} {% if model.report %} {% if model.status !=
+'INTERNAL_ERROR' and model.report != 'not_created' %} {{ render_allure_button
+(model) }} {% endif %} {% else %}
  {% endif %} {% if model.status == 'SUCCESS' %} {{ render_pr_button(model) }}
 {% endif %} {% endblock %} {% macro render_edit_button(model) %} Edit_feature
 {% endmacro %} {% macro render_allure_button(model) %}
  Allure report
 {% endmacro %} {% macro render_pr_button(model) %}
  Create pull-request
 {% endmacro %}
```

### Comparing `overhave-3.9.0/overhave/admin/templates/test_user.html` & `overhave-4.0.0/overhave/admin/templates/test_user.html`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/views/access.py` & `overhave-4.0.0/overhave/admin/views/access.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,18 +26,18 @@
             return redirect(url_for("admin.index"))
         return redirect(url_for("admin.login", next=request.url))
 
 
 class UserView(AccessModelView):
     """View for application user access management."""
 
-    column_list = ["login", "role", "created_at"]
-    column_searchable_list = ["login"]
-    form_excluded_columns = ["created_at"]
+    column_list = ("login", "role", "created_at")
+    column_searchable_list = ("login",)
+    form_excluded_columns = ("created_at",)
 
 
 class GroupView(AccessModelView):
     """View for application group access management."""
 
-    column_list = ["group", "created_at"]
-    column_searchable_list = ["group"]
-    form_excluded_columns = ["created_at"]
+    column_list = ("group", "created_at")
+    column_searchable_list = ("group",)
+    form_excluded_columns = ("created_at",)
```

### Comparing `overhave-3.9.0/overhave/admin/views/base.py` & `overhave-4.0.0/overhave/admin/views/base.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/views/draft.py` & `overhave-4.0.0/overhave/admin/views/draft.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/views/emulation.py` & `overhave-4.0.0/overhave/admin/views/emulation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import logging
-from typing import Optional
 
 import flask
 import werkzeug
 from flask_admin import expose
 from flask_admin.model.helpers import get_mdict_item_or_list
 from flask_login import current_user
 from wtforms import Form, ValidationError
@@ -34,42 +33,42 @@
         "name": "Emulation template name",
         "test_user.feature_type": "Type of template supported by specified test user",
         "test_user": "Related Test User used for specified emulation",
         "command": "Flags and values for emulation execution",
     }
 
     @property
-    def additional_cmd_description(self) -> Optional[str]:
+    def additional_cmd_description(self) -> str | None:
         return get_admin_factory().context.emulation_settings.emulation_desc_link
 
     def on_model_change(self, form: Form, model: db.Emulation, is_created: bool) -> None:
         if is_created:
             model.created_by = current_user.login
 
     def on_model_delete(self, model: db.Emulation) -> None:
         if not (current_user.login == model.created_by or current_user.role == db.Role.admin):
             raise ValidationError("Only emulation item creator or administrator could delete it!")
 
     @staticmethod
     def _run_emulation(emulation_id: int) -> werkzeug.Response:
         factory = get_admin_factory()
-        emulation_run = factory.emulation_storage.create_emulation_run(
+        emulation_run_id = factory.emulation_storage.create_emulation_run(
             emulation_id=emulation_id, initiated_by=current_user.login
         )
-        if not factory.redis_producer.add_task(EmulationTask(data=EmulationData(emulation_run_id=emulation_run.id))):
+        if not factory.redis_producer.add_task(EmulationTask(data=EmulationData(emulation_run_id=emulation_run_id))):
             flask.flash("Problems with Redis service! EmulationTask has not been sent.", category="error")
             return flask.redirect(flask.url_for("emulation.edit_view", id=emulation_id))
-        return flask.redirect(flask.url_for("emulationrun.details_view", id=emulation_run.id))
+        return flask.redirect(flask.url_for("emulationrun.details_view", id=emulation_run_id))
 
     @property
-    def description_link(self) -> Optional[str]:
+    def description_link(self) -> str | None:
         return get_admin_factory().context.emulation_settings.emulation_desc_link
 
     @expose("/edit/", methods=("GET", "POST"))
-    def edit_view(self) -> Optional[werkzeug.Response]:
+    def edit_view(self) -> werkzeug.Response | None:
         data = flask.request.form
         logger.debug("Request data:\n%s", json.dumps(data))
 
         rendered: werkzeug.Response = super().edit_view()
 
         emulation_action = data.get("emulate")
         if not emulation_action:
```

### Comparing `overhave-3.9.0/overhave/admin/views/emulation_run.py` & `overhave-4.0.0/overhave/admin/views/emulation_run.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/views/feature.py` & `overhave-4.0.0/overhave/admin/views/feature.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 import logging
 import re
 from functools import cached_property
 from pathlib import Path
-from typing import Any, Dict, List, Optional
+from typing import Any, Callable, cast
 
 import flask
 import werkzeug
 from flask_admin import expose
 from flask_admin.model import InlineFormAdmin
 from flask_login import current_user
 from markupsafe import Markup
 from pytest_bdd.types import STEP_TYPES
-from wtforms import Field, TextAreaField, ValidationError
+from wtforms import Field, Form, TextAreaField, ValidationError
 from wtforms.widgets import HiddenInput
 
 from overhave import db
 from overhave.admin.views.base import ModelViewConfigured
 from overhave.factory import IAdminFactory, get_admin_factory, get_test_execution_factory
 from overhave.pytest_plugin import get_proxy_manager
 from overhave.storage import FeatureTypeName
@@ -52,19 +52,19 @@
     form_overrides = dict(text=ScenarioTextAreaField)
     form_excluded_columns = ("created_at", "test_runs")
 
 
 class FactoryViewUtilsMixin:
     """Mixin for :class:`FeatureView`. Extra methods for working with cached instance of :class:`IAdminFactory`."""
 
-    _task_pattern = re.compile(r"\w+[-]\d+")
+    _task_pattern = re.compile(r"\w+-\d+")
     _file_path_pattern = re.compile(r"^[0-9a-zA-Zа-яА-ЯёЁ_/\\ ]{8,}")
 
     @classmethod
-    def _validate_tasks(cls, tasks: List[str]) -> None:
+    def _validate_tasks(cls, tasks: list[str]) -> None:
         for task in tasks:
             if cls._task_pattern.match(task):
                 continue
             raise ValidationError(
                 f"Incorrect format of task specification: '{task}'! "
                 "Supported: <PROJECT>-<NUMBER>, for example 'PRJ-1234'."
             )
@@ -80,34 +80,34 @@
             )
         prepared_file_path = file_path.replace(" ", "").lstrip("/")
         path = Path(prepared_file_path).with_suffix(self.feature_suffix).as_posix()
         logger.debug("Processed feature file path: '%s'", path)
         return path
 
     @property
-    def task_tracker_url(self) -> Optional[str]:
+    def task_tracker_url(self) -> str | None:
         task_tracker_url_value = get_admin_factory().context.project_settings.task_tracker_url
         if task_tracker_url_value is not None:
-            return task_tracker_url_value.human_repr()
+            return str(task_tracker_url_value)
         return None
 
     @cached_property
     def feature_suffix(self) -> str:
         return get_admin_factory().context.file_settings.feature_suffix
 
     @staticmethod
-    def _get_feature_type_steps(factory: IAdminFactory, feature_type: FeatureTypeName) -> List[BddStepModel]:
+    def _get_feature_type_steps(factory: IAdminFactory, feature_type: FeatureTypeName) -> list[BddStepModel]:
         return factory.step_collector.get_steps(feature_type) or []
 
     @cached_property
-    def get_bdd_steps(self) -> Dict[FeatureTypeName, Dict[StepTypeName, List[BddStepModel]]]:
+    def get_bdd_steps(self) -> dict[FeatureTypeName, dict[StepTypeName, list[BddStepModel]]]:
         factory = get_admin_factory()
         return {
             feature_type: {
-                step_type: [
+                StepTypeName(step_type): [
                     step
                     for step in self._get_feature_type_steps(factory=factory, feature_type=feature_type)
                     if step.type == step_type
                 ]
                 for step_type in STEP_TYPES
             }
             for feature_type in factory.feature_extractor.feature_types
@@ -141,23 +141,23 @@
         "last_edited_by",
         "last_edited_at",
         "released",
         "versions",
         "feature_tags.value",
     )
 
-    column_searchable_list = [
+    column_searchable_list = (
         "id",
         "name",
         "task",
         "author",
         "file_path",
         "last_edited_by",
         "feature_tags.value",
-    ]
+    )
     column_filters = (
         "id",
         "name",
         "feature_type",
         "last_edited_by",
         "author",
         "created_at",
@@ -207,26 +207,24 @@
         model.released = False
 
     def on_model_delete(self, model) -> None:  # type: ignore
         if not (current_user.login == model.author or current_user.role == db.Role.admin):
             raise ValidationError("Only feature author or administrator could delete feature!")
 
     @staticmethod
-    def _run_test(data: Dict[str, Any], rendered: werkzeug.Response) -> werkzeug.Response:
+    def _run_test(data: dict[str, Any], rendered: werkzeug.Response) -> werkzeug.Response:
         scenario_id = data.get(f"{_SCENARIO_PREFIX}-id")
         scenario_text = data.get(f"{_SCENARIO_PREFIX}-text")
         if not scenario_id or not scenario_text:
             flask.flash("Scenario information not requested.", category="error")
             return rendered
         factory = get_admin_factory()
-        scenario = factory.scenario_storage.get_scenario(int(scenario_id))
-        if scenario is None:
-            flask.flash("Scenario does not exist, so could not run test.", category="error")
-            return rendered
-        test_run_id = factory.test_run_storage.create_test_run(scenario_id=scenario.id, executed_by=current_user.login)
+        with db.create_session() as session:
+            scenario = factory.scenario_storage.scenario_model_by_id(session=session, scenario_id=int(scenario_id))
+        test_run_id = factory.test_run_storage.create_testrun(scenario_id=scenario.id, executed_by=current_user.login)
         if not factory.context.admin_settings.consumer_based:
             proxy_manager = get_proxy_manager()
             test_execution_factory = get_test_execution_factory()
             proxy_manager.clear_factory()
             proxy_manager.set_factory(test_execution_factory)
             factory.threadpool.apply_async(get_test_execution_factory().test_executor.execute_test, args=(test_run_id,))
         if factory.context.admin_settings.consumer_based and not factory.redis_producer.add_task(
@@ -254,7 +252,22 @@
         tasks = data["task"].split(",")
         self._validate_tasks(tasks=tasks)
 
         mutable_data = dict(data)
         mutable_data["file_path"] = self._make_file_path(data["file_path"])
 
         return self._run_test(data, rendered)
+
+    @staticmethod
+    def _form_remove_validators(form_change: Callable[..., Form]) -> Callable[..., Form]:
+        admin_settings = get_admin_factory().context.admin_settings
+        if not admin_settings.strict_feature_tasks:
+            form_change.task.kwargs["validators"] = []  # type: ignore[attr-defined]
+        return form_change
+
+    def get_create_form(self) -> Callable[..., Form]:
+        form_create = cast(Callable[..., Form], super().get_create_form())
+        return self._form_remove_validators(form_change=form_create)
+
+    def get_edit_form(self) -> Callable[..., Form]:
+        form_edit = cast(Callable[..., Form], super().get_edit_form())
+        return self._form_remove_validators(form_change=form_edit)
```

### Comparing `overhave-3.9.0/overhave/admin/views/formatters/formatters.py` & `overhave-4.0.0/overhave/admin/views/formatters/formatters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import re
 from datetime import datetime
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 import allure
+import httpx
 from flask_admin.contrib.sqla import ModelView
 from markupsafe import Markup
-from yarl import URL
 
 from overhave import db
 from overhave.admin.views.formatters.helpers import (
     get_button_class_by_status,
     get_feature_link_markup,
     get_report_index_link,
     get_testrun_details_link,
 )
 from overhave.admin.views.formatters.safe_formatter import safe_formatter
-from overhave.db import TestReportStatus
 
 
 @safe_formatter(
     type=datetime,
     supported_models=(
         db.UserRole,
         db.GroupRole,
@@ -33,60 +32,57 @@
     ),
 )
 def datetime_formatter(view: ModelView, context: Any, model: db.BaseTable, value: datetime) -> Markup:
     return Markup(value.strftime("%d-%m-%Y %H:%M:%S"))
 
 
 @safe_formatter(type=list, supported_models=(db.Feature,))
-def task_formatter(view: ModelView, context: Any, model: db.Feature, value: List[str]) -> Markup:
+def task_formatter(view: ModelView, context: Any, model: db.Feature, value: list[str]) -> Markup:
     task_tracker_url = getattr(view, "task_tracker_url")
     if not task_tracker_url:
         return Markup(", ".join(value))
-    task_links: List[str] = []
-    for task in value:
-        task_links.append(f"<a href='{task_tracker_url}/{task}' target='blank'>{task}</a>")
+    task_links = (f"<a href='{task_tracker_url}/{task}' target='blank'>{task}</a>" for task in value)
     return Markup(", ".join(task_links))
 
 
 @safe_formatter(type=str, supported_models=(db.Feature,))
 def file_path_formatter(view: ModelView, context: Any, model: db.Feature, value: str) -> Markup:
     if isinstance(model, db.Feature):
         value_without_suffix = re.sub(rf"({view.feature_suffix})", "", value)
         value_to_visualize = value_without_suffix.split("/")[-1]
         return Markup(f"<i>{value_to_visualize}</i>")
     raise NotImplementedError()
 
 
 @safe_formatter(type=str, supported_models=(db.TestRun,))
-def result_report_formatter(view: ModelView, context: Any, model: db.TestRun, value: str) -> Markup:
-    report_status = TestReportStatus[getattr(model, "report_status")]
+def result_report_formatter(view: ModelView, context: Any, model: db.TestRun, value: db.TestRunStatus) -> Markup:
     test_run_id = getattr(model, "id")
     if test_run_id is None:
         raise ValueError("test_run_id could not be None!")
-    report = getattr(model, "report")
-    if report_status.has_report and isinstance(report, str):
+    report = model.report
+    if model.report_status.has_report and isinstance(report, str):
         return Markup(
             f"<form action='{get_report_index_link(report)}' method='POST' target='_blank'>"
             f"<input type='hidden' name='run_id' value='{test_run_id}' />"
             f"<fieldset title='Go to report'>"
-            f"<button class='link-button {get_button_class_by_status(value)}' type='submit'>{value}</button>"
+            f"<button class='link-button {get_button_class_by_status(value)}' type='submit'>{value.upper()}</button>"
             "</fieldset>"
             "</form>"
         )
     return Markup(
         f"<form action='{get_testrun_details_link(test_run_id)}'>"
         f"<fieldset title='Show details'>"
-        f"<button class='link-button {get_button_class_by_status(value)}'>{value}</button>"
+        f"<button class='link-button {get_button_class_by_status(value)}'>{value.upper()}</button>"
         "</fieldset>"
         "</form>"
     )
 
 
 @safe_formatter(type=dict, supported_models=(db.TestUser,))
-def json_formatter(view: ModelView, context: Any, model: db.BaseTable, value: Dict[str, Optional[str]]) -> Markup:
+def json_formatter(view: ModelView, context: Any, model: db.BaseTable, value: dict[str, str | None]) -> Markup:
     info = ""
     for k, v in list(filter(lambda x: x, value.items())):
         info += f"<b>{k}</b>:&nbsp;&nbsp;{v}<br>"
     return Markup("<form>" "<fieldset>" f"<div class='json-data'>{info}</div>" "</fieldset>" "</form>")
 
 
 @safe_formatter(type=str, supported_models=(db.Feature, db.TestRun))
@@ -125,8 +121,8 @@
 @safe_formatter(type=int, supported_models=(db.Draft,))
 def draft_testrun_formatter(view: ModelView, context: Any, model: db.BaseTable, value: int) -> Markup:
     return Markup(f"<a {get_testrun_details_link(value)}>{value}</a>")
 
 
 @safe_formatter(type=str, supported_models=(db.Draft,))
 def draft_prurl_formatter(view: ModelView, context: Any, model: db.BaseTable, value: str) -> Markup:
-    return Markup(f"<a href='{URL(value).human_repr()}'>{value}</a>")
+    return Markup(f"<a href='{httpx.URL(value)}'>{value}</a>")
```

### Comparing `overhave-3.9.0/overhave/admin/views/formatters/helpers.py` & `overhave-4.0.0/overhave/admin/views/formatters/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from typing import Union
-
 from markupsafe import Markup
 
 from overhave.db import TestRunStatus
 
 
 def get_button_class_by_status(status: str) -> str:
     enum_member = TestRunStatus[status]
     if enum_member is TestRunStatus.SUCCESS:
         return "success-btn"
     return "default-btn"
 
 
-def get_testrun_details_link(test_run_id: Union[int, str]) -> str:
+def get_testrun_details_link(test_run_id: int | str) -> str:
     return f"/testrun/details/?id={test_run_id}"
 
 
 def get_report_index_link(report: str) -> str:
     return f"/reports/{report}/index.html"
 
 
-def get_feature_link_markup(feature_id: Union[int, str], feature_name: str) -> Markup:
+def get_feature_link_markup(feature_id: int | str, feature_name: str) -> Markup:
     return Markup(f"<a href='/feature/edit/?id={feature_id}'>{feature_name}</a>")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-from typing import Union from markupsafe import Markup from overhave.db import
-TestRunStatus def get_button_class_by_status(status: str) -> str: enum_member =
-TestRunStatus[status] if enum_member is TestRunStatus.SUCCESS: return "success-
-btn" return "default-btn" def get_testrun_details_link(test_run_id: Union[int,
-str]) -> str: return f"/testrun/details/?id={test_run_id}" def
-get_report_index_link(report: str) -> str: return f"/reports/{report}/
-index.html" def get_feature_link_markup(feature_id: Union[int, str],
-feature_name: str) -> Markup: return Markup(f"{feature_name}")
+from markupsafe import Markup from overhave.db import TestRunStatus def
+get_button_class_by_status(status: str) -> str: enum_member = TestRunStatus
+[status] if enum_member is TestRunStatus.SUCCESS: return "success-btn" return
+"default-btn" def get_testrun_details_link(test_run_id: int | str) -> str:
+return f"/testrun/details/?id={test_run_id}" def get_report_index_link(report:
+str) -> str: return f"/reports/{report}/index.html" def get_feature_link_markup
+(feature_id: int | str, feature_name: str) -> Markup: return Markup(f"
+{feature_name}")
```

### Comparing `overhave-3.9.0/overhave/admin/views/formatters/safe_formatter.py` & `overhave-4.0.0/overhave/admin/views/formatters/safe_formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import logging
 from types import FunctionType
-from typing import Any, Callable, Sequence, Type, Union
+from typing import Any, Callable, Sequence, Type
 
 from flask_admin.contrib.sqla import ModelView
 from markupsafe import Markup
 
 from overhave import db
 
 logger = logging.getLogger(__name__)
 
 
 def _default_formatter_result(
-    model: db.BaseTable, name: str, supported_models: Sequence[Type[db.BaseTable]]
-) -> Union[Markup, Any]:
+    model: db.BaseTable, name: str, supported_models: Sequence[type[db.BaseTable]]
+) -> Markup | Any:
     value = getattr(model, name, None)
     if value is None:
         return Markup("")
     if not isinstance(model, tuple(supported_models)):
         return Markup(value)
     return value
 
 
 def safe_formatter(type: Type[object], supported_models: Sequence[Type[db.BaseTable]]):  # type: ignore  # noqa: A002
-    def decorator(func: FunctionType) -> Callable[[ModelView, Any, db.BaseTable, str], Union[Markup, Any]]:
-        def wrapper(view: ModelView, context: Any, model: db.BaseTable, name: str) -> Union[Markup, Any]:
+    def decorator(func: FunctionType) -> Callable[[ModelView, Any, db.BaseTable, str], Markup | Any]:
+        def wrapper(view: ModelView, context: Any, model: db.BaseTable, name: str) -> Markup | Any:
             logger.debug("Wrapping function '%s'...", func.__name__)
             result = _default_formatter_result(model=model, name=name, supported_models=supported_models)
             logger.debug("Default formatter result: '%s'", result)
             if not isinstance(result, Markup) and isinstance(result, type):
                 result = func(view, context, model, result)
                 logger.debug("'%s' result: '%s'", func.__name__, result)
             return result
```

### Comparing `overhave-3.9.0/overhave/admin/views/index/custom_page.py` & `overhave-4.0.0/overhave/admin/views/index/custom_page.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import typing
 from pathlib import Path
+from typing import Any
 
 from flask_admin.form import BaseForm
 from flask_admin.model.widgets import XEditableWidget
 from markupsafe import Markup
 from wtforms import Field
 
 
 class CustomPageWidget(XEditableWidget):
     """Customising widget.
 
     Widget content is filled with content from specified
     ``self.template_path```.
     """
 
-    def __init__(self, *args: typing.Any, **kwargs: typing.Any) -> None:
-        self.template_path: typing.Optional[Path] = None
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        self.template_path: Path | None = None
         super().__init__(*args, **kwargs)
 
-    def __call__(self, field: Field, **kwargs: typing.Any) -> Markup:
+    def __call__(self, field: Field, **kwargs: Any) -> Markup:
         if self.template_path is not None:
             with self.template_path.open("r") as template:
                 return Markup(template.read())
         return Markup(
             """
             <h1>Overhave index</h1>
             <p>This is Overhave info page. You could replace this page with your own HTML template.</p>
@@ -40,11 +40,11 @@
 
 
 class CustomPageForm(BaseForm):
     """Form for custom page."""
 
     type = CustomPageField()
 
-    def __init__(self, template_path: typing.Optional[Path]):
+    def __init__(self, template_path: Path | None):
         super().__init__()
         self.type.widget.template_path = template_path
         self.type.label = None
```

### Comparing `overhave-3.9.0/overhave/admin/views/index/login_form.py` & `overhave-4.0.0/overhave/admin/views/index/login_form.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import flask
 from flask_wtf import FlaskForm as Form
 from pydantic import SecretStr
 from werkzeug import Response
 from wtforms import PasswordField, StringField, validators
 
+from overhave.admin.flask.login_manager import AdminPanelUser
 from overhave.entities import IAdminAuthorizationManager
-from overhave.storage import SystemUserModel
 
 logger = logging.getLogger(__name__)
 
 _INVALID_AUTH_MSG = "Specified username '{username}' and password pair is invalid!"
 
 
 class LoginForm(Form):
@@ -27,19 +27,19 @@
         render_kw={"placeholder": "Password", "icon": "glyphicon-certificate"},
     )
 
     def __init__(self, auth_manager: IAdminAuthorizationManager) -> None:
         super().__init__()
         self._auth_manager = auth_manager
 
-    def get_user(self) -> SystemUserModel:
+    def get_user(self) -> AdminPanelUser:
         authorized_user = self._auth_manager.authorize_user(
             username=self.username.data, password=SecretStr(self.password.data)
         )
         if authorized_user is None:
             raise validators.ValidationError(_INVALID_AUTH_MSG.format(username=self.username.data))
-        return authorized_user
+        return AdminPanelUser(user_data=authorized_user)
 
     @staticmethod
     def flash_and_redirect(flash_msg: str) -> Response:
         flask.flash(flash_msg, category="error")
         return flask.redirect(flask.url_for("admin.login"))
```

### Comparing `overhave-3.9.0/overhave/admin/views/index/view.py` & `overhave-4.0.0/overhave/admin/views/index/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any
 
 import flask
 import ldap
 from flask_admin import AdminIndexView, expose
 from flask_login import login_required, login_user, logout_user
 from sqlalchemy.exc import OperationalError, ProgrammingError
 from werkzeug.wrappers import Response
@@ -17,15 +17,15 @@
 logger = logging.getLogger(__name__)
 
 
 class OverhaveIndexView(AdminIndexView):
     """View for index."""
 
     def __init__(
-        self, name: str, url: str, auth_manager: IAdminAuthorizationManager, index_template_path: Optional[Path]
+        self, name: str, url: str, auth_manager: IAdminAuthorizationManager, index_template_path: Path | None
     ) -> None:
         super().__init__(
             name=name,
             url=url,
         )
         self._auth_manager = auth_manager
         self._index_template_path = index_template_path
```

### Comparing `overhave-3.9.0/overhave/admin/views/scenario_test_run.py` & `overhave-4.0.0/overhave/admin/views/scenario_test_run.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/views/tag.py` & `overhave-4.0.0/overhave/admin/views/tag.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/admin/views/testing_users.py` & `overhave-4.0.0/overhave/admin/views/testing_users.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,85 +1,86 @@
-from typing import Dict, Optional, Type, Union
+from typing import cast
 
 from flask_admin.form import JSONField
 from flask_login import current_user
 from pydantic import BaseModel
 from wtforms import Form, ValidationError
 
 from overhave import db
 from overhave.admin.views.base import ModelViewConfigured
 from overhave.factory import get_admin_factory
+from overhave.storage import FeatureTypeName
 from overhave.utils import get_current_time
 
 
-def _make_dict_from_model(model: Optional[Type[BaseModel]]) -> Optional[Dict[str, Union[int, str]]]:
-    if model is not None:
-        prepared_dict = {}
-        for key, value in model.__fields__.items():
-            prepared_dict[key] = value.type_.__name__
-        return prepared_dict
-    return None
+def _make_dict_from_model(model: type[BaseModel]) -> dict[str, int | str]:
+    return {key: value.type_.__name__ for key, value in model.__fields__.items()}
 
 
 class TestUserView(ModelViewConfigured):
     """View for :class:`TestUser` table."""
 
     __test__ = False
 
     create_template = "test_user_create.html"
     edit_template = "test_user_edit.html"
 
     can_view_details = False
     column_list = ("id", "name", "feature_type", "specification", "allow_update", "created_by", "changed_at")
     column_searchable_list = ("id", "name", "created_by")
-    column_filters = ("id", "name", "created_by", "allow_update")
+    column_filters = ("id", "name", "key", "created_by", "allow_update")
     form_excluded_columns = ("created_at", "emulations", "changed_at")
     form_overrides = dict(specification=JSONField)
 
     form_extra_fields = {"template": JSONField("Specification format")}
     form_widget_args = {"template": {"readonly": True}}
 
     column_labels = {
-        "name": "Test user name",
+        "key": "Key",
+        "name": "Name",
         "feature_type": "Feature type",
     }
     column_descriptions = {
+        "key": "Test user key",
         "name": "Custom name for test user",
         "feature_type": "Type of scenarios set, where test user will be used",
         "specification": "Test user specification in JSON format placed below",
         "created_by": "Author of test user set",
         "allow_update": "Property of updating allowance through API",
     }
 
-    _feature_type: Optional[str] = None
+    _feature_type: FeatureTypeName | None = None
 
     def on_form_prefill(self, form, id) -> None:  # type: ignore  # noqa: A002
-        if isinstance(form._obj, db.TestUser):
-            self._feature_type = form._obj.feature_type.name
+        if not isinstance(form._obj, db.TestUser):
+            return
+        self._feature_type = cast(FeatureTypeName, form._obj.feature_type.name)
 
-    def get_specification_template(self) -> Optional[Dict[str, Union[int, str]]]:
+    def get_specification_template(self) -> dict[str, int | str] | None:
         factory = get_admin_factory()
         if self._feature_type is None:
-            self._feature_type = factory.feature_type_storage.get_default_feature_type().name
+            self._feature_type: FeatureTypeName = factory.feature_type_storage.default_feature_type_name
         parser = factory.context.project_settings.user_spec_template_mapping.get(self._feature_type)
-        return _make_dict_from_model(parser)
+        if parser is not None:
+            return _make_dict_from_model(parser)
+        return None
 
     @staticmethod
     def _validate_json(model: db.TestUser) -> None:
         if not isinstance(model.specification, dict):
             raise ValidationError("Could not convert specified data into correct JSON!")
         parser = get_admin_factory().context.project_settings.user_spec_template_mapping.get(model.feature_type.name)
         if parser is not None:
             try:
                 parser.parse_obj(model.specification)
             except ValueError:
                 raise ValidationError(f"Could not convert specified data into {parser.__name__} model!")
 
     def on_model_change(self, form: Form, model: db.TestUser, is_created: bool) -> None:
-        self._feature_type = model.feature_type.name
+        self._feature_type = cast(FeatureTypeName, model.feature_type.name)
         self._validate_json(model)
         if is_created:
             model.created_by = current_user.login
         model.changed_at = get_current_time()
 
     def on_model_delete(self, model: db.TestUser) -> None:
         if not (current_user.login == model.created_by or current_user.role == db.Role.admin):
```

### Comparing `overhave-3.9.0/overhave/api/app.py` & `overhave-4.0.0/overhave/api/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 import fastapi
 
 from overhave.api.auth import get_authorized_user
 from overhave.api.views import (
     delete_test_user_handler,
     docs,
     emulation_run_list_handler,
@@ -41,42 +39,42 @@
         response_model=TagModel,
         summary="Get FeatureTag",
         description="Get feature tag by `value`",
     )
     tags_router.add_api_route(
         "/list",
         tags_list_handler,
-        response_model=List[TagModel],
+        response_model=list[TagModel],
         methods=["GET"],
         summary="Get FeatureTags",
         description="Get list of feature tags like `value`",
     )
     return tags_router
 
 
 def _get_feature_type_router() -> fastapi.APIRouter:
     feature_router = fastapi.APIRouter()
     feature_router.add_api_route(
         "/list",
         feature_types_list_handler,
         methods=["GET"],
-        response_model=List[FeatureTypeModel],
+        response_model=list[FeatureTypeModel],
         summary="Get list of FeatureType info",
         description="Get list of feature types",
     )
     return feature_router
 
 
 def _get_feature_router() -> fastapi.APIRouter:
     feature_router = fastapi.APIRouter()
     feature_router.add_api_route(
         "/",
         get_features_handler,
         methods=["GET"],
-        response_model=List[FeatureModel],
+        response_model=list[FeatureModel],
         summary="Get list of Feature info",
         description="Get list of feature info by `tag_id` or `tag_value`",
     )
     return feature_router
 
 
 def _get_testrun_router() -> fastapi.APIRouter:
@@ -105,21 +103,21 @@
 
     test_user_router.add_api_route(
         "/",
         get_test_user_handler,
         methods=["GET"],
         response_model=TestUserModel,
         summary="Get TestUser",
-        description="Get test user full info by `user_id` or `user_name`",
+        description="Get test user full info by `user_id` or `user_key`",
     )
     test_user_router.add_api_route(
         "/list",
         test_user_list_handler,
         methods=["GET"],
-        response_model=List[TestUserModel],
+        response_model=list[TestUserModel],
         summary="Get list of TestUsers",
         description="Get list of test users with given `feature_type` and `allow_update`",
     )
     test_user_router.add_api_route(
         "/{user_id}/delete",
         delete_test_user_handler,
         methods=["DELETE"],
@@ -146,15 +144,15 @@
 
 def _get_emulation_router() -> fastapi.APIRouter:
     emulation_router = fastapi.APIRouter()
     emulation_router.add_api_route(
         "/run/list",
         emulation_run_list_handler,
         methods=["GET"],
-        response_model=List[EmulationRunModel],
+        response_model=list[EmulationRunModel],
         summary="Get list of EmulationRun info",
         description="Get list of EmulationRun info by `test_user_id`",
     )
     return emulation_router
 
 
 def _get_auth_router() -> fastapi.APIRouter:
@@ -169,15 +167,15 @@
         include_in_schema=False,
     )
     return auth_router
 
 
 def create_overhave_api() -> fastapi.FastAPI:
     app = fastapi.FastAPI()
-    auth_deps = [fastapi.Depends(get_authorized_user)]
+    auth_deps = (fastapi.Depends(get_authorized_user),)
 
     app.include_router(_get_tags_router(), dependencies=auth_deps, prefix="/feature/tags", tags=["feature_tags"])
     app.include_router(
         _get_feature_type_router(), dependencies=auth_deps, prefix="/feature/types", tags=["feature_types"]
     )
     app.include_router(_get_feature_router(), dependencies=auth_deps, prefix="/feature", tags=["features"])
     app.include_router(_get_testuser_router(), dependencies=auth_deps, prefix="/test_user", tags=["test_users"])
```

### Comparing `overhave-3.9.0/overhave/api/auth/regular.py` & `overhave-4.0.0/overhave/api/auth/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/api/auth/token.py` & `overhave-4.0.0/overhave/api/auth/token.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime
-from typing import Dict, Optional, Union, cast
+from typing import cast
 
 from jose import jwt
 
 from overhave.api.auth.models import AuthTokenData
 from overhave.api.settings import OverhaveApiAuthSettings
 
 
 def create_access_token(auth_settings: OverhaveApiAuthSettings, username: str, expires_at: datetime) -> str:
-    to_encode: Dict[str, Union[str, datetime]] = {"sub": username, "exp": expires_at}
+    to_encode: dict[str, str | datetime] = {"sub": username, "exp": expires_at}
     return cast(
         str, jwt.encode(to_encode, auth_settings.secret_key.get_secret_value(), algorithm=auth_settings.algorithm)
     )
 
 
-def get_token_data(auth_settings: OverhaveApiAuthSettings, token: str) -> Optional[AuthTokenData]:
+def get_token_data(auth_settings: OverhaveApiAuthSettings, token: str) -> AuthTokenData | None:
     payload = jwt.decode(token, auth_settings.secret_key.get_secret_value(), algorithms=[auth_settings.algorithm])
-    username: Optional[str] = payload.get("sub")
+    username: str | None = payload.get("sub")
     if username is not None:
         return AuthTokenData(username=username)
     return None
```

### Comparing `overhave-3.9.0/overhave/api/settings.py` & `overhave-4.0.0/overhave/api/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/api/views/__init__.py` & `overhave-4.0.0/overhave/api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/api/views/auth_views.py` & `overhave-4.0.0/overhave/api/views/auth_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/api/views/emulation_views.py` & `overhave-4.0.0/overhave/api/views/emulation_views.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import logging
-from typing import List
 
 import fastapi
 
 from overhave.api.deps import get_emulation_storage
 from overhave.storage import EmulationRunModel, IEmulationStorage
 
 logger = logging.getLogger(__name__)
 
 
 def emulation_run_list_handler(
     test_user_id: int,
     emulation_storage: IEmulationStorage = fastapi.Depends(get_emulation_storage),
-) -> List[EmulationRunModel]:
+) -> list[EmulationRunModel]:
     logger.info("Getting %s list with test_user_id=%s...", EmulationRunModel.__name__, test_user_id)
     return emulation_storage.get_emulation_runs_by_test_user_id(test_user_id=test_user_id)
```

### Comparing `overhave-3.9.0/overhave/api/views/extra_views.py` & `overhave-4.0.0/overhave/api/views/extra_views.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/api/views/feature_views.py` & `overhave-4.0.0/overhave/api/views/feature_views.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import logging
 from http import HTTPStatus
-from typing import List, Optional
 
 import fastapi
 
 from overhave.api.deps import get_feature_storage, get_feature_tag_storage
 from overhave.api.views.tags_views import tags_item_handler
 from overhave.storage import FeatureModel, IFeatureStorage, IFeatureTagStorage
 
 logger = logging.getLogger(__name__)
 
 
 def get_features_handler(
-    tag_id: Optional[int] = None,
-    tag_value: Optional[str] = None,
+    tag_id: int | None = None,
+    tag_value: str | None = None,
     feature_storage: IFeatureStorage = fastapi.Depends(get_feature_storage),
     tag_storage: IFeatureTagStorage = fastapi.Depends(get_feature_tag_storage),
-) -> List[FeatureModel]:
+) -> list[FeatureModel]:
     if tag_id is not None:
         logger.info("Getting %s by tag_id=%s...", FeatureModel.__name__, tag_id)
         return feature_storage.get_features_by_tag(tag_id=tag_id)
     if tag_value is not None:
         logger.info("Getting %s by tag_value=%s...", FeatureModel.__name__, tag_value)
         tag_model = tags_item_handler(value=tag_value, feature_tag_storage=tag_storage)
         return feature_storage.get_features_by_tag(tag_id=tag_model.id)
```

### Comparing `overhave-3.9.0/overhave/api/views/tags_views.py` & `overhave-4.0.0/overhave/api/views/tags_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from http import HTTPStatus
-from typing import List
 
 import fastapi
 
 from overhave.api.deps import get_feature_tag_storage
 from overhave.storage import IFeatureTagStorage, TagModel
 
 logger = logging.getLogger(__name__)
@@ -22,10 +21,10 @@
         )
     return tag_model
 
 
 def tags_list_handler(
     value: str,
     feature_tag_storage: IFeatureTagStorage = fastapi.Depends(get_feature_tag_storage),
-) -> List[TagModel]:
+) -> list[TagModel]:
     logger.info("Getting %s list like value='%s...'", TagModel.__name__, value)
     return feature_tag_storage.get_tags_like_value(value)
```

### Comparing `overhave-3.9.0/overhave/api/views/testrun_views.py` & `overhave-4.0.0/overhave/api/views/testrun_views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 from http import HTTPStatus
 
 import fastapi
 
-from overhave.api.deps import get_feature_storage, get_feature_tag_storage, get_redis_producer, get_test_run_storage
+from overhave.api.deps import (
+    get_feature_storage,
+    get_feature_tag_storage,
+    get_redis_producer,
+    get_scenario_storage,
+    get_test_run_storage,
+)
 from overhave.api.views.tags_views import tags_item_handler
-from overhave.storage import IFeatureStorage, IFeatureTagStorage, TestRunModel, TestRunStorage
+from overhave.storage import IFeatureStorage, IFeatureTagStorage, IScenarioStorage, TestRunModel, TestRunStorage
 from overhave.transport import RedisProducer, TestRunData, TestRunTask
 
 
 def get_test_run_handler(
     test_run_id: int,
     test_run_storage: TestRunStorage = fastapi.Depends(get_test_run_storage),
 ) -> TestRunModel:
-    test_run = test_run_storage.get_test_run(test_run_id)
+    test_run = test_run_storage.get_testrun_model(test_run_id)
     if test_run is not None:
         return test_run
     raise fastapi.HTTPException(
         status_code=HTTPStatus.BAD_REQUEST, detail=f"Test run with id ='{test_run_id}' not found"
     )
 
 
 def run_tests_by_tag_handler(
     tag_value: str,
     feature_storage: IFeatureStorage = fastapi.Depends(get_feature_storage),
     tag_storage: IFeatureTagStorage = fastapi.Depends(get_feature_tag_storage),
+    scenario_storage: IScenarioStorage = fastapi.Depends(get_scenario_storage),
     test_run_storage: TestRunStorage = fastapi.Depends(get_test_run_storage),
     redis_producer: RedisProducer = fastapi.Depends(get_redis_producer),
 ) -> list[int]:
     tag_model = tags_item_handler(value=tag_value, feature_tag_storage=tag_storage)
     features = feature_storage.get_features_by_tag(tag_id=tag_model.id)
     if not features:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"Features with tag='{tag_value}' do not exist"
         )
     test_run_ids: list[int] = []
     for feature in features:
-        test_run_id = test_run_storage.create_test_run(scenario_id=feature.id, executed_by=feature.last_edited_by)
+        scenario = scenario_storage.get_scenario_by_feature_id(feature.id)
+        test_run_id = test_run_storage.create_testrun(scenario_id=scenario.id, executed_by=feature.last_edited_by)
         redis_producer.add_task(TestRunTask(data=TestRunData(test_run_id=test_run_id)))
         test_run_ids.append(test_run_id)
     return test_run_ids
```

### Comparing `overhave-3.9.0/overhave/api/views/testuser_views.py` & `overhave-4.0.0/overhave/api/views/testuser_views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from http import HTTPStatus
-from typing import List, Optional
 
 import fastapi
 
+from overhave import db
 from overhave.api.deps import get_feature_type_storage, get_test_user_storage
 from overhave.storage import (
     FeatureTypeName,
     FeatureTypeNotExistsError,
     IFeatureTypeStorage,
     ITestUserStorage,
     TestUserDoesNotExistError,
@@ -25,35 +25,35 @@
     if test_user is None:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"User with id={user_id} does not exist!"
         )
     return test_user
 
 
-def _get_test_user_by_name_handler(user_name: str, test_user_storage: ITestUserStorage) -> TestUserModel:
-    logger.info("Getting %s with user_name='%s'...", TestUserModel.__name__, user_name)
-    test_user = test_user_storage.get_test_user_by_name(user_name)
+def _get_test_user_by_key_handler(user_key: str, test_user_storage: ITestUserStorage) -> TestUserModel:
+    logger.info("Getting %s with user_key='%s'...", TestUserModel.__name__, user_key)
+    test_user = test_user_storage.get_test_user_by_key(user_key)
     if test_user is None:
         raise fastapi.HTTPException(
-            status_code=HTTPStatus.BAD_REQUEST, detail=f"User with name='{user_name}' does not exist!"
+            status_code=HTTPStatus.BAD_REQUEST, detail=f"User with key='{user_key}' does not exist!"
         )
     return test_user
 
 
 def get_test_user_handler(
-    user_id: Optional[int] = None,
-    user_name: Optional[str] = None,
+    user_id: int | None = None,
+    user_key: str | None = None,
     test_user_storage: ITestUserStorage = fastapi.Depends(get_test_user_storage),
 ) -> TestUserModel:
     if user_id is not None:
         return _get_test_user_by_id_handler(user_id=user_id, test_user_storage=test_user_storage)
-    if user_name is not None:
-        return _get_test_user_by_name_handler(user_name=user_name, test_user_storage=test_user_storage)
+    if user_key is not None:
+        return _get_test_user_by_key_handler(user_key=user_key, test_user_storage=test_user_storage)
     raise fastapi.HTTPException(
-        status_code=HTTPStatus.BAD_REQUEST, detail="'user_id' or 'user_name' query parameter should be set!"
+        status_code=HTTPStatus.BAD_REQUEST, detail="'user_id' or 'user_key' query parameter should be set!"
     )
 
 
 def delete_test_user_handler(
     user_id: int,
     test_user_storage: ITestUserStorage = fastapi.Depends(get_test_user_storage),
 ) -> None:
@@ -66,24 +66,27 @@
 
 
 def test_user_list_handler(
     feature_type: FeatureTypeName,
     allow_update: bool,
     feature_type_storage: IFeatureTypeStorage = fastapi.Depends(get_feature_type_storage),
     test_user_storage: ITestUserStorage = fastapi.Depends(get_test_user_storage),
-) -> List[TestUserModel]:
+) -> list[TestUserModel]:
     logger.info(
         "Getting %s list with feature_type=%s and allow_update=%s ...",
         TestUserModel.__name__,
         feature_type,
         allow_update,
     )
     try:
-        feature_type_model = feature_type_storage.get_feature_type_by_name(feature_type)
-        return test_user_storage.get_test_users(feature_type_id=feature_type_model.id, allow_update=allow_update)
+        with db.create_session() as session:
+            db_feature_type = feature_type_storage.feature_type_by_name(session=session, name=feature_type)
+            return test_user_storage.get_test_users_by_feature_type_name(
+                session=session, feature_type_id=db_feature_type.id, allow_update=allow_update
+            )
     except FeatureTypeNotExistsError:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"FeatureType with name='{feature_type}' does not exist!"
         )
 
 
 def test_user_get_spec_handler(
```

### Comparing `overhave-3.9.0/overhave/base_settings.py` & `overhave-4.0.0/overhave/base_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,102 @@
 import enum
 import logging
 import socket
 from logging.config import DictConfigurator  # type: ignore
-from typing import Any, Dict, Optional
+from typing import Any
 
+import sqlalchemy as sa
+import sqlalchemy.engine
+import sqlalchemy.exc
+import sqlalchemy.pool
 from pydantic import BaseSettings, Field, validator
-from sqlalchemy import engine_from_config
-from sqlalchemy.engine import Engine
-from sqlalchemy.engine.url import URL, make_url
-from sqlalchemy.exc import ArgumentError
+from sqlalchemy import Pool
 from sqlalchemy.pool import SingletonThreadPool
 
 OVERHAVE_ENV_PREFIX = "OVERHAVE_"
 
 
 class BaseOverhavePrefix(BaseSettings):
     """Possibility to change Overhave default settings from environment."""
 
     class Config:
         env_prefix = OVERHAVE_ENV_PREFIX
 
 
-class SAUrl(URL):
-    """Custom SQLAlchemy URL for Pydantic BaseSettings validation."""
+class SAUrl(sqlalchemy.engine.URL):  # SQLAlchemy2.0 - sa.URL
+    """Custom URL for Pydantic BaseSettings validation."""
 
     @classmethod
     def __get_validators__(cls):  # type: ignore
         yield cls.validate
 
     @classmethod
-    def validate(cls, v: str) -> URL:
+    def validate(cls, v: str) -> sqlalchemy.engine.URL:  # SQLAlchemy2.0 - sa.URL
         try:
-            return make_url(v)
-        except ArgumentError as e:
+            return sqlalchemy.engine.make_url(v)  # SQLAlchemy2.0 - sa.make_url
+        except sqlalchemy.exc.ArgumentError as e:
             raise ValueError from e
 
 
 class DataBaseSettings(BaseOverhavePrefix):
     """Overhave database settings."""
 
-    db_url: SAUrl = Field(SAUrl.validate("postgresql://postgres:postgres@localhost/overhave"))
+    db_url: SAUrl = Field(
+        SAUrl.validate("postgresql://postgres:postgres@localhost/overhave")  # type: ignore[assignment]
+    )
     db_pool_recycle: int = 500
     db_pool_size: int = 6
     db_echo: bool = False
     db_application_name: str = socket.gethostname()
     db_connect_timeout: int = 30
+    db_poolclass: type[Pool] = SingletonThreadPool
 
-    def create_engine(self) -> Engine:
-        return engine_from_config(
+    def _create_engine(self) -> sqlalchemy.engine.Engine:  # SQLAlchemy2.0 - sa.Engine
+        return sa.engine_from_config(
             {
                 "url": self.db_url,
                 "pool_recycle": self.db_pool_recycle,
                 "pool_pre_ping": True,
                 "pool_size": self.db_pool_size,
-                "poolclass": SingletonThreadPool,
+                "poolclass": self.db_poolclass,
                 "connect_args": {
                     "connect_timeout": self.db_connect_timeout,
                     "application_name": self.db_application_name,
                 },
             },
             prefix="",
         )
 
-    def setup_db(self) -> None:
-        from overhave.db.base import metadata
+    def setup_engine(self) -> None:
+        from overhave.db.base import current_session, metadata
 
-        metadata.bind = self.create_engine()
+        metadata.set_engine(engine=self._create_engine())
+        current_session.configure(bind=metadata.engine)
 
 
 class LoggingSettings(BaseOverhavePrefix):
     """Overhave logging settings."""
 
     log_level: str = logging.getLevelName(logging.INFO)
-    log_config: Dict[str, Any] = {}
+    log_config: dict[str, Any] = {}
 
     @validator("log_config", each_item=True)
-    def dict_config_validator(cls, v: Dict[str, Any]) -> Optional[DictConfigurator]:
+    def dict_config_validator(cls, v: dict[str, Any]) -> DictConfigurator | None:
         if not v:
             return None
         return DictConfigurator(v)
 
     def setup_logging(self) -> None:
         if isinstance(self.log_config, DictConfigurator):
             self.log_config.configure()
         else:
             logging.basicConfig(level=self.log_level)
 
 
-class AuthorizationStrategy(str, enum.Enum):
+class AuthorizationStrategy(enum.StrEnum):
     """
     Authorization strategies Enum.
 
     Simple - strategy without real auth_managers. Each user could use preferred name. This name will be used for user
     authority. Each user is unique. Password not required.
     Default - strategy with real auth_managers. Each user could use only registered credentials.
     LDAP - strategy with auth_managers using remote LDAP server. Each user should use his LDAP credentials. LDAP
```

### Comparing `overhave-3.9.0/overhave/cli/admin.py` & `overhave-4.0.0/overhave/cli/admin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from overhave import OverhaveAdminApp, overhave_app
 from overhave.base_settings import DataBaseSettings, LoggingSettings
 from overhave.cli.group import overhave
 from overhave.factory import get_admin_factory
 
 
 def _get_admin_app() -> OverhaveAdminApp:
-    DataBaseSettings().setup_db()
+    DataBaseSettings().setup_engine()
     LoggingSettings().setup_logging()
     return overhave_app(get_admin_factory())
 
 
 @overhave.command(short_help="Run Overhave Admin panel")
 def admin(port: int = 8076, debug: bool = False) -> None:
     _get_admin_app().run(host="localhost", port=port, debug=debug)
```

### Comparing `overhave-3.9.0/overhave/cli/api.py` & `overhave-4.0.0/overhave/cli/api.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/cli/consumers.py` & `overhave-4.0.0/overhave/cli/consumers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from overhave.base_settings import DataBaseSettings, LoggingSettings
 from overhave.cli.group import overhave
 from overhave.factory import ConsumerFactory
 from overhave.transport import RedisStream
 
 
 def _run_consumer(stream: RedisStream) -> None:
-    DataBaseSettings().setup_db()
+    DataBaseSettings().setup_engine()
     LoggingSettings().setup_logging()
     ConsumerFactory(stream=stream).runner.run()
 
 
 @overhave.command(short_help="Run Overhave Redis consumer")
 def consumer(
     stream: RedisStream = typer.Option(..., "-s", "--stream", help="Redis stream, which defines application")
```

### Comparing `overhave-3.9.0/overhave/cli/db_cmds/group.py` & `overhave-4.0.0/overhave/cli/db_cmds/group.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/cli/db_cmds/regular.py` & `overhave-4.0.0/overhave/cli/db_cmds/regular.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+# import sqlalchemy as sa  # noqa: E800
+import sqlalchemy.engine
 import sqlalchemy_utils as sau
 import typer
 from alembic.config import Config
-from sqlalchemy.engine.url import URL
 from sqlalchemy.exc import OperationalError
 
-from overhave import db as database
+from overhave import db
 from overhave.base_settings import DataBaseSettings
 
 
 def create_schema(config: Config) -> None:
     typer.echo("Creating...")
-    config.attributes["metadata"].create_all()
+    config.attributes["metadata"].create_all(bind=db.metadata.engine)
     typer.secho("Completed.", fg="green")
 
 
 def drop_schema(config: Config) -> None:
     typer.echo("Dropping...")
     meta = config.attributes["metadata"]
-    engine = config.attributes["engine"]
+    engine: sqlalchemy.engine.Engine = config.attributes["engine"]  # SQLAlchemy2.0 - sa.Engine
+
+    connection: sqlalchemy.engine.Connection = engine.connect()  # SQLAlchemy2.0 - sa.Connection
     for table in meta.tables:
-        engine.execute(f'DROP TABLE IF EXISTS "{table}" CASCADE')
-    engine.execute("DROP TABLE IF EXISTS alembic_version")
-    engine.execute("DROP SCHEMA IF EXISTS huey")
-    meta.drop_all()
+        connection.execute(sqlalchemy.text(f'DROP TABLE IF EXISTS "{table}" CASCADE'))
+    connection.execute(sqlalchemy.text("DROP TABLE IF EXISTS alembic_version"))
+
+    meta.drop_all(engine)
     typer.secho("Completed.", fg="green")
 
 
-def _ensure_database_exists(db_url: URL) -> None:
+def _ensure_database_exists(db_url: sqlalchemy.engine.URL) -> None:  # SQLAlchemy2.0 - sa.URL
     try:
         if not sau.database_exists(db_url):
             sau.create_database(db_url)
     except OperationalError as e:
         typer.echo(e)
         typer.echo("Catched error when trying to check database existence!")
 
 
 def set_config_to_context(context: typer.Context, settings: DataBaseSettings) -> None:
     """Set Alembic config to Typer context for easy operations and migrations ability."""
-    _ensure_database_exists(settings.db_url)
-    settings.setup_db()
+    settings.setup_engine()
+    _ensure_database_exists(db.metadata.engine.url)
+
     config = Config()
-    config.attributes["engine"] = settings.create_engine()
-    config.attributes["metadata"] = database.metadata
+    config.attributes["engine"] = db.metadata.engine
+    config.attributes["metadata"] = db.metadata
     context.obj = config
```

### Comparing `overhave-3.9.0/overhave/cli/s3.py` & `overhave-4.0.0/overhave/cli/s3.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/cli/synchronizer.py` & `overhave-4.0.0/overhave/cli/synchronizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import typer
 
 from overhave.base_settings import DataBaseSettings, LoggingSettings
 from overhave.factory import get_synchronizer_factory
-from overhave.scenario import FeatureValidator
+from overhave.scenario import IFeatureValidator
 from overhave.synchronization import IOverhaveSynchronizer
 
 sync_app = typer.Typer(short_help="Run Overhave features synchronization commands")
 
 
 def _create_synchronizer() -> IOverhaveSynchronizer:
-    DataBaseSettings().setup_db()
+    DataBaseSettings().setup_engine()
     LoggingSettings().setup_logging()
     return get_synchronizer_factory().synchronizer
 
 
 @sync_app.command(short_help="Run Overhave features synchronization")
 def run(
     create_db_features: bool = typer.Option(
         False, "-c", "--create-db-features", is_flag=True, help="Create features in database if necessary"
     ),
     pull_repository: bool = typer.Option(False, "-p", "--pull-repository", is_flag=True, help="Pull remote repository"),
 ) -> None:
     _create_synchronizer().synchronize(create_db_features, pull_repository)
 
 
-def _create_validator() -> FeatureValidator:
+def _create_validator() -> IFeatureValidator:
     LoggingSettings().setup_logging()
     return get_synchronizer_factory().feature_validator
 
 
 @sync_app.command(short_help="Run Overhave feature files validation")
 def validate_features(
     raise_if_nullable_id: bool = typer.Option(
```

### Comparing `overhave-3.9.0/overhave/db/base.py` & `overhave-4.0.0/overhave/db/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,103 @@
-from __future__ import annotations
-
-import datetime
 import logging
 import re
-from typing import List, Tuple, Type, Union
+from typing import Any, cast
 
 import sqlalchemy as sa
-from sqlalchemy import MetaData
-from sqlalchemy.ext.declarative import as_declarative, declared_attr
-from sqlalchemy.orm import Mapper
-from sqlalchemy.orm import Session as SessionClass
-from sqlalchemy.orm import scoped_session, sessionmaker
-from sqlalchemy.orm.query import Query
+import sqlalchemy.engine as se
+import sqlalchemy.orm as so
 
 logger = logging.getLogger(__name__)
 
 convention = {
     "ix": "ix_%(column_0_label)s",
     "uq": "uq_%(table_name)s_%(column_0_name)s",
     "ck": "ck_%(table_name)s_%(constraint_name)s",
     "fk": "fk_%(table_name)s_%(column_0_name)s_%(referred_table_name)s",
     "pk": "pk_%(table_name)s",
 }
-metadata = MetaData(naming_convention=convention)
 
 
-@as_declarative(metadata=metadata)
+class SAMetadata(sa.MetaData):
+    """Custom SQLAlchemy MetaData with bounded engine."""
+
+    def __init__(self, *args, **kwargs) -> None:  # type: ignore[no-untyped-def]
+        super().__init__(*args, **kwargs)
+        self._engine: se.Engine | None = None  # SQLAlchemy2.0 - sa.Engine
+
+    @property
+    def engine(self) -> se.Engine:  # SQLAlchemy2.0 - sa.Engine
+        if isinstance(self._engine, se.Engine):  # SQLAlchemy2.0 - sa.Engine
+            return self._engine
+        raise RuntimeError("MetaData has not got bounded Engine!")
+
+    def set_engine(self, engine: se.Engine) -> None:  # SQLAlchemy2.0 - sa.Engine
+        self._engine = engine
+
+
+metadata = SAMetadata(naming_convention=convention)
+
+
+def _classname_to_tablename(name: str) -> str:
+    result: list[str] = []
+
+    last_index = 0
+    for match in re.finditer(r"(?P<abbreviation>[A-Z]+(?![a-z\d]))|(?P<word>[A-Z][a-z]*)|(?P<digit>\d+)", name):
+        if match.start() != last_index:
+            raise ValueError(f'Could not translate class name "{name}" to table name')
+
+        last_index = match.end()
+        result.append(match.group().lower())
+
+    return "_".join(result)
+
+
+@so.as_declarative(metadata=metadata)
 class BaseTable:
     """Base table class with __tablename__."""
 
-    @declared_attr
+    @so.declared_attr  # SQLAlchemy2.0 - @so.declared_attr.directive
     def __tablename__(cls) -> str:
-        return _classname_to_tablename(cls.__name__)  # type: ignore
+        return _classname_to_tablename(cls.__name__)
 
 
 class PrimaryKeyWithoutDateMixin:
     """Table mixin with declared attribute `id`."""
 
-    @declared_attr
-    def id(cls) -> sa.Column[int]:
-        return sa.Column(f"{cls.__tablename__}_id", sa.Integer(), primary_key=True)  # type: ignore
+    @so.declared_attr.cascading
+    def id(cls):  # type: ignore[no-untyped-def]
+        return sa.Column(f"{getattr(cls, '__tablename__')}_id", sa.Integer(), primary_key=True)
 
 
 class PrimaryKeyMixin(PrimaryKeyWithoutDateMixin):
     """Table mixin with `id` and `created_at` declared attributes."""
 
-    @declared_attr
-    def created_at(cls) -> sa.Column[datetime.datetime]:
+    @so.declared_attr.cascading
+    def created_at(cls):  # type: ignore[no-untyped-def]
         return sa.Column(sa.DateTime(timezone=True), nullable=True, server_default=sa.func.now())
 
 
-def _get_query_cls(mapper: Union[Tuple[Type[BaseTable], ...], Mapper], session: SessionClass) -> Query:
+def _get_query_cls(
+    mapper: tuple[type[BaseTable], ...] | so.Mapper,  # type: ignore[type-arg]
+    session: Any,  # SQLAlchemy2.0 - session: so.SessionClass
+) -> so.Query:  # type: ignore[type-arg]  # SQLAlchemy2.0 - so.Query[Any]
     if mapper:
         m = mapper
         if isinstance(m, tuple):
-            m = mapper[0]
-        if isinstance(m, Mapper):
+            m = mapper[0]  # type: ignore[index, assignment]
+        if isinstance(m, so.Mapper):
             m = m.entity
 
         try:
-            return m.__query_cls__(mapper, session)
+            return cast(
+                so.Query,  # type: ignore[type-arg]  # SQLAlchemy2.0 - so.Query[Any]
+                m.__query_cls__(mapper, session),  # type: ignore[union-attr]
+            )
         except AttributeError:
             pass
 
-    return Query(mapper, session)
-
-
-def _classname_to_tablename(name: str) -> str:
-    result: List[str] = []
-
-    last_index = 0
-    for match in re.finditer(r"(?P<abbreviation>[A-Z]+(?![a-z\d]))|(?P<word>[A-Z][a-z]*)|(?P<digit>\d+)", name):
-        if match.start() != last_index:
-            raise ValueError(f'Could not translate class name "{name}" to table name')
-
-        last_index = match.end()
-        result.append(match.group().lower())
-
-    return "_".join(result)
+    return so.Query(mapper, session)  # type: ignore[arg-type]
 
 
-Session = sessionmaker(query_cls=_get_query_cls)
+Session = so.sessionmaker(query_cls=_get_query_cls)
 
-current_session = scoped_session(Session)
+current_session = so.scoped_session(Session)
```

### Comparing `overhave-3.9.0/overhave/db/statuses.py` & `overhave-4.0.0/overhave/db/statuses.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import enum
 
 
-class TestRunStatus(str, enum.Enum):
+class TestRunStatus(enum.StrEnum):
     """Enum for test run statuses."""
 
     __test__ = False
 
     STARTED = "STARTED"
     RUNNING = "RUNNING"
     FAILED = "FAILED"
@@ -28,32 +28,32 @@
     SAVED = "SAVED"
 
     @property
     def has_report(self) -> bool:
         return self in (TestReportStatus.GENERATED, TestReportStatus.SAVED)
 
 
-class EmulationStatus(str, enum.Enum):
+class EmulationStatus(enum.StrEnum):
     """Enum for emulation statuses."""
 
     CREATED = "CREATED"
     REQUESTED = "REQUESTED"
     READY = "READY"
     ERROR = "ERROR"
 
     @property
     def processed(self) -> bool:
         return self in (EmulationStatus.READY, EmulationStatus.ERROR)
 
 
-class DraftStatus(str, enum.Enum):
+class DraftStatus(enum.StrEnum):
     """Enum for draft statuses."""
 
     REQUESTED = "REQUESTED"
     CREATING = "CREATING"
     CREATED = "CREATED"
     INTERNAL_ERROR = "INTERNAL_ERROR"
     DUPLICATE = "DUPLICATE"
 
     @property
-    def success(self) -> bool:
+    def is_succeed(self) -> bool:
         return self in (DraftStatus.CREATED, DraftStatus.DUPLICATE)
```

### Comparing `overhave-3.9.0/overhave/db/tables.py` & `overhave-4.0.0/overhave/db/tables.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import datetime
-from typing import List, Optional, cast
+from typing import Dict, List
 
 import allure
 import sqlalchemy as sa
 import sqlalchemy_utils as su
 from flask import url_for
 from sqlalchemy import orm as so
 
@@ -13,206 +13,168 @@
 from overhave.db.statuses import DraftStatus, EmulationStatus, TestReportStatus, TestRunStatus
 from overhave.db.users import UserRole
 
 
 class FeatureType(BaseTable, PrimaryKeyWithoutDateMixin):
     """Feature types table."""
 
-    name = sa.Column(sa.Text, unique=True, nullable=False, doc="Feature types choice")
+    name: str = sa.Column(sa.Text, unique=True, nullable=False, doc="Feature types choice")
 
     def __repr__(self) -> str:
-        return cast(str, self.name.upper())
+        return self.name.upper()
 
 
 class Tags(BaseTable, PrimaryKeyMixin):
     """Feature tags table."""
 
-    value = sa.Column(sa.String(), nullable=False, doc="Feature tags choice", unique=True)
-    created_by = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), doc="Author login", nullable=False)
+    value: str = sa.Column(sa.String(), nullable=False, unique=True, doc="Feature tags choice")
+    created_by: str = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), nullable=False, doc="Author login")
 
     def __repr__(self) -> str:
-        return cast(str, self.value)
+        return self.value
 
     def __init__(self, value: str, created_by: str) -> None:
         self.value = value
         self.created_by = created_by
 
 
 @su.generic_repr("id", "name", "last_edited_by")
 class Feature(BaseTable, PrimaryKeyMixin):
     """Features table."""
 
-    name = sa.Column(sa.String(), doc="Feature name", nullable=False, unique=True)
-    author = sa.Column(
+    name: str = sa.Column(sa.String(), doc="Feature name", nullable=False, unique=True)
+    author: str = sa.Column(
         sa.String(), sa.ForeignKey(UserRole.login), doc="Feature author login", nullable=False, index=True
     )
-    type_id = sa.Column(sa.Integer(), sa.ForeignKey(FeatureType.id), nullable=False, doc="Feature types choice")
-    file_path = sa.Column(sa.String(), doc="Feature file path", nullable=False, unique=True)
-    task = sa.Column(sa.ARRAY(sa.String()), doc="Feature tasks list", nullable=False)
-    last_edited_by = sa.Column(sa.String(), doc="Last feature editor login", nullable=False)
-    last_edited_at = sa.Column(sa.DateTime(timezone=True), nullable=False, server_default=sa.func.now())
-    released = sa.Column(sa.Boolean, doc="Feature release state boolean", nullable=False, default=False)
-    severity = sa.Column(
+    type_id: int = sa.Column(sa.Integer(), sa.ForeignKey(FeatureType.id), nullable=False, doc="Feature types choice")
+    file_path: str = sa.Column(sa.String(), doc="Feature file path", nullable=False, unique=True)
+    task: List[str] = sa.Column(sa.ARRAY(sa.String()), doc="Feature tasks list", nullable=False)
+    last_edited_by: str = sa.Column(sa.String(), doc="Last feature editor login", nullable=False)
+    last_edited_at: datetime.datetime = sa.Column(
+        sa.DateTime(timezone=True), nullable=False, server_default=sa.func.now()
+    )
+    released: bool = sa.Column(sa.Boolean, doc="Feature release state boolean", nullable=False, default=False)
+    severity: allure.severity_level = sa.Column(
         sa.Enum(allure.severity_level),
         nullable=False,
         default=allure.severity_level.NORMAL,
         doc="Feature severity choice",
     )
 
-    feature_type = so.relationship(FeatureType)
-    feature_tags = so.relationship(Tags, order_by=Tags.value, secondary="feature_tags_association_table")
-
-    def __init__(
-        self,
-        name: str,
-        author: str,
-        type_id: int,
-        file_path: str,
-        task: List[str],
-        severity: allure.severity_level,
-        last_edited_at: datetime.datetime,
-    ) -> None:
-        self.name = name
-        self.author = author
-        self.type_id = type_id
-        self.file_path = file_path
-        self.task = task
-        self.last_edited_by = author
-        self.severity = severity
-        self.last_edited_at = last_edited_at
+    feature_type: so.Mapped[FeatureType] = so.relationship(FeatureType, uselist=False)
+    feature_tags: so.Mapped[List[Tags]] = so.relationship(
+        Tags, uselist=True, order_by=Tags.value, secondary="feature_tags_association_table"
+    )
 
 
 class FeatureTagsAssociationTable(BaseTable, PrimaryKeyWithoutDateMixin):
     """Association table between features and tags."""
 
     extend_existing = True
 
-    tags_id = sa.Column(sa.Integer(), sa.ForeignKey(Tags.id))
-    feature_id = sa.Column(sa.Integer(), sa.ForeignKey(Feature.id))
+    tags_id: int = sa.Column(sa.Integer(), sa.ForeignKey(Tags.id))
+    feature_id: int = sa.Column(sa.Integer(), sa.ForeignKey(Feature.id))
 
 
 @su.generic_repr("feature_id")
 class Scenario(BaseTable, PrimaryKeyMixin):
     """Scenarios table."""
 
-    feature_id = sa.Column(sa.Integer(), sa.ForeignKey(Feature.id), nullable=False, unique=True)
-    text = sa.Column(sa.Text(), doc="Text storage for scenarios in feature")
+    feature_id: int = sa.Column(sa.Integer(), sa.ForeignKey(Feature.id), nullable=False, unique=True)
+    text: str | None = sa.Column(sa.Text(), doc="Text storage for scenarios in feature")
 
-    feature = so.relationship(Feature, backref=so.backref("scenario", cascade="all, delete-orphan"))
+    feature: so.Mapped[Feature] = so.relationship(
+        Feature, uselist=False, backref=so.backref("scenario", cascade="all, delete-orphan")
+    )
 
 
 class TestRun(BaseTable, PrimaryKeyMixin):
     """Test runs table."""
 
     __test__ = False
 
-    scenario_id = sa.Column(sa.Integer(), sa.ForeignKey(Scenario.id), nullable=False, index=True)
-    name = sa.Column(sa.String(), nullable=False)
-    start = sa.Column(sa.DateTime(timezone=True), doc="Test start time")
-    end = sa.Column(sa.DateTime(timezone=True), doc="Test finish time")
-    status = sa.Column(sa.Enum(TestRunStatus), doc="Current test status", nullable=False)
-    report_status = sa.Column(sa.Enum(TestReportStatus), doc="Report generation result", nullable=False)
-    executed_by = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), doc="Test executor login", nullable=False)
-    report = sa.Column(sa.String(), doc="Relative report URL")
-    traceback = sa.Column(sa.Text(), doc="Text storage for error traceback")
-
-    scenario = so.relationship(Scenario, backref=so.backref("test_runs", cascade="all, delete-orphan"))
-
-
-class DraftQuery(so.Query):
-    """Scenario versions table."""
+    scenario_id: int = sa.Column(sa.Integer(), sa.ForeignKey(Scenario.id), nullable=False, index=True)
+    name: str = sa.Column(sa.String(), nullable=False)
+    start: datetime.datetime | None = sa.Column(sa.DateTime(timezone=True), doc="Test start time")
+    end: datetime.datetime | None = sa.Column(sa.DateTime(timezone=True), doc="Test finish time")
+    status: TestRunStatus = sa.Column(sa.Enum(TestRunStatus), doc="Current test status", nullable=False)
+    report_status: TestReportStatus = sa.Column(
+        sa.Enum(TestReportStatus), doc="Report generation result", nullable=False
+    )
+    executed_by: str = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), doc="Test executor login", nullable=False)
+    report: str | None = sa.Column(sa.String(), doc="Relative report URL")
+    traceback: str | None = sa.Column(sa.Text(), doc="Text storage for error traceback")
 
-    def as_unique(self, test_run_id: int, published_by: str, status: DraftStatus) -> Draft:
-        with self.session.no_autoflush:
-            run = self.session.query(TestRun).get(test_run_id)
-            if run is None:
-                raise RuntimeError(f"Unknown test_run_id={test_run_id}!")
-            draft: Optional[Draft] = (
-                self.session.query(Draft)
-                .filter(Draft.test_run_id == run.id, Draft.text == run.scenario.text)
-                .one_or_none()
-            )
-        if draft:
-            return draft
-        return Draft(
-            feature_id=run.scenario.feature_id,
-            test_run_id=test_run_id,
-            text=run.scenario.text,
-            published_by=published_by,
-            status=status,
-        )
+    scenario: so.Mapped[Scenario] = so.relationship(
+        Scenario, uselist=False, backref=so.backref("test_runs", cascade="all, delete-orphan")
+    )
 
 
 class Draft(BaseTable, PrimaryKeyMixin):
     """Scenario versions table."""
 
-    __query_cls__ = DraftQuery
-
-    feature_id = sa.Column(sa.Integer(), sa.ForeignKey(Feature.id), nullable=False, index=True)
-    test_run_id = sa.Column(sa.Integer(), sa.ForeignKey(TestRun.id), nullable=False)
-    text = sa.Column(sa.Text(), doc="Released scenario text")
-    pr_url = sa.Column(sa.String(), doc="Absolute pull-request URL", nullable=True)
-    published_by = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), doc="Draft publisher login", nullable=False)
-    published_at = sa.Column(sa.DateTime(timezone=True), doc="Publication time")
-    traceback = sa.Column(sa.Text(), doc="Text storage for error traceback", nullable=True)
-    status = sa.Column(sa.Enum(DraftStatus), doc="Version publishing status", nullable=False)
-
-    feature = so.relationship(Feature, backref=so.backref("versions", cascade="all, delete-orphan"))
+    feature_id: int = sa.Column(sa.Integer(), sa.ForeignKey(Feature.id), nullable=False, index=True)
+    test_run_id: int = sa.Column(sa.Integer(), sa.ForeignKey(TestRun.id), unique=True, nullable=False)
+    text: str | None = sa.Column(sa.Text(), doc="Released scenario text")
+    pr_url: str | None = sa.Column(sa.String(), doc="Absolute pull-request URL")
+    published_by: str = sa.Column(
+        sa.String(), sa.ForeignKey(UserRole.login), doc="Draft publisher login", nullable=False
+    )
+    published_at: datetime.datetime | None = sa.Column(sa.DateTime(timezone=True), doc="Publication time")
+    traceback: str | None = sa.Column(sa.Text(), doc="Text storage for error traceback")
+    status: DraftStatus = sa.Column(sa.Enum(DraftStatus), doc="Version publishing status", nullable=False)
 
-    __table_args__ = (sa.UniqueConstraint(test_run_id),)
+    feature: so.Mapped[Feature] = so.relationship(
+        Feature, uselist=False, backref=so.backref("versions", cascade="all, delete-orphan")
+    )
 
     def __html__(self) -> str:
         return f'<a href="{url_for("draft.details_view", id=self.id)}">Draft: {self.id}</a>'
 
-    def __init__(self, feature_id: int, test_run_id: int, text: str, published_by: str, status: DraftStatus) -> None:
-        self.feature_id = feature_id
-        self.test_run_id = test_run_id
-        self.text = text
-        self.published_by = published_by
-        self.status = status
-
 
 @su.generic_repr("id", "name", "created_by")
 class TestUser(BaseTable, PrimaryKeyMixin):
     """Test users table."""
 
     __test__ = False
 
-    name = sa.Column(sa.String(), nullable=False, unique=True)
-    feature_type_id = sa.Column(sa.Integer(), sa.ForeignKey(FeatureType.id), nullable=False, doc="Feature types choice")
-    specification = sa.Column(sa.JSON(none_as_null=True))
-    created_by = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), doc="Author login", nullable=False)
-    allow_update = sa.Column(sa.Boolean(), doc="User updating allowance", nullable=False, default=False)
-    changed_at = sa.Column(sa.DateTime(timezone=True), nullable=False, server_default=sa.func.now())
+    key: str = sa.Column(sa.String(), nullable=False, unique=True, doc="Unique user key")
+    name: str = sa.Column(sa.String(), nullable=False, unique=True, doc="Informational user name")
+    feature_type_id: int = sa.Column(
+        sa.Integer(), sa.ForeignKey(FeatureType.id), nullable=False, doc="Feature types choice"
+    )
+    specification: Dict[str, str | None] = sa.Column(sa.JSON(none_as_null=True))
+    created_by: str = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), doc="Author login", nullable=False)
+    allow_update: bool = sa.Column(sa.Boolean(), doc="User updating allowance", nullable=False, default=False)
+    changed_at: datetime.datetime = sa.Column(sa.DateTime(timezone=True), nullable=False, server_default=sa.func.now())
 
-    feature_type = so.relationship(FeatureType)
+    feature_type: so.Mapped[FeatureType] = so.relationship(FeatureType, uselist=False)
 
 
 class Emulation(BaseTable, PrimaryKeyMixin):
     """Emulation templates table."""
 
-    name = sa.Column(sa.String(), nullable=False, unique=True)
-    test_user_id = sa.Column(sa.Integer(), sa.ForeignKey(TestUser.id), nullable=False, doc="Test user ID")
-    command = sa.Column(sa.String(), nullable=False, doc="Command for emulator's execution")
-    created_by = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), doc="Author login", nullable=False)
-    test_user = so.relationship(TestUser, backref=so.backref("emulations", cascade="all, delete-orphan"))
+    name: str = sa.Column(sa.String(), nullable=False, unique=True)
+    test_user_id: int = sa.Column(sa.Integer(), sa.ForeignKey(TestUser.id), nullable=False, doc="Test user ID")
+    command: str = sa.Column(sa.String(), nullable=False, doc="Command for emulator's execution")
+    created_by: str = sa.Column(sa.String(), sa.ForeignKey(UserRole.login), doc="Author login", nullable=False)
+
+    test_user: so.Mapped[TestUser] = so.relationship(
+        TestUser, uselist=False, backref=so.backref("emulations", cascade="all, delete-orphan")
+    )
 
 
 class EmulationRun(BaseTable, PrimaryKeyMixin):
     """Emulation runs table."""
 
-    __tablename__ = "emulation_run"  # type: ignore
-    emulation_id = sa.Column(sa.Integer(), sa.ForeignKey(Emulation.id), nullable=False, index=True)
-    status = sa.Column(sa.Enum(EmulationStatus), doc="Current emulation status", nullable=False)
-    changed_at = sa.Column(sa.DateTime(timezone=True), nullable=False, server_default=sa.func.now())
-    port = sa.Column(sa.Integer(), doc="Port for emulation")
-    traceback = sa.Column(sa.Text(), doc="Text storage for error traceback")
-    initiated_by = sa.Column(
+    emulation_id: int = sa.Column(sa.Integer(), sa.ForeignKey(Emulation.id), nullable=False, index=True)
+    status: EmulationStatus = sa.Column(sa.Enum(EmulationStatus), doc="Current emulation status", nullable=False)
+    changed_at: datetime.datetime = sa.Column(sa.DateTime(timezone=True), nullable=False, server_default=sa.func.now())
+    port: int | None = sa.Column(sa.Integer(), doc="Port for emulation")
+    traceback: str | None = sa.Column(sa.Text(), doc="Text storage for error traceback")
+    initiated_by: str = sa.Column(
         sa.String(), sa.ForeignKey(UserRole.login), doc="Initiator of start emulation", nullable=False
     )
 
-    emulation = so.relationship(Emulation, backref=so.backref("emulation_runs", cascade="all, delete-orphan"))
-
-    def __init__(self, emulation_id: int, initiated_by: str) -> None:
-        self.emulation_id = emulation_id
-        self.status = EmulationStatus.CREATED
-        self.initiated_by = initiated_by
+    emulation: so.Mapped[Emulation] = so.relationship(
+        Emulation, uselist=False, backref=so.backref("emulation_runs", cascade="all, delete-orphan")
+    )
```

### Comparing `overhave-3.9.0/overhave/db/users.py` & `overhave-4.0.0/overhave/db/users.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,32 @@
 import enum
-from typing import Optional
 
 import sqlalchemy as sa
 import sqlalchemy_utils as su
 
 from overhave.db.base import BaseTable, PrimaryKeyMixin
 
 
-class Role(str, enum.Enum):
+class Role(enum.StrEnum):
     """Enum that declares user access roles."""
 
     user = "user"
     admin = "admin"
 
 
 @su.generic_repr("login", "role")
 class UserRole(BaseTable, PrimaryKeyMixin):
     """User access table."""
 
-    login = sa.Column(sa.String(), nullable=False, unique=True)
-    password = sa.Column(sa.String(), nullable=True)
-    role = sa.Column(sa.Enum(Role), nullable=False, default=Role.user)
-
-    def __init__(self, login: str, password: Optional[str], role: Role) -> None:
-        self.login = login
-        self.password = password
-        self.role = role
+    login: str = sa.Column(sa.String(), nullable=False, unique=True)
+    password: str | None = sa.Column(sa.String())
+    role: Role = sa.Column(sa.Enum(Role), nullable=False, default=Role.user)
 
     def __repr__(self) -> str:
         return f"{self.login} ({self.role})"
 
 
 @su.generic_repr("group")
 class GroupRole(BaseTable, PrimaryKeyMixin):
     """Group access table."""
 
-    group = sa.Column(sa.String(), nullable=False, unique=True)
-
-    def __init__(self, group: str) -> None:
-        self.group = group
+    group: str = sa.Column(sa.String(), nullable=False, unique=True)
```

### Comparing `overhave-3.9.0/overhave/db/utils.py` & `overhave-4.0.0/overhave/db/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import logging
 from contextlib import contextmanager
-from typing import Any, Iterator, List
+from typing import Any, Iterator
 
 import sqlalchemy.orm as so
 from sqlalchemy.exc import ProgrammingError
 
-from overhave.db.base import Session
+from overhave.db.base import Session, metadata
 from overhave.db.tables import FeatureType
 
 logger = logging.getLogger(__name__)
 
 
 @contextmanager
 def create_session(**kwargs: Any) -> Iterator[so.Session]:
     """Provide a transactional scope around a series of operations."""
-    new_session = Session(**kwargs)
+    new_session = Session(bind=metadata.engine, **kwargs)
     try:
         yield new_session
         new_session.commit()
     except Exception:
         new_session.rollback()
         raise
     finally:
         new_session.close()
 
 
-def ensure_feature_types_exist(feature_types: List[str]) -> None:
+def ensure_feature_types_exist(feature_types: list[str]) -> None:
     with create_session() as session:
         try:
             for feature_type in feature_types:
                 existing_type = session.query(FeatureType).filter_by(name=feature_type).one_or_none()
                 if existing_type is not None:
                     continue
-                session.add(FeatureType(name=feature_type))  # type: ignore
+                session.add(FeatureType(name=feature_type))
                 logger.info("Created feature type '%s'", feature_type)
         except ProgrammingError:
             logger.exception("Could not create feature types dynamically!")
```

### Comparing `overhave-3.9.0/overhave/emulation/emulator.py` & `overhave-4.0.0/overhave/emulation/emulator.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import re
 import subprocess
 from functools import cached_property
 from typing import Pattern
 
 from overhave import db
 from overhave.entities.settings import OverhaveEmulationSettings
+from overhave.metrics import EmulationRunOverhaveMetricContainer
 from overhave.storage import EmulationRunModel, EmulationStorageError, IEmulationStorage
 from overhave.transport import EmulationTask
 
 logger = logging.getLogger(__name__)
 
 
 class EmulationError(Exception):
@@ -36,17 +37,23 @@
         if self._dangerous_pattern.match(cmd) is not None:
             raise DangerousExternalCommandError(f"Dangerous external command: '{cmd}'")
 
 
 class Emulator(ExternalCommandCheckMixin):
     """Class for creation of emulation runs."""
 
-    def __init__(self, settings: OverhaveEmulationSettings, storage: IEmulationStorage):
+    def __init__(
+        self,
+        settings: OverhaveEmulationSettings,
+        storage: IEmulationStorage,
+        metric_container: EmulationRunOverhaveMetricContainer,
+    ):
         self._settings = settings
         self._storage = storage
+        self._metric_container = metric_container
 
     def _initiate(self, emulation_run: EmulationRunModel) -> None:
         if not isinstance(self._settings.emulation_base_cmd, str):
             raise EmulationNotEnabledError("Emulation not enabled: 'emulation_base_cmd' has not been specified!")
 
         cmd_from_user = emulation_run.emulation.command.strip()
         self._check_dangerous(cmd_from_user)
@@ -65,15 +72,15 @@
             [self._settings.emulation_core_path]
             + formatted_prefix.split(" ")
             + emulation_base_cmd
             + cmd_from_user.split(" ")
         )
         if isinstance(self._settings.emulation_postfix, str):
             emulation_cmd += self._settings.emulation_postfix.format(
-                name=emulation_run.emulation.test_user.name.replace(" ", "_"),
+                name=emulation_run.emulation.test_user.key.replace(" ", "_"),
                 model=json.dumps(emulation_run.emulation.test_user.specification).replace(" ", ""),
             ).split(" ")
         logger.debug("Emulation command: %s", " ".join(emulation_cmd))
         try:
             subprocess.Popen(emulation_cmd)
         except (subprocess.CalledProcessError, FileNotFoundError) as e:
             logger.error("Error while starting emulation process!")
@@ -82,10 +89,14 @@
     def start_emulation(self, task: EmulationTask) -> None:
         emulation_run_id = task.data.emulation_run_id
         try:
             emulation_run = self._storage.get_requested_emulation_run(emulation_run_id)
             logger.info("Try to emulate: %s", emulation_run.emulation)
             self._initiate(emulation_run)
             self._storage.set_emulation_run_status(emulation_run_id=emulation_run.id, status=db.EmulationStatus.READY)
+            self._metric_container.add_emulation_task_status(
+                status=db.EmulationStatus.READY.value, port=emulation_run.port
+            )
         except (EmulationError, EmulationStorageError) as e:
             logger.exception("Could not emulate task %s!", task)
             self._storage.set_error_emulation_run(emulation_run_id=emulation_run_id, traceback=str(e))
+            self._metric_container.add_emulation_task_status(status=db.EmulationStatus.ERROR.value, port=None)
```

### Comparing `overhave-3.9.0/overhave/entities/__init__.py` & `overhave-4.0.0/overhave/entities/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,12 +14,11 @@
 from .report_manager import ReportManager, ReportPresenceResolution
 from .settings import (
     OverhaveAdminSettings,
     OverhaveDescriptionManagerSettings,
     OverhaveEmulationSettings,
     OverhaveFileSettings,
     OverhaveLanguageSettings,
-    OverhaveRedisSettings,
     OverhaveReportManagerSettings,
     OverhaveStepContextSettings,
     ProcessorSettings,
 )
```

### Comparing `overhave-3.9.0/overhave/entities/archiver.py` & `overhave-4.0.0/overhave/entities/archiver.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/entities/auth_managers/default.py` & `overhave-4.0.0/overhave/entities/auth_managers/default.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Optional
 
 from pydantic import SecretStr
 
 from overhave.entities.auth_managers.secret_mixin import AdminSecretMixin
 from overhave.storage import SystemUserModel
 
 logger = logging.getLogger(__name__)
@@ -11,9 +10,9 @@
 
 class DefaultAdminAuthorizationManager(AdminSecretMixin):
     """Class for user auth_managers.
 
     Manager authorize users with registered credentials.
     """
 
-    def authorize_user(self, username: str, password: SecretStr) -> Optional[SystemUserModel]:
+    def authorize_user(self, username: str, password: SecretStr) -> SystemUserModel | None:
         return self._system_user_storage.get_user_by_credits(login=username, password=password)
```

### Comparing `overhave-3.9.0/overhave/entities/auth_managers/ldap/manager.py` & `overhave-4.0.0/overhave/entities/auth_managers/ldap/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from pprint import pformat
-from typing import List, Optional
 
 from pydantic import SecretStr
 
 from overhave.db import Role
 from overhave.entities.auth_managers.base import BaseAdminAuthorizationManager
 from overhave.entities.auth_managers.ldap.settings import OverhaveLdapManagerSettings
 from overhave.storage import ISystemUserGroupStorage, ISystemUserStorage, SystemUserModel
@@ -33,21 +32,21 @@
         ldap_authenticator: LDAPAuthenticator,
     ):
         super().__init__(system_user_storage)
         self._settings = settings
         self._system_user_group_storage = system_user_group_storage
         self._ldap_authenticator = ldap_authenticator
 
-    def _reassign_role_if_neccessary(self, user: SystemUserModel, user_groups: List[str]) -> None:
+    def _reassign_role_if_neccessary(self, user: SystemUserModel, user_groups: list[str]) -> None:
         if self._settings.ldap_admin_group not in user_groups:
             return
         user.role = Role.admin
         self._system_user_storage.update_user_role(user_model=user)
 
-    def authorize_user(self, username: str, password: SecretStr) -> Optional[SystemUserModel]:
+    def authorize_user(self, username: str, password: SecretStr) -> SystemUserModel | None:
         logger.debug("Try to authorize user '%s'...", username)
         user_groups = self._ldap_authenticator.get_user_groups(username, password)
         if not user_groups:
             logger.info("LDAP user '%s' does not exist!", username)
             return None
         logger.debug("LDAP user groups: \n %s", pformat(user_groups))
         user = self._system_user_storage.get_user_by_credits(login=username)
```

### Comparing `overhave-3.9.0/overhave/entities/auth_managers/secret_mixin.py` & `overhave-4.0.0/overhave/entities/auth_managers/secret_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/entities/auth_managers/simple.py` & `overhave-4.0.0/overhave/entities/auth_managers/simple.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Optional
 
 from pydantic import SecretStr
 
 from overhave.entities.auth_managers.secret_mixin import AdminSecretMixin
 from overhave.storage import SystemUserModel
 
 logger = logging.getLogger(__name__)
@@ -20,15 +19,15 @@
 class SimpleAdminAuthorizationManager(AdminSecretMixin):
     """Class for user registration.
 
     Manager does not provide real auth_managers. Each user could use preferred name.
     This name will be used for user authority. Each user is unique. Passwords not required.
     """
 
-    def authorize_user(self, username: str, password: SecretStr) -> Optional[SystemUserModel]:
+    def authorize_user(self, username: str, password: SecretStr) -> SystemUserModel | None:
         user = self._system_user_storage.get_user_by_credits(login=username)
         if user is None:
             user = self._system_user_storage.create_user(login=username, password=password)
         if user.password is None:
             raise NullablePasswordError(f"User with id={user.id} has not got password!")
         if user.password.get_secret_value() == password.get_secret_value():
             return user
```

### Comparing `overhave-3.9.0/overhave/entities/feature/extractor.py` & `overhave-4.0.0/overhave/entities/feature/extractor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 from pathlib import Path
-from typing import Dict, List
 
 from overhave.entities.feature.abstract import IFeatureExtractor
 from overhave.entities.feature.errors import FeatureTypeExtractionError, ScenariosTestFileNotFound
 from overhave.entities.settings import OverhaveFileSettings
 from overhave.storage import FeatureTypeName
 
 logger = logging.getLogger(__name__)
@@ -12,43 +11,40 @@
 
 class FeatureExtractor(IFeatureExtractor):
     """Class for specified project's feature types resolution."""
 
     def __init__(self, file_settings: OverhaveFileSettings):
         self._file_settings = file_settings
 
-        self._feature_types: List[FeatureTypeName] = []
-        self._feature_type_to_dir_mapping: Dict[FeatureTypeName, Path] = {}
+        self._feature_types: list[FeatureTypeName] = []
+        self._feature_type_to_dir_mapping: dict[FeatureTypeName, Path] = {}
         try:
             self._extract_project_data()
             self._check_pytest_bdd_scenarios_test_files()
         except FeatureTypeExtractionError:
             logger.exception("Extraction error while trying to collect features!")
 
     def _extract_project_data(self) -> None:
-        feature_type_dirs = []
         try:
-            feature_type_dirs = [
+            feature_type_dirs = tuple(
                 d
                 for d in self._file_settings.features_dir.iterdir()
                 if all(
                     (
                         d.is_dir(),
                         d != self._file_settings.tmp_dir,
                         not d.name.startswith("."),
                         not d.name.startswith("_"),
                     )
                 )
-            ]
-        except FileNotFoundError:
-            pass
-        if not feature_type_dirs:
+            )
+        except FileNotFoundError as err:
             raise FeatureTypeExtractionError(
                 f"Could not find any subdirectory in specified features directory '{self._file_settings.features_dir}'!"
-            )
+            ) from err
         self._feature_types = [FeatureTypeName(t.name) for t in feature_type_dirs]
         logger.info("Registered feature types: %s", self._feature_types)
         self._feature_type_to_dir_mapping = {FeatureTypeName(t.name): t for t in feature_type_dirs}
 
     def _check_pytest_bdd_scenarios_test_files(self) -> None:
         for feature_type in self._feature_types:
             scenarios_file = self._file_settings.fixtures_dir / self._file_settings.fixtures_file_template_mask.format(
@@ -58,13 +54,13 @@
                 continue
             raise ScenariosTestFileNotFound(
                 "Could not find pytest-bdd test file with scenarios definition! "
                 f"Maybe you don't created '{scenarios_file.name}' in '{scenarios_file.parent}' directory?"
             )
 
     @property
-    def feature_types(self) -> List[FeatureTypeName]:
+    def feature_types(self) -> list[FeatureTypeName]:
         return self._feature_types
 
     @property
-    def feature_type_to_dir_mapping(self) -> Dict[FeatureTypeName, Path]:
+    def feature_type_to_dir_mapping(self) -> dict[FeatureTypeName, Path]:
         return self._feature_type_to_dir_mapping
```

### Comparing `overhave-3.9.0/overhave/entities/file_extractor.py` & `overhave-4.0.0/overhave/entities/file_extractor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from pathlib import Path
-from typing import List
 
 
 class BaseFileExtractor:
     """Base class for file extraction."""
 
     def __init__(self, extenstion: str) -> None:
         self._extenstion = extenstion
@@ -18,18 +17,18 @@
                 not path.is_dir(),
                 path.suffix == self._extenstion,
                 not path.name.startswith("."),
                 not path.name.startswith("_"),
             )
         )
 
-    def _extract_recursively(self, folder: Path) -> List[Path]:
+    def _extract_recursively(self, folder: Path) -> list[Path]:
         files = []
         for path in folder.iterdir():
             if self._check_dir_compliance(path):
                 subdirs = self._extract_recursively(path)
                 files.extend(subdirs)
                 continue
             if not self._check_file_compliance(path):
                 continue
             files.append(path)
-        return files
+        return sorted(files, key=lambda x: str(x))
```

### Comparing `overhave-3.9.0/overhave/entities/git_initializer.py` & `overhave-4.0.0/overhave/entities/git_initializer.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/entities/language/prefixes.py` & `overhave-4.0.0/overhave/entities/language/prefixes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List, Optional, Tuple, cast
-
 from pydantic.main import BaseModel
 from pytest_bdd import types as default_types
 from pytest_bdd.parser import STEP_PREFIXES
 
 
 class StepPrefixesModel(BaseModel):
     """Base model for default STEP_PREFIXES extension."""
@@ -15,15 +13,15 @@
     EXAMPLES: str
     GIVEN: str
     WHEN: str
     THEN: str
     AND: str
     BUT: str
 
-    def extend_defaults(self) -> List[Tuple[str, Optional[str]]]:
+    def extend_defaults(self) -> list[tuple[str, str | None]]:
         """Extend default STEP_PREFIXES from pytest_bdd."""
         STEP_PREFIXES.append((self.FEATURE, default_types.FEATURE))
         STEP_PREFIXES.append((self.SCENARIO_OUTLINE, default_types.SCENARIO_OUTLINE))
         STEP_PREFIXES.append((self.SCENARIO, default_types.SCENARIO))
         STEP_PREFIXES.append((self.BACKGROUND, default_types.BACKGROUND))
 
         STEP_PREFIXES.append((self.EXAMPLES, default_types.EXAMPLES))
@@ -31,8 +29,8 @@
         STEP_PREFIXES.append((self.GIVEN, default_types.GIVEN))
         STEP_PREFIXES.append((self.WHEN, default_types.WHEN))
         STEP_PREFIXES.append((self.THEN, default_types.THEN))
 
         STEP_PREFIXES.append((self.AND, None))
         STEP_PREFIXES.append((self.BUT, None))
 
-        return cast(List[Tuple[str, Optional[str]]], STEP_PREFIXES)
+        return STEP_PREFIXES
```

### Comparing `overhave-3.9.0/overhave/entities/report_manager/report_manager.py` & `overhave-4.0.0/overhave/entities/report_manager/report_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 import subprocess  # noqa: S404
 from os import makedirs
 from pathlib import Path
-from typing import Optional
 from uuid import uuid1
 
 from overhave.db import TestReportStatus
 from overhave.entities.archiver import ArchiveManager
 from overhave.entities.report_manager.models import ReportPresenceResolution
 from overhave.entities.settings import OverhaveFileSettings, OverhaveReportManagerSettings
 from overhave.storage import ITestRunStorage
@@ -28,23 +27,23 @@
     ) -> None:
         self._settings = settings
         self._file_settings = file_settings
         self._test_run_storage = test_run_storage
         self._archive_manager = archive_manager
         self._s3_manager = s3_manager
 
-    def _generate_report(self, alluredir: Path, report_dir: Path) -> Optional[int]:
-        generation_cmd = [
+    def _generate_report(self, alluredir: Path, report_dir: Path) -> int | None:
+        generation_cmd = (
             self._settings.allure_cmdline,
             "generate",
             f"{alluredir}/",
             "--output",
             report_dir.as_posix(),
             "--clean",
-        ]
+        )
         logger.debug("Allure report generation command: %s", " ".join(generation_cmd))
         makedirs(report_dir.as_posix(), exist_ok=True)
         try:
             return subprocess.run(  # noqa: S603
                 generation_cmd,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
@@ -84,15 +83,15 @@
         if report_dir.exists() and report_index.exists():
             return ReportPresenceResolution(exists=True)
 
         if not report_dir.exists():
             logger.warning("Report '%s' does not exist!", report_index.parent.name)
         if not report_index.exists():
             logger.warning("Report '%s' does not contain compiled files for HTML view!", report_index.parent.name)
-        test_run = self._test_run_storage.get_test_run(run_id)
+        test_run = self._test_run_storage.get_testrun_model(run_id=run_id)
         if test_run is None:
             logger.warning("No one test run with id=%s exists!", run_id)
             return ReportPresenceResolution(exists=False)
 
         resolution = ReportPresenceResolution(
             exists=False, s3_enabled=self._s3_manager.enabled, report_status=test_run.report_status
         )
```

### Comparing `overhave-3.9.0/overhave/entities/settings.py` & `overhave-4.0.0/overhave/entities/settings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Sequence, Union
+from typing import Any, Sequence
 
+import httpx
 from flask_admin.contrib.sqla import ModelView
 from pydantic import root_validator, validator
 from pydantic.datetime_parse import timedelta
-from yarl import URL
 
 from overhave.base_settings import BaseOverhavePrefix
 from overhave.entities.language import StepPrefixesModel
 
 
 class OverhaveAdminSettings(BaseOverhavePrefix):
     """Settings for Overhave Flask Admin customization."""
 
     # Path to custom index template. By default, contains Overhave project info.
-    index_template_path: Optional[Path]
+    index_template_path: Path | None
 
     # Custom SQLAlchemy ModelViews for Overhave admin panel
-    custom_views: Optional[Sequence[ModelView]]
+    custom_views: Sequence[ModelView] | None
 
     # Enable testing with test execution consumer, based on Redis tasks. Enabled by default.
     # When disabled - all test runs will be executed with :class:`Threadpool`.
     consumer_based: bool = True
 
     # Threadpool size for admin service
     threadpool_process_num: int = 5
 
+    # Force filling the tasks field in feature creation
+    strict_feature_tasks: bool = False
+
 
 class OverhaveLanguageSettings(BaseOverhavePrefix):
     """Settings for language definitions."""
 
-    step_prefixes: Optional[StepPrefixesModel]
+    step_prefixes: StepPrefixesModel | None
 
 
 class OverhaveFileSettings(BaseOverhavePrefix):
     """Settings for scenario file savings."""
 
     feature_suffix: str = ".feature"
     fixture_suffix: str = ".py"
 
     # Current workdir, used for :class:`PluginResolver` for creating of relative pytest plugins' paths
     work_dir: Path = Path.cwd()
 
     # Root project directory with features, fixtures and steps packages
-    root_dir: Optional[Path]
+    root_dir: Path | None
 
     # Base directory for feature files, by default - root_dir / 'features'
     features_dir: Path
 
     # Base directory for pytest files with template mask, by default - root_dir / 'fixtures'
     fixtures_dir: Path
     # Template mask for fixtures pytest files which contain `feature_type` key
@@ -59,25 +62,25 @@
     # Base directory for pytest-bdd steps, , by default - root_dir / 'steps'
     steps_dir: Path
 
     # Temporary directory for scenarios test runs
     tmp_dir: Path = Path("/tmp/overhave")  # noqa: S108
 
     @root_validator(pre=True)
-    def validate_dirs(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+    def validate_dirs(cls, values: dict[str, Any]) -> dict[str, Any]:
         root_dir = values.get("root_dir")
         if root_dir:
             for directory in ("features_dir", "fixtures_dir", "steps_dir"):
                 if values.get(directory):
                     continue
                 values[directory] = Path(root_dir) / directory.replace("_dir", "")
         return values
 
     @validator("steps_dir")
-    def validate_nesting(cls, v: Path, values: Dict[str, Any]) -> Path:
+    def validate_nesting(cls, v: Path, values: dict[str, Any]) -> Path:
         validate_steps_dir = values["validate_steps_dir"]
         if validate_steps_dir:
             work_dir: Path = values["work_dir"]
             v.relative_to(work_dir)
         return v
 
     @property
@@ -104,83 +107,64 @@
 
 class ProcessorSettings(BaseOverhavePrefix):
     """Settings for :class:`Processor`."""
 
     processes_num: int = 5
 
 
-class OverhaveRedisSettings(BaseOverhavePrefix):
-    """Settings for Redis entities, which use for work with different framework tasks."""
-
-    redis_url: URL = URL("redis://localhost:6379")
-    redis_db: int = 0
-    redis_block_timeout: timedelta = timedelta(seconds=1)
-    redis_read_count: int = 1
-
-    @validator("redis_url", pre=True)
-    def validate_url(cls, v: Union[str, URL]) -> URL:
-        if isinstance(v, str):
-            return URL(v)
-        return v
-
-    @property
-    def timeout_milliseconds(self) -> int:
-        return int(self.redis_block_timeout.total_seconds() * 1000)
-
-
 class OverhaveEmulationSettings(BaseOverhavePrefix):
     """Settings for Overhave Emulator, which emulates session with test user."""
 
     # Path for emulation core application, such as GoTTY
     emulation_core_path: str = "/gotty"
 
     # All emulation core application prefixes for execution
     emulation_prefix: str = "--permit-write --once --address {address} --port {port} --timeout {timeout}"
 
     # Specific terminal tool startup command with relative `feature_type`, for example: `myapp {feature_type}`
-    emulation_base_cmd: Optional[str]
+    emulation_base_cmd: str | None
     # Terminal tool command postfix with specified user `name` and `model`, for example: `--name={name} --model={model}`
     # If it is no need in use - may be optional.
-    emulation_postfix: Optional[str]
+    emulation_postfix: str | None
 
     # Optional additional terminal tool usage description
-    emulation_desc_link: Optional[str]
+    emulation_desc_link: str | None
 
     emulation_bind_ip: str = "0.0.0.0"  # noqa: S104
     # Ports for emulation binding. Expects as string with format `["port1", "port2", ...]`
-    emulation_ports: List[int] = [8080]
+    emulation_ports: list[int] = [8080]
 
     # As a real service, should be used follow path: `http://my-service.domain/mount`
     # where `emulation_service_url` = `http://my-service.domain` - URL for service,
     # and `emulation_service_mount` = `mount` - mount point for service redirection.
     # If `emulation_service_mount` is `None` - this is localhost debug.
-    emulation_service_url: URL = URL("http://localhost")
-    emulation_service_mount: Optional[str]
+    emulation_service_url: httpx.URL = httpx.URL("http://localhost")
+    emulation_service_mount: str | None
 
     # Wait until emulation become served
     emulation_wait_timeout: timedelta = timedelta(seconds=300)
 
     @validator("emulation_service_url", pre=True)
-    def validate_url(cls, v: Union[str, URL]) -> URL:
+    def validate_url(cls, v: str | httpx.URL) -> httpx.URL:
         if isinstance(v, str):
-            return URL(v)
+            return httpx.URL(v)
         return v
 
     @validator("emulation_ports", pre=True)
-    def validate_ports(cls, v: Union[List[int], str]) -> List[int]:
+    def validate_ports(cls, v: list[int] | str) -> list[int]:
         if isinstance(v, str):
             return [int(x.strip()) for x in v.split(",")]
         return v
 
-    def get_emulation_url(self, port: str) -> str:
+    def get_emulation_url(self, port: str) -> httpx.URL:
         if isinstance(self.emulation_service_mount, str):
-            return (
-                self.emulation_service_url / self.emulation_service_mount / port / ""
-            ).human_repr()  # NGINX should redirect to `service:port` by mount point and specified port
-        return self.emulation_service_url.with_port(int(port)).human_repr()  # only for local debug
+            return httpx.URL(
+                f"{self.emulation_service_url}/{self.emulation_service_mount}/{port}/"
+            )  # NGINX should redirect to `service:port` by mount point and specified port
+        return self.emulation_service_url.copy_with(port=int(port))  # only for local debug
 
     @property
     def wait_timeout_seconds(self) -> int:
         return int(self.emulation_wait_timeout.total_seconds())
 
     @property
     def enabled(self) -> bool:
```

### Comparing `overhave-3.9.0/overhave/factory/__init__.py` & `overhave-4.0.0/overhave/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/factory/base_factory.py` & `overhave-4.0.0/overhave/factory/base_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import abc
 from functools import cached_property
-from typing import Generic, Optional, Type, cast
+from typing import Generic, cast
 
 from overhave.entities import (
     ArchiveManager,
     FeatureExtractor,
     GitRepositoryInitializer,
     IFeatureExtractor,
     ReportManager,
@@ -88,18 +88,18 @@
     def system_user_storage(self) -> ISystemUserStorage:
         pass
 
 
 class BaseOverhaveFactory(IOverhaveFactory[TApplicationContext]):
     """Base factory for application entities resolution and usage."""
 
-    context_cls: Type[TApplicationContext]
+    context_cls: type[TApplicationContext]
 
     def __init__(self) -> None:
-        self._context: Optional[TApplicationContext] = None
+        self._context: TApplicationContext | None = None
 
     def set_context(self, context: TApplicationContext) -> None:
         self._context = context
 
     @property
     def context(self) -> TApplicationContext:
         if self._context is None:
@@ -207,15 +207,17 @@
 
     @property
     def scenario_storage(self) -> IScenarioStorage:
         return self._scenario_storage
 
     @cached_property
     def _step_collector(self) -> StepCollector:
-        return StepCollector(step_prefixes=self.context.language_settings.step_prefixes)
+        return StepCollector(
+            settings=self.context.step_collector_settings, step_prefixes=self.context.language_settings.step_prefixes
+        )
 
     @property
     def step_collector(self) -> StepCollector:
         return self._step_collector
 
     @cached_property
     def _test_run_storage(self) -> TestRunStorage:
```

### Comparing `overhave-3.9.0/overhave/factory/components/admin_factory.py` & `overhave-4.0.0/overhave/factory/components/admin_factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 import abc
 from functools import cached_property, partial
 from multiprocessing.pool import ThreadPool
 from typing import Callable, Mapping
 
+import walrus
+
 from overhave.base_settings import AuthorizationStrategy
 from overhave.entities import (
     DefaultAdminAuthorizationManager,
     IAdminAuthorizationManager,
     LDAPAdminAuthorizationManager,
     ReportManager,
     SimpleAdminAuthorizationManager,
 )
 from overhave.factory.base_factory import IOverhaveFactory
 from overhave.factory.components.s3_init_factory import FactoryWithS3ManagerInit
 from overhave.factory.context import OverhaveAdminContext
+from overhave.metrics import get_common_metric_container
 from overhave.storage import IFeatureTypeStorage, SystemUserGroupStorage
 from overhave.transport import (
     EmulationTask,
     LDAPAuthenticator,
     PublicationTask,
     RedisProducer,
     RedisStream,
     TestRunTask,
 )
+from overhave.transport.redis.deps import get_redis_settings, make_redis
 
 
 class IAdminFactory(IOverhaveFactory[OverhaveAdminContext]):
     """Factory interface for Overhave admin application."""
 
     @property
     @abc.abstractmethod
@@ -92,22 +96,29 @@
         return partial_auth_manager()
 
     @property
     def feature_type_storage(self) -> IFeatureTypeStorage:
         return self._feature_type_storage
 
     @cached_property
+    def _database(self) -> walrus.Database:
+        redis = make_redis(get_redis_settings())
+        return walrus.Database(connection_pool=redis.connection_pool)
+
+    @cached_property
     def _redis_producer(self) -> RedisProducer:
         return RedisProducer(
-            settings=self.context.redis_settings,
+            settings=get_redis_settings(),
             mapping={
                 TestRunTask: RedisStream.TEST,
                 PublicationTask: RedisStream.PUBLICATION,
                 EmulationTask: RedisStream.EMULATION,
             },
+            database=self._database,
+            metric_container=get_common_metric_container(),
         )
 
     @property
     def redis_producer(self) -> RedisProducer:
         return self._redis_producer
 
     @cached_property
```

### Comparing `overhave-3.9.0/overhave/factory/components/publication_factory.py` & `overhave-4.0.0/overhave/factory/components/publication_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import abc
 from functools import cached_property
 
 from overhave.factory.base_factory import BaseOverhaveFactory, IOverhaveFactory
 from overhave.factory.components.abstract_consumer import ITaskConsumerFactory
 from overhave.factory.context import OverhavePublicationContext
+from overhave.metrics import PublicationOverhaveMetricContainer
+from overhave.metrics.getters import get_publication_metric_container
 from overhave.publication import (
     GitlabVersionPublisher,
     IVersionPublisher,
     PublicationManagerType,
     StashVersionPublisher,
     TokenizerClient,
 )
@@ -85,7 +87,11 @@
     def publisher(self) -> IVersionPublisher:
         if self.context.publication_settings.publication_manager_type is PublicationManagerType.GITLAB:
             return self._gitlab_publisher
         return self._stash_publisher
 
     def process_task(self, task: PublicationTask) -> None:
         return self.publisher.process_publish_task(task)
+
+    @property
+    def metric_container(self) -> PublicationOverhaveMetricContainer:
+        return get_publication_metric_container()
```

### Comparing `overhave-3.9.0/overhave/factory/components/synchronizer_factory.py` & `overhave-4.0.0/overhave/factory/components/synchronizer_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import abc
 from functools import cached_property
 
 from overhave.factory.base_factory import BaseOverhaveFactory, IOverhaveFactory
 from overhave.factory.context import OverhaveSynchronizerContext
-from overhave.scenario import FeatureValidator
+from overhave.scenario import FeatureValidator, IFeatureValidator
 from overhave.synchronization import IOverhaveSynchronizer, OverhaveSynchronizer, SynchronizerStorageManager
 
 
 class ISynchronizerFactory(IOverhaveFactory[OverhaveSynchronizerContext]):
     """Factory interface for Overhave feature synchronizer application."""
 
     @property
     @abc.abstractmethod
     def synchronizer(self) -> IOverhaveSynchronizer:
         pass
 
     @property
     @abc.abstractmethod
-    def feature_validator(self) -> FeatureValidator:
+    def feature_validator(self) -> IFeatureValidator:
         pass
 
 
 class SynchronizerFactory(BaseOverhaveFactory[OverhaveSynchronizerContext], ISynchronizerFactory):
     """Factory for Overhave feature synchronization application."""
 
     context_cls = OverhaveSynchronizerContext
@@ -52,9 +52,9 @@
         return FeatureValidator(
             file_settings=self.context.file_settings,
             scenario_parser=self._scenario_parser,
             git_initializer=self._git_initializer,
         )
 
     @property
-    def feature_validator(self) -> FeatureValidator:
+    def feature_validator(self) -> IFeatureValidator:
         return self._feature_validator
```

### Comparing `overhave-3.9.0/overhave/factory/components/test_execution_factory.py` & `overhave-4.0.0/overhave/factory/components/test_execution_factory.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import abc
 from functools import cached_property
 
 from overhave.factory.base_factory import IOverhaveFactory
 from overhave.factory.components.abstract_consumer import ITaskConsumerFactory
 from overhave.factory.components.s3_init_factory import FactoryWithS3ManagerInit
 from overhave.factory.context import OverhaveTestExecutionContext
+from overhave.metrics import TestRunOverhaveMetricContainer, get_test_metric_container
 from overhave.test_execution.executor import ITestExecutor, TestExecutor
 from overhave.transport import TestRunTask
 
 
 class ITestExecutionFactory(IOverhaveFactory[OverhaveTestExecutionContext], ITaskConsumerFactory[TestRunTask], abc.ABC):
     """Abstract factory for Overhave test execution application."""
 
@@ -29,15 +30,20 @@
             file_settings=self.context.file_settings,
             feature_storage=self._feature_storage,
             scenario_storage=self._scenario_storage,
             test_run_storage=self._test_run_storage,
             file_manager=self._file_manager,
             test_runner=self._test_runner,
             report_manager=self._report_manager,
+            metric_container=self._metric_container,
         )
 
     @property
     def test_executor(self) -> ITestExecutor:
         return self._test_executor
 
     def process_task(self, task: TestRunTask) -> None:
         return self._test_executor.process_test_task(task)
+
+    @property
+    def _metric_container(self) -> TestRunOverhaveMetricContainer:
+        return get_test_metric_container()
```

### Comparing `overhave-3.9.0/overhave/factory/consumer_factory.py` & `overhave-4.0.0/overhave/factory/consumer_factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 from functools import cached_property, partial
-from typing import Callable, Dict, Type
+from typing import Callable
+
+import walrus
 
 from overhave.factory.getters import get_emulation_factory, get_publication_factory, get_test_execution_factory
+from overhave.metrics import get_common_metric_container
 from overhave.pytest_plugin import get_proxy_manager
 from overhave.transport import (
     AnyRedisTask,
     EmulationTask,
     PublicationTask,
     RedisConsumer,
     RedisConsumerRunner,
     RedisStream,
     TestRunTask,
 )
+from overhave.transport.redis.deps import get_redis_settings, make_redis
 
 
 class ConsumerFactory:
     """Factory for :class:`RedisConsumer`, :class:`RedisConsumerRunner` and tasks mapping."""
 
     def __init__(self, stream: RedisStream):
         self._stream = stream
 
     @cached_property
-    def _consumer(self) -> RedisConsumer:
-        from overhave.entities import OverhaveRedisSettings
+    def _database(self) -> walrus.Database:
+        redis = make_redis(get_redis_settings())
+        return walrus.Database(connection_pool=redis.connection_pool)
 
-        return RedisConsumer(settings=OverhaveRedisSettings(), stream_name=self._stream)
+    @cached_property
+    def _consumer(self) -> RedisConsumer:
+        return RedisConsumer(
+            settings=get_redis_settings(),
+            stream_name=self._stream,
+            database=self._database,
+            metric_container=get_common_metric_container(),
+        )
 
     @cached_property
     def runner(self) -> RedisConsumerRunner:
         return RedisConsumerRunner(consumer=self._consumer, mapping=self._mapping)
 
     @cached_property
-    def _mapping(self) -> Dict[Type[AnyRedisTask], Callable[[AnyRedisTask], None]]:
+    def _mapping(self) -> dict[type[AnyRedisTask], Callable[[AnyRedisTask], None]]:
         return {
             TestRunTask: self._process_test_execution_task,  # type: ignore
             PublicationTask: get_publication_factory().process_task,  # type: ignore
             EmulationTask: get_emulation_factory().process_task,  # type: ignore
         }
 
     @cached_property
```

### Comparing `overhave-3.9.0/overhave/factory/context/__init__.py` & `overhave-4.0.0/overhave/factory/context/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/factory/context/admin_context.py` & `overhave-4.0.0/overhave/factory/context/admin_context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,53 @@
-from typing import Optional
-
 from overhave.base_settings import AuthorizationStrategy, OverhaveAuthorizationSettings
 from overhave.entities import (
     OverhaveAdminSettings,
     OverhaveEmulationSettings,
     OverhaveFileSettings,
     OverhaveLanguageSettings,
     OverhaveLdapManagerSettings,
-    OverhaveRedisSettings,
     OverhaveReportManagerSettings,
 )
 from overhave.factory.context.base_context import BaseFactoryContext
 from overhave.scenario import OverhaveProjectSettings, OverhaveScenarioCompilerSettings
-from overhave.test_execution import OverhaveTestSettings
+from overhave.test_execution import OverhaveStepCollectorSettings, OverhaveTestSettings
 from overhave.transport import OverhaveLdapClientSettings, OverhaveS3ManagerSettings
 
 
 class OverhaveAdminContext(BaseFactoryContext):
     """Overhave admin context, based on application BaseSettings.
 
     This context defines how Overhave admin will work.
     """
 
     def __init__(
         self,
-        admin_settings: Optional[OverhaveAdminSettings] = None,
-        auth_settings: Optional[OverhaveAuthorizationSettings] = None,
-        emulation_settings: Optional[OverhaveEmulationSettings] = None,
-        file_settings: Optional[OverhaveFileSettings] = None,
-        language_settings: Optional[OverhaveLanguageSettings] = None,
-        ldap_manager_settings: Optional[OverhaveLdapManagerSettings] = None,
-        ldap_client_settings: Optional[OverhaveLdapClientSettings] = None,
-        redis_settings: Optional[OverhaveRedisSettings] = None,
-        project_settings: Optional[OverhaveProjectSettings] = None,
-        compilation_settings: Optional[OverhaveScenarioCompilerSettings] = None,
-        report_manager_settings: Optional[OverhaveReportManagerSettings] = None,
-        s3_manager_settings: Optional[OverhaveS3ManagerSettings] = None,
-        test_settings: Optional[OverhaveTestSettings] = None,
+        admin_settings: OverhaveAdminSettings | None = None,
+        auth_settings: OverhaveAuthorizationSettings | None = None,
+        emulation_settings: OverhaveEmulationSettings | None = None,
+        file_settings: OverhaveFileSettings | None = None,
+        language_settings: OverhaveLanguageSettings | None = None,
+        ldap_manager_settings: OverhaveLdapManagerSettings | None = None,
+        ldap_client_settings: OverhaveLdapClientSettings | None = None,
+        project_settings: OverhaveProjectSettings | None = None,
+        compilation_settings: OverhaveScenarioCompilerSettings | None = None,
+        report_manager_settings: OverhaveReportManagerSettings | None = None,
+        s3_manager_settings: OverhaveS3ManagerSettings | None = None,
+        test_settings: OverhaveTestSettings | None = None,
+        step_collector_settings: OverhaveStepCollectorSettings | None = None,
     ) -> None:
         super().__init__(
             emulation_settings=emulation_settings or OverhaveEmulationSettings(),
             file_settings=file_settings or OverhaveFileSettings(),
             language_settings=language_settings or OverhaveLanguageSettings(),
             project_settings=project_settings or OverhaveProjectSettings(),
             compilation_settings=compilation_settings or OverhaveScenarioCompilerSettings(),
             report_manager_settings=report_manager_settings or OverhaveReportManagerSettings(),
             s3_manager_settings=s3_manager_settings or OverhaveS3ManagerSettings(),
             test_settings=test_settings or OverhaveTestSettings(),
+            step_collector_settings=step_collector_settings or OverhaveStepCollectorSettings(),
         )
         self.admin_settings = admin_settings or OverhaveAdminSettings()
         self.auth_settings = auth_settings or OverhaveAuthorizationSettings()
-        self.redis_settings = redis_settings or OverhaveRedisSettings()
-
         if self.auth_settings.auth_strategy is AuthorizationStrategy.LDAP:
             self.ldap_manager_settings = ldap_manager_settings or OverhaveLdapManagerSettings()
             self.ldap_client_settings = ldap_client_settings or OverhaveLdapClientSettings()
```

### Comparing `overhave-3.9.0/overhave/factory/context/base_context.py` & `overhave-4.0.0/overhave/factory/context/base_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Optional, cast
+from typing import cast
 
 from pydantic import BaseSettings
 
 from overhave.entities import (
     OverhaveEmulationSettings,
     OverhaveFileSettings,
     OverhaveLanguageSettings,
     OverhaveReportManagerSettings,
 )
 from overhave.scenario import OverhaveProjectSettings, OverhaveScenarioCompilerSettings, OverhaveScenarioParserSettings
-from overhave.test_execution import OverhaveTestSettings
+from overhave.test_execution import OverhaveStepCollectorSettings, OverhaveTestSettings
 from overhave.transport import OverhaveS3ManagerSettings
 
 
 class BaseFactoryContextException(Exception):
     """Base exception for :class:`BaseFactoryContext`."""
 
 
@@ -22,36 +22,38 @@
 
 
 class BaseFactoryContext:
     """Base class for factory context."""
 
     def __init__(
         self,
-        compilation_settings: Optional[OverhaveScenarioCompilerSettings] = None,
-        parser_settings: Optional[OverhaveScenarioParserSettings] = None,
-        emulation_settings: Optional[OverhaveEmulationSettings] = None,
-        file_settings: Optional[OverhaveFileSettings] = None,
-        language_settings: Optional[OverhaveLanguageSettings] = None,
-        project_settings: Optional[OverhaveProjectSettings] = None,
-        report_manager_settings: Optional[OverhaveReportManagerSettings] = None,
-        s3_manager_settings: Optional[OverhaveS3ManagerSettings] = None,
-        test_settings: Optional[OverhaveTestSettings] = None,
+        compilation_settings: OverhaveScenarioCompilerSettings | None = None,
+        parser_settings: OverhaveScenarioParserSettings | None = None,
+        emulation_settings: OverhaveEmulationSettings | None = None,
+        file_settings: OverhaveFileSettings | None = None,
+        language_settings: OverhaveLanguageSettings | None = None,
+        project_settings: OverhaveProjectSettings | None = None,
+        report_manager_settings: OverhaveReportManagerSettings | None = None,
+        s3_manager_settings: OverhaveS3ManagerSettings | None = None,
+        test_settings: OverhaveTestSettings | None = None,
+        step_collector_settings: OverhaveStepCollectorSettings | None = None,
     ):
         self._compilation_settings = compilation_settings
         self._parser_settings = parser_settings
         self._emulation_settings = emulation_settings
         self._file_settings = file_settings
         self._language_settings = language_settings
         self._project_settings = project_settings
         self._report_manager_settings = report_manager_settings
         self._s3_manager_settings = s3_manager_settings
         self._test_settings = test_settings
+        self._step_collector_settings = step_collector_settings
 
     @staticmethod
-    def _ensured_settings(settings: Optional[BaseSettings]) -> BaseSettings:
+    def _ensured_settings(settings: BaseSettings | None) -> BaseSettings:
         if settings is None:
             raise NotDefinedSettingsError(type(settings).__name__)
         return settings
 
     @property
     def compilation_settings(self) -> OverhaveScenarioCompilerSettings:
         return cast(OverhaveScenarioCompilerSettings, self._ensured_settings(self._compilation_settings))
@@ -83,7 +85,11 @@
     @property
     def s3_manager_settings(self) -> OverhaveS3ManagerSettings:
         return cast(OverhaveS3ManagerSettings, self._ensured_settings(self._s3_manager_settings))
 
     @property
     def test_settings(self) -> OverhaveTestSettings:
         return cast(OverhaveTestSettings, self._ensured_settings(self._test_settings))
+
+    @property
+    def step_collector_settings(self) -> OverhaveStepCollectorSettings:
+        return cast(OverhaveStepCollectorSettings, self._ensured_settings(self._step_collector_settings))
```

### Comparing `overhave-3.9.0/overhave/factory/context/publication_context.py` & `overhave-4.0.0/overhave/factory/context/publication_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from overhave.entities import OverhaveFileSettings, OverhaveLanguageSettings
 from overhave.factory.context.base_context import BaseFactoryContext
 from overhave.publication.gitlab import OverhaveGitlabPublisherSettings, TokenizerClientSettings
 from overhave.publication.settings import BaseGitPublisherSettings, PublicationSettings
 from overhave.scenario import OverhaveProjectSettings, OverhaveScenarioCompilerSettings
 from overhave.transport import OverhaveGitlabClientSettings
 from overhave.transport.http.base_client.settings import HttpSettingsType
@@ -13,22 +11,22 @@
     """Overhave publication context, based on application BaseSettings.
 
     This context defines how Overhave publication will work.
     """
 
     def __init__(
         self,
-        compilation_settings: Optional[OverhaveScenarioCompilerSettings] = None,
-        file_settings: Optional[OverhaveFileSettings] = None,
-        language_settings: Optional[OverhaveLanguageSettings] = None,
-        project_settings: Optional[OverhaveProjectSettings] = None,
-        client_settings: Optional[HttpSettingsType] = None,
-        publisher_settings: Optional[BaseGitPublisherSettings] = None,
-        publication_settings: Optional[PublicationSettings] = None,
-        tokenizer_client_settings: Optional[TokenizerClientSettings] = None,
+        compilation_settings: OverhaveScenarioCompilerSettings | None = None,
+        file_settings: OverhaveFileSettings | None = None,
+        language_settings: OverhaveLanguageSettings | None = None,
+        project_settings: OverhaveProjectSettings | None = None,
+        client_settings: HttpSettingsType | None = None,
+        publisher_settings: BaseGitPublisherSettings | None = None,
+        publication_settings: PublicationSettings | None = None,
+        tokenizer_client_settings: TokenizerClientSettings | None = None,
     ) -> None:
         super().__init__(
             compilation_settings=compilation_settings or OverhaveScenarioCompilerSettings(),
             file_settings=file_settings or OverhaveFileSettings(),
             language_settings=language_settings or OverhaveLanguageSettings(),
             project_settings=project_settings or OverhaveProjectSettings(),
         )
```

### Comparing `overhave-3.9.0/overhave/factory/context/test_execution_context.py` & `overhave-4.0.0/overhave/factory/context/test_execution_context.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from overhave.entities import (
     OverhaveDescriptionManagerSettings,
     OverhaveFileSettings,
     OverhaveLanguageSettings,
     OverhaveReportManagerSettings,
     OverhaveStepContextSettings,
 )
@@ -17,25 +15,25 @@
     """Overhave test run context, based on application BaseSettings.
 
     This context defines how Overhave test run will work.
     """
 
     def __init__(
         self,
-        compilation_settings: Optional[OverhaveScenarioCompilerSettings] = None,
-        parser_settings: Optional[OverhaveScenarioParserSettings] = None,
-        description_manager_settings: Optional[OverhaveDescriptionManagerSettings] = None,
-        file_settings: Optional[OverhaveFileSettings] = None,
-        language_settings: Optional[OverhaveLanguageSettings] = None,
-        project_settings: Optional[OverhaveProjectSettings] = None,
-        report_manager_settings: Optional[OverhaveReportManagerSettings] = None,
-        s3_manager_settings: Optional[OverhaveS3ManagerSettings] = None,
-        step_context_settings: Optional[OverhaveStepContextSettings] = None,
-        test_settings: Optional[OverhaveTestSettings] = None,
-        admin_link_settings: Optional[OverhaveAdminLinkSettings] = None,
+        compilation_settings: OverhaveScenarioCompilerSettings | None = None,
+        parser_settings: OverhaveScenarioParserSettings | None = None,
+        description_manager_settings: OverhaveDescriptionManagerSettings | None = None,
+        file_settings: OverhaveFileSettings | None = None,
+        language_settings: OverhaveLanguageSettings | None = None,
+        project_settings: OverhaveProjectSettings | None = None,
+        report_manager_settings: OverhaveReportManagerSettings | None = None,
+        s3_manager_settings: OverhaveS3ManagerSettings | None = None,
+        step_context_settings: OverhaveStepContextSettings | None = None,
+        test_settings: OverhaveTestSettings | None = None,
+        admin_link_settings: OverhaveAdminLinkSettings | None = None,
     ) -> None:
         super().__init__(
             compilation_settings=compilation_settings or OverhaveScenarioCompilerSettings(),
             parser_settings=parser_settings or OverhaveScenarioParserSettings(),
             file_settings=file_settings or OverhaveFileSettings(),
             language_settings=language_settings or OverhaveLanguageSettings(),
             project_settings=project_settings or OverhaveProjectSettings(),
```

### Comparing `overhave-3.9.0/overhave/factory/getters.py` & `overhave-4.0.0/overhave/factory/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/publication/git_publisher.py` & `overhave-4.0.0/overhave/publication/git_publisher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,57 @@
 import abc
 import logging
-from typing import Generic, Optional, cast
+from typing import Generic, cast
 
 import git
 
-from overhave.entities import GitPullError, GitRepositoryInitializer, OverhaveFileSettings
-from overhave.publication.base_publisher import BaseVersionPublisher, BaseVersionPublisherException
+from overhave.entities import GitRepositoryInitializer, OverhaveFileSettings
+from overhave.metrics import PublicationOverhaveMetricContainer
+from overhave.publication.base_publisher import BaseVersionPublisher
+from overhave.publication.errors import (
+    BaseGitVersionPublisherError,
+    CommitNotCreatedError,
+    CurrentBranchEqualToDefaultError,
+    CurrentBranchNotEqualToTargetError,
+)
 from overhave.publication.settings import GitPublisherSettings
 from overhave.scenario import FileManager, OverhaveProjectSettings
 from overhave.storage import IDraftStorage, IFeatureStorage, IScenarioStorage, ITestRunStorage, PublisherContext
 
 logger = logging.getLogger(__name__)
 
 
-class BaseGitVersionPublisherError(BaseVersionPublisherException):
-    """Base exception for git version publisher."""
-
-
-class CurrentBranchEqualToDefaultError(BaseGitVersionPublisherError):
-    """Exception for situation when current branch is equal to default branch."""
-
-
-class CurrentBranchNotEqualToTargetError(BaseGitVersionPublisherError):
-    """Exception for situation when current branch is not equal to target branch."""
-
-
-class CommitNotCreatedError(BaseGitVersionPublisherError):
-    """Exception for situation with not created commit."""
-
-
 class GitVersionPublisher(Generic[GitPublisherSettings], BaseVersionPublisher, abc.ABC):
     """Class for feature version's management, based on git."""
 
     def __init__(
         self,
         file_settings: OverhaveFileSettings,
         project_settings: OverhaveProjectSettings,
         feature_storage: IFeatureStorage,
         scenario_storage: IScenarioStorage,
         test_run_storage: ITestRunStorage,
         draft_storage: IDraftStorage,
         file_manager: FileManager,
         git_initializer: GitRepositoryInitializer,
+        git_publisher_settings: GitPublisherSettings,
+        metric_container: PublicationOverhaveMetricContainer,
     ) -> None:
         super().__init__(
             file_settings=file_settings,
             project_settings=project_settings,
             feature_storage=feature_storage,
             scenario_storage=scenario_storage,
             test_run_storage=test_run_storage,
             draft_storage=draft_storage,
             file_manager=file_manager,
+            metric_container=metric_container,
         )
         self._git_initializer = git_initializer
+        self._git_publisher_settings = git_publisher_settings
 
     def _create_head(self, name: str) -> git.SymbolicReference:
         repo = self._git_initializer.repository
         if name in repo.heads:
             repo.delete_head(repo.heads[name], force=True)
             logger.warning("Trashed existed branch with name '%s'", name)
 
@@ -107,19 +102,14 @@
             logger.info("Current branch is '%s'", repo.active_branch)
             original_branch.checkout()
             logger.info("Branch returned to '%s'", repo.active_branch)
 
         if not changes_pushed:
             raise CommitNotCreatedError("Commit has not been created!")
 
-    def _push_version(self, draft_id: int) -> Optional[PublisherContext]:
-        try:
+    def _prepare_repo(self, context: PublisherContext) -> None:
+        if not self._git_publisher_settings.pull_before_creating_mr_enabled:
+            logger.warning("Pulling before creating merge request is disabled!")
+        else:
             self._git_initializer.pull()
-            ctx = self._compile_context(draft_id)
-            git_branch = cast(git.Head, self._create_head(name=ctx.target_branch))
-            self._create_commit_and_push(context=ctx, target_branch=git_branch)
-            return ctx
-        except GitPullError:
-            logger.exception("Error while trying to pull remote repository!")
-        except (git.GitCommandError, BaseGitVersionPublisherError):
-            logger.exception("Error while trying to push scenario version!")
-        return None
+        git_branch = cast(git.Head, self._create_head(name=context.target_branch))
+        self._create_commit_and_push(context=context, target_branch=git_branch)
```

### Comparing `overhave-3.9.0/overhave/publication/gitlab/gitlab_publisher.py` & `overhave-4.0.0/overhave/publication/stash/stash_publisher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,96 @@
 import logging
-from http import HTTPStatus
 
-from gitlab import GitlabCreateError, GitlabHttpError
-from gitlab.v4.objects.merge_requests import ProjectMergeRequest
-from requests import HTTPError
+import httpx
 
-from overhave.db import DraftStatus
+from overhave import db
 from overhave.entities import GitRepositoryInitializer, OverhaveFileSettings
+from overhave.metrics import PublicationOverhaveMetricContainer
 from overhave.publication.git_publisher import GitVersionPublisher
-from overhave.publication.gitlab.settings import OverhaveGitlabPublisherSettings
-from overhave.publication.gitlab.tokenizer.client import TokenizerClient
+from overhave.publication.stash.settings import OverhaveStashPublisherSettings
 from overhave.scenario import FileManager, OverhaveProjectSettings
-from overhave.storage import IDraftStorage, IFeatureStorage, IScenarioStorage, ITestRunStorage, PublisherContext
-from overhave.transport.http.gitlab_client import GitlabHttpClient, GitlabMrRequest
+from overhave.storage import IDraftStorage, IFeatureStorage, IScenarioStorage, ITestRunStorage
+from overhave.transport import (
+    StashBranch,
+    StashErrorResponse,
+    StashHttpClient,
+    StashHttpClientConflictError,
+    StashPrCreationResponse,
+    StashPrRequest,
+)
 
 logger = logging.getLogger(__name__)
 
 
-class BaseGitlabVersionPublisherException(Exception):
-    """Base exception for :class:`GitlabVersionPublisher`."""
-
-
-class InvalidWebUrlException(BaseGitlabVersionPublisherException):
-    """Exception for case when web url is None."""
-
-
-class GitlabVersionPublisher(GitVersionPublisher[OverhaveGitlabPublisherSettings]):
-    """Class for feature version's merge requests management relative to Gitlab API."""
+class StashVersionPublisher(GitVersionPublisher[OverhaveStashPublisherSettings]):
+    """Class for feature version's pull requests management relative to Atlassian Stash API."""
 
     def __init__(
         self,
         file_settings: OverhaveFileSettings,
         project_settings: OverhaveProjectSettings,
         feature_storage: IFeatureStorage,
         scenario_storage: IScenarioStorage,
         test_run_storage: ITestRunStorage,
         draft_storage: IDraftStorage,
         file_manager: FileManager,
         git_initializer: GitRepositoryInitializer,
-        gitlab_publisher_settings: OverhaveGitlabPublisherSettings,
-        gitlab_client: GitlabHttpClient,
-        tokenizer_client: TokenizerClient,
+        stash_publisher_settings: OverhaveStashPublisherSettings,
+        stash_client: StashHttpClient,
+        metric_container: PublicationOverhaveMetricContainer,
     ):
         super().__init__(
             file_settings=file_settings,
             project_settings=project_settings,
             feature_storage=feature_storage,
             scenario_storage=scenario_storage,
             test_run_storage=test_run_storage,
             draft_storage=draft_storage,
             file_manager=file_manager,
             git_initializer=git_initializer,
+            git_publisher_settings=stash_publisher_settings,
+            metric_container=metric_container,
         )
-        self._gitlab_publisher_settings = gitlab_publisher_settings
-        self._gitlab_client = gitlab_client
-        self._tokenizer_client = tokenizer_client
-
-    def publish_version(self, draft_id: int) -> None:
-        logger.info("Start processing draft_id=%s...", draft_id)
-        self._draft_storage.set_draft_status(draft_id, DraftStatus.CREATING)
-        context = self._push_version(draft_id)
-        if not isinstance(context, PublisherContext):
-            return
-        merge_request = GitlabMrRequest(
-            project_id=self._gitlab_publisher_settings.repository_id,
+        self._client = stash_client
+
+    def publish_version(self, draft_id: int) -> db.DraftStatus:
+        context = self._prepare_publisher_context(draft_id)
+        if context is None:
+            self._draft_storage.set_draft_status(draft_id=draft_id, status=db.DraftStatus.INTERNAL_ERROR)
+            return db.DraftStatus.INTERNAL_ERROR
+        pull_request = StashPrRequest(
             title=context.feature.name,
-            source_branch=context.target_branch,
-            target_branch=self._gitlab_publisher_settings.target_branch,
             description=self._compile_publication_description(context),
-            reviewer_ids=self._gitlab_publisher_settings.get_reviewers(feature_type=context.feature.feature_type.name),
+            open=True,
+            fromRef=StashBranch(id=context.target_branch, repository=self._git_publisher_settings.repository),
+            toRef=self._git_publisher_settings.target_branch,
+            reviewers=self._git_publisher_settings.get_reviewers(feature_type=context.feature.feature_type.name),
         )
-        logger.info("Prepared merge-request: %s", merge_request.json(by_alias=True))
+        logger.info("Prepared pull-request: %s", pull_request.json(by_alias=True))
         try:
-            token = (
-                self._gitlab_client._settings.auth_token or self._tokenizer_client.get_token(draft_id=draft_id).token
-            )
-            response = self._gitlab_client.send_merge_request(
-                merge_request=merge_request, token=token, repository_id=self._gitlab_publisher_settings.repository_id
-            )
-            if isinstance(response, ProjectMergeRequest):
-                if response.web_url is None:
-                    raise InvalidWebUrlException("Please verify your gitlab url environment! It is invalid!")
-                self._draft_storage.save_response(
+            response = self._client.send_pull_request(pull_request)
+            if isinstance(response, StashPrCreationResponse):
+                self._draft_storage.save_response_as_created(
                     draft_id=draft_id,
-                    pr_url=response.web_url,
-                    published_at=response.created_at,
-                    status=DraftStatus.CREATED,
+                    pr_url=response.get_pr_url(),
+                    published_at=response.created_date,
                 )
-                return
-        except (GitlabCreateError, GitlabHttpError) as e:
-            if e.response_code == HTTPStatus.CONFLICT:
-                context.draft.traceback = str(e)
-                logger.exception("Gotten conflict. Try to return last merge-request for Draft with id=%s...", draft_id)
-                self._save_as_duplicate(context)
-                return
-            self._draft_storage.set_draft_status(draft_id, DraftStatus.INTERNAL_ERROR, traceback=str(e))
-        except HTTPError as e:
-            self._draft_storage.set_draft_status(draft_id, DraftStatus.INTERNAL_ERROR, traceback=str(e))
-            logger.exception("Got HTTP error while trying to sent merge-request!")
+                return db.DraftStatus.CREATED
+            if isinstance(response, StashErrorResponse) and response.duplicate:
+                self._draft_storage.save_response_as_duplicate(
+                    draft_id=context.draft.id, feature_id=context.feature.id, traceback=None
+                )
+                return db.DraftStatus.DUPLICATE
+            self._draft_storage.set_draft_status(draft_id, db.DraftStatus.INTERNAL_ERROR)
+            logger.error("Gotten error response from Stash: %s", response)
+            return db.DraftStatus.INTERNAL_ERROR
+
+        except StashHttpClientConflictError as err:
+            logger.exception("Gotten conflict. Try to return last pull-request for Draft with id=%s...", draft_id)
+            self._draft_storage.save_response_as_duplicate(
+                draft_id=context.draft.id, feature_id=context.feature.id, traceback=str(err)
+            )
+            return db.DraftStatus.DUPLICATE
+        except httpx.HTTPError as err:
+            self._draft_storage.set_draft_status(draft_id, db.DraftStatus.INTERNAL_ERROR, str(err))
+            logger.exception("Got HTTP error while trying to sent pull-request!")
+            return db.DraftStatus.INTERNAL_ERROR
```

### Comparing `overhave-3.9.0/overhave/publication/gitlab/settings.py` & `overhave-4.0.0/overhave/publication/gitlab/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List, Optional
-
 from overhave.publication.settings import BaseGitPublisherSettings
 from overhave.storage import FeatureTypeName
 from overhave.transport.http.gitlab_client import GitlabRepository
 
 
 class NotSpecifiedFeatureTypeError(RuntimeError):
     """Exception for not specified reviewers relative to feature type."""
@@ -25,16 +23,16 @@
     def repository(self) -> GitlabRepository:
         return GitlabRepository(project_id=self.repository_id)
 
     @property
     def target_branch(self) -> str:
         return self.default_target_branch_name
 
-    def get_reviewers(self, feature_type: FeatureTypeName) -> List[str]:
+    def get_reviewers(self, feature_type: FeatureTypeName) -> list[str]:
         if self.feature_type_to_reviewers_mapping:
-            reviewers: Optional[List[str]] = self.feature_type_to_reviewers_mapping.get(feature_type)
+            reviewers: list[str] | None = self.feature_type_to_reviewers_mapping.get(feature_type)
             if not reviewers:
                 raise NotSpecifiedFeatureTypeError(
                     f"'{feature_type}' reviewers are not specified in 'feature_type_to_reviewers_mapping' dict!"
                 )
             return reviewers
         return self.default_reviewers
```

### Comparing `overhave-3.9.0/overhave/publication/gitlab/tokenizer/client.py` & `overhave-4.0.0/overhave/publication/gitlab/tokenizer/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from typing import Dict, Union, cast
+import logging
+from typing import cast
 
 from pydantic.main import BaseModel
 
 from overhave.publication.gitlab.tokenizer.settings import TokenizerClientSettings
 from overhave.transport.http import BaseHttpClient
 from overhave.transport.http.base_client import HttpMethod
 
+logger = logging.getLogger(__name__)
+
 
 class TokenizerResponse(BaseModel):
     """Response from service tokenizer with token."""
 
     token: str
 
 
 class TokenizerRequestParamsModel(BaseModel):
     """Request for service tokenizer."""
 
     initiator: str
     id: int
     remote_key: str
 
-    def get_request_params(self, remote_key_name: str) -> Dict[str, Union[int, str]]:
+    def get_request_params(self, remote_key_name: str) -> dict[str, int | str]:
         return {"initiator": self.initiator, "id": self.id, remote_key_name: self.remote_key}
 
 
 class BaseTokenizerException(Exception):
     """Base tokenizer exception."""
 
 
@@ -52,8 +55,9 @@
         if self._settings.remote_key_name is None:
             raise InvalidRemoteKeyNameException("Please check remote key name! Value is invalid!")
         response = self._make_request(
             HttpMethod.POST,
             self._settings.url,
             params=params_model.get_request_params(self._settings.remote_key_name),
         )
+        logger.debug("Response with token: %s", response)
         return cast(TokenizerResponse, self._parse_or_raise(response, TokenizerResponse))
```

### Comparing `overhave-3.9.0/overhave/publication/settings.py` & `overhave-4.0.0/overhave/publication/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import List, Mapping, TypeVar
+from typing import Mapping, TypeVar
 
 from overhave.base_settings import BaseOverhavePrefix
 from overhave.publication.objects import PublicationManagerType
 from overhave.storage import FeatureTypeName
 
 
 class BaseGitPublisherSettings(BaseOverhavePrefix):
     """Base git publisher settings."""
 
-    default_reviewers: List[str] = []
-    feature_type_to_reviewers_mapping: Mapping[FeatureTypeName, List[str]] = {}
+    default_reviewers: list[str] = []
+    feature_type_to_reviewers_mapping: Mapping[FeatureTypeName, list[str]] = {}
     default_target_branch_name: str = "master"
+    pull_before_creating_mr_enabled: bool = True
 
 
 class PublicationSettings(BaseOverhavePrefix):
     """Publication settings where you can specify publication manager and its behavior."""
 
     # Choose gitlab or stash as a publication manager
     publication_manager_type: PublicationManagerType = PublicationManagerType.GITLAB
```

### Comparing `overhave-3.9.0/overhave/publication/stash/settings.py` & `overhave-4.0.0/overhave/publication/stash/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import List
-
 from overhave.publication.settings import BaseGitPublisherSettings
 from overhave.storage import FeatureTypeName
 from overhave.transport import StashBranch, StashProject, StashRepository, StashReviewer, StashReviewerInfo
 
 
 class NotSpecifiedFeatureTypeError(RuntimeError):
     """Exception for not specified reviewers relative to feature type."""
@@ -26,15 +24,15 @@
     def repository(self) -> StashRepository:
         return StashRepository(slug=self.repository_name, project=StashProject(key=self.project_key))
 
     @property
     def target_branch(self) -> StashBranch:
         return StashBranch(id=self.default_target_branch_name, repository=self.repository)
 
-    def get_reviewers(self, feature_type: FeatureTypeName) -> List[StashReviewer]:
+    def get_reviewers(self, feature_type: FeatureTypeName) -> list[StashReviewer]:
         if self.feature_type_to_reviewers_mapping:
             reviewers = self.feature_type_to_reviewers_mapping.get(feature_type)
             if not reviewers:
                 raise NotSpecifiedFeatureTypeError(
                     f"'{feature_type}' reviewers are not specified in 'feature_type_to_reviewers_mapping' dict!"
                 )
         else:
```

### Comparing `overhave-3.9.0/overhave/publication/stash/stash_publisher.py` & `overhave-4.0.0/overhave/publication/base_publisher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,89 @@
+import abc
 import logging
 
-from requests import HTTPError
+import git
 
-from overhave.db import DraftStatus
-from overhave.entities import GitRepositoryInitializer, OverhaveFileSettings
-from overhave.publication.git_publisher import GitVersionPublisher
-from overhave.publication.stash.settings import OverhaveStashPublisherSettings
-from overhave.scenario import FileManager, OverhaveProjectSettings
+from overhave import db
+from overhave.entities import GitPullError, OverhaveFileSettings
+from overhave.metrics import PublicationOverhaveMetricContainer
+from overhave.publication.abstract_publisher import IVersionPublisher
+from overhave.publication.errors import BaseGitVersionPublisherError
+from overhave.scenario import FileManager, OverhaveProjectSettings, generate_task_info
 from overhave.storage import IDraftStorage, IFeatureStorage, IScenarioStorage, ITestRunStorage, PublisherContext
-from overhave.transport import (
-    StashBranch,
-    StashErrorResponse,
-    StashHttpClient,
-    StashHttpClientConflictError,
-    StashPrCreationResponse,
-    StashPrRequest,
-)
+from overhave.transport import PublicationTask
 
 logger = logging.getLogger(__name__)
 
 
-class StashVersionPublisher(GitVersionPublisher[OverhaveStashPublisherSettings]):
+class BaseVersionPublisher(IVersionPublisher, abc.ABC):
     """Class for feature version's pull requests management relative to Atlassian Stash API."""
 
     def __init__(
         self,
         file_settings: OverhaveFileSettings,
         project_settings: OverhaveProjectSettings,
         feature_storage: IFeatureStorage,
         scenario_storage: IScenarioStorage,
         test_run_storage: ITestRunStorage,
         draft_storage: IDraftStorage,
         file_manager: FileManager,
-        git_initializer: GitRepositoryInitializer,
-        stash_publisher_settings: OverhaveStashPublisherSettings,
-        stash_client: StashHttpClient,
-    ):
-        super().__init__(
-            file_settings=file_settings,
-            project_settings=project_settings,
-            feature_storage=feature_storage,
-            scenario_storage=scenario_storage,
-            test_run_storage=test_run_storage,
-            draft_storage=draft_storage,
-            file_manager=file_manager,
-            git_initializer=git_initializer,
+        metric_container: PublicationOverhaveMetricContainer,
+    ) -> None:
+        self._file_settings = file_settings
+        self._project_settings = project_settings
+        self._feature_storage = feature_storage
+        self._scenario_storage = scenario_storage
+        self._test_run_storage = test_run_storage
+        self._draft_storage = draft_storage
+        self._file_manager = file_manager
+        self._metric_container = metric_container
+
+    def process_publish_task(self, task: PublicationTask) -> None:
+        status = self.publish_version(task.data.draft_id)
+        self._metric_container.add_publication_task_status(status=status.value)
+
+    def _compile_context(self, draft_id: int) -> PublisherContext:
+        with db.create_session() as session:
+            draft_model = self._draft_storage.draft_model_by_id(session=session, draft_id=draft_id)
+            test_run_model = self._test_run_storage.testrun_model_by_id(session=session, run_id=draft_model.test_run_id)
+            feature_model = self._feature_storage.feature_model_by_id(
+                session=session, feature_id=draft_model.feature_id
+            )
+            scenario_model = self._scenario_storage.scenario_model_by_id(
+                session=session, scenario_id=test_run_model.scenario_id
+            )
+        return PublisherContext(
+            feature=feature_model,
+            scenario=scenario_model,
+            test_run=test_run_model,
+            draft=draft_model,
+            target_branch=f"bdd-feature-{feature_model.id}",
         )
-        self._stash_publisher_settings = stash_publisher_settings
-        self._client = stash_client
 
-    def publish_version(self, draft_id: int) -> None:
-        logger.info("Start processing draft_id=%s...", draft_id)
-        self._draft_storage.set_draft_status(draft_id, DraftStatus.CREATING)
-        context = self._push_version(draft_id)
-        if not isinstance(context, PublisherContext):
-            return
-        pull_request = StashPrRequest(
-            title=context.feature.name,
-            description=self._compile_publication_description(context),
-            open=True,
-            fromRef=StashBranch(id=context.target_branch, repository=self._stash_publisher_settings.repository),
-            toRef=self._stash_publisher_settings.target_branch,
-            reviewers=self._stash_publisher_settings.get_reviewers(feature_type=context.feature.feature_type.name),
+    def _compile_publication_description(self, context: PublisherContext) -> str:
+        return "\n".join(
+            (
+                f"Feature ID: {context.feature.id}. Type: '{context.feature.feature_type.name}'.",
+                f"Created by: @{context.feature.author} at {context.feature.created_at.strftime('%d-%m-%Y %H:%M:%S')}.",
+                f"Last edited by: @{context.feature.last_edited_by}.",
+                f"PR from Test Run ID: {context.test_run.id}. Executed by: @{context.test_run.executed_by}",
+                f"Published by: @{context.draft.published_by}.",
+                generate_task_info(tasks=context.feature.task, header=self._project_settings.tasks_keyword),
+            )
         )
-        logger.info("Prepared pull-request: %s", pull_request.json(by_alias=True))
+
+    @abc.abstractmethod
+    def _prepare_repo(self, context: PublisherContext) -> None:
+        pass
+
+    def _prepare_publisher_context(self, draft_id: int) -> PublisherContext | None:
+        logger.info("Start processing draft_id=%s...", draft_id)
+        self._draft_storage.set_draft_status(draft_id, db.DraftStatus.CREATING)
+        context = self._compile_context(draft_id)
         try:
-            response = self._client.send_pull_request(pull_request)
-            if isinstance(response, StashPrCreationResponse):
-                self._draft_storage.save_response(
-                    draft_id=draft_id,
-                    pr_url=response.get_pr_url(),
-                    published_at=response.created_date,
-                    status=DraftStatus.CREATED,
-                )
-                return
-            if isinstance(response, StashErrorResponse) and response.duplicate:
-                self._save_as_duplicate(context)
-                return
-            logger.error("Gotten error response from Stash: %s", response)
-        except StashHttpClientConflictError:
-            logger.exception("Gotten conflict. Try to return last pull-request for Draft with id=%s...", draft_id)
-            self._save_as_duplicate(context)
-        except HTTPError as e:
-            self._draft_storage.set_draft_status(draft_id, DraftStatus.INTERNAL_ERROR, str(e))
-            logger.exception("Got HTTP error while trying to sent pull-request!")
+            self._prepare_repo(context)
+            return context
+        except (git.GitCommandError, GitPullError, BaseGitVersionPublisherError) as err:
+            logger.exception("Error while trying to pull or push!")
+            self._draft_storage.set_draft_status(draft_id, db.DraftStatus.INTERNAL_ERROR, traceback=str(err))
+            return None
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/config_injector.py` & `overhave-4.0.0/overhave/pytest_plugin/config_injector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Optional
 
 from _pytest.main import Session
 
 from overhave.entities import IFeatureExtractor, OverhaveFileSettings, StepPrefixesModel
 from overhave.test_execution import PytestRunner, StepCollector
 
 logger = logging.getLogger(__name__)
@@ -17,24 +16,24 @@
     """Excepion for situation with unresolved entities."""
 
 
 class ConfigInjector:
     """Special class to operate with pytest entites, for example get data and patch objects."""
 
     def __init__(self) -> None:
-        self._file_settings: Optional[OverhaveFileSettings] = None
-        self._step_collector: Optional[StepCollector] = None
-        self._test_runner: Optional[PytestRunner] = None
-        self._feature_extractor: Optional[IFeatureExtractor] = None
+        self._file_settings: OverhaveFileSettings | None = None
+        self._step_collector: StepCollector | None = None
+        self._test_runner: PytestRunner | None = None
+        self._feature_extractor: IFeatureExtractor | None = None
 
-        self._current_type: Optional[str] = None
+        self._current_type: str | None = None
         self._initialized = False
 
     @staticmethod
-    def patch_pytestbdd_prefixes(custom_step_prefixes: Optional[StepPrefixesModel]) -> None:
+    def patch_pytestbdd_prefixes(custom_step_prefixes: StepPrefixesModel | None) -> None:
         """Def for patch pytestbdd STEP_PREFIXES."""
         if custom_step_prefixes is not None:
             step_prefixes = custom_step_prefixes.extend_defaults()
             logger.debug("Successfully extended pytest-bdd step prefixes with custom prefixes:\n%s", step_prefixes)
 
     def supplement_components(
         self,
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/deps.py` & `overhave-4.0.0/overhave/pytest_plugin/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/pytest_plugin/helpers/__init__.py` & `overhave-4.0.0/overhave/pytest_plugin/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py` & `overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from typing import List
-
 import allure
 from markupsafe import Markup
 
 from overhave.entities import OverhaveDescriptionManagerSettings
 
 
 class DescriptionManager:
     """Class for test-suit custom description management and setting to Allure report."""
 
     def __init__(self, settings: OverhaveDescriptionManagerSettings):
         self._settings = settings
-        self._description: List[str] = []
+        self._description: list[str] = []
 
     def apply_description(self) -> None:
         if self._description:
             joined_description = self._settings.blocks_delimiter.join(self._description)
             if not self._settings.html:
                 allure.dynamic.description(joined_description)
                 return
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/links.py` & `overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/links.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 from pathlib import Path
-from typing import List
 
 import allure
 import allure_commons.types
 
 from overhave.scenario import OverhaveProjectSettings
 from overhave.test_execution import OverhaveAdminLinkSettings
 
 
-def add_task_links_to_report(project_settings: OverhaveProjectSettings, tasks: List[str]) -> None:
+def add_task_links_to_report(project_settings: OverhaveProjectSettings, tasks: list[str]) -> None:
     for task in tasks:
         allure.dynamic.link(
-            url=project_settings.get_task_link(task), link_type=allure_commons.types.LinkType.LINK, name=task
+            url=str(project_settings.get_task_link(task)), link_type=allure_commons.types.LinkType.LINK, name=task
         )
 
 
 def add_git_project_feature_link_to_report(project_settings: OverhaveProjectSettings, filepath: Path) -> None:
     allure.dynamic.link(
-        url=project_settings.get_git_feature_url(filepath),
+        url=str(project_settings.get_git_feature_url(filepath)),
         link_type=allure_commons.types.LinkType.TEST_CASE,
         name=filepath.as_posix(),
     )
 
 
 def add_admin_feature_link_to_report(admin_link_settings: OverhaveAdminLinkSettings, feature_id: int) -> None:
     allure.dynamic.link(
-        url=admin_link_settings.get_feature_url(feature_id),
+        url=str(admin_link_settings.get_feature_url(feature_id)),
         link_type=allure_commons.types.LinkType.TEST_CASE,
         name=admin_link_settings.get_feature_link_name(feature_id),
     )
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/severity.py` & `overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/severity.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from typing import Any, Optional
+from typing import Any
 
 import allure
 from _pytest.nodes import Item
 
 from overhave.pytest_plugin.helpers.parsed_info import get_feature_info_from_item
 from overhave.scenario import OverhaveScenarioCompilerSettings
 
 
-def _get_severity_level_from_tags(item: Item, keyword: str) -> Optional[allure.severity_level]:
+def _get_severity_level_from_tags(item: Item, keyword: str) -> allure.severity_level | None:
     for marker in reversed(item.own_markers):
         if not marker.name.startswith(keyword):
             continue
         severity = marker.name.removeprefix(keyword)
         return allure.severity_level(severity)
     return None
 
 
-def _get_parsed_feature_severity(item: Item, **kwargs: Any) -> Optional[allure.severity_level]:
+def _get_parsed_feature_severity(item: Item, **kwargs: Any) -> allure.severity_level | None:
     return get_feature_info_from_item(item).severity
 
 
 def _get_default_severity(*args: Any, **kwargs: Any) -> allure.severity_level:
     return allure.severity_level.NORMAL
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py` & `overhave-4.0.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import enum
 import logging
 from functools import cached_property
-from typing import Optional, cast
+from typing import cast
 from unittest.mock import MagicMock
 
 import allure
 from allure_commons._allure import StepContext
 
 from overhave.entities import OverhaveStepContextSettings
 
 
-class _WrapperPosition(str, enum.Enum):
+class _WrapperPosition(enum.StrEnum):
     ABOVE = "above"
     BELOW = "below"
 
 
 class StepContextNotDefinedError(Exception):
     """Exception for situation with calling for self._step, when StepContext has not been defined."""
 
 
 class StepContextRunner:
     """Class for Allure StepContext wrapping during pytest-bdd step execution."""
 
     def __init__(self, settings: OverhaveStepContextSettings) -> None:
         self._settings = settings
-        self._step: Optional[StepContext] = None
+        self._step: StepContext | None = None
 
     def set_title(self, title: str) -> None:
         self._step = allure.step(title)
 
     @cached_property
     def _defined_step(self) -> StepContext:
         if isinstance(self._step, StepContext):
@@ -53,14 +53,14 @@
             self._logger.info("%s", arg)
         self._logger.info("")
 
     def start(self) -> None:
         self._defined_step.__enter__()
         self._log_step_state(state="started", wrapper_position=_WrapperPosition.ABOVE, symbol="*")
 
-    def stop(self, exception: Optional[BaseException]) -> None:
+    def stop(self, exception: BaseException | None) -> None:
         if isinstance(exception, BaseException):
             self._log_step_state(state="failed", wrapper_position=_WrapperPosition.BELOW, symbol="!")
             self._defined_step.__exit__(exc_type=type(exception), exc_val=exception, exc_tb=exception.__traceback__)
         else:
             self._log_step_state(state="finished", wrapper_position=_WrapperPosition.BELOW, symbol="-")
             self._defined_step.__exit__(exc_type=None, exc_val=None, exc_tb=None)
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/helpers/bdd_item.py` & `overhave-4.0.0/overhave/pytest_plugin/helpers/bdd_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 
 def add_scenario_title_to_report(item: Item) -> None:
     item._obj.__allure_display_name__ = get_scenario(item).name  # type: ignore
 
 
 def is_pytest_bdd_item(item: Item) -> bool:
     if hasattr(item, "_obj"):
-        return hasattr(item._obj, "__scenario__") and isinstance(  # type: ignore
-            get_scenario(item), (Scenario, ScenarioTemplate)
-        )
+        return hasattr(item._obj, "__scenario__") and isinstance(get_scenario(item), (Scenario, ScenarioTemplate))
     return False
 
 
 def get_full_step_name(step: Step) -> str:
     return f"{step.keyword} {step._name}"
 
 
@@ -38,11 +36,11 @@
     item: Item,
     feature_type: FeatureTypeName,
 ) -> None:
     scenario = get_scenario(item)
     filename = Path(scenario.feature.filename)
     feature_type_dir = feature_extractor.feature_type_to_dir_mapping[feature_type]
     if not filename.is_relative_to(feature_type_dir):
-        logger.warning("pytest_bdd item file '%s' is not relative to '%s'!")
+        logger.warning("pytest_bdd item file '%s' is not relative to '%s'!", filename, feature_type_dir)
         return
     relative_path = filename.relative_to(feature_type_dir.parent)
     add_git_project_feature_link_to_report(project_settings=project_settings, filepath=relative_path)
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/helpers/parsed_info.py` & `overhave-4.0.0/overhave/pytest_plugin/helpers/parsed_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Optional, cast
+from typing import cast
 
 from _pytest.nodes import Item
 from pytest_bdd.parser import Scenario
 
 from overhave.pytest_plugin.helpers.bdd_item import get_scenario
 from overhave.scenario import FeatureInfo, ScenarioParser
 
@@ -18,11 +18,11 @@
         item,
         "feature_info",
         _parse_feature_info_from_file(scenario=get_scenario(item), scenario_parser=scenario_parser),
     )
 
 
 def get_feature_info_from_item(item: Item) -> FeatureInfo:
-    feature_info: Optional[FeatureInfo] = getattr(item, "feature_info")
+    feature_info: FeatureInfo | None = getattr(item, "feature_info")
     if feature_info is None:
         raise AttributeError(f"Item {item} has not got attr 'feature_info'!")
     return feature_info
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/helpers/tag_controller.py` & `overhave-4.0.0/overhave/pytest_plugin/helpers/tag_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 from functools import cached_property
-from typing import Mapping, Optional, Pattern, Tuple
+from typing import Mapping, Pattern
 
 import allure_commons.types
 import pytest
 from _pytest.mark.structures import MarkDecorator
 from pydantic import BaseModel
 
 
 class TagEvaluationResult(BaseModel):
     """Class for tag evaluation result."""
 
     marker: MarkDecorator
-    url: Optional[str]
+    url: str | None
     link_type: str
 
     class Config:
         arbitrary_types_allowed = True
 
 
 class BaseOverhaveTagControllerException(Exception):
@@ -33,15 +33,15 @@
     @staticmethod
     def _get_tag_pattern(keyword: str) -> Pattern[str]:
         return re.compile(rf"\b({keyword})+(\(+[^@()]+\)+)?\b")
 
     @cached_property
     def _tag_to_evaluation_result_mapping(
         self,
-    ) -> Mapping[Pattern[str], Tuple[MarkDecorator, allure_commons.types.LinkType]]:
+    ) -> Mapping[Pattern[str], tuple[MarkDecorator, allure_commons.types.LinkType]]:
         return {
             self._get_tag_pattern("disabled"): (
                 pytest.mark.skip,
                 allure_commons.types.LinkType.LINK,
             ),
             self._get_tag_pattern("xfail"): (
                 pytest.mark.xfail,
@@ -53,21 +53,21 @@
     def _reason_pattern(self) -> Pattern[str]:
         return re.compile(r"\w+\((?P<reason>[^@()]+)\)")
 
     @cached_property
     def _url_pattern(self) -> Pattern[str]:
         return re.compile(r"(?P<url>\b\w+://[^\s\"\']+\b)")
 
-    def _get_url(self, reason: str) -> Optional[str]:
+    def _get_url(self, reason: str) -> str | None:
         searched = self._url_pattern.search(reason)
         if searched is not None:
             return searched.group("url")
         return None
 
-    def get_suitable_pattern(self, name: str) -> Optional[Pattern[str]]:
+    def get_suitable_pattern(self, name: str) -> Pattern[str] | None:
         for pattern in self._tag_to_evaluation_result_mapping:
             result = pattern.match(name)
             if result is not None:
                 return pattern
         return None
 
     def evaluate_tag(self, name: str, pattern: Pattern[str]) -> TagEvaluationResult:
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/plugin.py` & `overhave-4.0.0/overhave/pytest_plugin/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-import enum
 import logging
-from typing import Any, Callable, Dict, Optional
+from typing import Any, Callable
 
 import _pytest
 import allure
+import httpx
 from _pytest.config import Config
-from _pytest.config.argparsing import Argument, Parser
 from _pytest.fixtures import FixtureRequest
 from _pytest.main import Session
 from _pytest.nodes import Item
 from _pytest.python import Function
 from pydantic import ValidationError
-from pydantic.dataclasses import dataclass
 from pytest_bdd.parser import Feature, Scenario, Step
-from yarl import URL
 
 from overhave.factory import IAdminFactory
 from overhave.pytest_plugin.deps import get_description_manager, get_step_context_runner, get_tag_controller
 from overhave.pytest_plugin.helpers import (
     add_admin_feature_link_to_report,
     add_scenario_title_to_report,
     add_task_links_to_report,
@@ -33,61 +30,28 @@
 logger = logging.getLogger(__name__)
 
 
 class StepNotFoundError(RuntimeError):
     """Exception for situation with missing or incorrect step definition."""
 
 
-class _OptionName(str, enum.Enum):
-    ENABLE_INJECTION = "--enable-injection"
-
-    @property
-    def as_variable(self) -> str:
-        return self.value.lstrip("--").replace("-", "_")
-
-
-_ENABLE_INJECTION_HELP = "Injection enabling of Overhave specified objects into PyTest session"
-_FACTORY_CONTEXT_HELP = (
-    "Relative path to lib with Overhave context definition for it's dynamical resolution before injection"
-)
-
-
-@dataclass(frozen=True)
-class _Options:
-    enable_injection = Argument(
-        _OptionName.ENABLE_INJECTION.value,
-        action="store_true",
-        dest=_OptionName.ENABLE_INJECTION.as_variable,
-        default=False,
-        help=_ENABLE_INJECTION_HELP,
-    )
-
-
-_PLUGIN_NAME = "overhave-pytest"
-_GROUP_HELP = "Overhave PyTest plugin commands"
-
-
-def pytest_addoption(parser: Parser) -> None:
-    group = parser.getgroup(_PLUGIN_NAME, _GROUP_HELP)
-    group.addoption(*_Options.enable_injection.names(), **_Options.enable_injection.attrs())
-
-
 def pytest_configure(config: Config) -> None:
     """Patch pytest_bdd objects in current hook."""
-    injection_enabled: bool = config.getoption(_OptionName.ENABLE_INJECTION.as_variable)
+    proxy_manager = get_proxy_manager()
+    if not proxy_manager.has_factory:
+        logger.debug("Overhave ProxyManager has not got prepared factory, so skip injection.")
+        return
     tw = _pytest.config.create_terminal_writer(config)
-    if injection_enabled:
-        logger.debug("Got %s flag.", _OptionName.ENABLE_INJECTION)
-        try:
-            logger.debug("Try to patch pytest objects...")
-            get_proxy_manager().patch_pytest()
-            logger.debug("Successfully patched pytest objects.")
-            tw.line("Overhave injector successfully initialized.", green=True)
-        except ValidationError as e:
-            tw.line(f"Could not initialize Overhave injector!\n{str(e)}", red=True)
+    try:
+        logger.debug("Try to patch pytest objects...")
+        proxy_manager.patch_pytest()
+        logger.debug("Successfully patched pytest objects.")
+        tw.line("Overhave injector successfully initialized.", green=True)
+    except ValidationError as e:
+        tw.line(f"Could not initialize Overhave injector!\n{str(e)}", red=True)
 
 
 def pytest_collection_modifyitems(session: Session) -> None:
     pytest_bdd_scenario_items = (item for item in session.items if is_pytest_bdd_item(item))
     for item in pytest_bdd_scenario_items:
         add_scenario_title_to_report(item)
 
@@ -103,34 +67,34 @@
 
 def pytest_bdd_after_step(
     request: FixtureRequest,
     feature: Feature,
     scenario: Scenario,
     step: Step,
     step_func: Callable[[Any], None],
-    step_func_args: Dict[str, Any],
+    step_func_args: dict[str, Any],
 ) -> None:
     runner = get_step_context_runner()
     runner.stop(None)
 
 
 def pytest_bdd_step_error(
     request: FixtureRequest,
     feature: Feature,
     scenario: Scenario,
     step: Step,
     step_func: Callable[[Any], None],
-    step_func_args: Dict[str, Any],
+    step_func_args: dict[str, Any],
     exception: BaseException,
 ) -> None:
     runner = get_step_context_runner()
     runner.stop(exception)
 
 
-def pytest_bdd_apply_tag(tag: str, function: Function) -> Optional[bool]:
+def pytest_bdd_apply_tag(tag: str, function: Function) -> bool | None:
     controller = get_tag_controller()
     tag_pattern = controller.get_suitable_pattern(tag)
     if not tag_pattern:
         logger.debug("Tag '%s' is not suitable for evaluation", tag)
         return None
     result = controller.evaluate_tag(name=tag, pattern=tag_pattern)
     result.marker(function)
@@ -143,49 +107,46 @@
 def pytest_bdd_step_func_lookup_error(
     request: FixtureRequest, feature: Feature, scenario: Scenario, step: Step, exception: BaseException
 ) -> None:
     raise StepNotFoundError(f"Could not found specified step '{get_full_step_name(step)}'") from exception
 
 
 def pytest_collection_finish(session: Session) -> None:
-    """Supplying of injector configs for steps collection."""
+    """Supplying of injector configs for steps collection (only :class:`IAdminFactory`)."""
     proxy_manager = get_proxy_manager()
-    if (
-        session.config.getoption(_OptionName.ENABLE_INJECTION.as_variable)
-        and proxy_manager.has_factory
-        and isinstance(proxy_manager.factory, IAdminFactory)
-    ):
-        tw = _pytest.config.create_terminal_writer(session.config)
-        if not proxy_manager.pytest_patched:
-            tw.line("Could not supplement Overhave injector - pytest session has not been patched!", yellow=True)
-            return
-        try:
-            proxy_manager.supply_injector_for_collection()
-            tw.line("Overhave injector successfully supplemented.", green=True)
-        except ValidationError as e:
-            tw.line(f"Could not supplement Overhave injector!\n{str(e)}", red=True)
-        proxy_manager.injector.adapt(session)
+    if not proxy_manager.has_factory or not isinstance(proxy_manager.factory, IAdminFactory):
+        return
+    tw = _pytest.config.create_terminal_writer(session.config)
+    if not proxy_manager.pytest_patched:
+        tw.line("Could not supplement Overhave injector - pytest session has not been patched!", yellow=True)
+        return
+    try:
+        proxy_manager.supply_injector_for_collection()
+        tw.line("Overhave injector successfully supplemented.", green=True)
+    except ValidationError as e:
+        tw.line(f"Could not supplement Overhave injector!\n{str(e)}", red=True)
+    proxy_manager.injector.adapt(session)
 
 
 def pytest_runtest_setup(item: Item) -> None:
     """Hook for purgation of `get_description_manager` func and upgrading item for reports."""
     get_description_manager.cache_clear()
-    if not is_pytest_bdd_item(item):
+    proxy_manager = get_proxy_manager()
+    if not proxy_manager.has_factory or not is_pytest_bdd_item(item):
         return
 
-    proxy_manager = get_proxy_manager()
     set_feature_info_for_item(item=item, scenario_parser=proxy_manager.factory.scenario_parser)
     feature_info = get_feature_info_from_item(item)
 
     admin_link_settings = proxy_manager.factory.context.admin_link_settings  # type: ignore
     if admin_link_settings.enabled and feature_info.id is not None:
         add_admin_feature_link_to_report(admin_link_settings=admin_link_settings, feature_id=feature_info.id)
 
     project_settings = proxy_manager.factory.context.project_settings
-    if isinstance(project_settings.git_project_url, URL) and feature_info.type is not None:
+    if isinstance(project_settings.git_project_url, httpx.URL) and feature_info.type is not None:
         set_git_project_url_if_necessary(
             project_settings=project_settings,
             feature_extractor=proxy_manager.factory.feature_extractor,
             item=item,
             feature_type=feature_info.type,
         )
     if isinstance(project_settings.tasks_keyword, str) and feature_info.tasks:
@@ -193,10 +154,12 @@
 
     set_severity_level(
         compilation_settings=proxy_manager.factory.context.compilation_settings,
         item=item,
     )
 
 
-def pytest_runtest_teardown(item: Item, nextitem: Optional[Item]) -> None:
+def pytest_runtest_teardown(item: Item, nextitem: Item | None) -> None:
     """Hook for description attachment to Allure report."""
+    if not get_proxy_manager().has_factory:
+        return
     get_description_manager().apply_description()
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/plugin_resolver.py` & `overhave-4.0.0/overhave/pytest_plugin/plugin_resolver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 import abc
 import logging
 from pathlib import Path
-from typing import Dict, List, Optional, Set
 
 from overhave.entities import BaseFileExtractor, OverhaveFileSettings
 
 logger = logging.getLogger(__name__)
 
 
 class IPluginResolver(abc.ABC):
     """Abstract class for custom pytest-bdd steps modules resolution."""
 
     @abc.abstractmethod
-    def get_plugins(self, plugin_type: Optional[str] = None) -> List[str]:
+    def get_plugins(self, plugin_type: str | None = None) -> list[str]:
         pass
 
 
 class PluginResolver(BaseFileExtractor, IPluginResolver):
     """Class for custom pytest-bdd steps modules resolution."""
 
     def __init__(self, file_settings: OverhaveFileSettings):
         super().__init__(extenstion=".py")
         self._file_settings = file_settings
         self._plugins = self._resolve_plugins(directory=self._file_settings.steps_dir)
         logger.debug("Available Overhave pytest plugin modules: %s", self._plugins)
 
-    def _resolve_plugins(self, directory: Path) -> Dict[str, List[Path]]:
+    def _resolve_plugins(self, directory: Path) -> dict[str, list[Path]]:
         plugin_folders = [d for d in directory.iterdir() if self._check_dir_compliance(d)]
         plugin_dict = {folder.name: self._extract_recursively(folder) for folder in plugin_folders}
 
         plugin_modules = [m for m in directory.iterdir() if self._check_file_compliance(m)]
         for folder in plugin_dict:
             plugin_dict[folder].extend(plugin_modules)
         return plugin_dict
 
     def _format_path(self, path: Path) -> str:
         relative_path = path.relative_to(self._file_settings.work_dir).as_posix()
         return relative_path.replace("/", ".").rstrip(".py")
 
-    def get_plugins(self, plugin_type: Optional[str] = None) -> List[str]:
+    def get_plugins(self, plugin_type: str | None = None) -> list[str]:
         if isinstance(plugin_type, str):
             if self._plugins.get(plugin_type) is None:
                 raise KeyError(f"Specified plugin type '{plugin_type}' does not exist!")
             plugins = [self._format_path(x) for x in self._plugins[plugin_type]]
             logger.debug("Return plugins by plugin_type='%s': %s", plugin_type, plugins)
             return plugins
 
-        joined_modules: Set[str] = set()
+        joined_modules: set[str] = set()
         for key in self._plugins:
             joined_modules.update(set(self.get_plugins(key)))
         modules_list = list(joined_modules)
         logger.debug("Return all existing plugins: %s", modules_list)
         return modules_list
```

### Comparing `overhave-3.9.0/overhave/pytest_plugin/proxy_manager.py` & `overhave-4.0.0/overhave/pytest_plugin/proxy_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import abc
 from functools import cache, cached_property
-from typing import Optional, Union
+from typing import Union
 
 from overhave.factory import IAdminFactory, ITestExecutionFactory
 from overhave.pytest_plugin.config_injector import ConfigInjector
 from overhave.pytest_plugin.plugin_resolver import IPluginResolver, PluginResolver
 
-AnyProxyFactory = Union[IAdminFactory, ITestExecutionFactory]
+AnyProxyFactory = Union[IAdminFactory | ITestExecutionFactory]
 
 
 class IProxyManager(abc.ABC):
     """Abstract class for proxy manager."""
 
     @property
     @abc.abstractmethod
@@ -71,15 +71,15 @@
     """Exception for situation with not defined `factory`."""
 
 
 class ProxyManager(IProxyManager):
     """Manager for application factory resolution and usage, based on proxy-object pattern."""
 
     def __init__(self) -> None:
-        self._factory: Optional[AnyProxyFactory] = None
+        self._factory: AnyProxyFactory | None = None
         self._pytest_patched = False
         self._collection_prepared = False
 
     @cached_property
     def _injector(self) -> ConfigInjector:
         return ConfigInjector()
```

### Comparing `overhave-3.9.0/overhave/scenario/compiler/compiler.py` & `overhave-4.0.0/overhave/scenario/compiler/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import List, Optional, cast
-
 import allure
 from pytest_bdd import types as default_types
 
 from overhave.entities import OverhaveLanguageSettings
 from overhave.scenario.compiler.settings import OverhaveScenarioCompilerSettings
 from overhave.scenario.prefix_mixin import PrefixMixin
 from overhave.storage import TestExecutorContext
 
 
-def generate_task_info(tasks: List[str], header: Optional[str]) -> str:
+def generate_task_info(tasks: list[str], header: str | None) -> str:
     if tasks and header is not None:
         return f"{header}: {', '.join(tasks)}"
     return ""
 
 
-def generate_tags_list(context: TestExecutorContext) -> Optional[List[str]]:
+def generate_tags_list(context: TestExecutorContext) -> list[str] | None:
     if feature_tags := [i.value for i in context.feature.feature_tags]:
         return feature_tags
     return None
 
 
 class ScenarioCompilerError(Exception):
     """Base exception for :class:`ScenarioCompiler` errors."""
@@ -32,53 +30,53 @@
 class ScenarioCompiler(PrefixMixin):
     """Class for scenario compilation from text view into pytest_bdd feature format."""
 
     def __init__(
         self,
         compilation_settings: OverhaveScenarioCompilerSettings,
         language_settings: OverhaveLanguageSettings,
-        tasks_keyword: Optional[str],
+        tasks_keyword: str | None,
     ):
         self._compilation_settings = compilation_settings
         self._language_settings = language_settings
         self._tasks_keyword = tasks_keyword
 
     def _get_feature_type_tag(self, scenario_text: str, tag: str) -> str:
         if f"{self._compilation_settings.tag_prefix}{tag}" in scenario_text:
             return ""
         return f"{self._compilation_settings.tag_prefix}{tag}"
 
-    def _get_additional_tags(self, scenario_text: str, tags: Optional[List[str]]) -> str:
+    def _get_additional_tags(self, scenario_text: str, tags: list[str] | None) -> str:
         if f"{self._compilation_settings.tag_prefix}{tags}" in scenario_text:
             return ""
         if tags is not None:
             tags_with_prefix = (f"{self._compilation_settings.tag_prefix}{tag}" for tag in tags)
             return f"{' '.join(tags_with_prefix)}"
         return ""
 
     def _get_severity_tag(self, severity: allure.severity_level) -> str:
         return f"{self._compilation_settings.severity_prefix}{severity.value}"
 
-    def _get_feature_prefix_if_specified(self, scenario_text: str) -> Optional[str]:
-        keywords: List[str] = [default_types.FEATURE]
+    def _get_feature_prefix_if_specified(self, scenario_text: str) -> str | None:
+        keywords: list[str] = [default_types.FEATURE]
         if self._language_settings.step_prefixes is not None:
             keywords.append(self._language_settings.step_prefixes.FEATURE)
 
         for key in keywords:
             if self._as_prefix(key) not in scenario_text:
                 continue
             return key
         return None
 
     def _detect_feature_prefix_by_scenario_format(self, scenario_text: str) -> str:
         if (
             self._as_prefix(default_types.SCENARIO) in scenario_text
             or self._as_prefix(default_types.SCENARIO_OUTLINE) in scenario_text
         ):
-            return cast(str, default_types.FEATURE)
+            return default_types.FEATURE
         step_prefixes = self._language_settings.step_prefixes
         if step_prefixes is not None and (
             self._as_prefix(step_prefixes.SCENARIO) in scenario_text
             or self._as_prefix(step_prefixes.SCENARIO_OUTLINE) in scenario_text
         ):
             return step_prefixes.FEATURE
         raise IncorrectScenarioTextError(
```

### Comparing `overhave-3.9.0/overhave/scenario/compiler/settings.py` & `overhave-4.0.0/overhave/scenario/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/scenario/file_manager/file_manager.py` & `overhave-4.0.0/overhave/scenario/file_manager/file_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def tmp_feature_file(
         self, context: TestExecutorContext
     ) -> Iterator[tempfile._TemporaryFileWrapper]:  # type: ignore
         file_name = Path(context.feature.file_path).name
         logger.debug("Feature file name: '%s'", file_name)
         with tempfile.NamedTemporaryFile(
             dir=self._file_settings.tmp_features_dir,
-            prefix=f"{file_name}_id{context.feature.id}",
+            prefix=f"{file_name}_id{context.feature.id}_",
             suffix=self._file_settings.feature_suffix,
             mode="w",
         ) as file:
             data = self._scenario_compiler.compile(context=context)
             logger.debug("Scenario file:\n%s", data)
             self._write_data(file=file, data=data, entity_name="feature")
             yield file
```

### Comparing `overhave-3.9.0/overhave/scenario/parser/parser.py` & `overhave-4.0.0/overhave/scenario/parser/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import re
 from datetime import datetime
 from functools import cached_property
-from typing import List, Optional, Sequence, Union
+from typing import Sequence
 
 import allure
 from pytest_bdd import types as default_types
 
 from overhave.entities import IFeatureExtractor, OverhaveLanguageSettings
 from overhave.scenario.compiler import OverhaveScenarioCompilerSettings
 from overhave.scenario.parser.models import FeatureInfo, StrictFeatureInfo
@@ -51,35 +51,35 @@
 
     def __init__(
         self,
         parser_settings: OverhaveScenarioParserSettings,
         compilation_settings: OverhaveScenarioCompilerSettings,
         language_settings: OverhaveLanguageSettings,
         feature_extractor: IFeatureExtractor,
-        tasks_keyword: Optional[str],
+        tasks_keyword: str | None,
     ) -> None:
         self._parser_settings = parser_settings
         self._compilation_settings = compilation_settings
         self._language_settings = language_settings
         self._feature_extractor = feature_extractor
         self._tasks_keyword = tasks_keyword
 
     def set_strict_mode(self, mode: bool) -> None:
         self._parser_settings.parser_strict_mode = mode
 
     @cached_property
-    def _feature_prefixes(self) -> List[str]:
+    def _feature_prefixes(self) -> list[str]:
         prefixes = [self._as_prefix(default_types.FEATURE)]
         if self._language_settings.step_prefixes is not None:
             prefixes.append(self._as_prefix(self._language_settings.step_prefixes.FEATURE))
         logger.debug("Cached ScenarioParser feature prefixes: %s", prefixes)
         return prefixes
 
     @cached_property
-    def _task_prefix(self) -> Optional[str]:
+    def _task_prefix(self) -> str | None:
         if isinstance(self._tasks_keyword, str):
             return self._as_prefix(self._tasks_keyword)
         return None
 
     def _get_id(self, id_line: str) -> int:
         return int(id_line.removeprefix(self._compilation_settings.id_prefix).strip())
 
@@ -87,41 +87,41 @@
         name_parts = name_line.split(feature_prefix)
         if not name_parts:
             raise FeatureNameParsingError(
                 f"Could not parse feature name from '{name_line}'!",
             )
         return name_parts[-1].strip()
 
-    def _get_tags(self, tags_line: str) -> List[str]:
+    def _get_tags(self, tags_line: str) -> list[str]:
         return [tag.strip() for tag in tags_line.split(self._compilation_settings.tag_prefix) if tag]
 
     def _get_feature_type(self, tags: Sequence[str]) -> FeatureTypeName:
         for tag in tags:
             if tag not in self._feature_extractor.feature_types:
                 continue
             return FeatureTypeName(tag)
         raise FeatureTypeParsingError(
             f"Could not get feature type from tags {tags}!",
         )
 
-    def _get_severity_tag(self, tags: Sequence[str]) -> Optional[str]:
+    def _get_severity_tag(self, tags: Sequence[str]) -> str | None:
         for tag in reversed(tags):
             if self._compilation_settings.severity_keyword not in tag:
                 continue
             return tag
         return None
 
     @staticmethod
     def _get_additional_info(additional_line: str, left_pointer: str, right_pointer: str) -> str:
         result = re.search(rf"({left_pointer})+\s?[\w.]+\s?({right_pointer})+", additional_line)
         if result:
             return result.group(0).removeprefix(left_pointer).removesuffix(right_pointer).strip()
         raise AdditionalInfoParsingError("Could not parse additional info from '%s'!", additional_line)
 
-    def _get_task_info(self, task_line: str) -> List[str]:
+    def _get_task_info(self, task_line: str) -> list[str]:
         tasks = []
         if self._task_prefix is not None:
             tasks.extend(task_line.removeprefix(self._task_prefix).split(","))
         return [x.strip() for x in tasks]
 
     def _get_time_info(self, line: str, left_pointer: str, right_pointer: str) -> datetime:
         result = re.search(rf"({left_pointer})+[\w\-:\s]+({right_pointer})+", line)
@@ -174,15 +174,15 @@
             if self._task_prefix is not None and self._task_prefix in line:
                 feature_info.tasks = self._get_task_info(line)
                 continue
         if feature_info.name is None:
             raise FeatureNameParsingError(f"Could not parse feature name from header:\n{header}")
         return feature_info
 
-    def parse(self, feature_txt: str) -> Union[FeatureInfo, StrictFeatureInfo]:
+    def parse(self, feature_txt: str) -> FeatureInfo | StrictFeatureInfo:
         blocks_delimiter = "\n\n"
         indent = "  "
         indent_substitute = "__"
         blocks = [
             block.lstrip(" \n") for block in feature_txt.replace(indent, indent_substitute).split(blocks_delimiter)
         ]
         header = blocks.pop(0)
```

### Comparing `overhave-3.9.0/overhave/scenario/validator.py` & `overhave-4.0.0/overhave/scenario/validator/validator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,59 @@
 import logging
 from pathlib import Path
-from typing import List
 
 from overhave.entities import BaseFileExtractor, GitRepositoryInitializer, OverhaveFileSettings
-from overhave.scenario import StrictFeatureParsingError
-from overhave.scenario.parser import NullableFeatureIdError, ScenarioParser
+from overhave.scenario.parser import NullableFeatureIdError, ScenarioParser, StrictFeatureParsingError
+from overhave.scenario.validator.abstract import IFeatureValidator
+from overhave.scenario.validator.duplicate_id_mixin import FeatureDuplicatedIdValidationMixin
+from overhave.scenario.validator.errors import FeaturesWithoutIDPresenceError, IncorrectFeaturesPresenceError
 
 logger = logging.getLogger(__name__)
 
 
-class BaseFeatureValidatorException(Exception):
-    """Base exception for :class:`FeatureValidator`."""
-
-
-class FeaturesWithoutIDPresenceError(BaseFeatureValidatorException):
-    """Exception for situation with nullable ID features presence."""
-
-
-class IncorrectFeaturesPresenceError(BaseFeatureValidatorException):
-    """Exception for situation with incorrect features presence."""
-
-
-class FeatureValidator(BaseFileExtractor):
+class FeatureValidator(IFeatureValidator, BaseFileExtractor, FeatureDuplicatedIdValidationMixin):
     """Class for features validation."""
 
     def __init__(
         self,
         file_settings: OverhaveFileSettings,
         scenario_parser: ScenarioParser,
         git_initializer: GitRepositoryInitializer,
     ):
         super().__init__(extenstion=file_settings.feature_suffix)
         self._file_settings = file_settings
         self._scenario_parser = scenario_parser
         self._git_initializer = git_initializer
 
         self._scenario_parser.set_strict_mode(True)
-        self._nullable_id_features: List[Path] = []
-        self._incorrect_features: List[Path] = []
+
+        self._nullable_id_features: list[Path] = []
+        self._incorrect_features: list[Path] = []
 
     def validate(self, raise_if_nullable_id: bool = False, pull_repository: bool = False) -> None:
         if pull_repository:
             self._git_initializer.pull()
         logger.info("Start validation...")
-        all_features = self._extract_recursively(self._file_settings.features_dir)
-        for feature_file in all_features:
-            logger.info("Read feature from file %s...", feature_file.as_posix())
+        feature_paths = self._extract_recursively(self._file_settings.features_dir)
+        for feature_path in feature_paths:
+            logger.info("Read feature from file %s...", feature_path.as_posix())
             try:
-                feature_info = self._scenario_parser.parse(feature_file.read_text())
+                feature_info = self._scenario_parser.parse(feature_path.read_text())
+                self._save_to_feature_id_to_path_mapping(feature_path=feature_path, feature_id=feature_info.id)
             except NullableFeatureIdError:
                 logger.warning("Feature has not got suitable Overhave ID!")
-                self._nullable_id_features.append(feature_file)
+                self._nullable_id_features.append(feature_path)
             except StrictFeatureParsingError:
                 logger.exception("Feature has incorrect format!")
-                self._incorrect_features.append(feature_file)
+                self._incorrect_features.append(feature_path)
             else:
                 logger.info("Feature successfully parsed: %s", feature_info)
         if self._incorrect_features:
             raise IncorrectFeaturesPresenceError(
                 f"Features with incorrect format: {[x.as_posix() for x in self._incorrect_features]}"
             )
         if raise_if_nullable_id and self._nullable_id_features:
             raise FeaturesWithoutIDPresenceError(
                 f"Features without IDs: {[x.as_posix() for x in self._nullable_id_features]}"
             )
+        self._validate_duplicate_ids()
         logger.info("All features are correct")
```

### Comparing `overhave-3.9.0/overhave/storage/__init__.py` & `overhave-4.0.0/overhave/storage/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     SystemUserModel,
     TagModel,
     TestExecutorContext,
     TestRunModel,
     TestUserModel,
     TestUserSpecification,
 )
-from .draft_storage import DraftStorage, IDraftStorage, UniqueDraftCreationError
+from .draft_storage import DraftStorage, IDraftStorage, NullableScenarioError
 from .emulation_storage import EmulationStorage, EmulationStorageError, IEmulationStorage
 from .feature_storage import FeatureStorage, IFeatureStorage
 from .feature_tag_storage import FeatureTagStorage, IFeatureTagStorage
 from .feature_type_storage import FeatureTypeNotExistsError, FeatureTypeStorage, IFeatureTypeStorage
 from .scenario_storage import IScenarioStorage, ScenarioStorage
 from .system_user_group_storage import ISystemUserGroupStorage, SystemUserGroupStorage
 from .system_user_storage import ISystemUserStorage, SystemUserStorage
```

### Comparing `overhave-3.9.0/overhave/storage/api_auth_storage.py` & `overhave-4.0.0/overhave/storage/api_auth_storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import abc
 from datetime import datetime
-from typing import Optional
 
 from pydantic.fields import Field
 from pydantic.main import BaseModel
 
 from overhave.utils import get_current_time
 
 
@@ -16,29 +15,29 @@
     token_type: str = Field("Bearer", const=True)
 
 
 class IAuthStorage(abc.ABC):
     """Abstract storage for auth_managers tokens."""
 
     @abc.abstractmethod
-    def get_auth_token(self, username: str) -> Optional[AuthToken]:
+    def get_auth_token(self, username: str) -> AuthToken | None:
         pass
 
     @abc.abstractmethod
     def update_auth_token(self, username: str, new_auth_token: AuthToken) -> None:
         pass
 
 
 class AuthStorage(IAuthStorage):
     """In-memory storage for auth_managers tokens."""
 
     def __init__(self) -> None:
         self._storage: dict[str, AuthToken] = {}
 
-    def get_auth_token(self, username: str) -> Optional[AuthToken]:
+    def get_auth_token(self, username: str) -> AuthToken | None:
         auth_token = self._storage.get(username)
         if auth_token and auth_token.expires_at > get_current_time():
             return auth_token
         return None
 
     def update_auth_token(self, username: str, new_auth_token: AuthToken) -> None:
         self._storage[username] = new_auth_token
```

### Comparing `overhave-3.9.0/overhave/storage/emulation_storage.py` & `overhave-4.0.0/overhave/storage/emulation_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import abc
 import logging
 import socket
-from typing import List, cast
+from typing import cast
 
+import sqlalchemy as sa
 import sqlalchemy.orm as so
 from pydantic.tools import parse_obj_as
 
 from overhave import db
 from overhave.entities.settings import OverhaveEmulationSettings
 from overhave.storage import EmulationRunModel
 from overhave.utils import get_current_time
@@ -14,28 +15,24 @@
 logger = logging.getLogger(__name__)
 
 
 class EmulationStorageError(Exception):
     """Base Exception for :class:`EmulationStorage`."""
 
 
-class NotFoundEmulationError(EmulationStorageError):
-    """Exception for situation without saved emulation.."""
-
-
 class AllPortsAreBusyError(EmulationStorageError):
     """Exception for situation when all ports are busy."""
 
 
 class IEmulationStorage(abc.ABC):
     """Abstract class for emulation runs storage."""
 
     @staticmethod
     @abc.abstractmethod
-    def create_emulation_run(emulation_id: int, initiated_by: str) -> EmulationRunModel:
+    def create_emulation_run(emulation_id: int, initiated_by: str) -> int:
         pass
 
     @abc.abstractmethod
     def get_requested_emulation_run(self, emulation_run_id: int) -> EmulationRunModel:
         pass
 
     @abc.abstractmethod
@@ -44,107 +41,98 @@
 
     @abc.abstractmethod
     def set_error_emulation_run(self, emulation_run_id: int, traceback: str) -> None:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def get_emulation_runs_by_test_user_id(test_user_id: int) -> List[EmulationRunModel]:
+    def get_emulation_runs_by_test_user_id(test_user_id: int) -> list[EmulationRunModel]:
         pass
 
 
 class EmulationStorage(IEmulationStorage):
     """Class for emulation runs storage."""
 
     def __init__(self, settings: OverhaveEmulationSettings):
         self._settings = settings
+        self._emulation_ports_len = len(self._settings.emulation_ports)
 
     @staticmethod
-    def create_emulation_run(emulation_id: int, initiated_by: str) -> EmulationRunModel:
+    def create_emulation_run(emulation_id: int, initiated_by: str) -> int:
         with db.create_session() as session:
-            emulation_run = db.EmulationRun(emulation_id=emulation_id, initiated_by=initiated_by)
+            emulation_run = db.EmulationRun(
+                emulation_id=emulation_id, initiated_by=initiated_by, status=db.EmulationStatus.CREATED
+            )
             session.add(emulation_run)
             session.flush()
-            return cast(EmulationRunModel, EmulationRunModel.from_orm(emulation_run))
-
-    @staticmethod
-    def _get_emulation_run(session: so.Session, emulation_run_id: int) -> db.EmulationRun:
-        emulation_run: db.EmulationRun = session.query(db.EmulationRun).get(emulation_run_id)
-        if emulation_run is not None:
-            return emulation_run
-        raise NotFoundEmulationError(f"Not found emulation run with ID {emulation_run_id}!")
+            return emulation_run.id
 
     def _get_next_port(self, session: so.Session) -> int:
         runs_with_allocated_ports = (  # noqa: ECE001
             session.query(db.EmulationRun)
             .filter(db.EmulationRun.port.isnot(None))
             .order_by(db.EmulationRun.id.desc())
-            .limit(len(self._settings.emulation_ports))
+            .limit(self._emulation_ports_len)
             .all()
         )
         allocated_sorted_runs = sorted(
             runs_with_allocated_ports,
-            key=lambda t: t.changed_at,  # type: ignore
+            key=lambda t: t.changed_at,
         )
 
         allocated_ports = {run.port for run in allocated_sorted_runs}
         logger.debug("Allocated ports: %s", allocated_ports)
         not_allocated_ports = set(self._settings.emulation_ports).difference(allocated_ports)
         logger.debug("Not allocated ports: %s", not_allocated_ports)
         if not_allocated_ports:
             for port in not_allocated_ports:
                 if self._is_port_in_use(port):
                     continue
                 return port
             logger.debug("All not allocated ports are busy!")
         for run in allocated_sorted_runs:
-            if self._is_port_in_use(run.port):
+            if self._is_port_in_use(cast(int, run.port)):
                 continue
             return cast(int, run.port)
         raise AllPortsAreBusyError("All ports are busy - could not find free port!")
 
     def _is_port_in_use(self, port: int) -> bool:
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             return s.connect_ex((self._settings.emulation_bind_ip, port)) == 0
 
     def get_requested_emulation_run(self, emulation_run_id: int) -> EmulationRunModel:
         with db.create_session() as session:
-            emulation_run = self._get_emulation_run(session, emulation_run_id)
+            emulation_run = session.query(db.EmulationRun).filter(db.EmulationRun.id == emulation_run_id).one()
             emulation_run.status = db.EmulationStatus.REQUESTED
             emulation_run.port = self._get_next_port(session)
             emulation_run.changed_at = get_current_time()
-            return cast(EmulationRunModel, EmulationRunModel.from_orm(emulation_run))
+            return EmulationRunModel.from_orm(emulation_run)
 
     def set_emulation_run_status(self, emulation_run_id: int, status: db.EmulationStatus) -> None:
         with db.create_session() as session:
-            emulation_run = self._get_emulation_run(session, emulation_run_id)
-            if emulation_run.status != status:
-                emulation_run.status = status
-                emulation_run.changed_at = get_current_time()
+            session.execute(
+                sa.update(db.EmulationRun)
+                .where(db.EmulationRun.id == emulation_run_id)
+                .values(status=status, changed_at=get_current_time())
+            )
 
     def set_error_emulation_run(self, emulation_run_id: int, traceback: str) -> None:
         with db.create_session() as session:
-            emulation_run = self._get_emulation_run(session, emulation_run_id)
-            emulation_run.status = db.EmulationStatus.ERROR
-            emulation_run.traceback = traceback
-            emulation_run.changed_at = get_current_time()
-
-    def get_emulation_run_by_id(self, emulation_run_id: int) -> EmulationRunModel:
-        with db.create_session() as session:
-            emulation_run: EmulationRunModel = EmulationRunModel.from_orm(
-                self._get_emulation_run(session, emulation_run_id)
+            session.execute(
+                sa.update(db.EmulationRun)
+                .where(db.EmulationRun.id == emulation_run_id)
+                .values(status=db.EmulationStatus.ERROR, changed_at=get_current_time(), traceback=traceback)
             )
-            return emulation_run
 
     @staticmethod
-    def get_emulation_runs_by_test_user_id(test_user_id: int) -> List[EmulationRunModel]:
+    def get_emulation_runs_by_test_user_id(test_user_id: int) -> list[EmulationRunModel]:
         with db.create_session() as session:
             emulation_ids_query = (
                 session.query(db.Emulation)
                 .with_entities(db.Emulation.id)
                 .filter(db.Emulation.test_user_id == test_user_id)
                 .scalar_subquery()
             )
             emulation_runs = (
-                session.query(db.EmulationRun).filter(db.EmulationRun.emulation_id == emulation_ids_query).all()
+                session.query(db.EmulationRun).where(db.EmulationRun.emulation_id.in_(emulation_ids_query)).all()
             )
-            return parse_obj_as(List[EmulationRunModel], emulation_runs)
+            return parse_obj_as(list[EmulationRunModel], emulation_runs)
```

### Comparing `overhave-3.9.0/overhave/storage/feature_storage.py` & `overhave-4.0.0/overhave/storage/feature_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,135 @@
 import abc
 import logging
-from typing import Iterable, List, Optional, cast
+from typing import Iterable, cast
 
+import sqlalchemy as sa
 import sqlalchemy.orm as so
 from pydantic.tools import parse_obj_as
 
 from overhave import db
 from overhave.storage.converters import FeatureModel
 from overhave.utils import get_current_time
 
 logger = logging.getLogger(__name__)
 
 
 class BaseFeatureStorageException(Exception):
     """Base exception for :class:`FeatureStorage`."""
 
 
-class FeatureNotExistsError(BaseFeatureStorageException):
-    """Error for situation when feature not found."""
-
-
 class FeatureTagNotExistsError(BaseFeatureStorageException):
     """Error for situation when tag not found."""
 
 
 class IFeatureStorage(abc.ABC):
     """Abstract class for feature storage."""
 
     @staticmethod
     @abc.abstractmethod
-    def get_feature(feature_id: int) -> Optional[FeatureModel]:
+    def feature_model_by_id(session: so.Session, feature_id: int) -> FeatureModel:
+        pass
+
+    @staticmethod
+    def get_feature_model(feature_id: int) -> FeatureModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
     def create_feature(model: FeatureModel) -> int:
         pass
 
     @staticmethod
     @abc.abstractmethod
     def update_feature(model: FeatureModel) -> None:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def get_features_by_tag(tag_id: int) -> List[FeatureModel]:
+    def get_features_by_tag(tag_id: int) -> list[FeatureModel]:
         pass
 
 
 def _append_tags_to_feature(session: so.Session, feature: db.Feature, tag_ids: Iterable[int]) -> None:
-    db_tags: List[db.Tags] = []
+    db_tags: list[db.Tags] = []
     for tag_id in tag_ids:
-        db_tag = session.query(db.Tags).get(tag_id)
+        db_tag = session.get(db.Tags, tag_id)
         if db_tag is None:
             raise FeatureTagNotExistsError(f"Feature tag with id={tag_id} does not exist!")
         logger.info("Append tag with id=%s and value=%s", tag_id, db_tag.value)
         db_tags.append(db_tag)
     feature.feature_tags.extend(db_tags)
 
 
 class FeatureStorage(IFeatureStorage):
     """Class for feature storage."""
 
     @staticmethod
-    def get_feature(feature_id: int) -> Optional[FeatureModel]:
-        with db.create_session() as session:
-            feature: Optional[db.Feature] = session.query(db.Feature).get(feature_id)
-            if feature is not None:
-                return cast(FeatureModel, FeatureModel.from_orm(feature))
-            return None
+    def feature_model_by_id(session: so.Session, feature_id: int) -> FeatureModel:
+        feature = session.query(db.Feature).filter(db.Feature.id == feature_id).one()
+        return FeatureModel.from_orm(feature)
 
     @staticmethod
     def create_feature(model: FeatureModel) -> int:
         with db.create_session() as session:
             feature = db.Feature(
                 name=model.name,
                 author=model.author,
                 type_id=model.feature_type.id,
                 file_path=model.file_path,
                 task=model.task,
                 severity=model.severity,
-                last_edited_at=get_current_time(),
+                last_edited_by=model.last_edited_by,
+                last_edited_at=model.last_edited_at,
+                released=model.released,
             )
-            feature.last_edited_at = model.last_edited_at
-            feature.released = model.released
             _append_tags_to_feature(session=session, feature=feature, tag_ids=(tag.id for tag in model.feature_tags))
             session.add(feature)
             session.flush()
             return cast(int, feature.id)
 
     @staticmethod
     def update_feature(model: FeatureModel) -> None:
         with db.create_session() as session:
-            feature: db.Feature = session.query(db.Feature).get(model.id)
-            if feature is None:
-                raise FeatureNotExistsError(f"Feature with id {model.id} does not exist!")
-            feature.name = model.name
-            feature.file_path = model.file_path
-            feature.task = model.task
-            feature.severity = model.severity
-            feature.last_edited_by = model.last_edited_by
-            feature.last_edited_at = get_current_time()
-            feature.released = True
-            session.flush()
-
+            session.execute(
+                sa.update(db.Feature)
+                .where(db.Feature.id == model.id)
+                .values(
+                    name=model.name,
+                    file_path=model.file_path,
+                    task=model.task,
+                    severity=model.severity,
+                    last_edited_by=model.last_edited_by,
+                    last_edited_at=get_current_time(),
+                    released=True,
+                )
+            )
+            feature = session.query(db.Feature).filter(db.Feature.id == model.id).one()
             existing_tags = {tag.id for tag in feature.feature_tags}
             model_tags = {tag.id for tag in model.feature_tags}
             tags_to_delete = existing_tags.difference(model_tags)
             for tag_id in tags_to_delete:
                 db_tag = next(tag for tag in feature.feature_tags if tag.id == tag_id)
                 logger.info("Remove tag with id=%s and value=%s", tag_id, db_tag.value)
                 feature.feature_tags.remove(db_tag)
             tags_to_append = model_tags.difference(existing_tags)
             _append_tags_to_feature(session=session, feature=feature, tag_ids=tags_to_append)
 
     @staticmethod
-    def get_features_by_tag(tag_id: int) -> List[FeatureModel]:
+    def get_features_by_tag(tag_id: int) -> list[FeatureModel]:
         with db.create_session() as session:
             feature_ids_query = (
                 session.query(db.FeatureTagsAssociationTable)
                 .with_entities(db.FeatureTagsAssociationTable.feature_id)
                 .filter(db.FeatureTagsAssociationTable.tags_id == tag_id)
                 .scalar_subquery()
             )
-            features = session.query(db.Feature).filter(db.Feature.id == feature_ids_query).all()
-            return parse_obj_as(List[FeatureModel], features)
+            features = session.query(db.Feature).filter(db.Feature.id.in_(feature_ids_query)).all()
+            return parse_obj_as(list[FeatureModel], features)
+
+    @staticmethod
+    def get_feature_model(feature_id: int) -> FeatureModel | None:
+        with db.create_session() as session:
+            feature = session.get(db.Feature, feature_id)
+            if feature is not None:
+                return FeatureModel.from_orm(feature)
+            return None
```

### Comparing `overhave-3.9.0/overhave/storage/scenario_storage.py` & `overhave-4.0.0/overhave/storage/system_user_storage.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 import abc
-from typing import Optional, cast
-
-from overhave import db
-from overhave.storage.converters import ScenarioModel
-
-
-class BaseScenarioStorageException(Exception):
-    """Base exception for :class:`ScenarioStorage`."""
 
+import sqlalchemy as sa
+from pydantic import SecretStr
 
-class ScenarioNotExistsError(BaseScenarioStorageException):
-    """Exception for situation without scenario."""
+from overhave import db
+from overhave.storage.converters import SystemUserModel
 
 
-class IScenarioStorage(abc.ABC):
-    """Abstract class for feature type storage."""
+class ISystemUserStorage(abc.ABC):
+    """Abstract class for system user storage."""
 
     @staticmethod
     @abc.abstractmethod
-    def get_scenario(scenario_id: int) -> Optional[ScenarioModel]:
+    def get_user(user_id: int) -> SystemUserModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def get_scenario_by_feature_id(feature_id: int) -> ScenarioModel:
+    def create_user(login: str, password: SecretStr | None = None, role: db.Role = db.Role.user) -> SystemUserModel:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def update_scenario(model: ScenarioModel) -> None:
+    def get_user_by_credits(login: str, password: SecretStr | None = None) -> SystemUserModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def create_scenario(model: ScenarioModel) -> int:
+    def update_user_role(user_model: SystemUserModel) -> None:
         pass
 
 
-class ScenarioStorage(IScenarioStorage):
-    """Class for feature type storage."""
+class SystemUserStorage(ISystemUserStorage):
+    """Class for system user storage."""
 
     @staticmethod
-    def get_scenario(scenario_id: int) -> Optional[ScenarioModel]:
+    def get_user(user_id: int) -> SystemUserModel | None:
         with db.create_session() as session:
-            scenario: Optional[db.Scenario] = session.query(db.Scenario).get(scenario_id)
-            if scenario is not None:
-                return cast(ScenarioModel, ScenarioModel.from_orm(scenario))
+            db_user = session.get(db.UserRole, user_id)
+            if db_user is not None:
+                return SystemUserModel.from_orm(db_user)
             return None
 
     @staticmethod
-    def get_scenario_by_feature_id(feature_id: int) -> ScenarioModel:
+    def create_user(login: str, password: SecretStr | None = None, role: db.Role = db.Role.user) -> SystemUserModel:
         with db.create_session() as session:
-            scenario: db.Scenario = session.query(db.Scenario).filter(db.Scenario.feature_id == feature_id).one()
-            return cast(ScenarioModel, ScenarioModel.from_orm(scenario))
+            db_password = None
+            if password is not None:
+                db_password = password.get_secret_value()
+            db_user = db.UserRole(login=login, password=db_password, role=role)
+            session.add(db_user)
+            session.flush()
+            return SystemUserModel.from_orm(db_user)
 
     @staticmethod
-    def update_scenario(model: ScenarioModel) -> None:
+    def get_user_by_credits(login: str, password: SecretStr | None = None) -> SystemUserModel | None:
         with db.create_session() as session:
-            scenario: db.Scenario = session.query(db.Scenario).get(model.id)
-            if scenario is None:
-                raise ScenarioNotExistsError(f"Scenario with id={model.id} does not exist!")
-            scenario.text = model.text
+            query = session.query(db.UserRole).filter(db.UserRole.login == login)
+            if password is not None:
+                query = query.filter(db.UserRole.password == password.get_secret_value())
+            db_user = query.one_or_none()
+            if db_user is not None:
+                return SystemUserModel.from_orm(db_user)
+            return None
 
     @staticmethod
-    def create_scenario(model: ScenarioModel) -> int:
+    def update_user_role(user_model: SystemUserModel) -> None:
         with db.create_session() as session:
-            scenario = db.Scenario(feature_id=model.feature_id, text=model.text)  # type: ignore
-            session.add(scenario)
-            session.flush()
-            return cast(int, scenario.id)
+            session.execute(sa.update(db.UserRole).where(db.UserRole.id == user_model.id).values(role=user_model.role))
```

### Comparing `overhave-3.9.0/overhave/storage/system_user_group_storage.py` & `overhave-4.0.0/overhave/storage/system_user_group_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import abc
-from typing import List
 
 from overhave import db
 
 
 class ISystemUserGroupStorage(abc.ABC):
     """Abstract class for system user storage."""
 
     @staticmethod
     @abc.abstractmethod
-    def has_any_group(user_groups: List[str]) -> bool:
+    def has_any_group(user_groups: list[str]) -> bool:
         pass
 
 
 class SystemUserGroupStorage(ISystemUserGroupStorage):
     """Class for system user storage."""
 
     @staticmethod
-    def has_any_group(user_groups: List[str]) -> bool:
+    def has_any_group(user_groups: list[str]) -> bool:
         with db.create_session() as session:
             group = session.query(db.GroupRole).filter(db.GroupRole.group.in_(user_groups)).first()
             return group is not None
```

### Comparing `overhave-3.9.0/overhave/storage/test_user_storage.py` & `overhave-4.0.0/overhave/storage/test_user_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
-from typing import List, Optional, cast
+
+import sqlalchemy.orm as so
 
 from overhave import db
 from overhave.storage import TestUserModel, TestUserSpecification
 from overhave.utils import get_current_time
 
 
 class BaseTestUserStorageException(Exception):
@@ -23,30 +24,33 @@
 
 
 class ITestUserStorage(abc.ABC):
     """Abstract class for Test User storage."""
 
     @staticmethod
     @abc.abstractmethod
-    def get_test_user_by_id(user_id: int) -> Optional[TestUserModel]:
+    def get_test_user_by_id(user_id: int) -> TestUserModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def get_test_user_by_name(name: str) -> Optional[TestUserModel]:
+    def get_test_user_by_key(key: str) -> TestUserModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def get_test_users(feature_type_id: int, allow_update: bool) -> List[TestUserModel]:
+    def get_test_users_by_feature_type_name(
+        session: so.Session, feature_type_id: int, allow_update: bool
+    ) -> list[TestUserModel]:
         pass
 
     @staticmethod
     @abc.abstractmethod
     def create_test_user(
+        key: str,
         name: str,
         specification: TestUserSpecification,
         created_by: str,
         feature_type_id: int,
         allow_update: bool,
     ) -> TestUserModel:
         pass
@@ -62,71 +66,74 @@
         pass
 
 
 class TestUserStorage(ITestUserStorage):
     """Class for Test User storage."""
 
     @staticmethod
-    def get_test_user_by_id(user_id: int) -> Optional[TestUserModel]:
+    def get_test_user_by_id(user_id: int) -> TestUserModel | None:
         with db.create_session() as session:
-            user: Optional[db.TestUser] = session.query(db.TestUser).get(user_id)
+            user = session.get(db.TestUser, user_id)
             if user is not None:
-                return cast(TestUserModel, TestUserModel.from_orm(user))
+                return TestUserModel.from_orm(user)
             return None
 
     @staticmethod
-    def get_test_user_by_name(name: str) -> Optional[TestUserModel]:
+    def get_test_user_by_key(key: str) -> TestUserModel | None:
         with db.create_session() as session:
-            user: Optional[db.TestUser] = session.query(db.TestUser).filter(db.TestUser.name == name).one_or_none()
+            user: db.TestUser | None = session.query(db.TestUser).filter(db.TestUser.key == key).one_or_none()
             if user is not None:
-                return cast(TestUserModel, TestUserModel.from_orm(user))
+                return TestUserModel.from_orm(user)
             return None
 
     @staticmethod
-    def get_test_users(feature_type_id: int, allow_update: bool) -> List[TestUserModel]:
-        with db.create_session() as session:
-            db_users: List[db.TestUser] = (
-                session.query(db.TestUser)
-                .filter(db.TestUser.feature_type_id == feature_type_id, db.TestUser.allow_update == allow_update)
-                .all()
-            )
-            return [cast(TestUserModel, TestUserModel.from_orm(user)) for user in db_users]
+    def get_test_users_by_feature_type_name(
+        session: so.Session, feature_type_id: int, allow_update: bool
+    ) -> list[TestUserModel]:
+        db_users = (
+            session.query(db.TestUser)
+            .filter(db.TestUser.feature_type_id == feature_type_id, db.TestUser.allow_update.is_(allow_update))
+            .all()
+        )
+        return [TestUserModel.from_orm(user) for user in db_users]
 
     @staticmethod
     def create_test_user(
+        key: str,
         name: str,
         specification: TestUserSpecification,
         created_by: str,
         feature_type_id: int,
         allow_update: bool,
     ) -> TestUserModel:
         with db.create_session() as session:
-            test_user = db.TestUser(  # type: ignore
+            test_user = db.TestUser(
+                key=key,
                 name=name,
                 specification=specification,
                 feature_type_id=feature_type_id,
                 created_by=created_by,
                 allow_update=allow_update,
                 changed_at=get_current_time(),
             )
             session.add(test_user)
             session.flush()
-            return cast(TestUserModel, TestUserModel.from_orm(test_user))
+            return TestUserModel.from_orm(test_user)
 
     @staticmethod
     def update_test_user_specification(user_id: int, specification: TestUserSpecification) -> None:
         with db.create_session() as session:
-            test_user = session.query(db.TestUser).get(user_id)
+            test_user = session.get(db.TestUser, user_id)
             if test_user is None:
                 raise TestUserDoesNotExistError(f"Test user with id {user_id} does not exist!")
             if not test_user.allow_update:
                 raise TestUserUpdatingNotAllowedError(f"Test user updating with id {user_id} not allowed!")
             test_user.specification = specification
             test_user.changed_at = get_current_time()
 
     @staticmethod
     def delete_test_user(user_id: int) -> None:
         with db.create_session() as session:
-            user: Optional[db.TestUser] = session.query(db.TestUser).get(user_id)
+            user = session.get(db.TestUser, user_id)
             if user is None:
                 raise TestUserDoesNotExistError(f"Test user with id {user_id} does not exist!")
             session.delete(user)
```

### Comparing `overhave-3.9.0/overhave/synchronization/storage_manager.py` & `overhave-4.0.0/overhave/synchronization/storage_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
 from datetime import datetime
-from typing import List, Optional
+
+import sqlalchemy.orm as so
+from pydantic import parse_obj_as
 
 from overhave.scenario import StrictFeatureInfo
 from overhave.storage import (
     FeatureModel,
     FeatureTypeModel,
     FeatureTypeName,
     IDraftStorage,
@@ -44,44 +46,42 @@
         self._feature_storage = feature_storage
         self._feature_type_storage = feature_type_storage
         self._scenario_storage = scenario_storage
         self._tag_storage = tag_storage
         self._draft_storage = draft_storage
         self._system_user_storage = system_user_storage
 
-    def get_feature(self, feature_id: int) -> Optional[FeatureModel]:
-        return self._feature_storage.get_feature(feature_id)
+    def get_feature(self, feature_id: int) -> FeatureModel | None:
+        return self._feature_storage.get_feature_model(feature_id)
 
     def get_last_change_time(self, model: FeatureModel) -> datetime:
-        draft_models = self._draft_storage.get_drafts_by_feature_id(model.id)
-        if draft_models:
-            logger.info("Feature has got drafts.")
-            last_published_draft = draft_models[-1]
-            if last_published_draft.published_at is not None:
-                logger.info(
-                    "Last version has been published at %s.",
-                    last_published_draft.published_at.strftime("%d-%m-%Y %H:%M:%S"),
-                )
-                return last_published_draft.published_at
+        last_draft_published_at = self._draft_storage.get_last_published_at_for_feature(model.id)
+        if last_draft_published_at is not None:
+            logger.info(
+                "Last version has been published at %s.",
+                last_draft_published_at.strftime("%d-%m-%Y %H:%M:%S"),
+            )
+            return last_draft_published_at
         logger.info("Feature hasn't got any published version.")
         return model.last_edited_at
 
-    def get_feature_tags(self, info: StrictFeatureInfo) -> List[TagModel]:
-        tags: List[TagModel] = []
-        if info.tags is not None:
-            for tag in info.tags:
-                tag_model = self._tag_storage.get_or_create_tag(value=tag, created_by=info.last_edited_by)
-                tags.append(tag_model)
-        return tags
-
-    def get_feature_type(self, feature_type: FeatureTypeName) -> FeatureTypeModel:
-        return self._feature_type_storage.get_feature_type_by_name(feature_type)
+    def get_feature_tags(self, session: so.Session, info: StrictFeatureInfo) -> list[TagModel]:
+        db_tags = [
+            self._tag_storage.get_or_create_tag(session=session, value=tag, created_by=info.last_edited_by)
+            for tag in info.tags
+        ]
+        session.flush()
+        return parse_obj_as(list[TagModel], db_tags)
+
+    def feature_type_by_name(self, session: so.Session, feature_type: FeatureTypeName) -> FeatureTypeModel:
+        db_feature_type = self._feature_type_storage.feature_type_by_name(session=session, name=feature_type)
+        return FeatureTypeModel.from_orm(db_feature_type)
 
     def ensure_users_exist(self, info: StrictFeatureInfo) -> None:
-        for user in (x for x in {info.author, info.last_edited_by} if x):
+        for user in {info.author, info.last_edited_by}:
             if self._system_user_storage.get_user_by_credits(login=user) is not None:
                 continue
             raise FeatureInfoUserNotFoundError(f"Could not find user with login={user}!")
 
     def update_db_feature(self, model: FeatureModel, scenario: str) -> None:
         scenario_model = self._scenario_storage.get_scenario_by_feature_id(model.id)
         self._feature_storage.update_feature(model)
```

### Comparing `overhave-3.9.0/overhave/synchronization/synchronizer.py` & `overhave-4.0.0/overhave/synchronization/synchronizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 from datetime import datetime
 from pathlib import Path
 from typing import cast
 
 import allure
 import pytz
 
+from overhave import db
 from overhave.entities import BaseFileExtractor, FeatureExtractor, GitRepositoryInitializer, OverhaveFileSettings
 from overhave.scenario import FeatureInfo, NullableFeatureIdError, ScenarioParser, StrictFeatureInfo
 from overhave.storage import FeatureModel
 from overhave.synchronization.abstract import IOverhaveSynchronizer
 from overhave.synchronization.storage_manager import SynchronizerStorageManager
+from overhave.utils import ANY_INT, get_current_time
 
 logger = logging.getLogger(__name__)
 
 
 class BaseOverhaveSynchronizerException(Exception):
     """Base exception for :class:`OverhaveSynchronizer`."""
 
@@ -49,15 +51,16 @@
         self._git_initializer = git_initializer
         self._storage_manager = storage_manager
 
     def _update_feature(self, model: FeatureModel, info: StrictFeatureInfo, file_ts: datetime) -> None:
         logger.info("Feature is gonna be updated...")
         self._storage_manager.ensure_users_exist(info)
         model.name = info.name
-        model.feature_tags = self._storage_manager.get_feature_tags(info=info)
+        with db.create_session() as session:
+            model.feature_tags = self._storage_manager.get_feature_tags(session=session, info=info)
         model.severity = info.severity
         model.last_edited_by = info.last_edited_by
         model.last_edited_at = file_ts
         model.task = info.tasks
         self._storage_manager.update_db_feature(model=model, scenario=info.scenarios)
         logger.info("Feature has been updated successfully.")
 
@@ -65,36 +68,43 @@
         logger.info("Feature is gonna be created...")
         if info.name is None:
             raise NullableInfoNameError("Feature info has not got feature name!")
         if info.type is None:
             raise NullableInfoFeatureTypeError("Could not create feature without feature type!")
         if info.author is None:
             raise NullableInfoAuthorError("Could not create feature without author!")
-        self._storage_manager.ensure_users_exist(info)  # type: ignore
-        feature_tags = self._storage_manager.get_feature_tags(info=info)  # type: ignore
-        feature_type = self._storage_manager.get_feature_type(info.type)
         if info.last_edited_by is None:
             info.last_edited_by = info.author
+
+        info.id = ANY_INT
+        strict_info = StrictFeatureInfo(**info.dict())
+        self._storage_manager.ensure_users_exist(strict_info)
+
+        with db.create_session() as session:
+            feature_tags = self._storage_manager.get_feature_tags(session=session, info=strict_info)
+            feature_type = self._storage_manager.feature_type_by_name(session=session, feature_type=strict_info.type)
+
         feature_model = FeatureModel(
-            id=0,
-            name=info.name,
-            author=info.author,
+            id=strict_info.id,
+            created_at=get_current_time(),
+            name=strict_info.name,
+            author=strict_info.author,
             type_id=feature_type.id,
-            last_edited_by=info.last_edited_by,
-            last_edited_at=info.last_edited_at,
-            task=info.tasks or [],
+            last_edited_by=strict_info.last_edited_by,
+            last_edited_at=strict_info.last_edited_at,
+            task=strict_info.tasks or [],
             file_path=file.relative_to(
                 self._feature_extractor.feature_type_to_dir_mapping[feature_type.name]
             ).as_posix(),
             released=True,
             feature_type=feature_type,
             feature_tags=feature_tags,
-            severity=info.severity or allure.severity_level.NORMAL,
+            severity=strict_info.severity or allure.severity_level.NORMAL,
         )
-        self._storage_manager.create_db_feature(model=feature_model, scenario=info.scenarios)  # type: ignore
+        self._storage_manager.create_db_feature(model=feature_model, scenario=strict_info.scenarios)
         logger.info("Feature with ID=%s has been created successfully.", feature_model.id)
 
     def synchronize(self, create_db_features: bool = False, pull_repository: bool = False) -> None:  # noqa: C901
         if pull_repository:
             self._git_initializer.pull()
         logger.info("Start synchronization...")
         all_features = self._extract_recursively(self._file_settings.features_dir)
```

### Comparing `overhave-3.9.0/overhave/test_execution/executor.py` & `overhave-4.0.0/overhave/test_execution/executor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import abc
 import logging
 import tempfile
 from pathlib import Path
 
+from overhave import db
 from overhave.db import TestRunStatus
 from overhave.entities import OverhaveFileSettings, ReportManager
+from overhave.metrics import TestRunOverhaveMetricContainer
 from overhave.scenario import FileManager
 from overhave.storage import IFeatureStorage, IScenarioStorage, ITestRunStorage, TestExecutorContext
 from overhave.test_execution.test_runner import PytestRunner
 from overhave.transport import TestRunTask
 
 logger = logging.getLogger(__name__)
 
@@ -21,70 +23,55 @@
         pass
 
     @abc.abstractmethod
     def process_test_task(self, task: TestRunTask) -> None:
         pass
 
 
-class BaseTestExecutionException(Exception):
-    """Base exception for :class:`TestExecutionManager`."""
-
-
-class FeatureNotExistsError(BaseTestExecutionException):
-    """Exception for situation with not existing Feature."""
-
-
-class TestRunNotExistsError(BaseTestExecutionException):
-    """Exception for situation with not existing TestRun."""
-
-
-class ScenarioNotExistsError(BaseTestExecutionException):
-    """Exception for situation with not existing Scenario."""
-
-
 class TestExecutor(ITestExecutor):
     """Class for test execution."""
 
     def __init__(
         self,
         file_settings: OverhaveFileSettings,
         feature_storage: IFeatureStorage,
         scenario_storage: IScenarioStorage,
         test_run_storage: ITestRunStorage,
         file_manager: FileManager,
         test_runner: PytestRunner,
         report_manager: ReportManager,
+        metric_container: TestRunOverhaveMetricContainer,
     ):
         self._file_settings = file_settings
         self._feature_storage = feature_storage
         self._scenario_storage = scenario_storage
         self._test_run_storage = test_run_storage
         self._file_manager = file_manager
         self._test_runner = test_runner
         self._report_manager = report_manager
+        self._metric_container = metric_container
 
     def _run_test(self, context: TestExecutorContext, alluredir: Path) -> int:
         with self._file_manager.tmp_feature_file(context=context) as feature_file:
             with self._file_manager.tmp_fixture_file(context=context, feature_file=feature_file) as fixture_file:
                 return self._test_runner.run(fixture_file=fixture_file.name, alluredir=alluredir.as_posix())
 
     def _compile_context(self, test_run_id: int) -> TestExecutorContext:
-        test_run = self._test_run_storage.get_test_run(test_run_id)
-        if test_run is None:
-            raise TestRunNotExistsError(f"TestRun with id={test_run_id} does not exist!")
-        scenario = self._scenario_storage.get_scenario(test_run.scenario_id)
-        if scenario is None:
-            raise ScenarioNotExistsError(f"Scenario with id={test_run.scenario_id} does not exist!")
-        feature = self._feature_storage.get_feature(scenario.feature_id)
-        if feature is None:
-            raise FeatureNotExistsError(f"Feature with id={scenario.feature_id} does not exist!")
+        with db.create_session() as session:
+            test_run_model = self._test_run_storage.testrun_model_by_id(session=session, run_id=test_run_id)
+            scenario_model = self._scenario_storage.scenario_model_by_id(
+                session=session, scenario_id=test_run_model.scenario_id
+            )
+            feature_model = self._feature_storage.feature_model_by_id(
+                session=session, feature_id=scenario_model.feature_id
+            )
         return TestExecutorContext(
-            feature=feature,
-            scenario=scenario,
-            test_run=test_run,
+            feature=feature_model,
+            scenario=scenario_model,
+            test_run=test_run_model,
         )
 
     def execute_test(self, test_run_id: int) -> None:
         self._test_run_storage.set_run_status(run_id=test_run_id, status=TestRunStatus.RUNNING)
         ctx = self._compile_context(test_run_id)
 
         results_dir = Path(tempfile.mkdtemp())
@@ -92,20 +79,23 @@
         try:
             test_return_code = self._run_test(context=ctx, alluredir=results_dir)
         except Exception as e:
             logger.exception("Error!")
             self._test_run_storage.set_run_status(
                 run_id=test_run_id, status=TestRunStatus.INTERNAL_ERROR, traceback=str(e)
             )
+            self._metric_container.add_test_run_status(status=TestRunStatus.INTERNAL_ERROR.value)
             return
 
         logger.debug("Test returncode: %s", test_return_code)
         if test_return_code == 0:
             self._test_run_storage.set_run_status(run_id=test_run_id, status=TestRunStatus.SUCCESS)
+            self._metric_container.add_test_run_status(status=TestRunStatus.SUCCESS.value)
         else:
             self._test_run_storage.set_run_status(
                 run_id=test_run_id, status=TestRunStatus.FAILED, traceback="Test run failed!"
             )
+            self._metric_container.add_test_run_status(status=TestRunStatus.FAILED.value)
         self._report_manager.create_allure_report(test_run_id=test_run_id, results_dir=results_dir)
 
     def process_test_task(self, task: TestRunTask) -> None:
         self.execute_test(test_run_id=task.data.test_run_id)
```

### Comparing `overhave-3.9.0/overhave/test_execution/settings.py` & `overhave-4.0.0/overhave/test_execution/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,49 @@
-from typing import Optional
-
+import httpx
 from pydantic import validator
-from yarl import URL
 
 from overhave.base_settings import BaseOverhavePrefix
 from overhave.utils import make_url
 
 
 class EmptyOverhaveAdminURLError(ValueError):
     """Exception for situation with empty ````admin_url``` while trying to ```get_feature_url```."""
 
 
 class OverhaveAdminLinkSettings(BaseOverhavePrefix):
     """Settings for dynamic links to Overhave Admin in Allure report."""
 
-    admin_url: Optional[URL]
+    admin_url: httpx.URL | None
 
     feature_id_filter_path: str = "feature/?flt2_0={feature_id}"
     feature_id_placeholder: str = "Overhave feature #{feature_id}"
 
     @validator("admin_url", pre=True)
-    def make_admin_url(cls, v: Optional[str]) -> Optional[URL]:
+    def make_admin_url(cls, v: str | None) -> httpx.URL | None:
         return make_url(v)
 
     @property
     def enabled(self) -> bool:
         return self.admin_url is not None
 
-    def get_feature_url(self, feature_id: int) -> str:
-        if isinstance(self.admin_url, URL):
-            return self.admin_url.human_repr() + f"/{self.feature_id_filter_path.format(feature_id=feature_id)}"
+    def get_feature_url(self, feature_id: int) -> httpx.URL:
+        if isinstance(self.admin_url, httpx.URL):
+            return httpx.URL(f"{self.admin_url}/{self.feature_id_filter_path.format(feature_id=feature_id)}")
         raise EmptyOverhaveAdminURLError("Overhave admin URL is None, so could not create link URL!")
 
     def get_feature_link_name(self, feature_id: int) -> str:
         return self.feature_id_placeholder.format(feature_id=feature_id)
 
 
 class OverhaveTestSettings(BaseOverhavePrefix):
     """Settings for PytestRunner, which runs scenario tests with specified addoptions."""
 
     default_pytest_addoptions: str = "--disable-warnings"
-    extra_pytest_addoptions: Optional[str]
+    extra_pytest_addoptions: str | None
+
+    workers: int | None  # Number of xdist workers, `None` by default
+
+
+class OverhaveStepCollectorSettings(BaseOverhavePrefix):
+    """Settings for StepCollector, which collect BDD steps for Overhave Admin UI."""
 
-    workers: Optional[int]  # Number of xdist workers, `None` by default
+    hide_non_public_steps: bool = False
```

### Comparing `overhave-3.9.0/overhave/test_execution/step_collector.py` & `overhave-4.0.0/overhave/test_execution/step_collector.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from operator import attrgetter
-from typing import Any, Dict, List, Optional, Tuple, cast
+from typing import Any, cast
 
 from _pytest.fixtures import FixtureDef
 from _pytest.main import Session
 
 from overhave.entities import StepPrefixesModel
 from overhave.storage import FeatureTypeName
-from overhave.test_execution.objects import BddStepModel
+from overhave.test_execution.objects import BddStepModel, is_public_step
+from overhave.test_execution.settings import OverhaveStepCollectorSettings
 
 _PYTESTBDD_FIXTURE_MARK = "pytestbdd_"
 _PYTESTBDD_FIXTURE_TRACE_MARK = "_trace"
 
 logger = logging.getLogger(__name__)
 
 
@@ -22,72 +23,77 @@
 class BddStepWithoutDocsError(BaseStepCollectorException):
     """Error for situation when pytest_bdd steps declared without docstring."""
 
 
 class StepCollector:
     """Class for `pytest-bdd` steps dynamic collection."""
 
-    def __init__(self, step_prefixes: Optional[StepPrefixesModel]) -> None:
+    def __init__(self, settings: OverhaveStepCollectorSettings, step_prefixes: StepPrefixesModel | None) -> None:
+        self._settings = settings
         self._step_prefixes = step_prefixes
-        self._steps: Dict[FeatureTypeName, List[BddStepModel]] = {}
+        self._steps: dict[FeatureTypeName, list[BddStepModel]] = {}
 
-    @staticmethod
-    def _is_bdd_step(fixture: FixtureDef[Any]) -> bool:
+    def _is_bdd_step(self, fixture: FixtureDef[Any]) -> bool:
         is_bdd_step = (
             isinstance(fixture.argname, str)
             and fixture.argname.startswith(_PYTESTBDD_FIXTURE_MARK)
             and not fixture.argname.endswith(_PYTESTBDD_FIXTURE_TRACE_MARK)
         )
         logger.debug("Fixture: %s - is_bdd_step=%s", fixture.argname, is_bdd_step)
-        if is_bdd_step and not isinstance(fixture.func.__doc__, str):
+        if not is_bdd_step:
+            return False
+        step_func = fixture.func._pytest_bdd_step_context.step_func  # type: ignore[union-attr]
+        if self._settings.hide_non_public_steps and not is_public_step(step_func):
+            logger.debug("Step func: %s is not public! Mark as non bdd step.", step_func)
+            return False
+        if not isinstance(step_func.__doc__, str):
             raise BddStepWithoutDocsError(
                 f"Fixture {fixture} does not have description! Please, set it via docstrings."
             )
-        return is_bdd_step
+        return True
 
-    @classmethod
-    def _get_pytestbdd_step_fixtures(cls, session: Session) -> Tuple[FixtureDef[Any]]:
+    def _get_pytestbdd_step_fixtures(self, session: Session) -> tuple[FixtureDef[Any], ...]:
         return cast(
-            Tuple[FixtureDef[Any]],
+            tuple[FixtureDef[Any], ...],
             sorted(
                 (
                     fx
                     for fx_list in session._fixturemanager._arg2fixturedefs.values()
                     for fx in fx_list
-                    if cls._is_bdd_step(fx)
+                    if self._is_bdd_step(fx)
                 ),
-                key=attrgetter("func.step_type"),
+                key=attrgetter("func._pytest_bdd_step_context.type"),
                 reverse=True,
             ),
         )
 
     def _compile_full_step_name(self, fixture_name: str, step_type: str) -> str:
         prefix = step_type.title()
         if self._step_prefixes is not None:
             prefix = self._step_prefixes.dict()[step_type.upper()].strip()
         return f"{prefix} {fixture_name}"
 
-    def _compile_step_models(self, steps: Tuple[FixtureDef[Any]]) -> List[BddStepModel]:
+    def _compile_step_models(self, steps: tuple[FixtureDef[Any], ...]) -> list[BddStepModel]:
         return [
             BddStepModel(
-                type=f.func.step_type,  # type: ignore
+                type=f.func._pytest_bdd_step_context.type,  # type: ignore
                 name=self._compile_full_step_name(
-                    fixture_name=f.func._pytest_bdd_parsers[0].name,  # type: ignore
-                    step_type=f.func.step_type,  # type: ignore
+                    fixture_name=f.func._pytest_bdd_step_context.parser.name,  # type: ignore
+                    step_type=f.func._pytest_bdd_step_context.type,  # type: ignore
                 ),
-                doc=f.func.__doc__,
+                doc=f.func._pytest_bdd_step_context.step_func.__doc__,  # type: ignore
             )
             for f in steps
         ]
 
     def collect_steps(self, session: Session, feature_type: FeatureTypeName) -> None:
         logger.debug("Collecting steps for feature_type=%s...", feature_type)
         step_fixtures = self._get_pytestbdd_step_fixtures(session)
         bdd_steps = self._compile_step_models(step_fixtures)
         if bdd_steps:
             logger.debug("Loaded steps dict:\n%s", bdd_steps)
         else:
             logger.warning("Feature type '%s' does not have any pytest_bdd steps!", feature_type)
         self._steps[feature_type] = bdd_steps
 
-    def get_steps(self, feature_type: FeatureTypeName) -> Optional[List[BddStepModel]]:
+    def get_steps(self, feature_type: FeatureTypeName) -> list[BddStepModel] | None:
         return self._steps.get(feature_type)
```

### Comparing `overhave-3.9.0/overhave/test_execution/test_runner.py` & `overhave-4.0.0/overhave/test_execution/test_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 import logging
 from pathlib import Path
-from typing import List, Optional
 
 import pytest
 
 from overhave.test_execution.settings import OverhaveTestSettings
 
 logger = logging.getLogger(__name__)
 
 
+def _extend_cmd_args(cmd: list[str], addoptions: str | None) -> None:
+    if not isinstance(addoptions, str):
+        return
+    cmd.extend(addoptions.split(" "))
+
+
 class PytestRunner:
     """Class for running `PyTest` in test and collect-only modes."""
 
     def __init__(self, settings: OverhaveTestSettings) -> None:
         self._settings = settings
 
-    @staticmethod
-    def _extend_cmd_args(cmd: List[str], addoptions: Optional[str]) -> None:
-        if not isinstance(addoptions, str):
-            return
-        cmd.extend(addoptions.split(" "))
-
     def run(self, fixture_file: str, alluredir: str) -> int:
         pytest_cmd = [fixture_file, f"--alluredir={alluredir}"]
         for addoptions in (self._settings.default_pytest_addoptions, self._settings.extra_pytest_addoptions):
-            self._extend_cmd_args(cmd=pytest_cmd, addoptions=addoptions)
+            _extend_cmd_args(cmd=pytest_cmd, addoptions=addoptions)
         if self._settings.workers is not None:
             pytest_cmd.extend(["-n", f"{self._settings.workers}"])
 
         logger.debug("Prepared pytest args: %s", pytest_cmd)
         return pytest.main(pytest_cmd)
 
     def collect_only(self, fixture_file: Path) -> None:
         logger.info("Started tests collection process with '%s'...", fixture_file.name)
-        pytest_cmd = [
+        pytest_cmd = [  # pylint: disable=W8301
             fixture_file.as_posix(),
             "--collect-only",
             "--disable-pytest-warnings",
         ]
-        self._extend_cmd_args(cmd=pytest_cmd, addoptions=self._settings.extra_pytest_addoptions)
+        _extend_cmd_args(cmd=pytest_cmd, addoptions=self._settings.extra_pytest_addoptions)
         logger.debug("Prepared pytest args: %s", pytest_cmd)
         pytest.main(pytest_cmd)
         logger.info("Finished tests collection process with '%s'.", fixture_file.name)
```

### Comparing `overhave-3.9.0/overhave/transport/http/__init__.py` & `overhave-4.0.0/overhave/transport/http/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # flake8: noqa
 from .api_client import OverhaveApiAuthenticator, OverhaveApiAuthenticatorSettings
 from .base_client import BaseHttpClient, BaseHttpClientSettings, BearerAuth
 from .gitlab_client import (
     GitlabHttpClient,
-    GitlabHttpClientConflictError,
     GitlabMrCreationResponse,
     GitlabMrRequest,
     GitlabRepository,
     OverhaveGitlabClientSettings,
 )
 from .stash_client import (
     OverhaveStashClientSettings,
```

### Comparing `overhave-3.9.0/overhave/transport/http/api_client/authenticator.py` & `overhave-4.0.0/overhave/transport/http/api_client/authenticator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Optional
 
 from pydantic.types import SecretStr
 
 from overhave.storage import AuthStorage, AuthToken
 from overhave.transport.http.api_client.models import TokenRequestData
 from overhave.transport.http.api_client.settings import OverhaveApiAuthenticatorSettings
 from overhave.transport.http.base_client import BaseHttpClient, BearerAuth, HttpMethod
@@ -29,15 +28,15 @@
             method=HttpMethod.POST,
             url=self._settings.get_auth_token_url,
             data=data.dict(by_alias=True),
         )
         return AuthToken.parse_obj(response.json())
 
     def _get_auth_token(self, username: str, password: SecretStr) -> AuthToken:
-        token: Optional[AuthToken] = self._auth_storage.get_auth_token(username=username)
+        token: AuthToken | None = self._auth_storage.get_auth_token(username=username)
         if token is None:
             token = self._auth_by_credentials(username=username, password=password)
             self._auth_storage.update_auth_token(username=username, new_auth_token=token)
         return token
 
     def get_bearer_auth(self, username: str, password: SecretStr) -> BearerAuth:
         token = self._get_auth_token(username=username, password=password)
```

### Comparing `overhave-3.9.0/overhave/transport/http/base_client/client.py` & `overhave-4.0.0/overhave/transport/http/base_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import logging
-from json import JSONDecodeError
-from typing import Any, Dict, Generic, Mapping, Optional, Union, cast
+from typing import Any, Generic, Mapping, cast
 
-import requests
+import httpx
 import tenacity
 from pydantic import BaseModel, ValidationError
 from pydantic.main import ModelMetaclass
-from requests.auth import AuthBase
-from yarl import URL
 
 from overhave.transport.http.base_client.objects import HttpMethod
 from overhave.transport.http.base_client.settings import HttpSettingsType
 
 logger = logging.getLogger(__name__)
 
 
@@ -26,43 +23,43 @@
 class BaseHttpClient(Generic[HttpSettingsType]):
     """Base client for HTTP communications."""
 
     def __init__(self, settings: HttpSettingsType) -> None:
         self._settings = settings
 
     @staticmethod
-    def _parse_or_raise(response: requests.Response, model: ModelMetaclass) -> BaseModel:
+    def _parse_or_raise(response: httpx.Response, model: ModelMetaclass) -> BaseModel:
         try:
             return cast(BaseModel, model).parse_obj(response.json())
-        except (ValueError, ValidationError, JSONDecodeError) as e:
+        except (ValueError, ValidationError) as e:
             url = getattr(response, "raw_url", response.url)
             raise HttpClientValidationError(f'Response validation error for "{url}"') from e
 
     @tenacity.retry(
         reraise=True,
-        retry=tenacity.retry_if_exception_type(requests.ConnectionError),
+        retry=tenacity.retry_if_exception_type(httpx.ConnectError),
         stop=tenacity.stop_after_attempt(3),
         before_sleep=tenacity.before_sleep_log(logger, logger.level),
         after=tenacity.after_log(logger, logger.level),
     )
     def _make_request(
         self,
         method: HttpMethod,
-        url: URL,
-        params: Optional[Dict[str, Any]] = None,
-        json: Optional[Dict[str, Any]] = None,
-        data: Optional[Union[str, bytes, Mapping[Any, Any]]] = None,
-        auth: Optional[AuthBase] = None,
+        url: httpx.URL,
+        params: dict[str, Any] | None = None,
+        json: dict[str, Any] | None = None,
+        data: str | bytes | Mapping[Any, Any] | None = None,
+        auth: httpx.Auth | None = None,
         raise_for_status: bool = True,
-    ) -> requests.Response:
-        response = requests.request(
-            method=method.value,
-            url=url.human_repr(),
+    ) -> httpx.Response:
+        response = httpx.request(
+            method=str(method.value),
+            url=str(url),
             params=params,
             json=json,
-            data=data,
+            data=data,  # type: ignore
             auth=auth,
             timeout=self._settings.timeout,
         )
         if raise_for_status:
             response.raise_for_status()
         return response
```

### Comparing `overhave-3.9.0/overhave/transport/http/gitlab_client/utils.py` & `overhave-4.0.0/overhave/transport/http/gitlab_client/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import gitlab
+import httpx
 
 from overhave.transport.http.gitlab_client.objects import TokenType
 
 
 class InvalidTokenTypeError(Exception):
     """Error for choosing invalid token type value."""
 
 
-def get_gitlab_python_client(url: str, token_type: TokenType, token: str) -> gitlab.Gitlab:
+def get_gitlab_python_client(url: httpx.URL, token_type: TokenType, token: str) -> gitlab.Gitlab:
     if token_type is TokenType.OAUTH:
-        return gitlab.Gitlab(url, oauth_token=token)
+        return gitlab.Gitlab(str(url), oauth_token=token)
     if token_type is TokenType.PRIVATE:
-        return gitlab.Gitlab(url, private_token=token)
+        return gitlab.Gitlab(str(url), private_token=token)
     if token_type is TokenType.JOB:
-        return gitlab.Gitlab(url, private_token=token)
+        return gitlab.Gitlab(str(url), private_token=token)
     raise InvalidTokenTypeError(
         f"Please, verify your token type! {token_type} not in {[TokenType.OAUTH, TokenType.JOB, TokenType.PRIVATE]}"
     )
```

### Comparing `overhave-3.9.0/overhave/transport/http/stash_client/client.py` & `overhave-4.0.0/overhave/transport/http/stash_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-3.9.0/overhave/transport/http/stash_client/models.py` & `overhave-4.0.0/overhave/transport/http/stash_client/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Dict, Final, List, Optional, Union
+from typing import Final
 
 from pydantic import BaseModel, Field, validator
 
 
 class StashProject(BaseModel):
     """Model for Stash pull-request project slug."""
 
@@ -39,42 +39,42 @@
 
     user: StashReviewerInfo
 
 
 class StashBasicPrInfo(BaseModel):
     """Model for Stash basic pull-request information."""
 
-    title: Optional[str]
+    title: str | None
     open: bool
 
 
 class StashPrRequest(StashBasicPrInfo):
     """Model for Stash pull-request request."""
 
     description: str
     state: str = "OPEN"
     closed: bool = False
     source_branch: StashBranch = Field(..., alias="fromRef")
     target_branch: StashBranch = Field(..., alias="toRef")
     locked: bool = False
     close_source_branch: bool = True
-    reviewers: List[StashReviewer]
+    reviewers: list[StashReviewer]
 
 
-StashLinksType = Dict[str, List[Dict[str, str]]]
+StashLinksType = dict[str, list[dict[str, str]]]
 
 
 class StashPrCreationResponse(StashBasicPrInfo):
     """Model for Stash pull-request creation response."""
 
     created_date: datetime = Field(..., alias="createdDate")
     updated_date: datetime = Field(..., alias="updatedDate")
-    pull_request_url: Optional[str]
-    traceback: Optional[Exception]
-    links: Optional[StashLinksType]
+    pull_request_url: str | None
+    traceback: Exception | None
+    links: StashLinksType | None
 
     class Config:
         arbitrary_types_allowed = True
 
     def get_pr_url(self) -> str:
         if isinstance(self.pull_request_url, str):
             return self.pull_request_url
@@ -82,28 +82,28 @@
             return self.links["self"][0]["href"]
         raise RuntimeError("Could not get pull-request URL from response!")
 
 
 class StashRequestError(BaseModel):
     """Model for Stash request error."""
 
-    context: Optional[str]
+    context: str | None
     message: str
     exception_name: str = Field(..., alias="exceptionName")
 
 
 class StashErrorResponse(BaseModel):
     """Model for Stash error response."""
 
-    errors: List[StashRequestError]
+    errors: list[StashRequestError]
 
     @property
     def duplicate(self) -> bool:
         for error in self.errors:
             if not error.exception_name.endswith("DuplicatePullRequestException"):
                 continue
             return True
         return False
 
 
-AnyStashResponseModel = Union[StashPrCreationResponse, StashErrorResponse]
+AnyStashResponseModel = StashPrCreationResponse | StashErrorResponse
 STASH_RESPONSE_MODELS: Final = [StashPrCreationResponse, StashErrorResponse]
```

### Comparing `overhave-3.9.0/overhave/transport/http/stash_client/settings.py` & `overhave-4.0.0/overhave/transport/http/stash_client/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from yarl import URL
+import httpx
 
 from overhave.transport.http.base_client import BaseHttpClientSettings
 
 
 class OverhaveStashClientSettings(BaseHttpClientSettings):
     """Settings for :class:`StashHttpClient`."""
 
     pr_path: str = "rest/api/1.0/projects/{project_key}/repos/{repository_name}/pull-requests"
     auth_token: str
 
     class Config:
         env_prefix = "OVERHAVE_STASH_"
 
-    def get_pr_url(self, project_key: str, repository_name: str) -> URL:
-        return self.url / self.pr_path.format(project_key=project_key, repository_name=repository_name)
+    def get_pr_url(self, project_key: str, repository_name: str) -> httpx.URL:
+        return httpx.URL(f"{self.url}/{self.pr_path.format(project_key=project_key, repository_name=repository_name)}")
```

### Comparing `overhave-3.9.0/overhave/transport/ldap/authenticator.py` & `overhave-4.0.0/overhave/transport/ldap/authenticator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import re
-from typing import List, Optional
 
 import ldap
 from ldap.ldapobject import LDAPObject
 from pydantic import SecretStr
 
 from overhave.transport.ldap.settings import OverhaveLdapClientSettings
 
@@ -12,25 +11,25 @@
 
 
 class LDAPAuthenticator:
     """Class-client for LDAP authentication."""
 
     def __init__(self, settings: OverhaveLdapClientSettings) -> None:
         self._settings = settings
-        self._ldap_connection: Optional[LDAPObject] = None
+        self._ldap_connection: LDAPObject | None = None
 
     def _connect(self, login: str, password: SecretStr) -> None:
         ldap_connection = ldap.initialize(self._settings.url)
         ldap_connection.set_option(ldap.OPT_REFERRALS, 0)
         ldap_connection.set_option(ldap.OPT_NETWORK_TIMEOUT, self._settings.timeout.seconds)
         ldap_connection.simple_bind_s(f"{self._settings.domain}{login}", password.get_secret_value())
 
         self._ldap_connection = ldap_connection
 
-    def _ask_ad_usergroups(self, login: str) -> List[str]:
+    def _ask_ad_usergroups(self, login: str) -> list[str]:
         result = self._ldap_connection.search_st(  # type: ignore
             base=self._settings.dn,
             scope=ldap.SCOPE_SUBTREE,
             filterstr=f"(sAMAccountName={login})",
             attrlist=["memberOf"],
             timeout=self._settings.timeout.seconds,
         )
@@ -39,15 +38,15 @@
 
         p = re.compile("CN=(.*?),", re.IGNORECASE)
         return [
             p.match(x).group(1)  # type: ignore
             for x in list(filter(lambda x: "OU=Security Groups" in x or "OU=Mail Groups" in x, member_of))
         ]
 
-    def get_user_groups(self, login: str, password: SecretStr) -> Optional[List[str]]:
+    def get_user_groups(self, login: str, password: SecretStr) -> list[str] | None:
         try:
             self._connect(login, password)
         except ldap.INVALID_CREDENTIALS:
             logger.info("Failed LDAP auth_managers for user: %s", login)
             return None
 
         return self._ask_ad_usergroups(login)
```

### Comparing `overhave-3.9.0/overhave/transport/redis/consumer.py` & `overhave-4.0.0/overhave/transport/redis/consumer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,60 @@
 import logging
 from types import TracebackType
-from typing import Iterator, List, Sequence, Type
+from typing import Iterator, Sequence
 
 import walrus
 
-from overhave.entities.settings import OverhaveRedisSettings
+from overhave.metrics import BaseOverhaveMetricContainer
 from overhave.transport.redis.objects import RedisPendingData, RedisStream, RedisUnreadData
-from overhave.transport.redis.template import RedisTemplate
+from overhave.transport.redis.settings import BaseRedisSettings
 
 logger = logging.getLogger(__name__)
 
 
-class RedisConsumer(RedisTemplate):
+class RedisConsumer:
     """Class for consuming tasks from Redis stream ```stream_name```."""
 
-    def __init__(self, settings: OverhaveRedisSettings, stream_name: RedisStream):
-        super().__init__(settings)
+    def __init__(
+        self,
+        settings: BaseRedisSettings,
+        stream_name: RedisStream,
+        database: walrus.Database,
+        metric_container: BaseOverhaveMetricContainer,
+    ):
+        self._settings = settings
         self._stream_name = stream_name
+        self._database = database
+        self._metric_container = metric_container
 
     @property
     def _consumer_group(self) -> walrus.ConsumerGroup:
         consumer_group = self._database.consumer_group(f"cg-{self._stream_name}", (self._stream_name,))
         consumer_group.create()
         return consumer_group
 
     @property
     def _stream(self) -> walrus.containers.ConsumerGroupStream:
         return getattr(self._consumer_group, self._stream_name.with_dunder)
 
     def _clean_pending(self) -> None:
         pending_messages = self._stream.pending()
-        models: List[RedisPendingData] = [RedisPendingData.parse_obj(msg) for msg in pending_messages]
+        models: list[RedisPendingData] = [RedisPendingData.parse_obj(msg) for msg in pending_messages]
         if models:
             message_ids = [x.message_id for x in models]
             self._stream.claim(*message_ids)
             self._stream.ack(*message_ids)
             logger.info("Clean all pending messages for stream %s: %s", self._stream_name, models)
 
     def _consume(self) -> Sequence[RedisUnreadData]:
-        messages = self._stream.read(count=self._settings.redis_read_count, block=self._settings.timeout_milliseconds)
-        objects: List[RedisUnreadData] = []
+        messages = self._stream.read(count=self._settings.read_count, block=self._settings.timeout_milliseconds)
+        objects: list[RedisUnreadData] = []
         for msg in messages:
             data = RedisUnreadData(*msg)
-            logger.info("Message from redis: %s", data)
+            logger.debug("Message from redis: %s", data)
             self._stream.ack(data.message_id)
             objects.append(data)
         return objects
 
     def __enter__(self) -> None:
         logger.info("Starting consuming from %s...", self._stream_name)
         self._clean_pending()
@@ -54,15 +62,16 @@
     def __iter__(self) -> Iterator[Sequence[RedisUnreadData]]:
         while True:
             try:
                 logger.debug("Check messages...")
                 messages = self._consume()
                 if messages:
                     logger.debug("Has messages, return them")
+                    self._metric_container.consume_redis_task(task_type=self._stream_name.value)
                     yield messages
                 continue
             except Exception:
                 logger.exception("Error while trying to consume message from redis!")
             raise StopIteration()
 
-    def __exit__(self, exc_type: Type[Exception], exc_val: Exception, exc_tb: TracebackType) -> None:
+    def __exit__(self, exc_type: type[Exception], exc_val: Exception, exc_tb: TracebackType) -> None:
         pass
```

### Comparing `overhave-3.9.0/overhave/transport/redis/objects.py` & `overhave-4.0.0/overhave/transport/redis/objects.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import abc
 import enum
 import json
-from typing import Any, Dict, TypeVar, Union
+from typing import Any, TypeVar
 
 from pydantic.main import BaseModel
 
 
-class RedisStream(str, enum.Enum):
+class RedisStream(enum.StrEnum):
     """Enum that declares Redis streams."""
 
     TEST = "test"
     PUBLICATION = "publication"
     EMULATION = "emulation"
 
     @property
     def with_dunder(self) -> str:
         return self.value.replace("-", "_")
 
 
 class _IRedisTask(BaseModel, abc.ABC):
     @property
     @abc.abstractmethod
-    def message(self) -> Dict[bytes, bytes]:
+    def message(self) -> dict[bytes, bytes]:
         pass
 
 
 class BaseRedisTask(_IRedisTask):
     """Base task for Redis streams."""
 
     data: Any
 
     @property
-    def message(self) -> Dict[bytes, bytes]:
+    def message(self) -> dict[bytes, bytes]:
         return {b"data": self.data.json().encode("utf-8")}
 
 
 class TestRunData(BaseModel):
     """Specific data for test run."""
 
     __test__ = False
@@ -72,37 +72,40 @@
 class EmulationTask(BaseRedisTask):
     """Redis stream task for emulation run."""
 
     data: EmulationData
 
 
 TRedisTask = TypeVar("TRedisTask", TestRunTask, EmulationTask, PublicationTask, covariant=True)
-AnyRedisTask = Union[TestRunTask, PublicationTask, EmulationTask]
+AnyRedisTask = TestRunTask | PublicationTask | EmulationTask
 
 
 class RedisPendingData(BaseModel):
     """Class that describes pending data from Redis stream."""
 
     message_id: str
     consumer: str
     time_since_delivered: int
     times_delivered: int
 
 
 class RedisUnreadData:
     """Class for unread data from Redis stream."""
 
-    def __init__(self, message_id: bytes, message: Dict[bytes, bytes]) -> None:
+    def __init__(self, message_id: bytes, message: dict[bytes, bytes]) -> None:
         self.message_id = message_id.decode()
         self.message = message
 
     @property
-    def decoded_message(self) -> Dict[str, Any]:
+    def decoded_message(self) -> dict[str, Any]:
         return {key.decode(): json.loads(value.decode("utf-8")) for key, value in self.message.items()}
 
+    def __str__(self) -> str:
+        return f"{RedisUnreadData.__name__}(id={self.message_id}, message='{self.message}')"
+
 
 class RedisContainer(BaseModel):
     """Class for parsing instance of :class:`RedisUnreadData` from Redis stream.
 
     ```task``` will be parsed to one of declared models.
     """
```

### Comparing `overhave-3.9.0/overhave/transport/redis/producer.py` & `overhave-4.0.0/overhave/transport/redis/producer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 import logging
-from typing import Dict, Type
 
 import redis
+import walrus
 
-from overhave.entities.settings import OverhaveRedisSettings
+from overhave.metrics import BaseOverhaveMetricContainer
 from overhave.transport.redis.objects import BaseRedisTask, RedisStream
-from overhave.transport.redis.template import RedisTemplate
+from overhave.transport.redis.settings import BaseRedisSettings
 
 logger = logging.getLogger(__name__)
 
 
-class RedisProducer(RedisTemplate):
+class RedisProducer:
     """Class for producing tasks.
 
     Producer send tasks into Redis stream specified by ```mapping``.
     """
 
-    def __init__(self, settings: OverhaveRedisSettings, mapping: Dict[Type[BaseRedisTask], RedisStream]):
-        super().__init__(settings)
-        self._streams = {task: self._database.Stream(stream.value) for task, stream in mapping.items()}
+    def __init__(
+        self,
+        settings: BaseRedisSettings,
+        mapping: dict[type[BaseRedisTask], RedisStream],
+        database: walrus.Database,
+        metric_container: BaseOverhaveMetricContainer,
+    ):
+        self._settings = settings
+        self._streams = {task: database.Stream(stream.value) for task, stream in mapping.items()}
+        self._mapping = mapping
+        self._metric_container = metric_container
 
     def add_task(self, task: BaseRedisTask) -> bool:
         stream = self._streams[type(task)]
         logger.info("Added Redis task %s", task)
         try:
             stream.add(task.message)
+            self._metric_container.produce_redis_task(task_type=self._mapping[type(task)].value)
             return True
         except redis.exceptions.ConnectionError:
             logger.exception("Could not add %s to Redis!", type(task).__name__)
             return False
```

### Comparing `overhave-3.9.0/overhave/transport/redis/runner.py` & `overhave-4.0.0/overhave/transport/redis/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Callable, Dict, Type
+from typing import Callable
 
 from overhave.transport.redis.consumer import RedisConsumer
 from overhave.transport.redis.objects import AnyRedisTask, RedisContainer, RedisUnreadData
 
 logger = logging.getLogger(__name__)
 
 
@@ -16,15 +16,15 @@
 class RedisConsumerRunner:
     """Class for running tasks specified by ```mapping```.
 
     Runner tasks launch with instance of :class:`RedisConsumer` ```consumer```.
     """
 
     def __init__(
-        self, consumer: RedisConsumer, mapping: Dict[Type[AnyRedisTask], Callable[[AnyRedisTask], None]]
+        self, consumer: RedisConsumer, mapping: dict[type[AnyRedisTask], Callable[[AnyRedisTask], None]]
     ) -> None:
         self._consumer = consumer
         self._mapping = mapping
 
     def run(self) -> None:
         try:
             self._run()
```

### Comparing `overhave-3.9.0/overhave/transport/s3/manager.py` & `overhave-4.0.0/overhave/transport/s3/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 from datetime import timedelta
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable
 
 import boto3
 import botocore.exceptions
+import httpx
 import urllib3
 from boto3_type_annotations.s3 import Client
 from pydantic.tools import parse_obj_as
-from yarl import URL
 
 from overhave.transport.s3.models import BucketModel, DeletionResultModel, ObjectModel
 from overhave.transport.s3.objects import OverhaveS3Bucket
 from overhave.transport.s3.settings import OverhaveS3ManagerSettings
 from overhave.utils import make_url
 
 logger = logging.getLogger(__name__)
@@ -44,15 +44,15 @@
 
 class EmptyObjectsListError(BaseS3ManagerException):
     """Exception for situation with empty object list."""
 
 
 def _s3_error(msg: str):  # type: ignore
     def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
-        def wrapper(*args: Any, **kwargs: Dict[str, Any]) -> Any:
+        def wrapper(*args: Any, **kwargs: dict[str, Any]) -> Any:
             try:
                 return func(*args, **kwargs)
             except botocore.exceptions.ClientError as e:
                 raise ClientError(msg) from e
 
         return wrapper
 
@@ -60,15 +60,15 @@
 
 
 class S3Manager:
     """Class for s3 management with boto3 client."""
 
     def __init__(self, settings: OverhaveS3ManagerSettings):
         self._settings = settings
-        self._client: Optional[Client] = None
+        self._client: Client | None = None
 
     def initialize(self) -> None:
         if not self._settings.enabled:
             logger.info("S3Manager disabled and has not been initialized.")
             return
         self._client = self._get_client(self._settings)
         if self._settings.autocreate_buckets:
@@ -107,50 +107,50 @@
             raise UndefinedClientException("s3 client has not been initialized!")
         return self._client
 
     def _ensure_buckets_exists(self) -> None:
         remote_buckets = self._get_buckets()
         logger.info("Existing remote s3 buckets: %s", remote_buckets)
         bucket_names = [model.name for model in remote_buckets]
-        for bucket in list(filter(lambda x: x.value not in bucket_names, OverhaveS3Bucket)):
+        for bucket in list(filter(lambda x: x.value not in bucket_names, list(OverhaveS3Bucket))):
             self.create_bucket(bucket.value)
         logger.info("Successfully ensured existence of Overhave service buckets.")
 
     @_s3_error(msg="Error while getting buckets list!")
-    def _get_buckets(self) -> List[BucketModel]:
+    def _get_buckets(self) -> list[BucketModel]:
         response = self._ensured_client.list_buckets()
-        return parse_obj_as(List[BucketModel], response.get("Buckets"))
+        return parse_obj_as(list[BucketModel], response.get("Buckets"))
 
     @_s3_error(msg="Error while creating bucket!")
     def create_bucket(self, bucket: str) -> None:
         logger.info("Creating bucket %s...", bucket)
-        kwargs: Dict[str, Any] = {"Bucket": bucket}
+        kwargs: dict[str, Any] = {"Bucket": bucket}
         if isinstance(self._settings.region_name, str):
             kwargs["CreateBucketConfiguration"] = {"LocationConstraint": self._settings.region_name}
         self._ensured_client.create_bucket(**kwargs)
         logger.info("Bucket %s successfully created.", bucket)
 
     def upload_file(self, file: Path, bucket: OverhaveS3Bucket) -> bool:
         logger.info("Start uploading file '%s'...", file.name)
         try:
-            self._ensured_client.upload_file(file.as_posix(), bucket.value, file.name)
+            self._ensured_client.upload_file(file.as_posix(), str(bucket.value), file.name)
             logger.info("File '%s' successfully uploaded", file.name)
             return True
         except botocore.exceptions.ClientError:
             logger.exception("Could not upload file to s3 cloud!")
             return False
 
     @_s3_error(msg="Error while getting bucket objects list!")
-    def get_bucket_objects(self, bucket: str) -> List[ObjectModel]:
+    def get_bucket_objects(self, bucket: str) -> list[ObjectModel]:
         response = self._ensured_client.list_objects(Bucket=bucket)
         logger.debug("List objects response:\n%s", response)
-        return parse_obj_as(List[ObjectModel], response.get("Contents"))
+        return parse_obj_as(list[ObjectModel], response.get("Contents"))
 
     @_s3_error(msg="Error while deleting bucket objects!")
-    def delete_bucket_objects(self, bucket: str, objects: List[ObjectModel]) -> DeletionResultModel:
+    def delete_bucket_objects(self, bucket: str, objects: list[ObjectModel]) -> DeletionResultModel:
         if not objects:
             raise EmptyObjectsListError("No one object specified for deletion!")
         logger.info("Deleting items %s...", [obj.name for obj in objects])
         response = self._ensured_client.delete_objects(
             Bucket=bucket,
             Delete={"Objects": [{"Key": obj.name} for obj in objects]},
         )
@@ -184,15 +184,15 @@
             )
             logger.info("File '%s' successfully downloaded", filename)
             return True
         except botocore.exceptions.ClientError:
             logger.exception("Could not download file from s3 cloud!")
             return False
 
-    def create_presigned_url(self, bucket: str, object_name: str, expiration: timedelta) -> Optional[URL]:
+    def create_presigned_url(self, bucket: str, object_name: str, expiration: timedelta) -> httpx.URL | None:
         try:
             response = self._ensured_client.generate_presigned_url(
                 "get_object", Params={"Bucket": bucket, "Key": object_name}, ExpiresIn=int(expiration.total_seconds())
             )
             logger.info("Created presigned URL: '%s'", response)
             return make_url(response)
         except botocore.exceptions.ClientError:
```

### Comparing `overhave-3.9.0/overhave/transport/s3/models.py` & `overhave-4.0.0/overhave/transport/s3/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 from pydantic import Extra, Field, root_validator
 from pydantic.main import BaseModel
 
 
 class BucketModel(BaseModel):
     """Model for boto3 client Bucket."""
@@ -33,38 +33,38 @@
         extra = Extra.allow
 
 
 class BaseObjectToDeletionModel(BaseModel):
     """Base model for boto3 client object deletion result."""
 
     name: str = Field(alias="Key")
-    etag: Optional[str] = Field(alias="VersionId")
+    etag: str | None = Field(alias="VersionId")
 
 
 class DeletedObjectModel(BaseObjectToDeletionModel):
     """Model for boto3 client deleted object."""
 
-    marker: Optional[bool] = Field(alias="DeleteMarker")
-    marker_id: Optional[bool] = Field(alias="DeleteMarkerVersionId")
+    marker: bool | None = Field(alias="DeleteMarker")
+    marker_id: bool | None = Field(alias="DeleteMarkerVersionId")
 
 
 class NotDeletedObjectModel(BaseObjectToDeletionModel):
     """Model for boto3 client not deleted object."""
 
     code: str = Field(alias="Code")
     message: str = Field(alias="Message")
 
 
 class DeletionResultModel(BaseModel):
     """Model for boto3 client objects deletion result."""
 
-    deleted: Optional[List[DeletedObjectModel]] = Field(alias="Deleted")
-    errors: Optional[List[NotDeletedObjectModel]] = Field(alias="Errors")
-    requester: Optional[str] = Field(alias="RequestCharged")
+    deleted: list[DeletedObjectModel] | None = Field(alias="Deleted")
+    errors: list[NotDeletedObjectModel] | None = Field(alias="Errors")
+    requester: str | None = Field(alias="RequestCharged")
 
     @root_validator(pre=True)
-    def validate_results(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+    def validate_results(cls, values: dict[str, Any]) -> dict[str, Any]:
         deleted = values.get("Deleted")
         errors = values.get("Errors")
         if deleted is None and errors is None:
             raise ValueError("At least one result field should be presented!")
         return values
```

### Comparing `overhave-3.9.0/overhave/transport/s3/settings.py` & `overhave-4.0.0/overhave/transport/s3/settings.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Any, Dict, Optional
+from typing import Any
 
 from pydantic import BaseSettings, root_validator
 
 
 class OverhaveS3ManagerSettings(BaseSettings):
     """Settings for S3Client."""
 
     enabled: bool = False
 
-    url: Optional[str]
-    region_name: Optional[str]
-    access_key: Optional[str]
-    secret_key: Optional[str]
+    url: str | None
+    region_name: str | None
+    access_key: str | None
+    secret_key: str | None
     verify: bool = True
 
     autocreate_buckets: bool = False
 
     class Config:
         env_prefix = "OVERHAVE_S3_"
 
     @root_validator
-    def validate_enabling(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+    def validate_enabling(cls, values: dict[str, Any]) -> dict[str, Any]:
         enabled = values.get("enabled")
         if enabled and not all(
             (
                 isinstance(values.get("url"), str),
                 isinstance(values.get("access_key"), str),
                 isinstance(values.get("secret_key"), str),
             )
```

### Comparing `overhave-3.9.0/pyproject.toml` & `overhave-4.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,99 @@
 [tool.poetry]
 name = "overhave"
-version = "3.9.0"
+version = "4.0.0"
 description = "Overhave - web-framework for BDD"
 readme = "README.rst"
 authors = [
     "Vladislav Mukhamatnurov <livestreamepidemz@yandex.ru>",
     "Tinkoff Backend Dialog System Team <bds-dev@tinkoff.ru>"
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Testing :: BDD",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
     "Framework :: Flask",
     "Framework :: Pytest",
 ]
 
 [tool.poetry.scripts]
 overhave = 'overhave.cli:overhave'
 overhave-demo = 'demo:overhave_demo'
 
 [tool.poetry.plugins.pytest11]
 overhave = "overhave.pytest_plugin.plugin"
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-sqlalchemy = ">=1.3.23"
+python = ">=3.8,<3.12"
 psycopg2-binary = "^2.8"
 pydantic = ">=1.7"
-requests = ">=2.0.0"
 tenacity = "*"
 yarl = ">=1.1.1"
 pytz = "*"
 flask-admin = ">=1.5"
 WTForms = ">=2.2"
-Flask-WTF = ">=0.14.2"
 python-ldap = "^3.2"
 ldap3 = "^2.6"
 wsgi_intercept = "^1.8"
 redis = "^4.2.0"
-walrus = "^0.8.0"
 docker = "*"
-sqlalchemy-utc = "^0.14.0"
-httptools = "^0.1.1"
+httptools = "^0.5.0"
 python-dateutil = "^2.8.1"
 alembic = "^1.4.3"
 boto3 = "^1.17.16"
 boto3-type-annotations = "^0.3.1"
-SQLAlchemy-Utils = "^0.38.0"
-Flask = "^2.0.1"
 GitPython = "^3.1.15"
 python-gitlab = "^2.9.0"
-pydantic-sqlalchemy = "^0.0.9"
 fastapi = ">=0.57.0"
-typer = "^0.4.0"
-Flask-Login = "^0.6.0"
 python-jose = "^3.3.0"
 python-multipart = "^0.0.5"
 aiofiles = "^0.8.0"
+httpx = "^0.23.0"
+walrus = "^0.9.2"
+typer = "^0.7.0"
+flask-login = "^0.6.2"
+flask-wtf = "^1.1.1"
+flask = "^2.3.2"
+sqlalchemy = ">=1.4"
+sqlalchemy-utils = "^0.41.1"
+sqlalchemy-utc = "^0.14.0"
+prometheus-client = "^0.17.0"
 
-
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 flake8-awesome = "<1.3"
 requests_mock = "*"
 flake8-docstrings = "^1.5"
 pytest-faker = "^2.0"
 filelock = "*"
 pytest-cov = "^2.10.1"
 pytest-deadfixtures = "^2.2.1"
 pytest-random-order = "^1.0.4"
-tox = "^3.24.4"
-twine = "^3.3.0"
-Sphinx = "^4.4.0"
-mypy-extensions = "^0.4.3"
 alchemy-mock = "^0.4.3"
 coverage = {version = "^6.0.1", extras = ["toml"]}
 pytest-mock = "^3.6.1"
-pytest = "^6.2.5"
 allure-pytest = "^2.9.45"
 pytest-xdist = "^2.5.0"
 uvicorn = "^0.17.5"
 black = "^22.1.0"
 coverage-badge = "^1.1.0"
 pytest-bdd = "^6.0.1"
-mypy = "^0.971"
+docutils-stubs = "^0.0.22"
+pytest-redis = "^2.4.0"
+perflint = "^0.7.3"
+pytest = "^6.2.5"
+sphinx = "^7.0.0"
+mypy = "^1.3.0"
+tox = "^4.5.1"
+twine = "^4.0.2"
 
 [tool.pytest.ini_options]
 addopts = "-l -v --random-order-bucket=module --random-order-seed=$RANDOM -p no:overhave"
 testpaths = "tests"
 python_files = ["test_*.py"]
 python_classes = ["*Test", "Test*"]
 python_functions = ["test_*"]
@@ -116,32 +115,35 @@
 default_section = "THIRDPARTY"
 include_trailing_comma = true
 known_first_party = ["docker", "docs", "overhave", "tests", "demo"]
 line_length = 120
 multi_line_output = 3
 
 [tool.black]
-target-version = ['py310']
+target-version = ['py311']
 line-length = 120
 
 [build-system]
-requires = ["poetry>=1.1.8"]
+requires = ["poetry>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
 isolated_build_env = .package
-envlist = py310
+envlist = py311
 [testenv]
-whitelist_externals =
+allowlist_externals =
     make
 venv = {toxworkdir}/{[tox]isolated_build_env}
 setenv =
     VENV = {[testenv]venv}
     WORK_DIR = {toxworkdir}
 passenv =
     OVERHAVE_DB_URL
+    OVERHAVE_REDIS_URL
+    OVERHAVE_REDIS_SENTINEL_URLS
+    PACKAGE_BUILD_DIR
 commands =
     make check
 """
```

### Comparing `overhave-3.9.0/setup.py` & `overhave-4.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,115 +1,724 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: overhave
+Version: 4.0.0
+Summary: Overhave - web-framework for BDD
+Author: Vladislav Mukhamatnurov
+Author-email: livestreamepidemz@yandex.ru
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Flask
+Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: Software Development :: Testing :: BDD
+Requires-Dist: GitPython (>=3.1.15,<4.0.0)
+Requires-Dist: WTForms (>=2.2)
+Requires-Dist: aiofiles (>=0.8.0,<0.9.0)
+Requires-Dist: alembic (>=1.4.3,<2.0.0)
+Requires-Dist: boto3 (>=1.17.16,<2.0.0)
+Requires-Dist: boto3-type-annotations (>=0.3.1,<0.4.0)
+Requires-Dist: docker
+Requires-Dist: fastapi (>=0.57.0)
+Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: flask-admin (>=1.5)
+Requires-Dist: flask-login (>=0.6.2,<0.7.0)
+Requires-Dist: flask-wtf (>=1.1.1,<2.0.0)
+Requires-Dist: httptools (>=0.5.0,<0.6.0)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: ldap3 (>=2.6,<3.0)
+Requires-Dist: prometheus-client (>=0.17.0,<0.18.0)
+Requires-Dist: psycopg2-binary (>=2.8,<3.0)
+Requires-Dist: pydantic (>=1.7)
+Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
+Requires-Dist: python-gitlab (>=2.9.0,<3.0.0)
+Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: python-ldap (>=3.2,<4.0)
+Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
+Requires-Dist: pytz
+Requires-Dist: redis (>=4.2.0,<5.0.0)
+Requires-Dist: sqlalchemy (>=1.4)
+Requires-Dist: sqlalchemy-utc (>=0.14.0,<0.15.0)
+Requires-Dist: sqlalchemy-utils (>=0.41.1,<0.42.0)
+Requires-Dist: tenacity
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: walrus (>=0.9.2,<0.10.0)
+Requires-Dist: wsgi_intercept (>=1.8,<2.0)
+Requires-Dist: yarl (>=1.1.1)
+Description-Content-Type: text/x-rst
 
-packages = \
-['overhave',
- 'overhave.admin',
- 'overhave.admin.flask',
- 'overhave.admin.views',
- 'overhave.admin.views.formatters',
- 'overhave.admin.views.index',
- 'overhave.api',
- 'overhave.api.auth',
- 'overhave.api.views',
- 'overhave.cli',
- 'overhave.cli.db_cmds',
- 'overhave.db',
- 'overhave.emulation',
- 'overhave.entities',
- 'overhave.entities.auth_managers',
- 'overhave.entities.auth_managers.ldap',
- 'overhave.entities.feature',
- 'overhave.entities.language',
- 'overhave.entities.report_manager',
- 'overhave.extra',
- 'overhave.factory',
- 'overhave.factory.components',
- 'overhave.factory.context',
- 'overhave.publication',
- 'overhave.publication.gitlab',
- 'overhave.publication.gitlab.tokenizer',
- 'overhave.publication.stash',
- 'overhave.pytest_plugin',
- 'overhave.pytest_plugin.helpers',
- 'overhave.pytest_plugin.helpers.allure_utils',
- 'overhave.scenario',
- 'overhave.scenario.compiler',
- 'overhave.scenario.file_manager',
- 'overhave.scenario.parser',
- 'overhave.storage',
- 'overhave.synchronization',
- 'overhave.test_execution',
- 'overhave.transport',
- 'overhave.transport.http',
- 'overhave.transport.http.api_client',
- 'overhave.transport.http.base_client',
- 'overhave.transport.http.gitlab_client',
- 'overhave.transport.http.stash_client',
- 'overhave.transport.ldap',
- 'overhave.transport.redis',
- 'overhave.transport.s3',
- 'overhave.utils']
-
-package_data = \
-{'': ['*'],
- 'overhave.admin': ['files/*', 'files/ace-src/*', 'files/css/*', 'templates/*']}
-
-install_requires = \
-['Flask-Login>=0.6.0,<0.7.0',
- 'Flask-WTF>=0.14.2',
- 'Flask>=2.0.1,<3.0.0',
- 'GitPython>=3.1.15,<4.0.0',
- 'SQLAlchemy-Utils>=0.38.0,<0.39.0',
- 'WTForms>=2.2',
- 'aiofiles>=0.8.0,<0.9.0',
- 'alembic>=1.4.3,<2.0.0',
- 'boto3-type-annotations>=0.3.1,<0.4.0',
- 'boto3>=1.17.16,<2.0.0',
- 'docker',
- 'fastapi>=0.57.0',
- 'flask-admin>=1.5',
- 'httptools>=0.1.1,<0.2.0',
- 'ldap3>=2.6,<3.0',
- 'psycopg2-binary>=2.8,<3.0',
- 'pydantic-sqlalchemy>=0.0.9,<0.0.10',
- 'pydantic>=1.7',
- 'python-dateutil>=2.8.1,<3.0.0',
- 'python-gitlab>=2.9.0,<3.0.0',
- 'python-jose>=3.3.0,<4.0.0',
- 'python-ldap>=3.2,<4.0',
- 'python-multipart>=0.0.5,<0.0.6',
- 'pytz',
- 'redis>=4.2.0,<5.0.0',
- 'requests>=2.0.0',
- 'sqlalchemy-utc>=0.14.0,<0.15.0',
- 'sqlalchemy>=1.3.23',
- 'tenacity',
- 'typer>=0.4.0,<0.5.0',
- 'walrus>=0.8.0,<0.9.0',
- 'wsgi_intercept>=1.8,<2.0',
- 'yarl>=1.1.1']
-
-entry_points = \
-{'console_scripts': ['overhave = overhave.cli:overhave',
-                     'overhave-demo = demo:overhave_demo'],
- 'pytest11': ['overhave = overhave.pytest_plugin.plugin']}
-
-setup_kwargs = {
-    'name': 'overhave',
-    'version': '3.9.0',
-    'description': 'Overhave - web-framework for BDD',
-    'long_description': '========\nOverhave\n========\n\n.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/label_img.png\n  :width: 700\n  :align: center\n  :alt: Overhave framework\n\n  `Overhave`_ is the web-framework for BDD: scalable, configurable, easy to use, based on\n  `Flask Admin`_ and `Pydantic`_.\n\n  .. image:: https://github.com/TinkoffCreditSystems/overhave/workflows/CI/badge.svg\n    :target: https://github.com/TinkoffCreditSystems/overhave/actions?query=workflow%3ACI\n    :alt: CI\n\n  .. image:: https://img.shields.io/pypi/pyversions/overhave.svg\n    :target: https://pypi.org/project/overhave\n    :alt: Python versions\n\n  .. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/TinkoffCreditSystems/overhave\n    :alt: Code style\n\n  .. image:: https://img.shields.io/pypi/v/overhave?color=%2334D058&label=pypi%20package\n    :target: https://pypi.org/project/overhave\n    :alt: Package version\n\n  .. image:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/coverage.svg\n    :target: https://github.com/TinkoffCreditSystems/overhave\n    :alt: PyTest Coverage percent\n    \n  .. image:: https://img.shields.io/pypi/dm/overhave.svg\n    :target: https://pypi.org/project/overhave\n    :alt: Downloads per month\n\n--------\nFeatures\n--------\n\n* Ready web-interface for easy BDD features management with `Ace`_ editor\n* Traditional Gherkin format for scenarios provided by `pytest-bdd`_\n* Execution and reporting of BDD features based on `Allure`_\n* Auto-collection of `pytest-bdd`_ steps and display on web-interface\n* Simple scenarios structure, easy horizontal scaling\n* Built-in wrappers for `pytest-bdd`_ hooks to supplement `Allure`_ report\n* Ability to create and use several BDD keywords dictionary with different languages\n* Versioning and deployment of scenario drafts to `Bitbucket`_ or `GitLab`_\n* Synchronization between `git`_ repository and database with features\n* Built-in configurable access management of users and groups\n* Configurable strategy for user authorization (LDAP also provided)\n* Database schema based on `SQLAlchemy`_ models and works with PostgreSQL\n* Still configurable as `Flask Admin`_, supports plug-ins and extensions\n* Has built-in API application with Swagger docs, based on `FastAPI`_\n* Distributed `producer-consumer` architecture based on `Walrus`_ Redis streams\n* Command-line interface, provided with `Typer`_\n* Integrated interaction for files storage with s3-cloud based on `boto3`_\n* Web-browser emulation ability with custom toolkit (`GoTTY`_, for example)\n\n------------\nInstallation\n------------\n\nYou can install **Overhave** via pip from PyPI:\n\n.. code-block:: shell\n\n    pip install overhave\n\n--------\nOverview\n--------\n\nWeb-interface\n-------------\n\nThe web-interface is a basic tool for BDD features management. It consists of:\n\n* `Info` - index page with optional information about your tool or project;\n* `Scenarios` - section for features management, contains subsections\n    `Features`, `Test runs`, `Versions` and `Tags`:\n\n    * `Features`\n        gives an interface for features records management and provides info\n        about id, name author, time, editor and publishing status; it is possible\n        to search, edit or delete items through Script panel.\n\n        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/label_img.png\n          :width: 500\n          :align: center\n          :alt: Features list\n\n    * `Test runs`\n        gives an interface for test runs management and provides info about.\n\n        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/test_runs_img.png\n          :width: 500\n          :align: center\n          :alt: Test runs list\n\n    * Versions\n        contains feature versions in corresponding to test runs; versions contains PR-links to\n        the remote Git repository.\n\n        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/versions_img.png\n          :width: 500\n          :align: center\n          :alt: Feature published versions list\n\n    * Tags\n        contains tags values, which are used for feature\'s tagging.\n\n        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/tags_img.png\n          :width: 500\n          :align: center\n          :alt: Feature published versions list\n\n* `Test users` - section for viewing and configuring test users;\n* `Access` - section for access management, contains `Users` and\n    `Groups` subsections;\n* `Emulation` - experimental section for alternative tools implementation\n    (in development).\n\n**Overhave** features could be created and/or edited through special\n*script panel* in feature edit mode. Feature should have type registered by the\napplication, unique name, specified tasks list with the traditional format\n```PRJ-NUMBER``` and scenario text.\n\n**Script panel** has `pytest-bdd`_ steps table on the right side of interface.\nThese steps should be defined in appropriate fixture modules and registered\nat the application on start-up to be displayed.\n\n\n.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/panel_img.png\n  :width: 600\n  :align: center\n  :alt: Script panel\n\n  Example of **Overhave** script panel in feature edit mode\n\nAllure report\n-------------\n\n**Overhave** generates `Allure`_ report after tests execution in web-interface.\nIf you execute tests manually through `PyTest`_, these results are could be\nconverted into the `Allure`_ report also with the `Allure CLI`_ tool.\nThis report contains scenarios descriptions as they are described in features.\n\n.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/report_img.png\n  :width: 600\n  :align: center\n  :alt: Allure test-case report\n\n  Example of generated `Allure`_ report after execution of **Overhave**\'s feature\n\nDemo-mode (Quickstart)\n----------------------\n\n**Overhave** has special demo-mode (in development), which could be possibly\nused for framework demonstration and manual debugging / testing. The framework\nprovides a CLI entrypoints for easy server run in debug mode:\n\n.. code-block:: shell\n\n    make up  # start PostgreSQL database and Redis\n    overhave db create-all  # create Overhave database schema\n    overhave-demo admin  # start Overhave admin on port 8076 in debug mode\n    overhave-demo consumer -s test  # start Overhave test execution consumer\n\n**Note**: you could run admin in special mode, which does not require\nconsumers. This mode uses *threadpool* for running testing and publication\ntasks asynchronously:\n\n.. code-block:: shell\n\n    overhave-demo admin --threadpool --language=ru\n\nBut this *threadpool* mode is unscalable in *kubernetes* paradigm. So,\nit\'s highly recommended to use corresponding consumers exactly.\n\nCommand-line interface\n----------------------\n\n**Overhave** has a CLI that provides a simple way to start service web-interface,\nrun consumer and execute basic database operations. Examples are below:\n\n.. code-block:: shell\n\n    overhave db create-all\n    overhave admin --port 8080\n    overhave consumer -s publication\n    overhave api -p 8000 -w 4\n\n**Note**: service start-up takes a set of settings, so you can set them through\nvirtual environment with prefix ```OVERHAVE_```, for example ```OVERHAVE_DB_URL```.\nIf you want to configure settings in more explicit way through context injection,\nplease see next part of docs.\n\nContext injection\n-----------------\n\nContext setting\n^^^^^^^^^^^^^^^\n\nService could be configured via application context injection with prepared\ninstance of `OverhaveContext` object. This context could be set using\n```set_context``` function of initialized ```ProxyFactory``` instance.\n\nFor example, ```my_custom_context``` prepared. So, application start-up could\nbe realised with follow code:\n\n.. code-block:: python\n\n    from overhave import overhave_app, overhave_admin_factory\n\n    factory = overhave_admin_factory()\n    factory.set_context(my_custom_context)\n    overhave_app(factory).run(host=\'localhost\', port=8080, debug=True)\n\n**Note**:\n\n* ```overhave_app``` is the prepared `Flask` application with already enabled\n    Flask Admin and Login Manager plug-ins;\n* ```overhave_factory``` is a function for LRU cached instance of the **Overhave**\n    factory ```ProxyFactory```; the instance has an access to application components,\n    directly used in ```overhave_app```.\n* ```my_custom_context``` is an example of context configuration, see an\n    example code in `context_example.rst`_.\n\nEnabling of injection\n^^^^^^^^^^^^^^^^^^^^^\n\n**Overhave** has it\'s own built-in `PyTest`_ plugin, which is used to enable\nand configure injection of prepared context into application core instance.\nThe plugin provides one option:\n\n* `--enable-injection` - flag to enable context injection.\n\nThe `PyTest` usage should be similar to:\n\n.. code-block:: bash\n\n    pytest --enable-injection\n\nConsumers\n---------\n\n**Overhave** has `producer-consumer` architecture, based on Redis streams,\nand supported 3 consumer\'s types:\n\n* **TEST** - consumer for test execution with it\'s own factory\n    ```overhave_test_execution_factory```;\n\n* **PUBLICATION** - consumer for features publication with it\'s own factory\n    ```overhave_publication_factory```;\n\n* **EMULATION** - consumer for specific emulation with it\'s own factory\n    ```overhave_emulation_factory```.\n\n**Note**: the ```overhave_test_execution_factory``` has ability for context injection\nand could be enriched with the custom context as the ```overhave_admin_factory```.\n\nProject structure\n-----------------\n\n**Overhave** supports it\'s own special project structure:\n\n.. image:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/project_structure.png\n  :width: 300\n  :alt: **Overhave** project structure\n\nThe right approach is to create a **root directory** (like "demo" inside the current\nrepository) that contains **features**, **fixtures** and **steps** directories.\n\nThe **Features** directory contains different feature types as\nseparate directories, each of them corresponds to predefined `pytest-bdd`_\nset of steps.\n\nThe **Fixtures** directory contains typical `PyTest`_ modules splitted by different\nfeature types. These modules are used for `pytest-bdd`_ isolated test runs. It is\nnecessary because of special mechanism of `pytest-bdd`_ steps collection.\n\nThe **Steps** directory contains `pytest-bdd`_ steps packages splitted by differrent\nfeature types also. Each steps subdirectory has it\'s own declared steps in according\nto supported feature type.\n\nSo, it is possible to create your own horizontal structure of\ndifferent product directions with unique steps and `PyTest`_ fixtures.\n\n**Note**: this structure is used in **Overhave** application. The formed data\ngives a possibility to specify registered feature type in the web-interface\n*script panel*. Also, this structure defines which steps will be displayed in\nthe right side of *script panel*.\n\nFeature format\n--------------\n\n**Overhave** has it\'s own special feature\'s text format, which inherits\nGherkin from `pytest-bdd`_ with unique updates:\n\n* required tag that is related to existing feature type directory, where\n    current feature is located;\n* any amount of arbitrary tags;\n* severity tag - implements `Allure`_ severity to feature or just tagged\n    scenario (for example: ```@severity.blocker```);\n* info about feature - who is creator, last editor and publisher;\n* task tracker\'s tickets with format ```PRJ-1234```;\n\nAn example of filled feature content is located in\n`feature_example.rst`_.\n\nPytest markers\n--------------\n\n**Overhave** implements solution for `PyTest`_ markers usage with custom\nadditional information:\n\n* "`disabled`": same as `skip` marker, but it\'s necessary to setup reason;\n* "`xfail`": traditional `xfail` with strict reason presence.\n\nExamples:\n\n.. code-block:: gherkin\n\n    @disabled(not ready)\n    Feature: My business feature\n\n.. code-block:: gherkin\n\n    @disabled(TODO: https://tracker.myorg.com/browse/PRJ-333; deadline 01.01.25)\n    Scenario: Yet another business feature\n\n\n.. code-block:: gherkin\n\n    @xfail(bug: https://tracker.myorg.com/browse/PRJ-555)\n    Scenario outline: Other business feature\n\nIf reason contains URL, so **Overhave** will attach `Allure` link to report:\nfor `disabled` - it will be `LinkType.LINK`, for `xfail` - `LinkType.ISSUE`.\n\nFeature links\n-------------\n\n**Overhave** has ability to set links to it\'s own admin service in `Allure`_\ntest-cases. Link will be set automatically when you generate `Allure`_ report.\nThis function can be enabled via setup of environment variable\n```OVERHAVE_ADMIN_URL```:\n\n.. code-block:: bash\n\n    export OVERHAVE_ADMIN_URL=https://overhave-admin.myorg.com\n\nAlso, **Overhave** has ability to set links to feature file in `Git`_ repository.\nLink will be set automatically when you generate `Allure`_ report. This function\ncan be enabled via setup of environment variable\n```OVERHAVE_GIT_PROJECT_URL```:\n\n.. code-block:: bash\n\n    export OVERHAVE_GIT_PROJECT_URL=https://git.myorg.com/bdd-features-repo\n\n\nLanguage\n--------\n\nThe web-interface language is ENG by default and could not be switched\n(if it\'s necessary - please, create a ```feature request``` or contribute\nyourself).\n\nThe feature text as well as `pytest-bdd`_ BDD keywords are configurable\nwith **Overhave** extra models, for example RUS keywords are already defined\nin framework and available for usage:\n\n.. code-block:: python\n\n    from overhave.extra import RUSSIAN_PREFIXES\n\n    language_settings = OverhaveLanguageSettings(step_prefixes=RUSSIAN_PREFIXES)\n\n**Note**: you could create your own prefix-value mapping for your language:\n\n.. code-block:: python\n\n    from overhave import StepPrefixesModel\n\n    GERMAN_PREFIXES = StepPrefixesModel(\n        FEATURE="Merkmal:",\n        SCENARIO_OUTLINE="Szenarioübersicht:",\n        SCENARIO="Szenario:",\n        BACKGROUND="Hintergrund:",\n        EXAMPLES="Beispiele:",\n        EXAMPLES_VERTICAL="Beispiele: Vertikal",\n        GIVEN="Gegeben ",\n        WHEN="Wann ",\n        THEN="Dann ",\n        AND="Und ",\n        BUT="Aber ",\n    )\n\nGit integration\n---------------\n\n**Overhave** gives an ability to sent your new features or changes to\nremote git repository, which is hosted by `Bitbucket`_ or `GitLab`_.\nIntegration with bitbucket is native, while integration with GitLab\nuses `python-gitlab`_ library.\n\nYou are able to set necessary settings for your project:\n\n.. code-block:: python\n\n    publisher_settings = OverhaveGitlabPublisherSettings(\n        repository_id=\'123\',\n        default_target_branch_name=\'master\',\n    )\n    client_settings=OverhaveGitlabClientSettings(\n        url="https://gitlab.mycompany.com",\n        auth_token=os.environ.get("MY_GITLAB_AUTH_TOKEN"),\n    )\n\nThe pull-request (for Bitbucket) or merge-request (for GitLab)\ncreated when you click the button `Create pull request` on\ntest run result\'s page. This button is available only for `success`\ntest run\'s result.\n\n**Note**: one of the most popular cases of GitLab API\nauthentication is the OAUTH2 schema with service account.\nIn according to this schema, you should have OAUTH2 token,\nwhich is might have a short life-time and could not be\nspecified through environment. For this situation, **Overhave**\nhas special `TokenizerClient` with it\'s own\n`TokenizerClientSettings` - this simple client could take\nthe token from a remote custom GitLab tokenizer service.\n\nGit-to-DataBase synchronization\n-------------------------------\n\n**Overhave** gives an ability to synchronize your current `git`_\nrepository\'s state with database. It means that your features,\nwhich are located on the database, could be updated - and the source\nof updates is your repository.\n\n**For example**: you had to do bulk data replacement in `git`_\nrepository, and now you want to deliver changes to remote database.\nThis not so easy matter could be solved with **Overhave** special\ntooling:\n\nYou are able to set necessary settings for your project:\n\n.. code-block:: bash\n\n    overhave sync run  # only update existing features\n    overhave sync run --create-db-features  # update + create new features\n    overhave sync run --pull-repository  # pull git repo and run sync\n\nYou are able to test this tool with **Overhave** demo mode.\nBy default, 3 features are created in demo database. Just try\nto change them or create new features and run synchronization\ncommand - you will get the result.\n\n.. code-block:: bash\n\n    overhave-demo sync-run  # or with \'--create-db-features\'\n\n**Overhave** supports validation of existing feature files.\nCommand try to parse features and fill defined feature info format.\nIf there is any problem, special error will be thrown.\n\n.. code-block:: bash\n\n    overhave sync validate-features\n    overhave sync validate-features --raise-if-nullable-id\n    overhave sync validate-features --pull-repository\n\nAnd yes, your are able to try it with demo mode:\n\n.. code-block:: bash\n\n    overhave-demo validate-features\n    overhave sync validate-features -r  # --raise-if-nullable-id\n\nCustom index\n------------\n\n**Overhave** gives an ability to set custom index.html file for rendering. Path\nto file could be set through environment as well as set with context:\n\n.. code-block:: python\n\n    admin_settings = OverhaveAdminSettings(\n        index_template_path="/path/to/index.html"\n    )\n\nAuthorization strategy\n----------------------\n\n**Overhave** provides several authorization strategies, declared by\n```AuthorizationStrategy``` enum:\n\n* `Simple` - strategy without real authorization.\n    Each user could use preferred name. This name will be used for user\n    authority. Each user is unique. Password not required.\n\n* `Default` - strategy with real authorization.\n    Each user could use only registered credentials.\n\n* `LDAP` - strategy with authorization using remote LDAP server.\n    Each user should use his LDAP credentials. LDAP\n    server returns user groups. If user in default \'admin\' group or his groups\n    list contains admin group - user will be authorized. If user already placed\n    in database - user will be authorized too. No one password stores.\n\nAppropriate strategy and additional data should be placed into\n```OverhaveAuthorizationSettings```, for example LDAP strategy could be\nconfigured like this:\n\n.. code-block:: python\n\n    auth_settings = OverhaveAuthorizationSettings(auth_strategy=AuthorizationStrategy.LDAP)\n    ldap_manager_settings = OverhaveLdapManagerSettings(ldap_admin_group="admin")\n\nS3 cloud\n--------\n\n**Overhave** implements functionality for *s3* cloud interactions, such as\nbucket creation and deletion, files uploading, downloading and deletion.\nThe framework provides an ability to store reports and other files in\nthe remote s3 cloud storage. You could enrich your environment with following\nsettings:\n\n.. code-block:: shell\n\n    OVERHAVE_S3_ENABLED=true\n    OVERHAVE_S3_URL=https://s3.example.com\n    OVERHAVE_S3_ACCESS_KEY=<MY_ACCESS_KEY>\n    OVERHAVE_S3_SECRET_KEY=<MY_SECRET_KEY>\n\nOptionally, you could change default settings also:\n\n.. code-block:: shell\n\n    OVERHAVE_S3_VERIFY=false\n    OVERHAVE_S3_AUTOCREATE_BUCKETS=true\n\nThe framework with enabled ```OVERHAVE_S3_AUTOCREATE_BUCKETS``` flag will create\napplication buckets in remote storage if buckets don\'t exist.\n\nAPI\n---\n**Overhave** has it\'s own application programming interface, based on\n`FastAPI`_.\n\n.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/api_img.png\n  :width: 600\n  :align: center\n  :alt: Allure test-case report\n\n  **Overhave** openapi.json through `Swagger`_\n\nCurrent possibilities could be displayed through built-in\n`Swagger`_ - just run the API and open http://localhost:8000 in your\nbrowser.\n\n.. code-block:: bash\n\n    overhave api -p 8000\n\nInterface has authorization through `oauth2`_ scheme, so you should setup\n```OVERHAVE_API_AUTH_SECRET_KEY``` for usage.\n\nRight now, API implements types of resources:\n\n* `feature_tags`\n    get feature tag or get list of feature tags;\n* `features`\n    get features info by tag ID or tag value;\n* `test_users`\n    get test user info, specification, put new specification or delete\n    test user;\n* `test_runs`\n    get test run info or create test run with given parameters;\n* `emulations`\n    get emulation runs by test user id.\n\n------------\nContributing\n------------\n\nContributions are very welcome.\n\nPreparation\n-----------\n\nProject installation is very easy\nand takes just few prepared commands (`make pre-init` works only for Ubuntu;\nso you can install same packages for your OS manually):\n\n.. code-block:: shell\n\n    make pre-init\n    make init\n\nPackages management is provided by `Poetry`_.\n\nCheck\n-----\n\nTests can be run with `Tox`_. `Docker-compose`_ is used for other services\npreparation and serving, such as database. Simple tests and linters execution:\n\n.. code-block:: shell\n\n    make up\n    make test\n    make lint\n\nPlease, see `make` file and discover useful shortcuts. You could run tests\nin docker container also:\n\n.. code-block:: shell\n\n    make test-docker\n\nDocumentation build\n-------------------\n\nProject documentation could be built via `Sphinx`_ and simple `make` command:\n\n.. code-block:: shell\n\n    make build-docs\n\nBy default, the documentation will be built using `html` builder into `_build`\ndirectory.\n\n-------\nLicense\n-------\n\nDistributed under the terms of the `GNU GPLv2`_ license.\n\n------\nIssues\n------\n\nIf you encounter any problems, please report them here in section `Issues`\nwith a detailed description.\n\n.. _`Overhave`: https://github.com/TinkoffCreditSystems/overhave\n.. _`Pydantic`: https://github.com/samuelcolvin/pydantic\n.. _`Flask Admin`: https://github.com/flask-admin/flask-admin\n.. _`Ace`: https://github.com/ajaxorg/ace\n.. _`PyTest`: https://github.com/pytest-dev/pytest\n.. _`pytest-bdd`: https://github.com/pytest-dev/pytest-bdd\n.. _`Allure`: https://github.com/allure-framework/allure-python\n.. _`Allure CLI`: https://docs.qameta.io/allure/#_get_started\n.. _`Bitbucket`: https://www.atlassian.com/git\n.. _`GitLab`: https://about.gitlab.com\n.. _`python-gitlab`: https://python-gitlab.readthedocs.io\n.. _`SQLAlchemy`: https://github.com/sqlalchemy/sqlalchemy\n.. _`Walrus`: https://github.com/coleifer/walrus\n.. _`GoTTY`: https://github.com/yudai/gotty\n.. _`GNU GPLv2`: http://www.apache.org/licenses/LICENSE-2.0\n.. _`Tox`: https://github.com/tox-dev/tox\n.. _`Poetry`: https://github.com/python-poetry/poetry\n.. _`Docker-compose`: https://docs.docker.com/compose\n.. _`Typer`: https://github.com/tiangolo/typer\n.. _`Sphinx`: https://github.com/sphinx-doc/sphinx\n.. _`boto3`: https://github.com/boto/boto3\n.. _`git`: https://git-scm.com/\n.. _`FastAPI`: https://github.com/tiangolo/fastapi\n.. _`Swagger`: https://swagger.io\n.. _`oauth2`: https://oauth.net/2/\n.. _`context_example.rst`: https://github.com/TinkoffCreditSystems/overhave/blob/master/docs/includes/context_example.rst\n.. _`feature_example.rst`: https://github.com/TinkoffCreditSystems/overhave/blob/master/docs/includes/features_structure_example/feature_type_1/full_feature_example_en.feature\n',
-    'author': 'Vladislav Mukhamatnurov',
-    'author_email': 'livestreamepidemz@yandex.ru',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+========
+Overhave
+========
 
+.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/label_img.png
+  :width: 700
+  :align: center
+  :alt: Overhave framework
+
+  `Overhave`_ is the web-framework for BDD: scalable, configurable, easy to use, based on
+  `Flask Admin`_ and `Pydantic`_.
+
+  .. image:: https://github.com/TinkoffCreditSystems/overhave/workflows/CI/badge.svg
+    :target: https://github.com/TinkoffCreditSystems/overhave/actions?query=workflow%3ACI
+    :alt: CI
+
+  .. image:: https://img.shields.io/pypi/pyversions/overhave.svg
+    :target: https://pypi.org/project/overhave
+    :alt: Python versions
+
+  .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/TinkoffCreditSystems/overhave
+    :alt: Code style
+
+  .. image:: https://img.shields.io/pypi/v/overhave?color=%2334D058&label=pypi%20package
+    :target: https://pypi.org/project/overhave
+    :alt: Package version
+
+  .. image:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/coverage.svg
+    :target: https://github.com/TinkoffCreditSystems/overhave
+    :alt: PyTest Coverage percent
+    
+  .. image:: https://img.shields.io/pypi/dm/overhave.svg
+    :target: https://pypi.org/project/overhave
+    :alt: Downloads per month
+
+--------
+Features
+--------
+
+* Ready web-interface for easy BDD features management with `Ace`_ editor
+* Traditional Gherkin format for scenarios provided by `pytest-bdd`_
+* Execution and reporting of BDD features based on `Allure`_
+* Auto-collection of `pytest-bdd`_ steps and display on web-interface
+* Simple scenarios structure, easy horizontal scaling
+* Built-in wrappers for `pytest-bdd`_ hooks to supplement `Allure`_ report
+* Ability to create and use several BDD keywords dictionary with different languages
+* Versioning and deployment of scenario drafts to `Bitbucket`_ or `GitLab`_
+* Synchronization between `git`_ repository and database with features
+* Built-in configurable access management of users and groups
+* Configurable strategy for user authorization (LDAP also provided)
+* Database schema based on `SQLAlchemy`_ models and works with PostgreSQL
+* Still configurable as `Flask Admin`_, supports plug-ins and extensions
+* Has built-in API application with Swagger docs, based on `FastAPI`_
+* Distributed `producer-consumer` architecture based on `Walrus`_ Redis streams
+* Command-line interface, provided with `Typer`_
+* Integrated interaction for files storage with s3-cloud based on `boto3`_
+* Web-browser emulation ability with custom toolkit (`GoTTY`_, for example)
+
+------------
+Installation
+------------
+
+You can install **Overhave** via pip from PyPI:
+
+.. code-block:: shell
+
+    pip install overhave
+
+--------
+Overview
+--------
+
+Web-interface
+-------------
+
+The web-interface is a basic tool for BDD features management. It consists of:
+
+* `Info` - index page with optional information about your tool or project;
+* `Scenarios` - section for features management, contains subsections
+    `Features`, `Test runs`, `Versions` and `Tags`:
+
+    * `Features`
+        gives an interface for features records management and provides info
+        about id, name author, time, editor and publishing status; it is possible
+        to search, edit or delete items through Script panel.
+
+        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/label_img.png
+          :width: 500
+          :align: center
+          :alt: Features list
+
+    * `Test runs`
+        gives an interface for test runs management and provides info about.
+
+        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/test_runs_img.png
+          :width: 500
+          :align: center
+          :alt: Test runs list
+
+    * Versions
+        contains feature versions in corresponding to test runs; versions contains PR-links to
+        the remote Git repository.
+
+        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/versions_img.png
+          :width: 500
+          :align: center
+          :alt: Feature published versions list
+
+    * Tags
+        contains tags values, which are used for feature's tagging.
+
+        .. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/tags_img.png
+          :width: 500
+          :align: center
+          :alt: Feature published versions list
+
+* `Test users` - section for viewing and configuring test users;
+* `Access` - section for access management, contains `Users` and
+    `Groups` subsections;
+* `Emulation` - experimental section for alternative tools implementation
+    (in development).
+
+**Overhave** features could be created and/or edited through special
+*script panel* in feature edit mode. Feature should have type registered by the
+application, unique name, specified tasks list with the traditional format
+```PRJ-NUMBER``` and scenario text.
+
+**Script panel** has `pytest-bdd`_ steps table on the right side of interface.
+These steps should be defined in appropriate fixture modules and registered
+at the application on start-up to be displayed.
+
+
+.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/panel_img.png
+  :width: 600
+  :align: center
+  :alt: Script panel
+
+  Example of **Overhave** script panel in feature edit mode
+
+Allure report
+-------------
+
+**Overhave** generates `Allure`_ report after tests execution in web-interface.
+If you execute tests manually through `PyTest`_, these results are could be
+converted into the `Allure`_ report also with the `Allure CLI`_ tool.
+This report contains scenarios descriptions as they are described in features.
+
+.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/report_img.png
+  :width: 600
+  :align: center
+  :alt: Allure test-case report
+
+  Example of generated `Allure`_ report after execution of **Overhave**'s feature
+
+Demo-mode (Quickstart)
+----------------------
+
+**Overhave** has special demo-mode (in development), which could be possibly
+used for framework demonstration and manual debugging / testing. The framework
+provides a CLI entrypoints for easy server run in debug mode:
+
+.. code-block:: shell
+
+    make up  # start PostgreSQL database and Redis
+    overhave db create-all  # create Overhave database schema
+    overhave-demo admin  # start Overhave admin on port 8076 in debug mode
+    overhave-demo consumer -s test  # start Overhave test execution consumer
+
+**Note**: you could run admin in special mode, which does not require
+consumers. This mode uses *threadpool* for running testing and publication
+tasks asynchronously:
+
+.. code-block:: shell
+
+    overhave-demo admin --threadpool --language=ru
+
+But this *threadpool* mode is unscalable in *kubernetes* paradigm. So,
+it's highly recommended to use corresponding consumers exactly.
+
+Command-line interface
+----------------------
+
+**Overhave** has a CLI that provides a simple way to start service web-interface,
+run consumer and execute basic database operations. Examples are below:
+
+.. code-block:: shell
+
+    overhave db create-all
+    overhave admin --port 8080
+    overhave consumer -s publication
+    overhave api -p 8000 -w 4
+
+**Note**: service start-up takes a set of settings, so you can set them through
+virtual environment with prefix ```OVERHAVE_```, for example ```OVERHAVE_DB_URL```.
+If you want to configure settings in more explicit way through context injection,
+please see next part of docs.
+
+Context injection
+-----------------
+
+Context setting
+^^^^^^^^^^^^^^^
+
+Service could be configured via application context injection with prepared
+instance of `OverhaveContext` object. This context could be set using
+```set_context``` function of initialized ```ProxyFactory``` instance.
+
+For example, ```my_custom_context``` prepared. So, application start-up could
+be realised with follow code:
+
+.. code-block:: python
+
+    from overhave import overhave_app, overhave_admin_factory
+
+    factory = overhave_admin_factory()
+    factory.set_context(my_custom_context)
+    overhave_app(factory).run(host='localhost', port=8080, debug=True)
+
+**Note**:
+
+* ```overhave_app``` is the prepared `Flask` application with already enabled
+    Flask Admin and Login Manager plug-ins;
+* ```overhave_factory``` is a function for LRU cached instance of the **Overhave**
+    factory ```ProxyFactory```; the instance has an access to application components,
+    directly used in ```overhave_app```.
+* ```my_custom_context``` is an example of context configuration, see an
+    example code in `context_example.rst`_.
+
+Redis
+---------
+* **RedisSentinel** - redis connection through sentinel. To enable sentinel connection use env OVERHAVE_REDIS_SENTINEL_ENABLED=True
+
+* **Redis** - default redis connection without sentinel.
+
+Consumers
+---------
+
+**Overhave** has `producer-consumer` architecture, based on Redis streams,
+and supported 3 consumer's types:
+
+* **TEST** - consumer for test execution with it's own factory
+    ```overhave_test_execution_factory```;
+
+* **PUBLICATION** - consumer for features publication with it's own factory
+    ```overhave_publication_factory```;
+
+* **EMULATION** - consumer for specific emulation with it's own factory
+    ```overhave_emulation_factory```.
+
+**Note**: the ```overhave_test_execution_factory``` has ability for context injection
+and could be enriched with the custom context as the ```overhave_admin_factory```.
+
+Project structure
+-----------------
+
+**Overhave** supports it's own special project structure:
+
+.. image:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/project_structure.png
+  :width: 300
+  :alt: **Overhave** project structure
+
+The right approach is to create a **root directory** (like "demo" inside the current
+repository) that contains **features**, **fixtures** and **steps** directories.
+
+The **Features** directory contains different feature types as
+separate directories, each of them corresponds to predefined `pytest-bdd`_
+set of steps.
+
+The **Fixtures** directory contains typical `PyTest`_ modules splitted by different
+feature types. These modules are used for `pytest-bdd`_ isolated test runs. It is
+necessary because of special mechanism of `pytest-bdd`_ steps collection.
+
+The **Steps** directory contains `pytest-bdd`_ steps packages splitted by differrent
+feature types also. Each steps subdirectory has it's own declared steps in according
+to supported feature type.
+
+So, it is possible to create your own horizontal structure of
+different product directions with unique steps and `PyTest`_ fixtures.
+
+**Note**: this structure is used in **Overhave** application. The formed data
+gives a possibility to specify registered feature type in the web-interface
+*script panel*. Also, this structure defines which steps will be displayed in
+the right side of *script panel*.
+
+Feature format
+--------------
+
+**Overhave** has it's own special feature's text format, which inherits
+Gherkin from `pytest-bdd`_ with unique updates:
+
+* required tag that is related to existing feature type directory, where
+    current feature is located;
+* any amount of arbitrary tags;
+* severity tag - implements `Allure`_ severity to feature or just tagged
+    scenario (for example: ```@severity.blocker```);
+* info about feature - who is creator, last editor and publisher;
+* task tracker's tickets with format ```PRJ-1234```;
+
+An example of filled feature content is located in
+`feature_example.rst`_.
+
+Pytest markers
+--------------
+
+**Overhave** implements solution for `PyTest`_ markers usage with custom
+additional information:
+
+* "`disabled`": same as `skip` marker, but it's necessary to setup reason;
+* "`xfail`": traditional `xfail` with strict reason presence.
+
+Examples:
+
+.. code-block:: gherkin
+
+    @disabled(not ready)
+    Feature: My business feature
+
+.. code-block:: gherkin
+
+    @disabled(TODO: https://tracker.myorg.com/browse/PRJ-333; deadline 01.01.25)
+    Scenario: Yet another business feature
+
+
+.. code-block:: gherkin
+
+    @xfail(bug: https://tracker.myorg.com/browse/PRJ-555)
+    Scenario outline: Other business feature
+
+If reason contains URL, so **Overhave** will attach `Allure` link to report:
+for `disabled` - it will be `LinkType.LINK`, for `xfail` - `LinkType.ISSUE`.
+
+Feature links
+-------------
+
+**Overhave** has ability to set links to it's own admin service in `Allure`_
+test-cases. Link will be set automatically when you generate `Allure`_ report.
+This function can be enabled via setup of environment variable
+```OVERHAVE_ADMIN_URL```:
+
+.. code-block:: bash
+
+    export OVERHAVE_ADMIN_URL=https://overhave-admin.myorg.com
+
+Also, **Overhave** has ability to set links to feature file in `Git`_ repository.
+Link will be set automatically when you generate `Allure`_ report. This function
+can be enabled via setup of environment variable
+```OVERHAVE_GIT_PROJECT_URL```:
+
+.. code-block:: bash
+
+    export OVERHAVE_GIT_PROJECT_URL=https://git.myorg.com/bdd-features-repo
+
+
+Language
+--------
+
+The web-interface language is ENG by default and could not be switched
+(if it's necessary - please, create a ```feature request``` or contribute
+yourself).
+
+The feature text as well as `pytest-bdd`_ BDD keywords are configurable
+with **Overhave** extra models, for example RUS keywords are already defined
+in framework and available for usage:
+
+.. code-block:: python
+
+    from overhave.extra import RUSSIAN_PREFIXES
+
+    language_settings = OverhaveLanguageSettings(step_prefixes=RUSSIAN_PREFIXES)
+
+**Note**: you could create your own prefix-value mapping for your language:
+
+.. code-block:: python
+
+    from overhave import StepPrefixesModel
+
+    GERMAN_PREFIXES = StepPrefixesModel(
+        FEATURE="Merkmal:",
+        SCENARIO_OUTLINE="Szenarioübersicht:",
+        SCENARIO="Szenario:",
+        BACKGROUND="Hintergrund:",
+        EXAMPLES="Beispiele:",
+        EXAMPLES_VERTICAL="Beispiele: Vertikal",
+        GIVEN="Gegeben ",
+        WHEN="Wann ",
+        THEN="Dann ",
+        AND="Und ",
+        BUT="Aber ",
+    )
+
+Git integration
+---------------
+
+**Overhave** gives an ability to sent your new features or changes to
+remote git repository, which is hosted by `Bitbucket`_ or `GitLab`_.
+Integration with bitbucket is native, while integration with GitLab
+uses `python-gitlab`_ library.
+
+You are able to set necessary settings for your project:
+
+.. code-block:: python
+
+    publisher_settings = OverhaveGitlabPublisherSettings(
+        repository_id='123',
+        default_target_branch_name='master',
+    )
+    client_settings=OverhaveGitlabClientSettings(
+        url="https://gitlab.mycompany.com",
+        auth_token=os.environ.get("MY_GITLAB_AUTH_TOKEN"),
+    )
+
+The pull-request (for Bitbucket) or merge-request (for GitLab)
+created when you click the button `Create pull request` on
+test run result's page. This button is available only for `success`
+test run's result.
+
+**Note**: one of the most popular cases of GitLab API
+authentication is the OAUTH2 schema with service account.
+In according to this schema, you should have OAUTH2 token,
+which is might have a short life-time and could not be
+specified through environment. For this situation, **Overhave**
+has special `TokenizerClient` with it's own
+`TokenizerClientSettings` - this simple client could take
+the token from a remote custom GitLab tokenizer service.
+
+Git-to-DataBase synchronization
+-------------------------------
+
+**Overhave** gives an ability to synchronize your current `git`_
+repository's state with database. It means that your features,
+which are located on the database, could be updated - and the source
+of updates is your repository.
+
+**For example**: you had to do bulk data replacement in `git`_
+repository, and now you want to deliver changes to remote database.
+This not so easy matter could be solved with **Overhave** special
+tooling:
+
+You are able to set necessary settings for your project:
+
+.. code-block:: bash
+
+    overhave sync run  # only update existing features
+    overhave sync run --create-db-features  # update + create new features
+    overhave sync run --pull-repository  # pull git repo and run sync
+
+You are able to test this tool with **Overhave** demo mode.
+By default, 3 features are created in demo database. Just try
+to change them or create new features and run synchronization
+command - you will get the result.
+
+.. code-block:: bash
+
+    overhave-demo sync-run  # or with '--create-db-features'
+
+**Overhave** supports validation of existing feature files.
+Command try to parse features and fill defined feature info format.
+If there is any problem, special error will be thrown.
+
+.. code-block:: bash
+
+    overhave sync validate-features
+    overhave sync validate-features --raise-if-nullable-id
+    overhave sync validate-features --pull-repository
+
+And yes, your are able to try it with demo mode:
+
+.. code-block:: bash
+
+    overhave-demo validate-features
+    overhave sync validate-features -r  # --raise-if-nullable-id
+
+Custom index
+------------
+
+**Overhave** gives an ability to set custom index.html file for rendering. Path
+to file could be set through environment as well as set with context:
+
+.. code-block:: python
+
+    admin_settings = OverhaveAdminSettings(
+        index_template_path="/path/to/index.html"
+    )
+
+Authorization strategy
+----------------------
+
+**Overhave** provides several authorization strategies, declared by
+```AuthorizationStrategy``` enum:
+
+* `Simple` - strategy without real authorization.
+    Each user could use preferred name. This name will be used for user
+    authority. Each user is unique. Password not required.
+
+* `Default` - strategy with real authorization.
+    Each user could use only registered credentials.
+
+* `LDAP` - strategy with authorization using remote LDAP server.
+    Each user should use his LDAP credentials. LDAP
+    server returns user groups. If user in default 'admin' group or his groups
+    list contains admin group - user will be authorized. If user already placed
+    in database - user will be authorized too. No one password stores.
+
+Appropriate strategy and additional data should be placed into
+```OverhaveAuthorizationSettings```, for example LDAP strategy could be
+configured like this:
+
+.. code-block:: python
+
+    auth_settings = OverhaveAuthorizationSettings(auth_strategy=AuthorizationStrategy.LDAP)
+    ldap_manager_settings = OverhaveLdapManagerSettings(ldap_admin_group="admin")
+
+S3 cloud
+--------
+
+**Overhave** implements functionality for *s3* cloud interactions, such as
+bucket creation and deletion, files uploading, downloading and deletion.
+The framework provides an ability to store reports and other files in
+the remote s3 cloud storage. You could enrich your environment with following
+settings:
+
+.. code-block:: shell
+
+    OVERHAVE_S3_ENABLED=true
+    OVERHAVE_S3_URL=https://s3.example.com
+    OVERHAVE_S3_ACCESS_KEY=<MY_ACCESS_KEY>
+    OVERHAVE_S3_SECRET_KEY=<MY_SECRET_KEY>
+
+Optionally, you could change default settings also:
+
+.. code-block:: shell
+
+    OVERHAVE_S3_VERIFY=false
+    OVERHAVE_S3_AUTOCREATE_BUCKETS=true
+
+The framework with enabled ```OVERHAVE_S3_AUTOCREATE_BUCKETS``` flag will create
+application buckets in remote storage if buckets don't exist.
+
+API
+---
+**Overhave** has it's own application programming interface, based on
+`FastAPI`_.
+
+.. figure:: https://raw.githubusercontent.com/TinkoffCreditSystems/overhave/master/docs/includes/images/api_img.png
+  :width: 600
+  :align: center
+  :alt: Allure test-case report
+
+  **Overhave** openapi.json through `Swagger`_
+
+Current possibilities could be displayed through built-in
+`Swagger`_ - just run the API and open http://localhost:8000 in your
+browser.
+
+.. code-block:: bash
+
+    overhave api -p 8000
+
+Interface has authorization through `oauth2`_ scheme, so you should setup
+```OVERHAVE_API_AUTH_SECRET_KEY``` for usage.
+
+Right now, API implements types of resources:
+
+* `feature_tags`
+    get feature tag or get list of feature tags;
+* `features`
+    get features info by tag ID or tag value;
+* `test_users`
+    get test user info, specification, put new specification or delete
+    test user;
+* `test_runs`
+    get test run info or create test run with given parameters;
+* `emulations`
+    get emulation runs by test user id.
+
+------------
+Contributing
+------------
+
+Contributions are very welcome.
+
+Preparation
+-----------
+
+Project installation is very easy
+and takes just few prepared commands (`make pre-init` works only for Ubuntu;
+so you can install same packages for your OS manually):
+
+.. code-block:: shell
+
+    make pre-init
+    make init
+
+Packages management is provided by `Poetry`_.
+
+Check
+-----
+
+Tests can be run with `Tox`_. `Docker-compose`_ is used for other services
+preparation and serving, such as database. Simple tests and linters execution:
+
+.. code-block:: shell
+
+    make up
+    make test
+    make lint
+
+Please, see `make` file and discover useful shortcuts. You could run tests
+in docker container also:
+
+.. code-block:: shell
+
+    make test-docker
+
+Documentation build
+-------------------
+
+Project documentation could be built via `Sphinx`_ and simple `make` command:
+
+.. code-block:: shell
+
+    make build-docs
+
+By default, the documentation will be built using `html` builder into `_build`
+directory.
+
+-------
+License
+-------
+
+Distributed under the terms of the `GNU GPLv2`_ license.
+
+------
+Issues
+------
+
+If you encounter any problems, please report them here in section `Issues`
+with a detailed description.
+
+.. _`Overhave`: https://github.com/TinkoffCreditSystems/overhave
+.. _`Pydantic`: https://github.com/samuelcolvin/pydantic
+.. _`Flask Admin`: https://github.com/flask-admin/flask-admin
+.. _`Ace`: https://github.com/ajaxorg/ace
+.. _`PyTest`: https://github.com/pytest-dev/pytest
+.. _`pytest-bdd`: https://github.com/pytest-dev/pytest-bdd
+.. _`Allure`: https://github.com/allure-framework/allure-python
+.. _`Allure CLI`: https://docs.qameta.io/allure/#_get_started
+.. _`Bitbucket`: https://www.atlassian.com/git
+.. _`GitLab`: https://about.gitlab.com
+.. _`python-gitlab`: https://python-gitlab.readthedocs.io
+.. _`SQLAlchemy`: https://github.com/sqlalchemy/sqlalchemy
+.. _`Walrus`: https://github.com/coleifer/walrus
+.. _`GoTTY`: https://github.com/yudai/gotty
+.. _`GNU GPLv2`: http://www.apache.org/licenses/LICENSE-2.0
+.. _`Tox`: https://github.com/tox-dev/tox
+.. _`Poetry`: https://github.com/python-poetry/poetry
+.. _`Docker-compose`: https://docs.docker.com/compose
+.. _`Typer`: https://github.com/tiangolo/typer
+.. _`Sphinx`: https://github.com/sphinx-doc/sphinx
+.. _`boto3`: https://github.com/boto/boto3
+.. _`git`: https://git-scm.com/
+.. _`FastAPI`: https://github.com/tiangolo/fastapi
+.. _`Swagger`: https://swagger.io
+.. _`oauth2`: https://oauth.net/2/
+.. _`context_example.rst`: https://github.com/TinkoffCreditSystems/overhave/blob/master/docs/includes/context_example.rst
+.. _`feature_example.rst`: https://github.com/TinkoffCreditSystems/overhave/blob/master/docs/includes/features_structure_example/feature_type_1/full_feature_example_en.feature
 
-setup(**setup_kwargs)
```

