# Comparing `tmp/swibots-1.2.8.tar.gz` & `tmp/swibots-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swibots-1.2.8.tar", last modified: Wed Jun 21 02:23:10 2023, max compression
+gzip compressed data, was "swibots-1.2.9.tar", last modified: Mon Jun 26 12:41:30 2023, max compression
```

## Comparing `swibots-1.2.8.tar` & `swibots-1.2.9.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.822942 swibots-1.2.8/
--rw-r--r--   0 root         (0) root         (0)     1817 2023-06-21 02:23:10.822942 swibots-1.2.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1538 2023-06-21 00:14:53.000000 swibots-1.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 02:23:10.826942 swibots-1.2.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      731 2023-06-21 02:23:08.000000 swibots-1.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.750942 swibots-1.2.8/swibots/
--rw-rw-r--   0 root         (0) root         (0)      236 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.754942 swibots-1.2.8/swibots/api/
--rw-rw-r--   0 root         (0) root         (0)      140 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2236 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.754942 swibots-1.2.8/swibots/api/auth/
--rw-rw-r--   0 root         (0) root         (0)       85 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1220 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/auth_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.754942 swibots-1.2.8/swibots/api/auth/controllers/
--rw-rw-r--   0 root         (0) root         (0)       73 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/controllers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1514 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/controllers/user_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.754942 swibots-1.2.8/swibots/api/auth/methods/
--rwxrwxr-x   0 root         (0) root         (0)       94 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/methods/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      650 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/methods/get_me.py
--rw-rw-r--   0 root         (0) root         (0)      837 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/methods/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.758942 swibots-1.2.8/swibots/api/auth/models/
--rw-rw-r--   0 root         (0) root         (0)       56 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4642 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/auth/models/auth_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.758942 swibots-1.2.8/swibots/api/bot/
--rwxrwxr-x   0 root         (0) root         (0)       83 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1141 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/bot_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.758942 swibots-1.2.8/swibots/api/bot/controllers/
--rw-rw-r--   0 root         (0) root         (0)       71 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/controllers/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1790 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/controllers/bot_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.762942 swibots-1.2.8/swibots/api/bot/methods/
--rwxrwxr-x   0 root         (0) root         (0)      209 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/methods/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      540 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/methods/delete_bot_info.py
--rwxrwxr-x   0 root         (0) root         (0)      582 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/methods/get_bot_info.py
--rwxrwxr-x   0 root         (0) root         (0)      615 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/methods/update_bot_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.762942 swibots-1.2.8/swibots/api/bot/models/
--rwxrwxr-x   0 root         (0) root         (0)      116 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/models/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      955 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/models/bot_command_info.py
--rwxrwxr-x   0 root         (0) root         (0)     1585 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/bot/models/bot_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.762942 swibots-1.2.8/swibots/api/chat/
--rw-rw-r--   0 root         (0) root         (0)      107 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5372 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/chat_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.762942 swibots-1.2.8/swibots/api/chat/controllers/
--rw-rw-r--   0 root         (0) root         (0)       83 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/controllers/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)    21518 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/controllers/message_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.766942 swibots-1.2.8/swibots/api/chat/events/
--rwxrwxr-x   0 root         (0) root         (0)      326 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/events/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2073 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/events/callback_query_event.py
--rwxrwxr-x   0 root         (0) root         (0)     2731 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/events/chat_event.py
--rwxrwxr-x   0 root         (0) root         (0)     2095 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/events/command_event.py
--rwxrwxr-x   0 root         (0) root         (0)     2103 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/events/inline_query_event.py
--rwxrwxr-x   0 root         (0) root         (0)     2434 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/events/message_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.778942 swibots-1.2.8/swibots/api/chat/methods/
--rwxrwxr-x   0 root         (0) root         (0)     1709 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      654 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/answer_inline_query.py
--rwxrwxr-x   0 root         (0) root         (0)      693 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/clear_conversation.py
--rwxrwxr-x   0 root         (0) root         (0)      705 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/delete_message.py
--rwxrwxr-x   0 root         (0) root         (0)      707 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/delete_messages_from_user.py
--rwxrwxr-x   0 root         (0) root         (0)     1358 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/download_media.py
--rwxrwxr-x   0 root         (0) root         (0)      750 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/edit_message.py
--rwxrwxr-x   0 root         (0) root         (0)      853 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/edit_message_text.py
--rwxrwxr-x   0 root         (0) root         (0)      693 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/flag_message.py
--rwxrwxr-x   0 root         (0) root         (0)     1192 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/forward_message.py
--rwxrwxr-x   0 root         (0) root         (0)     1139 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_channel_chat_history.py
--rwxrwxr-x   0 root         (0) root         (0)      725 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_community_media_files.py
--rwxrwxr-x   0 root         (0) root         (0)      883 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_community_media_files_by_status.py
--rwxrwxr-x   0 root         (0) root         (0)      636 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_flag_messages.py
--rwxrwxr-x   0 root         (0) root         (0)     1090 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_group_chat_history.py
--rwxrwxr-x   0 root         (0) root         (0)      649 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_message.py
--rwxrwxr-x   0 root         (0) root         (0)      707 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_messages.py
--rwxrwxr-x   0 root         (0) root         (0)     1102 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_messages_between_users.py
--rwxrwxr-x   0 root         (0) root         (0)      560 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_unread_messages_count.py
--rwxrwxr-x   0 root         (0) root         (0)      785 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/get_user_media_files.py
--rwxrwxr-x   0 root         (0) root         (0)      881 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/reply_message.py
--rwxrwxr-x   0 root         (0) root         (0)     1032 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/reply_message_text.py
--rwxrwxr-x   0 root         (0) root         (0)      849 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/send_message.py
--rwxrwxr-x   0 root         (0) root         (0)     1136 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/methods/send_text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.782942 swibots-1.2.8/swibots/api/chat/models/
--rw-rw-r--   0 root         (0) root         (0)      305 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      920 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/group_chat_history.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.786942 swibots-1.2.8/swibots/api/chat/models/inline/
--rwxrwxr-x   0 root         (0) root         (0)      565 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1371 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/base_typed_inline_query_result.py
--rwxrwxr-x   0 root         (0) root         (0)     2533 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/inline_query.py
--rwxrwxr-x   0 root         (0) root         (0)     1871 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/inline_query_answer.py
--rwxrwxr-x   0 root         (0) root         (0)      991 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result.py
--rwxrwxr-x   0 root         (0) root         (0)     1158 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result_article.py
--rw-rw-r--   0 root         (0) root         (0)     1273 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result_document.py
--rw-rw-r--   0 root         (0) root         (0)     1620 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result_photo.py
--rw-rw-r--   0 root         (0) root         (0)     1760 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result_video.py
--rwxrwxr-x   0 root         (0) root         (0)      581 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/input_message_content.py
--rwxrwxr-x   0 root         (0) root         (0)      201 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline/types.py
--rwxrwxr-x   0 root         (0) root         (0)      886 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline_keyboard_button.py
--rwxrwxr-x   0 root         (0) root         (0)      170 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline_keyboard_color.py
--rwxrwxr-x   0 root         (0) root         (0)      146 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline_keyboard_size.py
--rwxrwxr-x   0 root         (0) root         (0)     2065 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/chat/models/inline_markup.py
--rw-rw-r--   0 root         (0) root         (0)    10888 2023-06-21 02:07:01.000000 swibots-1.2.8/swibots/api/chat/models/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.786942 swibots-1.2.8/swibots/api/common/
--rwxrwxr-x   0 root         (0) root         (0)       44 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.786942 swibots-1.2.8/swibots/api/common/events/
--rwxrwxr-x   0 root         (0) root         (0)       46 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/common/events/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2789 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/common/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.786942 swibots-1.2.8/swibots/api/common/models/
--rwxrwxr-x   0 root         (0) root         (0)      101 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/common/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2004 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/common/models/media.py
--rwxrwxr-x   0 root         (0) root         (0)     1565 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/common/models/media_upload_request.py
--rwxrwxr-x   0 root         (0) root         (0)     1706 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/common/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.790942 swibots-1.2.8/swibots/api/community/
--rwxrwxr-x   0 root         (0) root         (0)       90 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5059 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/community_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.790942 swibots-1.2.8/swibots/api/community/controllers/
--rw-rw-r--   0 root         (0) root         (0)      102 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/controllers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      595 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/controllers/channel_controller.py
--rwxrwxr-x   0 root         (0) root         (0)      616 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/controllers/community_controller.py
--rw-rw-r--   0 root         (0) root         (0)      576 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/controllers/group_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.794942 swibots-1.2.8/swibots/api/community/events/
--rwxrwxr-x   0 root         (0) root         (0)      566 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1387 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/channel_created_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1387 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/channel_deleted_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1387 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/channel_updated_event.py
--rwxrwxr-x   0 root         (0) root         (0)     2303 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/community_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1383 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/community_updated_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1381 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/group_created_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1381 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/group_deleted_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1381 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/group_updated_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1380 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/member_joined_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1377 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/member_left_event.py
--rwxrwxr-x   0 root         (0) root         (0)     1373 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/events/user_banned_event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.798942 swibots-1.2.8/swibots/api/community/methods/
--rwxrwxr-x   0 root         (0) root         (0)      194 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/methods/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      643 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/methods/get_channel.py
--rwxrwxr-x   0 root         (0) root         (0)      668 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/methods/get_community.py
--rw-rw-r--   0 root         (0) root         (0)      619 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/methods/get_group.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.798942 swibots-1.2.8/swibots/api/community/models/
--rwxrwxr-x   0 root         (0) root         (0)      132 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/models/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2743 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/models/channel.py
--rwxrwxr-x   0 root         (0) root         (0)     2954 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/models/community.py
--rwxrwxr-x   0 root         (0) root         (0)     2720 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/api/community/models/group.py
--rwxrwxr-x   0 root         (0) root         (0)     9347 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.802942 swibots-1.2.8/swibots/base/
--rw-rw-r--   0 root         (0) root         (0)      262 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/base/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       69 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/base/rest_controller.py
--rw-rw-r--   0 root         (0) root         (0)      370 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/base/rest_request.py
--rw-rw-r--   0 root         (0) root         (0)      644 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/base/rest_response.py
--rw-rw-r--   0 root         (0) root         (0)     4261 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/base/switch_client.py
--rw-rw-r--   0 root         (0) root         (0)     1180 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/base/switch_object.py
--rwxrwxr-x   0 root         (0) root         (0)      543 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/base/switch_ws_async_client.py
--rwxrwxr-x   0 root         (0) root         (0)     4598 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bot_app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.806942 swibots-1.2.8/swibots/bots/
--rwxrwxr-x   0 root         (0) root         (0)      201 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     4646 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/bot.py
--rwxrwxr-x   0 root         (0) root         (0)     1646 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/bot_context.py
--rwxrwxr-x   0 root         (0) root         (0)      109 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.810942 swibots-1.2.8/swibots/bots/decorators/
--rwxrwxr-x   0 root         (0) root         (0)      999 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)      540 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_callback_query.py
--rwxrwxr-x   0 root         (0) root         (0)      510 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_channel_created.py
--rwxrwxr-x   0 root         (0) root         (0)      544 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_channel_deleted.py
--rwxrwxr-x   0 root         (0) root         (0)      541 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_channel_updated.py
--rwxrwxr-x   0 root         (0) root         (0)      574 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_command.py
--rwxrwxr-x   0 root         (0) root         (0)      544 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_community_updated.py
--rwxrwxr-x   0 root         (0) root         (0)      536 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_group_created.py
--rwxrwxr-x   0 root         (0) root         (0)      536 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_group_deleted.py
--rwxrwxr-x   0 root         (0) root         (0)      534 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_group_updated.py
--rw-rw-r--   0 root         (0) root         (0)      537 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_inline_query.py
--rwxrwxr-x   0 root         (0) root         (0)      534 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_member_joined.py
--rwxrwxr-x   0 root         (0) root         (0)      529 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_member_left.py
--rwxrwxr-x   0 root         (0) root         (0)      503 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_message.py
--rwxrwxr-x   0 root         (0) root         (0)      543 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_unknown_command.py
--rwxrwxr-x   0 root         (0) root         (0)      509 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/decorators/on_user_banned.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.810942 swibots-1.2.8/swibots/bots/filters/
--rwxrwxr-x   0 root         (0) root         (0)       22 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/filters/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     7785 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/filters/filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.818942 swibots-1.2.8/swibots/bots/handlers/
--rwxrwxr-x   0 root         (0) root         (0)     1300 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     1048 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/base_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      985 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/callback_query_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      681 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/channel_created_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      688 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/channel_deleted_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      734 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/channel_updated_handler.py
--rwxrwxr-x   0 root         (0) root         (0)     1514 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/command_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      686 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/community_updated_handler.py
--rwxrwxr-x   0 root         (0) root         (0)     1325 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/event_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      680 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/group_created_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      775 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/group_deleted_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      775 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/group_updated_handler.py
--rw-rw-r--   0 root         (0) root         (0)      867 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/inline_query_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      679 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/member_joined_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      674 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/member_left_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      960 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/message_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      885 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/unknown_command_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      670 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/handlers/user_banned_handler.py
--rwxrwxr-x   0 root         (0) root         (0)      285 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/bots/register_command.py
--rwxrwxr-x   0 root         (0) root         (0)     1621 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/config.py
--rw-rw-r--   0 root         (0) root         (0)     1333 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/error.py
--rwxrwxr-x   0 root         (0) root         (0)      854 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.822942 swibots-1.2.8/swibots/utils/
--rw-rw-r--   0 root         (0) root         (0)       75 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5880 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/rest_client.py
--rw-rw-r--   0 root         (0) root         (0)     2475 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.822942 swibots-1.2.8/swibots/utils/ws/
--rw-rw-r--   0 root         (0) root         (0)       48 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/ws/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.822942 swibots-1.2.8/swibots/utils/ws/asyncstomp/
--rw-rw-r--   0 root         (0) root         (0)      150 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/ws/asyncstomp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9787 2023-06-21 02:01:49.000000 swibots-1.2.8/swibots/utils/ws/asyncstomp/async_ws_client.py
--rw-rw-r--   0 root         (0) root         (0)      980 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/ws/asyncstomp/async_ws_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.822942 swibots-1.2.8/swibots/utils/ws/common/
--rw-rw-r--   0 root         (0) root         (0)      100 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/ws/common/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1654 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/ws/common/ws_frame.py
--rw-rw-r--   0 root         (0) root         (0)      430 2023-06-21 00:14:53.000000 swibots-1.2.8/swibots/utils/ws/common/ws_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 02:23:10.754942 swibots-1.2.8/swibots.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1817 2023-06-21 02:23:10.000000 swibots-1.2.8/swibots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7283 2023-06-21 02:23:10.000000 swibots-1.2.8/swibots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 02:23:10.000000 swibots-1.2.8/swibots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-21 02:23:10.000000 swibots-1.2.8/swibots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-21 02:23:10.000000 swibots-1.2.8/swibots.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.148310 swibots-1.2.9/
+-rw-rw-rw-   0        0        0     1892 2023-06-26 12:41:30.146306 swibots-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1601 2023-06-26 07:52:28.000000 swibots-1.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 12:41:30.149311 swibots-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-06-26 07:56:28.000000 swibots-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.726901 swibots-1.2.9/swibots/
+-rw-rw-rw-   0        0        0      247 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.742903 swibots-1.2.9/swibots/api/
+-rw-rw-rw-   0        0        0      146 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/__init__.py
+-rw-rw-rw-   0        0        0     2317 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.747900 swibots-1.2.9/swibots/api/auth/
+-rw-rw-rw-   0        0        0       88 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/auth_client.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.752902 swibots-1.2.9/swibots/api/auth/controllers/
+-rw-rw-rw-   0        0        0       75 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/controllers/__init__.py
+-rw-rw-rw-   0        0        0     1565 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/controllers/user_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.758901 swibots-1.2.9/swibots/api/auth/methods/
+-rw-rw-rw-   0        0        0       99 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/methods/__init__.py
+-rw-rw-rw-   0        0        0      671 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/methods/get_me.py
+-rw-rw-rw-   0        0        0      861 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/methods/login.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.764902 swibots-1.2.9/swibots/api/auth/models/
+-rw-rw-rw-   0        0        0       59 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/models/__init__.py
+-rw-rw-rw-   0        0        0     4765 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/auth/models/auth_user.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.769902 swibots-1.2.9/swibots/api/bot/
+-rw-rw-rw-   0        0        0       86 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/__init__.py
+-rw-rw-rw-   0        0        0     1177 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/bot_client.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.773900 swibots-1.2.9/swibots/api/bot/controllers/
+-rw-rw-rw-   0        0        0       74 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/controllers/__init__.py
+-rw-rw-rw-   0        0        0     1852 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/controllers/bot_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.784898 swibots-1.2.9/swibots/api/bot/methods/
+-rw-rw-rw-   0        0        0      220 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/methods/__init__.py
+-rw-rw-rw-   0        0        0      557 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/methods/delete_bot_info.py
+-rw-rw-rw-   0        0        0      600 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/methods/get_bot_info.py
+-rw-rw-rw-   0        0        0      633 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/methods/update_bot_info.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.790899 swibots-1.2.9/swibots/api/bot/models/
+-rw-rw-rw-   0        0        0      120 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/models/__init__.py
+-rw-rw-rw-   0        0        0      987 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/models/bot_command_info.py
+-rw-rw-rw-   0        0        0     1633 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/bot/models/bot_info.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.795907 swibots-1.2.9/swibots/api/chat/
+-rw-rw-rw-   0        0        0      111 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/__init__.py
+-rw-rw-rw-   0        0        0     5512 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/chat_client.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.801900 swibots-1.2.9/swibots/api/chat/controllers/
+-rw-rw-rw-   0        0        0       86 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/controllers/__init__.py
+-rw-rw-rw-   0        0        0    22044 2023-06-26 12:37:56.000000 swibots-1.2.9/swibots/api/chat/controllers/message_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.817901 swibots-1.2.9/swibots/api/chat/events/
+-rw-rw-rw-   0        0        0      334 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/events/__init__.py
+-rw-rw-rw-   0        0        0     2134 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/events/callback_query_event.py
+-rw-rw-rw-   0        0        0     2809 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/events/chat_event.py
+-rw-rw-rw-   0        0        0     2157 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/events/command_event.py
+-rw-rw-rw-   0        0        0     2166 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/events/inline_query_event.py
+-rw-rw-rw-   0        0        0     2503 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/events/message_event.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.882901 swibots-1.2.9/swibots/api/chat/methods/
+-rw-rw-rw-   0        0        0     1761 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/__init__.py
+-rw-rw-rw-   0        0        0      668 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/answer_inline_query.py
+-rw-rw-rw-   0        0        0      714 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/clear_conversation.py
+-rw-rw-rw-   0        0        0      726 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/delete_message.py
+-rw-rw-rw-   0        0        0      728 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/delete_messages_from_user.py
+-rw-rw-rw-   0        0        0     1392 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/download_media.py
+-rw-rw-rw-   0        0        0      774 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/edit_message.py
+-rw-rw-rw-   0        0        0      877 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/edit_message_text.py
+-rw-rw-rw-   0        0        0      714 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/flag_message.py
+-rw-rw-rw-   0        0        0     1223 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/forward_message.py
+-rw-rw-rw-   0        0        0     1172 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_channel_chat_history.py
+-rw-rw-rw-   0        0        0      748 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_community_media_files.py
+-rw-rw-rw-   0        0        0      909 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_community_media_files_by_status.py
+-rw-rw-rw-   0        0        0      655 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_flag_messages.py
+-rw-rw-rw-   0        0        0     1122 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_group_chat_history.py
+-rw-rw-rw-   0        0        0      670 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_message.py
+-rw-rw-rw-   0        0        0      728 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_messages.py
+-rw-rw-rw-   0        0        0     1134 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_messages_between_users.py
+-rw-rw-rw-   0        0        0      576 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_unread_messages_count.py
+-rw-rw-rw-   0        0        0      810 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/get_user_media_files.py
+-rw-rw-rw-   0        0        0      906 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/reply_message.py
+-rw-rw-rw-   0        0        0     1058 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/reply_message_text.py
+-rw-rw-rw-   0        0        0      874 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/send_message.py
+-rw-rw-rw-   0        0        0     1163 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/methods/send_text.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.899899 swibots-1.2.9/swibots/api/chat/models/
+-rw-rw-rw-   0        0        0      312 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/__init__.py
+-rw-rw-rw-   0        0        0      951 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/group_chat_history.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.925901 swibots-1.2.9/swibots/api/chat/models/inline/
+-rw-rw-rw-   0        0        0      575 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/__init__.py
+-rw-rw-rw-   0        0        0     1410 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/base_typed_inline_query_result.py
+-rw-rw-rw-   0        0        0     2605 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/inline_query.py
+-rw-rw-rw-   0        0        0     1931 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/inline_query_answer.py
+-rw-rw-rw-   0        0        0     1021 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result.py
+-rw-rw-rw-   0        0        0     1190 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result_article.py
+-rw-rw-rw-   0        0        0     1308 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result_document.py
+-rw-rw-rw-   0        0        0     1664 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result_photo.py
+-rw-rw-rw-   0        0        0     1807 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result_video.py
+-rw-rw-rw-   0        0        0      603 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/input_message_content.py
+-rw-rw-rw-   0        0        0      211 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline/types.py
+-rw-rw-rw-   0        0        0      919 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline_keyboard_button.py
+-rw-rw-rw-   0        0        0      180 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline_keyboard_color.py
+-rw-rw-rw-   0        0        0      154 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline_keyboard_size.py
+-rw-rw-rw-   0        0        0     2123 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/chat/models/inline_markup.py
+-rw-rw-rw-   0        0        0    12171 2023-06-26 11:54:49.000000 swibots-1.2.9/swibots/api/chat/models/message.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.929899 swibots-1.2.9/swibots/api/common/
+-rw-rw-rw-   0        0        0       46 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.933899 swibots-1.2.9/swibots/api/common/events/
+-rw-rw-rw-   0        0        0       49 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/common/events/__init__.py
+-rw-rw-rw-   0        0        0     2859 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/common/events/event.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.942898 swibots-1.2.9/swibots/api/common/models/
+-rw-rw-rw-   0        0        0      104 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/common/models/__init__.py
+-rw-rw-rw-   0        0        0     2061 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/common/models/media.py
+-rw-rw-rw-   0        0        0     1624 2023-06-26 12:38:24.000000 swibots-1.2.9/swibots/api/common/models/media_upload_request.py
+-rw-rw-rw-   0        0        0     1759 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/common/models/user.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.947899 swibots-1.2.9/swibots/api/community/
+-rw-rw-rw-   0        0        0       93 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/__init__.py
+-rw-rw-rw-   0        0        0     5180 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/community_client.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.955898 swibots-1.2.9/swibots/api/community/controllers/
+-rw-rw-rw-   0        0        0      105 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/controllers/__init__.py
+-rw-rw-rw-   0        0        0      618 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/controllers/channel_controller.py
+-rw-rw-rw-   0        0        0      636 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/controllers/community_controller.py
+-rw-rw-rw-   0        0        0      596 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/controllers/group_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.984899 swibots-1.2.9/swibots/api/community/events/
+-rw-rw-rw-   0        0        0      577 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/channel_created_event.py
+-rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/channel_deleted_event.py
+-rw-rw-rw-   0        0        0     1428 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/channel_updated_event.py
+-rw-rw-rw-   0        0        0     2373 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/community_event.py
+-rw-rw-rw-   0        0        0     1424 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/community_updated_event.py
+-rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/group_created_event.py
+-rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/group_deleted_event.py
+-rw-rw-rw-   0        0        0     1422 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/group_updated_event.py
+-rw-rw-rw-   0        0        0     1421 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/member_joined_event.py
+-rw-rw-rw-   0        0        0     1418 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/member_left_event.py
+-rw-rw-rw-   0        0        0     1414 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/events/user_banned_event.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.995906 swibots-1.2.9/swibots/api/community/methods/
+-rw-rw-rw-   0        0        0      205 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/methods/__init__.py
+-rw-rw-rw-   0        0        0      664 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/methods/get_channel.py
+-rw-rw-rw-   0        0        0      689 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/methods/get_community.py
+-rw-rw-rw-   0        0        0      640 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/methods/get_group.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.005296 swibots-1.2.9/swibots/api/community/models/
+-rw-rw-rw-   0        0        0      137 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/models/__init__.py
+-rw-rw-rw-   0        0        0     2814 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/models/channel.py
+-rw-rw-rw-   0        0        0     3033 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/models/community.py
+-rw-rw-rw-   0        0        0     2792 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/api/community/models/group.py
+-rw-rw-rw-   0        0        0     9630 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/app.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.021307 swibots-1.2.9/swibots/base/
+-rw-rw-rw-   0        0        0      268 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/base/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/base/rest_controller.py
+-rw-rw-rw-   0        0        0      386 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/base/rest_request.py
+-rw-rw-rw-   0        0        0      669 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/base/rest_response.py
+-rw-rw-rw-   0        0        0     4380 2023-06-26 11:37:39.000000 swibots-1.2.9/swibots/base/switch_client.py
+-rw-rw-rw-   0        0        0     1221 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/base/switch_object.py
+-rw-rw-rw-   0        0        0      563 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/base/switch_ws_async_client.py
+-rw-rw-rw-   0        0        0     4734 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bot_app.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.032307 swibots-1.2.9/swibots/bots/
+-rw-rw-rw-   0        0        0      208 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/__init__.py
+-rw-rw-rw-   0        0        0     4782 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/bot.py
+-rw-rw-rw-   0        0        0     1690 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/bot_context.py
+-rw-rw-rw-   0        0        0      111 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.071307 swibots-1.2.9/swibots/bots/decorators/
+-rw-rw-rw-   0        0        0     1034 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_callback_query.py
+-rw-rw-rw-   0        0        0      526 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_channel_created.py
+-rw-rw-rw-   0        0        0      562 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_channel_deleted.py
+-rw-rw-rw-   0        0        0      559 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_channel_updated.py
+-rw-rw-rw-   0        0        0      593 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_command.py
+-rw-rw-rw-   0        0        0      562 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_community_updated.py
+-rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_group_created.py
+-rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_group_deleted.py
+-rw-rw-rw-   0        0        0      552 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_group_updated.py
+-rw-rw-rw-   0        0        0      554 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_inline_query.py
+-rw-rw-rw-   0        0        0      552 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_member_joined.py
+-rw-rw-rw-   0        0        0      547 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_member_left.py
+-rw-rw-rw-   0        0        0      519 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_message.py
+-rw-rw-rw-   0        0        0      561 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_unknown_command.py
+-rw-rw-rw-   0        0        0      525 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/decorators/on_user_banned.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.075308 swibots-1.2.9/swibots/bots/filters/
+-rw-rw-rw-   0        0        0       23 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/filters/__init__.py
+-rw-rw-rw-   0        0        0     8057 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/filters/filter.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.120304 swibots-1.2.9/swibots/bots/handlers/
+-rw-rw-rw-   0        0        0     1337 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/__init__.py
+-rw-rw-rw-   0        0        0     1087 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/base_handler.py
+-rw-rw-rw-   0        0        0     1016 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/callback_query_handler.py
+-rw-rw-rw-   0        0        0      704 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/channel_created_handler.py
+-rw-rw-rw-   0        0        0      711 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/channel_deleted_handler.py
+-rw-rw-rw-   0        0        0      758 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/channel_updated_handler.py
+-rw-rw-rw-   0        0        0     1557 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/command_handler.py
+-rw-rw-rw-   0        0        0      709 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/community_updated_handler.py
+-rw-rw-rw-   0        0        0     1365 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/event_handler.py
+-rw-rw-rw-   0        0        0      703 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/group_created_handler.py
+-rw-rw-rw-   0        0        0      800 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/group_deleted_handler.py
+-rw-rw-rw-   0        0        0      800 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/group_updated_handler.py
+-rw-rw-rw-   0        0        0      896 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/inline_query_handler.py
+-rw-rw-rw-   0        0        0      702 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/member_joined_handler.py
+-rw-rw-rw-   0        0        0      697 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/member_left_handler.py
+-rw-rw-rw-   0        0        0      991 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/message_handler.py
+-rw-rw-rw-   0        0        0      914 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/unknown_command_handler.py
+-rw-rw-rw-   0        0        0      693 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/handlers/user_banned_handler.py
+-rw-rw-rw-   0        0        0      298 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/bots/register_command.py
+-rw-rw-rw-   0        0        0     1664 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/config.py
+-rw-rw-rw-   0        0        0     1387 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/error.py
+-rw-rw-rw-   0        0        0      878 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/types.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.125306 swibots-1.2.9/swibots/utils/
+-rw-rw-rw-   0        0        0       78 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/__init__.py
+-rw-rw-rw-   0        0        0     6030 2023-06-26 11:43:01.000000 swibots-1.2.9/swibots/utils/rest_client.py
+-rw-rw-rw-   0        0        0     2558 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/types.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.129311 swibots-1.2.9/swibots/utils/ws/
+-rw-rw-rw-   0        0        0       50 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/ws/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.136316 swibots-1.2.9/swibots/utils/ws/asyncstomp/
+-rw-rw-rw-   0        0        0      154 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/ws/asyncstomp/__init__.py
+-rw-rw-rw-   0        0        0    10071 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/ws/asyncstomp/async_ws_client.py
+-rw-rw-rw-   0        0        0     1010 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/ws/asyncstomp/async_ws_subscription.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:30.143308 swibots-1.2.9/swibots/utils/ws/common/
+-rw-rw-rw-   0        0        0      104 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/ws/common/__init__.py
+-rw-rw-rw-   0        0        0     1716 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/ws/common/ws_frame.py
+-rw-rw-rw-   0        0        0      441 2023-06-26 07:52:28.000000 swibots-1.2.9/swibots/utils/ws/common/ws_message.py
+drwxrwxrwx   0        0        0        0 2023-06-26 12:41:29.738899 swibots-1.2.9/swibots.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-06-26 12:41:29.000000 swibots-1.2.9/swibots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7283 2023-06-26 12:41:29.000000 swibots-1.2.9/swibots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 12:41:29.000000 swibots-1.2.9/swibots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-26 12:41:29.000000 swibots-1.2.9/swibots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-26 12:41:29.000000 swibots-1.2.9/swibots.egg-info/top_level.txt
```

### Comparing `swibots-1.2.8/setup.py` & `swibots-1.2.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from setuptools import setup, find_packages
-
-with open("requirements.txt", encoding="utf-8") as r:
-    requires = [i.strip() for i in r]
-
-try:
-    import pypandoc
-
-    long_description = pypandoc.convert_file("README.md", "rst")
-except (IOError, ImportError):
-    long_description = open("README.md").read()
-
-
-setup(
-    name="swibots",
-    version="1.2.8",
-    packages=find_packages(),
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/switchcollab/Switch-Bots-Python-Library",
-    description="Switch bot api",
-    author="switchadmin",
-    author_email="support@switch.pe",
-    license="LGPLv3",
-    python_requires=">=3.10",
-    install_requires=requires,
-)
+from setuptools import setup, find_packages
+
+with open("requirements.txt", encoding="utf-8") as r:
+    requires = [i.strip() for i in r]
+
+try:
+    import pypandoc
+
+    long_description = pypandoc.convert_file("README.md", "rst")
+except (IOError, ImportError):
+    long_description = open("README.md").read()
+
+
+setup(
+    name="swibots",
+    version="1.2.9",
+    packages=find_packages(),
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/switchcollab/Switch-Bots-Python-Library",
+    description="Switch bot api",
+    author="switchadmin",
+    author_email="support@switch.pe",
+    license="LGPLv3",
+    python_requires=">=3.10",
+    install_requires=requires,
+)
```

### Comparing `swibots-1.2.8/swibots/api/api_client.py` & `swibots-1.2.9/swibots/api/api_client.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-import swibots
-from .auth import AuthClient
-from .chat import ChatClient
-from .community import CommunityClient
-from .bot import BotClient
-from .auth.models import AuthUser
-
-from .auth.methods import AuthMethods
-from .bot.methods import BotMethods
-from .chat.methods import ChatMethods
-from .community.methods import CommunityMethods
-
-
-class ApiClient(
-    AuthMethods,
-    BotMethods,
-    ChatMethods,
-    CommunityMethods,
-):
-    def __init__(self, **kwargs):
-        """Initialize the client"""
-        self._token: str = None
-        self.__dict__.update(kwargs)
-        self._chat_client: ChatClient = None
-        self._auth_client: AuthClient = None
-        self._community_client: CommunityClient = None
-        self._bot_client: BotClient = None
-        self._user: AuthUser = None
-        self.initialize()
-
-    def initialize(self):
-        """Initialize the client"""
-        self.chat_service.initialize()
-        self.auth_service.initialize()
-        self.community_service.initialize()
-
-    @property
-    def user(self) -> AuthUser:
-        return self._user
-
-    @user.setter
-    def user(self, value: AuthUser):
-        self._user = value
-
-    @property
-    def token(self) -> str:
-        """Get the token"""
-        return self._token
-
-    @token.setter
-    def token(self, value: str):
-        """Set the token"""
-        self._token = value
-
-    @property
-    def chat_service(self) -> ChatClient:
-        """Get the chat client"""
-        if self._chat_client is None:
-            self._chat_client = ChatClient(self)
-        return self._chat_client
-
-    @property
-    def auth_service(self) -> AuthClient:
-        """Get the auth client"""
-        if self._auth_client is None:
-            self._auth_client = AuthClient(self)
-        return self._auth_client
-
-    @property
-    def community_service(self) -> CommunityClient:
-        """Get the community client"""
-        if self._community_client is None:
-            self._community_client = CommunityClient(self)
-        return self._community_client
-
-    @property
-    def bots_service(self) -> BotClient:
-        """Get the bot client"""
-        if self._bot_client is None:
-            self._bot_client = BotClient(self)
-        return self._bot_client
+import swibots
+from .auth import AuthClient
+from .chat import ChatClient
+from .community import CommunityClient
+from .bot import BotClient
+from .auth.models import AuthUser
+
+from .auth.methods import AuthMethods
+from .bot.methods import BotMethods
+from .chat.methods import ChatMethods
+from .community.methods import CommunityMethods
+
+
+class ApiClient(
+    AuthMethods,
+    BotMethods,
+    ChatMethods,
+    CommunityMethods,
+):
+    def __init__(self, **kwargs):
+        """Initialize the client"""
+        self._token: str = None
+        self.__dict__.update(kwargs)
+        self._chat_client: ChatClient = None
+        self._auth_client: AuthClient = None
+        self._community_client: CommunityClient = None
+        self._bot_client: BotClient = None
+        self._user: AuthUser = None
+        self.initialize()
+
+    def initialize(self):
+        """Initialize the client"""
+        self.chat_service.initialize()
+        self.auth_service.initialize()
+        self.community_service.initialize()
+
+    @property
+    def user(self) -> AuthUser:
+        return self._user
+
+    @user.setter
+    def user(self, value: AuthUser):
+        self._user = value
+
+    @property
+    def token(self) -> str:
+        """Get the token"""
+        return self._token
+
+    @token.setter
+    def token(self, value: str):
+        """Set the token"""
+        self._token = value
+
+    @property
+    def chat_service(self) -> ChatClient:
+        """Get the chat client"""
+        if self._chat_client is None:
+            self._chat_client = ChatClient(self)
+        return self._chat_client
+
+    @property
+    def auth_service(self) -> AuthClient:
+        """Get the auth client"""
+        if self._auth_client is None:
+            self._auth_client = AuthClient(self)
+        return self._auth_client
+
+    @property
+    def community_service(self) -> CommunityClient:
+        """Get the community client"""
+        if self._community_client is None:
+            self._community_client = CommunityClient(self)
+        return self._community_client
+
+    @property
+    def bots_service(self) -> BotClient:
+        """Get the bot client"""
+        if self._bot_client is None:
+            self._bot_client = BotClient(self)
+        return self._bot_client
```

### Comparing `swibots-1.2.8/swibots/api/auth/auth_client.py` & `swibots-1.2.9/swibots/api/auth/auth_client.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from swibots.api.auth.controllers import UserController
-from swibots.base import SwitchRestClient
-from swibots.config import get_config
-import swibots
-
-
-class AuthClient(SwitchRestClient):
-    """Auth client
-
-    This client is used to communicate with the auth service.
-
-    Controllers:
-        - :attr:`users`: :obj:`~switch.api.auth.controllers.UserController` : The users controller
-    """
-
-    def __init__(self, app: "swibots.App", base_url: str = None):
-        """Initialize the auth client"""
-        base_url = base_url or get_config()["AUTH_SERVICE"]["BASE_URL"]
-        super().__init__(app, base_url)
-        self._users = None
-        self._authorization = None
-
-    @property
-    def users(self) -> UserController:
-        """Get the users controller
-
-        Returns:
-            :obj:`~switch.api.auth.controllers.UserController`: The users controller
-        """
-        if self._users is None:
-            self._users = UserController(self)
-        return self._users
-
-    def prepare_request_headers(self, headers: dict) -> dict:
-        headers = super().prepare_request_headers(headers)
-        if self.token is not None:
-            headers["authtoken"] = f"{self.token}"
-        return headers
+from swibots.api.auth.controllers import UserController
+from swibots.base import SwitchRestClient
+from swibots.config import get_config
+import swibots
+
+
+class AuthClient(SwitchRestClient):
+    """Auth client
+
+    This client is used to communicate with the auth service.
+
+    Controllers:
+        - :attr:`users`: :obj:`~switch.api.auth.controllers.UserController` : The users controller
+    """
+
+    def __init__(self, app: "swibots.App", base_url: str = None):
+        """Initialize the auth client"""
+        base_url = base_url or get_config()["AUTH_SERVICE"]["BASE_URL"]
+        super().__init__(app, base_url)
+        self._users = None
+        self._authorization = None
+
+    @property
+    def users(self) -> UserController:
+        """Get the users controller
+
+        Returns:
+            :obj:`~switch.api.auth.controllers.UserController`: The users controller
+        """
+        if self._users is None:
+            self._users = UserController(self)
+        return self._users
+
+    def prepare_request_headers(self, headers: dict) -> dict:
+        headers = super().prepare_request_headers(headers)
+        if self.token is not None:
+            headers["authtoken"] = f"{self.token}"
+        return headers
```

### Comparing `swibots-1.2.8/swibots/api/auth/controllers/user_controller.py` & `swibots-1.2.9/swibots/api/auth/controllers/user_controller.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import logging
-import swibots
-from typing import TYPE_CHECKING, Type, TypeVar
-from ..models import AuthUser
-
-if TYPE_CHECKING:
-    from swibots.api.auth import AuthClient
-
-log = logging.getLogger(__name__)
-
-BASE_PATH = "/user"
-T = TypeVar("T", bound="AuthUser")
-
-
-class UserController:
-    """User controller
-
-    This controller is used to communicate with the user endpoints.
-
-    """
-
-    def __init__(self, client: "AuthClient"):
-        self.client = client
-
-    async def me(self, user_type: Type[T] = AuthUser) -> T:
-        """Get the current user
-
-        Parameters:
-            user_type (``Type[T]``, *optional*): The user type to return. Defaults to :obj:`~switch.api.auth.models.AuthUser`.
-
-        Returns:
-            ``T``: The current user
-
-        """
-        response = await self.client.get(f"{BASE_PATH}")
-        return self.client.build_object(user_type, response.data)
-    
-    async def login(self, username: str, password: str, user_type: Type[T] = AuthUser) -> T:
-        """Login with username and password
-
-        Parameters:
-            username (``str``): The username
-            password (``str``): The password
-            user_type (``Type[T]``, *optional*): The user type to return. Defaults to :obj:`~switch.api.auth.models.AuthUser`.
-
-        Returns:
-            ``T``: The user
-
-        """
-        response = await self.client.post(f"{BASE_PATH}/login", json={"username": username, "password": password})
-        return self.client.build_object(user_type, response.data)
+import logging
+import swibots
+from typing import TYPE_CHECKING, Type, TypeVar
+from ..models import AuthUser
+
+if TYPE_CHECKING:
+    from swibots.api.auth import AuthClient
+
+log = logging.getLogger(__name__)
+
+BASE_PATH = "/user"
+T = TypeVar("T", bound="AuthUser")
+
+
+class UserController:
+    """User controller
+
+    This controller is used to communicate with the user endpoints.
+
+    """
+
+    def __init__(self, client: "AuthClient"):
+        self.client = client
+
+    async def me(self, user_type: Type[T] = AuthUser) -> T:
+        """Get the current user
+
+        Parameters:
+            user_type (``Type[T]``, *optional*): The user type to return. Defaults to :obj:`~switch.api.auth.models.AuthUser`.
+
+        Returns:
+            ``T``: The current user
+
+        """
+        response = await self.client.get(f"{BASE_PATH}")
+        return self.client.build_object(user_type, response.data)
+    
+    async def login(self, username: str, password: str, user_type: Type[T] = AuthUser) -> T:
+        """Login with username and password
+
+        Parameters:
+            username (``str``): The username
+            password (``str``): The password
+            user_type (``Type[T]``, *optional*): The user type to return. Defaults to :obj:`~switch.api.auth.models.AuthUser`.
+
+        Returns:
+            ``T``: The user
+
+        """
+        response = await self.client.post(f"{BASE_PATH}/login", json={"username": username, "password": password})
+        return self.client.build_object(user_type, response.data)
```

### Comparing `swibots-1.2.8/swibots/api/auth/methods/login.py` & `swibots-1.2.9/swibots/api/auth/methods/login.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.auth.models import AuthUser
-
-T = TypeVar("T", bound="swibots.AuthUser")
-
-
-class Login:
-    async def login(self: "swibots.ApiClient", username: str, password: str, user_type: Type[T] = AuthUser) -> T:
-        """Login with username and password
-
-        Parameters:
-            username (``str``): The username   
-            password (``str``): The password
-            user_type (``Type[T]``, *optional*): The user type to return. Defaults to :obj:`~switch.api.auth.models.AuthUser`.
-
-        Returns:
-            ``T``: The user
-
-        This functions does the same as :meth:`~switch.api.auth.controllers.UserController.login`.
-        
-        
-        """
-        return await self.auth_service.users.login(username=username, password=password, user_type=user_type)
+from typing import Type, TypeVar
+import swibots
+from swibots.api.auth.models import AuthUser
+
+T = TypeVar("T", bound="swibots.AuthUser")
+
+
+class Login:
+    async def login(self: "swibots.ApiClient", username: str, password: str, user_type: Type[T] = AuthUser) -> T:
+        """Login with username and password
+
+        Parameters:
+            username (``str``): The username   
+            password (``str``): The password
+            user_type (``Type[T]``, *optional*): The user type to return. Defaults to :obj:`~switch.api.auth.models.AuthUser`.
+
+        Returns:
+            ``T``: The user
+
+        This functions does the same as :meth:`~switch.api.auth.controllers.UserController.login`.
+        
+        
+        """
+        return await self.auth_service.users.login(username=username, password=password, user_type=user_type)
```

### Comparing `swibots-1.2.8/swibots/api/auth/models/auth_user.py` & `swibots-1.2.9/swibots/api/auth/models/auth_user.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,123 @@
-from typing import Optional
-from swibots.base.switch_object import SwitchObject
-from swibots.utils.types import JSONDict
-
-
-class AuthUser(SwitchObject):
-    def __init__(
-        self,
-        id: Optional[int] = None,
-        user_name: Optional[str] = None,
-        name: Optional[str] = None,
-        creator_name: Optional[str] = None,
-        verify_email: Optional[bool] = None,
-        privacy: Optional[str] = None,
-        is_bot: Optional[bool] = None,
-        bot_privacy: Optional[str] = None,
-        profile_colour: Optional[str] = None,
-        otp: Optional[str] = None,
-        otp_expiry: Optional[str] = None,
-        bio: Optional[str] = None,
-        imageurl: Optional[str] = None,
-        private_imageurl: Optional[str] = None,
-        gender: Optional[str] = None,
-        date_of_birth: Optional[str] = None,
-        media1: Optional[str] = None,
-        media2: Optional[str] = None,
-        media3: Optional[str] = None,
-        media4: Optional[str] = None,
-        media5: Optional[str] = None,
-        more_about_this: Optional[str] = None,
-        active: Optional[bool] = None,
-        parent_id: Optional[int] = None,
-        created_at: Optional[str] = None,
-        updated_at: Optional[str] = None,
-    ):
-        self.id = id
-        self.user_name = user_name
-        self.name = name
-        self.creator_name = creator_name
-        self.verify_email = verify_email
-        self.privacy = privacy
-        self.is_bot = is_bot
-        self.bot_privacy = bot_privacy
-        self.profile_colour = profile_colour
-        self.otp = otp
-        self.otp_expiry = otp_expiry
-        self.bio = bio
-        self.imageurl = imageurl
-        self.private_imageurl = private_imageurl
-        self.gender = gender
-        self.date_of_birth = date_of_birth
-        self.media1 = media1
-        self.media2 = media2
-        self.media3 = media3
-        self.media4 = media4
-        self.media5 = media5
-        self.more_about_this = more_about_this
-        self.active = active
-        self.parent_id = parent_id
-        self.created_at = created_at
-        self.updated_at = updated_at
-
-    def from_json(self, data: Optional[JSONDict]) -> "AuthUser":
-        super().from_json(data)
-        if data is not None:
-            self.id = data.get("id")
-            self.user_name = data.get("user_name")
-            self.name = data.get("name")
-            self.creator_name = data.get("creator_name")
-            self.verify_email = data.get("verifyEmail")
-            self.privacy = data.get("privacy")
-            self.is_bot = data.get("is_bot")
-            self.bot_privacy = data.get("bot_privacy")
-            self.profile_colour = data.get("profile_colour")
-            self.otp = data.get("otp")
-            self.otp_expiry = data.get("otp_expiry")
-            self.bio = data.get("bio")
-            self.imageurl = data.get("imageurl")
-            self.private_imageurl = data.get("private_imageurl")
-            self.gender = data.get("gender")
-            self.date_of_birth = data.get("date_of_birth")
-            self.media1 = data.get("media1")
-            self.media2 = data.get("media2")
-            self.media3 = data.get("media3")
-            self.media4 = data.get("media4")
-            self.media5 = data.get("media5")
-            self.more_about_this = data.get("more_about_this")
-            self.active = data.get("active")
-            self.parent_id = data.get("parent_id")
-            self.created_at = data.get("createdAt")
-            self.updated_at = data.get("updatedAt")
-
-        return self
-
-    def to_json(self) -> JSONDict:
-        return {
-            "id": self.id,
-            "user_name": self.user_name,
-            "name": self.name,
-            "creator_name": self.creator_name,
-            "verifyEmail": self.verify_email,
-            "privacy": self.privacy,
-            "is_bot": self.is_bot,
-            "bot_privacy": self.bot_privacy,
-            "profile_colour": self.profile_colour,
-            "otp": self.otp,
-            "otp_expiry": self.otp_expiry,
-            "bio": self.bio,
-            "imageurl": self.imageurl,
-            "private_imageurl": self.private_imageurl,
-            "gender": self.gender,
-            "date_of_birth": self.date_of_birth,
-            "media1": self.media1,
-            "media2": self.media2,
-            "media3": self.media3,
-            "media4": self.media4,
-            "media5": self.media5,
-            "more_about_this": self.more_about_this,
-            "active": self.active,
-            "parent_id": self.parent_id,
-            "createdAt": self.created_at,
-            "updatedAt": self.updated_at,
-        }
+from typing import Optional
+from swibots.base.switch_object import SwitchObject
+from swibots.utils.types import JSONDict
+
+
+class AuthUser(SwitchObject):
+    def __init__(
+        self,
+        id: Optional[int] = None,
+        user_name: Optional[str] = None,
+        name: Optional[str] = None,
+        creator_name: Optional[str] = None,
+        verify_email: Optional[bool] = None,
+        privacy: Optional[str] = None,
+        is_bot: Optional[bool] = None,
+        bot_privacy: Optional[str] = None,
+        profile_colour: Optional[str] = None,
+        otp: Optional[str] = None,
+        otp_expiry: Optional[str] = None,
+        bio: Optional[str] = None,
+        imageurl: Optional[str] = None,
+        private_imageurl: Optional[str] = None,
+        gender: Optional[str] = None,
+        date_of_birth: Optional[str] = None,
+        media1: Optional[str] = None,
+        media2: Optional[str] = None,
+        media3: Optional[str] = None,
+        media4: Optional[str] = None,
+        media5: Optional[str] = None,
+        more_about_this: Optional[str] = None,
+        active: Optional[bool] = None,
+        parent_id: Optional[int] = None,
+        created_at: Optional[str] = None,
+        updated_at: Optional[str] = None,
+    ):
+        self.id = id
+        self.user_name = user_name
+        self.name = name
+        self.creator_name = creator_name
+        self.verify_email = verify_email
+        self.privacy = privacy
+        self.is_bot = is_bot
+        self.bot_privacy = bot_privacy
+        self.profile_colour = profile_colour
+        self.otp = otp
+        self.otp_expiry = otp_expiry
+        self.bio = bio
+        self.imageurl = imageurl
+        self.private_imageurl = private_imageurl
+        self.gender = gender
+        self.date_of_birth = date_of_birth
+        self.media1 = media1
+        self.media2 = media2
+        self.media3 = media3
+        self.media4 = media4
+        self.media5 = media5
+        self.more_about_this = more_about_this
+        self.active = active
+        self.parent_id = parent_id
+        self.created_at = created_at
+        self.updated_at = updated_at
+
+    def from_json(self, data: Optional[JSONDict]) -> "AuthUser":
+        super().from_json(data)
+        if data is not None:
+            self.id = data.get("id")
+            self.user_name = data.get("user_name")
+            self.name = data.get("name")
+            self.creator_name = data.get("creator_name")
+            self.verify_email = data.get("verifyEmail")
+            self.privacy = data.get("privacy")
+            self.is_bot = data.get("is_bot")
+            self.bot_privacy = data.get("bot_privacy")
+            self.profile_colour = data.get("profile_colour")
+            self.otp = data.get("otp")
+            self.otp_expiry = data.get("otp_expiry")
+            self.bio = data.get("bio")
+            self.imageurl = data.get("imageurl")
+            self.private_imageurl = data.get("private_imageurl")
+            self.gender = data.get("gender")
+            self.date_of_birth = data.get("date_of_birth")
+            self.media1 = data.get("media1")
+            self.media2 = data.get("media2")
+            self.media3 = data.get("media3")
+            self.media4 = data.get("media4")
+            self.media5 = data.get("media5")
+            self.more_about_this = data.get("more_about_this")
+            self.active = data.get("active")
+            self.parent_id = data.get("parent_id")
+            self.created_at = data.get("createdAt")
+            self.updated_at = data.get("updatedAt")
+
+        return self
+
+    def to_json(self) -> JSONDict:
+        return {
+            "id": self.id,
+            "user_name": self.user_name,
+            "name": self.name,
+            "creator_name": self.creator_name,
+            "verifyEmail": self.verify_email,
+            "privacy": self.privacy,
+            "is_bot": self.is_bot,
+            "bot_privacy": self.bot_privacy,
+            "profile_colour": self.profile_colour,
+            "otp": self.otp,
+            "otp_expiry": self.otp_expiry,
+            "bio": self.bio,
+            "imageurl": self.imageurl,
+            "private_imageurl": self.private_imageurl,
+            "gender": self.gender,
+            "date_of_birth": self.date_of_birth,
+            "media1": self.media1,
+            "media2": self.media2,
+            "media3": self.media3,
+            "media4": self.media4,
+            "media5": self.media5,
+            "more_about_this": self.more_about_this,
+            "active": self.active,
+            "parent_id": self.parent_id,
+            "createdAt": self.created_at,
+            "updatedAt": self.updated_at,
+        }
```

### Comparing `swibots-1.2.8/swibots/api/bot/bot_client.py` & `swibots-1.2.9/swibots/api/bot/bot_client.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from swibots.api.auth.models.auth_user import AuthUser
-from swibots.api.bot.controllers import BotController
-from swibots.base import SwitchRestClient
-from swibots.config import get_config
-import swibots
-
-
-class BotClient(SwitchRestClient):
-    """Bot client
-
-    This client is used to communicate with the bot service.
-
-    Controllers:
-        - :attr:`bots`: :obj:`~switch.api.bot.controllers.BotController` : The bot controller
-
-    Properties:
-        - :attr:`user`: :obj:`~switch.api.auth.models.auth_user.AuthUser` : The current user
-
-    """
-
-    def __init__(self, app: "swibots.App" = None, base_url: str = None):
-        """Initialize the bot client
-
-        Parameters:
-            base_url (``str``): The base url of the bot service. Defaults to the value in the config.
-        """
-        base_url = base_url or get_config()["BOT_SERVICE"]["BASE_URL"]
-        super().__init__(app, base_url)
-        self._bots: BotController = None
-
-    @property
-    def bots(self) -> BotController:
-        """Get the bot controller"""
-        if self._bots is None:
-            self._bots = BotController(self)
-        return self._bots
+from swibots.api.auth.models.auth_user import AuthUser
+from swibots.api.bot.controllers import BotController
+from swibots.base import SwitchRestClient
+from swibots.config import get_config
+import swibots
+
+
+class BotClient(SwitchRestClient):
+    """Bot client
+
+    This client is used to communicate with the bot service.
+
+    Controllers:
+        - :attr:`bots`: :obj:`~switch.api.bot.controllers.BotController` : The bot controller
+
+    Properties:
+        - :attr:`user`: :obj:`~switch.api.auth.models.auth_user.AuthUser` : The current user
+
+    """
+
+    def __init__(self, app: "swibots.App" = None, base_url: str = None):
+        """Initialize the bot client
+
+        Parameters:
+            base_url (``str``): The base url of the bot service. Defaults to the value in the config.
+        """
+        base_url = base_url or get_config()["BOT_SERVICE"]["BASE_URL"]
+        super().__init__(app, base_url)
+        self._bots: BotController = None
+
+    @property
+    def bots(self) -> BotController:
+        """Get the bot controller"""
+        if self._bots is None:
+            self._bots = BotController(self)
+        return self._bots
```

### Comparing `swibots-1.2.8/swibots/api/bot/controllers/bot_controller.py` & `swibots-1.2.9/swibots/api/bot/controllers/bot_controller.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import json
-import logging
-from typing import TYPE_CHECKING, List
-from swibots.api.bot.models import BotInfo, BotCommandInfo
-from swibots.error import SwitchError
-from swibots.utils.types import JSONDict
-
-if TYPE_CHECKING:
-    from swibots.api.bot import BotClient
-
-log = logging.getLogger(__name__)
-
-BASE_PATH = "/v1/bots"
-
-
-class BotController:
-    """Bot controller
-
-    This controller is used to communicate with the bot endpoints.
-    """
-
-    def __init__(self, client: "BotClient"):
-        self.client = client
-
-    async def get_bot_info(self, bot_id: str) -> BotInfo:
-        """Get bot info
-
-        Parameters:
-            bot_id (``str``): The bot id. Defaults to the current bot id.
-
-        Returns:
-            :obj:``~switch.api.bot.models.BotInfo``: The bot info
-        """
-        if bot_id is None:
-            bot_id = self.client.user.id
-        response = await self.client.get(f"{BASE_PATH}/{bot_id}")
-        return BotInfo.build_from_json(response.data)
-
-    async def update_bot_info(self, bot_info: BotInfo) -> BotInfo:
-        """Update bot info
-
-        Parameters:
-            bot_info (``~switch.api.bot.models.BotInfo``): The bot info to update
-
-        Returns:
-            :obj:``~switch.api.bot.models.BotInfo``: The bot info
-        """
-        data = bot_info.to_json_request()
-        response = await self.client.put(f"{BASE_PATH}", data=data)
-        return BotInfo.build_from_json(response.data)
-
-    async def delete_bot_info(self, bot_id: str) -> bool:
-        """Delete bot info
-
-        Parameters:
-            bot_id (``str``): The bot id. Defaults to the current bot id.
-
-        Returns:
-            ``bool``: True if the bot was deleted
-        """
-        response = await self.client.delete(f"{BASE_PATH}/{bot_id}")
-        return True
+import json
+import logging
+from typing import TYPE_CHECKING, List
+from swibots.api.bot.models import BotInfo, BotCommandInfo
+from swibots.error import SwitchError
+from swibots.utils.types import JSONDict
+
+if TYPE_CHECKING:
+    from swibots.api.bot import BotClient
+
+log = logging.getLogger(__name__)
+
+BASE_PATH = "/v1/bots"
+
+
+class BotController:
+    """Bot controller
+
+    This controller is used to communicate with the bot endpoints.
+    """
+
+    def __init__(self, client: "BotClient"):
+        self.client = client
+
+    async def get_bot_info(self, bot_id: str) -> BotInfo:
+        """Get bot info
+
+        Parameters:
+            bot_id (``str``): The bot id. Defaults to the current bot id.
+
+        Returns:
+            :obj:``~switch.api.bot.models.BotInfo``: The bot info
+        """
+        if bot_id is None:
+            bot_id = self.client.user.id
+        response = await self.client.get(f"{BASE_PATH}/{bot_id}")
+        return BotInfo.build_from_json(response.data)
+
+    async def update_bot_info(self, bot_info: BotInfo) -> BotInfo:
+        """Update bot info
+
+        Parameters:
+            bot_info (``~switch.api.bot.models.BotInfo``): The bot info to update
+
+        Returns:
+            :obj:``~switch.api.bot.models.BotInfo``: The bot info
+        """
+        data = bot_info.to_json_request()
+        response = await self.client.put(f"{BASE_PATH}", data=data)
+        return BotInfo.build_from_json(response.data)
+
+    async def delete_bot_info(self, bot_id: str) -> bool:
+        """Delete bot info
+
+        Parameters:
+            bot_id (``str``): The bot id. Defaults to the current bot id.
+
+        Returns:
+            ``bool``: True if the bot was deleted
+        """
+        response = await self.client.delete(f"{BASE_PATH}/{bot_id}")
+        return True
```

### Comparing `swibots-1.2.8/swibots/api/bot/methods/get_bot_info.py` & `swibots-1.2.9/swibots/api/bot/methods/get_bot_info.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.bot.models import BotInfo
-
-
-class GetBotInfo:
-    async def get_bot_info(self: "swibots.ApiClient", bot_id: str) -> BotInfo:
-        """Get bot info
-
-        Parameters:
-            bot_id (``str``): The bot id. Defaults to the current bot id.
-
-        Returns:
-            :obj:``~switch.api.bot.models.BotInfo``: The bot info
-
-        This functions does the same as :meth:`~switch.api.bot.controllers.BotController.get_bot_info`.
-        """
-        return await self.bots_service.bots.get_bot_info(bot_id=bot_id)
+from typing import Type, TypeVar
+import swibots
+from swibots.api.bot.models import BotInfo
+
+
+class GetBotInfo:
+    async def get_bot_info(self: "swibots.ApiClient", bot_id: str) -> BotInfo:
+        """Get bot info
+
+        Parameters:
+            bot_id (``str``): The bot id. Defaults to the current bot id.
+
+        Returns:
+            :obj:``~switch.api.bot.models.BotInfo``: The bot info
+
+        This functions does the same as :meth:`~switch.api.bot.controllers.BotController.get_bot_info`.
+        """
+        return await self.bots_service.bots.get_bot_info(bot_id=bot_id)
```

### Comparing `swibots-1.2.8/swibots/api/bot/methods/update_bot_info.py` & `swibots-1.2.9/swibots/api/bot/methods/update_bot_info.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.bot.models import BotInfo
-
-
-class UpdateBotInfo:
-    async def update_bot_info(self: "swibots.ApiClient", bot_info: BotInfo) -> BotInfo:
-        """Update bot info
-
-        Parameters:
-            bot_info (``~switch.api.bot.models.BotInfo``): The bot info to update
-
-        Returns:
-            :obj:``~switch.api.bot.models.BotInfo``: The bot info
-
-        This functions does the same as :meth:`~switch.api.bot.controllers.BotController.update_bot_info`.
-        """
-        return await self.bots_service.bots.update_bot_info(bot_info=bot_info)
+from typing import Type, TypeVar
+import swibots
+from swibots.api.bot.models import BotInfo
+
+
+class UpdateBotInfo:
+    async def update_bot_info(self: "swibots.ApiClient", bot_info: BotInfo) -> BotInfo:
+        """Update bot info
+
+        Parameters:
+            bot_info (``~switch.api.bot.models.BotInfo``): The bot info to update
+
+        Returns:
+            :obj:``~switch.api.bot.models.BotInfo``: The bot info
+
+        This functions does the same as :meth:`~switch.api.bot.controllers.BotController.update_bot_info`.
+        """
+        return await self.bots_service.bots.update_bot_info(bot_info=bot_info)
```

### Comparing `swibots-1.2.8/swibots/api/bot/models/bot_command_info.py` & `swibots-1.2.9/swibots/api/bot/models/bot_command_info.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import Optional
-from swibots.base import SwitchObject
-from swibots.utils.types import JSONDict
-
-
-class BotCommandInfo(SwitchObject):
-    def __init__(
-        self,
-        command: Optional[str] = None,
-        description: Optional[str] = None,
-        channel: Optional[bool] = False,
-    ):
-        self.bot_id = None
-        self.command = command
-        self.description = description
-        self.channel = channel
-
-    def from_json(self, data: JSONDict) -> "BotCommandInfo":
-        if data is not None:
-            self.bot_id = data.get("botId")
-            self.command = data.get("command")
-            self.description = data.get("description")
-            self.channel = data.get("channel")
-        return self
-
-    def to_json(self) -> JSONDict:
-        return {
-            "botId": self.bot_id,
-            "command": self.command,
-            "description": self.description,
-            "channel": self.channel,
-        }
+from typing import Optional
+from swibots.base import SwitchObject
+from swibots.utils.types import JSONDict
+
+
+class BotCommandInfo(SwitchObject):
+    def __init__(
+        self,
+        command: Optional[str] = None,
+        description: Optional[str] = None,
+        channel: Optional[bool] = False,
+    ):
+        self.bot_id = None
+        self.command = command
+        self.description = description
+        self.channel = channel
+
+    def from_json(self, data: JSONDict) -> "BotCommandInfo":
+        if data is not None:
+            self.bot_id = data.get("botId")
+            self.command = data.get("command")
+            self.description = data.get("description")
+            self.channel = data.get("channel")
+        return self
+
+    def to_json(self) -> JSONDict:
+        return {
+            "botId": self.bot_id,
+            "command": self.command,
+            "description": self.description,
+            "channel": self.channel,
+        }
```

### Comparing `swibots-1.2.8/swibots/api/chat/chat_client.py` & `swibots-1.2.9/swibots/api/chat/chat_client.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-import json
-import logging
-from typing import Tuple
-from swibots.api.auth.models.auth_user import AuthUser
-from swibots.api.chat.controllers import MessageController
-from swibots.api.chat.events import ChatEvent, CallbackQueryEvent, MessageEvent, CommandEvent, InlineQueryEvent
-from swibots.base import SwitchRestClient, SwitchWSAsyncClient
-from swibots.config import get_config
-from swibots.error import SwitchError
-from swibots.types import EventType
-from swibots.utils.ws.asyncstomp.async_ws_subscription import AsyncWsSubscription
-from swibots.utils.ws.common.ws_message import WsMessage
-import swibots
-
-logger = logging.getLogger(__name__)
-
-
-class ChatClient(SwitchRestClient):
-    """Chat client
-
-    This client is used to communicate with the chat service.
-
-    Controllers:
-        - :attr:`messages`: :obj:`~switch.api.chat.controllers.MessageController` : The message controller
-
-    Properties:
-        - :attr:`user`: :obj:`~switch.api.auth.models.auth_user.AuthUser` : The current user
-        - :attr:`ws`: :obj:`~switch.base.SwitchWSAsyncClient` : The websocket client
-
-    """
-
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        base_url: str = None,
-        ws_url: str = None,
-    ):
-        """Initialize the chat client
-
-        Parameters:
-            base_url (``str``): The base url of the chat service. Defaults to the value in the config.
-            ws_url (``str``): The websocket url of the chat service. Defaults to the value in the config.
-        """
-        base_url = base_url or get_config()["CHAT_SERVICE"]["BASE_URL"]
-        self._ws_url = ws_url or get_config()["CHAT_SERVICE"]["WS_URL"]
-        super().__init__(app, base_url)
-        self._messages: MessageController = None
-        self._ws: SwitchWSAsyncClient = None
-        self._started = False
-
-    @property
-    def ws(self) -> SwitchWSAsyncClient:
-        if self._ws is None:
-            self._ws = SwitchWSAsyncClient(self._ws_url, self.token)
-        return self._ws
-
-    @property
-    def messages(self) -> MessageController:
-        """Get the message controller"""
-        if self._messages is None:
-            self._messages = MessageController(self)
-        return self._messages
-
-    async def subscribe(self, endpoint: str, callback=None) -> AsyncWsSubscription:
-        """Subscribe to a websocket endpoint
-
-        Parameters:
-            endpoint (``str``): The endpoint to subscribe to
-            callback (``callable``): The callback to call when a message is received
-
-        Returns:
-            :obj:`~switch.utils.ws.asyncstomp.async_ws_subscription.AsyncWsSubscription`: The subscription
-
-        Raises:
-            :obj:`~switch.error.SwitchError`: If the user is not set or the callback is not set
-        """
-        if self.user is None:
-            raise SwitchError("User is not set")
-        if callback is None:
-            raise SwitchError("Callback is not set")
-        return await self.ws.subscribe(endpoint, callback=callback)
-
-    async def subscribe_to_notifications(self, callback=None) -> AsyncWsSubscription:
-        """Subscribe to the notification endpoint
-
-        Parameters:
-            callback (``callable``): The callback to call when a message is received
-
-        Returns:
-            :obj:`~switch.utils.ws.asyncstomp.async_ws_subscription.AsyncWsSubscription`: The subscription
-
-        Raises:
-            :obj:`~switch.error.SwitchError`: If the user is not set or the callback is not set
-
-        This is a shortcut for :meth:`subscribe` with the endpoint set to ``/chat/queue/events``
-        """
-        subscription = await self.ws.subscribe(
-            "/chat/queue/events",
-            callback=lambda event: callback(self._parse_event(event)),
-        )
-        return subscription
-
-    def _parse_event(self, raw_message: WsMessage) -> ChatEvent:
-        try:
-            json_data = json.loads(raw_message.body)
-            type = json_data.get("type", "MESSAGE")
-            evt: ChatEvent = None
-            if type == EventType.MESSAGE.value:
-                evt = self.build_object(MessageEvent, json_data)
-                # evt = MessageEvent.build_from_json(json_data)
-            elif type == EventType.COMMAND.value:
-                evt = self.build_object(CommandEvent, json_data)
-                # evt = CommandEvent.build_from_json(json_data)
-            elif type == EventType.CALLBACK_QUERY.value:
-                evt = self.build_object(CallbackQueryEvent, json_data)
-                # evt = CallbackQueryEvent.build_from_json(json_data)
-            elif type == EventType.INLINE_QUERY.value:
-                evt = self.build_object(InlineQueryEvent, json_data)
-            else:
-                evt = self.build_object(ChatEvent, json_data)
-                # evt = ChatEvent.build_from_json(json_data)
-            return evt
-        except Exception as e:
-            logger.exception(e)
-
-    async def start(self):
-        """Start the chat websocket client
-        Raises:
-            :obj:`~switch.error.SwitchError`: If the user is not set
-        """
-        if self.user is None:
-            raise SwitchError("User is not set")
-        await self.ws.connect()
-        self._started = True
-
-    async def stop(self):
-        """Stop the chat websocket client"""
-        if self._started:
-            await self.ws.disconnect()
-            self._started = False
+import json
+import logging
+from typing import Tuple
+from swibots.api.auth.models.auth_user import AuthUser
+from swibots.api.chat.controllers import MessageController
+from swibots.api.chat.events import ChatEvent, CallbackQueryEvent, MessageEvent, CommandEvent, InlineQueryEvent
+from swibots.base import SwitchRestClient, SwitchWSAsyncClient
+from swibots.config import get_config
+from swibots.error import SwitchError
+from swibots.types import EventType
+from swibots.utils.ws.asyncstomp.async_ws_subscription import AsyncWsSubscription
+from swibots.utils.ws.common.ws_message import WsMessage
+import swibots
+
+logger = logging.getLogger(__name__)
+
+
+class ChatClient(SwitchRestClient):
+    """Chat client
+
+    This client is used to communicate with the chat service.
+
+    Controllers:
+        - :attr:`messages`: :obj:`~switch.api.chat.controllers.MessageController` : The message controller
+
+    Properties:
+        - :attr:`user`: :obj:`~switch.api.auth.models.auth_user.AuthUser` : The current user
+        - :attr:`ws`: :obj:`~switch.base.SwitchWSAsyncClient` : The websocket client
+
+    """
+
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        base_url: str = None,
+        ws_url: str = None,
+    ):
+        """Initialize the chat client
+
+        Parameters:
+            base_url (``str``): The base url of the chat service. Defaults to the value in the config.
+            ws_url (``str``): The websocket url of the chat service. Defaults to the value in the config.
+        """
+        base_url = base_url or get_config()["CHAT_SERVICE"]["BASE_URL"]
+        self._ws_url = ws_url or get_config()["CHAT_SERVICE"]["WS_URL"]
+        super().__init__(app, base_url)
+        self._messages: MessageController = None
+        self._ws: SwitchWSAsyncClient = None
+        self._started = False
+
+    @property
+    def ws(self) -> SwitchWSAsyncClient:
+        if self._ws is None:
+            self._ws = SwitchWSAsyncClient(self._ws_url, self.token)
+        return self._ws
+
+    @property
+    def messages(self) -> MessageController:
+        """Get the message controller"""
+        if self._messages is None:
+            self._messages = MessageController(self)
+        return self._messages
+
+    async def subscribe(self, endpoint: str, callback=None) -> AsyncWsSubscription:
+        """Subscribe to a websocket endpoint
+
+        Parameters:
+            endpoint (``str``): The endpoint to subscribe to
+            callback (``callable``): The callback to call when a message is received
+
+        Returns:
+            :obj:`~switch.utils.ws.asyncstomp.async_ws_subscription.AsyncWsSubscription`: The subscription
+
+        Raises:
+            :obj:`~switch.error.SwitchError`: If the user is not set or the callback is not set
+        """
+        if self.user is None:
+            raise SwitchError("User is not set")
+        if callback is None:
+            raise SwitchError("Callback is not set")
+        return await self.ws.subscribe(endpoint, callback=callback)
+
+    async def subscribe_to_notifications(self, callback=None) -> AsyncWsSubscription:
+        """Subscribe to the notification endpoint
+
+        Parameters:
+            callback (``callable``): The callback to call when a message is received
+
+        Returns:
+            :obj:`~switch.utils.ws.asyncstomp.async_ws_subscription.AsyncWsSubscription`: The subscription
+
+        Raises:
+            :obj:`~switch.error.SwitchError`: If the user is not set or the callback is not set
+
+        This is a shortcut for :meth:`subscribe` with the endpoint set to ``/chat/queue/events``
+        """
+        subscription = await self.ws.subscribe(
+            "/chat/queue/events",
+            callback=lambda event: callback(self._parse_event(event)),
+        )
+        return subscription
+
+    def _parse_event(self, raw_message: WsMessage) -> ChatEvent:
+        try:
+            json_data = json.loads(raw_message.body)
+            type = json_data.get("type", "MESSAGE")
+            evt: ChatEvent = None
+            if type == EventType.MESSAGE.value:
+                evt = self.build_object(MessageEvent, json_data)
+                # evt = MessageEvent.build_from_json(json_data)
+            elif type == EventType.COMMAND.value:
+                evt = self.build_object(CommandEvent, json_data)
+                # evt = CommandEvent.build_from_json(json_data)
+            elif type == EventType.CALLBACK_QUERY.value:
+                evt = self.build_object(CallbackQueryEvent, json_data)
+                # evt = CallbackQueryEvent.build_from_json(json_data)
+            elif type == EventType.INLINE_QUERY.value:
+                evt = self.build_object(InlineQueryEvent, json_data)
+            else:
+                evt = self.build_object(ChatEvent, json_data)
+                # evt = ChatEvent.build_from_json(json_data)
+            return evt
+        except Exception as e:
+            logger.exception(e)
+
+    async def start(self):
+        """Start the chat websocket client
+        Raises:
+            :obj:`~switch.error.SwitchError`: If the user is not set
+        """
+        if self.user is None:
+            raise SwitchError("User is not set")
+        await self.ws.connect()
+        self._started = True
+
+    async def stop(self):
+        """Stop the chat websocket client"""
+        if self._started:
+            await self.ws.disconnect()
+            self._started = False
```

### Comparing `swibots-1.2.8/swibots/api/chat/controllers/message_controller.py` & `swibots-1.2.9/swibots/api/chat/controllers/message_controller.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,576 +1,575 @@
-import asyncio
-import json
-import logging
-from typing import TYPE_CHECKING, List, Optional
-from swibots.api.common.models import User, MediaUploadRequest, Media
-from swibots.api.chat.models import Message, GroupChatHistory, InlineMarkup, InlineQuery, InlineQueryAnswer
-from swibots.error import SwitchError
-from swibots.utils.types import JSONDict
-from swibots.api.community.models import Channel, Community, Group
-
-if TYPE_CHECKING:
-    from swibots.api.chat import ChatClient
-
-log = logging.getLogger(__name__)
-
-BASE_PATH = "/v1/message"
-
-
-class MessageController:
-    """Message controller
-
-    This controller is used to communicate with the message endpoints.
-
-    """
-
-    def __init__(self, client: "ChatClient"):
-        self.client = client
-
-    async def new_message(self, to: Optional[int | User] = None, channel: Optional[Channel | str] = None, group: Optional[Group | str] = None) -> Message:
-        """Create a new message"""
-        if isinstance(to, User):
-            to = to.id
-
-        if isinstance(channel, Channel):
-            channel = channel.id
-
-        if isinstance(group, Group):
-            group = group.id
-
-        return Message(
-            user_id=self.client.user.id,
-            receiver_id=to,
-            channel_id=channel,
-            group_id=group,
-            app=self.client.app,
-        )
-
-    async def get_messages(self, user_id: int = None) -> List[Message]:
-        """Get messages for a user
-
-        Parameters:
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The messages
-
-        Raises:
-            ``~switch.error.SwitchError``: If the messages could not be retrieved
-        """
-        if user_id is None:
-            user_id = self.client.user.id
-        log.debug("Getting messages for user %s", user_id)
-        response = await self.client.get(f"{BASE_PATH}/{user_id}")
-        return self.client.build_list(Message, response.data)
-
-    async def send_message(self, message: Message, media: MediaUploadRequest = None) -> Message:
-        """Send a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message``): The message to send
-            media (``~switch.api.common.models.MediaUploadRequest``, *optional*): The media to send with the message
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be sent
-        """
-        data = message.to_json_request()
-        log.debug("Sending message %s", json.dumps(data))
-
-        if media:
-            url = f"{BASE_PATH}/create-with-media"
-            data.update(media.data_to_request())
-            upload_fn = self.client.post(
-                url, form_data=data, files=media.file_to_request(url))
-            if media.block:
-                response = await upload_fn
-            else:
-                asyncio.get_event_loop().create_task(upload_fn)
-                return
-        else:
-            response = await self.client.post(f"{BASE_PATH}/create", data=data)
-        return self.client.build_object(Message, response.data["message"])
-
-    async def send_text(self, text: str, to: Optional[int | User] = None, channel: Optional[Channel | str] = None, group: Optional[Group | str] = None,  inline_markup: InlineMarkup = None, media: MediaUploadRequest = None) -> Message:
-        """Send a message with text
-
-        Parameters:
-            to (``int`` | ``~switch.api.common.models.User``, *optional*): The user id to send the message to. Defaults to the current user id.
-            text (``str``): The text to send
-            channel (``~switch.api.community.models.Channel``, *optional*): The channel to send the message to
-            group (``~switch.api.community.models.Group``, *optional*): The group to send the message to
-            inline_markup (``~switch.api.chat.models.InlineMarkup``, *optional*): The inline markup to send with the message
-            media (``~switch.api.common.models.MediaUploadRequest``, *optional*): The media to send with the message
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be sent
-        """
-        message = await self.new_message(to, channel, group)
-        message.message = text
-        message.inline_markup = inline_markup
-        return await self.send_message(message, media)
-
-    async def reply(self, message: int | Message, reply: Message, media: MediaUploadRequest = None) -> Message:
-        if isinstance(message, Message):
-            id = message.id
-        else:
-            id = message
-        reply.replied_to_id = id
-        return await self.send_message(reply, media)
-
-    async def reply_text(self, message: int | Message, text: str, inline_markup: InlineMarkup = None, media: MediaUploadRequest = None, cached_media: Media = None) -> Message:
-        """Reply to a message with text
-
-        Parameters:
-            message (``~switch.api.chat.models.Message``): The message to reply to
-            text (``str``): The text to reply with
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be sent
-        """
-        if isinstance(message, Message):
-            id = message.id
-        else:
-            id = message
-
-        m = Message(message=text, inline_markup=inline_markup,
-                    cached_media=cached_media)
-
-        return await self.reply(id, m, media)
-
-    async def edit_message(self, message: Message) -> Message:
-        """Edit a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message``): The message to edit
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be edited
-        """
-        data = message.to_json_request()
-        log.debug("Editing message %s", json.dumps(data))
-        response = await self.client.put(f"{BASE_PATH}?id={message.id}", data=data)
-        return self.client.build_object(Message, response.data["message"])
-
-    async def edit_message_text(self, message: int | Message, text: str, inline_markup: InlineMarkup = None) -> Message:
-        """Edit a message with text
-
-        Parameters:
-            message (``~switch.api.chat.models.Message``): The message to edit
-            text (``str``): The text to edit with
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be edited
-        """
-        if isinstance(message, Message):
-            id = message.id
-        else:
-            id = message
-        return await self.edit_message(Message(id=id, message=text, inline_markup=inline_markup))
-
-    async def delete_message(self, message: int | Message) -> bool:
-        """Delete a message
-
-        Parameters:
-            message (``int`` | ``~switch.api.chat.models.Message``): The message id or message to delete
-
-        Returns:
-            ``bool``: True if the message was deleted
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be deleted
-        """
-        if isinstance(message, Message):
-            id = message.id
-        else:
-            id = message
-        log.debug("Deleting message %s", id)
-        response = await self.client.delete(f"{BASE_PATH}/{id}")
-        return True
-
-    async def delete_messages_from_user(self, recipient_id: int, user_id: int = None) -> bool:
-        """Delete messages from a user
-
-        Parameters:
-            recipient_id (``int``): The recipient id
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-
-        Returns:
-            ``bool``: True if the messages were deleted
-
-        Raises:
-            ``~switch.error.SwitchError``: If the messages could not be deleted
-
-        """
-        log.debug("Deleting messages for user %s", recipient_id)
-        if user_id is None:
-            user_id = self.client.user.id
-
-        response = await self.client.delete(f"{BASE_PATH}/{user_id}/{recipient_id}")
-        return True
-
-    async def get_messages_between_users(
-        self, recipient_id: int, user_id: int = None, page_limit: int = 100, page_offset: int = 0
-    ) -> List[Message]:
-        """Get messages between two users
-
-        Parameters:
-            recipient_id (``int``): The recipient id
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-            page_limit (``int``, *optional*): The page limit. Defaults to 100.
-            page_offset (``int``, *optional*): The page offset. Defaults to 0.
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The messages
-
-        Raises:
-            ``~switch.error.SwitchError``: If the messages could not be retrieved
-        """
-        q = []
-        if page_limit:
-            q.append(f"pageLimit={page_limit}")
-        if page_offset:
-            q.append(f"pageOffset={page_offset}")
-
-        str_q = "&".join(q)
-
-        if user_id is None:
-            user_id = self.client.user.id
-
-        log.debug("Getting messages for user %s", recipient_id)
-        response = await self.client.get(f"{BASE_PATH}/{user_id}/{recipient_id}?{str_q}")
-        return self.client.build_list(Message, response.data["messages"])
-
-    async def forward_message(
-        self,
-        message: Message | int,
-        group_channel: Group | Channel | str = None,
-        receiver_id: str = None,
-    ) -> Message:
-        """Forward a message to a group or user
-
-        Parameters:
-            message (``~switch.api.chat.models.Message`` | ``int``): The message to forward
-            group_channel (``~switch.api.chat.models.Group`` | ``~switch.api.chat.models.Channel`` | ``str``, *optional*): The group or channel to forward to. Defaults to None.
-            receiver_id (``str``, *optional*): The user id to forward to. Defaults to None.
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be forwarded
-        """
-        if isinstance(message, Message):
-            id = message.id
-        else:
-            id = message
-
-        if isinstance(group_channel, Group):
-            group_channel = group_channel.id
-        elif isinstance(group_channel, Channel):
-            group_channel = group_channel.id
-        elif group_channel is not None:
-            group_channel = group_channel
-
-        q = []
-        if group_channel is not None:
-            q.append(f"groupChannelId={group_channel}")
-        if receiver_id is not None:
-            q.append(f"receiverId={receiver_id}")
-
-        strQuery = q.join("&")
-
-        log.debug("Forwarding message %s", id)
-        response = await self.client.post(f"{BASE_PATH}/forward/{id}?{strQuery}")
-        return self.client.build_object(Message, response.data["message"])
-        # return Message.build_from_json(response.data["message"])
-
-    async def get_message(self, message: int | Message) -> Message:
-        """Get a message by id
-
-        Parameters:
-            message (``int`` | ``~switch.api.chat.models.Message``): The message id or message to get, if a message is passed, the id will be extracted from it.
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be retrieved
-        """
-        if isinstance(message, Message):
-            id = message.id
-        else:
-            id = message
-        log.debug("Getting message %s", id)
-        response = await self.client.get(f"{BASE_PATH}/{id}")
-        return self.client.build_object(Message, response.data["message"])
-        # return Message.build_from_json(response.data["message"])
-
-    async def get_group_chat_history(
-        self,
-        group_id: str,
-        community_id: str,
-        user_id: int = None,
-        page_limit: int = 100,
-        page_offset=0,
-    ) -> GroupChatHistory:
-        """Get group chat history
-
-        Parameters:
-            group_id (``str``): The group id
-            community_id (``str``): The community id
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-            page_limit (``int``, *optional*): The page limit. Defaults to 100.
-            page_offset (``int``, *optional*): The page offset. Defaults to 0.
-
-        Returns:
-            ``~switch.api.chat.models.GroupChatHistory``: The group chat history
-
-        Raises:
-            ``~switch.error.SwitchError``: If the group chat history could not be retrieved
-
-        """
-        log.debug("Getting group chat history for group %s", group_id)
-        q = ["isChannel=false"]
-        if page_limit:
-            q.append(f"pageLimit={page_limit}")
-        else:
-            q.append(f"pageLimit=0")
-        if page_offset:
-            q.append(f"pageOffset={page_offset}")
-        else:
-            q.append(f"pageOffset=0")
-        if community_id:
-            q.append(f"communityId={community_id}")
-
-        str_q = "&".join(q)
-
-        if user_id is None:
-            user_id = self.client.user.id
-
-        response = await self.client.get(f"{BASE_PATH}/group/{user_id}/{group_id}?{str_q}")
-        return self.client.build_object(GroupChatHistory, response.data)
-        # return GroupChatHistory.build_from_json(response.data)
-
-    async def get_channel_chat_history(
-        self,
-        channel_id: str,
-        community_id: str,
-        user_id: int = None,
-        page_limit: int = 100,
-        page_offset=0,
-    ) -> GroupChatHistory:
-        """Get channel chat history
-
-        Parameters:
-            channel_id (``str``): The channel id
-            community_id (``str``): The community id
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-            page_limit (``int``, *optional*): The page limit. Defaults to 100.
-            page_offset (``int``, *optional*): The page offset. Defaults to 0.
-
-        Returns:
-            ``~switch.api.chat.models.ChannelChatHistory``: The channel chat history
-
-        Raises:
-            ``~switch.error.SwitchError``: If the channel chat history could not be retrieved
-
-        """
-        log.debug("Getting channel chat history for channel %s", channel_id)
-        q = ["isChannel=true"]
-        if page_limit:
-            q.append(f"pageLimit={page_limit}")
-        else:
-            q.append(f"pageLimit=0")
-        if page_offset:
-            q.append(f"pageOffset={page_offset}")
-        else:
-            q.append(f"pageOffset=0")
-        if community_id:
-            q.append(f"communityId={community_id}")
-
-        str_q = "&".join(q)
-
-        if user_id is None:
-            user_id = self.client.user.id
-
-        response = await self.client.get(f"{BASE_PATH}/group/{user_id}/{channel_id}?{str_q}")
-        return self.client.build_object(GroupChatHistory, response.data)
-        # return GroupChatHistory.build_from_json(response.data)
-
-    async def get_community_media_files(self, community_id: str) -> List[Message]:
-        """Get community media files
-
-        Parameters:
-            community_id (``str``): The community id
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The community media files
-
-        Raises:
-            ``~switch.error.SwitchError``: If the community media files could not be retrieved
-        """
-        log.debug("Getting community media files for community %s", community_id)
-        response = await self.client.get(f"{BASE_PATH}/media?communityId={community_id}")
-        return self.client.build_list(Message, response.data)
-        # return Message.build_from_json_list(response.data)
-
-    async def get_community_media_files_by_status(
-        self, community_id: str, status: str
-    ) -> List[Message]:
-        """Get community media files by status
-
-        Parameters:
-            community_id (``str``): The community id
-            status (``str``): The status of the media files
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The community media files
-
-
-        Raises:
-            ``~switch.error.SwitchError``: If the community media files could not be retrieved
-        """
-        log.debug("Getting community media files for community %s", community_id)
-        response = await self.client.get(
-            f"{BASE_PATH}/media?communityId={community_id}&status={status}"
-        )
-        return self.client.build_list(Message, response.data)
-        # return Message.build_from_json_list(response.data)
-
-    async def get_user_media_files(self, user_id: int = None) -> List[Message]:
-        """Get user media files
-
-
-        Parameters:
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The user media files
-
-        Raises:
-            ``~switch.error.SwitchError``: If the user media files could not be retrieved
-        """
-        if user_id is None:
-            user_id = self.client.user.id
-        log.debug("Getting user media files for user %s", user_id)
-        response = await self.client.get(f"{BASE_PATH}/media/{user_id}")
-        return self.client.build_list(Message, response.data)
-        # return Message.build_from_json_list(response.data)
-
-    async def clear_conversation(self, receiver_id: int) -> bool:
-        """Clear a conversation
-
-        Parameters:
-            receiver_id (``int``): The receiver id
-
-        Returns:
-            ``bool``: True if the conversation was cleared
-
-        Raises:
-            ``~switch.error.SwitchError``: If the conversation could not be cleared
-        """
-        log.debug("Clearing conversation %s", receiver_id)
-        response = await self.client.get(f"{BASE_PATH}/clearconversationwith/{receiver_id}")
-        return True
-
-    async def get_flag_messages(self, user_id: int = None) -> List[Message]:
-        """Get flagged messages
-
-        Parameters:
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The flagged messages
-
-        Raises:
-            ``~switch.error.SwitchError``: If the flagged messages could not be retrieved
-        """
-        if user_id is None:
-            user_id = self.client.user.id
-
-        log.debug("Get flag messages for %s", user_id)
-        response = await self.client.get(f"{BASE_PATH}/flag?userId={user_id}")
-        return self.client.build_list(Message, response.data)
-        # return Message.build_from_json_list(response.data)
-
-    async def flag_message(self, message: Message | int) -> bool:
-        """Flag a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message`` | ``int``): The message to flag
-
-        Returns:
-            ``bool``: True if the message was flagged
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be flagged
-        """
-        if isinstance(message, Message):
-            message_id = message.id
-        else:
-            message_id = message
-        log.debug("Flagging message %s", message_id)
-        response = await self.client.post(f"{BASE_PATH}/flag?messageId={message_id}")
-        return True
-
-    async def get_unread_messages_count(self, user_id: int = None) -> int:
-        """Get unread messages
-
-        Parameters:
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-
-        Returns:
-            ``int``: The unread messages count
-        """
-        if user_id is None:
-            user_id = self.client.user.id
-
-        log.debug("Get unread messages count for %s", user_id)
-        response = await self.client.get(f"{BASE_PATH}/unread-messages?userId={user_id}")
-        return response.data
-
-    async def answer_inline_query(self, query: InlineQuery, answer: InlineQueryAnswer) -> bool:
-        """Answer an inline query
-
-        Parameters:
-            query (``~switch.api.chat.models.InlineQuery``): The inline query
-            answer (``~switch.api.chat.models.InlineQueryAnser``): The answer
-
-        Returns:
-            ``bool``: True if the query was answered
-
-        Raises:
-            ``~switch.error.SwitchError``: If the query could not be answered
-        """
-        if not isinstance(query, InlineQuery):
-            raise TypeError("query must be an InlineQuery instance")
-
-        if isinstance(answer, str):
-            answer = InlineQueryAnswer(query_id=query.query_id, title=answer, results=[
-            ], cache_time=0, is_personal=True, next_offset=None, pm_text=None, pm_parameter=None, user_id=query.user_id)
-
-        if isinstance(answer, List):
-            answer = InlineQueryAnswer(query_id=query.query_id, title=None, results=answer, cache_time=0,
-                                       is_personal=True, next_offset=None, pm_text=None, pm_parameter=None, user_id=query.user_id)
-
-        if not answer.user_id:
-            answer.user_id = query.user_id
-
-        log.debug("Answering inline query %s", query.query_id)
-        response = await self.client.post(f"{BASE_PATH}/inline/answer", answer.to_json_request())
-        return response.data
+import asyncio
+import json
+import logging
+from typing import TYPE_CHECKING, List, Optional
+
+from swibots.api.chat.models import Message, GroupChatHistory, InlineMarkup, InlineQuery, InlineQueryAnswer
+from swibots.api.common.models import User, MediaUploadRequest, Media
+from swibots.api.community.models import Channel, Group
+
+if TYPE_CHECKING:
+    from swibots.api.chat import ChatClient
+
+log = logging.getLogger(__name__)
+
+BASE_PATH = "/v1/message"
+
+
+class MessageController:
+    """Message controller
+
+    This controller is used to communicate with the message endpoints.
+
+    """
+
+    def __init__(self, client: "ChatClient"):
+        self.client = client
+
+    async def new_message(self, to: Optional[int | User] = None, channel: Optional[Channel | str] = None, group: Optional[Group | str] = None) -> Message:
+        """Create a new message"""
+        if isinstance(to, User):
+            to = to.id
+
+        if isinstance(channel, Channel):
+            channel = channel.id
+
+        if isinstance(group, Group):
+            group = group.id
+
+        return Message(
+            user_id=self.client.user.id,
+            receiver_id=to,
+            channel_id=channel,
+            group_id=group,
+            app=self.client.app,
+        )
+
+    async def get_messages(self, user_id: int = None) -> List[Message]:
+        """Get messages for a user
+
+        Parameters:
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The messages
+
+        Raises:
+            ``~switch.error.SwitchError``: If the messages could not be retrieved
+        """
+        if user_id is None:
+            user_id = self.client.user.id
+        log.debug("Getting messages for user %s", user_id)
+        response = await self.client.get(f"{BASE_PATH}/{user_id}")
+        return self.client.build_list(Message, response.data)
+
+    async def send_message(self, message: Message, media: MediaUploadRequest = None) -> Message:
+        """Send a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to send
+            media (``~switch.api.common.models.MediaUploadRequest``, *optional*): The media to send with the message
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be sent
+        """
+        data = message.to_json_request()
+        log.debug("Sending message %s", json.dumps(data))
+
+        if media:
+            url = f"{BASE_PATH}/create-with-media"
+            form_data = message.to_form_data()
+            form_data.update(media.data_to_request())
+            upload_fn = self.client.post(url, form_data=form_data, files=media.file_to_request(url))
+            if media.block:
+                response = await upload_fn
+            else:
+                asyncio.get_event_loop().create_task(upload_fn)
+                return
+        else:
+            response = await self.client.post(f"{BASE_PATH}/create", data=data)
+        return self.client.build_object(Message, response.data["message"])
+
+    async def send_text(self, text: str, to: Optional[int | User] = None, channel: Optional[Channel | str] = None, group: Optional[Group | str] = None,  inline_markup: InlineMarkup = None, media: MediaUploadRequest = None) -> Message:
+        """Send a message with text
+
+        Parameters:
+            to (``int`` | ``~switch.api.common.models.User``, *optional*): The user id to send the message to. Defaults to the current user id.
+            text (``str``): The text to send
+            channel (``~switch.api.community.models.Channel``, *optional*): The channel to send the message to
+            group (``~switch.api.community.models.Group``, *optional*): The group to send the message to
+            inline_markup (``~switch.api.chat.models.InlineMarkup``, *optional*): The inline markup to send with the message
+            media (``~switch.api.common.models.MediaUploadRequest``, *optional*): The media to send with the message
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be sent
+        """
+        message = await self.new_message(to, channel, group)
+        message.message = text
+        message.inline_markup = inline_markup
+        return await self.send_message(message, media)
+
+    async def reply(self, message: int | Message, reply: Message, media: MediaUploadRequest = None) -> Message:
+        if isinstance(message, Message):
+            id = message.id
+        else:
+            id = message
+        reply.replied_to_id = id
+        return await self.send_message(reply, media)
+
+    async def reply_text(self, message: int | Message, text: str, inline_markup: InlineMarkup = None, media: MediaUploadRequest = None, cached_media: Media = None) -> Message:
+        """Reply to a message with text
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to reply to
+            text (``str``): The text to reply with
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be sent
+        """
+        if isinstance(message, Message):
+            id = message.id
+        else:
+            id = message
+
+        m = Message(message=text, inline_markup=inline_markup,
+                    cached_media=cached_media)
+
+        return await self.reply(id, m, media)
+
+    async def edit_message(self, message: Message) -> Message:
+        """Edit a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to edit
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be edited
+        """
+        data = message.to_json_request()
+        log.debug("Editing message %s", json.dumps(data))
+        response = await self.client.put(f"{BASE_PATH}?id={message.id}", data=data)
+        return self.client.build_object(Message, response.data["message"])
+
+    async def edit_message_text(self, message: int | Message, text: str, inline_markup: InlineMarkup = None) -> Message:
+        """Edit a message with text
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to edit
+            text (``str``): The text to edit with
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be edited
+        """
+        if isinstance(message, Message):
+            id = message.id
+        else:
+            id = message
+        return await self.edit_message(Message(id=id, message=text, inline_markup=inline_markup))
+
+    async def delete_message(self, message: int | Message) -> bool:
+        """Delete a message
+
+        Parameters:
+            message (``int`` | ``~switch.api.chat.models.Message``): The message id or message to delete
+
+        Returns:
+            ``bool``: True if the message was deleted
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be deleted
+        """
+        if isinstance(message, Message):
+            id = message.id
+        else:
+            id = message
+        log.debug("Deleting message %s", id)
+        response = await self.client.delete(f"{BASE_PATH}/{id}")
+        return True
+
+    async def delete_messages_from_user(self, recipient_id: int, user_id: int = None) -> bool:
+        """Delete messages from a user
+
+        Parameters:
+            recipient_id (``int``): The recipient id
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+
+        Returns:
+            ``bool``: True if the messages were deleted
+
+        Raises:
+            ``~switch.error.SwitchError``: If the messages could not be deleted
+
+        """
+        log.debug("Deleting messages for user %s", recipient_id)
+        if user_id is None:
+            user_id = self.client.user.id
+
+        response = await self.client.delete(f"{BASE_PATH}/{user_id}/{recipient_id}")
+        return True
+
+    async def get_messages_between_users(
+        self, recipient_id: int, user_id: int = None, page_limit: int = 100, page_offset: int = 0
+    ) -> List[Message]:
+        """Get messages between two users
+
+        Parameters:
+            recipient_id (``int``): The recipient id
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+            page_limit (``int``, *optional*): The page limit. Defaults to 100.
+            page_offset (``int``, *optional*): The page offset. Defaults to 0.
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The messages
+
+        Raises:
+            ``~switch.error.SwitchError``: If the messages could not be retrieved
+        """
+        q = []
+        if page_limit:
+            q.append(f"pageLimit={page_limit}")
+        if page_offset:
+            q.append(f"pageOffset={page_offset}")
+
+        str_q = "&".join(q)
+
+        if user_id is None:
+            user_id = self.client.user.id
+
+        log.debug("Getting messages for user %s", recipient_id)
+        response = await self.client.get(f"{BASE_PATH}/{user_id}/{recipient_id}?{str_q}")
+        return self.client.build_list(Message, response.data["messages"])
+
+    async def forward_message(
+        self,
+        message: Message | int,
+        group_channel: Group | Channel | str = None,
+        receiver_id: str = None,
+    ) -> Message:
+        """Forward a message to a group or user
+
+        Parameters:
+            message (``~switch.api.chat.models.Message`` | ``int``): The message to forward
+            group_channel (``~switch.api.chat.models.Group`` | ``~switch.api.chat.models.Channel`` | ``str``, *optional*): The group or channel to forward to. Defaults to None.
+            receiver_id (``str``, *optional*): The user id to forward to. Defaults to None.
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be forwarded
+        """
+        if isinstance(message, Message):
+            id = message.id
+        else:
+            id = message
+
+        if isinstance(group_channel, Group):
+            group_channel = group_channel.id
+        elif isinstance(group_channel, Channel):
+            group_channel = group_channel.id
+        elif group_channel is not None:
+            group_channel = group_channel
+
+        q = []
+        if group_channel is not None:
+            q.append(f"groupChannelId={group_channel}")
+        if receiver_id is not None:
+            q.append(f"receiverId={receiver_id}")
+
+        strQuery = q.join("&")
+
+        log.debug("Forwarding message %s", id)
+        response = await self.client.post(f"{BASE_PATH}/forward/{id}?{strQuery}")
+        return self.client.build_object(Message, response.data["message"])
+        # return Message.build_from_json(response.data["message"])
+
+    async def get_message(self, message: int | Message) -> Message:
+        """Get a message by id
+
+        Parameters:
+            message (``int`` | ``~switch.api.chat.models.Message``): The message id or message to get, if a message is passed, the id will be extracted from it.
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be retrieved
+        """
+        if isinstance(message, Message):
+            id = message.id
+        else:
+            id = message
+        log.debug("Getting message %s", id)
+        response = await self.client.get(f"{BASE_PATH}/{id}")
+        return self.client.build_object(Message, response.data["message"])
+        # return Message.build_from_json(response.data["message"])
+
+    async def get_group_chat_history(
+        self,
+        group_id: str,
+        community_id: str,
+        user_id: int = None,
+        page_limit: int = 100,
+        page_offset=0,
+    ) -> GroupChatHistory:
+        """Get group chat history
+
+        Parameters:
+            group_id (``str``): The group id
+            community_id (``str``): The community id
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+            page_limit (``int``, *optional*): The page limit. Defaults to 100.
+            page_offset (``int``, *optional*): The page offset. Defaults to 0.
+
+        Returns:
+            ``~switch.api.chat.models.GroupChatHistory``: The group chat history
+
+        Raises:
+            ``~switch.error.SwitchError``: If the group chat history could not be retrieved
+
+        """
+        log.debug("Getting group chat history for group %s", group_id)
+        q = ["isChannel=false"]
+        if page_limit:
+            q.append(f"pageLimit={page_limit}")
+        else:
+            q.append(f"pageLimit=0")
+        if page_offset:
+            q.append(f"pageOffset={page_offset}")
+        else:
+            q.append(f"pageOffset=0")
+        if community_id:
+            q.append(f"communityId={community_id}")
+
+        str_q = "&".join(q)
+
+        if user_id is None:
+            user_id = self.client.user.id
+
+        response = await self.client.get(f"{BASE_PATH}/group/{user_id}/{group_id}?{str_q}")
+        return self.client.build_object(GroupChatHistory, response.data)
+        # return GroupChatHistory.build_from_json(response.data)
+
+    async def get_channel_chat_history(
+        self,
+        channel_id: str,
+        community_id: str,
+        user_id: int = None,
+        page_limit: int = 100,
+        page_offset=0,
+    ) -> GroupChatHistory:
+        """Get channel chat history
+
+        Parameters:
+            channel_id (``str``): The channel id
+            community_id (``str``): The community id
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+            page_limit (``int``, *optional*): The page limit. Defaults to 100.
+            page_offset (``int``, *optional*): The page offset. Defaults to 0.
+
+        Returns:
+            ``~switch.api.chat.models.ChannelChatHistory``: The channel chat history
+
+        Raises:
+            ``~switch.error.SwitchError``: If the channel chat history could not be retrieved
+
+        """
+        log.debug("Getting channel chat history for channel %s", channel_id)
+        q = ["isChannel=true"]
+        if page_limit:
+            q.append(f"pageLimit={page_limit}")
+        else:
+            q.append(f"pageLimit=0")
+        if page_offset:
+            q.append(f"pageOffset={page_offset}")
+        else:
+            q.append(f"pageOffset=0")
+        if community_id:
+            q.append(f"communityId={community_id}")
+
+        str_q = "&".join(q)
+
+        if user_id is None:
+            user_id = self.client.user.id
+
+        response = await self.client.get(f"{BASE_PATH}/group/{user_id}/{channel_id}?{str_q}")
+        return self.client.build_object(GroupChatHistory, response.data)
+        # return GroupChatHistory.build_from_json(response.data)
+
+    async def get_community_media_files(self, community_id: str) -> List[Message]:
+        """Get community media files
+
+        Parameters:
+            community_id (``str``): The community id
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The community media files
+
+        Raises:
+            ``~switch.error.SwitchError``: If the community media files could not be retrieved
+        """
+        log.debug("Getting community media files for community %s", community_id)
+        response = await self.client.get(f"{BASE_PATH}/media?communityId={community_id}")
+        return self.client.build_list(Message, response.data)
+        # return Message.build_from_json_list(response.data)
+
+    async def get_community_media_files_by_status(
+        self, community_id: str, status: str
+    ) -> List[Message]:
+        """Get community media files by status
+
+        Parameters:
+            community_id (``str``): The community id
+            status (``str``): The status of the media files
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The community media files
+
+
+        Raises:
+            ``~switch.error.SwitchError``: If the community media files could not be retrieved
+        """
+        log.debug("Getting community media files for community %s", community_id)
+        response = await self.client.get(
+            f"{BASE_PATH}/media?communityId={community_id}&status={status}"
+        )
+        return self.client.build_list(Message, response.data)
+        # return Message.build_from_json_list(response.data)
+
+    async def get_user_media_files(self, user_id: int = None) -> List[Message]:
+        """Get user media files
+
+
+        Parameters:
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The user media files
+
+        Raises:
+            ``~switch.error.SwitchError``: If the user media files could not be retrieved
+        """
+        if user_id is None:
+            user_id = self.client.user.id
+        log.debug("Getting user media files for user %s", user_id)
+        response = await self.client.get(f"{BASE_PATH}/media/{user_id}")
+        return self.client.build_list(Message, response.data)
+        # return Message.build_from_json_list(response.data)
+
+    async def clear_conversation(self, receiver_id: int) -> bool:
+        """Clear a conversation
+
+        Parameters:
+            receiver_id (``int``): The receiver id
+
+        Returns:
+            ``bool``: True if the conversation was cleared
+
+        Raises:
+            ``~switch.error.SwitchError``: If the conversation could not be cleared
+        """
+        log.debug("Clearing conversation %s", receiver_id)
+        response = await self.client.get(f"{BASE_PATH}/clearconversationwith/{receiver_id}")
+        return True
+
+    async def get_flag_messages(self, user_id: int = None) -> List[Message]:
+        """Get flagged messages
+
+        Parameters:
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The flagged messages
+
+        Raises:
+            ``~switch.error.SwitchError``: If the flagged messages could not be retrieved
+        """
+        if user_id is None:
+            user_id = self.client.user.id
+
+        log.debug("Get flag messages for %s", user_id)
+        response = await self.client.get(f"{BASE_PATH}/flag?userId={user_id}")
+        return self.client.build_list(Message, response.data)
+        # return Message.build_from_json_list(response.data)
+
+    async def flag_message(self, message: Message | int) -> bool:
+        """Flag a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message`` | ``int``): The message to flag
+
+        Returns:
+            ``bool``: True if the message was flagged
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be flagged
+        """
+        if isinstance(message, Message):
+            message_id = message.id
+        else:
+            message_id = message
+        log.debug("Flagging message %s", message_id)
+        response = await self.client.post(f"{BASE_PATH}/flag?messageId={message_id}")
+        return True
+
+    async def get_unread_messages_count(self, user_id: int = None) -> int:
+        """Get unread messages
+
+        Parameters:
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+
+        Returns:
+            ``int``: The unread messages count
+        """
+        if user_id is None:
+            user_id = self.client.user.id
+
+        log.debug("Get unread messages count for %s", user_id)
+        response = await self.client.get(f"{BASE_PATH}/unread-messages?userId={user_id}")
+        return response.data
+
+    async def answer_inline_query(self, query: InlineQuery, answer: InlineQueryAnswer) -> bool:
+        """Answer an inline query
+
+        Parameters:
+            query (``~switch.api.chat.models.InlineQuery``): The inline query
+            answer (``~switch.api.chat.models.InlineQueryAnser``): The answer
+
+        Returns:
+            ``bool``: True if the query was answered
+
+        Raises:
+            ``~switch.error.SwitchError``: If the query could not be answered
+        """
+        if not isinstance(query, InlineQuery):
+            raise TypeError("query must be an InlineQuery instance")
+
+        if isinstance(answer, str):
+            answer = InlineQueryAnswer(query_id=query.query_id, title=answer, results=[
+            ], cache_time=0, is_personal=True, next_offset=None, pm_text=None, pm_parameter=None, user_id=query.user_id)
+
+        if isinstance(answer, List):
+            answer = InlineQueryAnswer(query_id=query.query_id, title=None, results=answer, cache_time=0,
+                                       is_personal=True, next_offset=None, pm_text=None, pm_parameter=None, user_id=query.user_id)
+
+        if not answer.user_id:
+            answer.user_id = query.user_id
+
+        log.debug("Answering inline query %s", query.query_id)
+        response = await self.client.post(f"{BASE_PATH}/inline/answer", answer.to_json_request())
+        return response.data
```

### Comparing `swibots-1.2.8/swibots/api/chat/events/callback_query_event.py` & `swibots-1.2.9/swibots/api/chat/events/callback_query_event.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-from typing import Optional
-import swibots
-from swibots.api.common.events.event import Event
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.api.chat.models.message import Message
-from swibots.types import EventType
-from swibots.utils.types import JSONDict
-from .command_event import CommandEvent
-
-
-class CallbackQueryEvent(CommandEvent):
-    """Message event"""
-
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        type: Optional[EventType] = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-        message: Optional[Message] = None,
-        command: Optional[str] = None,
-        params: Optional[str] = None,
-        callback_data: Optional[JSONDict] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=type or EventType.CALLBACK_QUERY,
-            community_id=community_id,
-            community=community,
-            group_id=group_id,
-            group=group,
-            channel_id=channel_id,
-            channel=channel,
-            action_by_id=action_by_id,
-            action_by=action_by,
-            data=data,
-            user_id=user_id,
-            user=user,
-            message=message,
-            command=command,
-            params=params,
-        )
-        self.callback_data = callback_data
-
-    def from_json(self, data: JSONDict) -> "CallbackQueryEvent":
-        super().from_json(data)
-        if data is not None:
-            self.callback_data = self.data.get("callbackData")
-        return self
+from typing import Optional
+import swibots
+from swibots.api.common.events.event import Event
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.api.chat.models.message import Message
+from swibots.types import EventType
+from swibots.utils.types import JSONDict
+from .command_event import CommandEvent
+
+
+class CallbackQueryEvent(CommandEvent):
+    """Message event"""
+
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        type: Optional[EventType] = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+        message: Optional[Message] = None,
+        command: Optional[str] = None,
+        params: Optional[str] = None,
+        callback_data: Optional[JSONDict] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=type or EventType.CALLBACK_QUERY,
+            community_id=community_id,
+            community=community,
+            group_id=group_id,
+            group=group,
+            channel_id=channel_id,
+            channel=channel,
+            action_by_id=action_by_id,
+            action_by=action_by,
+            data=data,
+            user_id=user_id,
+            user=user,
+            message=message,
+            command=command,
+            params=params,
+        )
+        self.callback_data = callback_data
+
+    def from_json(self, data: JSONDict) -> "CallbackQueryEvent":
+        super().from_json(data)
+        if data is not None:
+            self.callback_data = self.data.get("callbackData")
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/chat/events/command_event.py` & `swibots-1.2.9/swibots/api/chat/events/command_event.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from typing import Optional
-import swibots
-from swibots.api.common.events.event import Event
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.api.chat.models.message import Message
-from swibots.types import EventType
-from swibots.utils.types import JSONDict
-from .message_event import MessageEvent
-
-
-class CommandEvent(MessageEvent):
-    """Message event"""
-
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        type: Optional[EventType] = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-        message: Optional[Message] = None,
-        message_id: Optional[int] = None,
-        command: Optional[str] = None,
-        params: Optional[str] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=type or EventType.COMMAND,
-            community_id=community_id,
-            community=community,
-            group_id=group_id,
-            group=group,
-            channel_id=channel_id,
-            channel=channel,
-            action_by_id=action_by_id,
-            action_by=action_by,
-            data=data,
-            user_id=user_id,
-            user=user,
-            message_id = message_id,
-            message=message,
-        )
-        self.command = command
-        self.params = params
-
-    def from_json(self, data: JSONDict) -> "CommandEvent":
-        super().from_json(data)
-        if self.data is not None:
-            self.command = self.data.get("command")
-            self.params = self.data.get("commandParams")
-        return self
+from typing import Optional
+import swibots
+from swibots.api.common.events.event import Event
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.api.chat.models.message import Message
+from swibots.types import EventType
+from swibots.utils.types import JSONDict
+from .message_event import MessageEvent
+
+
+class CommandEvent(MessageEvent):
+    """Message event"""
+
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        type: Optional[EventType] = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+        message: Optional[Message] = None,
+        message_id: Optional[int] = None,
+        command: Optional[str] = None,
+        params: Optional[str] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=type or EventType.COMMAND,
+            community_id=community_id,
+            community=community,
+            group_id=group_id,
+            group=group,
+            channel_id=channel_id,
+            channel=channel,
+            action_by_id=action_by_id,
+            action_by=action_by,
+            data=data,
+            user_id=user_id,
+            user=user,
+            message_id = message_id,
+            message=message,
+        )
+        self.command = command
+        self.params = params
+
+    def from_json(self, data: JSONDict) -> "CommandEvent":
+        super().from_json(data)
+        if self.data is not None:
+            self.command = self.data.get("command")
+            self.params = self.data.get("commandParams")
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/chat/events/inline_query_event.py` & `swibots-1.2.9/swibots/api/chat/events/inline_query_event.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import Optional
-import swibots
-from swibots.api.common.events.event import Event
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.api.chat.models.message import Message
-from swibots.api.chat.models.inline.inline_query import InlineQuery
-from swibots.types import EventType
-from swibots.utils.types import JSONDict
-from .chat_event import ChatEvent
-
-
-class InlineQueryEvent(ChatEvent):
-    """Message event"""
-
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        type: Optional[EventType] = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[int] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[int] = None,
-        user: Optional[User] = None,
-        query: Optional[str] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=type or EventType.MESSAGE,
-            community_id=community_id,
-            community=community,
-            group_id=group_id,
-            group=group,
-            channel_id=channel_id,
-            channel=channel,
-            action_by_id=action_by_id,
-            action_by=action_by,
-            data=data,
-            user_id=user_id,
-            user=user,
-        )
-        self.query = query
-
-    def from_json(self, data: JSONDict) -> "InlineQueryEvent":
-        super().from_json(data)
-        if self.data is not None:
-            self.query = InlineQuery.build_from_json(
-                self.data.get("inlineQuery"), self.app)
-            self.user = self.action_by
-            self.user_id = self.action_by_id
-
-        self.query.user = self.user
-        self.query.user_id = self.user_id
-
-        return self
+from typing import Optional
+import swibots
+from swibots.api.common.events.event import Event
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.api.chat.models.message import Message
+from swibots.api.chat.models.inline.inline_query import InlineQuery
+from swibots.types import EventType
+from swibots.utils.types import JSONDict
+from .chat_event import ChatEvent
+
+
+class InlineQueryEvent(ChatEvent):
+    """Message event"""
+
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        type: Optional[EventType] = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[int] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[int] = None,
+        user: Optional[User] = None,
+        query: Optional[str] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=type or EventType.MESSAGE,
+            community_id=community_id,
+            community=community,
+            group_id=group_id,
+            group=group,
+            channel_id=channel_id,
+            channel=channel,
+            action_by_id=action_by_id,
+            action_by=action_by,
+            data=data,
+            user_id=user_id,
+            user=user,
+        )
+        self.query = query
+
+    def from_json(self, data: JSONDict) -> "InlineQueryEvent":
+        super().from_json(data)
+        if self.data is not None:
+            self.query = InlineQuery.build_from_json(
+                self.data.get("inlineQuery"), self.app)
+            self.user = self.action_by
+            self.user_id = self.action_by_id
+
+        self.query.user = self.user
+        self.query.user_id = self.user_id
+
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/chat/events/message_event.py` & `swibots-1.2.9/swibots/api/chat/events/message_event.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-from typing import Optional
-import swibots
-from swibots.api.common.events.event import Event
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.api.chat.models.message import Message
-from swibots.types import EventType
-from swibots.utils.types import JSONDict
-from .chat_event import ChatEvent
-
-
-class MessageEvent(ChatEvent):
-    """Message event"""
-
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        type: Optional[EventType] = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-        message: Optional[Message] = None,
-        message_id: Optional[int] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=type or EventType.MESSAGE,
-            community_id=community_id,
-            community=community,
-            group_id=group_id,
-            group=group,
-            channel_id=channel_id,
-            channel=channel,
-            action_by_id=action_by_id,
-            action_by=action_by,
-            data=data,
-            user_id=user_id,
-            user=user,
-        )
-        self.message_id = message_id
-        self.message = message
-
-    def from_json(self, data: JSONDict) -> "MessageEvent":
-        super().from_json(data)
-        if self.data is not None:
-            self.message_id = data.get("messageId") or 0
-            self.message: Message = Message.build_from_json(
-                self.data.get("message"), self.app)
-
-            self.message.user = self.user
-            self.message.community = self.community
-            self.message.group = self.group
-            self.message.channel = self.channel
-            self.message.receiver_id = self.message.receiver_id or self.data.get(
-                "receiverId") or 0
-            self.message.receiver = User.build_from_json(
-                self.data.get("receiver") or {}, self.app)
-
-        return self
+from typing import Optional
+import swibots
+from swibots.api.common.events.event import Event
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.api.chat.models.message import Message
+from swibots.types import EventType
+from swibots.utils.types import JSONDict
+from .chat_event import ChatEvent
+
+
+class MessageEvent(ChatEvent):
+    """Message event"""
+
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        type: Optional[EventType] = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+        message: Optional[Message] = None,
+        message_id: Optional[int] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=type or EventType.MESSAGE,
+            community_id=community_id,
+            community=community,
+            group_id=group_id,
+            group=group,
+            channel_id=channel_id,
+            channel=channel,
+            action_by_id=action_by_id,
+            action_by=action_by,
+            data=data,
+            user_id=user_id,
+            user=user,
+        )
+        self.message_id = message_id
+        self.message = message
+
+    def from_json(self, data: JSONDict) -> "MessageEvent":
+        super().from_json(data)
+        if self.data is not None:
+            self.message_id = data.get("messageId") or 0
+            self.message: Message = Message.build_from_json(
+                self.data.get("message"), self.app)
+
+            self.message.user = self.user
+            self.message.community = self.community
+            self.message.group = self.group
+            self.message.channel = self.channel
+            self.message.receiver_id = self.message.receiver_id or self.data.get(
+                "receiverId") or 0
+            self.message.receiver = User.build_from_json(
+                self.data.get("receiver") or {}, self.app)
+
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/__init__.py` & `swibots-1.2.9/swibots/api/chat/methods/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from .clear_conversation import ClearConversation
-from .delete_message import DeleteMessage
-from .delete_messages_from_user import DeleteMessagesFromUser
-from .edit_message import EditMessage
-from .flag_message import FlagMessage
-from .forward_message import ForwardMessage
-from .get_channel_chat_history import GetChannelChatHistory
-from .get_group_chat_history import GetGroupChatHistory
-from .get_community_media_files import GetCommunityMediaFiles
-from .get_community_media_files_by_status import GetCommunityMediaFilesByStatus
-from .get_flag_messages import GetFlagMessages
-from .flag_message import FlagMessage
-from .get_message import GetMessage
-from .get_messages_between_users import GetMessagesBetweenUsers
-from .get_messages import GetMessages
-from .get_unread_messages_count import GetUnreadMessagesCount
-from .get_user_media_files import GetUserMediaFiles
-from .send_message import SendMessage
-from .send_text import SendText
-from .reply_message_text import ReplyMessageText
-from .reply_message import ReplyMessage
-from .edit_message_text import EditMessageText
-from .answer_inline_query import AnswerInlineQuery
-from .download_media import DownloadMedia
-
-
-class ChatMethods(
-    ClearConversation,
-    DeleteMessage,
-    DeleteMessagesFromUser,
-    EditMessage,
-    FlagMessage,
-    ForwardMessage,
-    GetChannelChatHistory,
-    GetGroupChatHistory,
-    GetCommunityMediaFiles,
-    GetCommunityMediaFilesByStatus,
-    GetFlagMessages,
-    GetMessage,
-    GetMessagesBetweenUsers,
-    GetMessages,
-    GetUnreadMessagesCount,
-    GetUserMediaFiles,
-    SendMessage,
-    SendText,
-    ReplyMessageText,
-    ReplyMessage,
-    EditMessageText,
-    AnswerInlineQuery,
-    DownloadMedia,
-):
-    pass
+from .clear_conversation import ClearConversation
+from .delete_message import DeleteMessage
+from .delete_messages_from_user import DeleteMessagesFromUser
+from .edit_message import EditMessage
+from .flag_message import FlagMessage
+from .forward_message import ForwardMessage
+from .get_channel_chat_history import GetChannelChatHistory
+from .get_group_chat_history import GetGroupChatHistory
+from .get_community_media_files import GetCommunityMediaFiles
+from .get_community_media_files_by_status import GetCommunityMediaFilesByStatus
+from .get_flag_messages import GetFlagMessages
+from .flag_message import FlagMessage
+from .get_message import GetMessage
+from .get_messages_between_users import GetMessagesBetweenUsers
+from .get_messages import GetMessages
+from .get_unread_messages_count import GetUnreadMessagesCount
+from .get_user_media_files import GetUserMediaFiles
+from .send_message import SendMessage
+from .send_text import SendText
+from .reply_message_text import ReplyMessageText
+from .reply_message import ReplyMessage
+from .edit_message_text import EditMessageText
+from .answer_inline_query import AnswerInlineQuery
+from .download_media import DownloadMedia
+
+
+class ChatMethods(
+    ClearConversation,
+    DeleteMessage,
+    DeleteMessagesFromUser,
+    EditMessage,
+    FlagMessage,
+    ForwardMessage,
+    GetChannelChatHistory,
+    GetGroupChatHistory,
+    GetCommunityMediaFiles,
+    GetCommunityMediaFilesByStatus,
+    GetFlagMessages,
+    GetMessage,
+    GetMessagesBetweenUsers,
+    GetMessages,
+    GetUnreadMessagesCount,
+    GetUserMediaFiles,
+    SendMessage,
+    SendText,
+    ReplyMessageText,
+    ReplyMessage,
+    EditMessageText,
+    AnswerInlineQuery,
+    DownloadMedia,
+):
+    pass
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/answer_inline_query.py` & `swibots-1.2.9/swibots/api/chat/methods/answer_inline_query.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.chat.models import InlineQueryAnswer, InlineQuery
-
-
-class AnswerInlineQuery:
-    async def answer_inline_query(self: "swibots.ApiClient", query: InlineQuery, answer: InlineQueryAnswer) -> bool:
-        """Answer inline query
-
-        Args:
-            query (:obj:`InlineQuery`): Inline query to answer to
-            answer (str | InlineQueryAnswer): Answer to inline query, it can be either a string or an InlineQueryAnswer object, if it's a string, it will be used as the text of the answer
-        """
-        return await self.chat_service.messages.answer_inline_query(query, answer)
+from typing import Type, TypeVar
+import swibots
+from swibots.api.chat.models import InlineQueryAnswer, InlineQuery
+
+
+class AnswerInlineQuery:
+    async def answer_inline_query(self: "swibots.ApiClient", query: InlineQuery, answer: InlineQueryAnswer) -> bool:
+        """Answer inline query
+
+        Args:
+            query (:obj:`InlineQuery`): Inline query to answer to
+            answer (str | InlineQueryAnswer): Answer to inline query, it can be either a string or an InlineQueryAnswer object, if it's a string, it will be used as the text of the answer
+        """
+        return await self.chat_service.messages.answer_inline_query(query, answer)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/clear_conversation.py` & `swibots-1.2.9/swibots/api/chat/methods/clear_conversation.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message
-
-
-class ClearConversation:
-    async def clear_conversation(self: "swibots.ApiClient", receiver_id: int) -> bool:
-        """Clear a conversation
-
-        Parameters:
-            receiver_id (``int``): The receiver id
-
-        Returns:
-            ``bool``: True if the conversation was cleared
-
-        Raises:
-            ``~switch.error.SwitchError``: If the conversation could not be cleared
-
-        This method does the same as :meth:`~switch.api.chat.controllers.MessageController.clear_conversation`.
-        """
-        return await self.chat_service.messages.clear_conversation(receiver_id)
+from typing import Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message
+
+
+class ClearConversation:
+    async def clear_conversation(self: "swibots.ApiClient", receiver_id: int) -> bool:
+        """Clear a conversation
+
+        Parameters:
+            receiver_id (``int``): The receiver id
+
+        Returns:
+            ``bool``: True if the conversation was cleared
+
+        Raises:
+            ``~switch.error.SwitchError``: If the conversation could not be cleared
+
+        This method does the same as :meth:`~switch.api.chat.controllers.MessageController.clear_conversation`.
+        """
+        return await self.chat_service.messages.clear_conversation(receiver_id)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/delete_message.py` & `swibots-1.2.9/swibots/api/chat/methods/delete_message.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message
-
-
-class DeleteMessage:
-    async def delete_message(self: "swibots.ApiClient", message: int | Message) -> bool:
-        """Delete a message
-
-        Parameters:
-            message (``int`` | ``~switch.api.chat.models.Message``): The message to delete
-
-        Returns:
-            ``bool``: Whether the message was deleted
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be deleted
-
-        This method does the same as :meth:`~switch.api.chat.controllers.MessageController.delete_message`.
-        """
-        return await self.chat_service.messages.delete_message(message)
+from typing import Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message
+
+
+class DeleteMessage:
+    async def delete_message(self: "swibots.ApiClient", message: int | Message) -> bool:
+        """Delete a message
+
+        Parameters:
+            message (``int`` | ``~switch.api.chat.models.Message``): The message to delete
+
+        Returns:
+            ``bool``: Whether the message was deleted
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be deleted
+
+        This method does the same as :meth:`~switch.api.chat.controllers.MessageController.delete_message`.
+        """
+        return await self.chat_service.messages.delete_message(message)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/delete_messages_from_user.py` & `swibots-1.2.9/swibots/api/chat/methods/reply_message_text.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message
-
-
-class DeleteMessagesFromUser:
-    async def delete_messages_from_user(self: "swibots.ApiClient", user_id: int) -> bool:
-        """Delete all messages from a user
-
-        Parameters:
-            user_id (``int``): The user id
-
-        Returns:
-            ``bool``: Whether the messages were deleted
-
-        Raises:
-            ``~switch.error.SwitchError``: If the messages could not be deleted
-
-        This method does the same as :meth:`~switch.api.chat.controllers.MessageController.delete_messages_from_user`.
-        """
-        return await self.chat_service.messages.delete_messages_from_user(user_id)
+from typing import TYPE_CHECKING, Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message, InlineMarkup
+from swibots.api.common.models import MediaUploadRequest
+from swibots.api.common.models import Media
+
+if TYPE_CHECKING:
+    from swibots.api import ApiClient
+
+
+class ReplyMessageText:
+    async def reply_message_text(self: "ApiClient", message: int | Message, text: str, inline_markup: InlineMarkup = None, media: MediaUploadRequest = None, cached_media: Media = None) -> Message:
+        """Send a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to send
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be sent
+
+        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.send_message`.
+        """
+        return await self.chat_service.messages.reply_text(message, text, inline_markup, media, cached_media)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/edit_message.py` & `swibots-1.2.9/swibots/api/chat/methods/edit_message_text.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from typing import TYPE_CHECKING, Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message
-
-if TYPE_CHECKING:
-    from swibots.api import ApiClient
-
-
-class EditMessage:
-    async def edit_message(self: "ApiClient", message: Message) -> Message:
-        """Edit a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message``): The message to edit
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be edited
-
-        This method does the same as :meth:`~switch.api.chat.controllers.MessageController.edit_message`.
-        """
-        return await self.chat_service.messages.edit_message(message)
+from typing import TYPE_CHECKING, Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message, InlineMarkup
+
+if TYPE_CHECKING:
+    from swibots.api import ApiClient
+
+
+class EditMessageText:
+    async def edit_message_text(self: "ApiClient", message: int | Message, text: str, inline_markup: InlineMarkup = None) -> Message:
+        """Send a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to send
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be sent
+
+        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.send_message`.
+        """
+        return await self.chat_service.messages.edit_message_text(message, text, inline_markup)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/edit_message_text.py` & `swibots-1.2.9/swibots/api/chat/methods/send_message.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from typing import TYPE_CHECKING, Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message, InlineMarkup
-
-if TYPE_CHECKING:
-    from swibots.api import ApiClient
-
-
-class EditMessageText:
-    async def edit_message_text(self: "ApiClient", message: int | Message, text: str, inline_markup: InlineMarkup = None) -> Message:
-        """Send a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message``): The message to send
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be sent
-
-        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.send_message`.
-        """
-        return await self.chat_service.messages.edit_message_text(message, text, inline_markup)
+from typing import TYPE_CHECKING, Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message
+from swibots.api.common.models import MediaUploadRequest
+
+if TYPE_CHECKING:
+    from swibots.api import ApiClient
+
+
+class SendMessage:
+    async def send_message(self: "ApiClient", message: Message, media: MediaUploadRequest = None) -> Message:
+        """Send a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to send
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be sent
+
+        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.send_message`.
+        """
+        return await self.chat_service.messages.send_message(message, media)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/flag_message.py` & `swibots-1.2.9/swibots/api/chat/methods/flag_message.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message
-
-
-class FlagMessage:
-    async def flag_message(self: "swibots.ApiClient", message: Message | int) -> bool:
-        """Flag a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message`` | ``int``): The message to flag
-
-        Returns:
-            ``bool``: True if the message was flagged
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be flagged
-
-        This method does the same as :meth:`~switch.api.chat.controllers.MessageController.flag_message`.
-        """
-        return await self.chat_service.messages.flag_message(message)
+from typing import Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message
+
+
+class FlagMessage:
+    async def flag_message(self: "swibots.ApiClient", message: Message | int) -> bool:
+        """Flag a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message`` | ``int``): The message to flag
+
+        Returns:
+            ``bool``: True if the message was flagged
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be flagged
+
+        This method does the same as :meth:`~switch.api.chat.controllers.MessageController.flag_message`.
+        """
+        return await self.chat_service.messages.flag_message(message)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/forward_message.py` & `swibots-1.2.9/swibots/api/chat/methods/forward_message.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message
-from swibots.api.community.models import Group, Channel
-
-
-class ForwardMessage:
-    async def forward_message(
-        self: "swibots.ApiClient",
-        message: Message | int,
-        group_channel: Group | Channel | str = None,
-        receiver_id: str = None
-    ) -> Message:
-        """Forward a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message`` | ``int``): The message to forward
-            group_channel (``~switch.api.community.models.Group`` | ``~switch.api.community.models.Channel`` | ``str``): The group/channel to forward the message to
-            receiver_id (``str``): The receiver id to forward the message to
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The forwarded message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be forwarded
-
-        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.forward_message`.
-        """
-        return await self.chat_service.messages.forward_message(
-            message, group_channel, receiver_id
-        )
+from typing import Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message
+from swibots.api.community.models import Group, Channel
+
+
+class ForwardMessage:
+    async def forward_message(
+        self: "swibots.ApiClient",
+        message: Message | int,
+        group_channel: Group | Channel | str = None,
+        receiver_id: str = None
+    ) -> Message:
+        """Forward a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message`` | ``int``): The message to forward
+            group_channel (``~switch.api.community.models.Group`` | ``~switch.api.community.models.Channel`` | ``str``): The group/channel to forward the message to
+            receiver_id (``str``): The receiver id to forward the message to
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The forwarded message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be forwarded
+
+        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.forward_message`.
+        """
+        return await self.chat_service.messages.forward_message(
+            message, group_channel, receiver_id
+        )
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/get_channel_chat_history.py` & `swibots-1.2.9/swibots/api/chat/methods/get_group_chat_history.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-from typing import List
-import swibots
-from swibots.api.chat.models import GroupChatHistory
-
-
-class GetChannelChatHistory:
-    async def get_channel_chat_history(
-        self: "swibots.ApiClient",
-        channel_id: str,
-        community_id: str,
-        user_id: int = None,
-        page_limit: int = 100,
-        page_offset=0,
-    ) -> GroupChatHistory:
-        """Get channel chat history
-
-
-        Parameters:
-            channel_id (``int``): The channel id
-            limit (``int``, *optional*): The maximum number of messages to return. Defaults to 100.
-            offset (``int``, *optional*): The offset. Defaults to 0.
-            community_id (``int``): The community id
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-
-        Returns:
-            ``List[~switch.api.chat.models.GroupChatHistory]``: The messages
-
-        Raises:
-            ``~switch.error.SwitchError``: If the messages could not be retrieved
-        """
-        return await self.chat_service.messages.get_channel_chat_history(
-            channel_id, community_id, user_id, page_limit, page_offset
-        )
+from typing import List
+import swibots
+from swibots.api.chat.models import GroupChatHistory
+
+
+class GetGroupChatHistory:
+    async def get_group_chat_history(
+        self: "swibots.ApiClient",
+        group_id: str,
+        community_id: str,
+        user_id: int = None,
+        page_limit: int = 100,
+        page_offset=0,
+    ) -> GroupChatHistory:
+        """Get group chat history
+
+        Parameters:
+            group_id (``int``): The group id
+            limit (``int``, *optional*): The maximum number of messages to return. Defaults to 100.
+            offset (``int``, *optional*): The offset. Defaults to 0.
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The messages
+
+        Raises:
+            ``~switch.error.SwitchError``: If the messages could not be retrieved
+
+        This function does the same as :meth:`~switch.api.chat.controllers.MessageController.get_group_chat_history`.
+        """
+        return await self.chat_service.messages.get_group_chat_history(
+            group_id, community_id, user_id, page_limit, page_offset
+        )
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/get_community_media_files.py` & `swibots-1.2.9/swibots/api/chat/methods/get_community_media_files_by_status.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from typing import List
-import swibots
-from swibots.api.chat.models import Message
-
-
-class GetCommunityMediaFiles:
-    async def get_community_media_files(
-        self: "swibots.ApiClient", community_id: str
-    ) -> List[Message]:
-        """Get community media files
-
-        Parameters:
-            community_id (``int``): The community id
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The messages
-
-        Raises:
-            ``~switch.error.SwitchError``: If the messages could not be retrieved
-
-        This function does the same as :meth:`~switch.api.chat.controllers.MessageController.get_messages`.
-        """
-        return await self.chat_service.messages.get_messages(community_id)
+from typing import List
+import swibots
+from swibots.api.chat.models import Message
+
+
+class GetCommunityMediaFilesByStatus:
+    async def get_community_media_files_by_status(
+        self: "swibots.ApiClient", community_id: str, status: str
+    ) -> List[Message]:
+        """Get community media files by status
+
+        Parameters:
+            community_id (``int``): The community id
+            status (``str``): The status
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The messages
+
+        Raises:
+            ``~switch.error.SwitchError``: If the messages could not be retrieved
+
+        This function does the same as :meth:`~switch.api.chat.controllers.MessageController.get_community_media_files_by_status`.
+        """
+        return await self.chat_service.messages.get_community_media_files_by_status(
+            community_id, status
+        )
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/get_flag_messages.py` & `swibots-1.2.9/swibots/api/chat/methods/get_user_media_files.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from typing import List
-import swibots
-from swibots.api.chat.models import Message
-
-
-class GetFlagMessages:
-    async def get_flag_messages(self: "swibots.ApiClient", user_id: int = None) -> List[Message]:
-        """Get flagged messages
-
-        Parameters:
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The flagged messages
-
-        Raises:
-            ``~switch.error.SwitchError``: If the flagged messages could not be retrieved
-        """
-        return await self.chat_service.messages.get_flag_messages(user_id)
+from typing import List
+import swibots
+from swibots.api.chat.models import Message
+
+
+class GetUserMediaFiles:
+    async def get_user_media_files(
+        self: "swibots.ApiClient",
+        user_id: int = None,
+    ) -> List[Message]:
+        """Get user media files
+
+
+        Parameters:
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The user media files
+
+        Raises:
+            ``~switch.error.SwitchError``: If the user media files could not be retrieved
+
+        This function does the same as :meth:`~switch.api.chat.controllers.MessageController.get_user_media_files`.
+        """
+        return await self.chat_service.messages.get_user_media_files(user_id)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/get_messages.py` & `swibots-1.2.9/swibots/api/chat/methods/get_messages.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from typing import List
-import swibots
-from swibots.api.chat.models import Message
-
-
-class GetMessages:
-    async def get_messages(self: "swibots.ApiClient", user_id: int = None) -> List[Message]:
-        """Get messages
-
-        Parameters:
-            user_id (``int``, *optional*): The user id. Defaults to the current user id.
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The messages
-
-        Raises:
-            ``~switch.error.SwitchError``: If the messages could not be retrieved
-
-        This function does the same as :meth:`~switch.api.chat.controllers.MessageController.get_messages`.
-        """
-        return await self.chat_service.messages.get_messages(user_id)
+from typing import List
+import swibots
+from swibots.api.chat.models import Message
+
+
+class GetMessages:
+    async def get_messages(self: "swibots.ApiClient", user_id: int = None) -> List[Message]:
+        """Get messages
+
+        Parameters:
+            user_id (``int``, *optional*): The user id. Defaults to the current user id.
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The messages
+
+        Raises:
+            ``~switch.error.SwitchError``: If the messages could not be retrieved
+
+        This function does the same as :meth:`~switch.api.chat.controllers.MessageController.get_messages`.
+        """
+        return await self.chat_service.messages.get_messages(user_id)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/get_messages_between_users.py` & `swibots-1.2.9/swibots/api/chat/methods/get_messages_between_users.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from typing import List
-import swibots
-from swibots.api.chat.models import Message
-
-
-class GetMessagesBetweenUsers:
-    async def get_messages_between_users(
-        self: "swibots.ApiClient",
-        user_id: int,
-        other_user_id: int,
-        limit: int = 100,
-        offset: int = 0,
-    ) -> List[Message]:
-        """Get messages between users
-
-        Parameters:
-            user_id (``int``): The user id
-            other_user_id (``int``): The other user id
-            limit (``int``, *optional*): The maximum number of messages to retrieve. Defaults to 100.
-            offset (``int``, *optional*): The offset. Defaults to 0.
-
-        Returns:
-            ``List[~switch.api.chat.models.Message]``: The messages
-
-        Raises:
-            ``~switch.error.SwitchError``: If the messages could not be retrieved
-
-        This function does the same as :meth:`~switch.api.chat.controllers.MessageController.get_messages_between_users`.
-        """
-        return await self.chat_service.messages.get_messages_between_users(
-            user_id, other_user_id, limit, offset
-        )
+from typing import List
+import swibots
+from swibots.api.chat.models import Message
+
+
+class GetMessagesBetweenUsers:
+    async def get_messages_between_users(
+        self: "swibots.ApiClient",
+        user_id: int,
+        other_user_id: int,
+        limit: int = 100,
+        offset: int = 0,
+    ) -> List[Message]:
+        """Get messages between users
+
+        Parameters:
+            user_id (``int``): The user id
+            other_user_id (``int``): The other user id
+            limit (``int``, *optional*): The maximum number of messages to retrieve. Defaults to 100.
+            offset (``int``, *optional*): The offset. Defaults to 0.
+
+        Returns:
+            ``List[~switch.api.chat.models.Message]``: The messages
+
+        Raises:
+            ``~switch.error.SwitchError``: If the messages could not be retrieved
+
+        This function does the same as :meth:`~switch.api.chat.controllers.MessageController.get_messages_between_users`.
+        """
+        return await self.chat_service.messages.get_messages_between_users(
+            user_id, other_user_id, limit, offset
+        )
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/reply_message.py` & `swibots-1.2.9/swibots/api/chat/methods/reply_message.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import TYPE_CHECKING, Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message
-from swibots.api.common.models import MediaUploadRequest
-
-if TYPE_CHECKING:
-    from swibots.api import ApiClient
-
-
-class ReplyMessage:
-    async def reply_message(self: "swibots.ApiClient", message: int | Message, reply: Message, media: MediaUploadRequest = None) -> Message:
-        """Send a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message``): The message to send
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be sent
-
-        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.send_message`.
-        """
-        return await self.chat_service.messages.reply(message, reply, media)
+from typing import TYPE_CHECKING, Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message
+from swibots.api.common.models import MediaUploadRequest
+
+if TYPE_CHECKING:
+    from swibots.api import ApiClient
+
+
+class ReplyMessage:
+    async def reply_message(self: "swibots.ApiClient", message: int | Message, reply: Message, media: MediaUploadRequest = None) -> Message:
+        """Send a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to send
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be sent
+
+        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.send_message`.
+        """
+        return await self.chat_service.messages.reply(message, reply, media)
```

### Comparing `swibots-1.2.8/swibots/api/chat/methods/reply_message_text.py` & `swibots-1.2.9/swibots/api/chat/methods/send_text.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from typing import TYPE_CHECKING, Type, TypeVar
-import swibots
-from swibots.api.chat.models import Message, InlineMarkup
-from swibots.api.common.models import MediaUploadRequest
-from swibots.api.common.models import Media
-
-if TYPE_CHECKING:
-    from swibots.api import ApiClient
-
-
-class ReplyMessageText:
-    async def reply_message_text(self: "ApiClient", message: int | Message, text: str, inline_markup: InlineMarkup = None, media: MediaUploadRequest = None, cached_media: Media = None) -> Message:
-        """Send a message
-
-        Parameters:
-            message (``~switch.api.chat.models.Message``): The message to send
-
-        Returns:
-            ``~switch.api.chat.models.Message``: The message
-
-        Raises:
-            ``~switch.error.SwitchError``: If the message could not be sent
-
-        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.send_message`.
-        """
-        return await self.chat_service.messages.reply_text(message, text, inline_markup, media, cached_media)
+from typing import TYPE_CHECKING, Optional, Type, TypeVar
+import swibots
+from swibots.api.chat.models import Message, InlineMarkup
+from swibots.api.community.models import Channel, Group
+from swibots.api.common.models import User
+from swibots.api.common.models import MediaUploadRequest
+
+if TYPE_CHECKING:
+    from swibots.api import ApiClient
+
+
+class SendText:
+    async def send_text(self: "ApiClient", text: str, to: Optional[int | User] = None, channel: Optional[Channel | str] = None, group: Optional[Group | str] = None,  inline_markup: InlineMarkup = None, media: MediaUploadRequest = None) -> Message:
+        """Send a message
+
+        Parameters:
+            message (``~switch.api.chat.models.Message``): The message to send
+
+        Returns:
+            ``~switch.api.chat.models.Message``: The message
+
+        Raises:
+            ``~switch.error.SwitchError``: If the message could not be sent
+
+        This functions does the same as :meth:`~switch.api.chat.controllers.MessageController.send_message`.
+        """
+        return await self.chat_service.messages.send_text(text, to, channel, group, inline_markup, media)
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/group_chat_history.py` & `swibots-1.2.9/swibots/api/chat/models/group_chat_history.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from swibots.base import SwitchObject
-from typing import List
-
-from .message import Message
-from swibots.api.common.models.user import User
-import swibots
-
-
-class GroupChatHistory(SwitchObject):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        users: List[User] = None,
-        messages: List[Message] = None,
-    ):
-        super().__init__(app)
-        self.users = users or []
-        self.messages = messages or []
-
-    def from_json(self, data: dict) -> "GroupChatHistory":
-        self.users = User.build_from_json_list(
-            data.get("userInfo", []), self.app)
-        self.messages = Message.build_from_json_list(
-            data.get("message", []),  self.app)
-        return self
-
-    def to_json(self) -> dict:
-        return {
-            "userInfo": [user.to_json() for user in self.users],
-            "message": [message.to_json() for message in self.messages],
-        }
+from swibots.base import SwitchObject
+from typing import List
+
+from .message import Message
+from swibots.api.common.models.user import User
+import swibots
+
+
+class GroupChatHistory(SwitchObject):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        users: List[User] = None,
+        messages: List[Message] = None,
+    ):
+        super().__init__(app)
+        self.users = users or []
+        self.messages = messages or []
+
+    def from_json(self, data: dict) -> "GroupChatHistory":
+        self.users = User.build_from_json_list(
+            data.get("userInfo", []), self.app)
+        self.messages = Message.build_from_json_list(
+            data.get("message", []),  self.app)
+        return self
+
+    def to_json(self) -> dict:
+        return {
+            "userInfo": [user.to_json() for user in self.users],
+            "message": [message.to_json() for message in self.messages],
+        }
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline/__init__.py` & `swibots-1.2.9/swibots/api/chat/models/inline/__init__.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .inline_query import InlineQuery
-from .inline_query_answer import InlineQueryAnswer
-from .inline_query_result import InlineQueryResult
-from .types import InlineQueryResultType
-from .base_typed_inline_query_result import BaseTypedInlineQueryResult
-from .inline_query_result_article import InlineQueryResultArticle
-from .inline_query_result_photo import InlineQueryResultPhoto
-from .inline_query_result_document import InlineQueryResultDocument
-from .inline_query_result_video import InlineQueryResultVideo
-from .input_message_content import InputMessageContent
+from .inline_query import InlineQuery
+from .inline_query_answer import InlineQueryAnswer
+from .inline_query_result import InlineQueryResult
+from .types import InlineQueryResultType
+from .base_typed_inline_query_result import BaseTypedInlineQueryResult
+from .inline_query_result_article import InlineQueryResultArticle
+from .inline_query_result_photo import InlineQueryResultPhoto
+from .inline_query_result_document import InlineQueryResultDocument
+from .inline_query_result_video import InlineQueryResultVideo
+from .input_message_content import InputMessageContent
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline/base_typed_inline_query_result.py` & `swibots-1.2.9/swibots/api/chat/models/inline/base_typed_inline_query_result.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from .types import InlineQueryResultType
-import swibots
-from swibots.utils.types import JSONDict
-from swibots.base import SwitchObject
-from .input_message_content import InputMessageContent
-from ..inline_markup import InlineMarkup
-from .inline_query_result import InlineQueryResult
-
-
-class BaseTypedInlineQueryResult(InlineQueryResult):
-    def __init__(self,
-                 id: str,
-                 type: InlineQueryResultType,
-                 title: str = None,
-                 description: str = None,
-                 thumb_url: str = None,
-                 thumb_width: int = None,
-                 thumb_height: int = None,
-                 input_message: "InputMessageContent" = None,
-                 reply_markup: "InlineMarkup" = None,
-                 ):
-        super().__init__(id, type, input_message, reply_markup)
-        self.type = type
-        self.title = title
-        self.description = description
-        self.thumb_url = thumb_url
-        self.thumb_width = thumb_width
-        self.thumb_height = thumb_height
-
-    def to_json(self) -> JSONDict:
-        data = super().to_json()
-        data.update({
-            "title": self.title,
-            "description": self.description,
-            "thumbUrl": self.thumb_url,
-            "thumbWidth": self.thumb_width,
-            "thumbHeight": self.thumb_height,
-        })
-        return data
+from .types import InlineQueryResultType
+import swibots
+from swibots.utils.types import JSONDict
+from swibots.base import SwitchObject
+from .input_message_content import InputMessageContent
+from ..inline_markup import InlineMarkup
+from .inline_query_result import InlineQueryResult
+
+
+class BaseTypedInlineQueryResult(InlineQueryResult):
+    def __init__(self,
+                 id: str,
+                 type: InlineQueryResultType,
+                 title: str = None,
+                 description: str = None,
+                 thumb_url: str = None,
+                 thumb_width: int = None,
+                 thumb_height: int = None,
+                 input_message: "InputMessageContent" = None,
+                 reply_markup: "InlineMarkup" = None,
+                 ):
+        super().__init__(id, type, input_message, reply_markup)
+        self.type = type
+        self.title = title
+        self.description = description
+        self.thumb_url = thumb_url
+        self.thumb_width = thumb_width
+        self.thumb_height = thumb_height
+
+    def to_json(self) -> JSONDict:
+        data = super().to_json()
+        data.update({
+            "title": self.title,
+            "description": self.description,
+            "thumbUrl": self.thumb_url,
+            "thumbWidth": self.thumb_width,
+            "thumbHeight": self.thumb_height,
+        })
+        return data
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline/inline_query.py` & `swibots-1.2.9/swibots/api/chat/models/inline/inline_query.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from typing import List, Optional
-import swibots
-from swibots.base import SwitchObject
-from swibots.api.common import User
-from swibots.api.community import Community, Channel, Group
-from .inline_query_answer import InlineQueryAnswer
-
-from swibots.utils.types import JSONDict
-
-
-class InlineQuery(SwitchObject):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        user_id: int = None,
-        user: "User" = None,
-        # receiver_id: int = None,
-        # receiver: "User" = None,
-        community_id: int = None,
-        community: "Community" = None,
-        group_id: int = None,
-        group: "Group" = None,
-        channel_id: int = None,
-        channel: "Channel" = None,
-        query_id: Optional[str] = None,
-        offset: Optional[str] = None,
-        query: Optional[str] = None,
-    ):
-        super().__init__(app)
-        self.user_id = user_id
-        self.user = user
-        # self.receiver_id = receiver_id
-        # self.receiver = receiver
-        self.community_id = community_id
-        self.community = community
-        self.group_id = group_id
-        self.group = group
-        self.channel_id = channel_id
-        self.channel = channel
-        self.query_id = query_id
-        self.offset = offset
-        self.query = query
-
-    def to_json(self) -> JSONDict:
-        return {
-            "text": self.text,
-            "url": self.url,
-            "callbackData": self.callback_data,
-        }
-
-    def from_json(self, data: JSONDict) -> "InlineQuery":
-        if data is not None:
-            self.user_id = data.get("userId")
-            self.user = User.build_from_json(data.get("user"), self.app)
-            # self.receiver_id = data.get("receiverId")
-            # self.receiver = User.build_from_json(
-            #     data.get("receiver"), self.app)
-            self.community_id = data.get("communityId")
-            self.community = Community.build_from_json(
-                data.get("community"), self.app)
-            self.group_id = data.get("groupId")
-            self.group = Group.build_from_json(data.get("group"), self.app)
-            self.channel_id = data.get("channelId")
-            self.channel = Channel.build_from_json(
-                data.get("channel"), self.app)
-            self.query_id = data.get("id")
-            self.offset = data.get("offset")
-            self.query = data.get("query")
-        return self
-
-    async def answer(self, response: "InlineQueryAnswer"):
-        return await self.app.answer_inline_query(self, response)
+from typing import List, Optional
+import swibots
+from swibots.base import SwitchObject
+from swibots.api.common import User
+from swibots.api.community import Community, Channel, Group
+from .inline_query_answer import InlineQueryAnswer
+
+from swibots.utils.types import JSONDict
+
+
+class InlineQuery(SwitchObject):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        user_id: int = None,
+        user: "User" = None,
+        # receiver_id: int = None,
+        # receiver: "User" = None,
+        community_id: int = None,
+        community: "Community" = None,
+        group_id: int = None,
+        group: "Group" = None,
+        channel_id: int = None,
+        channel: "Channel" = None,
+        query_id: Optional[str] = None,
+        offset: Optional[str] = None,
+        query: Optional[str] = None,
+    ):
+        super().__init__(app)
+        self.user_id = user_id
+        self.user = user
+        # self.receiver_id = receiver_id
+        # self.receiver = receiver
+        self.community_id = community_id
+        self.community = community
+        self.group_id = group_id
+        self.group = group
+        self.channel_id = channel_id
+        self.channel = channel
+        self.query_id = query_id
+        self.offset = offset
+        self.query = query
+
+    def to_json(self) -> JSONDict:
+        return {
+            "text": self.text,
+            "url": self.url,
+            "callbackData": self.callback_data,
+        }
+
+    def from_json(self, data: JSONDict) -> "InlineQuery":
+        if data is not None:
+            self.user_id = data.get("userId")
+            self.user = User.build_from_json(data.get("user"), self.app)
+            # self.receiver_id = data.get("receiverId")
+            # self.receiver = User.build_from_json(
+            #     data.get("receiver"), self.app)
+            self.community_id = data.get("communityId")
+            self.community = Community.build_from_json(
+                data.get("community"), self.app)
+            self.group_id = data.get("groupId")
+            self.group = Group.build_from_json(data.get("group"), self.app)
+            self.channel_id = data.get("channelId")
+            self.channel = Channel.build_from_json(
+                data.get("channel"), self.app)
+            self.query_id = data.get("id")
+            self.offset = data.get("offset")
+            self.query = data.get("query")
+        return self
+
+    async def answer(self, response: "InlineQueryAnswer"):
+        return await self.app.answer_inline_query(self, response)
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline/inline_query_answer.py` & `swibots-1.2.9/swibots/api/chat/models/inline/inline_query_answer.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from typing import Any, List, Optional
-import swibots
-from swibots.base import SwitchObject
-
-from swibots.utils.types import JSONDict, SCT
-from .inline_query_result import InlineQueryResult
-
-
-class InlineQueryAnswer(SwitchObject):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        query_id: Optional[str] = None,
-        user_id: int = None,
-        title: Optional[str] = None,
-        results: List["InlineQueryResult"] = None,
-        next_offset: Optional[str] = None,
-        cache_time: int = None,
-        is_personal: bool = True,
-        pm_text: Optional[str] = None,
-        pm_parameter: Optional[str] = None,
-    ):
-        super().__init__(app)
-        self.query_id = query_id
-        self.user_id = user_id
-        self.title = title
-        self.results = results
-        self.next_offset = next_offset
-        self.cache_time = cache_time
-        self.is_personal = is_personal
-        self.pm_text = pm_text
-        self.pm_parameter = pm_parameter
-
-    def to_json(self) -> JSONDict:
-        return {
-            "queryId": self.query_id,
-            "userId": self.user_id,
-            "title": self.title,
-            "results":   [self._result_json(result) for result in self.results or []],
-            "nextOffset": self.next_offset,
-            "cacheTime": self.cache_time,
-            "isPersonal": self.is_personal,
-            "pmText": self.pm_text,
-            "pmParameter": self.pm_parameter,
-        }
-
-    def _result_json(self, result):
-        if isinstance(result, dict):
-            return result
-        else:
-            return result.to_json()
-
-    def add_result(self, result: SCT[Any]) -> "InlineQueryAnswer":
-        if not self.results:
-            self.results = []
-
-        if isinstance(result, List):
-            self.results.extend(result)
-        else:
-            self.results.append(result)
+from typing import Any, List, Optional
+import swibots
+from swibots.base import SwitchObject
+
+from swibots.utils.types import JSONDict, SCT
+from .inline_query_result import InlineQueryResult
+
+
+class InlineQueryAnswer(SwitchObject):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        query_id: Optional[str] = None,
+        user_id: int = None,
+        title: Optional[str] = None,
+        results: List["InlineQueryResult"] = None,
+        next_offset: Optional[str] = None,
+        cache_time: int = None,
+        is_personal: bool = True,
+        pm_text: Optional[str] = None,
+        pm_parameter: Optional[str] = None,
+    ):
+        super().__init__(app)
+        self.query_id = query_id
+        self.user_id = user_id
+        self.title = title
+        self.results = results
+        self.next_offset = next_offset
+        self.cache_time = cache_time
+        self.is_personal = is_personal
+        self.pm_text = pm_text
+        self.pm_parameter = pm_parameter
+
+    def to_json(self) -> JSONDict:
+        return {
+            "queryId": self.query_id,
+            "userId": self.user_id,
+            "title": self.title,
+            "results":   [self._result_json(result) for result in self.results or []],
+            "nextOffset": self.next_offset,
+            "cacheTime": self.cache_time,
+            "isPersonal": self.is_personal,
+            "pmText": self.pm_text,
+            "pmParameter": self.pm_parameter,
+        }
+
+    def _result_json(self, result):
+        if isinstance(result, dict):
+            return result
+        else:
+            return result.to_json()
+
+    def add_result(self, result: SCT[Any]) -> "InlineQueryAnswer":
+        if not self.results:
+            self.results = []
+
+        if isinstance(result, List):
+            self.results.extend(result)
+        else:
+            self.results.append(result)
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result.py` & `swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result_document.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-from .types import InlineQueryResultType
-import swibots
-from swibots.base import SwitchObject
-from swibots.utils.types import JSONDict
-from .input_message_content import InputMessageContent
-from ..inline_markup import InlineMarkup
-
-
-class InlineQueryResult(SwitchObject):
-    def __init__(self,
-                 id: str,
-                 type: InlineQueryResultType,
-                 input_message: "InputMessageContent" = None,
-                 reply_markup: "InlineMarkup" = None,
-                 ):
-        self.id = id
-        self.type = type
-        self.input_message = input_message
-        self.reply_markup = reply_markup
-
-    def to_json(self) -> JSONDict:
-        data = {
-            "id": self.id,
-            "type": self.type.value,
-        }
-        if self.input_message is not None:
-            data["inputMessage"] = self.input_message.to_json()
-        if self.reply_markup is not None:
-            data["replyMarkup"] = self.reply_markup.to_json()
-        return data
+import swibots
+from swibots.utils.types import JSONDict
+from swibots.base import SwitchObject
+
+from .base_typed_inline_query_result import BaseTypedInlineQueryResult
+from .input_message_content import InputMessageContent
+from ..inline_markup import InlineMarkup
+from .types import InlineQueryResultType
+
+
+class InlineQueryResultDocument(BaseTypedInlineQueryResult):
+    def __init__(self,
+                 id: str,
+                 title: str,
+                 document_url: str,
+                 mime_type: str,
+                 input_message: "InputMessageContent" = None,
+                 description: str = None,
+                 thumb_url: str = None,
+                 thumb_width: int = None,
+                 thumb_height: int = None,
+                 reply_markup: "InlineMarkup" = None,
+                 ):
+        super().__init__(id, InlineQueryResultType.DOCUMENT, title, description, thumb_url, thumb_width, thumb_height,
+                         input_message, reply_markup)
+        self.document_url = document_url
+        self.mime_type = mime_type
+
+    def to_json(self) -> JSONDict:
+        data = super().to_json()
+        data.update({
+            "documentUrl": self.document_url,
+            "mimeType": self.mime_type,
+        })
+        return data
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result_article.py` & `swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result_article.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import swibots
-from swibots.utils.types import JSONDict
-from swibots.base import SwitchObject
-
-from .base_typed_inline_query_result import BaseTypedInlineQueryResult
-from .input_message_content import InputMessageContent
-from ..inline_markup import InlineMarkup
-from .types import InlineQueryResultType
-
-
-class InlineQueryResultArticle(BaseTypedInlineQueryResult):
-    def __init__(self,
-                 id: str,
-                 title: str,
-                 article_url: str,
-                 input_message: "InputMessageContent" = None,
-                 description: str = None,
-                 thumb_url: str = None,
-                 thumb_width: int = None,
-                 thumb_height: int = None,
-                 reply_markup: "InlineMarkup" = None,
-                 ):
-        super().__init__(id, InlineQueryResultType.ARTICLE, title, description, thumb_url, thumb_width, thumb_height,
-                         input_message, reply_markup)
-        self.article_url = article_url
-
-    def to_json(self) -> JSONDict:
-        data = super().to_json()
-        data.update({
-            "articleUrl": self.article_url,
-        })
-        return data
+import swibots
+from swibots.utils.types import JSONDict
+from swibots.base import SwitchObject
+
+from .base_typed_inline_query_result import BaseTypedInlineQueryResult
+from .input_message_content import InputMessageContent
+from ..inline_markup import InlineMarkup
+from .types import InlineQueryResultType
+
+
+class InlineQueryResultArticle(BaseTypedInlineQueryResult):
+    def __init__(self,
+                 id: str,
+                 title: str,
+                 article_url: str,
+                 input_message: "InputMessageContent" = None,
+                 description: str = None,
+                 thumb_url: str = None,
+                 thumb_width: int = None,
+                 thumb_height: int = None,
+                 reply_markup: "InlineMarkup" = None,
+                 ):
+        super().__init__(id, InlineQueryResultType.ARTICLE, title, description, thumb_url, thumb_width, thumb_height,
+                         input_message, reply_markup)
+        self.article_url = article_url
+
+    def to_json(self) -> JSONDict:
+        data = super().to_json()
+        data.update({
+            "articleUrl": self.article_url,
+        })
+        return data
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result_document.py` & `swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result_video.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,47 @@
-import swibots
-from swibots.utils.types import JSONDict
-from swibots.base import SwitchObject
-
-from .base_typed_inline_query_result import BaseTypedInlineQueryResult
-from .input_message_content import InputMessageContent
-from ..inline_markup import InlineMarkup
-from .types import InlineQueryResultType
-
-
-class InlineQueryResultDocument(BaseTypedInlineQueryResult):
-    def __init__(self,
-                 id: str,
-                 title: str,
-                 document_url: str,
-                 mime_type: str,
-                 input_message: "InputMessageContent" = None,
-                 description: str = None,
-                 thumb_url: str = None,
-                 thumb_width: int = None,
-                 thumb_height: int = None,
-                 reply_markup: "InlineMarkup" = None,
-                 ):
-        super().__init__(id, InlineQueryResultType.DOCUMENT, title, description, thumb_url, thumb_width, thumb_height,
-                         input_message, reply_markup)
-        self.document_url = document_url
-        self.mime_type = mime_type
-
-    def to_json(self) -> JSONDict:
-        data = super().to_json()
-        data.update({
-            "documentUrl": self.document_url,
-            "mimeType": self.mime_type,
-        })
-        return data
+import swibots
+from swibots.utils.types import JSONDict
+from swibots.base import SwitchObject
+
+from .base_typed_inline_query_result import BaseTypedInlineQueryResult
+from .input_message_content import InputMessageContent
+from ..inline_markup import InlineMarkup
+from .types import InlineQueryResultType
+
+
+class InlineQueryResultVideo(BaseTypedInlineQueryResult):
+    def __init__(self,
+                 id: str,
+                 title: str,
+                 video_url: str,
+                 mime_type: str = None,
+                 video_width: int = None,
+                 video_height: int = None,
+                 video_duration: int = None,
+                 caption: str = None,
+                 input_message: "InputMessageContent" = None,
+                 description: str = None,
+                 thumb_url: str = None,
+                 thumb_width: int = None,
+                 thumb_height: int = None,
+                 reply_markup: "InlineMarkup" = None,
+                 ):
+        super().__init__(id, InlineQueryResultType.VIDEO, title, description, thumb_url, thumb_width, thumb_height,
+                         input_message, reply_markup)
+        self.video_url = video_url
+        self.video_width = video_width
+        self.video_height = video_height
+        self.video_duration = video_duration
+        self.caption = caption
+        self.mime_type = mime_type
+
+    def to_json(self) -> JSONDict:
+        data = super().to_json()
+        data.update({
+            "videoUrl": self.video_url,
+            "videoWidth": self.video_width,
+            "videoHeight": self.video_height,
+            "videoDuration": self.video_duration,
+            "caption": self.caption,
+            "mimeType": self.mime_type,
+        })
+        return data
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline/inline_query_result_photo.py` & `swibots-1.2.9/swibots/api/chat/models/inline/inline_query_result_photo.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import swibots
-from swibots.utils.types import JSONDict
-from swibots.base import SwitchObject
-
-from .base_typed_inline_query_result import BaseTypedInlineQueryResult
-from .input_message_content import InputMessageContent
-from ..inline_markup import InlineMarkup
-from .types import InlineQueryResultType
-
-
-class InlineQueryResultPhoto(BaseTypedInlineQueryResult):
-    def __init__(self,
-                 id: str,
-                 title: str,
-                 photo_url: str,
-                 mime_type: str = None,
-                 photo_width: int = None,
-                 photo_height: int = None,
-                 caption: str = None,
-                 input_message: "InputMessageContent" = None,
-                 description: str = None,
-                 thumb_url: str = None,
-                 thumb_width: int = None,
-                 thumb_height: int = None,
-                 reply_markup: "InlineMarkup" = None,
-                 ):
-        super().__init__(id, InlineQueryResultType.PHOTO, title, description, thumb_url, thumb_width, thumb_height,
-                         input_message, reply_markup)
-        self.photo_url = photo_url
-        self.photo_width = photo_width
-        self.photo_height = photo_height
-        self.caption = caption
-        self.mime_type = mime_type
-
-    def to_json(self) -> JSONDict:
-        data = super().to_json()
-        data.update({
-            "photoUrl": self.photo_url,
-            "photoWidth": self.photo_width,
-            "photoHeight": self.photo_height,
-            "caption": self.caption,
-            "mimeType": self.mime_type,
-        })
-        return data
+import swibots
+from swibots.utils.types import JSONDict
+from swibots.base import SwitchObject
+
+from .base_typed_inline_query_result import BaseTypedInlineQueryResult
+from .input_message_content import InputMessageContent
+from ..inline_markup import InlineMarkup
+from .types import InlineQueryResultType
+
+
+class InlineQueryResultPhoto(BaseTypedInlineQueryResult):
+    def __init__(self,
+                 id: str,
+                 title: str,
+                 photo_url: str,
+                 mime_type: str = None,
+                 photo_width: int = None,
+                 photo_height: int = None,
+                 caption: str = None,
+                 input_message: "InputMessageContent" = None,
+                 description: str = None,
+                 thumb_url: str = None,
+                 thumb_width: int = None,
+                 thumb_height: int = None,
+                 reply_markup: "InlineMarkup" = None,
+                 ):
+        super().__init__(id, InlineQueryResultType.PHOTO, title, description, thumb_url, thumb_width, thumb_height,
+                         input_message, reply_markup)
+        self.photo_url = photo_url
+        self.photo_width = photo_width
+        self.photo_height = photo_height
+        self.caption = caption
+        self.mime_type = mime_type
+
+    def to_json(self) -> JSONDict:
+        data = super().to_json()
+        data.update({
+            "photoUrl": self.photo_url,
+            "photoWidth": self.photo_width,
+            "photoHeight": self.photo_height,
+            "caption": self.caption,
+            "mimeType": self.mime_type,
+        })
+        return data
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/inline_markup.py` & `swibots-1.2.9/swibots/api/chat/models/inline_markup.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from typing import TYPE_CHECKING, List, Optional
-import swibots
-from .inline_keyboard_color import InlineKeyboardColor
-from .inline_keyboard_size import InlineKeyboardSize
-from .inline_keyboard_button import InlineKeyboardButton
-from swibots.base import SwitchObject
-
-from swibots.utils.types import JSONDict
-
-if TYPE_CHECKING:
-    from .inline_keyboard_button import InlineKeyboardButton
-
-
-class InlineMarkup(SwitchObject):
-    def __init__(
-        self,
-        inline_keyboard: List[List["InlineKeyboardButton"]] = None,
-        color: Optional[InlineKeyboardColor] = InlineKeyboardColor.RANDOM,
-        size: Optional[InlineKeyboardSize] = InlineKeyboardSize.DEFAULT,
-    ):
-        super().__init__()
-        self._inline_keyboard = inline_keyboard
-        self._color = color or InlineKeyboardColor.RANDOM
-        self._size = size or InlineKeyboardSize.DEFAULT
-
-    @property
-    def inline_keyboard(self) -> List[List["InlineKeyboardButton"]]:
-        if self._inline_keyboard is None:
-            self._inline_keyboard = []
-        return self._inline_keyboard
-
-    def add_row(self, buttons: List["InlineKeyboardButton"]):
-        if len(buttons) > 0:
-            self.inline_keyboard.append(list(buttons))
-
-    def to_json(self) -> JSONDict:
-        if self._inline_keyboard is None:
-            return None
-        return {
-            "inlineKeyboard": [[x.to_json() for x in row] for row in self._inline_keyboard],
-            "color": self._color.value,
-            "size": self._size.value,
-        }
-
-    def from_json(self, data: JSONDict) -> "InlineMarkup":
-        if data is None or data.get("inlineKeyboard") is None:
-            return None
-        self._color = InlineKeyboardColor(data.get("color") or "RANDOM")
-        self._size = InlineKeyboardSize(data.get("size") or "DEFAULT")
-        self._inline_keyboard = (
-            [
-                [InlineKeyboardButton.build_from_json(
-                    x, self.app) for x in row]
-                for row in data.get("inlineKeyboard") or []
-            ],
-        )
-
-        return self
+from typing import TYPE_CHECKING, List, Optional
+import swibots
+from .inline_keyboard_color import InlineKeyboardColor
+from .inline_keyboard_size import InlineKeyboardSize
+from .inline_keyboard_button import InlineKeyboardButton
+from swibots.base import SwitchObject
+
+from swibots.utils.types import JSONDict
+
+if TYPE_CHECKING:
+    from .inline_keyboard_button import InlineKeyboardButton
+
+
+class InlineMarkup(SwitchObject):
+    def __init__(
+        self,
+        inline_keyboard: List[List["InlineKeyboardButton"]] = None,
+        color: Optional[InlineKeyboardColor] = InlineKeyboardColor.RANDOM,
+        size: Optional[InlineKeyboardSize] = InlineKeyboardSize.DEFAULT,
+    ):
+        super().__init__()
+        self._inline_keyboard = inline_keyboard
+        self._color = color or InlineKeyboardColor.RANDOM
+        self._size = size or InlineKeyboardSize.DEFAULT
+
+    @property
+    def inline_keyboard(self) -> List[List["InlineKeyboardButton"]]:
+        if self._inline_keyboard is None:
+            self._inline_keyboard = []
+        return self._inline_keyboard
+
+    def add_row(self, buttons: List["InlineKeyboardButton"]):
+        if len(buttons) > 0:
+            self.inline_keyboard.append(list(buttons))
+
+    def to_json(self) -> JSONDict:
+        if self._inline_keyboard is None:
+            return None
+        return {
+            "inlineKeyboard": [[x.to_json() for x in row] for row in self._inline_keyboard],
+            "color": self._color.value,
+            "size": self._size.value,
+        }
+
+    def from_json(self, data: JSONDict) -> "InlineMarkup":
+        if data is None or data.get("inlineKeyboard") is None:
+            return None
+        self._color = InlineKeyboardColor(data.get("color") or "RANDOM")
+        self._size = InlineKeyboardSize(data.get("size") or "DEFAULT")
+        self._inline_keyboard = (
+            [
+                [InlineKeyboardButton.build_from_json(
+                    x, self.app) for x in row]
+                for row in data.get("inlineKeyboard") or []
+            ],
+        )
+
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/chat/models/message.py` & `swibots-1.2.9/swibots/api/chat/models/message.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,271 +1,295 @@
-from typing import TYPE_CHECKING, BinaryIO, Callable, List, Optional, Union
-import swibots
-from swibots.base import SwitchObject
-from swibots.api.common import User, MediaUploadRequest, Media
-from swibots.api.community import Community, Channel, Group
-from swibots.utils.types import JSONDict
-from .inline_markup import InlineMarkup
-
-
-class Message(
-    SwitchObject,
-):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        id: int = None,
-        user_id: int = None,
-        user: "User" = None,
-        receiver_id: int = None,
-        receiver: "User" = None,
-        message: str = None,
-        sent_date: int = None,
-        status: int = None,
-        request_id: int = None,
-        button_name: str = None,
-        button_pressed_id: int = None,
-        callback_data: str = None,
-        channel_chat: bool = None,
-        channel_id: int = None,
-        channel: "Channel" = None,
-        command_name: str = None,
-        community_id: int = None,
-        community: "Community" = None,
-        edit: bool = None,
-        flag: int = None,
-        forward: bool = None,
-        group_chat: bool = None,
-        group_id: int = None,
-        group: "Group" = None,
-        information: str = None,
-        inline_markup: "InlineMarkup" = None,
-        is_read: bool = None,
-        media_link: str = None,
-        mentioned_ids: List[int] = None,
-        personal_chat: bool = None,
-        pinned: bool = None,
-        reactions: List[str] = None,
-        replied_message: str = None,
-        replied_to_id: int = None,
-        replied_to: "Message" = None,
-        replies: List["Message"] = None,
-        reply_count: int = None,
-        media_id: int = None,
-        media_info: Media = None,
-        cached_media: Media = None,
-        **kwargs,
-    ):
-        super().__init__(app=app)
-        self.id = id
-        self.user_id = user_id
-        self.user = user
-        self.receiver_id = receiver_id
-        self.receiver = receiver
-        self.message = message
-        self.sent_date = sent_date
-        self.status = status
-        self.request_id = request_id
-        self.button_name = button_name
-        self.button_pressed_id = button_pressed_id
-        self.callback_data = callback_data
-        self.channel_chat = channel_chat
-        self.channel_id = channel_id
-        self.channel = channel
-        self.command_name = command_name
-        self.community_id = community_id
-        self.community = community
-        self.edit = edit
-        self.flag = flag
-        self.forward = forward
-        self.group_chat = group_chat
-        self.group_id = group_id
-        self.group = group
-        self.information = information
-        self.inline_markup = inline_markup
-        self.is_read = is_read
-        self.media_link = media_link
-        self.media_id = media_id
-        self.media_info = media_info
-        self.mentioned_ids = mentioned_ids
-        self.personal_chat = personal_chat
-        self.pinned = pinned
-        self.reactions = reactions
-        self.replied_message = replied_message
-        self.replied_to_id = replied_to_id
-        self.replied_to = replied_to
-        self.replies = replies
-        self.reply_count = reply_count
-        self.cached_media = cached_media
-        self.__dict__.update(**kwargs)
-
-    def to_json_request(self) -> JSONDict:
-        return {
-            "id": self.id,
-            "message": self.message,
-            "receiverId": self.receiver_id,
-            "requestId": self.request_id,
-            "userId": self.user_id,
-            "communityId": self.community_id,
-            "groupId": self.group_id,
-            "channelId": self.channel_id,
-            "inline_markup": self.inline_markup.to_json_request() if self.inline_markup else None,
-            "callback_data": self.callback_data,
-            "repliedTo": self.replied_to_id,
-            "mediaLink": self.media_link,
-            "status": self.status,
-            "cachedMedia": self.cached_media.to_json() if self.cached_media else None,
-            "mediaId": self.media_id,
-            "mediaInfo": self.media_info.to_json() if self.media_info else None,
-        }
-
-    def to_json(self) -> JSONDict:
-        return {
-            "buttonName": self.button_name,
-            "buttonPressedId": self.button_pressed_id,
-            "callback_data": self.callback_data,
-            "channelChat": self.channel_chat,
-            "channelId": self.channel_id,
-            "commandName": self.command_name,
-            "communityId": self.community_id,
-            "edit": self.edit,
-            "flag": self.flag,
-            "forward": self.forward,
-            "groupChat": self.group_chat,
-            "groupId": self.group_id,
-            "id": self.id,
-            "information": self.information,
-            "inline_markup": self.inline_markup.to_json() if self.inline_markup else None,
-            "isRead": self.is_read,
-            "mediaLink": self.media_link,
-            "mentionedIds": self.mentioned_ids,
-            "message": self.message,
-            "personalChat": self.personal_chat,
-            "pinned": self.pinned,
-            "reactions": self.reactions,
-            "receiverId": self.receiver_id,
-            "repliedMessage": self.replied_message,
-            "repliedTo": self.replied_to_id,
-            "replies": self.replies,
-            "replyCount": self.reply_count,
-            "requestId": self.request_id,
-            "sentDate": self.sent_date,
-            "status": self.status,
-            "userId": self.user_id,
-        }
-
-    def from_json(self, data: Optional[JSONDict]) -> "Message":
-        if data is not None:
-            self.button_name = data.get("buttonName")
-            self.button_pressed_id = data.get("buttonPressedId")
-            self.callback_data = data.get("callback_data")
-            self.channel_chat = data.get("channelChat")
-            self.channel_id = data.get("channelId")
-            self.channel = Channel.build_from_json(
-                data.get("channel"), self.app)
-            self.command_name = data.get("commandName")
-            self.community_id = data.get("communityId")
-            self.community = Community.build_from_json(
-                data.get("community"), self.app)
-            self.edit = data.get("edit")
-            self.flag = data.get("flag")
-            self.forward = data.get("forward")
-            self.group_chat = data.get("groupChat")
-            self.group_id = data.get("groupId")
-            self.group = Group.build_from_json(data.get("group"), self.app)
-            self.id = data.get("id")
-            self.information = data.get("information")
-            self.inline_markup = InlineMarkup.build_from_json(
-                data.get("inline_markup"), self.app)
-            self.is_read = data.get("isRead")
-            self.media_link = data.get("mediaLink")
-            self.media_id = data.get("mediaId")
-            self.media_info = Media.build_from_json(
-                data.get("mediaInfo"), self.app)
-            self.mentioned_ids = data.get("mentionedIds")
-            self.message = data.get("message")
-            self.personal_chat = data.get("personalChat")
-            self.pinned = data.get("pinned")
-            self.reactions = data.get("reactions")
-            self.receiver_id = data.get("receiverId")
-            self.replied_to = data.get("repliedMessage")
-            self.replied_to_id = data.get("repliedTo")
-            self.replies = data.get("replies")
-            self.reply_count = data.get("replyCount")
-            self.request_id = data.get("requestId")
-            self.sent_date = data.get("sentDate")
-            self.status = data.get("status")
-            self.user_id = data.get("userId")
-        return self
-
-    # async def get_receiver(self) -> "User":
-    #     if self.receiver_id is None:
-    #         return None
-    #     if self._receiver is None:
-    #         self._receiver = await self.app.get_user(self.receiver_id)
-    #     return self._receiver
-
-    # async def get_group(self) -> "Group":
-    #     if self.group_id is None:
-    #         return None
-    #     if self.group is None:
-    #         self.group = await self.app.getgroup(self.group_id)
-    #     return self.group
-
-    # async def get_channel(self) -> "Channel":
-    #     if self.channel_id is None:
-    #         return None
-    #     if self.channel is None:
-    #         self.channel = await self.app.get_channel(self.channel_id)
-    #     return self.channel
-
-    # async def get_community(self) -> "Community":
-    #     if self.community_id is None:
-    #         return None
-    #     if self.community is None:
-    #         self.community = await self.app.get_community(self.community_id)
-    #     return self.community
-
-    # async def get_replied_to(self) -> "Message":
-    #     if self.replied_to_id is None or self.replied_to_id <= 0:
-    #         return None
-    #     if self.replied_to is None:
-    #         self.replied_to = await self.app.get_message(self.replied_to_id)
-    #     return self.replied_to
-
-    async def get_replies(self) -> List["Message"]:
-        if self.reply_count <= 0:
-            return []
-        if self.replies is None:
-            self.replies = await self.app.get_message_replies(self.id)
-        return self.replies
-
-    async def get_replied_message(self) -> "Message":
-        if self.replied_to_id is None or self.replied_to_id <= 0:
-            return None
-        if self.replied_to is None:
-            self.replied_to = await self.app.get_message(self.replied_to_id)
-        return self.replied_to
-
-    ### API Methods ###
-
-    async def send(self,  media: MediaUploadRequest = None) -> "Message":
-        if self.id is not None:
-            return await self.app.edit_message(self)
-        return await self.app.send_message(self, media)
-
-    async def delete(self) -> None:
-        await self.app.delete_message(self)
-
-    async def reply(self, reply: "Message", media: MediaUploadRequest = None) -> "Message":
-        if isinstance(reply, str):
-            return await self.app.reply_message_text(self, reply, media)
-        return await self.app.reply_message(self, reply, media)
-
-    async def reply_text(self, text: str, inline_markup: Optional[InlineMarkup] = None,  media: MediaUploadRequest = None, cached_media: Media = None) -> "Message":
-        return await self.app.reply_message_text(self, text, inline_markup, media, cached_media)
-
-    async def edit_text(self, text: str,  inline_markup: Optional[InlineMarkup] = None) -> "Message":
-        return await self.app.edit_message_text(self, text, inline_markup)
-
-    async def download(self, file_name: str = None, in_memory: bool = False, block: bool = True, progress: Callable = None, progress_args: tuple = ()) -> Optional[Union[BinaryIO, bytes]]:
-        await self.app.download_media(self, file_name, in_memory, block, progress, progress_args)
+from typing import TYPE_CHECKING, BinaryIO, Callable, List, Optional, Union
+import swibots
+from swibots.base import SwitchObject
+from swibots.api.common import User, MediaUploadRequest, Media
+from swibots.api.community import Community, Channel, Group
+from swibots.utils.types import JSONDict
+from .inline_markup import InlineMarkup
+
+
+class Message(
+    SwitchObject,
+):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        id: int = None,
+        user_id: int = None,
+        user: "User" = None,
+        receiver_id: int = None,
+        receiver: "User" = None,
+        message: str = None,
+        sent_date: int = None,
+        status: int = None,
+        request_id: int = None,
+        button_name: str = None,
+        button_pressed_id: int = None,
+        callback_data: str = None,
+        channel_chat: bool = None,
+        channel_id: int = None,
+        channel: "Channel" = None,
+        command_name: str = None,
+        community_id: int = None,
+        community: "Community" = None,
+        edit: bool = None,
+        flag: int = None,
+        forward: bool = None,
+        group_chat: bool = None,
+        group_id: int = None,
+        group: "Group" = None,
+        information: str = None,
+        inline_markup: "InlineMarkup" = None,
+        is_read: bool = None,
+        media_link: str = None,
+        mentioned_ids: List[int] = None,
+        personal_chat: bool = None,
+        pinned: bool = None,
+        reactions: List[str] = None,
+        replied_message: str = None,
+        replied_to_id: int = None,
+        replied_to: "Message" = None,
+        replies: List["Message"] = None,
+        reply_count: int = None,
+        media_id: int = None,
+        media_info: Media = None,
+        cached_media: Media = None,
+        **kwargs,
+    ):
+        super().__init__(app=app)
+        self.id = id
+        self.user_id = user_id
+        self.user = user
+        self.receiver_id = receiver_id
+        self.receiver = receiver
+        self.message = message
+        self.sent_date = sent_date
+        self.status = status
+        self.request_id = request_id
+        self.button_name = button_name
+        self.button_pressed_id = button_pressed_id
+        self.callback_data = callback_data
+        self.channel_chat = channel_chat
+        self.channel_id = channel_id
+        self.channel = channel
+        self.command_name = command_name
+        self.community_id = community_id
+        self.community = community
+        self.edit = edit
+        self.flag = flag
+        self.forward = forward
+        self.group_chat = group_chat
+        self.group_id = group_id
+        self.group = group
+        self.information = information
+        self.inline_markup = inline_markup
+        self.is_read = is_read
+        self.media_link = media_link
+        self.media_id = media_id
+        self.media_info = media_info
+        self.mentioned_ids = mentioned_ids
+        self.personal_chat = personal_chat
+        self.pinned = pinned
+        self.reactions = reactions
+        self.replied_message = replied_message
+        self.replied_to_id = replied_to_id
+        self.replied_to = replied_to
+        self.replies = replies
+        self.reply_count = reply_count
+        self.cached_media = cached_media
+        self.__dict__.update(**kwargs)
+
+    def to_json_request(self) -> JSONDict:
+        return {
+            "id": self.id,
+            "message": self.message,
+            "receiverId": self.receiver_id,
+            "requestId": self.request_id,
+            "userId": self.user_id,
+            "communityId": self.community_id,
+            "groupId": self.group_id,
+            "channelId": self.channel_id,
+            "inline_markup": self.inline_markup.to_json_request() if self.inline_markup else None,
+            "callback_data": self.callback_data,
+            "repliedTo": self.replied_to_id,
+            "mediaLink": self.media_link,
+            "status": self.status,
+            "cachedMedia": self.cached_media.to_json() if self.cached_media else None,
+            "mediaId": self.media_id,
+            "mediaInfo": self.media_info.to_json() if self.media_info else None,
+        }
+
+    def to_form_data(self):
+        form_data = {}
+        if self.user_id is not None:
+            form_data["userId"] = self.user_id
+        if self.receiver_id is not None:
+            form_data["receiverId"] = self.receiver_id
+        if self.request_id is not None:
+            form_data["requestId"] = self.request_id
+        if self.community_id is not None:
+            form_data["communityId"] = self.community_id
+        if self.channel_id is not None:
+            form_data["channelId"] = self.channel_id
+        if self.group_id is not None:
+            form_data["groupId"] = self.group_id
+        if self.replied_to_id is not None:
+            form_data["repliedTo"] = self.replied_to_id
+        if self.message is not None:
+            form_data["message"] = self.message
+        if self.media_link is not None:
+            form_data["mediaLink"] = self.media_link
+        if self.status is not None:
+            form_data["status"] = self.status
+        return form_data
+
+    def to_json(self) -> JSONDict:
+        return {
+            "buttonName": self.button_name,
+            "buttonPressedId": self.button_pressed_id,
+            "callback_data": self.callback_data,
+            "channelChat": self.channel_chat,
+            "channelId": self.channel_id,
+            "commandName": self.command_name,
+            "communityId": self.community_id,
+            "edit": self.edit,
+            "flag": self.flag,
+            "forward": self.forward,
+            "groupChat": self.group_chat,
+            "groupId": self.group_id,
+            "id": self.id,
+            "information": self.information,
+            "inline_markup": self.inline_markup.to_json() if self.inline_markup else None,
+            "isRead": self.is_read,
+            "mediaLink": self.media_link,
+            "mentionedIds": self.mentioned_ids,
+            "message": self.message,
+            "personalChat": self.personal_chat,
+            "pinned": self.pinned,
+            "reactions": self.reactions,
+            "receiverId": self.receiver_id,
+            "repliedMessage": self.replied_message,
+            "repliedTo": self.replied_to_id,
+            "replies": self.replies,
+            "replyCount": self.reply_count,
+            "requestId": self.request_id,
+            "sentDate": self.sent_date,
+            "status": self.status,
+            "userId": self.user_id,
+        }
+
+    def from_json(self, data: Optional[JSONDict]) -> "Message":
+        if data is not None:
+            self.button_name = data.get("buttonName")
+            self.button_pressed_id = data.get("buttonPressedId")
+            self.callback_data = data.get("callback_data")
+            self.channel_chat = data.get("channelChat")
+            self.channel_id = data.get("channelId")
+            self.channel = Channel.build_from_json(
+                data.get("channel"), self.app)
+            self.command_name = data.get("commandName")
+            self.community_id = data.get("communityId")
+            self.community = Community.build_from_json(
+                data.get("community"), self.app)
+            self.edit = data.get("edit")
+            self.flag = data.get("flag")
+            self.forward = data.get("forward")
+            self.group_chat = data.get("groupChat")
+            self.group_id = data.get("groupId")
+            self.group = Group.build_from_json(data.get("group"), self.app)
+            self.id = data.get("id")
+            self.information = data.get("information")
+            self.inline_markup = InlineMarkup.build_from_json(
+                data.get("inline_markup"), self.app)
+            self.is_read = data.get("isRead")
+            self.media_link = data.get("mediaLink")
+            self.media_id = data.get("mediaId")
+            self.media_info = Media.build_from_json(
+                data.get("mediaInfo"), self.app)
+            self.mentioned_ids = data.get("mentionedIds")
+            self.message = data.get("message")
+            self.personal_chat = data.get("personalChat")
+            self.pinned = data.get("pinned")
+            self.reactions = data.get("reactions")
+            self.receiver_id = data.get("receiverId")
+            self.replied_to = data.get("repliedMessage")
+            self.replied_to_id = data.get("repliedTo")
+            self.replies = data.get("replies")
+            self.reply_count = data.get("replyCount")
+            self.request_id = data.get("requestId")
+            self.sent_date = data.get("sentDate")
+            self.status = data.get("status")
+            self.user_id = data.get("userId")
+        return self
+
+    # async def get_receiver(self) -> "User":
+    #     if self.receiver_id is None:
+    #         return None
+    #     if self._receiver is None:
+    #         self._receiver = await self.app.get_user(self.receiver_id)
+    #     return self._receiver
+
+    # async def get_group(self) -> "Group":
+    #     if self.group_id is None:
+    #         return None
+    #     if self.group is None:
+    #         self.group = await self.app.getgroup(self.group_id)
+    #     return self.group
+
+    # async def get_channel(self) -> "Channel":
+    #     if self.channel_id is None:
+    #         return None
+    #     if self.channel is None:
+    #         self.channel = await self.app.get_channel(self.channel_id)
+    #     return self.channel
+
+    # async def get_community(self) -> "Community":
+    #     if self.community_id is None:
+    #         return None
+    #     if self.community is None:
+    #         self.community = await self.app.get_community(self.community_id)
+    #     return self.community
+
+    # async def get_replied_to(self) -> "Message":
+    #     if self.replied_to_id is None or self.replied_to_id <= 0:
+    #         return None
+    #     if self.replied_to is None:
+    #         self.replied_to = await self.app.get_message(self.replied_to_id)
+    #     return self.replied_to
+
+    async def get_replies(self) -> List["Message"]:
+        if self.reply_count <= 0:
+            return []
+        if self.replies is None:
+            self.replies = await self.app.get_message_replies(self.id)
+        return self.replies
+
+    async def get_replied_message(self) -> "Message":
+        if self.replied_to_id is None or self.replied_to_id <= 0:
+            return None
+        if self.replied_to is None:
+            self.replied_to = await self.app.get_message(self.replied_to_id)
+        return self.replied_to
+
+    ### API Methods ###
+
+    async def send(self,  media: MediaUploadRequest = None) -> "Message":
+        if self.id is not None:
+            return await self.app.edit_message(self)
+        return await self.app.send_message(self, media)
+
+    async def delete(self) -> None:
+        await self.app.delete_message(self)
+
+    async def reply(self, reply: "Message", media: MediaUploadRequest = None) -> "Message":
+        if isinstance(reply, str):
+            return await self.app.reply_message_text(self, reply, media)
+        return await self.app.reply_message(self, reply, media)
+
+    async def reply_text(self, text: str, inline_markup: Optional[InlineMarkup] = None,  media: MediaUploadRequest = None, cached_media: Media = None) -> "Message":
+        return await self.app.reply_message_text(self, text, inline_markup, media, cached_media)
+
+    async def edit_text(self, text: str,  inline_markup: Optional[InlineMarkup] = None) -> "Message":
+        return await self.app.edit_message_text(self, text, inline_markup)
+
+    async def download(self, file_name: str = None, in_memory: bool = False, block: bool = True, progress: Callable = None, progress_args: tuple = ()) -> Optional[Union[BinaryIO, bytes]]:
+        await self.app.download_media(self, file_name, in_memory, block, progress, progress_args)
```

### Comparing `swibots-1.2.8/swibots/api/common/events/event.py` & `swibots-1.2.9/swibots/api/common/events/event.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from typing import Optional
-import swibots
-from swibots.base.switch_object import SwitchObject
-
-# from switch.api.community.models import Community, Group, Channel
-# from switch.base.switch_object import SwitchObject
-# from switch.types import EventType
-# from switch.api.common.models.user import User
-# from switch.utils.types import JSONDict
-
-
-class Event(SwitchObject):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        type: Optional["swibots.EventType"] = None,
-        data: Optional[dict] = None,
-        community_id: Optional[str] = None,
-        community: Optional["swibots.Community"] = None,
-        group_id: Optional[str] = None,
-        group: Optional["swibots.Group"] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional["swibots.Channel"] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional["swibots.User"] = None,
-    ):
-        super().__init__(app)
-        self.type = type
-        self.data = data
-        self.action_by_id = action_by_id
-        self.action_by = action_by
-        self.community_id = community_id
-        self.community = community
-        self.group_id = group_id
-        self.group = group
-        self.channel_id = channel_id
-        self.channel = channel
-
-    def from_json(self, data: swibots.JSONDict) -> "Event":
-        if data is not None:
-            details = data.get("details") or {}
-            self.type = swibots.EventType(data.get("type"))
-            self.action_by_id = data.get("actionById")
-            self.action_by = swibots.User.build_from_json(
-                data.get("actionBy"), self.app)
-            self.community_id = details.get("communityId")
-            self.community = swibots.Community.build_from_json(
-                details.get("community"), self.app)
-            self.group_id = details.get("groupId")
-            self.group = swibots.Group.build_from_json(
-                details.get("group"), self.app)
-            self.channel_id = details.get("channelId")
-            self.channel = swibots.Channel.build_from_json(
-                details.get("channel"), self.app)
-            self.data = details
-        return self
-
-    def to_json(self) -> swibots.JSONDict:
-        return {
-            "type": self.type,
-            "details": self.data,
-            "communityId": self.community_id,
-            "community": self.community.to_json() if self.community else None,
-            "groupId": self.group_id,
-            "group": self.group.to_json() if self.group else None,
-            "channelId": self.channel_id,
-            "channel": self.channel.to_json() if self.channel else None,
-            "actionById": self.action_by_id,
-            "actionBy": self.action_by.to_json() if self.action_by else None,
-        }
+from typing import Optional
+import swibots
+from swibots.base.switch_object import SwitchObject
+
+# from switch.api.community.models import Community, Group, Channel
+# from switch.base.switch_object import SwitchObject
+# from switch.types import EventType
+# from switch.api.common.models.user import User
+# from switch.utils.types import JSONDict
+
+
+class Event(SwitchObject):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        type: Optional["swibots.EventType"] = None,
+        data: Optional[dict] = None,
+        community_id: Optional[str] = None,
+        community: Optional["swibots.Community"] = None,
+        group_id: Optional[str] = None,
+        group: Optional["swibots.Group"] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional["swibots.Channel"] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional["swibots.User"] = None,
+    ):
+        super().__init__(app)
+        self.type = type
+        self.data = data
+        self.action_by_id = action_by_id
+        self.action_by = action_by
+        self.community_id = community_id
+        self.community = community
+        self.group_id = group_id
+        self.group = group
+        self.channel_id = channel_id
+        self.channel = channel
+
+    def from_json(self, data: swibots.JSONDict) -> "Event":
+        if data is not None:
+            details = data.get("details") or {}
+            self.type = swibots.EventType(data.get("type"))
+            self.action_by_id = data.get("actionById")
+            self.action_by = swibots.User.build_from_json(
+                data.get("actionBy"), self.app)
+            self.community_id = details.get("communityId")
+            self.community = swibots.Community.build_from_json(
+                details.get("community"), self.app)
+            self.group_id = details.get("groupId")
+            self.group = swibots.Group.build_from_json(
+                details.get("group"), self.app)
+            self.channel_id = details.get("channelId")
+            self.channel = swibots.Channel.build_from_json(
+                details.get("channel"), self.app)
+            self.data = details
+        return self
+
+    def to_json(self) -> swibots.JSONDict:
+        return {
+            "type": self.type,
+            "details": self.data,
+            "communityId": self.community_id,
+            "community": self.community.to_json() if self.community else None,
+            "groupId": self.group_id,
+            "group": self.group.to_json() if self.group else None,
+            "channelId": self.channel_id,
+            "channel": self.channel.to_json() if self.channel else None,
+            "actionById": self.action_by_id,
+            "actionBy": self.action_by.to_json() if self.action_by else None,
+        }
```

### Comparing `swibots-1.2.8/swibots/api/common/models/media.py` & `swibots-1.2.9/swibots/api/common/models/media.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from typing import Optional
-from swibots.utils.types import JSONDict
-from swibots.base.switch_object import SwitchObject
-
-
-class Media(SwitchObject):
-    def __init__(
-        self,
-        id: Optional[int] = None,
-        caption: Optional[str] = None,
-        description: Optional[str] = None,
-        thumbnail_url: Optional[str] = None,
-        source_id: Optional[bool] = None,
-        media_type: Optional[bool] = None,
-        mime_type: Optional[str] = None,
-        file_name: Optional[bool] = None,
-        file_size: Optional[bool] = None,
-        url: Optional[bool] = None,
-    ):
-        self.id = id
-        self.caption = caption
-        self.description = description
-        self.thumbnail_url = thumbnail_url
-        self.source_id = source_id
-        self.media_type = media_type
-        self.mime_type = mime_type
-        self.file_name = file_name
-        self.file_size = file_size
-        self.url = url
-
-    def to_json(self) -> JSONDict:
-        return {
-            "id": self.id,
-            "caption": self.caption,
-            "description": self.description,
-            "thumbnailUrl": self.thumbnail_url,
-            "sourceId": self.source_id,
-            "mediaType": self.media_type,
-            "mimeType": self.mime_type,
-            "fileName": self.file_name,
-            "fileSize": self.file_size,
-            "downloadUrl": self.url,
-        }
-
-    def from_json(self, data: Optional[JSONDict] = None) -> "Media":
-        if data is not None:
-            self.id = data.get("id")
-            self.caption = data.get("caption")
-            self.description = data.get("description")
-            self.thumbnail_url = data.get("thumbnailUrl")
-            self.source_id = data.get("sourceId")
-            self.media_type = data.get("mediaType")
-            self.mime_type = data.get("mimeType")
-            self.file_name = data.get("fileName")
-            self.file_size = data.get("fileSize")
-            self.url = data.get("downloadUrl")
-        return self
+from typing import Optional
+from swibots.utils.types import JSONDict
+from swibots.base.switch_object import SwitchObject
+
+
+class Media(SwitchObject):
+    def __init__(
+        self,
+        id: Optional[int] = None,
+        caption: Optional[str] = None,
+        description: Optional[str] = None,
+        thumbnail_url: Optional[str] = None,
+        source_id: Optional[bool] = None,
+        media_type: Optional[bool] = None,
+        mime_type: Optional[str] = None,
+        file_name: Optional[bool] = None,
+        file_size: Optional[bool] = None,
+        url: Optional[bool] = None,
+    ):
+        self.id = id
+        self.caption = caption
+        self.description = description
+        self.thumbnail_url = thumbnail_url
+        self.source_id = source_id
+        self.media_type = media_type
+        self.mime_type = mime_type
+        self.file_name = file_name
+        self.file_size = file_size
+        self.url = url
+
+    def to_json(self) -> JSONDict:
+        return {
+            "id": self.id,
+            "caption": self.caption,
+            "description": self.description,
+            "thumbnailUrl": self.thumbnail_url,
+            "sourceId": self.source_id,
+            "mediaType": self.media_type,
+            "mimeType": self.mime_type,
+            "fileName": self.file_name,
+            "fileSize": self.file_size,
+            "downloadUrl": self.url,
+        }
+
+    def from_json(self, data: Optional[JSONDict] = None) -> "Media":
+        if data is not None:
+            self.id = data.get("id")
+            self.caption = data.get("caption")
+            self.description = data.get("description")
+            self.thumbnail_url = data.get("thumbnailUrl")
+            self.source_id = data.get("sourceId")
+            self.media_type = data.get("mediaType")
+            self.mime_type = data.get("mimeType")
+            self.file_name = data.get("fileName")
+            self.file_size = data.get("fileSize")
+            self.url = data.get("downloadUrl")
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/common/models/user.py` & `swibots-1.2.9/swibots/api/common/models/user.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from typing import Optional
-from swibots.utils.types import JSONDict
-from swibots.base.switch_object import SwitchObject
-
-
-class User(SwitchObject):
-    def __init__(
-        self,
-        id: Optional[int] = None,
-        name: Optional[str] = None,
-        username: Optional[str] = None,
-        image_url: Optional[str] = None,
-        active: Optional[bool] = None,
-        deleted: Optional[bool] = None,
-        role_info: Optional[str] = None,
-        admin: Optional[bool] = None,
-        is_bot: Optional[bool] = None,
-    ):
-        self.id = id
-        self.name = name
-        self.username = username
-        self.image_url = image_url
-        self.active = active
-        self.deleted = deleted
-        self.role_info = role_info
-        self.admin = admin
-        self.is_bot = is_bot
-
-    def to_json(self) -> JSONDict:
-        return {
-            "id": self.id,
-            "name": self.name,
-            "username": self.username,
-            "imageUrl": self.image_url,
-            "active": self.active,
-            "deleted": self.deleted,
-            "roleInfo": self.role_info,
-            "admin": self.admin,
-            "is_bot": self.is_bot,
-        }
-
-    def from_json(self, data: Optional[JSONDict] = None) -> "User":
-        if data is not None:
-            self.id = data.get("id")
-            self.name = data.get("name")
-            self.username = data.get("username")
-            self.image_url = data.get("imageUrl")
-            self.active = data.get("active")
-            self.deleted = data.get("deleted")
-            self.role_info = data.get("roleInfo")
-            self.admin = data.get("admin")
-            self.is_bot = data.get("is_bot")
-        return self
+from typing import Optional
+from swibots.utils.types import JSONDict
+from swibots.base.switch_object import SwitchObject
+
+
+class User(SwitchObject):
+    def __init__(
+        self,
+        id: Optional[int] = None,
+        name: Optional[str] = None,
+        username: Optional[str] = None,
+        image_url: Optional[str] = None,
+        active: Optional[bool] = None,
+        deleted: Optional[bool] = None,
+        role_info: Optional[str] = None,
+        admin: Optional[bool] = None,
+        is_bot: Optional[bool] = None,
+    ):
+        self.id = id
+        self.name = name
+        self.username = username
+        self.image_url = image_url
+        self.active = active
+        self.deleted = deleted
+        self.role_info = role_info
+        self.admin = admin
+        self.is_bot = is_bot
+
+    def to_json(self) -> JSONDict:
+        return {
+            "id": self.id,
+            "name": self.name,
+            "username": self.username,
+            "imageUrl": self.image_url,
+            "active": self.active,
+            "deleted": self.deleted,
+            "roleInfo": self.role_info,
+            "admin": self.admin,
+            "is_bot": self.is_bot,
+        }
+
+    def from_json(self, data: Optional[JSONDict] = None) -> "User":
+        if data is not None:
+            self.id = data.get("id")
+            self.name = data.get("name")
+            self.username = data.get("username")
+            self.image_url = data.get("imageUrl")
+            self.active = data.get("active")
+            self.deleted = data.get("deleted")
+            self.role_info = data.get("roleInfo")
+            self.admin = data.get("admin")
+            self.is_bot = data.get("is_bot")
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/community/community_client.py` & `swibots-1.2.9/swibots/api/community/community_client.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-import json
-from swibots.api.auth.models.auth_user import AuthUser
-from swibots.api.community.events import *
-from swibots.base import SwitchRestClient, SwitchWSAsyncClient
-from swibots.config import get_config
-from swibots.error import SwitchError
-from swibots.utils.ws.asyncstomp.async_ws_subscription import AsyncWsSubscription
-from swibots.utils.ws.common.ws_message import WsMessage
-from swibots.types import EventType
-from .controllers import ChannelController, GroupController, CommunityController
-import swibots
-
-
-class CommunityClient(SwitchRestClient):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        base_url: str = None,
-        ws_url: str = None,
-    ):
-        base_url = base_url or get_config()["COMMUNITY_SERVICE"]["BASE_URL"]
-        self._ws_url = ws_url or get_config()["COMMUNITY_SERVICE"]["WS_URL"]
-        super().__init__(app, base_url)
-        self._channels = None
-        self._groups = None
-        self._communities = None
-        self._ws: SwitchWSAsyncClient = None
-        self._started = False
-
-    @property
-    def channels(self) -> ChannelController:
-        """Get the channels controller"""
-        if self._channels is None:
-            self._channels = ChannelController(self)
-        return self._channels
-
-    @property
-    def groups(self) -> GroupController:
-        """Get the channels controller"""
-        if self._groups is None:
-            self._groups = GroupController(self)
-        return self._groups
-
-    @property
-    def communities(self) -> CommunityController:
-        """Get the channels controller"""
-        if self._communities is None:
-            self._communities = CommunityController(self)
-        return self._communities
-
-    @property
-    def ws(self) -> SwitchWSAsyncClient:
-        if self._ws is None:
-            self._ws = SwitchWSAsyncClient(self._ws_url, self.token)
-        return self._ws
-
-    @property
-    async def subscribe(self, endpoint: str, callback=None) -> AsyncWsSubscription:
-        if self.user is None:
-            raise SwitchError("User is not set")
-        if callback is None:
-            raise SwitchError("Callback is not set")
-        return await self.ws.subscribe(endpoint, callback=callback)
-
-    async def subscribe_to_notifications(self, callback=None) -> AsyncWsSubscription:
-        subscription = await self.ws.subscribe(
-            "/user/queue/events",
-            callback=lambda event: callback(self._parse_event(event)),
-        )
-        return subscription
-
-    def _parse_event(self, raw_message: WsMessage) -> CommunityEvent:
-        json_data = json.loads(raw_message.body)
-        type = json_data.get("type", "COMMUNITY")
-        evt = None
-        if type == EventType.COMMUNITY_CHANNEL_CREATE.value:
-            evt = self.build_object(ChannelCreatedEvent, json_data)
-            # return ChannelCreatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_CHANNEL_UPDATE.value:
-            evt = self.build_object(ChannelUpdatedEvent, json_data)
-            # return ChannelUpdatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_CHANNEL_DELETE.value:
-            evt = self.build_object(ChannelDeletedEvent, json_data)
-            # return ChannelDeletedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_UPDATE.value:
-            evt = self.build_object(CommunityUpdatedEvent, json_data)
-            # return CommunityUpdatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_GROUP_CREATE.value:
-            evt = self.build_object(GroupCreatedEvent, json_data)
-            # return GroupCreatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_GROUP_UPDATE.value:
-            evt = self.build_object(GroupUpdatedEvent, json_data)
-            # return GroupUpdatedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_GROUP_DELETE.value:
-            evt = self.build_object(GroupDeletedEvent, json_data)
-            # return GroupDeletedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_USER_BAN.value:
-            evt = self.build_object(UserBannedEvent, json_data)
-            # return UserBannedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_MEMBER_JOIN.value:
-            evt = self.build_object(MemberJoinedEvent, json_data)
-            # return MemberJoinedEvent.build_from_json(json_data)
-        elif type == EventType.COMMUNITY_MEMBER_LEAVE.value:
-            evt = self.build_object(MemberLeftEvent, json_data)
-            # return MemberLeftEvent.build_from_json(json_data)
-        else:
-            evt = self.build_object(CommunityEvent, json_data)
-
-        return evt
-
-    async def start(self):
-        """Start the community client"""
-        if self.user is None:
-            raise SwitchError("User is not set")
-        await self.ws.connect()
-        self._started = True
-
-    async def stop(self):
-        if self._started:
-            await self.ws.disconnect()
-            self._started = False
+import json
+from swibots.api.auth.models.auth_user import AuthUser
+from swibots.api.community.events import *
+from swibots.base import SwitchRestClient, SwitchWSAsyncClient
+from swibots.config import get_config
+from swibots.error import SwitchError
+from swibots.utils.ws.asyncstomp.async_ws_subscription import AsyncWsSubscription
+from swibots.utils.ws.common.ws_message import WsMessage
+from swibots.types import EventType
+from .controllers import ChannelController, GroupController, CommunityController
+import swibots
+
+
+class CommunityClient(SwitchRestClient):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        base_url: str = None,
+        ws_url: str = None,
+    ):
+        base_url = base_url or get_config()["COMMUNITY_SERVICE"]["BASE_URL"]
+        self._ws_url = ws_url or get_config()["COMMUNITY_SERVICE"]["WS_URL"]
+        super().__init__(app, base_url)
+        self._channels = None
+        self._groups = None
+        self._communities = None
+        self._ws: SwitchWSAsyncClient = None
+        self._started = False
+
+    @property
+    def channels(self) -> ChannelController:
+        """Get the channels controller"""
+        if self._channels is None:
+            self._channels = ChannelController(self)
+        return self._channels
+
+    @property
+    def groups(self) -> GroupController:
+        """Get the channels controller"""
+        if self._groups is None:
+            self._groups = GroupController(self)
+        return self._groups
+
+    @property
+    def communities(self) -> CommunityController:
+        """Get the channels controller"""
+        if self._communities is None:
+            self._communities = CommunityController(self)
+        return self._communities
+
+    @property
+    def ws(self) -> SwitchWSAsyncClient:
+        if self._ws is None:
+            self._ws = SwitchWSAsyncClient(self._ws_url, self.token)
+        return self._ws
+
+    @property
+    async def subscribe(self, endpoint: str, callback=None) -> AsyncWsSubscription:
+        if self.user is None:
+            raise SwitchError("User is not set")
+        if callback is None:
+            raise SwitchError("Callback is not set")
+        return await self.ws.subscribe(endpoint, callback=callback)
+
+    async def subscribe_to_notifications(self, callback=None) -> AsyncWsSubscription:
+        subscription = await self.ws.subscribe(
+            "/user/queue/events",
+            callback=lambda event: callback(self._parse_event(event)),
+        )
+        return subscription
+
+    def _parse_event(self, raw_message: WsMessage) -> CommunityEvent:
+        json_data = json.loads(raw_message.body)
+        type = json_data.get("type", "COMMUNITY")
+        evt = None
+        if type == EventType.COMMUNITY_CHANNEL_CREATE.value:
+            evt = self.build_object(ChannelCreatedEvent, json_data)
+            # return ChannelCreatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_CHANNEL_UPDATE.value:
+            evt = self.build_object(ChannelUpdatedEvent, json_data)
+            # return ChannelUpdatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_CHANNEL_DELETE.value:
+            evt = self.build_object(ChannelDeletedEvent, json_data)
+            # return ChannelDeletedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_UPDATE.value:
+            evt = self.build_object(CommunityUpdatedEvent, json_data)
+            # return CommunityUpdatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_GROUP_CREATE.value:
+            evt = self.build_object(GroupCreatedEvent, json_data)
+            # return GroupCreatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_GROUP_UPDATE.value:
+            evt = self.build_object(GroupUpdatedEvent, json_data)
+            # return GroupUpdatedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_GROUP_DELETE.value:
+            evt = self.build_object(GroupDeletedEvent, json_data)
+            # return GroupDeletedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_USER_BAN.value:
+            evt = self.build_object(UserBannedEvent, json_data)
+            # return UserBannedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_MEMBER_JOIN.value:
+            evt = self.build_object(MemberJoinedEvent, json_data)
+            # return MemberJoinedEvent.build_from_json(json_data)
+        elif type == EventType.COMMUNITY_MEMBER_LEAVE.value:
+            evt = self.build_object(MemberLeftEvent, json_data)
+            # return MemberLeftEvent.build_from_json(json_data)
+        else:
+            evt = self.build_object(CommunityEvent, json_data)
+
+        return evt
+
+    async def start(self):
+        """Start the community client"""
+        if self.user is None:
+            raise SwitchError("User is not set")
+        await self.ws.connect()
+        self._started = True
+
+    async def stop(self):
+        if self._started:
+            await self.ws.disconnect()
+            self._started = False
```

### Comparing `swibots-1.2.8/swibots/api/community/controllers/community_controller.py` & `swibots-1.2.9/swibots/api/community/controllers/channel_controller.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-import logging
-from typing import TYPE_CHECKING
-from swibots.api.community.models import Channel, Community, Group
-
-if TYPE_CHECKING:
-    from swibots.api.community import CommunityClient
-
-log = logging.getLogger(__name__)
-
-BASE_PATH = "/v1/community"
-
-
-class CommunityController:
-    def __init__(self, client: "CommunityClient"):
-        self.client = client
-
-    async def get_community(self, community_id: str):
-        """Get a community by id"""
-        response = await self.client.get(f"{BASE_PATH}?communityId={community_id}")
-        return self.client.build_object(Community, response.data.get("result"))
+
+import logging
+from typing import TYPE_CHECKING
+
+from swibots.api.community.models import Channel
+
+
+if TYPE_CHECKING:
+    from swibots.api.community import CommunityClient
+
+log = logging.getLogger(__name__)
+
+BASE_PATH = "/v1/community/channel"
+
+
+class ChannelController:
+    def __init__(self, client: "CommunityClient"):
+        self.client = client
+
+    async def get_channel(self, channel_id: str):
+        """Get a channel by id"""
+        response = await self.client.get(f"{BASE_PATH}?channelId={channel_id}")
+        return self.client.build_object(Channel, response.data.get("result"))
```

### Comparing `swibots-1.2.8/swibots/api/community/controllers/group_controller.py` & `swibots-1.2.9/swibots/api/community/controllers/group_controller.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import logging
-from typing import TYPE_CHECKING
-from swibots.api.community.models import Group
-
-if TYPE_CHECKING:
-    from swibots.api.community import CommunityClient
-
-log = logging.getLogger(__name__)
-
-BASE_PATH = "/v1/community/group"
-
-
-class GroupController:
-    def __init__(self, client: "CommunityClient"):
-        self.client = client
-
-    async def get_group(self, group_id: str):
-        """Get a channel by id"""
-        response = await self.client.get(f"{BASE_PATH}?groupId={group_id}")
-        return self.client.build_object(Group, response.data.get("result"))
+import logging
+from typing import TYPE_CHECKING
+from swibots.api.community.models import Group
+
+if TYPE_CHECKING:
+    from swibots.api.community import CommunityClient
+
+log = logging.getLogger(__name__)
+
+BASE_PATH = "/v1/community/group"
+
+
+class GroupController:
+    def __init__(self, client: "CommunityClient"):
+        self.client = client
+
+    async def get_group(self, group_id: str):
+        """Get a channel by id"""
+        response = await self.client.get(f"{BASE_PATH}?groupId={group_id}")
+        return self.client.build_object(Group, response.data.get("result"))
```

### Comparing `swibots-1.2.8/swibots/api/community/events/__init__.py` & `swibots-1.2.9/swibots/api/community/events/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .community_event import CommunityEvent
-from .channel_updated_event import ChannelUpdatedEvent
-from .channel_created_event import ChannelCreatedEvent
-from .channel_deleted_event import ChannelDeletedEvent
-from .community_updated_event import CommunityUpdatedEvent
-from .group_created_event import GroupCreatedEvent
-from .group_updated_event import GroupUpdatedEvent
-from .group_deleted_event import GroupDeletedEvent
-from .member_joined_event import MemberJoinedEvent
-from .member_left_event import MemberLeftEvent
-from .user_banned_event import UserBannedEvent
+from .community_event import CommunityEvent
+from .channel_updated_event import ChannelUpdatedEvent
+from .channel_created_event import ChannelCreatedEvent
+from .channel_deleted_event import ChannelDeletedEvent
+from .community_updated_event import CommunityUpdatedEvent
+from .group_created_event import GroupCreatedEvent
+from .group_updated_event import GroupUpdatedEvent
+from .group_deleted_event import GroupDeletedEvent
+from .member_joined_event import MemberJoinedEvent
+from .member_left_event import MemberLeftEvent
+from .user_banned_event import UserBannedEvent
```

### Comparing `swibots-1.2.8/swibots/api/community/events/channel_created_event.py` & `swibots-1.2.9/swibots/api/community/events/member_joined_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class ChannelCreatedEvent(CommunityEvent["ChannelCreatedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_CHANNEL_CREATE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class MemberJoinedEvent(CommunityEvent["MemberJoinedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_MEMBER_JOIN,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.2.8/swibots/api/community/events/channel_deleted_event.py` & `swibots-1.2.9/swibots/api/community/events/group_updated_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class ChannelDeletedEvent(CommunityEvent["ChannelDeletedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_CHANNEL_DELETE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class GroupUpdatedEvent(CommunityEvent["GroupUpdatedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_GROUP_UPDATE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.2.8/swibots/api/community/events/channel_updated_event.py` & `swibots-1.2.9/swibots/api/community/events/user_banned_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class ChannelUpdatedEvent(CommunityEvent["ChannelUpdatedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_CHANNEL_UPDATE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class UserBannedEvent(CommunityEvent["UserBannedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_USER_BAN,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.2.8/swibots/api/community/events/community_event.py` & `swibots-1.2.9/swibots/api/community/events/community_event.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from typing import Generic, Optional, TypeVar
-import swibots
-from swibots.api.common.events.event import Event
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-from swibots.utils.types import JSONDict
-
-T = TypeVar("T", bound="CommunityEvent")
-
-
-class CommunityEvent(Event, Generic[T]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        type: Optional[EventType] = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=type,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-        )
-        self.user_id = user_id
-        self.user = user
-
-    def to_json(self) -> JSONDict:
-        d = super().to_json()
-
-        d.update(
-            {
-                "communityId": self.community_id,
-                "community": self.community.to_json(),
-                "groupId": self.group_id,
-                "group": self.group.to_json(),
-                "channelId": self.channel_id,
-                "channel": self.channel.to_json(),
-                "userId": self.user_id,
-                "user": self.user.to_json(),
-            }
-        )
-        return d
-
-    def from_json(self, data: JSONDict) -> T:
-        if data is not None:
-            super().from_json(data)
-            details = data.get("details") or {}
-            self.user_id = data.get("userId")
-            self.user = User.build_from_json(details.get("user"), self.app)
-        return self
+from typing import Generic, Optional, TypeVar
+import swibots
+from swibots.api.common.events.event import Event
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+from swibots.utils.types import JSONDict
+
+T = TypeVar("T", bound="CommunityEvent")
+
+
+class CommunityEvent(Event, Generic[T]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        type: Optional[EventType] = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=type,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+        )
+        self.user_id = user_id
+        self.user = user
+
+    def to_json(self) -> JSONDict:
+        d = super().to_json()
+
+        d.update(
+            {
+                "communityId": self.community_id,
+                "community": self.community.to_json(),
+                "groupId": self.group_id,
+                "group": self.group.to_json(),
+                "channelId": self.channel_id,
+                "channel": self.channel.to_json(),
+                "userId": self.user_id,
+                "user": self.user.to_json(),
+            }
+        )
+        return d
+
+    def from_json(self, data: JSONDict) -> T:
+        if data is not None:
+            super().from_json(data)
+            details = data.get("details") or {}
+            self.user_id = data.get("userId")
+            self.user = User.build_from_json(details.get("user"), self.app)
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/community/events/community_updated_event.py` & `swibots-1.2.9/swibots/api/community/events/group_deleted_event.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class CommunityUpdatedEvent(CommunityEvent["CommunityUpdatedEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_UPDATE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class GroupDeletedEvent(CommunityEvent["GroupDeletedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_GROUP_DELETE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.2.8/swibots/api/community/events/member_left_event.py` & `swibots-1.2.9/swibots/api/community/events/community_updated_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Optional
-import swibots
-from .community_event import CommunityEvent
-from swibots.api.community.models.channel import Channel
-from swibots.api.community.models.community import Community
-from swibots.api.community.models.group import Group
-from swibots.api.common.models.user import User
-from swibots.types import EventType
-
-
-class MemberLeftEvent(CommunityEvent["MemberLeftEvent"]):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        community_id: Optional[str] = None,
-        community: Optional[Community] = None,
-        group_id: Optional[str] = None,
-        group: Optional[Group] = None,
-        channel_id: Optional[str] = None,
-        channel: Optional[Channel] = None,
-        action_by_id: Optional[str] = None,
-        action_by: Optional[User] = None,
-        data: Optional[dict] = None,
-        user_id: Optional[str] = None,
-        user: Optional[User] = None,
-    ):
-        super().__init__(
-            app=app,
-            type=EventType.COMMUNITY_MEMBER_LEAVE,
-            data=data,
-            action_by=action_by,
-            action_by_id=action_by_id,
-            community=community,
-            community_id=community_id,
-            group=group,
-            group_id=group_id,
-            channel=channel,
-            channel_id=channel_id,
-            user=user,
-            user_id=user_id,
-        )
+from typing import Optional
+import swibots
+from .community_event import CommunityEvent
+from swibots.api.community.models.channel import Channel
+from swibots.api.community.models.community import Community
+from swibots.api.community.models.group import Group
+from swibots.api.common.models.user import User
+from swibots.types import EventType
+
+
+class CommunityUpdatedEvent(CommunityEvent["CommunityUpdatedEvent"]):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        community_id: Optional[str] = None,
+        community: Optional[Community] = None,
+        group_id: Optional[str] = None,
+        group: Optional[Group] = None,
+        channel_id: Optional[str] = None,
+        channel: Optional[Channel] = None,
+        action_by_id: Optional[str] = None,
+        action_by: Optional[User] = None,
+        data: Optional[dict] = None,
+        user_id: Optional[str] = None,
+        user: Optional[User] = None,
+    ):
+        super().__init__(
+            app=app,
+            type=EventType.COMMUNITY_UPDATE,
+            data=data,
+            action_by=action_by,
+            action_by_id=action_by_id,
+            community=community,
+            community_id=community_id,
+            group=group,
+            group_id=group_id,
+            channel=channel,
+            channel_id=channel_id,
+            user=user,
+            user_id=user_id,
+        )
```

### Comparing `swibots-1.2.8/swibots/api/community/methods/get_group.py` & `swibots-1.2.9/swibots/api/community/methods/get_group.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import swibots
-
-from swibots.api.community.models import Group
-
-
-class GetGroup:
-    async def get_group(self: "swibots.ApiClient", id: str) -> Group:
-        """Get a community by its ID
-
-        Args:
-            id (`str`): The ID of the group
-
-        Returns:
-            :obj:`swibots.api.community.models.Group`: The group object.
-
-        Raises:
-            :obj:`switch.error.SwitchError`: If the group could not be retrieved
-
-        This method does the same as :meth:`switch.api.community.controllers.GroupController.get_group`.
-        """
-        return await self.community_service.groups.get_group(id)
+import swibots
+
+from swibots.api.community.models import Group
+
+
+class GetGroup:
+    async def get_group(self: "swibots.ApiClient", id: str) -> Group:
+        """Get a community by its ID
+
+        Args:
+            id (`str`): The ID of the group
+
+        Returns:
+            :obj:`swibots.api.community.models.Group`: The group object.
+
+        Raises:
+            :obj:`switch.error.SwitchError`: If the group could not be retrieved
+
+        This method does the same as :meth:`switch.api.community.controllers.GroupController.get_group`.
+        """
+        return await self.community_service.groups.get_group(id)
```

### Comparing `swibots-1.2.8/swibots/api/community/models/channel.py` & `swibots-1.2.9/swibots/api/community/models/channel.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-from typing import Optional
-from swibots.utils.types import JSONDict
-from swibots.base.switch_object import SwitchObject
-import swibots
-
-class Channel(SwitchObject):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        id: Optional[str] = None,
-        name: Optional[str] = None,
-        community_id: Optional[str] = None,
-        enabled_free: Optional[bool] = None,
-        enabled_public: Optional[bool] = None,
-        default_channel: Optional[bool] = None,
-        is_public: Optional[bool] = None,
-        created_by: Optional[str] = None,
-        icon: Optional[str] = None,
-        channel_logo_url: Optional[str] = None,
-        allowed_content: Optional[str] = None,
-        created_at: Optional[str] = None,
-        updated_at: Optional[str] = None,
-    ):
-        super().__init__(app)
-        self.id = id
-        self.name = name
-        self.community_id = community_id
-        self.enabled_free = enabled_free
-        self.enabled_public = enabled_public
-        self.default_channel = default_channel
-        self.is_public = is_public
-        self.created_by = created_by
-        self.icon = icon
-        self.channel_logo_url = channel_logo_url
-        self.allowed_content = allowed_content
-        self.created_at = created_at
-        self.updated_at = updated_at
-
-    def to_json(self) -> JSONDict:
-        return {
-            "channelId": self.id,
-            "channelName": self.name,
-            "communityId": self.community_id,
-            "enabledFree": self.enabled_free,
-            "enabledPublic": self.enabled_public,
-            "defaultChannel": self.default_channel,
-            "isPublic": self.is_public,
-            "createdBy": self.created_by,
-            "icon": self.icon,
-            "channelLogoUrl": self.channel_logo_url,
-            "allowedContent": self.allowed_content,
-            "createdAt": self.created_at,
-            "updatedAt": self.updated_at,
-        }
-
-    def from_json(self, data: JSONDict) -> "Channel":
-        if data is not None:
-            self.id = data.get("channelId")
-            self.name = data.get("channelName")
-            self.community_id = data.get("communityId")
-            self.enabled_free = data.get("enabledFree")
-            self.enabled_public = data.get("enabledPublic")
-            self.default_channel = data.get("defaultChannel")
-            self.is_public = data.get("isPublic")
-            self.created_by = data.get("createdBy")
-            self.icon = data.get("icon")
-            self.channel_logo_url = data.get("channelLogoUrl")
-            self.allowed_content = data.get("allowedContent")
-            self.created_at = data.get("createdAt")
-            self.updated_at = data.get("updatedAt")
-        return self
+from typing import Optional
+from swibots.utils.types import JSONDict
+from swibots.base.switch_object import SwitchObject
+import swibots
+
+class Channel(SwitchObject):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        id: Optional[str] = None,
+        name: Optional[str] = None,
+        community_id: Optional[str] = None,
+        enabled_free: Optional[bool] = None,
+        enabled_public: Optional[bool] = None,
+        default_channel: Optional[bool] = None,
+        is_public: Optional[bool] = None,
+        created_by: Optional[str] = None,
+        icon: Optional[str] = None,
+        channel_logo_url: Optional[str] = None,
+        allowed_content: Optional[str] = None,
+        created_at: Optional[str] = None,
+        updated_at: Optional[str] = None,
+    ):
+        super().__init__(app)
+        self.id = id
+        self.name = name
+        self.community_id = community_id
+        self.enabled_free = enabled_free
+        self.enabled_public = enabled_public
+        self.default_channel = default_channel
+        self.is_public = is_public
+        self.created_by = created_by
+        self.icon = icon
+        self.channel_logo_url = channel_logo_url
+        self.allowed_content = allowed_content
+        self.created_at = created_at
+        self.updated_at = updated_at
+
+    def to_json(self) -> JSONDict:
+        return {
+            "channelId": self.id,
+            "channelName": self.name,
+            "communityId": self.community_id,
+            "enabledFree": self.enabled_free,
+            "enabledPublic": self.enabled_public,
+            "defaultChannel": self.default_channel,
+            "isPublic": self.is_public,
+            "createdBy": self.created_by,
+            "icon": self.icon,
+            "channelLogoUrl": self.channel_logo_url,
+            "allowedContent": self.allowed_content,
+            "createdAt": self.created_at,
+            "updatedAt": self.updated_at,
+        }
+
+    def from_json(self, data: JSONDict) -> "Channel":
+        if data is not None:
+            self.id = data.get("channelId")
+            self.name = data.get("channelName")
+            self.community_id = data.get("communityId")
+            self.enabled_free = data.get("enabledFree")
+            self.enabled_public = data.get("enabledPublic")
+            self.default_channel = data.get("defaultChannel")
+            self.is_public = data.get("isPublic")
+            self.created_by = data.get("createdBy")
+            self.icon = data.get("icon")
+            self.channel_logo_url = data.get("channelLogoUrl")
+            self.allowed_content = data.get("allowedContent")
+            self.created_at = data.get("createdAt")
+            self.updated_at = data.get("updatedAt")
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/community/models/community.py` & `swibots-1.2.9/swibots/api/community/models/community.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-from typing import Optional
-from swibots.utils.types import JSONDict
-from swibots.base.switch_object import SwitchObject
-import swibots
-
-class Community(SwitchObject):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        id: Optional[str] = None,
-        name: Optional[str] = None,
-        username: Optional[str] = None,
-        profile_url: Optional[str] = None,
-        cover_url: Optional[str] = None,
-        is_public: Optional[bool] = None,
-        is_free: Optional[bool] = None,
-        created_by: Optional[str] = None,
-        guidelines: Optional[str] = None,
-        description: Optional[str] = None,
-        verified: Optional[bool] = None,
-        category: Optional[str] = None,
-        type: Optional[str] = None,
-        link: Optional[str] = None,
-        icon: Optional[str] = None,
-    ):
-        super().__init__(app)
-        self.id = id
-        self.name = name
-        self.username = username
-        self.profile_url = profile_url
-        self.cover_url = cover_url
-        self.is_public = is_public
-        self.is_free = is_free
-        self.created_by = created_by
-        self.guidelines = guidelines
-        self.description = description
-        self.verified = verified
-        self.category = category
-        self.type = type
-        self.link = link
-        self.icon = icon
-
-    def to_json(self) -> JSONDict:
-        return {
-            "communityId": self.id,
-            "communityName": self.name,
-            "communityUsername": self.username,
-            "communityProfileUrl": self.profile_url,
-            "communityCoverUrl": self.cover_url,
-            "isPublic": self.is_public,
-            "isFree": self.is_free,
-            "createdBy": self.created_by,
-            "communityGuidelines": self.guidelines,
-            "communityDescription": self.description,
-            "verified": self.verified,
-            "communityCategory": self.category,
-            "communityType": self.type,
-            "link": self.link,
-            "icon": self.icon,
-        }
-
-    def from_json(self, data: Optional[JSONDict]) -> Optional["Community"]:
-        if data is not None:
-            self.id = data.get("communityId")
-            self.name = data.get("communityName")
-            self.username = data.get("communityUsername")
-            self.profile_url = data.get("communityProfileUrl")
-            self.cover_url = data.get("communityCoverUrl")
-            self.is_public = data.get("isPublic")
-            self.is_free = data.get("isFree")
-            self.created_by = data.get("createdBy")
-            self.guidelines = data.get("communityGuidelines")
-            self.description = data.get("communityDescription")
-            self.verified = data.get("verified")
-            self.category = data.get("communityCategory")
-            self.type = data.get("communityType")
-            self.link = data.get("link")
-            self.icon = data.get("icon")
-        return self
+from typing import Optional
+from swibots.utils.types import JSONDict
+from swibots.base.switch_object import SwitchObject
+import swibots
+
+class Community(SwitchObject):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        id: Optional[str] = None,
+        name: Optional[str] = None,
+        username: Optional[str] = None,
+        profile_url: Optional[str] = None,
+        cover_url: Optional[str] = None,
+        is_public: Optional[bool] = None,
+        is_free: Optional[bool] = None,
+        created_by: Optional[str] = None,
+        guidelines: Optional[str] = None,
+        description: Optional[str] = None,
+        verified: Optional[bool] = None,
+        category: Optional[str] = None,
+        type: Optional[str] = None,
+        link: Optional[str] = None,
+        icon: Optional[str] = None,
+    ):
+        super().__init__(app)
+        self.id = id
+        self.name = name
+        self.username = username
+        self.profile_url = profile_url
+        self.cover_url = cover_url
+        self.is_public = is_public
+        self.is_free = is_free
+        self.created_by = created_by
+        self.guidelines = guidelines
+        self.description = description
+        self.verified = verified
+        self.category = category
+        self.type = type
+        self.link = link
+        self.icon = icon
+
+    def to_json(self) -> JSONDict:
+        return {
+            "communityId": self.id,
+            "communityName": self.name,
+            "communityUsername": self.username,
+            "communityProfileUrl": self.profile_url,
+            "communityCoverUrl": self.cover_url,
+            "isPublic": self.is_public,
+            "isFree": self.is_free,
+            "createdBy": self.created_by,
+            "communityGuidelines": self.guidelines,
+            "communityDescription": self.description,
+            "verified": self.verified,
+            "communityCategory": self.category,
+            "communityType": self.type,
+            "link": self.link,
+            "icon": self.icon,
+        }
+
+    def from_json(self, data: Optional[JSONDict]) -> Optional["Community"]:
+        if data is not None:
+            self.id = data.get("communityId")
+            self.name = data.get("communityName")
+            self.username = data.get("communityUsername")
+            self.profile_url = data.get("communityProfileUrl")
+            self.cover_url = data.get("communityCoverUrl")
+            self.is_public = data.get("isPublic")
+            self.is_free = data.get("isFree")
+            self.created_by = data.get("createdBy")
+            self.guidelines = data.get("communityGuidelines")
+            self.description = data.get("communityDescription")
+            self.verified = data.get("verified")
+            self.category = data.get("communityCategory")
+            self.type = data.get("communityType")
+            self.link = data.get("link")
+            self.icon = data.get("icon")
+        return self
```

### Comparing `swibots-1.2.8/swibots/api/community/models/group.py` & `swibots-1.2.9/swibots/api/community/models/group.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from typing import Optional
-from swibots.utils.types import JSONDict
-from swibots.base.switch_object import SwitchObject
-import swibots
-
-class Group(SwitchObject):
-    def __init__(
-        self,
-        app: "swibots.App" = None,
-        id: Optional[str] = None,
-        name: Optional[str] = None,
-        community_id: Optional[str] = None,
-        enabled_free: Optional[bool] = None,
-        enabled_public: Optional[bool] = None,
-        default_group: Optional[bool] = None,
-        is_public: Optional[bool] = None,
-        created_by: Optional[str] = None,
-        icon: Optional[str] = None,
-        group_logo_url: Optional[str] = None,
-        allowed_content: Optional[str] = None,
-        created_at: Optional[str] = None,
-        updated_at: Optional[str] = None,
-    ):
-        super().__init__(app)
-        self.id = id
-        self.name = name
-        self.community_id = community_id
-        self.enabled_free = enabled_free
-        self.enabled_public = enabled_public
-        self.default_group = default_group
-        self.is_public = is_public
-        self.created_by = created_by
-        self.icon = icon
-        self.group_logo_url = group_logo_url
-        self.allowed_content = allowed_content
-        self.created_at = created_at
-        self.updated_at = updated_at
-
-    def to_json(self) -> JSONDict:
-        return {
-            "groupId": self.id,
-            "groupName": self.name,
-            "communityId": self.community_id,
-            "enabledFree": self.enabled_free,
-            "enabledPublic": self.enabled_public,
-            "defaultGroup": self.default_group,
-            "isPublic": self.is_public,
-            "createdBy": self.created_by,
-            "icon": self.icon,
-            "groupLogoUrl": self.group_logo_url,
-            "allowedContent": self.allowed_content,
-            "createdAt": self.created_at,
-            "updatedAt": self.updated_at,
-        }
-
-    @classmethod
-    def from_json(self, data: JSONDict) -> "Group":
-        if data is not None:
-            self.id = data.get("groupId")
-            self.name = data.get("groupName")
-            self.community_id = data.get("communityId")
-            self.enabled_free = data.get("enabledFree")
-            self.enabled_public = data.get("enabledPublic")
-            self.default_group = data.get("defaultGroup")
-            self.is_public = data.get("isPublic")
-            self.created_by = data.get("createdBy")
-            self.icon = data.get("icon")
-            self.group_logo_url = data.get("groupLogoUrl")
-            self.allowed_content = data.get("allowedContent")
-            self.created_at = data.get("createdAt")
-            self.updated_at = data.get("updatedAt")
-        return self
+from typing import Optional
+from swibots.utils.types import JSONDict
+from swibots.base.switch_object import SwitchObject
+import swibots
+
+class Group(SwitchObject):
+    def __init__(
+        self,
+        app: "swibots.App" = None,
+        id: Optional[str] = None,
+        name: Optional[str] = None,
+        community_id: Optional[str] = None,
+        enabled_free: Optional[bool] = None,
+        enabled_public: Optional[bool] = None,
+        default_group: Optional[bool] = None,
+        is_public: Optional[bool] = None,
+        created_by: Optional[str] = None,
+        icon: Optional[str] = None,
+        group_logo_url: Optional[str] = None,
+        allowed_content: Optional[str] = None,
+        created_at: Optional[str] = None,
+        updated_at: Optional[str] = None,
+    ):
+        super().__init__(app)
+        self.id = id
+        self.name = name
+        self.community_id = community_id
+        self.enabled_free = enabled_free
+        self.enabled_public = enabled_public
+        self.default_group = default_group
+        self.is_public = is_public
+        self.created_by = created_by
+        self.icon = icon
+        self.group_logo_url = group_logo_url
+        self.allowed_content = allowed_content
+        self.created_at = created_at
+        self.updated_at = updated_at
+
+    def to_json(self) -> JSONDict:
+        return {
+            "groupId": self.id,
+            "groupName": self.name,
+            "communityId": self.community_id,
+            "enabledFree": self.enabled_free,
+            "enabledPublic": self.enabled_public,
+            "defaultGroup": self.default_group,
+            "isPublic": self.is_public,
+            "createdBy": self.created_by,
+            "icon": self.icon,
+            "groupLogoUrl": self.group_logo_url,
+            "allowedContent": self.allowed_content,
+            "createdAt": self.created_at,
+            "updatedAt": self.updated_at,
+        }
+
+    @classmethod
+    def from_json(self, data: JSONDict) -> "Group":
+        if data is not None:
+            self.id = data.get("groupId")
+            self.name = data.get("groupName")
+            self.community_id = data.get("communityId")
+            self.enabled_free = data.get("enabledFree")
+            self.enabled_public = data.get("enabledPublic")
+            self.default_group = data.get("defaultGroup")
+            self.is_public = data.get("isPublic")
+            self.created_by = data.get("createdBy")
+            self.icon = data.get("icon")
+            self.group_logo_url = data.get("groupLogoUrl")
+            self.allowed_content = data.get("allowedContent")
+            self.created_at = data.get("createdAt")
+            self.updated_at = data.get("updatedAt")
+        return self
```

### Comparing `swibots-1.2.8/swibots/app.py` & `swibots-1.2.9/swibots/app.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-import asyncio
-from contextlib import AbstractContextManager
-from io import BytesIO
-import logging
-import mimetypes
-import os
-import re
-import shutil
-import signal
-from signal import signal as signal_fn, SIGINT, SIGTERM, SIGABRT
-from typing import Callable, Optional
-import swibots
-from swibots.api import ApiClient
-from swibots.api.auth.models import AuthUser
-from swibots.error import CancelError, SwitchError
-from swibots.utils import RestClient, DownloadProgressCallback, UploadProgress, DownloadProgress, IOClient, ReadCallbackStream
-import httpx
-
-log = logging.getLogger(__name__)
-
-# Signal number to name
-signals = {
-    k: v for v, k in signal.__dict__.items() if v.startswith("SIG") and not v.startswith("SIG_")
-}
-
-
-class App(AbstractContextManager, ApiClient):
-    def __init__(
-        self,
-        # username: Optional[str] = None,
-        # password: Optional[str] = None,
-        token: Optional[str] = None,
-        loop: asyncio.AbstractEventLoop = None,
-    ):
-        """Initialize the client"""
-        super().__init__()
-        self.token = token
-        self._loop = loop or asyncio.get_event_loop()
-        self._running = False
-        self._user_type = AuthUser
-        self.on_community_service_start: Callable = None
-        self.on_chat_service_start: Callable = None
-        self.on_app_stop: Callable = None
-        self.on_app_start: Callable = None
-        self.rest_client = RestClient()
-
-    async def handle_upload(self, url, file_name, data=None, file_field="file", progress=None,  progress_args: tuple = ()):
-        dProgress = UploadProgress(
-            current=0,
-            readed=0,
-            file_name=file_name,
-            client=IOClient(),
-            url=file_name,
-            callback=progress,
-            callback_args=progress_args
-        )
-        file = open(file_name, "rb")
-        reader = ReadCallbackStream(
-            file, dProgress.update
-        )
-        mime = mimetypes.guess_type(file_name)[0] or "application/octet-stream"
-        try:
-            r = await self.rest_client._client.post(url, files={file_field: (file_name, reader, mime)}, data=data, headers={"Authorization": f"Bearer {self.token}"})
-            return r.json()
-        except CancelError:
-            pass
-
-    async def handle_download(self, url: str, file_name: str, directory="downloads/", in_memory: bool = False, block: bool = True, progress: DownloadProgressCallback = None, progress_args: tuple = ()):
-        if directory is None or directory == "":
-            directory = "downloads/"
-        os.makedirs(directory, exist_ok=True) if not in_memory else None
-        temp_file_path = os.path.abspath(
-            re.sub("\\\\", "/", os.path.join(directory, file_name))) + ".temp"
-        file = BytesIO() if in_memory else open(temp_file_path, "wb")
-
-        dProgress = DownloadProgress(
-            total=0,
-            downloaded=0,
-            file_name=file_name,
-            client=IOClient(),
-            url=url,
-        )
-
-        if (progress):
-            await progress(dProgress, *progress_args)
-
-        try:
-            with httpx.stream("GET", url) as response:
-                dProgress.total = int(response.headers["Content-Length"])
-                dProgress.downloaded = response.num_bytes_downloaded
-                dProgress.client = response
-                dProgress.started = True
-                for chunk in response.iter_bytes():
-                    file.write(chunk)
-                    dProgress.downloaded += len(chunk)
-                    if progress:
-                        await progress(dProgress, *progress_args)
-
-        except BaseException as e:
-            if not in_memory:
-                file.close()
-                os.remove(temp_file_path)
-            if isinstance(e, CancelError):
-                return None
-            if isinstance(e, asyncio.CancelledError):
-                raise e
-
-            return None
-        else:
-            if in_memory:
-                file.name = file_name
-                return file
-            else:
-                file.close()
-                file_path = os.path.splitext(temp_file_path)[0]
-                shutil.move(temp_file_path, file_path)
-                return file_path
-
-        # file_id, directory, file_name, in_memory, file_size, progress, progress_args = packet
-
-        # os.makedirs(directory, exist_ok=True) if not in_memory else None
-        # temp_file_path = os.path.abspath(re.sub("\\\\", "/", os.path.join(directory, file_name))) + ".temp"
-        # file = BytesIO() if in_memory else open(temp_file_path, "wb")
-
-        # try:
-        #     async for chunk in self.get_file(file_id, file_size, 0, 0, progress, progress_args):
-        #         file.write(chunk)
-        # except BaseException as e:
-        #     if not in_memory:
-        #         file.close()
-        #         os.remove(temp_file_path)
-
-        #     if isinstance(e, asyncio.CancelledError):
-        #         raise e
-
-        #     return None
-        # else:
-        #     if in_memory:
-        #         file.name = file_name
-        #         return file
-        #     else:
-        #         file.close()
-        #         file_path = os.path.splitext(temp_file_path)[0]
-        #         shutil.move(temp_file_path, file_path)
-        #         return file_path
-
-    async def _validate_credentials(self):
-        if self.token is not None:
-            return await self._validate_token()
-        if self.username is None or self.password is None:
-            raise SwitchError(
-                "Username and password are required when token is not set")
-        user = await self.login(user_type=self._user_type)
-        self.user = user
-
-    async def _validate_token(self):
-        # check if token is valid
-        if self.token is None:
-            raise SwitchError("Token is not set")
-
-        try:
-            log.debug("checking token...")
-            user = await self.get_me(user_type=self._user_type)
-            self.user = user
-            log.info("Logged in as [%s][%d]", user.user_name, user.id)
-        except Exception as e:
-            log.exception(e)
-            await self.stop()
-            raise SwitchError("Invalid token")
-
-        if self.user is None:
-            raise SwitchError("Invalid token")
-
-    async def _validate_run(self):
-        await self._validate_credentials()
-
-    async def _on_app_stop(self):
-        await self.chat_service.stop()
-        await self.community_service.stop()
-        if self.on_app_stop is not None:
-            await self.on_app_stop(self)
-
-    async def _on_app_start(self):
-        if self.on_app_start is not None:
-            await self.on_app_start(self)
-
-    async def start(self):
-        try:
-            if self._running:
-                raise SwitchError("App is already running")
-            self._running = True
-            """Starts the app"""
-            log.info("🚀 Starting app...")
-
-            await self._validate_run()
-
-            try:
-                await (self.chat_service.start())
-                if self.on_chat_service_start is not None:
-                    await self.on_chat_service_start(self)
-            except Exception as e:
-                log.exception(e)
-
-            try:
-                await (self.community_service.start())
-                if self.on_community_service_start is not None:
-                    await self.on_community_service_start(self)
-            except Exception as e:
-                log.exception(e)
-
-            await self._on_app_start()
-
-            log.info("🚀 App started!")
-
-            # # run forever
-            # while self._running:
-            #     await asyncio.sleep(1)
-        except asyncio.CancelledError:
-            self._running = False
-            # await self._do_stop()
-
-    async def _do_stop(self):
-        log.info("🛑 Stopping app...")
-        await self._on_app_stop()
-        self._running = False
-
-    async def stop(self):
-        if not self._running:
-            return
-        await self._do_stop()
-
-    def __enter__(self):
-        return self.start()
-
-    def __exit__(self, *args):
-        try:
-            self.stop()
-        except ConnectionError:
-            pass
-
-    async def __aenter__(self):
-        return await self.start()
-
-    async def __aexit__(self, *args):
-        try:
-            await self.stop()
-        except ConnectionError:
-            pass
-
-    async def idle(self):
-        task = None
-
-        def signal_handler(signum, __):
-            logging.info(
-                f"Stop signal received ({signals[signum]}). Exiting...")
-            task.cancel()
-
-        for s in (SIGINT, SIGTERM, SIGABRT):
-            signal_fn(s, signal_handler)
-
-        while True:
-            task = asyncio.create_task(asyncio.sleep(600))
-
-            try:
-                await task
-            except asyncio.CancelledError:
-                break
-
-    def run(self, task: Callable = None):
-        loop = asyncio.get_event_loop()
-        run = loop.run_until_complete
-        if task is not None:
-            run(task)
-        else:
-            try:
-                run(self.start())
-                run(self.idle())
-                run(self.stop())
-            except KeyboardInterrupt:
-                run(self.stop())
-            except Exception as e:
-                log.exception(e)
-                run(self.stop())
+import asyncio
+from contextlib import AbstractContextManager
+from io import BytesIO
+import logging
+import mimetypes
+import os
+import re
+import shutil
+import signal
+from signal import signal as signal_fn, SIGINT, SIGTERM, SIGABRT
+from typing import Callable, Optional
+import swibots
+from swibots.api import ApiClient
+from swibots.api.auth.models import AuthUser
+from swibots.error import CancelError, SwitchError
+from swibots.utils import RestClient, DownloadProgressCallback, UploadProgress, DownloadProgress, IOClient, ReadCallbackStream
+import httpx
+
+log = logging.getLogger(__name__)
+
+# Signal number to name
+signals = {
+    k: v for v, k in signal.__dict__.items() if v.startswith("SIG") and not v.startswith("SIG_")
+}
+
+
+class App(AbstractContextManager, ApiClient):
+    def __init__(
+        self,
+        # username: Optional[str] = None,
+        # password: Optional[str] = None,
+        token: Optional[str] = None,
+        loop: asyncio.AbstractEventLoop = None,
+    ):
+        """Initialize the client"""
+        super().__init__()
+        self.token = token
+        self._loop = loop or asyncio.get_event_loop()
+        self._running = False
+        self._user_type = AuthUser
+        self.on_community_service_start: Callable = None
+        self.on_chat_service_start: Callable = None
+        self.on_app_stop: Callable = None
+        self.on_app_start: Callable = None
+        self.rest_client = RestClient()
+
+    async def handle_upload(self, url, file_name, data=None, file_field="file", progress=None,  progress_args: tuple = ()):
+        dProgress = UploadProgress(
+            current=0,
+            readed=0,
+            file_name=file_name,
+            client=IOClient(),
+            url=file_name,
+            callback=progress,
+            callback_args=progress_args
+        )
+        file = open(file_name, "rb")
+        reader = ReadCallbackStream(
+            file, dProgress.update
+        )
+        mime = mimetypes.guess_type(file_name)[0] or "application/octet-stream"
+        try:
+            r = await self.rest_client._client.post(url, files={file_field: (file_name, reader, mime)}, data=data, headers={"Authorization": f"Bearer {self.token}"})
+            return r.json()
+        except CancelError:
+            pass
+
+    async def handle_download(self, url: str, file_name: str, directory="downloads/", in_memory: bool = False, block: bool = True, progress: DownloadProgressCallback = None, progress_args: tuple = ()):
+        if directory is None or directory == "":
+            directory = "downloads/"
+        os.makedirs(directory, exist_ok=True) if not in_memory else None
+        temp_file_path = os.path.abspath(
+            re.sub("\\\\", "/", os.path.join(directory, file_name))) + ".temp"
+        file = BytesIO() if in_memory else open(temp_file_path, "wb")
+
+        dProgress = DownloadProgress(
+            total=0,
+            downloaded=0,
+            file_name=file_name,
+            client=IOClient(),
+            url=url,
+        )
+
+        if (progress):
+            await progress(dProgress, *progress_args)
+
+        try:
+            with httpx.stream("GET", url) as response:
+                dProgress.total = int(response.headers["Content-Length"])
+                dProgress.downloaded = response.num_bytes_downloaded
+                dProgress.client = response
+                dProgress.started = True
+                for chunk in response.iter_bytes():
+                    file.write(chunk)
+                    dProgress.downloaded += len(chunk)
+                    if progress:
+                        await progress(dProgress, *progress_args)
+
+        except BaseException as e:
+            if not in_memory:
+                file.close()
+                os.remove(temp_file_path)
+            if isinstance(e, CancelError):
+                return None
+            if isinstance(e, asyncio.CancelledError):
+                raise e
+
+            return None
+        else:
+            if in_memory:
+                file.name = file_name
+                return file
+            else:
+                file.close()
+                file_path = os.path.splitext(temp_file_path)[0]
+                shutil.move(temp_file_path, file_path)
+                return file_path
+
+        # file_id, directory, file_name, in_memory, file_size, progress, progress_args = packet
+
+        # os.makedirs(directory, exist_ok=True) if not in_memory else None
+        # temp_file_path = os.path.abspath(re.sub("\\\\", "/", os.path.join(directory, file_name))) + ".temp"
+        # file = BytesIO() if in_memory else open(temp_file_path, "wb")
+
+        # try:
+        #     async for chunk in self.get_file(file_id, file_size, 0, 0, progress, progress_args):
+        #         file.write(chunk)
+        # except BaseException as e:
+        #     if not in_memory:
+        #         file.close()
+        #         os.remove(temp_file_path)
+
+        #     if isinstance(e, asyncio.CancelledError):
+        #         raise e
+
+        #     return None
+        # else:
+        #     if in_memory:
+        #         file.name = file_name
+        #         return file
+        #     else:
+        #         file.close()
+        #         file_path = os.path.splitext(temp_file_path)[0]
+        #         shutil.move(temp_file_path, file_path)
+        #         return file_path
+
+    async def _validate_credentials(self):
+        if self.token is not None:
+            return await self._validate_token()
+        if self.username is None or self.password is None:
+            raise SwitchError(
+                "Username and password are required when token is not set")
+        user = await self.login(user_type=self._user_type)
+        self.user = user
+
+    async def _validate_token(self):
+        # check if token is valid
+        if self.token is None:
+            raise SwitchError("Token is not set")
+
+        try:
+            log.debug("checking token...")
+            user = await self.get_me(user_type=self._user_type)
+            self.user = user
+            log.info("Logged in as [%s][%d]", user.user_name, user.id)
+        except Exception as e:
+            log.exception(e)
+            await self.stop()
+            raise SwitchError("Invalid token")
+
+        if self.user is None:
+            raise SwitchError("Invalid token")
+
+    async def _validate_run(self):
+        await self._validate_credentials()
+
+    async def _on_app_stop(self):
+        await self.chat_service.stop()
+        await self.community_service.stop()
+        if self.on_app_stop is not None:
+            await self.on_app_stop(self)
+
+    async def _on_app_start(self):
+        if self.on_app_start is not None:
+            await self.on_app_start(self)
+
+    async def start(self):
+        try:
+            if self._running:
+                raise SwitchError("App is already running")
+            self._running = True
+            """Starts the app"""
+            log.info("🚀 Starting app...")
+
+            await self._validate_run()
+
+            try:
+                await (self.chat_service.start())
+                if self.on_chat_service_start is not None:
+                    await self.on_chat_service_start(self)
+            except Exception as e:
+                log.exception(e)
+
+            try:
+                await (self.community_service.start())
+                if self.on_community_service_start is not None:
+                    await self.on_community_service_start(self)
+            except Exception as e:
+                log.exception(e)
+
+            await self._on_app_start()
+
+            log.info("🚀 App started!")
+
+            # # run forever
+            # while self._running:
+            #     await asyncio.sleep(1)
+        except asyncio.CancelledError:
+            self._running = False
+            # await self._do_stop()
+
+    async def _do_stop(self):
+        log.info("🛑 Stopping app...")
+        await self._on_app_stop()
+        self._running = False
+
+    async def stop(self):
+        if not self._running:
+            return
+        await self._do_stop()
+
+    def __enter__(self):
+        return self.start()
+
+    def __exit__(self, *args):
+        try:
+            self.stop()
+        except ConnectionError:
+            pass
+
+    async def __aenter__(self):
+        return await self.start()
+
+    async def __aexit__(self, *args):
+        try:
+            await self.stop()
+        except ConnectionError:
+            pass
+
+    async def idle(self):
+        task = None
+
+        def signal_handler(signum, __):
+            logging.info(
+                f"Stop signal received ({signals[signum]}). Exiting...")
+            task.cancel()
+
+        for s in (SIGINT, SIGTERM, SIGABRT):
+            signal_fn(s, signal_handler)
+
+        while True:
+            task = asyncio.create_task(asyncio.sleep(600))
+
+            try:
+                await task
+            except asyncio.CancelledError:
+                break
+
+    def run(self, task: Callable = None):
+        loop = asyncio.get_event_loop()
+        run = loop.run_until_complete
+        if task is not None:
+            run(task)
+        else:
+            try:
+                run(self.start())
+                run(self.idle())
+                run(self.stop())
+            except KeyboardInterrupt:
+                run(self.stop())
+            except Exception as e:
+                log.exception(e)
+                run(self.stop())
```

### Comparing `swibots-1.2.8/swibots/base/rest_response.py` & `swibots-1.2.9/swibots/base/rest_response.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import Generic, TypeVar
-from http.client import responses
-
-from swibots.utils.types import RequestMethod
-
-
-T = TypeVar("T")
-
-
-class RestResponse(Generic[T]):
-    def __init__(self, data: T, status_code: int, headers: dict):
-        self.data = data
-        self.status_code = status_code
-        self.headers = headers
-
-    @property
-    def is_error(self) -> bool:
-        return self.status_code >= 400
-
-    @property
-    def error_message(self) -> str:
-        err = (
-            self.data if self.data is not None and self.data != "" else responses[self.status_code]
-        )
-        return f"Error {self.status_code}: {err}"
+from typing import Generic, TypeVar
+from http.client import responses
+
+from swibots.utils.types import RequestMethod
+
+
+T = TypeVar("T")
+
+
+class RestResponse(Generic[T]):
+    def __init__(self, data: T, status_code: int, headers: dict):
+        self.data = data
+        self.status_code = status_code
+        self.headers = headers
+
+    @property
+    def is_error(self) -> bool:
+        return self.status_code >= 400
+
+    @property
+    def error_message(self) -> str:
+        err = (
+            self.data if self.data is not None and self.data != "" else responses[self.status_code]
+        )
+        return f"Error {self.status_code}: {err}"
```

### Comparing `swibots-1.2.8/swibots/base/switch_client.py` & `swibots-1.2.9/swibots/base/switch_client.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-import json
-from typing import List, Tuple, Type, TypeVar
-import swibots
-from swibots.error import NetworkError
-from swibots.utils import RestClient
-from swibots.utils.types import JSONDict
-from swibots.base import RestResponse
-
-T = TypeVar("T", bound="swibots.SwitchObject")
-
-
-class SwitchRestClient(RestClient):
-    def __init__(self, app: "swibots.App" = None, base_url: str = None, token: str = None):
-        super().__init__()
-        self._app = app
-        self._auth_token = token
-        self._base_url = base_url
-
-    @property
-    def app(self) -> "swibots.App":
-        return self._app
-
-    @app.setter
-    def app(self, app: "swibots.App"):
-        self._app = app
-
-    @property
-    def token(self):
-        return self._app.token
-
-    @property
-    def user(self) -> "swibots.AuthUser":
-        return self._app.user
-
-    @property
-    def base_url(self, url: str):
-        self._base_url = url
-
-    @base_url.setter
-    def base_url(self, url: str):
-        self._base_url = url
-
-    def build_object(self, obj_type: Type[T],  data: JSONDict) -> T:
-        return obj_type.build_from_json(data, self.app)
-
-    def build_list(self, obj_type: Type[T], data: JSONDict) -> List[T]:
-        return obj_type.build_from_json_list(data, self.app)
-
-    async def get(
-        self, url: str, data: dict = None, headers: dict = None
-    ) -> RestResponse[JSONDict]:
-        """See :meth:`BaseRequest.get`."""
-        return await self.do_request(url, "GET", data, headers=headers)
-
-    async def post(
-        self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None
-    ) -> RestResponse[JSONDict]:
-        """See :meth:`BaseRequest.post`."""
-        return await self.do_request(url, "POST", data, form_data, files, headers)
-
-    async def put(
-        self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None
-    ) -> RestResponse[JSONDict]:
-        """See :meth:`BaseRequest.put`."""
-        return await self.do_request(url, "PUT", data, form_data, files, headers)
-
-    async def delete(
-        self, url: str, data: dict = None, headers: dict = None
-    ) -> RestResponse[JSONDict]:
-        """See :meth:`BaseRequest.delete`."""
-        return await self.do_request(url, "DELETE", data, headers=headers)
-
-    async def patch(
-        self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None
-    ) -> RestResponse[JSONDict]:
-        """See :meth:`BaseRequest.patch`."""
-        return await self.do_request(url, "PATCH", data, form_data, files, headers)
-
-    async def head(
-        self, url: str, data: dict = None, headers: dict = None
-    ) -> RestResponse[JSONDict]:
-        """See :meth:`BaseRequest.head`."""
-        return await self.do_request(url, "HEAD", data, headers)
-
-    async def options(
-        self, url: str, data: dict = None, headers: dict = None
-    ) -> RestResponse[JSONDict]:
-        """See :meth:`BaseRequest.options`."""
-        return await self.do_request(url, "OPTIONS", data, headers)
-
-    def parse_response(self, response: Tuple[int, bytes]) -> RestResponse[JSONDict]:
-        decoded_s = response[1].decode("utf-8", "replace")
-        try:
-            jsonObject = json.loads(decoded_s)
-        except ValueError as exc:
-            jsonObject = decoded_s
-
-        response = RestResponse(jsonObject, response[0], {})
-        if response.is_error:
-            raise NetworkError(response.error_message)
-        return response
-
-    def prepare_request_data(self, data: dict) -> dict:
-        return super().prepare_request_data(data)
-
-    def prepare_request_headers(self, headers: dict) -> dict:
-        headers = super().prepare_request_headers(headers)
-        if self.token is not None:
-            headers["Authorization"] = f"Bearer {self.token}"
-        return headers
-
-    async def do_request(
-        self, path: str, method: str, data: dict = None, form_data=None, files=None, headers: dict = None
-    ) -> RestResponse[JSONDict]:
-        data = self.prepare_request_data(data)
-        headers = self.prepare_request_headers(headers)
-        return self.parse_response(
-            await RestClient.do_request(self, self._base_url + (path if path is not None else ""), method, data, form_data, files, headers)
-        )
+import json
+from typing import List, Tuple, Type, TypeVar
+import swibots
+from swibots.error import NetworkError
+from swibots.utils import RestClient
+from swibots.utils.types import JSONDict
+from swibots.base import RestResponse
+
+T = TypeVar("T", bound="swibots.SwitchObject")
+
+
+class SwitchRestClient(RestClient):
+    def __init__(self, app: "swibots.App" = None, base_url: str = None, token: str = None):
+        super().__init__()
+        self._app = app
+        self._auth_token = token
+        self._base_url = base_url
+
+    @property
+    def app(self) -> "swibots.App":
+        return self._app
+
+    @app.setter
+    def app(self, app: "swibots.App"):
+        self._app = app
+
+    @property
+    def token(self):
+        return self._app.token
+
+    @property
+    def user(self) -> "swibots.AuthUser":
+        return self._app.user
+
+    @property
+    def base_url(self, url: str):
+        self._base_url = url
+
+    @base_url.setter
+    def base_url(self, url: str):
+        self._base_url = url
+
+    def build_object(self, obj_type: Type[T],  data: JSONDict) -> T:
+        return obj_type.build_from_json(data, self.app)
+
+    def build_list(self, obj_type: Type[T], data: JSONDict) -> List[T]:
+        return obj_type.build_from_json_list(data, self.app)
+
+    async def get(
+        self, url: str, data: dict = None, headers: dict = None
+    ) -> RestResponse[JSONDict]:
+        """See :meth:`BaseRequest.get`."""
+        return await self.do_request(url, "GET", data, headers=headers)
+
+    async def post(
+        self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None
+    ) -> RestResponse[JSONDict]:
+        """See :meth:`BaseRequest.post`."""
+        return await self.do_request(url, "POST", data, form_data, files, headers)
+
+    async def put(
+        self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None
+    ) -> RestResponse[JSONDict]:
+        """See :meth:`BaseRequest.put`."""
+        return await self.do_request(url, "PUT", data, form_data, files, headers)
+
+    async def delete(
+        self, url: str, data: dict = None, headers: dict = None
+    ) -> RestResponse[JSONDict]:
+        """See :meth:`BaseRequest.delete`."""
+        return await self.do_request(url, "DELETE", data, headers=headers)
+
+    async def patch(
+        self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None
+    ) -> RestResponse[JSONDict]:
+        """See :meth:`BaseRequest.patch`."""
+        return await self.do_request(url, "PATCH", data, form_data, files, headers)
+
+    async def head(
+        self, url: str, data: dict = None, headers: dict = None
+    ) -> RestResponse[JSONDict]:
+        """See :meth:`BaseRequest.head`."""
+        return await self.do_request(url, "HEAD", data, headers)
+
+    async def options(
+        self, url: str, data: dict = None, headers: dict = None
+    ) -> RestResponse[JSONDict]:
+        """See :meth:`BaseRequest.options`."""
+        return await self.do_request(url, "OPTIONS", data, headers)
+
+    def parse_response(self, response: Tuple[int, bytes]) -> RestResponse[JSONDict]:
+        decoded_s = response[1].decode("utf-8", "replace")
+        try:
+            jsonObject = json.loads(decoded_s)
+        except ValueError as exc:
+            jsonObject = decoded_s
+
+        response = RestResponse(jsonObject, response[0], {})
+        if response.is_error:
+            raise NetworkError(response.error_message)
+        return response
+
+    def prepare_request_data(self, data: dict) -> dict:
+        return super().prepare_request_data(data)
+
+    def prepare_request_headers(self, headers: dict) -> dict:
+        headers = super().prepare_request_headers(headers)
+        if self.token is not None:
+            headers["Authorization"] = f"Bearer {self.token}"
+        return headers
+
+    async def do_request(
+        self, path: str, method: str, data: dict = None, form_data=None, files=None, headers: dict = None
+    ) -> RestResponse[JSONDict]:
+        data = self.prepare_request_data(data)
+        headers = self.prepare_request_headers(headers)
+        return self.parse_response(
+            await RestClient.do_request(self, self._base_url + (path if path is not None else ""), method, data, form_data, files, headers)
+        )
```

### Comparing `swibots-1.2.8/swibots/base/switch_object.py` & `swibots-1.2.9/swibots/base/switch_object.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-from typing import Generic, List, Optional, TypeVar
-import swibots
-from swibots.utils.types import JSONDict
-
-
-T = TypeVar("T")
-
-
-class SwitchObject(Generic[T]):
-    def __init__(self, app:"swibots.App"=None, **kwargs):
-        self._app = app
-        for key, value in kwargs.items():
-            setattr(self, key, value)
-
-    @property
-    def app(self) -> "swibots.App":
-        return self._app
-
-    @classmethod
-    def build_from_json(cls, data: Optional[JSONDict] = None, app: Optional["swibots.App"] = None) -> Optional[T]:
-        if data is None:
-            return None
-        return cls(app).from_json(data)
-
-    @classmethod
-    def build_from_json_list(cls, data: Optional[JSONDict], app: Optional["swibots.App"] = None) -> List[T]:
-        return [cls.build_from_json(item, app) for item in data]
-
-    def to_json_request(self) -> JSONDict:
-        return self.to_json()
-
-    def to_json(self) -> JSONDict:
-        return self.__dict__
-
-    def from_json(self, data: Optional[JSONDict]) -> T:
-        for key, value in data.items():
-            setattr(self, key, value)
-        return self
-
-    def __repr__(self) -> str:
-        return self.to_json().__repr__()
+from typing import Generic, List, Optional, TypeVar
+import swibots
+from swibots.utils.types import JSONDict
+
+
+T = TypeVar("T")
+
+
+class SwitchObject(Generic[T]):
+    def __init__(self, app:"swibots.App"=None, **kwargs):
+        self._app = app
+        for key, value in kwargs.items():
+            setattr(self, key, value)
+
+    @property
+    def app(self) -> "swibots.App":
+        return self._app
+
+    @classmethod
+    def build_from_json(cls, data: Optional[JSONDict] = None, app: Optional["swibots.App"] = None) -> Optional[T]:
+        if data is None:
+            return None
+        return cls(app).from_json(data)
+
+    @classmethod
+    def build_from_json_list(cls, data: Optional[JSONDict], app: Optional["swibots.App"] = None) -> List[T]:
+        return [cls.build_from_json(item, app) for item in data]
+
+    def to_json_request(self) -> JSONDict:
+        return self.to_json()
+
+    def to_json(self) -> JSONDict:
+        return self.__dict__
+
+    def from_json(self, data: Optional[JSONDict]) -> T:
+        for key, value in data.items():
+            setattr(self, key, value)
+        return self
+
+    def __repr__(self) -> str:
+        return self.to_json().__repr__()
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_callback_query.py` & `swibots-1.2.9/swibots/bots/decorators/on_callback_query.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnCallbackQuery:
-    def on_callback_query(
-        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling callback queries."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.CallbackQueryHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnCallbackQuery:
+    def on_callback_query(
+        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
+    ) -> Callable:
+        """Decorator for handling callback queries."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.CallbackQueryHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_channel_deleted.py` & `swibots-1.2.9/swibots/bots/decorators/on_member_left.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnChannelDeleted:
-    def on_channel_created(
-        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling channel creations."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.ChannelDeletedHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnMemberLeft:
+    def on_member_leaft(
+        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
+    ) -> Callable:
+        """Decorator for handling members joins."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.MemberLeftHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_channel_updated.py` & `swibots-1.2.9/swibots/bots/decorators/on_community_updated.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnChannelUpdated:
-    def on_channel_updated(
-        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling channel update."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.ChannelUpdatedHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnCommunityUpdated:
+    def on_community_update(
+        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
+    ) -> Callable:
+        """Decorator for handling new commands."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.CommunityUpdatedHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_command.py` & `swibots-1.2.9/swibots/bots/decorators/on_inline_query.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-from swibots.utils.types import SCT
-
-
-class OnCommand:
-    def on_command(
-        self: "swibots.BotApp", command: SCT[str], filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling new commands."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.CommandHandler(command, func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnInlineQuery:
+    def on_inline_query(self: "swibots.BotApp" = None, filter: Optional[Filter] = None) -> Callable:
+        """Decorator for handling new messages."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(
+                    swibots.bots.handlers.InlineQueryHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_group_created.py` & `swibots-1.2.9/swibots/bots/decorators/on_group_created.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnGroupCreated:
-    def on_group_created(
-        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling group creations."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.GroupCreatedHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnGroupCreated:
+    def on_group_created(
+        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
+    ) -> Callable:
+        """Decorator for handling group creations."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.GroupCreatedHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_group_deleted.py` & `swibots-1.2.9/swibots/bots/decorators/on_command.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnGroupDeleted:
-    def on_group_deleted(
-        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling group deletions."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.GroupDeletedHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+from swibots.utils.types import SCT
+
+
+class OnCommand:
+    def on_command(
+        self: "swibots.BotApp", command: SCT[str], filter: Optional[Filter] = None
+    ) -> Callable:
+        """Decorator for handling new commands."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.CommandHandler(command, func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_group_updated.py` & `swibots-1.2.9/swibots/bots/decorators/on_group_updated.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnGroupUpdated:
-    def on_group_updated(
-        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling group updates."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.GroupUpdatedHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnGroupUpdated:
+    def on_group_updated(
+        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
+    ) -> Callable:
+        """Decorator for handling group updates."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.GroupUpdatedHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_inline_query.py` & `swibots-1.2.9/swibots/bots/decorators/on_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnInlineQuery:
-    def on_inline_query(self: "swibots.BotApp" = None, filter: Optional[Filter] = None) -> Callable:
-        """Decorator for handling new messages."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(
-                    swibots.bots.handlers.InlineQueryHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnMessage:
+    def on_message(self: "swibots.BotApp" = None, filter: Optional[Filter] = None) -> Callable:
+        """Decorator for handling new messages."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.MessageHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_member_joined.py` & `swibots-1.2.9/swibots/bots/decorators/on_unknown_command.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnMemberJoined:
-    def on_member_joined(
-        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling members joins."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.MemberJoinedHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnUnknownCommand:
+    def on_unknown_command(
+        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
+    ) -> Callable:
+        """Decorator for handling unknown commands."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.UnknownCommandHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/decorators/on_member_left.py` & `swibots-1.2.9/swibots/bots/decorators/on_member_joined.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Callable, Optional
-import swibots
-from swibots.bots.filters.filter import Filter
-
-
-class OnMemberLeft:
-    def on_member_leaft(
-        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
-    ) -> Callable:
-        """Decorator for handling members joins."""
-
-        def decorator(func: Callable) -> Callable:
-            if isinstance(self, swibots.BotApp):
-                self.add_handler(swibots.bots.handlers.MemberLeftHandler(func, filter))
-
-            return func
-
-        return decorator
+from typing import Callable, Optional
+import swibots
+from swibots.bots.filters.filter import Filter
+
+
+class OnMemberJoined:
+    def on_member_joined(
+        self: "swibots.BotApp" = None, filter: Optional[Filter] = None
+    ) -> Callable:
+        """Decorator for handling members joins."""
+
+        def decorator(func: Callable) -> Callable:
+            if isinstance(self, swibots.BotApp):
+                self.add_handler(swibots.bots.handlers.MemberJoinedHandler(func, filter))
+
+            return func
+
+        return decorator
```

### Comparing `swibots-1.2.8/swibots/bots/filters/filter.py` & `swibots-1.2.9/swibots/bots/filters/filter.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-import re
-from typing import Optional
-from swibots.api.chat.events import MessageEvent
-from swibots.api.chat.events.chat_event import ChatEvent
-from swibots.api.common.events import Event
-from swibots.bots.bot_context import BotContext
-from swibots.utils.types import SCT, FilterCallback
-from swibots.types import EventType
-from typing import Callable, Union, List, Pattern
-
-
-class Filter:
-    async def __call__(self, ctx: BotContext) -> bool:
-        raise NotImplementedError
-
-    def __invert__(self):
-        return InvertFilter(self)
-
-    def __and__(self, other):
-        return AndFilter(self, other)
-
-    def __or__(self, other):
-        return OrFilter(self, other)
-
-
-class InvertFilter(Filter):
-    def __init__(self, base):
-        self.base = base
-
-    async def __call__(self, ctx: BotContext) -> bool:
-        result = await self.base(ctx)
-        return not result
-
-
-class AndFilter(Filter):
-    def __init__(self, base, other):
-        self.base = base
-        self.other = other
-
-    async def __call__(self, ctx: BotContext) -> bool:
-        r1 = await self.base(ctx)
-        # short circuit
-        if not r1:
-            return False
-        r2 = await self.other(ctx)
-
-        return r1 and r2
-
-
-class OrFilter(Filter):
-    def __init__(self, base, other):
-        self.base = base
-        self.other = other
-
-    async def __call__(self, ctx: BotContext) -> bool:
-        r1 = await self.base(ctx)
-        # short circuit
-        if r1:
-            return True
-
-        return await self.other(ctx)
-
-
-CUSTOM_FILTER_NAME = "CustomFilter"
-
-
-def create(func: FilterCallback, name: str = None, **kwargs) -> Filter:
-    return type(
-        name or func.__name__ or CUSTOM_FILTER_NAME, (Filter,), {
-            "__call__": func, **kwargs}
-    )()
-
-
-async def all_filter(self, ctx: BotContext):
-    return True
-
-
-all = create(all_filter)
-"""Filter all messages."""
-
-
-async def self_filter(self, ctx: BotContext[MessageEvent]):
-    return bool(
-        ctx.event.message is not None
-        and ctx.event.message.user_id == ctx.event.message.receiver_id
-    )
-
-
-self = create(self_filter)
-"""Filter messages generated by the same user."""
-
-
-async def bot_filter(self, ctx: BotContext[MessageEvent]):
-    return bool(
-        ctx.event.message is not None and ctx.event.user is not None and ctx.event.user.is_bot
-    )
-
-
-is_bot = create(bot_filter)
-"""Filter messages coming from bots."""
-
-
-async def me_filter(self, ctx: BotContext[MessageEvent]):
-    return bool(ctx.event.message is not None and ctx.event.message.user_id == ctx.user.id)
-
-
-me = create(me_filter)
-"""Filter messages coming from your user."""
-
-
-async def incoming_filter(self, ctx: BotContext[MessageEvent]):
-    return bool(ctx.event.message is not None and ctx.event.message.receiver_id == ctx.user.id)
-
-
-incoming = create(incoming_filter)
-"""Filter incoming messages. Messages that are sent to the users recipient."""
-
-
-async def outgoing_filter(self, ctx: BotContext[MessageEvent]):
-    return not incoming(ctx)
-
-
-outgoing = create(outgoing_filter)
-"""Filter outgoing messages. Messages that are sent by the user."""
-
-
-class community(Filter, set):
-    """Filter events comming from a specific community or communities"""
-
-    def __init__(self, community_id: Optional[SCT[str]]):
-        community_id = community_id
-
-    async def __call__(self, ctx: BotContext[Event]):
-        community_id = self.community_id
-        if community_id is None:
-            return bool(ctx.event.community_id is not None)
-        if isinstance(community_id, str):
-            community_id = frozenset({community_id})
-        else:
-            community_id = frozenset(community_id)
-        return bool(ctx.event.community_id in community_id)
-
-
-class channel(Filter, set):
-    """Filter events comming from a specific channel or channels"""
-
-    def __init__(self, channel_id: Optional[SCT[str]]):
-        channel_id = channel_id
-
-    async def __call__(self, ctx: BotContext[Event]):
-        channel_id = self.channel_id
-        if channel_id is None:
-            return bool(ctx.event.channel_id is not None)
-        if isinstance(channel_id, str):
-            channel_id = frozenset({channel_id})
-        else:
-            channel_id = frozenset(channel_id)
-        return bool(ctx.event.channel_id in channel_id)
-
-
-class group(Filter, set):
-    def __init__(self, group_id: Optional[SCT[str]]):
-        group_id = group_id
-
-    async def __call__(self, ctx: BotContext[Event]):
-        group_id = self.group_id
-        if group_id is None:
-            return bool(ctx.event.group_id is not None)
-        if isinstance(group_id, str):
-            group_id = frozenset({group_id})
-        else:
-            group_id = frozenset(group_id)
-        return bool(ctx.event.group_id in group_id)
-
-
-class user(Filter, set):
-    def __init__(self, user_id: Optional[SCT[int]]):
-        user_id = user_id
-
-    async def __call__(self, ctx: BotContext[Event]):
-        user_id = self.user_id
-        if user_id is None:
-            return bool(ctx.event.action_by_id is not None)
-        if isinstance(user_id, int):
-            user_id = frozenset({user_id})
-        else:
-            user_id = frozenset(user_id)
-        return bool(ctx.event.action_by_id in user_id)
-
-
-def text(text: Optional[SCT[str]]):
-    async def func(self, ctx: BotContext[MessageEvent]):
-        text = self.text
-        if text is None:
-            return bool(ctx.event.message is not None and ctx.event.message.message is not None)
-        if isinstance(text, str):
-            text = frozenset({text})
-        else:
-            text = frozenset(text)
-
-        if ctx.event.type == EventType.MESSAGE:
-            value = ctx.event.message.message
-        elif ctx.event.type == EventType.COMMAND:
-            value = ctx.event.command
-        elif ctx.event.type == EventType.CALLBACK_QUERY:
-            value = ctx.event.callback_data
-
-        for t in text:
-            if t in value:
-                return True
-            else:
-                try:
-                    regexp = re.compile(t)
-                    if regexp.search(value):
-                        return True
-                except re.error:
-                    pass
-        return False
-
-    return create(func, name="TextFilter", text=text)
-
-
-""" Filter messages by text. """
-
-
-def regexp(regexp: Optional[SCT[str]]):
-    async def func(self, ctx: BotContext[MessageEvent]):
-        regexp = self.regexp
-        if regexp is None:
-            return bool(ctx.event.message is not None and ctx.event.message.message is not None)
-        if isinstance(regexp, str):
-            regexp = frozenset({regexp})
-        else:
-            regexp = frozenset(regexp)
-
-        if ctx.event.type == EventType.MESSAGE:
-            value = ctx.event.message.message
-        elif ctx.event.type == EventType.COMMAND:
-            value = ctx.event.command
-        elif ctx.event.type == EventType.CALLBACK_QUERY:
-            value = ctx.event.callback_data
-
-        if value is None:
-            return False
-
-        for r in regexp:
-            try:
-
-                cr = re.compile(r)
-                if cr.match(value):
-                    return True
-            except re.error:
-                pass
-        return False
-
-    return create(func, name="RegexpFilter", regexp=regexp)
-
-
-""" Filter messages by regexp. """
-
-
-async def message_type(types: Optional[SCT[int]]):
-    async def func(self, ctx: BotContext[MessageEvent]):
-        types = self.types
-        if types is None:
-            return bool(ctx.event.message.status is not None)
-        if isinstance(types, int):
-            types = frozenset({types})
-        else:
-            types = frozenset(types)
-        return bool(ctx.event.message.status in types)
-    return create(func, name="MessageType", types=types)
+import re
+from typing import Optional
+from swibots.api.chat.events import MessageEvent
+from swibots.api.chat.events.chat_event import ChatEvent
+from swibots.api.common.events import Event
+from swibots.bots.bot_context import BotContext
+from swibots.utils.types import SCT, FilterCallback
+from swibots.types import EventType
+from typing import Callable, Union, List, Pattern
+
+
+class Filter:
+    async def __call__(self, ctx: BotContext) -> bool:
+        raise NotImplementedError
+
+    def __invert__(self):
+        return InvertFilter(self)
+
+    def __and__(self, other):
+        return AndFilter(self, other)
+
+    def __or__(self, other):
+        return OrFilter(self, other)
+
+
+class InvertFilter(Filter):
+    def __init__(self, base):
+        self.base = base
+
+    async def __call__(self, ctx: BotContext) -> bool:
+        result = await self.base(ctx)
+        return not result
+
+
+class AndFilter(Filter):
+    def __init__(self, base, other):
+        self.base = base
+        self.other = other
+
+    async def __call__(self, ctx: BotContext) -> bool:
+        r1 = await self.base(ctx)
+        # short circuit
+        if not r1:
+            return False
+        r2 = await self.other(ctx)
+
+        return r1 and r2
+
+
+class OrFilter(Filter):
+    def __init__(self, base, other):
+        self.base = base
+        self.other = other
+
+    async def __call__(self, ctx: BotContext) -> bool:
+        r1 = await self.base(ctx)
+        # short circuit
+        if r1:
+            return True
+
+        return await self.other(ctx)
+
+
+CUSTOM_FILTER_NAME = "CustomFilter"
+
+
+def create(func: FilterCallback, name: str = None, **kwargs) -> Filter:
+    return type(
+        name or func.__name__ or CUSTOM_FILTER_NAME, (Filter,), {
+            "__call__": func, **kwargs}
+    )()
+
+
+async def all_filter(self, ctx: BotContext):
+    return True
+
+
+all = create(all_filter)
+"""Filter all messages."""
+
+
+async def self_filter(self, ctx: BotContext[MessageEvent]):
+    return bool(
+        ctx.event.message is not None
+        and ctx.event.message.user_id == ctx.event.message.receiver_id
+    )
+
+
+self = create(self_filter)
+"""Filter messages generated by the same user."""
+
+
+async def bot_filter(self, ctx: BotContext[MessageEvent]):
+    return bool(
+        ctx.event.message is not None and ctx.event.user is not None and ctx.event.user.is_bot
+    )
+
+
+is_bot = create(bot_filter)
+"""Filter messages coming from bots."""
+
+
+async def me_filter(self, ctx: BotContext[MessageEvent]):
+    return bool(ctx.event.message is not None and ctx.event.message.user_id == ctx.user.id)
+
+
+me = create(me_filter)
+"""Filter messages coming from your user."""
+
+
+async def incoming_filter(self, ctx: BotContext[MessageEvent]):
+    return bool(ctx.event.message is not None and ctx.event.message.receiver_id == ctx.user.id)
+
+
+incoming = create(incoming_filter)
+"""Filter incoming messages. Messages that are sent to the users recipient."""
+
+
+async def outgoing_filter(self, ctx: BotContext[MessageEvent]):
+    return not incoming(ctx)
+
+
+outgoing = create(outgoing_filter)
+"""Filter outgoing messages. Messages that are sent by the user."""
+
+
+class community(Filter, set):
+    """Filter events comming from a specific community or communities"""
+
+    def __init__(self, community_id: Optional[SCT[str]]):
+        community_id = community_id
+
+    async def __call__(self, ctx: BotContext[Event]):
+        community_id = self.community_id
+        if community_id is None:
+            return bool(ctx.event.community_id is not None)
+        if isinstance(community_id, str):
+            community_id = frozenset({community_id})
+        else:
+            community_id = frozenset(community_id)
+        return bool(ctx.event.community_id in community_id)
+
+
+class channel(Filter, set):
+    """Filter events comming from a specific channel or channels"""
+
+    def __init__(self, channel_id: Optional[SCT[str]]):
+        channel_id = channel_id
+
+    async def __call__(self, ctx: BotContext[Event]):
+        channel_id = self.channel_id
+        if channel_id is None:
+            return bool(ctx.event.channel_id is not None)
+        if isinstance(channel_id, str):
+            channel_id = frozenset({channel_id})
+        else:
+            channel_id = frozenset(channel_id)
+        return bool(ctx.event.channel_id in channel_id)
+
+
+class group(Filter, set):
+    def __init__(self, group_id: Optional[SCT[str]]):
+        group_id = group_id
+
+    async def __call__(self, ctx: BotContext[Event]):
+        group_id = self.group_id
+        if group_id is None:
+            return bool(ctx.event.group_id is not None)
+        if isinstance(group_id, str):
+            group_id = frozenset({group_id})
+        else:
+            group_id = frozenset(group_id)
+        return bool(ctx.event.group_id in group_id)
+
+
+class user(Filter, set):
+    def __init__(self, user_id: Optional[SCT[int]]):
+        user_id = user_id
+
+    async def __call__(self, ctx: BotContext[Event]):
+        user_id = self.user_id
+        if user_id is None:
+            return bool(ctx.event.action_by_id is not None)
+        if isinstance(user_id, int):
+            user_id = frozenset({user_id})
+        else:
+            user_id = frozenset(user_id)
+        return bool(ctx.event.action_by_id in user_id)
+
+
+def text(text: Optional[SCT[str]]):
+    async def func(self, ctx: BotContext[MessageEvent]):
+        text = self.text
+        if text is None:
+            return bool(ctx.event.message is not None and ctx.event.message.message is not None)
+        if isinstance(text, str):
+            text = frozenset({text})
+        else:
+            text = frozenset(text)
+
+        if ctx.event.type == EventType.MESSAGE:
+            value = ctx.event.message.message
+        elif ctx.event.type == EventType.COMMAND:
+            value = ctx.event.command
+        elif ctx.event.type == EventType.CALLBACK_QUERY:
+            value = ctx.event.callback_data
+
+        for t in text:
+            if t in value:
+                return True
+            else:
+                try:
+                    regexp = re.compile(t)
+                    if regexp.search(value):
+                        return True
+                except re.error:
+                    pass
+        return False
+
+    return create(func, name="TextFilter", text=text)
+
+
+""" Filter messages by text. """
+
+
+def regexp(regexp: Optional[SCT[str]]):
+    async def func(self, ctx: BotContext[MessageEvent]):
+        regexp = self.regexp
+        if regexp is None:
+            return bool(ctx.event.message is not None and ctx.event.message.message is not None)
+        if isinstance(regexp, str):
+            regexp = frozenset({regexp})
+        else:
+            regexp = frozenset(regexp)
+
+        if ctx.event.type == EventType.MESSAGE:
+            value = ctx.event.message.message
+        elif ctx.event.type == EventType.COMMAND:
+            value = ctx.event.command
+        elif ctx.event.type == EventType.CALLBACK_QUERY:
+            value = ctx.event.callback_data
+
+        if value is None:
+            return False
+
+        for r in regexp:
+            try:
+
+                cr = re.compile(r)
+                if cr.match(value):
+                    return True
+            except re.error:
+                pass
+        return False
+
+    return create(func, name="RegexpFilter", regexp=regexp)
+
+
+""" Filter messages by regexp. """
+
+
+async def message_type(types: Optional[SCT[int]]):
+    async def func(self, ctx: BotContext[MessageEvent]):
+        types = self.types
+        if types is None:
+            return bool(ctx.event.message.status is not None)
+        if isinstance(types, int):
+            types = frozenset({types})
+        else:
+            types = frozenset(types)
+        return bool(ctx.event.message.status in types)
+    return create(func, name="MessageType", types=types)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/__init__.py` & `swibots-1.2.9/swibots/bots/handlers/__init__.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from .base_handler import BaseHandler
-from .event_handler import EventHandler
-from .command_handler import CommandHandler
-from .message_handler import MessageHandler
-from .callback_query_handler import CallbackQueryHandler
-from .channel_created_handler import ChannelCreatedHandler
-from .channel_deleted_handler import ChannelDeletedHandler
-from .channel_updated_handler import ChannelUpdatedHandler
-from .group_created_handler import GroupCreatedHandler
-from .group_deleted_handler import GroupDeletedHandler
-from .group_updated_handler import GroupUpdatedHandler
-from .member_joined_handler import MemberJoinedHandler
-from .member_left_handler import MemberLeftHandler
-from .user_banned_handler import UserBannedHandler
-from .community_updated_handler import CommunityUpdatedHandler
-from .unknown_command_handler import UnknownCommandHandler
-from .inline_query_handler import InlineQueryHandler
-
-
-class Handlers(
-    CommandHandler,
-    MessageHandler,
-    CallbackQueryHandler,
-    UnknownCommandHandler,
-    ChannelCreatedHandler,
-    ChannelDeletedHandler,
-    ChannelUpdatedHandler,
-    GroupCreatedHandler,
-    GroupDeletedHandler,
-    GroupUpdatedHandler,
-    MemberJoinedHandler,
-    MemberLeftHandler,
-    UserBannedHandler,
-    CommunityUpdatedHandler,
-    InlineQueryHandler,
-):
-    pass
+from .base_handler import BaseHandler
+from .event_handler import EventHandler
+from .command_handler import CommandHandler
+from .message_handler import MessageHandler
+from .callback_query_handler import CallbackQueryHandler
+from .channel_created_handler import ChannelCreatedHandler
+from .channel_deleted_handler import ChannelDeletedHandler
+from .channel_updated_handler import ChannelUpdatedHandler
+from .group_created_handler import GroupCreatedHandler
+from .group_deleted_handler import GroupDeletedHandler
+from .group_updated_handler import GroupUpdatedHandler
+from .member_joined_handler import MemberJoinedHandler
+from .member_left_handler import MemberLeftHandler
+from .user_banned_handler import UserBannedHandler
+from .community_updated_handler import CommunityUpdatedHandler
+from .unknown_command_handler import UnknownCommandHandler
+from .inline_query_handler import InlineQueryHandler
+
+
+class Handlers(
+    CommandHandler,
+    MessageHandler,
+    CallbackQueryHandler,
+    UnknownCommandHandler,
+    ChannelCreatedHandler,
+    ChannelDeletedHandler,
+    ChannelUpdatedHandler,
+    GroupCreatedHandler,
+    GroupDeletedHandler,
+    GroupUpdatedHandler,
+    MemberJoinedHandler,
+    MemberLeftHandler,
+    UserBannedHandler,
+    CommunityUpdatedHandler,
+    InlineQueryHandler,
+):
+    pass
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/callback_query_handler.py` & `swibots-1.2.9/swibots/bots/handlers/callback_query_handler.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import re
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.chat.events import CallbackQueryEvent
-from swibots.bots.filters.filter import Filter
-from swibots.types import EventType
-
-from swibots.utils.types import SCT, HandlerCallback
-from swibots.bots.handlers.event_handler import EventHandler
-from swibots.bots.bot_context import BotContext
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class CallbackQueryHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[CallbackQueryEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.CALLBACK_QUERY, callback, filter, **kwargs)
-
-    async def should_handle(self, context: BotContext[CallbackQueryEvent]) -> bool:
-        return (
-            await super().should_handle(context)
-            and context.event.callback_data is not None
-            and context.event.message is not None
-        )
+import re
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.chat.events import CallbackQueryEvent
+from swibots.bots.filters.filter import Filter
+from swibots.types import EventType
+
+from swibots.utils.types import SCT, HandlerCallback
+from swibots.bots.handlers.event_handler import EventHandler
+from swibots.bots.bot_context import BotContext
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class CallbackQueryHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[CallbackQueryEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.CALLBACK_QUERY, callback, filter, **kwargs)
+
+    async def should_handle(self, context: BotContext[CallbackQueryEvent]) -> bool:
+        return (
+            await super().should_handle(context)
+            and context.event.callback_data is not None
+            and context.event.message is not None
+        )
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/channel_created_handler.py` & `swibots-1.2.9/swibots/bots/handlers/channel_created_handler.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import ChannelCreatedEvent
-from swibots.bots.filters import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class ChannelCreatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[ChannelCreatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_CHANNEL_CREATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import ChannelCreatedEvent
+from swibots.bots.filters import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class ChannelCreatedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[ChannelCreatedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_CHANNEL_CREATE, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/channel_deleted_handler.py` & `swibots-1.2.9/swibots/bots/handlers/channel_deleted_handler.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import ChannelDeletedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class ChannelDeletedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[ChannelDeletedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_CHANNEL_DELETE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import ChannelDeletedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class ChannelDeletedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[ChannelDeletedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_CHANNEL_DELETE, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/channel_updated_handler.py` & `swibots-1.2.9/swibots/bots/handlers/group_deleted_handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import ChannelUpdatedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots.handlers import BaseHandler
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class ChannelUpdatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[ChannelUpdatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_CHANNEL_UPDATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.chat.events import MessageEvent
+from swibots.api.community.events import GroupDeletedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots.handlers import BaseHandler
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class GroupDeletedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[GroupDeletedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_GROUP_DELETE, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/community_updated_handler.py` & `swibots-1.2.9/swibots/bots/handlers/community_updated_handler.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import CommunityUpdatedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class CommunityUpdatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[CommunityUpdatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_UPDATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import CommunityUpdatedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class CommunityUpdatedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[CommunityUpdatedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_UPDATE, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/event_handler.py` & `swibots-1.2.9/swibots/bots/handlers/unknown_command_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,29 @@
-import re
-from typing import TYPE_CHECKING, Generic, Optional, TypeVar
-from swibots.bots.constants import VALID_COMMAND_REGEX
-from swibots.bots.filters.filter import Filter
-from swibots.types import EventType
-
-from swibots.utils.types import SCT, HandlerCallback
-from swibots.bots.handlers.base_handler import BaseHandler
-from swibots.bots.bot_context import BotContext
-from swibots.api.chat.events import CommandEvent
-from swibots.api.common.events import Event
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class EventHandler(BaseHandler):
-    def __init__(
-        self,
-        event_types: Optional[SCT[EventType]],
-        callback: HandlerCallback[BotContext[Event], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(callback, filter, **kwargs)
-        if isinstance(event_types, EventType):
-            event_types = frozenset({event_types})
-        else:
-            event_types = frozenset(event_types)
-        self.event_types = event_types
-        self.filter = filter
-
-    async def should_handle(self, context: BotContext[Event]) -> bool:
-        if (self.event_types is not None) and (not context.event.type in self.event_types):
-            return False
-        if self.filter:
-            return await self.filter(context)
-        return True
+import re
+from typing import TYPE_CHECKING, Any, Optional, TypeVar
+from swibots.bots.constants import VALID_COMMAND_REGEX
+from swibots.bots.filters.filter import Filter
+from swibots.types import EventType
+
+from swibots.utils.types import SCT, HandlerCallback
+from swibots.bots.handlers.base_handler import BaseHandler
+from swibots.bots.bot_context import BotContext
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class UnknownCommandHandler(BaseHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[Any], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(callback, filter, **kwargs)
+
+    async def should_handle(self, context: BotContext[Any]) -> bool:
+        if context.event.type == EventType.COMMAND and context.event.message is not None:
+            return True
+        return False
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/group_created_handler.py` & `swibots-1.2.9/swibots/bots/handlers/group_created_handler.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import GroupCreatedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class GroupCreatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[GroupCreatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_GROUP_CREATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import GroupCreatedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class GroupCreatedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[GroupCreatedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_GROUP_CREATE, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/group_deleted_handler.py` & `swibots-1.2.9/swibots/bots/handlers/member_joined_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.chat.events import MessageEvent
-from swibots.api.community.events import GroupDeletedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots.handlers import BaseHandler
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class GroupDeletedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[GroupDeletedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_GROUP_DELETE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import MemberJoinedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class MemberJoinedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[MemberJoinedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_MEMBER_JOIN, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/group_updated_handler.py` & `swibots-1.2.9/swibots/bots/handlers/group_updated_handler.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.chat.events import MessageEvent
-from swibots.api.community.events import GroupUpdatedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots.handlers import BaseHandler
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class GroupUpdatedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[GroupUpdatedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_GROUP_UPDATE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.chat.events import MessageEvent
+from swibots.api.community.events import GroupUpdatedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots.handlers import BaseHandler
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class GroupUpdatedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[GroupUpdatedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_GROUP_UPDATE, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/inline_query_handler.py` & `swibots-1.2.9/swibots/bots/handlers/inline_query_handler.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.chat.events import InlineQueryEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots.handlers import BaseHandler
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class InlineQueryHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[InlineQueryEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.INLINE_QUERY, callback, filter, **kwargs)
-
-    async def should_handle(self, context: BotContext[InlineQueryEvent]) -> bool:
-        return (
-            await super().should_handle(context)
-        )
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.chat.events import InlineQueryEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots.handlers import BaseHandler
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class InlineQueryHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[InlineQueryEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.INLINE_QUERY, callback, filter, **kwargs)
+
+    async def should_handle(self, context: BotContext[InlineQueryEvent]) -> bool:
+        return (
+            await super().should_handle(context)
+        )
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/member_joined_handler.py` & `swibots-1.2.9/swibots/bots/handlers/channel_updated_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import MemberJoinedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class MemberJoinedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[MemberJoinedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_MEMBER_JOIN, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import ChannelUpdatedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots.handlers import BaseHandler
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class ChannelUpdatedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[ChannelUpdatedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_CHANNEL_UPDATE, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/member_left_handler.py` & `swibots-1.2.9/swibots/bots/handlers/user_banned_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import MemberLeftEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class MemberLeftHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[MemberLeftEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_MEMBER_LEAVE, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import UserBannedEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class UserBannedHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[UserBannedEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_USER_BAN, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/message_handler.py` & `swibots-1.2.9/swibots/bots/handlers/message_handler.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.chat.events import MessageEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots.handlers import BaseHandler
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class MessageHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[MessageEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.MESSAGE, callback, filter, **kwargs)
-
-    async def should_handle(self, context: BotContext[MessageEvent]) -> bool:
-        return (
-            await super().should_handle(context)
-            and context.event.message is not None
-            and context.event.message.user_id != context.bot.id
-        )
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.chat.events import MessageEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots.handlers import BaseHandler
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class MessageHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[MessageEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.MESSAGE, callback, filter, **kwargs)
+
+    async def should_handle(self, context: BotContext[MessageEvent]) -> bool:
+        return (
+            await super().should_handle(context)
+            and context.event.message is not None
+            and context.event.message.user_id != context.bot.id
+        )
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/unknown_command_handler.py` & `swibots-1.2.9/swibots/bots/handlers/event_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,40 @@
-import re
-from typing import TYPE_CHECKING, Any, Optional, TypeVar
-from swibots.bots.constants import VALID_COMMAND_REGEX
-from swibots.bots.filters.filter import Filter
-from swibots.types import EventType
-
-from swibots.utils.types import SCT, HandlerCallback
-from swibots.bots.handlers.base_handler import BaseHandler
-from swibots.bots.bot_context import BotContext
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class UnknownCommandHandler(BaseHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[Any], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(callback, filter, **kwargs)
-
-    async def should_handle(self, context: BotContext[Any]) -> bool:
-        if context.event.type == EventType.COMMAND and context.event.message is not None:
-            return True
-        return False
+import re
+from typing import TYPE_CHECKING, Generic, Optional, TypeVar
+from swibots.bots.constants import VALID_COMMAND_REGEX
+from swibots.bots.filters.filter import Filter
+from swibots.types import EventType
+
+from swibots.utils.types import SCT, HandlerCallback
+from swibots.bots.handlers.base_handler import BaseHandler
+from swibots.bots.bot_context import BotContext
+from swibots.api.chat.events import CommandEvent
+from swibots.api.common.events import Event
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class EventHandler(BaseHandler):
+    def __init__(
+        self,
+        event_types: Optional[SCT[EventType]],
+        callback: HandlerCallback[BotContext[Event], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(callback, filter, **kwargs)
+        if isinstance(event_types, EventType):
+            event_types = frozenset({event_types})
+        else:
+            event_types = frozenset(event_types)
+        self.event_types = event_types
+        self.filter = filter
+
+    async def should_handle(self, context: BotContext[Event]) -> bool:
+        if (self.event_types is not None) and (not context.event.type in self.event_types):
+            return False
+        if self.filter:
+            return await self.filter(context)
+        return True
```

### Comparing `swibots-1.2.8/swibots/bots/handlers/user_banned_handler.py` & `swibots-1.2.9/swibots/bots/handlers/member_left_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import TYPE_CHECKING, Optional, TypeVar
-from swibots.api.community.events import UserBannedEvent
-from swibots.bots.filters.filter import Filter
-
-from swibots.bots import BotContext
-from .event_handler import EventHandler
-from swibots.types import EventType
-from swibots.utils.types import HandlerCallback
-
-if TYPE_CHECKING:
-    pass
-
-ResType = TypeVar("ResType")
-
-
-class UserBannedHandler(EventHandler):
-    def __init__(
-        self,
-        callback: HandlerCallback[BotContext[UserBannedEvent], ResType],
-        filter: Optional[Filter] = None,
-        **kwargs,
-    ):
-        super().__init__(EventType.COMMUNITY_USER_BAN, callback, filter, **kwargs)
+from typing import TYPE_CHECKING, Optional, TypeVar
+from swibots.api.community.events import MemberLeftEvent
+from swibots.bots.filters.filter import Filter
+
+from swibots.bots import BotContext
+from .event_handler import EventHandler
+from swibots.types import EventType
+from swibots.utils.types import HandlerCallback
+
+if TYPE_CHECKING:
+    pass
+
+ResType = TypeVar("ResType")
+
+
+class MemberLeftHandler(EventHandler):
+    def __init__(
+        self,
+        callback: HandlerCallback[BotContext[MemberLeftEvent], ResType],
+        filter: Optional[Filter] = None,
+        **kwargs,
+    ):
+        super().__init__(EventType.COMMUNITY_MEMBER_LEAVE, callback, filter, **kwargs)
```

### Comparing `swibots-1.2.8/swibots/config.py` & `swibots-1.2.9/swibots/config.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import os
-
-
-APP_CONFIG = {
-    "CHAT_SERVICE": {
-        "BASE_URL": os.getenv("CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe",
-        "WS_URL": os.getenv("CHAT_SERVICE_WS_URL")
-        or "wss://api-gateway.switch.pe/v1/websocket/message/ws",
-    },
-    "BOT_SERVICE": {
-        "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://chat.switch.pe",
-    },
-    "AUTH_SERVICE": {
-        "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api",
-    },
-    "COMMUNITY_SERVICE": {
-        "BASE_URL": os.getenv("COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
-        "WS_URL": os.getenv("COMMUNITY_SERVICE_WS_URL")
-        or "wss://api-gateway.switch.pe/v1/websocket/community/ws",
-    },
-}
-
-
-def get_config():
-    return APP_CONFIG
-
-
-def reload_config():
-    APP_CONFIG["CHAT_SERVICE"]['BASE_URL'] = os.getenv(
-        "CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe"
-    APP_CONFIG["CHAT_SERVICE"]['WS_URL'] = os.getenv(
-        "CHAT_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/message/ws"
-    APP_CONFIG["BOT_SERVICE"]['BASE_URL'] = os.getenv(
-        "BOT_SERVICE_BASE_URL") or "https://chat.switch.pe"
-    APP_CONFIG["AUTH_SERVICE"]['BASE_URL'] = os.getenv(
-        "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api"
-    APP_CONFIG["COMMUNITY_SERVICE"]['BASE_URL'] = os.getenv(
-        "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
-    APP_CONFIG["COMMUNITY_SERVICE"]['WS_URL'] = os.getenv(
-        "COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/community/ws"
-
-
-reload_config()
+import os
+
+
+APP_CONFIG = {
+    "CHAT_SERVICE": {
+        "BASE_URL": os.getenv("CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe",
+        "WS_URL": os.getenv("CHAT_SERVICE_WS_URL")
+        or "wss://api-gateway.switch.pe/v1/websocket/message/ws",
+    },
+    "BOT_SERVICE": {
+        "BASE_URL": os.getenv("BOT_SERVICE_BASE_URL") or "https://chat.switch.pe",
+    },
+    "AUTH_SERVICE": {
+        "BASE_URL": os.getenv("AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api",
+    },
+    "COMMUNITY_SERVICE": {
+        "BASE_URL": os.getenv("COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe",
+        "WS_URL": os.getenv("COMMUNITY_SERVICE_WS_URL")
+        or "wss://api-gateway.switch.pe/v1/websocket/community/ws",
+    },
+}
+
+
+def get_config():
+    return APP_CONFIG
+
+
+def reload_config():
+    APP_CONFIG["CHAT_SERVICE"]['BASE_URL'] = os.getenv(
+        "CHAT_SERVICE_BASE_URL") or "https://chat.switch.pe"
+    APP_CONFIG["CHAT_SERVICE"]['WS_URL'] = os.getenv(
+        "CHAT_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/message/ws"
+    APP_CONFIG["BOT_SERVICE"]['BASE_URL'] = os.getenv(
+        "BOT_SERVICE_BASE_URL") or "https://chat.switch.pe"
+    APP_CONFIG["AUTH_SERVICE"]['BASE_URL'] = os.getenv(
+        "AUTH_SERVICE_BASE_URL") or "https://api-gateway.switch.pe/api"
+    APP_CONFIG["COMMUNITY_SERVICE"]['BASE_URL'] = os.getenv(
+        "COMMUNITY_SERVICE_BASE_URL") or "https://api-gateway.switch.pe"
+    APP_CONFIG["COMMUNITY_SERVICE"]['WS_URL'] = os.getenv(
+        "COMMUNITY_SERVICE_WS_URL") or "wss://api-gateway.switch.pe/v1/websocket/community/ws"
+
+
+reload_config()
```

### Comparing `swibots-1.2.8/swibots/error.py` & `swibots-1.2.9/swibots/error.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from typing import Tuple
-
-
-def _lstrip_str(in_s: str, lstr: str) -> str:
-    """
-    Args:
-        in_s (:obj:`str`): in string
-        lstr (:obj:`str`): substr to strip from left side
-    Returns:
-        :obj:`str`: The stripped string.
-    """
-    if in_s.startswith(lstr):
-        res = in_s[len(lstr):]
-    else:
-        res = in_s
-    return res
-
-
-class SwitchError(Exception):
-    """
-    Base class for Seitch errors.
-    .. seealso:: :wiki:`Exceptions, Warnings and Logging <Exceptions%2C-Warnings-and-Logging>`
-    """
-
-    def __init__(self, message: str):
-        super().__init__()
-
-        msg = _lstrip_str(message, "Error: ")
-        msg = _lstrip_str(msg, "[Error]: ")
-        msg = _lstrip_str(msg, "Bad Request: ")
-        if msg != message:
-            # api_error - capitalize the msg...
-            msg = msg.capitalize()
-        self.message = msg
-
-    def __str__(self) -> str:
-        return self.message
-
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}('{self.message}')"
-
-    def __reduce__(self) -> Tuple[type, Tuple[str]]:
-        return self.__class__, (self.message,)
-
-
-class NetworkError(SwitchError):
-    """Base class for exceptions due to networking errors.
-    Examples:
-        :any:`Raw API Bot <examples.rawapibot>`
-    """
-
-
-class CancelError(SwitchError):
-    pass
+from typing import Tuple
+
+
+def _lstrip_str(in_s: str, lstr: str) -> str:
+    """
+    Args:
+        in_s (:obj:`str`): in string
+        lstr (:obj:`str`): substr to strip from left side
+    Returns:
+        :obj:`str`: The stripped string.
+    """
+    if in_s.startswith(lstr):
+        res = in_s[len(lstr):]
+    else:
+        res = in_s
+    return res
+
+
+class SwitchError(Exception):
+    """
+    Base class for Seitch errors.
+    .. seealso:: :wiki:`Exceptions, Warnings and Logging <Exceptions%2C-Warnings-and-Logging>`
+    """
+
+    def __init__(self, message: str):
+        super().__init__()
+
+        msg = _lstrip_str(message, "Error: ")
+        msg = _lstrip_str(msg, "[Error]: ")
+        msg = _lstrip_str(msg, "Bad Request: ")
+        if msg != message:
+            # api_error - capitalize the msg...
+            msg = msg.capitalize()
+        self.message = msg
+
+    def __str__(self) -> str:
+        return self.message
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}('{self.message}')"
+
+    def __reduce__(self) -> Tuple[type, Tuple[str]]:
+        return self.__class__, (self.message,)
+
+
+class NetworkError(SwitchError):
+    """Base class for exceptions due to networking errors.
+    Examples:
+        :any:`Raw API Bot <examples.rawapibot>`
+    """
+
+
+class CancelError(SwitchError):
+    pass
```

### Comparing `swibots-1.2.8/swibots/types.py` & `swibots-1.2.9/swibots/types.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import enum
-
-
-class EventType(enum.Enum):
-    """Represents the type of a event."""
-
-    # Chat
-    MESSAGE = "MESSAGE"
-    COMMAND = "COMMAND"
-    CALLBACK_QUERY = "CALLBACK_QUERY"
-    INLINE_QUERY = "INLINE_QUERY"
-    # Community
-    COMMUNITY_CHANNEL_CREATE = "COMMUNITY_CHANNEL_CREATE"
-    COMMUNITY_CHANNEL_UPDATE = "COMMUNITY_CHANNEL_UPDATE"
-    COMMUNITY_CHANNEL_DELETE = "COMMUNITY_CHANNEL_DELETE"
-    COMMUNITY_GROUP_CREATE = "COMMUNITY_GROUP_CREATE"
-    COMMUNITY_GROUP_UPDATE = "COMMUNITY_GROUP_UPDATE"
-    COMMUNITY_GROUP_DELETE = "COMMUNITY_GROUP_DELETE"
-    COMMUNITY_USER_BAN = "COMMUNITY_USER_BAN"
-    COMMUNITY_USER_UNBAN = "COMMUNITY_USER_UNBAN"
-    COMMUNITY_MEMBER_JOIN = "COMMUNITY_MEMBER_JOIN"
-    COMMUNITY_MEMBER_LEAVE = "COMMUNITY_MEMBER_LEAVE"
-    COMMUNITY_UPDATE = "COMMUNITY_UPDATE"
-    COMMUNITY_DELETE = "COMMUNITY_DELETE"
+import enum
+
+
+class EventType(enum.Enum):
+    """Represents the type of a event."""
+
+    # Chat
+    MESSAGE = "MESSAGE"
+    COMMAND = "COMMAND"
+    CALLBACK_QUERY = "CALLBACK_QUERY"
+    INLINE_QUERY = "INLINE_QUERY"
+    # Community
+    COMMUNITY_CHANNEL_CREATE = "COMMUNITY_CHANNEL_CREATE"
+    COMMUNITY_CHANNEL_UPDATE = "COMMUNITY_CHANNEL_UPDATE"
+    COMMUNITY_CHANNEL_DELETE = "COMMUNITY_CHANNEL_DELETE"
+    COMMUNITY_GROUP_CREATE = "COMMUNITY_GROUP_CREATE"
+    COMMUNITY_GROUP_UPDATE = "COMMUNITY_GROUP_UPDATE"
+    COMMUNITY_GROUP_DELETE = "COMMUNITY_GROUP_DELETE"
+    COMMUNITY_USER_BAN = "COMMUNITY_USER_BAN"
+    COMMUNITY_USER_UNBAN = "COMMUNITY_USER_UNBAN"
+    COMMUNITY_MEMBER_JOIN = "COMMUNITY_MEMBER_JOIN"
+    COMMUNITY_MEMBER_LEAVE = "COMMUNITY_MEMBER_LEAVE"
+    COMMUNITY_UPDATE = "COMMUNITY_UPDATE"
+    COMMUNITY_DELETE = "COMMUNITY_DELETE"
```

### Comparing `swibots-1.2.8/swibots/utils/rest_client.py` & `swibots-1.2.9/swibots/utils/rest_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-# import the standard JSON parser
-import json
-import logging
-from typing import Optional, Tuple
-
-# import the REST library
-import httpx
-
-from swibots.error import NetworkError, SwitchError
-from swibots.utils.types import JSONDict
-
-log = logging.getLogger(__name__)
-
-DEFAULT_HEADERS = {"Accept": "application/json"}
-
-
-class RestClient:
-    def __init__(
-        self,
-        connection_pool_size: int = 1,
-        proxy_url: str = None,
-        read_timeout: Optional[float] = None,
-        write_timeout: Optional[float] = None,
-        connect_timeout: Optional[float] = None,
-        pool_timeout: Optional[float] = 1.0,
-    ):
-        timeout = httpx.Timeout(
-            connect=connect_timeout,
-            read=read_timeout,
-            write=write_timeout,
-            pool=pool_timeout,
-        )
-        limits = httpx.Limits(
-            max_connections=connection_pool_size,
-            max_keepalive_connections=connection_pool_size,
-        )
-        self._client_kwargs = dict(
-            timeout=timeout,
-            proxies=proxy_url,
-            limits=limits,
-        )
-
-        try:
-            self._client = self._build_client()
-        except ImportError as exc:
-            if "httpx[socks]" not in str(exc):
-                raise exc
-
-            raise RuntimeError(
-                "To use Socks5 proxies, PTB must be installed via `pip install "
-                "python-telegram-bot[socks]`."
-            ) from exc
-
-    def _build_client(self) -> httpx.AsyncClient:
-        # type: ignore[arg-type]
-        return httpx.AsyncClient(**self._client_kwargs)
-
-    def initialize(self) -> None:
-        log.debug("Initializing HTTPXRequest")
-        if self._client.is_closed:
-            self._client = self._build_client()
-
-    async def shutdown(self) -> None:
-        """See :meth:`BaseRequest.shutdown`."""
-        if self._client.is_closed:
-            log.debug("This HTTPXRequest is already shut down. Returning.")
-            return
-        await self._client.aclose()
-
-    async def get(self, url: str, data: dict = None, headers: dict = None) -> Tuple[int, bytes]:
-        """See :meth:`BaseRequest.get`."""
-        return await self.do_request(url, "GET", data, headers=headers)
-
-    async def post(self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None) -> Tuple[int, bytes]:
-        """See :meth:`BaseRequest.post`."""
-        return await self.do_request(url, "POST", data, form_data, files, headers)
-
-    async def put(self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None) -> Tuple[int, bytes]:
-        """See :meth:`BaseRequest.put`."""
-        return await self.do_request(url, "PUT", data, form_data, files, headers)
-
-    async def delete(self, url: str, data: dict = None, headers: dict = None) -> Tuple[int, bytes]:
-        """See :meth:`BaseRequest.delete`."""
-        return await self.do_request(url, "DELETE", data, headers=headers)
-
-    async def patch(self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None) -> Tuple[int, bytes]:
-        """See :meth:`BaseRequest.patch`."""
-        return await self.do_request(url, "PATCH", data, form_data, files, headers)
-
-    async def head(self, url: str, data: dict = None, headers: dict = None) -> Tuple[int, bytes]:
-        """See :meth:`BaseRequest.head`."""
-        return await self.do_request(url, "HEAD", data, headers)
-
-    async def options(
-        self, url: str, data: dict = None, headers: dict = None
-    ) -> Tuple[int, bytes]:
-        """See :meth:`BaseRequest.options`."""
-        return await self.do_request(url, "OPTIONS", data, headers)
-
-    def prepare_request_data(self, data: dict) -> str | None:
-        data = {**data} if data else None
-        return data
-
-    def prepare_request_headers(self, headers: dict) -> dict:
-        if headers is None:
-            headers = {}
-        reqHeaders = {**headers}
-        return reqHeaders
-
-    async def do_request(
-        self, url: str, method: str, data: dict = None, form_data=None, files=None, headers: dict = None
-    ) -> Tuple[int, bytes]:
-        if self._client.is_closed:
-            raise RuntimeError("This RestClient is not initialized!")
-        try:
-            data = self.prepare_request_data(data)
-            reqHeaders = self.prepare_request_headers(headers)
-            if (form_data is not None):
-                # reqHeaders["Content-Type"] = "multipart/form-data"
-                # reqHeaders["Accept"] = "application/json"
-                response = await self._client.request(method, url, data=form_data, files=files, headers=reqHeaders)
-            else:
-                response = await self._client.request(method, url, json=data, headers=reqHeaders)
-        except httpx.HTTPError as err:
-            # HTTPError must come last as its the base httpx exception class
-            # TODO p4: do something smart here; for now just raise NetworkError
-            raise NetworkError(f"httpx HTTPError: {err}") from err
-
-        return response.status_code, response.content
-
-    @staticmethod
-    def parse_json_payload(payload: bytes) -> JSONDict:
-        """Parse the JSON returned from Switch.
-        Tip:
-            By default, this method uses the standard library's :func:`json.loads` and
-            ``errors="replace"`` in :meth:`bytes.decode`.
-            You can override it to customize either of these behaviors.
-        Args:
-            payload (:obj:`bytes`): The UTF-8 encoded JSON payload as returned by Telegram.
-        Returns:
-            dict: A JSON parsed as Python dict with results.
-        Raises:
-            SwitchError: If loading the JSON data failed
-        """
-        decoded_s = payload.decode("utf-8", "replace")
-        try:
-            return json.loads(decoded_s)
-        except ValueError as exc:
-            raise SwitchError("Invalid server response") from exc
+# import the standard JSON parser
+import json
+import logging
+from typing import Optional, Tuple
+
+# import the REST library
+import httpx
+
+from swibots.error import NetworkError, SwitchError
+from swibots.utils.types import JSONDict
+
+log = logging.getLogger(__name__)
+
+DEFAULT_HEADERS = {"Accept": "application/json"}
+
+
+class RestClient:
+    def __init__(
+        self,
+        connection_pool_size: int = 1,
+        proxy_url: str = None,
+        read_timeout: Optional[float] = None,
+        write_timeout: Optional[float] = None,
+        connect_timeout: Optional[float] = None,
+        pool_timeout: Optional[float] = 1.0,
+    ):
+        timeout = httpx.Timeout(
+            connect=connect_timeout,
+            read=read_timeout,
+            write=write_timeout,
+            pool=pool_timeout,
+        )
+        limits = httpx.Limits(
+            max_connections=connection_pool_size,
+            max_keepalive_connections=connection_pool_size,
+        )
+        self._client_kwargs = dict(
+            timeout=timeout,
+            proxies=proxy_url,
+            limits=limits,
+        )
+
+        try:
+            self._client = self._build_client()
+        except ImportError as exc:
+            if "httpx[socks]" not in str(exc):
+                raise exc
+
+            raise RuntimeError(
+                "To use Socks5 proxies, PTB must be installed via `pip install "
+                "python-telegram-bot[socks]`."
+            ) from exc
+
+    def _build_client(self) -> httpx.AsyncClient:
+        # type: ignore[arg-type]
+        return httpx.AsyncClient(**self._client_kwargs)
+
+    def initialize(self) -> None:
+        log.debug("Initializing HTTPXRequest")
+        if self._client.is_closed:
+            self._client = self._build_client()
+
+    async def shutdown(self) -> None:
+        """See :meth:`BaseRequest.shutdown`."""
+        if self._client.is_closed:
+            log.debug("This HTTPXRequest is already shut down. Returning.")
+            return
+        await self._client.aclose()
+
+    async def get(self, url: str, data: dict = None, headers: dict = None) -> Tuple[int, bytes]:
+        """See :meth:`BaseRequest.get`."""
+        return await self.do_request(url, "GET", data, headers=headers)
+
+    async def post(self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None) -> Tuple[int, bytes]:
+        """See :meth:`BaseRequest.post`."""
+        return await self.do_request(url, "POST", data, form_data, files, headers)
+
+    async def put(self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None) -> Tuple[int, bytes]:
+        """See :meth:`BaseRequest.put`."""
+        return await self.do_request(url, "PUT", data, form_data, files, headers)
+
+    async def delete(self, url: str, data: dict = None, headers: dict = None) -> Tuple[int, bytes]:
+        """See :meth:`BaseRequest.delete`."""
+        return await self.do_request(url, "DELETE", data, headers=headers)
+
+    async def patch(self, url: str, data: dict = None, form_data=None, files=None, headers: dict = None) -> Tuple[int, bytes]:
+        """See :meth:`BaseRequest.patch`."""
+        return await self.do_request(url, "PATCH", data, form_data, files, headers)
+
+    async def head(self, url: str, data: dict = None, headers: dict = None) -> Tuple[int, bytes]:
+        """See :meth:`BaseRequest.head`."""
+        return await self.do_request(url, "HEAD", data, headers)
+
+    async def options(
+        self, url: str, data: dict = None, headers: dict = None
+    ) -> Tuple[int, bytes]:
+        """See :meth:`BaseRequest.options`."""
+        return await self.do_request(url, "OPTIONS", data, headers)
+
+    def prepare_request_data(self, data: dict) -> str | None:
+        data = {**data} if data else None
+        return data
+
+    def prepare_request_headers(self, headers: dict) -> dict:
+        if headers is None:
+            headers = {}
+        reqHeaders = {**headers}
+        return reqHeaders
+
+    async def do_request(
+        self, url: str, method: str, data: dict = None, form_data=None, files=None, headers: dict = None
+    ) -> Tuple[int, bytes]:
+        if self._client.is_closed:
+            raise RuntimeError("This RestClient is not initialized!")
+        try:
+            data = self.prepare_request_data(data)
+            req_headers = self.prepare_request_headers(headers)
+            if form_data is not None:
+                # reqHeaders["Content-Type"] = "multipart/form-data"
+                # reqHeaders["Accept"] = "application/json"
+                response = await self._client.request(method, url, data=form_data, files=files, headers=req_headers)
+            else:
+                response = await self._client.request(method, url, json=data, headers=req_headers)
+        except httpx.HTTPError as err:
+            # HTTPError must come last as its the base httpx exception class
+            # TODO p4: do something smart here; for now just raise NetworkError
+            raise NetworkError(f"httpx HTTPError: {err}") from err
+
+        return response.status_code, response.content
+
+    @staticmethod
+    def parse_json_payload(payload: bytes) -> JSONDict:
+        """Parse the JSON returned from Switch.
+        Tip:
+            By default, this method uses the standard library's :func:`json.loads` and
+            ``errors="replace"`` in :meth:`bytes.decode`.
+            You can override it to customize either of these behaviors.
+        Args:
+            payload (:obj:`bytes`): The UTF-8 encoded JSON payload as returned by Telegram.
+        Returns:
+            dict: A JSON parsed as Python dict with results.
+        Raises:
+            SwitchError: If loading the JSON data failed
+        """
+        decoded_s = payload.decode("utf-8", "replace")
+        try:
+            return json.loads(decoded_s)
+        except ValueError as exc:
+            raise SwitchError("Invalid server response") from exc
```

### Comparing `swibots-1.2.8/swibots/utils/types.py` & `swibots-1.2.9/swibots/utils/types.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-from enum import Enum
-from typing import Any, Callable, Collection, Coroutine, Dict, TypeVar, Union
-
-from swibots.error import CancelError
-
-
-class IOClient:
-    def cancel(self) -> None:
-        raise CancelError()
-
-
-class DownloadProgress:
-    def __init__(self, downloaded: int, total: int, url: str, client: IOClient, file_name: str):
-        self.downloaded = downloaded
-        self.total = total
-        self.url = url
-        self.client = client
-        self.file_name = file_name
-        self.started = False
-
-
-class UploadProgress:
-    def __init__(self, current: int, readed: int, url: str, client: IOClient, file_name: str, callback, callback_args):
-        self.current = current
-        self.readed = readed
-        self.url = url
-        self.client = client
-        self.file_name = file_name
-        self.started = False
-        self.callback = callback
-        self.callback_args = callback_args
-
-    def update(self, current: int) -> None:
-        self.current = current
-        self.readed += current
-        if self.callback:
-            self.callback(self, *self.callback_args)
-
-
-CtxType = TypeVar("CtxType")
-ResType = TypeVar("ResType")
-HandlerCallback = Callable[[CtxType], Coroutine[Any, Any, ResType]]
-FilterCallback = Callable[[CtxType], Coroutine[Any, Any, bool]]
-DownloadProgressCallback = Callable[[
-    DownloadProgress], Coroutine[Any, Any, None]]
-UploadProgressCallback = Callable[[
-    DownloadProgress], Coroutine[Any, Any, None]]
-
-RT = TypeVar("RT")
-SCT = Union[RT, Collection[RT]]
-"""Single instance or collection of instances."""
-
-JSONDict = Dict[str, Any]
-
-
-class ReadCallbackStream(object):
-    """Wraps a file-like object in another, but also calls a user
-    callback with the number of bytes read whenever its `read()` method
-    is called. Used for tracking upload progress, for example for a
-    progress bar in a UI application. Idea taken from ActiveState Code Recipe:
-    http://code.activestate.com/recipes/578669-wrap-a-string-in-a-file-like-object-that-calls-a-u/
-    """
-
-    def __init__(self, file_like, callback):
-        self.file_like = file_like
-        self.callback = callback
-
-    def __len__(self):
-        raise NotImplementedError()
-
-    def read(self, *args):
-        chunk = self.file_like.read(*args)
-        if len(chunk) > 0:
-            self.callback(len(chunk))
-        return chunk
-
-
-class RequestMethod(Enum):
-    GET = "GET"
-    POST = "POST"
-    PUT = "PUT"
-    PATCH = "PATCH"
-    DELETE = "DELETE"
+from enum import Enum
+from typing import Any, Callable, Collection, Coroutine, Dict, TypeVar, Union
+
+from swibots.error import CancelError
+
+
+class IOClient:
+    def cancel(self) -> None:
+        raise CancelError()
+
+
+class DownloadProgress:
+    def __init__(self, downloaded: int, total: int, url: str, client: IOClient, file_name: str):
+        self.downloaded = downloaded
+        self.total = total
+        self.url = url
+        self.client = client
+        self.file_name = file_name
+        self.started = False
+
+
+class UploadProgress:
+    def __init__(self, current: int, readed: int, url: str, client: IOClient, file_name: str, callback, callback_args):
+        self.current = current
+        self.readed = readed
+        self.url = url
+        self.client = client
+        self.file_name = file_name
+        self.started = False
+        self.callback = callback
+        self.callback_args = callback_args
+
+    def update(self, current: int) -> None:
+        self.current = current
+        self.readed += current
+        if self.callback:
+            self.callback(self, *self.callback_args)
+
+
+CtxType = TypeVar("CtxType")
+ResType = TypeVar("ResType")
+HandlerCallback = Callable[[CtxType], Coroutine[Any, Any, ResType]]
+FilterCallback = Callable[[CtxType], Coroutine[Any, Any, bool]]
+DownloadProgressCallback = Callable[[
+    DownloadProgress], Coroutine[Any, Any, None]]
+UploadProgressCallback = Callable[[
+    DownloadProgress], Coroutine[Any, Any, None]]
+
+RT = TypeVar("RT")
+SCT = Union[RT, Collection[RT]]
+"""Single instance or collection of instances."""
+
+JSONDict = Dict[str, Any]
+
+
+class ReadCallbackStream(object):
+    """Wraps a file-like object in another, but also calls a user
+    callback with the number of bytes read whenever its `read()` method
+    is called. Used for tracking upload progress, for example for a
+    progress bar in a UI application. Idea taken from ActiveState Code Recipe:
+    http://code.activestate.com/recipes/578669-wrap-a-string-in-a-file-like-object-that-calls-a-u/
+    """
+
+    def __init__(self, file_like, callback):
+        self.file_like = file_like
+        self.callback = callback
+
+    def __len__(self):
+        raise NotImplementedError()
+
+    def read(self, *args):
+        chunk = self.file_like.read(*args)
+        if len(chunk) > 0:
+            self.callback(len(chunk))
+        return chunk
+
+
+class RequestMethod(Enum):
+    GET = "GET"
+    POST = "POST"
+    PUT = "PUT"
+    PATCH = "PATCH"
+    DELETE = "DELETE"
```

### Comparing `swibots-1.2.8/swibots/utils/ws/asyncstomp/async_ws_client.py` & `swibots-1.2.9/swibots/utils/ws/asyncstomp/async_ws_client.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,284 +1,284 @@
-import asyncio
-from typing import List
-
-from swibots.error import SwitchError
-
-from .async_ws_subscription import AsyncWsSubscription
-from swibots.utils.ws.common import WsFrame
-import websockets
-import logging
-
-VERSIONS = "1.1,1.0"
-
-log = logging.getLogger(__name__)
-
-class AsyncWsClient:
-    def __init__(
-        self,
-        url: str,
-    ):
-
-        self.url = url
-        self.ws = None
-        self._loop = asyncio.get_event_loop()
-        self.opened = False
-        self.connected = False
-        self.counter = 0
-        self.tasks: List[asyncio.Task] = []
-        self._heartbeatTask = None
-        self.subscriptions: dict[str, AsyncWsSubscription] = {}
-        self._connect_args = None
-        self._connectCallback = None
-        self.errorCallback = None
-        self._connectIntents = 0
-        self._connectInterval = 1
-        self._maxConnectIntents = 0
-        self._connecting = False
-        self._gracefully_disconnect = False
-
-    async def _start_heartbeat(self):
-        elapsed = 0
-        while self.connected:
-            await asyncio.sleep(0.1)
-            elapsed = elapsed + 0.1
-            if elapsed >= 5:
-                await self._transmit("\n", {})
-                elapsed = 0
-        log.debug("Heartbeat stopped")
-
-    async def _on_open(self, ws_app, *args):
-        self.opened = True
-
-    async def _on_close(self, ws_app, *args):
-        self.connected = False
-        if self._gracefully_disconnect:
-            return
-        log.error("Whoops! Lost connection to " + self.url)
-        await self._clean_up()
-        if self._connectIntents >= self._maxConnectIntents and self._maxConnectIntents > 0:
-            log.error("Max connection attempts reached. Aborting.")
-            raise SwitchError("Max connection attempts reached. Aborting.")
-        await asyncio.sleep(self._connectInterval)
-        self._connectIntents = self._connectIntents + 1
-        await self.connect(**self._connect_args)
-
-    async def _on_error(self, ws_app, error, *args):
-        await self._clean_up()
-        await self._on_close(ws_app, *args)
-        log.error(error)
-
-    async def _on_message(self, ws_app, message, *args):
-        frame = WsFrame.unmarshall_single(message)
-
-        if frame.command != "PONG":
-            log.debug("\n<<< " + str(message))
-        else:
-            log.debug("\n<<< " + frame.command)
-
-        _results = []
-        if frame.command == "CONNECTED":
-            self.connected = True
-            self._connecting = False
-            self._connectIntents = 0
-            log.debug("connected to server " + self.url)
-            self._heartbeatTask = self._loop.create_task(self._start_heartbeat())
-            # resubscribe
-            for sub in self.subscriptions.values():
-                await self._start_subscription(sub)
-
-            # if self._connectCallback is not None:
-            #     _results.append(await self._send_heartbeat(frame))
-        elif frame.command == "MESSAGE":
-
-            subscription = frame.headers["subscription"]
-
-            if subscription in self.subscriptions:
-                sub = self.subscriptions[subscription]
-                messageID = frame.headers["message-id"]
-
-                async def ack(headers):
-                    if headers is None:
-                        headers = {}
-                    return await self.ack(messageID, subscription, headers)
-
-                async def nack(headers):
-                    if headers is None:
-                        headers = {}
-                    return await self.nack(messageID, subscription, headers)
-
-                frame.ack = ack
-                frame.nack = nack
-
-                _results.append(self._loop.create_task(sub.receive(frame)))
-            else:
-                info = "Unhandled received MESSAGE: " + str(frame)
-                log.debug(info)
-                _results.append(info)
-        elif frame.command == "RECEIPT":
-            pass
-        elif frame.command == "ERROR":
-            if self.errorCallback is not None:
-                _results.append(self.errorCallback(frame))
-        elif frame.command == "PONG":
-            pass
-        else:
-            info = "Unhandled received MESSAGE: " + frame.command
-            log.debug(info)
-            _results.append(info)
-
-        return _results
-
-    async def _transmit(self, command, headers, body=None):
-        try:
-            if self.ws is None:
-                return
-            out = l = WsFrame.marshall(command, headers, body)
-            if command == "\n":
-                l = "PING"
-                out = command
-            log.debug("\n>>> " + l)
-            await self.ws.send(out)
-        except (websockets.exceptions.WebSocketException):
-            await self._on_close(self.ws)
-        except Exception as e:
-            await self._on_error(self.ws, e)
-
-    async def connect(
-        self,
-        login=None,
-        passcode=None,
-        headers=None,
-        connectCallback=None,
-        errorCallback=None,
-        timeout=0,
-        **kwargs,
-    ):
-        headers = self._set_default_headers(headers)
-        await self._connect(
-            login, passcode, headers, connectCallback, errorCallback, timeout, **kwargs
-        )
-
-    async def _connect(
-        self,
-        login=None,
-        passcode=None,
-        headers=None,
-        connectCallback=None,
-        errorCallback=None,
-        timeout=30,
-        **kwargs,
-    ):
-        if self.connected:
-            log.debug("Already connected to " + self.url)
-            return
-
-        if self._connecting:
-            log.debug("Already connecting to " + self.url)
-            return
-
-        try:
-            self._connecting = True
-            self._connect_args = kwargs
-            log.debug("Opening web socket...")
-            self.ws = await websockets.connect(self.url)
-            log.debug("Web socket opened.")
-            self._loop.create_task(self.read_messages())
-            headers = headers if headers is not None else {}
-            # headers['host'] = self.url
-            headers["accept-version"] = VERSIONS
-            headers["heart-beat"] = "10000,10000"
-            if login is not None:
-                headers["login"] = login
-            if passcode is not None:
-                headers["passcode"] = passcode
-            self._connectCallback = connectCallback
-            self.errorCallback = errorCallback
-            await self._transmit("CONNECT", headers)
-            # elapsed time
-            elapsed = 0
-            while not self.connected:
-                await asyncio.sleep(1)
-                elapsed += 1
-                if timeout > 0 and elapsed > timeout:
-                    raise Exception("Connection timeout")
-        # await self._start_heartbeat()
-        except (websockets.exceptions.WebSocketException,):
-            await self._on_close(self.ws)
-        except Exception as e:
-            await self._on_error(self.ws, e)
-
-    async def read_messages(self):
-        try:
-            async for message in self.ws:
-                await self._on_message(self.ws, message)
-            await self._on_close(self.ws)
-        except (websockets.exceptions.WebSocketException,):
-            await self._on_close(self.ws)
-        except Exception as e:
-            await self._on_error(self.ws, e)
-
-    async def disconnect(self, disconnectCallback=None, headers=None):
-        headers = self._set_default_headers(headers)
-        await self._transmit("DISCONNECT", headers)
-        self._gracefully_disconnect = True
-        await self.ws.close()
-        await self._clean_up()
-        if disconnectCallback is not None:
-            disconnectCallback()
-
-    async def _clean_up(self):
-        try:
-            self.connected = False
-            self._connecting = False
-            self.opened = False
-            # if self._heartbeatTask is not None:
-            #     await asyncio.wait_for(self._heartbeatTask, 5)
-            # [task.cancel() for task in self.tasks]
-            # self.ws = None
-            self.tasks = []
-        except Exception as e:
-            log.debug("Error cleaning up: " + str(e))
-
-    async def send(self, destination, headers=None, body=None):
-        headers = self._set_default_headers(headers)
-        if body is None:
-            body = ""
-        headers["destination"] = destination
-        return await self._transmit("SEND", headers, body)
-
-    async def subscribe(self, destination, callback=None, headers=None):
-        headers = self._set_default_headers(headers)
-        if "id" not in headers or headers["id"] is None or headers["id"] == "":
-            id = "sub-" + str(self.counter)
-            self.counter += 1
-        else:
-            id = headers["id"]
-
-        sub = AsyncWsSubscription(
-            client=self, destination=destination, callback=callback, headers=headers, id=id
-        )
-        await self._start_subscription(sub)
-        self.subscriptions[id] = sub
-        return sub
-
-    def _set_default_headers(self, headers):
-        return headers or {}
-
-    async def _start_subscription(self, subscription: AsyncWsSubscription):
-        return await subscription.start()
-
-    async def unsubscribe(self, id):
-        del self.subscriptions[id]
-        return await self._transmit("UNSUBSCRIBE", {"id": id})
-
-    async def ack(self, message_id, subscription, headers):
-        headers = self._set_default_headers(headers)
-        headers["message-id"] = message_id
-        headers["subscription"] = subscription
-        return await self._transmit("ACK", headers)
-
-    async def nack(self, message_id, subscription, headers):
-        headers = self._set_default_headers(headers)
-        headers["message-id"] = message_id
-        headers["subscription"] = subscription
-        return await self._transmit("NACK", headers)
+import asyncio
+from typing import List
+
+from swibots.error import SwitchError
+
+from .async_ws_subscription import AsyncWsSubscription
+from swibots.utils.ws.common import WsFrame
+import websockets
+import logging
+
+VERSIONS = "1.1,1.0"
+
+log = logging.getLogger(__name__)
+
+class AsyncWsClient:
+    def __init__(
+        self,
+        url: str,
+    ):
+
+        self.url = url
+        self.ws = None
+        self._loop = asyncio.get_event_loop()
+        self.opened = False
+        self.connected = False
+        self.counter = 0
+        self.tasks: List[asyncio.Task] = []
+        self._heartbeatTask = None
+        self.subscriptions: dict[str, AsyncWsSubscription] = {}
+        self._connect_args = None
+        self._connectCallback = None
+        self.errorCallback = None
+        self._connectIntents = 0
+        self._connectInterval = 1
+        self._maxConnectIntents = 0
+        self._connecting = False
+        self._gracefully_disconnect = False
+
+    async def _start_heartbeat(self):
+        elapsed = 0
+        while self.connected:
+            await asyncio.sleep(0.1)
+            elapsed = elapsed + 0.1
+            if elapsed >= 5:
+                await self._transmit("\n", {})
+                elapsed = 0
+        log.debug("Heartbeat stopped")
+
+    async def _on_open(self, ws_app, *args):
+        self.opened = True
+
+    async def _on_close(self, ws_app, *args):
+        self.connected = False
+        if self._gracefully_disconnect:
+            return
+        log.error("Whoops! Lost connection to " + self.url)
+        await self._clean_up()
+        if self._connectIntents >= self._maxConnectIntents and self._maxConnectIntents > 0:
+            log.error("Max connection attempts reached. Aborting.")
+            raise SwitchError("Max connection attempts reached. Aborting.")
+        await asyncio.sleep(self._connectInterval)
+        self._connectIntents = self._connectIntents + 1
+        await self.connect(**self._connect_args)
+
+    async def _on_error(self, ws_app, error, *args):
+        await self._clean_up()
+        await self._on_close(ws_app, *args)
+        log.error(error)
+
+    async def _on_message(self, ws_app, message, *args):
+        frame = WsFrame.unmarshall_single(message)
+
+        if frame.command != "PONG":
+            log.debug("\n<<< " + str(message))
+        else:
+            log.debug("\n<<< " + frame.command)
+
+        _results = []
+        if frame.command == "CONNECTED":
+            self.connected = True
+            self._connecting = False
+            self._connectIntents = 0
+            log.debug("connected to server " + self.url)
+            self._heartbeatTask = self._loop.create_task(self._start_heartbeat())
+            # resubscribe
+            for sub in self.subscriptions.values():
+                await self._start_subscription(sub)
+
+            # if self._connectCallback is not None:
+            #     _results.append(await self._send_heartbeat(frame))
+        elif frame.command == "MESSAGE":
+
+            subscription = frame.headers["subscription"]
+
+            if subscription in self.subscriptions:
+                sub = self.subscriptions[subscription]
+                messageID = frame.headers["message-id"]
+
+                async def ack(headers):
+                    if headers is None:
+                        headers = {}
+                    return await self.ack(messageID, subscription, headers)
+
+                async def nack(headers):
+                    if headers is None:
+                        headers = {}
+                    return await self.nack(messageID, subscription, headers)
+
+                frame.ack = ack
+                frame.nack = nack
+
+                _results.append(self._loop.create_task(sub.receive(frame)))
+            else:
+                info = "Unhandled received MESSAGE: " + str(frame)
+                log.debug(info)
+                _results.append(info)
+        elif frame.command == "RECEIPT":
+            pass
+        elif frame.command == "ERROR":
+            if self.errorCallback is not None:
+                _results.append(self.errorCallback(frame))
+        elif frame.command == "PONG":
+            pass
+        else:
+            info = "Unhandled received MESSAGE: " + frame.command
+            log.debug(info)
+            _results.append(info)
+
+        return _results
+
+    async def _transmit(self, command, headers, body=None):
+        try:
+            if self.ws is None:
+                return
+            out = l = WsFrame.marshall(command, headers, body)
+            if command == "\n":
+                l = "PING"
+                out = command
+            log.debug("\n>>> " + l)
+            await self.ws.send(out)
+        except (websockets.exceptions.WebSocketException):
+            await self._on_close(self.ws)
+        except Exception as e:
+            await self._on_error(self.ws, e)
+
+    async def connect(
+        self,
+        login=None,
+        passcode=None,
+        headers=None,
+        connectCallback=None,
+        errorCallback=None,
+        timeout=0,
+        **kwargs,
+    ):
+        headers = self._set_default_headers(headers)
+        await self._connect(
+            login, passcode, headers, connectCallback, errorCallback, timeout, **kwargs
+        )
+
+    async def _connect(
+        self,
+        login=None,
+        passcode=None,
+        headers=None,
+        connectCallback=None,
+        errorCallback=None,
+        timeout=30,
+        **kwargs,
+    ):
+        if self.connected:
+            log.debug("Already connected to " + self.url)
+            return
+
+        if self._connecting:
+            log.debug("Already connecting to " + self.url)
+            return
+
+        try:
+            self._connecting = True
+            self._connect_args = kwargs
+            log.debug("Opening web socket...")
+            self.ws = await websockets.connect(self.url)
+            log.debug("Web socket opened.")
+            self._loop.create_task(self.read_messages())
+            headers = headers if headers is not None else {}
+            # headers['host'] = self.url
+            headers["accept-version"] = VERSIONS
+            headers["heart-beat"] = "10000,10000"
+            if login is not None:
+                headers["login"] = login
+            if passcode is not None:
+                headers["passcode"] = passcode
+            self._connectCallback = connectCallback
+            self.errorCallback = errorCallback
+            await self._transmit("CONNECT", headers)
+            # elapsed time
+            elapsed = 0
+            while not self.connected:
+                await asyncio.sleep(1)
+                elapsed += 1
+                if timeout > 0 and elapsed > timeout:
+                    raise Exception("Connection timeout")
+        # await self._start_heartbeat()
+        except (websockets.exceptions.WebSocketException,):
+            await self._on_close(self.ws)
+        except Exception as e:
+            await self._on_error(self.ws, e)
+
+    async def read_messages(self):
+        try:
+            async for message in self.ws:
+                await self._on_message(self.ws, message)
+            await self._on_close(self.ws)
+        except (websockets.exceptions.WebSocketException,):
+            await self._on_close(self.ws)
+        except Exception as e:
+            await self._on_error(self.ws, e)
+
+    async def disconnect(self, disconnectCallback=None, headers=None):
+        headers = self._set_default_headers(headers)
+        await self._transmit("DISCONNECT", headers)
+        self._gracefully_disconnect = True
+        await self.ws.close()
+        await self._clean_up()
+        if disconnectCallback is not None:
+            disconnectCallback()
+
+    async def _clean_up(self):
+        try:
+            self.connected = False
+            self._connecting = False
+            self.opened = False
+            # if self._heartbeatTask is not None:
+            #     await asyncio.wait_for(self._heartbeatTask, 5)
+            # [task.cancel() for task in self.tasks]
+            # self.ws = None
+            self.tasks = []
+        except Exception as e:
+            log.debug("Error cleaning up: " + str(e))
+
+    async def send(self, destination, headers=None, body=None):
+        headers = self._set_default_headers(headers)
+        if body is None:
+            body = ""
+        headers["destination"] = destination
+        return await self._transmit("SEND", headers, body)
+
+    async def subscribe(self, destination, callback=None, headers=None):
+        headers = self._set_default_headers(headers)
+        if "id" not in headers or headers["id"] is None or headers["id"] == "":
+            id = "sub-" + str(self.counter)
+            self.counter += 1
+        else:
+            id = headers["id"]
+
+        sub = AsyncWsSubscription(
+            client=self, destination=destination, callback=callback, headers=headers, id=id
+        )
+        await self._start_subscription(sub)
+        self.subscriptions[id] = sub
+        return sub
+
+    def _set_default_headers(self, headers):
+        return headers or {}
+
+    async def _start_subscription(self, subscription: AsyncWsSubscription):
+        return await subscription.start()
+
+    async def unsubscribe(self, id):
+        del self.subscriptions[id]
+        return await self._transmit("UNSUBSCRIBE", {"id": id})
+
+    async def ack(self, message_id, subscription, headers):
+        headers = self._set_default_headers(headers)
+        headers["message-id"] = message_id
+        headers["subscription"] = subscription
+        return await self._transmit("ACK", headers)
+
+    async def nack(self, message_id, subscription, headers):
+        headers = self._set_default_headers(headers)
+        headers["message-id"] = message_id
+        headers["subscription"] = subscription
+        return await self._transmit("NACK", headers)
```

### Comparing `swibots-1.2.8/swibots/utils/ws/asyncstomp/async_ws_subscription.py` & `swibots-1.2.9/swibots/utils/ws/asyncstomp/async_ws_subscription.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from swibots.utils.ws.common import WsMessage
-
-
-class AsyncWsSubscription:
-    def __init__(
-        self, client, destination: str, id: str, headers: dict[str, str] = None, callback=None
-    ):
-        from .async_ws_client import AsyncWsClient
-
-        self.client: AsyncWsClient = client
-        self.destination = destination
-        self.callback = callback
-        self.id = id
-        self.headers = headers or {}
-
-    async def start(self):
-        self.headers["id"] = self.id
-        self.headers["destination"] = self.destination
-        await self.client._transmit("SUBSCRIBE", self.headers)
-
-    async def receive(self, message):
-        if self.callback is not None:
-            await self.callback(WsMessage(message))
-
-    async def send(self, body: str, headers: dict[str, str] = None):
-        headers = headers or {}
-        await self.client.send(self.destination, headers, body)
-
-    async def unsubscribe(self):
-        await self.client.unsubscribe(self.id)
+from swibots.utils.ws.common import WsMessage
+
+
+class AsyncWsSubscription:
+    def __init__(
+        self, client, destination: str, id: str, headers: dict[str, str] = None, callback=None
+    ):
+        from .async_ws_client import AsyncWsClient
+
+        self.client: AsyncWsClient = client
+        self.destination = destination
+        self.callback = callback
+        self.id = id
+        self.headers = headers or {}
+
+    async def start(self):
+        self.headers["id"] = self.id
+        self.headers["destination"] = self.destination
+        await self.client._transmit("SUBSCRIBE", self.headers)
+
+    async def receive(self, message):
+        if self.callback is not None:
+            await self.callback(WsMessage(message))
+
+    async def send(self, body: str, headers: dict[str, str] = None):
+        headers = headers or {}
+        await self.client.send(self.destination, headers, body)
+
+    async def unsubscribe(self):
+        await self.client.unsubscribe(self.id)
```

### Comparing `swibots-1.2.8/swibots.egg-info/SOURCES.txt` & `swibots-1.2.9/swibots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

