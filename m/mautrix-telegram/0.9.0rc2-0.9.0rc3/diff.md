# Comparing `tmp/mautrix-telegram-0.9.0rc2.tar.gz` & `tmp/mautrix-telegram-0.9.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mautrix-telegram-0.9.0rc2.tar", last modified: Fri Nov  6 19:30:24 2020, max compression
+gzip compressed data, was "dist/mautrix-telegram-0.9.0rc3.tar", last modified: Wed Nov 11 23:41:54 2020, max compression
```

## Comparing `mautrix-telegram-0.9.0rc2.tar` & `mautrix-telegram-0.9.0rc3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.956483 mautrix-telegram-0.9.0rc2/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/LICENSE
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       93 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/MANIFEST.in
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2984 2020-11-06 19:30:24.956483 mautrix-telegram-0.9.0rc2/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1723 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/README.md
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.940483 mautrix-telegram-0.9.0rc2/alembic/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2617 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/env.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.944483 mautrix-telegram-0.9.0rc2/alembic/versions/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      679 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/17574c57f3f8_add_disable_updates_field_for_puppets.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      745 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/1b241f7e8530_add_telegramfile_table.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      570 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/1fa46383a9d3_add_is_bot_field_to_puppets.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1612 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/2228d49c383f_add_cascade_rules_to_userportal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      661 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/24f31fc8a72b_add_encrypted_field_for_portals.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      563 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/30eca60587f1_add_megagroup_field_to_portals.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      815 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/3e3745baa458_store_matrix_avatar_url_in_database.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      625 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/4f7d7ed5792a_switch_mx_user_profile_to_native_enum.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4430 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/501dad2868bc_move_sessions_to_main_database.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4804 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/6ca3d74d51e4_move_state_store_to_main_database.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      618 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/7d47d84380b6_add_timestamp_to_telegramfile.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      856 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/888275d58e57_add_double_puppet_base_url_to_puppet_.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3685 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/97d2a942bcf8_initial_revision.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1859 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/9e9c89b0b877_add_edit_index_to_messages.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1339 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/a328bf4f0932_store_encryption_state_event_in_db.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      592 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/a7c04a56041b_store_custom_puppet_next_batch_in_.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      520 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/a9119be92164_add_phone_number_field_to_users.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      513 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/b54929c22c86_add_portal_specific_config.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      554 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/bcfefa1f1299_add_displayname_source_fields_for_.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1921 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/bdadd173ee02_update_telethon_update_state_table.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3588 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/ccbaff858240_switch_to_mautrix_python_crypto.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1193 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/cfc972368e50_add_metadata_to_telegramfile.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      627 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/d3c922a6acd2_add_decryption_info_field_for_.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      677 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/d5f7b8b4b456_add_access_token_and_custom_mxid_fields_.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2822 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/dff56c93da8d_add_matrix_nio_state_store_to_main_db.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1215 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic/versions/eeaf0dae87ce_add_telethon_update_state_table.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1592 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/alembic.ini
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.944483 mautrix-telegram-0.9.0rc2/mautrix_telegram/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       73 2020-11-06 19:28:00.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5122 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/__main__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    21533 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/abstract_user.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12968 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/bot.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.948483 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      493 2020-10-26 17:22:08.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5862 2020-10-24 17:23:39.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/handler.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5167 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/manhole.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5601 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/matrix_auth.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.948483 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       73 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3024 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/admin.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9559 2020-10-30 18:05:52.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/bridge.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6092 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/config.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2662 2020-10-30 18:03:05.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/create_chat.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3967 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/filter.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6808 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/misc.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4741 2020-10-29 21:01:17.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/unbridge.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2556 2020-10-30 18:15:57.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/util.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.948483 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/telegram/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       34 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/telegram/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5808 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/telegram/account.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    16487 2020-10-28 16:53:51.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/telegram/auth.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    15883 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/telegram/misc.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    10036 2020-10-30 10:29:07.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/config.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2116 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/context.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.948483 mautrix-telegram-0.9.0rc2/mautrix_telegram/db/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1267 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/db/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1380 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/db/bot_chat.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4052 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/db/message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2598 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/db/portal.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2548 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/db/puppet.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3158 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/db/telegram_file.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4249 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/db/user.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    25161 2020-10-24 17:49:56.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/example-config.yaml
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.948483 mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      293 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/__init__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.952483 mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_matrix/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5259 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_matrix/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3709 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_matrix/parser.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     3840 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_matrix/telegram_message.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    13668 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_telegram.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1468 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/get_version.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    18890 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/matrix.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.952483 mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      564 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    21011 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/base.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5321 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/deduplication.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    30242 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/matrix.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    39214 2020-10-30 17:42:38.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/metadata.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1509 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/send_lock.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    37887 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/telegram.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    17015 2020-10-24 18:07:18.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/puppet.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.952483 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/__init__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.952483 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/dbms_migrate/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/dbms_migrate/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2965 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/dbms_migrate/__main__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.952483 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/telematrix_import/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/telematrix_import/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4918 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/telematrix_import/__main__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1126 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/telematrix_import/models.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2845 2020-11-06 16:13:16.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/tgclient.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       68 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/types.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    19885 2020-10-29 20:38:41.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/user.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.952483 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      287 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1385 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/color_log.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    12099 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/file_transfer.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1432 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/format_duration.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    13719 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/parallel_file_transfer.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1900 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/recursive_dict.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     1230 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/sane_mimetypes.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     6277 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/util/tgs_converter.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      195 2020-11-06 19:30:24.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/version.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.952483 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       82 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/__init__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.952483 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/common/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       30 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/common/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    11624 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/common/auth_api.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.956483 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/provisioning/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    21722 2020-10-30 18:06:43.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/provisioning/__init__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.956483 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     9181 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    43371 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/favicon.png
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2328 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/login.css
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     4366 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/login.html.mako
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2817 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/matrix-login.html.mako
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.948483 mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2984 2020-11-06 19:30:24.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/PKG-INFO
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     5004 2020-11-06 19:30:24.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/SOURCES.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2020-11-06 19:30:24.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/dependency_links.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      732 2020-11-06 19:30:24.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/requires.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       23 2020-11-06 19:30:24.000000 mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/top_level.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      450 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/optional-requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      210 2020-11-05 20:15:58.000000 mautrix-telegram-0.9.0rc2/requirements.txt
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       63 2020-11-06 19:30:24.956483 mautrix-telegram-0.9.0rc2/setup.cfg
--rw-rw-r--   0 tulir     (1000) tulir     (1000)     2393 2020-10-24 17:16:03.000000 mautrix-telegram-0.9.0rc2/setup.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.956483 mautrix-telegram-0.9.0rc2/tests/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/tests/__init__.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.956483 mautrix-telegram-0.9.0rc2/tests/commands/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/tests/commands/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)    13476 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/tests/commands/test_handler.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)       49 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/tests/conftest.py
-drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-06 19:30:24.956483 mautrix-telegram-0.9.0rc2/tests/utils/
--rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/tests/utils/__init__.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      676 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/tests/utils/fixtures.py
--rw-rw-r--   0 tulir     (1000) tulir     (1000)      693 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc2/tests/utils/helpers.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    34523 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/LICENSE
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       93 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/MANIFEST.in
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2984 2020-11-11 23:41:54.433516 mautrix-telegram-0.9.0rc3/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1723 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/README.md
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.409516 mautrix-telegram-0.9.0rc3/alembic/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2617 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/env.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.413516 mautrix-telegram-0.9.0rc3/alembic/versions/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      679 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/17574c57f3f8_add_disable_updates_field_for_puppets.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      745 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/1b241f7e8530_add_telegramfile_table.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      570 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/1fa46383a9d3_add_is_bot_field_to_puppets.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1612 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/2228d49c383f_add_cascade_rules_to_userportal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      661 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/24f31fc8a72b_add_encrypted_field_for_portals.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      563 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/30eca60587f1_add_megagroup_field_to_portals.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      815 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/3e3745baa458_store_matrix_avatar_url_in_database.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      625 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/4f7d7ed5792a_switch_mx_user_profile_to_native_enum.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4430 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/501dad2868bc_move_sessions_to_main_database.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4804 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/6ca3d74d51e4_move_state_store_to_main_database.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      618 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/7d47d84380b6_add_timestamp_to_telegramfile.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      856 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/888275d58e57_add_double_puppet_base_url_to_puppet_.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3685 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/97d2a942bcf8_initial_revision.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1859 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/9e9c89b0b877_add_edit_index_to_messages.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1339 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/a328bf4f0932_store_encryption_state_event_in_db.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      592 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/a7c04a56041b_store_custom_puppet_next_batch_in_.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      520 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/a9119be92164_add_phone_number_field_to_users.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      513 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/b54929c22c86_add_portal_specific_config.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      554 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/bcfefa1f1299_add_displayname_source_fields_for_.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1921 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/bdadd173ee02_update_telethon_update_state_table.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3588 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/ccbaff858240_switch_to_mautrix_python_crypto.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1193 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/cfc972368e50_add_metadata_to_telegramfile.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      627 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/d3c922a6acd2_add_decryption_info_field_for_.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      677 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/d5f7b8b4b456_add_access_token_and_custom_mxid_fields_.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2822 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/dff56c93da8d_add_matrix_nio_state_store_to_main_db.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1215 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic/versions/eeaf0dae87ce_add_telethon_update_state_table.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1592 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/alembic.ini
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.417516 mautrix-telegram-0.9.0rc3/mautrix_telegram/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       73 2020-11-11 23:41:34.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5122 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/__main__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    21533 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/abstract_user.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    12968 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/bot.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.417516 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      493 2020-10-26 17:22:08.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5862 2020-10-24 17:23:39.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/handler.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5167 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/manhole.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5601 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/matrix_auth.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.421516 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       73 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3024 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/admin.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9559 2020-10-30 18:05:52.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/bridge.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6092 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/config.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2662 2020-10-30 18:03:05.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/create_chat.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3967 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/filter.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6808 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/misc.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4741 2020-10-29 21:01:17.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/unbridge.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2556 2020-10-30 18:15:57.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/util.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.421516 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/telegram/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       34 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/telegram/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5808 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/telegram/account.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    16487 2020-10-28 16:53:51.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/telegram/auth.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    15883 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/telegram/misc.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    10036 2020-10-30 10:29:07.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/config.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2116 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/context.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.421516 mautrix-telegram-0.9.0rc3/mautrix_telegram/db/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1267 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/db/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1380 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/db/bot_chat.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4052 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/db/message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2598 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/db/portal.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2548 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/db/puppet.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3158 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/db/telegram_file.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4249 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/db/user.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    25161 2020-10-24 17:49:56.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/example-config.yaml
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.421516 mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      240 2020-11-07 13:59:24.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/__init__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.421516 mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_matrix/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6500 2020-11-07 13:59:11.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_matrix/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3709 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_matrix/parser.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     3840 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_matrix/telegram_message.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    13660 2020-11-10 10:28:09.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_telegram.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1468 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/get_version.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    18890 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/matrix.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.425516 mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      564 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    21011 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/base.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5321 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/deduplication.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    29510 2020-11-07 13:51:13.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/matrix.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    39214 2020-10-30 17:42:38.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/metadata.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1509 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/send_lock.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    37887 2020-11-06 19:27:55.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/telegram.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    17015 2020-10-24 18:07:18.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/puppet.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.425516 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/__init__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.425516 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/dbms_migrate/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/dbms_migrate/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2965 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/dbms_migrate/__main__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.425516 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/telematrix_import/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/telematrix_import/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4918 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/telematrix_import/__main__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1126 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/telematrix_import/models.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2845 2020-11-06 16:13:16.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/tgclient.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       68 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/types.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    19885 2020-10-29 20:38:41.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/user.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      287 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1385 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/color_log.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    12300 2020-11-09 21:52:34.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/file_transfer.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1432 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/format_duration.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    13719 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/parallel_file_transfer.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1900 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/recursive_dict.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     1230 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/sane_mimetypes.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     6277 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/util/tgs_converter.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      195 2020-11-11 23:41:54.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/version.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       82 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/__init__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/common/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       30 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/common/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    11624 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/common/auth_api.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/provisioning/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    21722 2020-10-30 18:06:43.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/provisioning/__init__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     9181 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    43371 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/favicon.png
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2328 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/login.css
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     4366 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/login.html.mako
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2817 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/matrix-login.html.mako
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.417516 mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2984 2020-11-11 23:41:54.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/PKG-INFO
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     5004 2020-11-11 23:41:54.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/SOURCES.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        1 2020-11-11 23:41:54.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/dependency_links.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      734 2020-11-11 23:41:54.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/requires.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       23 2020-11-11 23:41:54.000000 mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/top_level.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      450 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/optional-requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      212 2020-11-09 22:21:21.000000 mautrix-telegram-0.9.0rc3/requirements.txt
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       63 2020-11-11 23:41:54.433516 mautrix-telegram-0.9.0rc3/setup.cfg
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)     2393 2020-10-24 17:16:03.000000 mautrix-telegram-0.9.0rc3/setup.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/tests/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/tests/__init__.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/tests/commands/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/tests/commands/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)    13476 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/tests/commands/test_handler.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)       49 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/tests/conftest.py
+drwxrwxr-x   0 tulir     (1000) tulir     (1000)        0 2020-11-11 23:41:54.429516 mautrix-telegram-0.9.0rc3/tests/utils/
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)        0 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/tests/utils/__init__.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      676 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/tests/utils/fixtures.py
+-rw-rw-r--   0 tulir     (1000) tulir     (1000)      693 2020-10-22 21:13:26.000000 mautrix-telegram-0.9.0rc3/tests/utils/helpers.py
```

### Comparing `mautrix-telegram-0.9.0rc2/LICENSE` & `mautrix-telegram-0.9.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/PKG-INFO` & `mautrix-telegram-0.9.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mautrix-telegram
-Version: 0.9.0rc2
+Version: 0.9.0rc3
 Summary: A Matrix-Telegram hybrid puppeting/relaybot bridge.
 Home-page: https://github.com/tulir/mautrix-telegram
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
 License: UNKNOWN
 Description: # mautrix-telegram
         ![Languages](https://img.shields.io/github/languages/top/tulir/mautrix-telegram.svg)
```

### Comparing `mautrix-telegram-0.9.0rc2/README.md` & `mautrix-telegram-0.9.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/env.py` & `mautrix-telegram-0.9.0rc3/alembic/env.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/17574c57f3f8_add_disable_updates_field_for_puppets.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/17574c57f3f8_add_disable_updates_field_for_puppets.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/1b241f7e8530_add_telegramfile_table.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/1b241f7e8530_add_telegramfile_table.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/1fa46383a9d3_add_is_bot_field_to_puppets.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/1fa46383a9d3_add_is_bot_field_to_puppets.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/2228d49c383f_add_cascade_rules_to_userportal.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/2228d49c383f_add_cascade_rules_to_userportal.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/24f31fc8a72b_add_encrypted_field_for_portals.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/24f31fc8a72b_add_encrypted_field_for_portals.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/30eca60587f1_add_megagroup_field_to_portals.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/30eca60587f1_add_megagroup_field_to_portals.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/3e3745baa458_store_matrix_avatar_url_in_database.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/3e3745baa458_store_matrix_avatar_url_in_database.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/4f7d7ed5792a_switch_mx_user_profile_to_native_enum.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/4f7d7ed5792a_switch_mx_user_profile_to_native_enum.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/501dad2868bc_move_sessions_to_main_database.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/501dad2868bc_move_sessions_to_main_database.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/6ca3d74d51e4_move_state_store_to_main_database.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/6ca3d74d51e4_move_state_store_to_main_database.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/7d47d84380b6_add_timestamp_to_telegramfile.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/7d47d84380b6_add_timestamp_to_telegramfile.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/888275d58e57_add_double_puppet_base_url_to_puppet_.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/888275d58e57_add_double_puppet_base_url_to_puppet_.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/97d2a942bcf8_initial_revision.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/97d2a942bcf8_initial_revision.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/9e9c89b0b877_add_edit_index_to_messages.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/9e9c89b0b877_add_edit_index_to_messages.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/a328bf4f0932_store_encryption_state_event_in_db.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/a328bf4f0932_store_encryption_state_event_in_db.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/a7c04a56041b_store_custom_puppet_next_batch_in_.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/a7c04a56041b_store_custom_puppet_next_batch_in_.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/a9119be92164_add_phone_number_field_to_users.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/a9119be92164_add_phone_number_field_to_users.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/b54929c22c86_add_portal_specific_config.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/b54929c22c86_add_portal_specific_config.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/bcfefa1f1299_add_displayname_source_fields_for_.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/bcfefa1f1299_add_displayname_source_fields_for_.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/bdadd173ee02_update_telethon_update_state_table.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/bdadd173ee02_update_telethon_update_state_table.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/ccbaff858240_switch_to_mautrix_python_crypto.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/ccbaff858240_switch_to_mautrix_python_crypto.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/cfc972368e50_add_metadata_to_telegramfile.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/cfc972368e50_add_metadata_to_telegramfile.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/d3c922a6acd2_add_decryption_info_field_for_.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/d3c922a6acd2_add_decryption_info_field_for_.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/d5f7b8b4b456_add_access_token_and_custom_mxid_fields_.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/d5f7b8b4b456_add_access_token_and_custom_mxid_fields_.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/dff56c93da8d_add_matrix_nio_state_store_to_main_db.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/dff56c93da8d_add_matrix_nio_state_store_to_main_db.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic/versions/eeaf0dae87ce_add_telethon_update_state_table.py` & `mautrix-telegram-0.9.0rc3/alembic/versions/eeaf0dae87ce_add_telethon_update_state_table.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/alembic.ini` & `mautrix-telegram-0.9.0rc3/alembic.ini`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/__main__.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/__main__.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/abstract_user.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/abstract_user.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/bot.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/bot.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/handler.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/handler.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/manhole.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/manhole.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/matrix_auth.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/matrix_auth.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/admin.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/admin.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/bridge.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/bridge.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/config.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/config.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/create_chat.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/create_chat.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/filter.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/filter.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/misc.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/misc.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/unbridge.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/unbridge.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/portal/util.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/portal/util.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/telegram/account.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/telegram/account.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/telegram/auth.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/telegram/auth.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/commands/telegram/misc.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/commands/telegram/misc.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/config.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/config.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/context.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/context.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/db/__init__.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/db/__init__.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/db/bot_chat.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/db/bot_chat.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/db/message.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/db/message.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/db/portal.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/db/portal.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/db/puppet.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/db/puppet.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/db/telegram_file.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/db/telegram_file.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/db/user.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/db/user.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/example-config.yaml` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/example-config.yaml`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_matrix/__init__.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_matrix/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,51 +14,42 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from typing import Optional, List, Tuple, Callable, Pattern, Match, TYPE_CHECKING
 import re
 import logging
 
 from telethon.tl.types import (MessageEntityMention, MessageEntityMentionName, MessageEntityItalic,
-                               TypeMessageEntity)
+                               TypeMessageEntity, InputMessageEntityMentionName)
 from telethon.helpers import add_surrogate, del_surrogate
+from telethon import TelegramClient
 
 from mautrix.types import RoomID, MessageEventContent
+from mautrix.util.logging import TraceLogger
 
 from ... import puppet as pu
 from ...types import TelegramID
 from ...db import Message as DBMessage
 from .parser import ParsedMessage, parse_html
 
 if TYPE_CHECKING:
     from ...context import Context
 
-log: logging.Logger = logging.getLogger("mau.fmt.mx")
+log: TraceLogger = logging.getLogger("mau.fmt.mx")
 should_bridge_plaintext_highlights: bool = False
 
 command_regex: Pattern = re.compile(r"^!([A-Za-z0-9@]+)")
 not_command_regex: Pattern = re.compile(r"^\\(![A-Za-z0-9@]+)")
 plain_mention_regex: Optional[Pattern] = None
 
-
-def plain_mention_to_html(match: Match) -> str:
-    puppet = pu.Puppet.find_by_displayname(match.group(2))
-    if puppet:
-        return (f"{match.group(1)}"
-                f"<a href='https://matrix.to/#/{puppet.mxid}'>"
-                f"{puppet.displayname}"
-                "</a>")
-    return "".join(match.groups())
-
-
 MAX_LENGTH = 4096
 CUTOFF_TEXT = " [message cut]"
 CUT_MAX_LENGTH = MAX_LENGTH - len(CUTOFF_TEXT)
 
 
-def cut_long_message(message: str, entities: List[TypeMessageEntity]) -> ParsedMessage:
+def _cut_long_message(message: str, entities: List[TypeMessageEntity]) -> ParsedMessage:
     if len(message) > MAX_LENGTH:
         message = message[0:CUT_MAX_LENGTH] + CUTOFF_TEXT
         new_entities = []
         for entity in entities:
             if entity.offset > CUT_MAX_LENGTH:
                 continue
             if entity.offset + entity.length > CUT_MAX_LENGTH:
@@ -69,57 +60,82 @@
     return message, entities
 
 
 class FormatError(Exception):
     pass
 
 
-def matrix_to_telegram(html: str) -> ParsedMessage:
+def matrix_reply_to_telegram(content: MessageEventContent, tg_space: TelegramID,
+                             room_id: Optional[RoomID] = None) -> Optional[TelegramID]:
+    event_id = content.get_reply_to()
+    if not event_id:
+        return
+    content.trim_reply_fallback()
+
+    message = DBMessage.get_by_mxid(event_id, room_id, tg_space)
+    if message:
+        return message.tgid
+    return None
+
+
+async def matrix_to_telegram(client: TelegramClient, *, text: Optional[str] = None,
+                             html: Optional[str] = None) -> ParsedMessage:
+    if html is not None:
+        text, entities = _matrix_html_to_telegram(html)
+    elif text is not None:
+        text, entities = _matrix_text_to_telegram(text)
+    else:
+        raise ValueError("text or html must be provided to convert formatting")
+    await _fix_name_mentions(client, entities)
+    return text, entities
+
+
+def _matrix_html_to_telegram(html: str) -> ParsedMessage:
     try:
         html = command_regex.sub(r"<command>\1</command>", html)
         html = html.replace("\t", " " * 4)
         html = not_command_regex.sub(r"\1", html)
         if should_bridge_plaintext_highlights:
-            html = plain_mention_regex.sub(plain_mention_to_html, html)
+            html = plain_mention_regex.sub(_plain_mention_to_html, html)
 
         text, entities = parse_html(add_surrogate(html))
         text = del_surrogate(text.strip())
-        text, entities = cut_long_message(text, entities)
+        text, entities = _cut_long_message(text, entities)
 
         return text, entities
     except Exception as e:
         raise FormatError(f"Failed to convert Matrix format: {html}") from e
 
 
-def matrix_reply_to_telegram(content: MessageEventContent, tg_space: TelegramID,
-                             room_id: Optional[RoomID] = None) -> Optional[TelegramID]:
-    event_id = content.get_reply_to()
-    if not event_id:
-        return
-    content.trim_reply_fallback()
-
-    message = DBMessage.get_by_mxid(event_id, room_id, tg_space)
-    if message:
-        return message.tgid
-    return None
-
-
-def matrix_text_to_telegram(text: str) -> ParsedMessage:
+def _matrix_text_to_telegram(text: str) -> ParsedMessage:
     text = command_regex.sub(r"/\1", text)
     text = text.replace("\t", " " * 4)
     text = not_command_regex.sub(r"\1", text)
     if should_bridge_plaintext_highlights:
-        entities, pmr_replacer = plain_mention_to_text()
+        entities, pmr_replacer = _plain_mention_to_text()
         text = plain_mention_regex.sub(pmr_replacer, text)
     else:
         entities = []
     return text, entities
 
 
-def plain_mention_to_text() -> Tuple[List[TypeMessageEntity], Callable[[Match], str]]:
+async def _fix_name_mentions(client: TelegramClient, entities: List[TypeMessageEntity]) -> None:
+    for index in reversed(range(len(entities))):
+        entity = entities[index]
+        if isinstance(entity, (MessageEntityMentionName, InputMessageEntityMentionName)):
+            try:
+                user = await client.get_input_entity(entity.user_id)
+            except (ValueError, TypeError) as e:
+                log.trace(f"Dropping mention of {entity.user_id}: {e}")
+                del entities[index]
+            else:
+                entities[index] = InputMessageEntityMentionName(entity.offset, entity.length, user)
+
+
+def _plain_mention_to_text() -> Tuple[List[TypeMessageEntity], Callable[[Match], str]]:
     entities = []
 
     def replacer(match: Match) -> str:
         puppet = pu.Puppet.find_by_displayname(match.group(2))
         if puppet:
             offset = match.start()
             length = match.end() - offset
@@ -132,14 +148,24 @@
             entities.append(entity)
             return text
         return "".join(match.groups())
 
     return entities, replacer
 
 
+def _plain_mention_to_html(match: Match) -> str:
+    puppet = pu.Puppet.find_by_displayname(match.group(2))
+    if puppet:
+        return (f"{match.group(1)}"
+                f"<a href='https://matrix.to/#/{puppet.mxid}'>"
+                f"{puppet.displayname}"
+                "</a>")
+    return "".join(match.groups())
+
+
 def init_mx(context: "Context") -> None:
     global plain_mention_regex, should_bridge_plaintext_highlights
     config = context.config
     dn_template = config["bridge.displayname_template"]
     dn_template = re.escape(dn_template).replace(re.escape("{displayname}"), "[^>]+")
     plain_mention_regex = re.compile(f"^({dn_template})")
     should_bridge_plaintext_highlights = config["bridge.plaintext_highlights"]
```

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_matrix/parser.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_matrix/parser.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_matrix/telegram_message.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_matrix/telegram_message.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/formatter/from_telegram.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/formatter/from_telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 def telegram_reply_to_matrix(evt: Message, source: 'AbstractUser') -> Optional[RelatesTo]:
     if evt.reply_to:
         space = (evt.peer_id.channel_id
                  if isinstance(evt, Message) and isinstance(evt.peer_id, PeerChannel)
                  else source.tgid)
         msg = DBMessage.get_one_by_tgid(TelegramID(evt.reply_to.reply_to_msg_id), space)
         if msg:
-            return RelatesTo(rel_type=RelationType.REFERENCE, event_id=msg.mxid)
+            return RelatesTo(rel_type=RelationType.REPLY, event_id=msg.mxid)
     return None
 
 
 async def _add_forward_header(source: 'AbstractUser', content: TextMessageEventContent,
                               fwd_from: MessageFwdHeader) -> None:
     if not content.formatted_body or content.format != Format.HTML:
         content.format = Format.HTML
@@ -122,15 +122,15 @@
              if isinstance(evt, Message) and isinstance(evt.peer_id, PeerChannel)
              else source.tgid)
 
     msg = DBMessage.get_one_by_tgid(TelegramID(evt.reply_to.reply_to_msg_id), space)
     if not msg:
         return
 
