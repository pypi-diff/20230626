# Comparing `tmp/pythonmc-1.0.5.tar.gz` & `tmp/pythonmc-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonmc-1.0.5.tar", last modified: Sun Jun 25 17:44:49 2023, max compression
+gzip compressed data, was "pythonmc-1.0.6.tar", last modified: Mon Jun 26 18:02:55 2023, max compression
```

## Comparing `pythonmc-1.0.5.tar` & `pythonmc-1.0.6.tar`

### file list

```diff
@@ -1,92 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.919944 pythonmc-1.0.5/
--rw-rw-rw-   0        0        0     5394 2023-06-25 17:44:49.918936 pythonmc-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2023-06-23 17:56:35.000000 pythonmc-1.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-06-23 19:54:25.000000 pythonmc-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-25 17:44:49.920462 pythonmc-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      792 2023-06-25 17:44:37.000000 pythonmc-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.852601 pythonmc-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.863929 pythonmc-1.0.5/src/pythonmc/
--rw-rw-rw-   0        0        0        0 2023-06-25 17:29:40.000000 pythonmc-1.0.5/src/pythonmc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.872607 pythonmc-1.0.5/src/pythonmc/block/
--rw-rw-rw-   0        0        0      124 2023-06-25 17:22:49.000000 pythonmc-1.0.5/src/pythonmc/block/__init__.py
--rw-rw-rw-   0        0        0      214 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/block/block.py
--rw-rw-rw-   0        0        0      108 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/block/block_pos.py
--rw-rw-rw-   0        0        0      140 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/block/block_state.py
--rw-rw-rw-   0        0        0    28276 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/block/blocks.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.879869 pythonmc-1.0.5/src/pythonmc/entity/
--rw-rw-rw-   0        0        0      259 2023-06-25 17:23:05.000000 pythonmc-1.0.5/src/pythonmc/entity/__init__.py
--rw-rw-rw-   0        0        0       47 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/arm.py
--rw-rw-rw-   0        0        0      519 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/damage_sources.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.881920 pythonmc-1.0.5/src/pythonmc/entity/effects/
--rw-rw-rw-   0        0        0      101 2023-06-25 17:24:15.000000 pythonmc-1.0.5/src/pythonmc/entity/effects/__init__.py
--rw-rw-rw-   0        0        0       72 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/effects/status_effect_instance.py
--rw-rw-rw-   0        0        0      779 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/effects/status_effects.py
--rw-rw-rw-   0        0        0     2713 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/entities.py
--rw-rw-rw-   0        0        0     2946 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/entity.py
--rw-rw-rw-   0        0        0       56 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/hand.py
--rw-rw-rw-   0        0        0     3026 2023-06-25 17:20:49.000000 pythonmc-1.0.5/src/pythonmc/entity/living_entity.py
--rw-rw-rw-   0        0        0      157 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/entity/removal_reasons.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.886518 pythonmc-1.0.5/src/pythonmc/item/
--rw-rw-rw-   0        0        0      185 2023-06-25 17:23:02.000000 pythonmc-1.0.5/src/pythonmc/item/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.890188 pythonmc-1.0.5/src/pythonmc/item/enchantment/
--rw-rw-rw-   0        0        0      129 2023-06-25 17:24:18.000000 pythonmc-1.0.5/src/pythonmc/item/enchantment/__init__.py
--rw-rw-rw-   0        0        0       57 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/enchantment/enchantment.py
--rw-rw-rw-   0        0        0      105 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/enchantment/enchantment_rarity.py
--rw-rw-rw-   0        0        0      923 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/enchantment/enchantments.py
--rw-rw-rw-   0        0        0      195 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/hide_flags.py
--rw-rw-rw-   0        0        0       76 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/item.py
--rw-rw-rw-   0        0        0       93 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/item_rarity.py
--rw-rw-rw-   0        0        0     1680 2023-06-25 17:13:02.000000 pythonmc-1.0.5/src/pythonmc/item/item_stack.py
--rw-rw-rw-   0        0        0    34784 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/item/items.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.894782 pythonmc-1.0.5/src/pythonmc/player/
--rw-rw-rw-   0        0        0      187 2023-06-25 17:22:56.000000 pythonmc-1.0.5/src/pythonmc/player/__init__.py
--rw-rw-rw-   0        0        0       47 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/player/ender_chest_inventory.py
--rw-rw-rw-   0        0        0       95 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/player/hunger_manager.py
--rw-rw-rw-   0        0        0     1261 2023-06-25 17:40:06.000000 pythonmc-1.0.5/src/pythonmc/player/player_entity.py
--rw-rw-rw-   0        0        0     1023 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/player/player_inventory.py
--rw-rw-rw-   0        0        0     1041 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/player/player_manager.py
--rw-rw-rw-   0        0        0        0 2023-06-23 17:56:35.000000 pythonmc-1.0.5/src/pythonmc/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.899953 pythonmc-1.0.5/src/pythonmc/scoreboard/
--rw-rw-rw-   0        0        0      293 2023-06-25 17:22:44.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/__init__.py
--rw-rw-rw-   0        0        0       59 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/render_types.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.902007 pythonmc-1.0.5/src/pythonmc/scoreboard/rules/
--rw-rw-rw-   0        0        0       92 2023-06-25 17:22:58.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/rules/__init__.py
--rw-rw-rw-   0        0        0      115 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/rules/collision_rules.py
--rw-rw-rw-   0        0        0      124 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/rules/visibility_rules.py
--rw-rw-rw-   0        0        0     1078 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard.py
--rw-rw-rw-   0        0        0     1285 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard_criterions.py
--rw-rw-rw-   0        0        0      316 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard_objective.py
--rw-rw-rw-   0        0        0      410 2023-06-25 17:38:22.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard_player_score.py
--rw-rw-rw-   0        0        0     1137 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/scoreboard/team.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.903034 pythonmc-1.0.5/src/pythonmc/server/
--rw-rw-rw-   0        0        0      101 2023-06-25 17:22:25.000000 pythonmc-1.0.5/src/pythonmc/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.905617 pythonmc-1.0.5/src/pythonmc/server/difficulty/
--rw-rw-rw-   0        0        0       76 2023-06-25 17:20:46.000000 pythonmc-1.0.5/src/pythonmc/server/difficulty/__init__.py
--rw-rw-rw-   0        0        0       95 2023-06-25 17:07:51.000000 pythonmc-1.0.5/src/pythonmc/server/difficulty/difficulties.py
--rw-rw-rw-   0        0        0       68 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/difficulty/difficulty.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.907640 pythonmc-1.0.5/src/pythonmc/server/gamemode/
--rw-rw-rw-   0        0        0       68 2023-06-25 17:24:06.000000 pythonmc-1.0.5/src/pythonmc/server/gamemode/__init__.py
--rw-rw-rw-   0        0        0      135 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/gamemode/game_mode.py
--rw-rw-rw-   0        0        0      104 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/gamemode/game_modes.py
--rw-rw-rw-   0        0        0     1138 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/server.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.910199 pythonmc-1.0.5/src/pythonmc/server/text/
--rw-rw-rw-   0        0        0       60 2023-06-25 17:24:23.000000 pythonmc-1.0.5/src/pythonmc/server/text/__init__.py
--rw-rw-rw-   0        0        0      460 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/text/formatting.py
--rw-rw-rw-   0        0        0      140 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/server/text/text.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.915836 pythonmc-1.0.5/src/pythonmc/world/
--rw-rw-rw-   0        0        0      200 2023-06-25 17:22:53.000000 pythonmc-1.0.5/src/pythonmc/world/__init__.py
--rw-rw-rw-   0        0        0      476 2023-06-25 17:37:56.000000 pythonmc-1.0.5/src/pythonmc/world/executor.py
--rw-rw-rw-   0        0        0     2109 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/particles.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.918936 pythonmc-1.0.5/src/pythonmc/world/position/
--rw-rw-rw-   0        0        0       52 2023-06-25 17:20:37.000000 pythonmc-1.0.5/src/pythonmc/world/position/__init__.py
--rw-rw-rw-   0        0        0       88 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/position/vec2f.py
--rw-rw-rw-   0        0        0      105 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/position/vec3d.py
--rw-rw-rw-   0        0        0       85 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/time_.py
--rw-rw-rw-   0        0        0       71 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/weather.py
--rw-rw-rw-   0        0        0     1178 2023-06-25 17:41:28.000000 pythonmc-1.0.5/src/pythonmc/world/world.py
--rw-rw-rw-   0        0        0       72 2023-06-25 17:07:52.000000 pythonmc-1.0.5/src/pythonmc/world/worlds.py
-drwxrwxrwx   0        0        0        0 2023-06-25 17:44:49.868035 pythonmc-1.0.5/src/pythonmc.egg-info/
--rw-rw-rw-   0        0        0     5394 2023-06-25 17:44:49.000000 pythonmc-1.0.5/src/pythonmc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2566 2023-06-25 17:44:49.000000 pythonmc-1.0.5/src/pythonmc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 17:44:49.000000 pythonmc-1.0.5/src/pythonmc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-25 17:44:49.000000 pythonmc-1.0.5/src/pythonmc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.747893 pythonmc-1.0.6/
+-rw-rw-rw-   0        0        0     5394 2023-06-26 18:02:55.746390 pythonmc-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-06-23 17:56:35.000000 pythonmc-1.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-23 19:54:25.000000 pythonmc-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 18:02:55.747893 pythonmc-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-06-26 18:02:43.000000 pythonmc-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.657772 pythonmc-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.669290 pythonmc-1.0.6/src/pythonmc/
+-rw-rw-rw-   0        0        0      212 2023-06-26 17:21:16.000000 pythonmc-1.0.6/src/pythonmc/__init__.py
+-rw-rw-rw-   0        0        0      221 2023-06-25 20:07:44.000000 pythonmc-1.0.6/src/pythonmc/__init__.pyi
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.679802 pythonmc-1.0.6/src/pythonmc/advancement/
+-rw-rw-rw-   0        0        0      261 2023-06-26 17:21:16.000000 pythonmc-1.0.6/src/pythonmc/advancement/__init__.py
+-rw-rw-rw-   0        0        0      136 2023-06-26 16:53:11.000000 pythonmc-1.0.6/src/pythonmc/advancement/advancement.py
+-rw-rw-rw-   0        0        0      145 2023-06-26 17:29:46.000000 pythonmc-1.0.6/src/pythonmc/advancement/advancement_display.py
+-rw-rw-rw-   0        0        0       81 2023-06-26 16:56:37.000000 pythonmc-1.0.6/src/pythonmc/advancement/advancement_frame.py
+-rw-rw-rw-   0        0        0       87 2023-06-26 16:58:02.000000 pythonmc-1.0.6/src/pythonmc/advancement/advancement_rewards.py
+-rw-rw-rw-   0        0        0       55 2023-06-26 17:21:16.000000 pythonmc-1.0.6/src/pythonmc/advancement/operation.py
+-rw-rw-rw-   0        0        0      113 2023-06-26 16:59:08.000000 pythonmc-1.0.6/src/pythonmc/advancement/selection.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.684805 pythonmc-1.0.6/src/pythonmc/block/
+-rw-rw-rw-   0        0        0      124 2023-06-25 17:22:49.000000 pythonmc-1.0.6/src/pythonmc/block/__init__.py
+-rw-rw-rw-   0        0        0      222 2023-06-26 15:56:31.000000 pythonmc-1.0.6/src/pythonmc/block/block.py
+-rw-rw-rw-   0        0        0      116 2023-06-26 15:54:31.000000 pythonmc-1.0.6/src/pythonmc/block/block_pos.py
+-rw-rw-rw-   0        0        0      148 2023-06-26 15:56:31.000000 pythonmc-1.0.6/src/pythonmc/block/block_state.py
+-rw-rw-rw-   0        0        0    28276 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/block/blocks.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.693319 pythonmc-1.0.6/src/pythonmc/entity/
+-rw-rw-rw-   0        0        0      259 2023-06-25 17:23:05.000000 pythonmc-1.0.6/src/pythonmc/entity/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/entity/arm.py
+-rw-rw-rw-   0        0        0      519 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/entity/damage_sources.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.696319 pythonmc-1.0.6/src/pythonmc/entity/effects/
+-rw-rw-rw-   0        0        0      101 2023-06-25 17:24:15.000000 pythonmc-1.0.6/src/pythonmc/entity/effects/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/entity/effects/status_effect_instance.py
+-rw-rw-rw-   0        0        0      779 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/entity/effects/status_effects.py
+-rw-rw-rw-   0        0        0     2713 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/entity/entities.py
+-rw-rw-rw-   0        0        0     2954 2023-06-26 15:54:31.000000 pythonmc-1.0.6/src/pythonmc/entity/entity.py
+-rw-rw-rw-   0        0        0       56 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/entity/hand.py
+-rw-rw-rw-   0        0        0     3026 2023-06-25 17:20:49.000000 pythonmc-1.0.6/src/pythonmc/entity/living_entity.py
+-rw-rw-rw-   0        0        0      157 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/entity/removal_reasons.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.702830 pythonmc-1.0.6/src/pythonmc/item/
+-rw-rw-rw-   0        0        0      185 2023-06-25 17:23:02.000000 pythonmc-1.0.6/src/pythonmc/item/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.705829 pythonmc-1.0.6/src/pythonmc/item/enchantment/
+-rw-rw-rw-   0        0        0      129 2023-06-25 17:24:18.000000 pythonmc-1.0.6/src/pythonmc/item/enchantment/__init__.py
+-rw-rw-rw-   0        0        0       57 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/item/enchantment/enchantment.py
+-rw-rw-rw-   0        0        0      105 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/item/enchantment/enchantment_rarity.py
+-rw-rw-rw-   0        0        0      923 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/item/enchantment/enchantments.py
+-rw-rw-rw-   0        0        0      195 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/item/hide_flags.py
+-rw-rw-rw-   0        0        0       84 2023-06-26 15:56:31.000000 pythonmc-1.0.6/src/pythonmc/item/item.py
+-rw-rw-rw-   0        0        0       93 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/item/item_rarity.py
+-rw-rw-rw-   0        0        0     1712 2023-06-26 15:56:31.000000 pythonmc-1.0.6/src/pythonmc/item/item_stack.py
+-rw-rw-rw-   0        0        0    34784 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/item/items.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.708338 pythonmc-1.0.6/src/pythonmc/other/
+-rw-rw-rw-   0        0        0       35 2023-06-26 17:21:16.000000 pythonmc-1.0.6/src/pythonmc/other/__init__.py
+-rw-rw-rw-   0        0        0      123 2023-06-26 15:54:31.000000 pythonmc-1.0.6/src/pythonmc/other/identifier.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.714342 pythonmc-1.0.6/src/pythonmc/player/
+-rw-rw-rw-   0        0        0      187 2023-06-25 17:22:56.000000 pythonmc-1.0.6/src/pythonmc/player/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/player/ender_chest_inventory.py
+-rw-rw-rw-   0        0        0       95 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/player/hunger_manager.py
+-rw-rw-rw-   0        0        0     1261 2023-06-25 17:40:06.000000 pythonmc-1.0.6/src/pythonmc/player/player_entity.py
+-rw-rw-rw-   0        0        0     1023 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/player/player_inventory.py
+-rw-rw-rw-   0        0        0     1041 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/player/player_manager.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 17:56:35.000000 pythonmc-1.0.6/src/pythonmc/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.720857 pythonmc-1.0.6/src/pythonmc/scoreboard/
+-rw-rw-rw-   0        0        0      293 2023-06-25 17:22:44.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/__init__.py
+-rw-rw-rw-   0        0        0       59 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/render_types.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.724856 pythonmc-1.0.6/src/pythonmc/scoreboard/rules/
+-rw-rw-rw-   0        0        0       92 2023-06-25 17:22:58.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/rules/__init__.py
+-rw-rw-rw-   0        0        0      115 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/rules/collision_rules.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/rules/visibility_rules.py
+-rw-rw-rw-   0        0        0     1078 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/scoreboard.py
+-rw-rw-rw-   0        0        0     1285 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/scoreboard_criterions.py
+-rw-rw-rw-   0        0        0      316 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/scoreboard_objective.py
+-rw-rw-rw-   0        0        0      410 2023-06-25 17:38:22.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/scoreboard_player_score.py
+-rw-rw-rw-   0        0        0     1137 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/scoreboard/team.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.725855 pythonmc-1.0.6/src/pythonmc/server_/
+-rw-rw-rw-   0        0        0      101 2023-06-25 17:22:25.000000 pythonmc-1.0.6/src/pythonmc/server_/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.729365 pythonmc-1.0.6/src/pythonmc/server_/difficulty/
+-rw-rw-rw-   0        0        0       76 2023-06-25 17:20:46.000000 pythonmc-1.0.6/src/pythonmc/server_/difficulty/__init__.py
+-rw-rw-rw-   0        0        0       95 2023-06-25 17:07:51.000000 pythonmc-1.0.6/src/pythonmc/server_/difficulty/difficulties.py
+-rw-rw-rw-   0        0        0       68 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/server_/difficulty/difficulty.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.733368 pythonmc-1.0.6/src/pythonmc/server_/gamemode/
+-rw-rw-rw-   0        0        0       68 2023-06-25 17:24:06.000000 pythonmc-1.0.6/src/pythonmc/server_/gamemode/__init__.py
+-rw-rw-rw-   0        0        0      135 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/server_/gamemode/game_mode.py
+-rw-rw-rw-   0        0        0      104 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/server_/gamemode/game_modes.py
+-rw-rw-rw-   0        0        0     1138 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/server_/server.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.735371 pythonmc-1.0.6/src/pythonmc/server_/text/
+-rw-rw-rw-   0        0        0       60 2023-06-25 17:24:23.000000 pythonmc-1.0.6/src/pythonmc/server_/text/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/server_/text/formatting.py
+-rw-rw-rw-   0        0        0      148 2023-06-26 15:54:31.000000 pythonmc-1.0.6/src/pythonmc/server_/text/text.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.742389 pythonmc-1.0.6/src/pythonmc/world/
+-rw-rw-rw-   0        0        0      200 2023-06-25 17:22:53.000000 pythonmc-1.0.6/src/pythonmc/world/__init__.py
+-rw-rw-rw-   0        0        0      476 2023-06-25 17:37:56.000000 pythonmc-1.0.6/src/pythonmc/world/executor.py
+-rw-rw-rw-   0        0        0     2109 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/world/particles.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.745390 pythonmc-1.0.6/src/pythonmc/world/position/
+-rw-rw-rw-   0        0        0       52 2023-06-25 17:20:37.000000 pythonmc-1.0.6/src/pythonmc/world/position/__init__.py
+-rw-rw-rw-   0        0        0       96 2023-06-26 15:54:31.000000 pythonmc-1.0.6/src/pythonmc/world/position/vec2f.py
+-rw-rw-rw-   0        0        0      113 2023-06-26 15:54:31.000000 pythonmc-1.0.6/src/pythonmc/world/position/vec3d.py
+-rw-rw-rw-   0        0        0       85 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/world/time_.py
+-rw-rw-rw-   0        0        0       71 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/world/weather.py
+-rw-rw-rw-   0        0        0     1436 2023-06-25 21:14:00.000000 pythonmc-1.0.6/src/pythonmc/world/world.py
+-rw-rw-rw-   0        0        0       72 2023-06-25 17:07:52.000000 pythonmc-1.0.6/src/pythonmc/world/worlds.py
+drwxrwxrwx   0        0        0        0 2023-06-26 18:02:55.674294 pythonmc-1.0.6/src/pythonmc.egg-info/
+-rw-rw-rw-   0        0        0     5394 2023-06-26 18:02:55.000000 pythonmc-1.0.6/src/pythonmc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2962 2023-06-26 18:02:55.000000 pythonmc-1.0.6/src/pythonmc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 18:02:55.000000 pythonmc-1.0.6/src/pythonmc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 18:02:55.000000 pythonmc-1.0.6/src/pythonmc.egg-info/top_level.txt
```

### Comparing `pythonmc-1.0.5/PKG-INFO` & `pythonmc-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.5
+Version: 1.0.6
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.5 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.6 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
```

### Comparing `pythonmc-1.0.5/README.md` & `pythonmc-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/setup.py` & `pythonmc-1.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pythonmc",
-    version="1.0.5",
+    version="1.0.6",
     author="RevolvingMadness",
     author_email="revolvingmad@gmail.com",
     description="The python library for PythonMC",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/RevolvingMadness/PythonMC",
     project_urls={"Bug Tracker": "https://github.com/RevolvingMadness/PythonMC/issues"},
