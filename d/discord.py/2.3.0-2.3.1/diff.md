# Comparing `tmp/discord.py-2.3.0.tar.gz` & `tmp/discord.py-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord.py-2.3.0.tar", last modified: Mon Jun 12 17:42:22 2023, max compression
+gzip compressed data, was "discord.py-2.3.1.tar", last modified: Mon Jun 26 08:15:10 2023, max compression
```

## Comparing `discord.py-2.3.0.tar` & `discord.py-2.3.1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.709865 discord.py-2.3.0/
--rw-rw-rw-   0        0        0     1081 2021-02-02 07:58:56.000000 discord.py-2.3.0/LICENSE
--rw-rw-rw-   0        0        0      111 2021-08-22 06:25:27.000000 discord.py-2.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4212 2023-06-12 17:42:22.708865 discord.py-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2945 2023-02-11 23:42:40.000000 discord.py-2.3.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.573744 discord.py-2.3.0/discord/
--rw-rw-rw-   0        0        0     1886 2023-06-12 17:40:31.000000 discord.py-2.3.0/discord/__init__.py
--rw-rw-rw-   0        0        0    11051 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/__main__.py
--rw-rw-rw-   0        0        0     1410 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/_types.py
--rw-rw-rw-   0        0        0    65844 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/abc.py
--rw-rw-rw-   0        0        0    26864 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/activity.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.610777 discord.py-2.3.0/discord/app_commands/
--rw-rw-rw-   0        0        0      424 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/__init__.py
--rw-rw-rw-   0        0        0    18077 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/checks.py
--rw-rw-rw-   0        0        0    94536 2023-05-03 00:13:10.000000 discord.py-2.3.0/discord/app_commands/commands.py
--rw-rw-rw-   0        0        0    19006 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/errors.py
--rw-rw-rw-   0        0        0    38502 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/app_commands/models.py
--rw-rw-rw-   0        0        0    13123 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/namespace.py
--rw-rw-rw-   0        0        0    32512 2023-06-04 11:51:52.000000 discord.py-2.3.0/discord/app_commands/transformers.py
--rw-rw-rw-   0        0        0    10686 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/app_commands/translator.py
--rw-rw-rw-   0        0        0    47965 2023-02-25 10:27:47.000000 discord.py-2.3.0/discord/app_commands/tree.py
--rw-rw-rw-   0        0        0    12713 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/appinfo.py
--rw-rw-rw-   0        0        0    15837 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/asset.py
--rw-rw-rw-   0        0        0    35367 2023-05-04 02:39:48.000000 discord.py-2.3.0/discord/audit_logs.py
--rw-rw-rw-   0        0        0    23833 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/automod.py
--rw-rw-rw-   0        0        0     3751 2022-02-22 03:41:08.000000 discord.py-2.3.0/discord/backoff.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.655817 discord.py-2.3.0/discord/bin/
--rw-rw-rw-   0        0        0   441856 2021-02-02 07:58:56.000000 discord.py-2.3.0/discord/bin/libopus-0.x64.dll
--rw-rw-rw-   0        0        0   366080 2021-02-02 07:58:56.000000 discord.py-2.3.0/discord/bin/libopus-0.x86.dll
--rw-rw-rw-   0        0        0   116803 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/channel.py
--rw-rw-rw-   0        0        0    85400 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/client.py
--rw-rw-rw-   0        0        0    14403 2023-06-08 02:11:50.000000 discord.py-2.3.0/discord/colour.py
--rw-rw-rw-   0        0        0    16836 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/components.py
--rw-rw-rw-   0        0        0     3032 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/context_managers.py
--rw-rw-rw-   0        0        0    22722 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/embeds.py
--rw-rw-rw-   0        0        0     8574 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/emoji.py
--rw-rw-rw-   0        0        0    22242 2023-06-08 02:11:39.000000 discord.py-2.3.0/discord/enums.py
--rw-rw-rw-   0        0        0     8952 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/errors.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.493673 discord.py-2.3.0/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.670831 discord.py-2.3.0/discord/ext/commands/
--rw-rw-rw-   0        0        0      437 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/__init__.py
--rw-rw-rw-   0        0        0     2638 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/_types.py
--rw-rw-rw-   0        0        0    51719 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/bot.py
--rw-rw-rw-   0        0        0    30245 2023-06-04 11:51:24.000000 discord.py-2.3.0/discord/ext/commands/cog.py
--rw-rw-rw-   0        0        0    40048 2023-05-20 01:12:09.000000 discord.py-2.3.0/discord/ext/commands/context.py
--rw-rw-rw-   0        0        0    45846 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/ext/commands/converter.py
--rw-rw-rw-   0        0        0     9716 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/cooldowns.py
--rw-rw-rw-   0        0        0    89619 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/ext/commands/core.py
--rw-rw-rw-   0        0        0    36450 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/ext/commands/errors.py
--rw-rw-rw-   0        0        0    22966 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/flags.py
--rw-rw-rw-   0        0        0    57732 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/ext/commands/help.py
--rw-rw-rw-   0        0        0    36595 2023-03-02 03:47:33.000000 discord.py-2.3.0/discord/ext/commands/hybrid.py
--rw-rw-rw-   0        0        0     9157 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/ext/commands/parameters.py
--rw-rw-rw-   0        0        0     6247 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/commands/view.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.671832 discord.py-2.3.0/discord/ext/tasks/
--rw-rw-rw-   0        0        0    29180 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ext/tasks/__init__.py
--rw-rw-rw-   0        0        0     5378 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/file.py
--rw-rw-rw-   0        0        0    54264 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/flags.py
--rw-rw-rw-   0        0        0    35191 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/gateway.py
--rw-rw-rw-   0        0        0   150174 2023-06-11 17:58:37.000000 discord.py-2.3.0/discord/guild.py
--rw-rw-rw-   0        0        0    90056 2023-06-08 01:54:09.000000 discord.py-2.3.0/discord/http.py
--rw-rw-rw-   0        0        0    13334 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/integrations.py
--rw-rw-rw-   0        0        0    45093 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/interactions.py
--rw-rw-rw-   0        0        0    20595 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/invite.py
--rw-rw-rw-   0        0        0    41018 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/member.py
--rw-rw-rw-   0        0        0     5592 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/mentions.py
--rw-rw-rw-   0        0        0    85375 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/message.py
--rw-rw-rw-   0        0        0     1485 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/mixins.py
--rw-rw-rw-   0        0        0     3702 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/object.py
--rw-rw-rw-   0        0        0     3646 2022-02-20 10:26:28.000000 discord.py-2.3.0/discord/oggparse.py
--rw-rw-rw-   0        0        0    15233 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/opus.py
--rw-rw-rw-   0        0        0     7950 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/partial_emoji.py
--rw-rw-rw-   0        0        0    30153 2023-06-11 17:51:43.000000 discord.py-2.3.0/discord/permissions.py
--rw-rw-rw-   0        0        0    26498 2023-06-04 11:51:24.000000 discord.py-2.3.0/discord/player.py
--rw-rw-rw-   0        0        0        0 2021-08-22 06:25:27.000000 discord.py-2.3.0/discord/py.typed
--rw-rw-rw-   0        0        0    16826 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/raw_models.py
--rw-rw-rw-   0        0        0     8207 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/reaction.py
--rw-rw-rw-   0        0        0    17906 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/role.py
--rw-rw-rw-   0        0        0    23629 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/scheduled_event.py
--rw-rw-rw-   0        0        0    20129 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/shard.py
--rw-rw-rw-   0        0        0     6498 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/stage_instance.py
--rw-rw-rw-   0        0        0    73376 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/state.py
--rw-rw-rw-   0        0        0    16039 2023-05-01 21:59:43.000000 discord.py-2.3.0/discord/sticker.py
--rw-rw-rw-   0        0        0     4792 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/team.py
--rw-rw-rw-   0        0        0     9574 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/template.py
--rw-rw-rw-   0        0        0    32456 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/threads.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.698855 discord.py-2.3.0/discord/types/
--rw-rw-rw-   0        0        0      149 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/__init__.py
--rw-rw-rw-   0        0        0     2707 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/activity.py
--rw-rw-rw-   0        0        0     2487 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/types/appinfo.py
--rw-rw-rw-   0        0        0     8192 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/audit_log.py
--rw-rw-rw-   0        0        0     4009 2023-02-27 01:22:42.000000 discord.py-2.3.0/discord/types/automod.py
--rw-rw-rw-   0        0        0     4804 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/types/channel.py
--rw-rw-rw-   0        0        0     6266 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/command.py
--rw-rw-rw-   0        0        0     3057 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/components.py
--rw-rw-rw-   0        0        0     2329 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/embed.py
--rw-rw-rw-   0        0        0     1528 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/emoji.py
--rw-rw-rw-   0        0        0     8453 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/gateway.py
--rw-rw-rw-   0        0        0     5279 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/types/guild.py
--rw-rw-rw-   0        0        0     2288 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/integration.py
--rw-rw-rw-   0        0        0     7046 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/types/interactions.py
--rw-rw-rw-   0        0        0     2704 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/invite.py
--rw-rw-rw-   0        0        0     1898 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/member.py
--rw-rw-rw-   0        0        0     4251 2023-05-03 00:12:57.000000 discord.py-2.3.0/discord/types/message.py
--rw-rw-rw-   0        0        0     1746 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/role.py
--rw-rw-rw-   0        0        0     3294 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/scheduled_event.py
--rw-rw-rw-   0        0        0     1182 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/snowflake.py
--rw-rw-rw-   0        0        0     2257 2023-05-01 21:59:43.000000 discord.py-2.3.0/discord/types/sticker.py
--rw-rw-rw-   0        0        0     1499 2022-02-20 10:26:29.000000 discord.py-2.3.0/discord/types/team.py
--rw-rw-rw-   0        0        0     1609 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/template.py
--rw-rw-rw-   0        0        0     2454 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/threads.py
--rw-rw-rw-   0        0        0     1572 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/types/user.py
--rw-rw-rw-   0        0        0     2268 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/voice.py
--rw-rw-rw-   0        0        0     1978 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/webhook.py
--rw-rw-rw-   0        0        0     1460 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/types/welcome_screen.py
--rw-rw-rw-   0        0        0     1883 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/types/widget.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.704861 discord.py-2.3.0/discord/ui/
--rw-rw-rw-   0        0        0      285 2022-02-20 10:13:32.000000 discord.py-2.3.0/discord/ui/__init__.py
--rw-rw-rw-   0        0        0    10620 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/ui/button.py
--rw-rw-rw-   0        0        0     4372 2023-03-02 00:44:50.000000 discord.py-2.3.0/discord/ui/item.py
--rw-rw-rw-   0        0        0     7035 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/ui/modal.py
--rw-rw-rw-   0        0        0    34030 2023-06-04 11:51:24.000000 discord.py-2.3.0/discord/ui/select.py
--rw-rw-rw-   0        0        0     8092 2023-06-04 11:53:08.000000 discord.py-2.3.0/discord/ui/text_input.py
--rw-rw-rw-   0        0        0    22878 2023-02-14 04:54:29.000000 discord.py-2.3.0/discord/ui/view.py
--rw-rw-rw-   0        0        0    16504 2023-06-08 02:12:29.000000 discord.py-2.3.0/discord/user.py
--rw-rw-rw-   0        0        0    41506 2023-05-20 01:21:20.000000 discord.py-2.3.0/discord/utils.py
--rw-rw-rw-   0        0        0    24974 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/voice_client.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.707863 discord.py-2.3.0/discord/webhook/
--rw-rw-rw-   0        0        0      182 2021-08-15 18:01:53.000000 discord.py-2.3.0/discord/webhook/__init__.py
--rw-rw-rw-   0        0        0    69729 2023-06-11 16:41:04.000000 discord.py-2.3.0/discord/webhook/async_.py
--rw-rw-rw-   0        0        0    42586 2023-05-20 00:58:46.000000 discord.py-2.3.0/discord/webhook/sync.py
--rw-rw-rw-   0        0        0     7539 2023-02-11 23:42:40.000000 discord.py-2.3.0/discord/welcome_screen.py
--rw-rw-rw-   0        0        0    10426 2023-05-20 00:59:19.000000 discord.py-2.3.0/discord/widget.py
-drwxrwxrwx   0        0        0        0 2023-06-12 17:42:22.599767 discord.py-2.3.0/discord.py.egg-info/
--rw-rw-rw-   0        0        0     4212 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3070 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      330 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-12 17:42:22.000000 discord.py-2.3.0/discord.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      869 2023-02-11 23:42:40.000000 discord.py-2.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       18 2023-02-11 23:42:40.000000 discord.py-2.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 17:42:22.709865 discord.py-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2946 2023-02-11 23:42:40.000000 discord.py-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:10.085263 discord.py-2.3.1/
+-rw-rw-rw-   0        0        0     1081 2021-02-02 07:58:56.000000 discord.py-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0      111 2021-08-22 06:25:27.000000 discord.py-2.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4212 2023-06-26 08:15:10.085263 discord.py-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2945 2023-02-11 23:42:40.000000 discord.py-2.3.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:09.947140 discord.py-2.3.1/discord/
+-rw-rw-rw-   0        0        0     1886 2023-06-26 08:14:59.000000 discord.py-2.3.1/discord/__init__.py
+-rw-rw-rw-   0        0        0    11051 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/__main__.py
+-rw-rw-rw-   0        0        0     1410 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/_types.py
+-rw-rw-rw-   0        0        0    65844 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/abc.py
+-rw-rw-rw-   0        0        0    26864 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/activity.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:09.960151 discord.py-2.3.1/discord/app_commands/
+-rw-rw-rw-   0        0        0      424 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/app_commands/__init__.py
+-rw-rw-rw-   0        0        0    18077 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/app_commands/checks.py
+-rw-rw-rw-   0        0        0    94536 2023-05-03 00:13:10.000000 discord.py-2.3.1/discord/app_commands/commands.py
+-rw-rw-rw-   0        0        0    19006 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/app_commands/errors.py
+-rw-rw-rw-   0        0        0    38502 2023-05-03 00:12:57.000000 discord.py-2.3.1/discord/app_commands/models.py
+-rw-rw-rw-   0        0        0    13123 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/app_commands/namespace.py
+-rw-rw-rw-   0        0        0    32512 2023-06-04 11:51:52.000000 discord.py-2.3.1/discord/app_commands/transformers.py
+-rw-rw-rw-   0        0        0    10686 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/app_commands/translator.py
+-rw-rw-rw-   0        0        0    47965 2023-02-25 10:27:47.000000 discord.py-2.3.1/discord/app_commands/tree.py
+-rw-rw-rw-   0        0        0    12713 2023-05-03 00:12:57.000000 discord.py-2.3.1/discord/appinfo.py
+-rw-rw-rw-   0        0        0    15837 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/asset.py
+-rw-rw-rw-   0        0        0    35367 2023-05-04 02:39:48.000000 discord.py-2.3.1/discord/audit_logs.py
+-rw-rw-rw-   0        0        0    23833 2023-05-03 00:12:57.000000 discord.py-2.3.1/discord/automod.py
+-rw-rw-rw-   0        0        0     3751 2022-02-22 03:41:08.000000 discord.py-2.3.1/discord/backoff.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:10.004190 discord.py-2.3.1/discord/bin/
+-rw-rw-rw-   0        0        0   441856 2021-02-02 07:58:56.000000 discord.py-2.3.1/discord/bin/libopus-0.x64.dll
+-rw-rw-rw-   0        0        0   366080 2021-02-02 07:58:56.000000 discord.py-2.3.1/discord/bin/libopus-0.x86.dll
+-rw-rw-rw-   0        0        0   116803 2023-05-20 00:58:46.000000 discord.py-2.3.1/discord/channel.py
+-rw-rw-rw-   0        0        0    85400 2023-05-20 00:58:46.000000 discord.py-2.3.1/discord/client.py
+-rw-rw-rw-   0        0        0    14403 2023-06-08 02:11:50.000000 discord.py-2.3.1/discord/colour.py
+-rw-rw-rw-   0        0        0    16850 2023-06-23 04:19:57.000000 discord.py-2.3.1/discord/components.py
+-rw-rw-rw-   0        0        0     3032 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/context_managers.py
+-rw-rw-rw-   0        0        0    22722 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/embeds.py
+-rw-rw-rw-   0        0        0     8574 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/emoji.py
+-rw-rw-rw-   0        0        0    22242 2023-06-08 02:11:39.000000 discord.py-2.3.1/discord/enums.py
+-rw-rw-rw-   0        0        0     8952 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/errors.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:09.854057 discord.py-2.3.1/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:10.020204 discord.py-2.3.1/discord/ext/commands/
+-rw-rw-rw-   0        0        0      437 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/ext/commands/__init__.py
+-rw-rw-rw-   0        0        0     2638 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/ext/commands/_types.py
+-rw-rw-rw-   0        0        0    51719 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/ext/commands/bot.py
+-rw-rw-rw-   0        0        0    30245 2023-06-04 11:51:24.000000 discord.py-2.3.1/discord/ext/commands/cog.py
+-rw-rw-rw-   0        0        0    40048 2023-05-20 01:12:09.000000 discord.py-2.3.1/discord/ext/commands/context.py
+-rw-rw-rw-   0        0        0    46172 2023-06-26 07:58:08.000000 discord.py-2.3.1/discord/ext/commands/converter.py
+-rw-rw-rw-   0        0        0     9716 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/ext/commands/cooldowns.py
+-rw-rw-rw-   0        0        0    89619 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/ext/commands/core.py
+-rw-rw-rw-   0        0        0    36450 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/ext/commands/errors.py
+-rw-rw-rw-   0        0        0    22966 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/ext/commands/flags.py
+-rw-rw-rw-   0        0        0    57732 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/ext/commands/help.py
+-rw-rw-rw-   0        0        0    36595 2023-03-02 03:47:33.000000 discord.py-2.3.1/discord/ext/commands/hybrid.py
+-rw-rw-rw-   0        0        0     9157 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/ext/commands/parameters.py
+-rw-rw-rw-   0        0        0     6247 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/ext/commands/view.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:10.021205 discord.py-2.3.1/discord/ext/tasks/
+-rw-rw-rw-   0        0        0    29180 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/ext/tasks/__init__.py
+-rw-rw-rw-   0        0        0     5378 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/file.py
+-rw-rw-rw-   0        0        0    54264 2023-05-20 00:59:19.000000 discord.py-2.3.1/discord/flags.py
+-rw-rw-rw-   0        0        0    35191 2023-06-17 05:28:55.000000 discord.py-2.3.1/discord/gateway.py
+-rw-rw-rw-   0        0        0   150337 2023-06-12 23:38:42.000000 discord.py-2.3.1/discord/guild.py
+-rw-rw-rw-   0        0        0    90056 2023-06-08 01:54:09.000000 discord.py-2.3.1/discord/http.py
+-rw-rw-rw-   0        0        0    13334 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/integrations.py
+-rw-rw-rw-   0        0        0    45246 2023-06-23 04:19:57.000000 discord.py-2.3.1/discord/interactions.py
+-rw-rw-rw-   0        0        0    20595 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/invite.py
+-rw-rw-rw-   0        0        0    41018 2023-05-20 00:59:19.000000 discord.py-2.3.1/discord/member.py
+-rw-rw-rw-   0        0        0     5592 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/mentions.py
+-rw-rw-rw-   0        0        0    85375 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/message.py
+-rw-rw-rw-   0        0        0     1485 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/mixins.py
+-rw-rw-rw-   0        0        0     3702 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/object.py
+-rw-rw-rw-   0        0        0     3646 2022-02-20 10:26:28.000000 discord.py-2.3.1/discord/oggparse.py
+-rw-rw-rw-   0        0        0    15233 2023-05-20 00:58:46.000000 discord.py-2.3.1/discord/opus.py
+-rw-rw-rw-   0        0        0     7954 2023-06-23 04:19:22.000000 discord.py-2.3.1/discord/partial_emoji.py
+-rw-rw-rw-   0        0        0    30153 2023-06-11 17:51:43.000000 discord.py-2.3.1/discord/permissions.py
+-rw-rw-rw-   0        0        0    26498 2023-06-04 11:51:24.000000 discord.py-2.3.1/discord/player.py
+-rw-rw-rw-   0        0        0        0 2021-08-22 06:25:27.000000 discord.py-2.3.1/discord/py.typed
+-rw-rw-rw-   0        0        0    16826 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/raw_models.py
+-rw-rw-rw-   0        0        0     8207 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/reaction.py
+-rw-rw-rw-   0        0        0    17906 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/role.py
+-rw-rw-rw-   0        0        0    23629 2023-05-03 00:12:57.000000 discord.py-2.3.1/discord/scheduled_event.py
+-rw-rw-rw-   0        0        0    20129 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/shard.py
+-rw-rw-rw-   0        0        0     6498 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/stage_instance.py
+-rw-rw-rw-   0        0        0    73376 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/state.py
+-rw-rw-rw-   0        0        0    16039 2023-05-01 21:59:43.000000 discord.py-2.3.1/discord/sticker.py
+-rw-rw-rw-   0        0        0     4792 2023-05-20 00:59:19.000000 discord.py-2.3.1/discord/team.py
+-rw-rw-rw-   0        0        0     9574 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/template.py
+-rw-rw-rw-   0        0        0    32456 2023-05-03 00:12:57.000000 discord.py-2.3.1/discord/threads.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:10.075254 discord.py-2.3.1/discord/types/
+-rw-rw-rw-   0        0        0      149 2021-08-15 18:01:53.000000 discord.py-2.3.1/discord/types/__init__.py
+-rw-rw-rw-   0        0        0     2707 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/activity.py
+-rw-rw-rw-   0        0        0     2487 2023-05-03 00:12:57.000000 discord.py-2.3.1/discord/types/appinfo.py
+-rw-rw-rw-   0        0        0     8192 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/audit_log.py
+-rw-rw-rw-   0        0        0     4009 2023-02-27 01:22:42.000000 discord.py-2.3.1/discord/types/automod.py
+-rw-rw-rw-   0        0        0     4804 2023-05-20 00:58:46.000000 discord.py-2.3.1/discord/types/channel.py
+-rw-rw-rw-   0        0        0     6266 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/command.py
+-rw-rw-rw-   0        0        0     3057 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/components.py
+-rw-rw-rw-   0        0        0     2329 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/embed.py
+-rw-rw-rw-   0        0        0     1528 2021-08-15 18:01:53.000000 discord.py-2.3.1/discord/types/emoji.py
+-rw-rw-rw-   0        0        0     8453 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/gateway.py
+-rw-rw-rw-   0        0        0     5279 2023-05-03 00:12:57.000000 discord.py-2.3.1/discord/types/guild.py
+-rw-rw-rw-   0        0        0     2288 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/integration.py
+-rw-rw-rw-   0        0        0     7046 2023-05-20 00:58:46.000000 discord.py-2.3.1/discord/types/interactions.py
+-rw-rw-rw-   0        0        0     2704 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/invite.py
+-rw-rw-rw-   0        0        0     1898 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/member.py
+-rw-rw-rw-   0        0        0     4251 2023-05-03 00:12:57.000000 discord.py-2.3.1/discord/types/message.py
+-rw-rw-rw-   0        0        0     1746 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/role.py
+-rw-rw-rw-   0        0        0     3294 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/scheduled_event.py
+-rw-rw-rw-   0        0        0     1182 2021-08-15 18:01:53.000000 discord.py-2.3.1/discord/types/snowflake.py
+-rw-rw-rw-   0        0        0     2257 2023-05-01 21:59:43.000000 discord.py-2.3.1/discord/types/sticker.py
+-rw-rw-rw-   0        0        0     1499 2022-02-20 10:26:29.000000 discord.py-2.3.1/discord/types/team.py
+-rw-rw-rw-   0        0        0     1609 2021-08-15 18:01:53.000000 discord.py-2.3.1/discord/types/template.py
+-rw-rw-rw-   0        0        0     2454 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/threads.py
+-rw-rw-rw-   0        0        0     1572 2023-05-20 00:59:19.000000 discord.py-2.3.1/discord/types/user.py
+-rw-rw-rw-   0        0        0     2268 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/voice.py
+-rw-rw-rw-   0        0        0     1978 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/webhook.py
+-rw-rw-rw-   0        0        0     1460 2021-08-15 18:01:53.000000 discord.py-2.3.1/discord/types/welcome_screen.py
+-rw-rw-rw-   0        0        0     1883 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/types/widget.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:10.081259 discord.py-2.3.1/discord/ui/
+-rw-rw-rw-   0        0        0      285 2022-02-20 10:13:32.000000 discord.py-2.3.1/discord/ui/__init__.py
+-rw-rw-rw-   0        0        0    10620 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/ui/button.py
+-rw-rw-rw-   0        0        0     4372 2023-03-02 00:44:50.000000 discord.py-2.3.1/discord/ui/item.py
+-rw-rw-rw-   0        0        0     7035 2023-05-20 00:58:46.000000 discord.py-2.3.1/discord/ui/modal.py
+-rw-rw-rw-   0        0        0    34030 2023-06-04 11:51:24.000000 discord.py-2.3.1/discord/ui/select.py
+-rw-rw-rw-   0        0        0     8092 2023-06-04 11:53:08.000000 discord.py-2.3.1/discord/ui/text_input.py
+-rw-rw-rw-   0        0        0    22878 2023-02-14 04:54:29.000000 discord.py-2.3.1/discord/ui/view.py
+-rw-rw-rw-   0        0        0    16504 2023-06-08 02:12:29.000000 discord.py-2.3.1/discord/user.py
+-rw-rw-rw-   0        0        0    41506 2023-05-20 01:21:20.000000 discord.py-2.3.1/discord/utils.py
+-rw-rw-rw-   0        0        0    24974 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/voice_client.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:10.084262 discord.py-2.3.1/discord/webhook/
+-rw-rw-rw-   0        0        0      182 2021-08-15 18:01:53.000000 discord.py-2.3.1/discord/webhook/__init__.py
+-rw-rw-rw-   0        0        0    69729 2023-06-11 16:41:04.000000 discord.py-2.3.1/discord/webhook/async_.py
+-rw-rw-rw-   0        0        0    42586 2023-05-20 00:58:46.000000 discord.py-2.3.1/discord/webhook/sync.py
+-rw-rw-rw-   0        0        0     7539 2023-02-11 23:42:40.000000 discord.py-2.3.1/discord/welcome_screen.py
+-rw-rw-rw-   0        0        0    10426 2023-05-20 00:59:19.000000 discord.py-2.3.1/discord/widget.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:15:09.951143 discord.py-2.3.1/discord.py.egg-info/
+-rw-rw-rw-   0        0        0     4212 2023-06-26 08:15:08.000000 discord.py-2.3.1/discord.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3070 2023-06-26 08:15:08.000000 discord.py-2.3.1/discord.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:15:08.000000 discord.py-2.3.1/discord.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      330 2023-06-26 08:15:08.000000 discord.py-2.3.1/discord.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-26 08:15:08.000000 discord.py-2.3.1/discord.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      869 2023-02-11 23:42:40.000000 discord.py-2.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       18 2023-02-11 23:42:40.000000 discord.py-2.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:15:10.086264 discord.py-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2946 2023-02-11 23:42:40.000000 discord.py-2.3.1/setup.py
```

### Comparing `discord.py-2.3.0/LICENSE` & `discord.py-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/PKG-INFO` & `discord.py-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord.py
-Version: 2.3.0
+Version: 2.3.1
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/Rapptz/discord.py
 Author: Rapptz
 License: MIT
 Project-URL: Documentation, https://discordpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Rapptz/discord.py/issues
 Platform: UNKNOWN