-    content.relates_to = RelatesTo(rel_type=RelationType.REFERENCE, event_id=msg.mxid)
+    content.relates_to = RelatesTo(rel_type=RelationType.REPLY, event_id=msg.mxid)
 
     try:
         event: MessageEvent = await main_intent.get_event(msg.mx_room, msg.mxid)
         if isinstance(event.content, TextMessageEventContent):
             event.content.trim_reply_fallback()
         puppet = await pu.Puppet.get_by_mxid(event.sender, create=False)
         content.set_reply(event, displayname=puppet.displayname if puppet else event.sender)
```

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/get_version.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/get_version.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/matrix.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/matrix.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/__init__.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/__init__.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/base.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/base.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/deduplication.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/deduplication.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/matrix.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,34 +9,34 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU Affero General Public License for more details.
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
-from typing import Awaitable, Dict, List, Optional, Tuple, Union, Any, TYPE_CHECKING
+from typing import Awaitable, Dict, Optional, Union, Any, TYPE_CHECKING
 from html import escape as escape_html
 from string import Template
 from abc import ABC
 
 import magic
 
 from telethon.tl.functions.messages import (EditChatPhotoRequest, EditChatTitleRequest,
                                             UpdatePinnedMessageRequest, SetTypingRequest,
                                             EditChatAboutRequest)
 from telethon.tl.functions.channels import EditPhotoRequest, EditTitleRequest, JoinChannelRequest
 from telethon.errors import (ChatNotModifiedError, PhotoExtInvalidError,
                              PhotoInvalidDimensionsError, PhotoSaveFileInvalidError,
                              RPCError)
 from telethon.tl.patched import Message, MessageService
-from telethon.tl.types import (
-    DocumentAttributeFilename, DocumentAttributeImageSize, GeoPoint,
-    InputChatUploadedPhoto, MessageActionChatEditPhoto, MessageMediaGeo,
-    SendMessageCancelAction, SendMessageTypingAction, TypeInputPeer, TypeMessageEntity,
-    UpdateNewMessage, InputMediaUploadedDocument, InputMediaUploadedPhoto)
+from telethon.tl.types import (DocumentAttributeFilename, DocumentAttributeImageSize, GeoPoint,
+                               InputChatUploadedPhoto, MessageActionChatEditPhoto, MessageMediaGeo,
+                               SendMessageCancelAction, SendMessageTypingAction, TypeInputPeer,
+                               UpdateNewMessage, InputMediaUploadedDocument,
+                               InputMediaUploadedPhoto)
 
 from mautrix.types import (EventID, RoomID, UserID, ContentURI, MessageType, MessageEventContent,
                            TextMessageEventContent, MediaMessageEventContent, Format,
                            LocationMessageEventContent, ImageInfo, VideoInfo)
 
 from ..types import TelegramID
 from ..db import Message as DBMessage
@@ -83,15 +83,15 @@
             return
         elif self.peer_type == "user" and not config["bridge.relaybot.private_chat.state_changes"]:
             return
         async with self.send_lock(self.bot.tgid):
             message = await self._get_state_change_message(event, user, **kwargs)
             if not message:
                 return
-            message, entities = formatter.matrix_to_telegram(message)
+            message, entities = await formatter.matrix_to_telegram(self.bot.client, html=message)
             response = await self.bot.client.send_message(self.peer, message,
                                                           formatting_entities=entities)
             space = self.tgid if self.peer_type == "channel" else self.bot.tgid
             self.dedup.check(response, (event_id, space))
 
     async def name_change_matrix(self, user: 'u.User', displayname: str, prev_displayname: str,
                                  event_id: EventID) -> None:
@@ -210,35 +210,19 @@
     async def _pre_process_matrix_message(self, sender: 'u.User', use_relaybot: bool,
                                           content: MessageEventContent) -> None:
         if use_relaybot:
             await self._apply_msg_format(sender, content)
         elif content.msgtype == MessageType.EMOTE:
             await self._apply_emote_format(sender, content)
 
-    @staticmethod
-    def _matrix_event_to_entities(event: Union[str, MessageEventContent]
-                                  ) -> Tuple[str, Optional[List[TypeMessageEntity]]]:
-        try:
-            if isinstance(event, str):
-                message, entities = formatter.matrix_to_telegram(event)
-            elif isinstance(event, TextMessageEventContent) and event.format == Format.HTML:
-                message, entities = formatter.matrix_to_telegram(event.formatted_body)
-            else:
-                message, entities = formatter.matrix_text_to_telegram(event.body)
-        except KeyError:
-            message, entities = None, None
-        return message, entities
-
     async def _handle_matrix_text(self, sender_id: TelegramID, event_id: EventID,
                                   space: TelegramID, client: 'MautrixTelegramClient',
                                   content: TextMessageEventContent, reply_to: TelegramID) -> None:
-        if content.formatted_body and content.format == Format.HTML:
-            message, entities = formatter.matrix_to_telegram(content.formatted_body)
-        else:
-            message, entities = formatter.matrix_text_to_telegram(content.body)
+        message, entities = await formatter.matrix_to_telegram(client, text=content.body,
+                                                               html=content.formatted(Format.HTML))
         async with self.send_lock(sender_id):
             lp = self.get_config("telegram_link_preview")
             if content.get_edit():
                 orig_msg = DBMessage.get_by_mxid(content.get_edit(), self.mxid, space)
                 if orig_msg:
                     response = await client.edit_message(self.peer, orig_msg.tgid, message,
                                                          formatting_entities=entities,
@@ -297,33 +281,29 @@
 
         if (mime == "image/png" or mime == "image/jpeg") and file_size < max_image_size:
             media = InputMediaUploadedPhoto(file_handle)
         else:
             media = InputMediaUploadedDocument(file=file_handle, attributes=attributes,
                                                mime_type=mime or "application/octet-stream")
 
-        if caption:
-            if caption.formatted_body and caption.format == Format.HTML:
-                caption, entities = formatter.matrix_to_telegram(caption.formatted_body)
-            else:
-                caption, entities = formatter.matrix_text_to_telegram(caption.body)
-        else:
-            caption, entities = None, None
+        capt, entities = (await formatter.matrix_to_telegram(client, text=caption.body,
+                                                             html=caption.formatted(Format.HTML))
+                          if caption else (None, None))
 
         async with self.send_lock(sender_id):
-            if await self._matrix_document_edit(client, content, space, caption, media, event_id):
+            if await self._matrix_document_edit(client, content, space, capt, media, event_id):
                 return
             try:
                 response = await client.send_media(self.peer, media, reply_to=reply_to,
-                                                   caption=caption, entities=entities)
+                                                   caption=capt, entities=entities)
             except (PhotoInvalidDimensionsError, PhotoSaveFileInvalidError, PhotoExtInvalidError):
                 media = InputMediaUploadedDocument(file=media.file, mime_type=mime,
                                                    attributes=attributes)
                 response = await client.send_media(self.peer, media, reply_to=reply_to,
-                                                   caption=caption, entities=entities)
+                                                   caption=capt, entities=entities)
             self._add_telegram_message_to_db(event_id, space, 0, response)
         await self._send_delivery_receipt(event_id)
 
     async def _matrix_document_edit(self, client: 'MautrixTelegramClient',
                                     content: MessageEventContent, space: TelegramID,
                                     caption: str, media: Any, event_id: EventID) -> bool:
         if content.get_edit():
@@ -342,15 +322,15 @@
                                       ) -> None:
         try:
             lat, long = content.geo_uri[len("geo:"):].split(",")
             lat, long = float(lat), float(long)
         except (KeyError, ValueError):
             self.log.exception("Failed to parse location")
             return None
-        caption, entities = formatter.matrix_text_to_telegram(content.body)
+        caption, entities = await formatter.matrix_to_telegram(client, text=content.body)
         media = MessageMediaGeo(geo=GeoPoint(lat, long, access_hash=0))
 
         async with self.send_lock(sender_id):
             if await self._matrix_document_edit(client, content, space, caption, media, event_id):
                 return
             response = await client.send_media(self.peer, media, reply_to=reply_to,
                                                caption=caption, entities=entities)
```

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/metadata.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/metadata.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/send_lock.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/send_lock.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/portal/telegram.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/portal/telegram.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/puppet.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/puppet.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/dbms_migrate/__main__.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/dbms_migrate/__main__.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/telematrix_import/__main__.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/telematrix_import/__main__.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/scripts/telematrix_import/models.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/scripts/telematrix_import/models.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/tgclient.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/tgclient.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/user.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/user.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/util/color_log.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/util/color_log.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/util/file_transfer.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/util/file_transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from telethon.tl.types import (Document, InputFileLocation, InputDocumentFileLocation,
                                TypePhotoSize, PhotoSize, PhotoCachedSize, InputPhotoFileLocation,
                                InputPeerPhotoFileLocation)
 from telethon.errors import (AuthBytesInvalidError, AuthKeyInvalidError, LocationInvalidError,
                              SecurityError, FileIdInvalidError)
 
 from mautrix.appservice import IntentAPI