@@ -14,9 +14,9 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages("src"),
     package_dir={"": "src"},
     python_requires=">=3.9",
-    package_data={"pythonmc": ["py.typed"]},
+    package_data={"pythonmc": ["py.typed", "**/py.typed", "*.pyi", "**/.pyi"]},
 )
```

### Comparing `pythonmc-1.0.5/src/pythonmc/block/blocks.py` & `pythonmc-1.0.6/src/pythonmc/block/blocks.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/entity/damage_sources.py` & `pythonmc-1.0.6/src/pythonmc/entity/damage_sources.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/entity/effects/status_effects.py` & `pythonmc-1.0.6/src/pythonmc/entity/effects/status_effects.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/entity/entities.py` & `pythonmc-1.0.6/src/pythonmc/entity/entities.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/entity/entity.py` & `pythonmc-1.0.6/src/pythonmc/entity/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 class Entity:
-    def __init__(self, entity, world):
+    def __init__(self, entity, world) -> None:
         ...
 
     def addVelocity(self, velocity):
         ...
 
     def canFreeze(self):
         ...
```

### Comparing `pythonmc-1.0.5/src/pythonmc/entity/living_entity.py` & `pythonmc-1.0.6/src/pythonmc/entity/living_entity.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/item/enchantment/enchantments.py` & `pythonmc-1.0.6/src/pythonmc/item/enchantment/enchantments.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/item/item_stack.py` & `pythonmc-1.0.6/src/pythonmc/item/item_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import overload
 
 
 class ItemStack:
     @overload