```

### Comparing `discord.py-2.3.0/README.rst` & `discord.py-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/__init__.py` & `discord.py-2.3.1/discord/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 """
 
 __title__ = 'discord'
 __author__ = 'Rapptz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2015-present Rapptz'
-__version__ = '2.3.0'
+__version__ = '2.3.1'
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
 import logging
 from typing import NamedTuple, Literal
 
 from .client import *
@@ -74,12 +74,12 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=2, minor=3, micro=0, releaselevel='final', serial=0)
+version_info: VersionInfo = VersionInfo(major=2, minor=3, micro=1, releaselevel='final', serial=0)
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 del logging, NamedTuple, Literal, VersionInfo
```

### Comparing `discord.py-2.3.0/discord/__main__.py` & `discord.py-2.3.1/discord/__main__.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/_types.py` & `discord.py-2.3.1/discord/_types.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/abc.py` & `discord.py-2.3.1/discord/abc.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/activity.py` & `discord.py-2.3.1/discord/activity.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/app_commands/checks.py` & `discord.py-2.3.1/discord/app_commands/checks.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/app_commands/commands.py` & `discord.py-2.3.1/discord/app_commands/commands.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/app_commands/errors.py` & `discord.py-2.3.1/discord/app_commands/errors.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/app_commands/models.py` & `discord.py-2.3.1/discord/app_commands/models.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/app_commands/namespace.py` & `discord.py-2.3.1/discord/app_commands/namespace.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/app_commands/transformers.py` & `discord.py-2.3.1/discord/app_commands/transformers.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/app_commands/translator.py` & `discord.py-2.3.1/discord/app_commands/translator.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/app_commands/tree.py` & `discord.py-2.3.1/discord/app_commands/tree.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/appinfo.py` & `discord.py-2.3.1/discord/appinfo.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/asset.py` & `discord.py-2.3.1/discord/asset.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/audit_logs.py` & `discord.py-2.3.1/discord/audit_logs.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/automod.py` & `discord.py-2.3.1/discord/automod.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/backoff.py` & `discord.py-2.3.1/discord/backoff.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/bin/libopus-0.x64.dll` & `discord.py-2.3.1/discord/bin/libopus-0.x64.dll`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/bin/libopus-0.x86.dll` & `discord.py-2.3.1/discord/bin/libopus-0.x86.dll`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/channel.py` & `discord.py-2.3.1/discord/channel.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/client.py` & `discord.py-2.3.1/discord/client.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/colour.py` & `discord.py-2.3.1/discord/colour.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/components.py` & `discord.py-2.3.1/discord/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,11 +523,11 @@
 
 
 def _component_factory(data: ComponentPayload) -> Optional[Union[ActionRow, ActionRowChildComponentType]]:
     if data['type'] == 1:
         return ActionRow(data)
     elif data['type'] == 2:
         return Button(data)
-    elif data['type'] == 3:
-        return SelectMenu(data)
     elif data['type'] == 4:
         return TextInput(data)
+    elif data['type'] in (3, 5, 6, 7, 8):
+        return SelectMenu(data)
```

### Comparing `discord.py-2.3.0/discord/context_managers.py` & `discord.py-2.3.1/discord/context_managers.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/embeds.py` & `discord.py-2.3.1/discord/embeds.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/emoji.py` & `discord.py-2.3.1/discord/emoji.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/enums.py` & `discord.py-2.3.1/discord/enums.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/errors.py` & `discord.py-2.3.1/discord/errors.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/_types.py` & `discord.py-2.3.1/discord/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/bot.py` & `discord.py-2.3.1/discord/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/cog.py` & `discord.py-2.3.1/discord/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/context.py` & `discord.py-2.3.1/discord/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/converter.py` & `discord.py-2.3.1/discord/ext/commands/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,17 +184,17 @@
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by mention.
     3. Lookup by username#discriminator (deprecated).
     4. Lookup by username#0 (deprecated, only gets users that migrated from their discriminator).
-    5. Lookup by guild nickname.
+    5. Lookup by user name.
     6. Lookup by global name.
-    7. Lookup by user name.
+    7. Lookup by guild nickname.
 
     .. versionchanged:: 1.5
          Raise :exc:`.MemberNotFound` instead of generic :exc:`.BadArgument`
 
     .. versionchanged:: 1.5.1
         This converter now lazily fetches members from the gateway and HTTP APIs,
         optionally caching the result if :attr:`.MemberCacheFlags.joined` is enabled.
@@ -203,20 +203,25 @@
         Looking up users by discriminator will be removed in a future version due to
         the removal of discriminators in an API change.
     """
 
     async def query_member_named(self, guild: discord.Guild, argument: str) -> Optional[discord.Member]:
         cache = guild._state.member_cache_flags.joined
         username, _, discriminator = argument.rpartition('#')