-from mautrix.types import EncryptedFile
+from mautrix.util.network_retry import call_with_net_retry
 
 from ..tgclient import MautrixTelegramClient
 from ..db import TelegramFile as DBTelegramFile
 from ..util import sane_mimetypes
 from .parallel_file_transfer import parallel_transfer_to_matrix
 from .tgs_converter import convert_tgs_to
 
@@ -141,15 +141,16 @@
         mime_type = magic.from_buffer(file, mime=True)
 
     decryption_info = None
     upload_mime_type = mime_type
     if encrypt:
         file, decryption_info = encrypt_attachment(file)
         upload_mime_type = "application/octet-stream"
-    content_uri = await intent.upload_media(file, upload_mime_type)
+    content_uri = await call_with_net_retry(intent.upload_media, file, upload_mime_type,
+                                            _action="upload media")
     if decryption_info:
         decryption_info.url = content_uri
 
     db_file = DBTelegramFile(id=loc_id, mxc=content_uri, mime_type=mime_type,
                              was_converted=False, timestamp=int(time.time()), size=len(file),
                              width=width, height=height, decryption_info=decryption_info)
     try:
@@ -242,15 +243,16 @@
             thumbnail = None
 
         decryption_info = None
         upload_mime_type = mime_type
         if encrypt and encrypt_attachment:
             file, decryption_info = encrypt_attachment(file)
             upload_mime_type = "application/octet-stream"