-    def __init__(self, item, count, nbt):
+    def __init__(self, item, count, nbt) -> None:
         ...
 
     @overload
-    def __init__(self, item, nbt):
+    def __init__(self, item, nbt) -> None:
         ...
 
     @overload
-    def __init__(self, item, count):
+    def __init__(self, item, count) -> None:
         ...
 
     @overload
-    def __init__(self, item):
+    def __init__(self, item) -> None:
         ...
 
     def addEnchantment(self, enchantment, level):
         ...
 
     def addHideFlag(self, hideFlag):
         ...
```

### Comparing `pythonmc-1.0.5/src/pythonmc/item/items.py` & `pythonmc-1.0.6/src/pythonmc/item/items.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/player/player_entity.py` & `pythonmc-1.0.6/src/pythonmc/player/player_entity.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/player/player_inventory.py` & `pythonmc-1.0.6/src/pythonmc/player/player_inventory.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/player/player_manager.py` & `pythonmc-1.0.6/src/pythonmc/player/player_manager.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard.py` & `pythonmc-1.0.6/src/pythonmc/scoreboard/scoreboard.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/scoreboard/scoreboard_criterions.py` & `pythonmc-1.0.6/src/pythonmc/scoreboard/scoreboard_criterions.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/scoreboard/team.py` & `pythonmc-1.0.6/src/pythonmc/scoreboard/team.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/server/server.py` & `pythonmc-1.0.6/src/pythonmc/server_/server.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/world/particles.py` & `pythonmc-1.0.6/src/pythonmc/world/particles.py`

 * *Files identical despite different names*

### Comparing `pythonmc-1.0.5/src/pythonmc/world/world.py` & `pythonmc-1.0.6/src/pythonmc/world/world.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,30 @@
     def getBlock(self, x, y, z):
         ...
 
     @overload
     def getBlock(self, blockPos):
         ...
 