+
+        # If # isn't found then "discriminator" actually has the username
+        if not username:
+            discriminator, username = username, discriminator
+
         if discriminator == '0' or (len(discriminator) == 4 and discriminator.isdigit()):
             lookup = username
             predicate = lambda m: m.name == username and m.discriminator == discriminator
         else:
             lookup = argument
-            predicate = lambda m: m.nick == argument or m.global_name == argument or m.name == argument
+            predicate = lambda m: m.name == argument or m.global_name == argument or m.nick == argument
 
         members = await guild.query_members(lookup, limit=100, cache=cache)
         return discord.utils.find(predicate, members)
 
     async def query_member_by_id(self, bot: _Bot, guild: discord.Guild, user_id: int) -> Optional[discord.Member]:
         ws = bot._get_websocket(shard_id=guild.shard_id)
         cache = guild._state.member_cache_flags.joined
@@ -280,16 +285,16 @@
 
     The lookup strategy is as follows (in order):
 
     1. Lookup by ID.
     2. Lookup by mention.
     3. Lookup by username#discriminator (deprecated).
     4. Lookup by username#0 (deprecated, only gets users that migrated from their discriminator).
-    5. Lookup by global name.
-    6. Lookup by user name.
+    5. Lookup by user name.
+    6. Lookup by global name.
 
     .. versionchanged:: 1.5
          Raise :exc:`.UserNotFound` instead of generic :exc:`.BadArgument`
 
     .. versionchanged:: 1.6
         This converter now lazily fetches users from the HTTP APIs if an ID is passed
         and it's not available in cache.