-        content_uri = await intent.upload_media(file, upload_mime_type)
+        content_uri = await call_with_net_retry(intent.upload_media, file, upload_mime_type,
+                                                _action="upload media")
         if decryption_info:
             decryption_info.url = content_uri
 
         db_file = DBTelegramFile(id=loc_id, mxc=content_uri, decryption_info=decryption_info,
                                  mime_type=mime_type, was_converted=image_converted,
                                  timestamp=int(time.time()), size=len(file),
                                  width=width, height=height)
```

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/util/format_duration.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/util/format_duration.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/util/parallel_file_transfer.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/util/parallel_file_transfer.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/util/recursive_dict.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/util/recursive_dict.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/util/sane_mimetypes.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/util/sane_mimetypes.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/util/tgs_converter.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/util/tgs_converter.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/web/common/auth_api.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/web/common/auth_api.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/web/provisioning/__init__.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/web/provisioning/__init__.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/__init__.py` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/__init__.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/favicon.png` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/favicon.png`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/login.css` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/login.css`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/login.html.mako` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/login.html.mako`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram/web/public/matrix-login.html.mako` & `mautrix-telegram-0.9.0rc3/mautrix_telegram/web/public/matrix-login.html.mako`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/PKG-INFO` & `mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mautrix-telegram
-Version: 0.9.0rc2
+Version: 0.9.0rc3
 Summary: A Matrix-Telegram hybrid puppeting/relaybot bridge.
 Home-page: https://github.com/tulir/mautrix-telegram
 Author: Tulir Asokan
 Author-email: tulir@maunium.net
 License: UNKNOWN
 Description: # mautrix-telegram
         ![Languages](https://img.shields.io/github/languages/top/tulir/mautrix-telegram.svg)
```

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/SOURCES.txt` & `mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/mautrix_telegram.egg-info/requires.txt` & `mautrix-telegram-0.9.0rc3/mautrix_telegram.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 SQLAlchemy<2,>=1.2
 aiohttp<4,>=3
 alembic<2,>=1
 commonmark<0.10,>=0.8
-mautrix==0.8.0rc5
+mautrix<0.9,>=0.8.2
 python-magic<0.5,>=0.4
 ruamel.yaml<0.17,>=0.15.35
 telethon-session-sqlalchemy<0.3,>=0.2.14
 telethon<1.18,>=1.17
 yarl<2,>=1
 
 [all]
```

### Comparing `mautrix-telegram-0.9.0rc2/setup.py` & `mautrix-telegram-0.9.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/tests/commands/test_handler.py` & `mautrix-telegram-0.9.0rc3/tests/commands/test_handler.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/tests/utils/fixtures.py` & `mautrix-telegram-0.9.0rc3/tests/utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `mautrix-telegram-0.9.0rc2/tests/utils/helpers.py` & `mautrix-telegram-0.9.0rc3/tests/utils/helpers.py`

 * *Files identical despite different names*