+    @overload
+    def getBlock(self, vec3d):
+        ...
+
+    def getAllPlayers(self):
+        ...
+
+    def getAllEntities(self):
+        ...
+
+    def getNearestPlayer(self, position):
+        ...
+
+    def getRandomPlayer(self):
+        ...
+
     def getDifficulty(self):
         ...
 
     def getSeed(self):
         ...
 
     @overload
```

### Comparing `pythonmc-1.0.5/src/pythonmc.egg-info/PKG-INFO` & `pythonmc-1.0.6/src/pythonmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonmc
-Version: 1.0.5
+Version: 1.0.6
 Summary: The python library for PythonMC
 Home-page: https://github.com/RevolvingMadness/PythonMC
 Author: RevolvingMadness
 Author-email: revolvingmad@gmail.com
 Project-URL: Bug Tracker, https://github.com/RevolvingMadness/PythonMC/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pythonmc Version: 1.0.5 Summary: The python library
+Metadata-Version: 2.1 Name: pythonmc Version: 1.0.6 Summary: The python library
 for PythonMC Home-page: https://github.com/RevolvingMadness/PythonMC Author:
 RevolvingMadness Author-email: revolvingmad@gmail.com Project-URL: Bug Tracker,
 https://github.com/RevolvingMadness/PythonMC/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
 Description-Content-Type: text/markdown  [![Contributors][contributors-shield]]
 [contributors-url] [![Forks][forks-shield]][forks-url] [![Stargazers][stars-
```

### Comparing `pythonmc-1.0.5/src/pythonmc.egg-info/SOURCES.txt` & `pythonmc-1.0.6/src/pythonmc.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 README.md
 pyproject.toml
 setup.py
 src/pythonmc/__init__.py
+src/pythonmc/__init__.pyi
 src/pythonmc/py.typed
 src/pythonmc.egg-info/PKG-INFO
 src/pythonmc.egg-info/SOURCES.txt
 src/pythonmc.egg-info/dependency_links.txt
 src/pythonmc.egg-info/top_level.txt
+src/pythonmc/advancement/__init__.py
+src/pythonmc/advancement/advancement.py
+src/pythonmc/advancement/advancement_display.py
+src/pythonmc/advancement/advancement_frame.py
+src/pythonmc/advancement/advancement_rewards.py
+src/pythonmc/advancement/operation.py
+src/pythonmc/advancement/selection.py
 src/pythonmc/block/__init__.py
 src/pythonmc/block/block.py
 src/pythonmc/block/block_pos.py
 src/pythonmc/block/block_state.py
 src/pythonmc/block/blocks.py
 src/pythonmc/entity/__init__.py
 src/pythonmc/entity/arm.py
@@ -29,14 +37,16 @@
 src/pythonmc/item/item_rarity.py
 src/pythonmc/item/item_stack.py
 src/pythonmc/item/items.py
 src/pythonmc/item/enchantment/__init__.py
 src/pythonmc/item/enchantment/enchantment.py
 src/pythonmc/item/enchantment/enchantment_rarity.py
 src/pythonmc/item/enchantment/enchantments.py
+src/pythonmc/other/__init__.py
+src/pythonmc/other/identifier.py
 src/pythonmc/player/__init__.py
 src/pythonmc/player/ender_chest_inventory.py
 src/pythonmc/player/hunger_manager.py
 src/pythonmc/player/player_entity.py
 src/pythonmc/player/player_inventory.py
 src/pythonmc/player/player_manager.py
 src/pythonmc/scoreboard/__init__.py
@@ -45,25 +55,25 @@
 src/pythonmc/scoreboard/scoreboard_criterions.py
 src/pythonmc/scoreboard/scoreboard_objective.py
 src/pythonmc/scoreboard/scoreboard_player_score.py
 src/pythonmc/scoreboard/team.py
 src/pythonmc/scoreboard/rules/__init__.py
 src/pythonmc/scoreboard/rules/collision_rules.py
 src/pythonmc/scoreboard/rules/visibility_rules.py
-src/pythonmc/server/__init__.py
-src/pythonmc/server/server.py
-src/pythonmc/server/difficulty/__init__.py
-src/pythonmc/server/difficulty/difficulties.py
-src/pythonmc/server/difficulty/difficulty.py
-src/pythonmc/server/gamemode/__init__.py
-src/pythonmc/server/gamemode/game_mode.py
-src/pythonmc/server/gamemode/game_modes.py
-src/pythonmc/server/text/__init__.py
-src/pythonmc/server/text/formatting.py
-src/pythonmc/server/text/text.py
+src/pythonmc/server_/__init__.py
+src/pythonmc/server_/server.py
+src/pythonmc/server_/difficulty/__init__.py
+src/pythonmc/server_/difficulty/difficulties.py
+src/pythonmc/server_/difficulty/difficulty.py
+src/pythonmc/server_/gamemode/__init__.py
+src/pythonmc/server_/gamemode/game_mode.py
+src/pythonmc/server_/gamemode/game_modes.py
+src/pythonmc/server_/text/__init__.py
+src/pythonmc/server_/text/formatting.py
+src/pythonmc/server_/text/text.py
 src/pythonmc/world/__init__.py
 src/pythonmc/world/executor.py
 src/pythonmc/world/particles.py
 src/pythonmc/world/time_.py
 src/pythonmc/world/weather.py
 src/pythonmc/world/world.py
 src/pythonmc/world/worlds.py
```