@@ -312,18 +317,23 @@
                     result = await ctx.bot.fetch_user(user_id)
                 except discord.HTTPException:
                     raise UserNotFound(argument) from None
 
             return result  # type: ignore
 
         username, _, discriminator = argument.rpartition('#')
+
+        # If # isn't found then "discriminator" actually has the username
+        if not username:
+            discriminator, username = username, discriminator
+
         if discriminator == '0' or (len(discriminator) == 4 and discriminator.isdigit()):
             predicate = lambda u: u.name == username and u.discriminator == discriminator
         else:
-            predicate = lambda u: u.global_name == argument or u.name == argument
+            predicate = lambda u: u.name == argument or u.global_name == argument
 
         result = discord.utils.find(predicate, state._users.values())
         if result is None:
             raise UserNotFound(argument)
 
         return result
```

### Comparing `discord.py-2.3.0/discord/ext/commands/cooldowns.py` & `discord.py-2.3.1/discord/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/core.py` & `discord.py-2.3.1/discord/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/errors.py` & `discord.py-2.3.1/discord/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/flags.py` & `discord.py-2.3.1/discord/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/help.py` & `discord.py-2.3.1/discord/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/hybrid.py` & `discord.py-2.3.1/discord/ext/commands/hybrid.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/parameters.py` & `discord.py-2.3.1/discord/ext/commands/parameters.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/commands/view.py` & `discord.py-2.3.1/discord/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ext/tasks/__init__.py` & `discord.py-2.3.1/discord/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/file.py` & `discord.py-2.3.1/discord/file.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/flags.py` & `discord.py-2.3.1/discord/flags.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/gateway.py` & `discord.py-2.3.1/discord/gateway.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/guild.py` & `discord.py-2.3.1/discord/guild.py`

 * *Files 0% similar despite different names*

```diff
@@ -1100,14 +1100,19 @@
             The member in this guild with the associated name. If not found
             then ``None`` is returned.
         """
 
         members = self.members
 
         username, _, discriminator = name.rpartition('#')
+
+        # If # isn't found then "discriminator" actually has the username
+        if not username:
+            discriminator, username = username, discriminator
+
         if discriminator == '0' or (len(discriminator) == 4 and discriminator.isdigit()):
             return utils.find(lambda m: m.name == username and m.discriminator == discriminator, members)
 
         def pred(m: Member) -> bool:
             return m.nick == name or m.global_name == name or m.name == name
 
         return utils.find(pred, members)
```

### Comparing `discord.py-2.3.0/discord/http.py` & `discord.py-2.3.1/discord/http.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/integrations.py` & `discord.py-2.3.1/discord/integrations.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/interactions.py` & `discord.py-2.3.1/discord/interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,53 +180,55 @@
         self.id: int = int(data['id'])
         self.type: InteractionType = try_enum(InteractionType, data['type'])
         self.data: Optional[InteractionData] = data.get('data')
         self.token: str = data['token']
         self.version: int = data['version']
         self.guild_id: Optional[int] = utils._get_as_snowflake(data, 'guild_id')
         self.channel: Optional[InteractionChannel] = None
-
-        raw_channel = data.get('channel', {})
-        raw_ch_type = raw_channel.get('type')
-        if raw_ch_type is not None:
-            factory, ch_type = _threaded_channel_factory(raw_ch_type)  # type is never None
-            if factory is None:
-                logging.info('Unknown channel type {type} for channel ID {id}.'.format_map(raw_channel))
-            else:
-                if ch_type in (ChannelType.group, ChannelType.private):
-                    channel = factory(me=self._client.user, data=raw_channel, state=self._state)  # type: ignore
-                else:
-                    guild = self._state._get_or_create_unavailable_guild(self.guild_id)  # type: ignore
-                    channel = factory(guild=guild, state=self._state, data=raw_channel)  # type: ignore
-
-                self.channel = channel
-
         self.application_id: int = int(data['application_id'])
 
         self.locale: Locale = try_enum(Locale, data.get('locale', 'en-US'))
         self.guild_locale: Optional[Locale]
         try:
             self.guild_locale = try_enum(Locale, data['guild_locale'])
         except KeyError:
             self.guild_locale = None
 
+        guild = None
+        if self.guild_id:
+            guild = self._state._get_or_create_unavailable_guild(self.guild_id)
+
+        raw_channel = data.get('channel', {})
+        channel_id = utils._get_as_snowflake(raw_channel, 'id')
+        if channel_id is not None and guild is not None:
+            self.channel = guild and guild._resolve_channel(channel_id)
+
+        raw_ch_type = raw_channel.get('type')
+        if self.channel is None and raw_ch_type is not None:
+            factory, ch_type = _threaded_channel_factory(raw_ch_type)  # type is never None
+            if factory is None:
+                logging.info('Unknown channel type {type} for channel ID {id}.'.format_map(raw_channel))
+            else:
+                if ch_type in (ChannelType.group, ChannelType.private):
+                    self.channel = factory(me=self._client.user, data=raw_channel, state=self._state)  # type: ignore
+                elif guild is not None:
+                    self.channel = factory(guild=guild, state=self._state, data=raw_channel)  # type: ignore
+
         self.message: Optional[Message]
         try:
             # The channel and message payloads are mismatched yet handled properly at runtime
             self.message = Message(state=self._state, channel=self.channel, data=data['message'])  # type: ignore
         except KeyError:
             self.message = None
 
         self.user: Union[User, Member] = MISSING
         self._permissions: int = 0
         self._app_permissions: int = int(data.get('app_permissions', 0))
 
-        if self.guild_id:
-            guild = self._state._get_or_create_unavailable_guild(self.guild_id)
-
+        if guild is not None:
             # Upgrade Message.guild in case it's missing with partial guild data
             if self.message is not None and self.message.guild is None:
                 self.message.guild = guild
 
             try:
                 member = data['member']  # type: ignore # The key is optional and handled
             except KeyError:
```

### Comparing `discord.py-2.3.0/discord/invite.py` & `discord.py-2.3.1/discord/invite.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/member.py` & `discord.py-2.3.1/discord/member.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/mentions.py` & `discord.py-2.3.1/discord/mentions.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/message.py` & `discord.py-2.3.1/discord/message.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/mixins.py` & `discord.py-2.3.1/discord/mixins.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/object.py` & `discord.py-2.3.1/discord/object.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/oggparse.py` & `discord.py-2.3.1/discord/oggparse.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/opus.py` & `discord.py-2.3.1/discord/opus.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/partial_emoji.py` & `discord.py-2.3.1/discord/partial_emoji.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         Whether the emoji is animated or not.
     id: Optional[:class:`int`]
         The ID of the custom emoji, if applicable.
     """
 
     __slots__ = ('animated', 'name', 'id', '_state')
 
-    _CUSTOM_EMOJI_RE = re.compile(r'<?(?P<animated>a)?:?(?P<name>[A-Za-z0-9\_]+):(?P<id>[0-9]{13,20})>?')
+    _CUSTOM_EMOJI_RE = re.compile(r'<?(?:(?P<animated>a)?:)?(?P<name>[A-Za-z0-9\_]+):(?P<id>[0-9]{13,20})>?')
 
     if TYPE_CHECKING:
         id: Optional[int]
 
     def __init__(self, *, name: str, animated: bool = False, id: Optional[int] = None):
         self.animated: bool = animated
         self.name: str = name
```

### Comparing `discord.py-2.3.0/discord/permissions.py` & `discord.py-2.3.1/discord/permissions.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/player.py` & `discord.py-2.3.1/discord/player.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/raw_models.py` & `discord.py-2.3.1/discord/raw_models.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/reaction.py` & `discord.py-2.3.1/discord/reaction.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/role.py` & `discord.py-2.3.1/discord/role.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/scheduled_event.py` & `discord.py-2.3.1/discord/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/shard.py` & `discord.py-2.3.1/discord/shard.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/stage_instance.py` & `discord.py-2.3.1/discord/stage_instance.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/state.py` & `discord.py-2.3.1/discord/state.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/sticker.py` & `discord.py-2.3.1/discord/sticker.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/team.py` & `discord.py-2.3.1/discord/team.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/template.py` & `discord.py-2.3.1/discord/template.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/threads.py` & `discord.py-2.3.1/discord/threads.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/activity.py` & `discord.py-2.3.1/discord/types/activity.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/appinfo.py` & `discord.py-2.3.1/discord/types/appinfo.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/audit_log.py` & `discord.py-2.3.1/discord/types/audit_log.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/automod.py` & `discord.py-2.3.1/discord/types/automod.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/channel.py` & `discord.py-2.3.1/discord/types/channel.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/command.py` & `discord.py-2.3.1/discord/types/command.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/components.py` & `discord.py-2.3.1/discord/types/components.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/embed.py` & `discord.py-2.3.1/discord/types/embed.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/emoji.py` & `discord.py-2.3.1/discord/types/emoji.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/gateway.py` & `discord.py-2.3.1/discord/types/gateway.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/guild.py` & `discord.py-2.3.1/discord/types/guild.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/integration.py` & `discord.py-2.3.1/discord/types/integration.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/interactions.py` & `discord.py-2.3.1/discord/types/interactions.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/invite.py` & `discord.py-2.3.1/discord/types/invite.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/member.py` & `discord.py-2.3.1/discord/types/member.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/message.py` & `discord.py-2.3.1/discord/types/message.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/role.py` & `discord.py-2.3.1/discord/types/role.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/scheduled_event.py` & `discord.py-2.3.1/discord/types/scheduled_event.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/snowflake.py` & `discord.py-2.3.1/discord/types/snowflake.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/sticker.py` & `discord.py-2.3.1/discord/types/sticker.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/team.py` & `discord.py-2.3.1/discord/types/team.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/template.py` & `discord.py-2.3.1/discord/types/template.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/threads.py` & `discord.py-2.3.1/discord/types/threads.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/user.py` & `discord.py-2.3.1/discord/types/user.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/voice.py` & `discord.py-2.3.1/discord/types/voice.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/webhook.py` & `discord.py-2.3.1/discord/types/webhook.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/welcome_screen.py` & `discord.py-2.3.1/discord/types/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/types/widget.py` & `discord.py-2.3.1/discord/types/widget.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ui/button.py` & `discord.py-2.3.1/discord/ui/button.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ui/item.py` & `discord.py-2.3.1/discord/ui/item.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ui/modal.py` & `discord.py-2.3.1/discord/ui/modal.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ui/select.py` & `discord.py-2.3.1/discord/ui/select.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ui/text_input.py` & `discord.py-2.3.1/discord/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/ui/view.py` & `discord.py-2.3.1/discord/ui/view.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/user.py` & `discord.py-2.3.1/discord/user.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/utils.py` & `discord.py-2.3.1/discord/utils.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/voice_client.py` & `discord.py-2.3.1/discord/voice_client.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/webhook/async_.py` & `discord.py-2.3.1/discord/webhook/async_.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/webhook/sync.py` & `discord.py-2.3.1/discord/webhook/sync.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/welcome_screen.py` & `discord.py-2.3.1/discord/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord/widget.py` & `discord.py-2.3.1/discord/widget.py`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/discord.py.egg-info/PKG-INFO` & `discord.py-2.3.1/discord.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord.py
-Version: 2.3.0
+Version: 2.3.1
 Summary: A Python wrapper for the Discord API
 Home-page: https://github.com/Rapptz/discord.py
 Author: Rapptz
 License: MIT
 Project-URL: Documentation, https://discordpy.readthedocs.io/en/latest/
 Project-URL: Issue tracker, https://github.com/Rapptz/discord.py/issues
 Platform: UNKNOWN
```

### Comparing `discord.py-2.3.0/discord.py.egg-info/SOURCES.txt` & `discord.py-2.3.1/discord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/pyproject.toml` & `discord.py-2.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `discord.py-2.3.0/setup.py` & `discord.py-2.3.1/setup.py`

 * *Files identical despite different names*

