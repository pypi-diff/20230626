# Comparing `tmp/babyrobot-1.0.8.tar.gz` & `tmp/babyrobot-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/babyrobot-1.0.8.tar", last modified: Sun Aug 21 10:03:14 2022, max compression
+gzip compressed data, was "babyrobot-1.0.9.tar", last modified: Wed Aug 24 07:54:42 2022, max compression
```

## Comparing `babyrobot-1.0.8.tar` & `babyrobot-1.0.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-21 10:03:14.000000 babyrobot-1.0.8/
--rw-rw-r--   0 steve     (1000) steve     (1000)     1073 2022-05-10 10:05:37.000000 babyrobot-1.0.8/LICENSE
--rw-rw-r--   0 steve     (1000) steve     (1000)       81 2022-05-15 17:47:19.000000 babyrobot-1.0.8/MANIFEST.in
--rw-rw-r--   0 steve     (1000) steve     (1000)     4427 2022-08-21 10:03:14.000000 babyrobot-1.0.8/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)     3988 2022-07-28 20:11:03.000000 babyrobot-1.0.8/README.md
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot/
--rw-rw-r--   0 steve     (1000) steve     (1000)      938 2022-08-15 16:54:05.000000 babyrobot-1.0.8/babyrobot/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      159 2022-08-21 10:02:48.000000 babyrobot-1.0.8/babyrobot/_version.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot/envs/
--rw-rw-r--   0 steve     (1000) steve     (1000)      627 2022-08-16 07:26:07.000000 babyrobot-1.0.8/babyrobot/envs/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      388 2022-05-27 07:46:46.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v0.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     1247 2022-05-27 07:41:18.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v1.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2074 2022-05-24 17:15:30.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v2.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     1157 2022-07-20 16:45:41.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v3.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3221 2022-07-27 19:45:48.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v4.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      759 2022-07-24 13:10:50.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v5.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     1486 2022-07-24 13:10:15.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v6.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5848 2022-07-27 20:36:55.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v7.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5004 2022-08-16 16:30:08.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_interface.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     2262 2022-08-16 10:36:55.000000 babyrobot-1.0.8/babyrobot/envs/baby_robot_v0.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot/envs/lib/
--rw-rw-r--   0 steve     (1000) steve     (1000)      266 2022-05-20 12:21:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/__init__.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      278 2022-05-15 10:21:05.000000 babyrobot-1.0.8/babyrobot/envs/lib/actions.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3328 2022-05-15 10:35:12.000000 babyrobot-1.0.8/babyrobot/envs/lib/arrows.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3557 2022-08-19 16:26:48.000000 babyrobot-1.0.8/babyrobot/envs/lib/direction.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    22794 2022-08-16 18:30:50.000000 babyrobot-1.0.8/babyrobot/envs/lib/draw_grid.py
--rw-rw-r--   0 steve     (1000) steve     (1000)    11998 2022-08-20 11:38:46.000000 babyrobot-1.0.8/babyrobot/envs/lib/draw_info.py
--rw-rw-r--   0 steve     (1000) steve     (1000)      561 2022-07-24 13:13:14.000000 babyrobot-1.0.8/babyrobot/envs/lib/dynamic_space.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     7450 2022-08-16 18:29:19.000000 babyrobot-1.0.8/babyrobot/envs/lib/grid_base.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     3909 2022-07-26 18:08:29.000000 babyrobot-1.0.8/babyrobot/envs/lib/grid_info.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     5580 2022-08-20 10:01:13.000000 babyrobot-1.0.8/babyrobot/envs/lib/grid_level.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/
--rw-rw-r--   0 steve     (1000) steve     (1000)    16805 2022-05-10 07:49:32.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/BabyRobot64_Sprites.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1985 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_0.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1991 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_1.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1934 2022-08-17 12:31:03.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_10.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1880 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_2.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1882 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_3.png
--rw-rw-r--   0 steve     (1000) steve     (1000)      980 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_4.png
--rw-rw-r--   0 steve     (1000) steve     (1000)      979 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_5.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1815 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_6.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1822 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_7.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1924 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_8.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1934 2022-05-11 10:59:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_9.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     4026 2022-05-20 11:39:38.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/big_puddle.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     1737 2022-05-20 11:39:38.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/small_puddle.png
--rw-rw-r--   0 steve     (1000) steve     (1000)     4026 2022-05-10 07:49:32.000000 babyrobot-1.0.8/babyrobot/envs/lib/images/splash_2.png
--rw-------   0 steve     (1000) steve     (1000)     9276 2022-05-10 07:49:32.000000 babyrobot-1.0.8/babyrobot/envs/lib/maze.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6569 2022-08-17 12:38:44.000000 babyrobot-1.0.8/babyrobot/envs/lib/robot_draw.py
--rw-------   0 steve     (1000) steve     (1000)     3831 2022-05-20 17:37:37.000000 babyrobot-1.0.8/babyrobot/envs/lib/robot_position.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot/envs/lib/themes/
--rw-rw-r--   0 steve     (1000) steve     (1000)      296 2022-05-13 18:27:13.000000 babyrobot-1.0.8/babyrobot/envs/lib/themes/black_orange.json
--rw-rw-r--   0 steve     (1000) steve     (1000)      242 2022-07-25 13:38:07.000000 babyrobot-1.0.8/babyrobot/envs/lib/themes/blue_green.json
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot/lib/
--rw-rw-r--   0 steve     (1000) steve     (1000)      234 2022-08-20 10:10:13.000000 babyrobot-1.0.8/babyrobot/lib/__init__.py
--rw-------   0 steve     (1000) steve     (1000)     4643 2022-08-20 09:03:35.000000 babyrobot-1.0.8/babyrobot/lib/policy.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     6212 2022-08-20 16:32:27.000000 babyrobot-1.0.8/babyrobot/lib/policy_evaluation.py
--rw-rw-r--   0 steve     (1000) steve     (1000)     1282 2022-08-21 08:16:15.000000 babyrobot-1.0.8/babyrobot/lib/utils.py
--rw-------   0 steve     (1000) steve     (1000)     4105 2022-08-18 18:05:13.000000 babyrobot-1.0.8/babyrobot/lib/value_iteration.py
-drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot.egg-info/
--rw-rw-r--   0 steve     (1000) steve     (1000)     4427 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot.egg-info/PKG-INFO
--rw-rw-r--   0 steve     (1000) steve     (1000)     1922 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot.egg-info/SOURCES.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)        1 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot.egg-info/dependency_links.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       20 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot.egg-info/requires.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       10 2022-08-21 10:03:14.000000 babyrobot-1.0.8/babyrobot.egg-info/top_level.txt
--rw-rw-r--   0 steve     (1000) steve     (1000)       38 2022-08-21 10:03:14.000000 babyrobot-1.0.8/setup.cfg
--rw-rw-r--   0 steve     (1000) steve     (1000)     1194 2022-08-15 17:03:41.000000 babyrobot-1.0.8/setup.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-24 07:54:42.143661 babyrobot-1.0.9/
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1073 2022-05-10 10:05:37.000000 babyrobot-1.0.9/LICENSE
+-rw-rw-r--   0 steve     (1000) steve     (1000)       81 2022-05-15 17:47:19.000000 babyrobot-1.0.9/MANIFEST.in
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4562 2022-08-24 07:54:42.139661 babyrobot-1.0.9/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4103 2022-08-22 07:27:05.000000 babyrobot-1.0.9/README.md
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-24 07:54:42.079663 babyrobot-1.0.9/babyrobot/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      967 2022-08-24 07:41:26.000000 babyrobot-1.0.9/babyrobot/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      159 2022-08-22 07:27:49.000000 babyrobot-1.0.9/babyrobot/_version.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-24 07:54:42.087663 babyrobot-1.0.9/babyrobot/envs/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      627 2022-08-16 07:26:07.000000 babyrobot-1.0.9/babyrobot/envs/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      388 2022-05-27 07:46:46.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v0.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1247 2022-05-27 07:41:18.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v1.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2074 2022-05-24 17:15:30.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v2.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1157 2022-07-20 16:45:41.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v3.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3221 2022-07-27 19:45:48.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v4.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      759 2022-07-24 13:10:50.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v5.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1486 2022-07-24 13:10:15.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v6.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5848 2022-07-27 20:36:55.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v7.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5000 2022-08-24 07:51:50.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_interface.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3042 2022-08-24 07:47:33.000000 babyrobot-1.0.9/babyrobot/envs/baby_robot_v0.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-24 07:54:42.099662 babyrobot-1.0.9/babyrobot/envs/lib/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      266 2022-05-20 12:21:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/__init__.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      278 2022-05-15 10:21:05.000000 babyrobot-1.0.9/babyrobot/envs/lib/actions.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3328 2022-05-15 10:35:12.000000 babyrobot-1.0.9/babyrobot/envs/lib/arrows.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3557 2022-08-19 16:26:48.000000 babyrobot-1.0.9/babyrobot/envs/lib/direction.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    22794 2022-08-16 18:30:50.000000 babyrobot-1.0.9/babyrobot/envs/lib/draw_grid.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)    11998 2022-08-20 11:38:46.000000 babyrobot-1.0.9/babyrobot/envs/lib/draw_info.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)      561 2022-07-24 13:13:14.000000 babyrobot-1.0.9/babyrobot/envs/lib/dynamic_space.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     7450 2022-08-16 18:29:19.000000 babyrobot-1.0.9/babyrobot/envs/lib/grid_base.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     3909 2022-07-26 18:08:29.000000 babyrobot-1.0.9/babyrobot/envs/lib/grid_info.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     5580 2022-08-20 10:01:13.000000 babyrobot-1.0.9/babyrobot/envs/lib/grid_level.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-24 07:54:42.131661 babyrobot-1.0.9/babyrobot/envs/lib/images/
+-rw-rw-r--   0 steve     (1000) steve     (1000)    16805 2022-05-10 07:49:32.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/BabyRobot64_Sprites.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1985 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_0.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1991 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_1.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1934 2022-08-17 12:31:03.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_10.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1880 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_2.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1882 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_3.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)      980 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_4.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)      979 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_5.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1815 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_6.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1822 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_7.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1924 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_8.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1934 2022-05-11 10:59:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_9.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4026 2022-05-20 11:39:38.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/big_puddle.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1737 2022-05-20 11:39:38.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/small_puddle.png
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4026 2022-05-10 07:49:32.000000 babyrobot-1.0.9/babyrobot/envs/lib/images/splash_2.png
+-rw-------   0 steve     (1000) steve     (1000)     9276 2022-05-10 07:49:32.000000 babyrobot-1.0.9/babyrobot/envs/lib/maze.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6569 2022-08-17 12:38:44.000000 babyrobot-1.0.9/babyrobot/envs/lib/robot_draw.py
+-rw-------   0 steve     (1000) steve     (1000)     3831 2022-05-20 17:37:37.000000 babyrobot-1.0.9/babyrobot/envs/lib/robot_position.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-24 07:54:42.131661 babyrobot-1.0.9/babyrobot/envs/lib/themes/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      296 2022-05-13 18:27:13.000000 babyrobot-1.0.9/babyrobot/envs/lib/themes/black_orange.json
+-rw-rw-r--   0 steve     (1000) steve     (1000)      242 2022-07-25 13:38:07.000000 babyrobot-1.0.9/babyrobot/envs/lib/themes/blue_green.json
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-24 07:54:42.139661 babyrobot-1.0.9/babyrobot/lib/
+-rw-rw-r--   0 steve     (1000) steve     (1000)      234 2022-08-24 07:38:23.000000 babyrobot-1.0.9/babyrobot/lib/__init__.py
+-rw-------   0 steve     (1000) steve     (1000)     4643 2022-08-20 09:03:35.000000 babyrobot-1.0.9/babyrobot/lib/policy.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     6212 2022-08-20 16:32:27.000000 babyrobot-1.0.9/babyrobot/lib/policy_evaluation.py
+-rw-rw-r--   0 steve     (1000) steve     (1000)     2506 2022-08-24 07:37:01.000000 babyrobot-1.0.9/babyrobot/lib/utils.py
+-rw-------   0 steve     (1000) steve     (1000)     4105 2022-08-18 18:05:13.000000 babyrobot-1.0.9/babyrobot/lib/value_iteration.py
+drwxrwxr-x   0 steve     (1000) steve     (1000)        0 2022-08-24 07:54:42.079663 babyrobot-1.0.9/babyrobot.egg-info/
+-rw-rw-r--   0 steve     (1000) steve     (1000)     4562 2022-08-24 07:54:41.000000 babyrobot-1.0.9/babyrobot.egg-info/PKG-INFO
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1922 2022-08-24 07:54:42.000000 babyrobot-1.0.9/babyrobot.egg-info/SOURCES.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)        1 2022-08-24 07:54:41.000000 babyrobot-1.0.9/babyrobot.egg-info/dependency_links.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       28 2022-08-24 07:54:41.000000 babyrobot-1.0.9/babyrobot.egg-info/requires.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       10 2022-08-24 07:54:41.000000 babyrobot-1.0.9/babyrobot.egg-info/top_level.txt
+-rw-rw-r--   0 steve     (1000) steve     (1000)       38 2022-08-24 07:54:42.143661 babyrobot-1.0.9/setup.cfg
+-rw-rw-r--   0 steve     (1000) steve     (1000)     1202 2022-08-24 07:42:54.000000 babyrobot-1.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `babyrobot-1.0.8/LICENSE` & `babyrobot-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/PKG-INFO` & `babyrobot-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: babyrobot
-Version: 1.0.8
+Version: 1.0.9
 Summary: An OpenAI Gym Environment for BabyRobot
 Home-page: https://github.com/WhatIThinkAbout/BabyRobotGym
 Author: Steve Roberts
 Author-email: steve@steveroberts.name
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BabyRobotGym
 ### A Reinforcement Learning Gym Environment for Baby Robot
 
 
-<center><img src="notebooks/images/black_maze_run_opt.gif"/></center>
+<center><img src="https://github.com/WhatIThinkAbout/BabyRobotGym/blob/main/notebooks/images/black_maze_run_opt.gif/></center>
 
 
 The code in this repository accompanies the Towards Data Science article _[<b>Creating a Custom Gym Environment for Jupyter Notebooks</b> - <i>Part 1: Creating the framework</i>](https://towardsdatascience.com/creating-a-custom-gym-environment-for-jupyter-notebooks-e17024474617)_ and shows the steps required to create a custom gym environment with graphical output in a Jupyter notebook.
 
 
-<center><img src="notebooks/images/green_babyrobot_small.gif"/></center>
+<center><img src="https://github.com/WhatIThinkAbout/BabyRobotGym/blob/main/notebooks/images/green_babyrobot_small.gif"/></center>
 
 
 ## To install:
 
 ```
 pip install babyrobot
 ```
@@ -101,7 +102,9 @@
 To start this in a browser, just type:
 
 `jupyter notebook baby_robot_gym_test.ipynb`<br>
 
 (When running in jupyter notebook the current Conda environment will automatically be used and the required packages should all be available. It's also possible to run "<i>python -m ipykernel install --user --name=BabyRobotGym</i>" which will create a Jupyter Notebook kernel, that can then be selected from the notebook's menu.)
 
 Or else just open this file in VS Code and make sure _'BabyRobotGym'_ is selected as the kernel. This should make the _'BabyRobotEnv-v1'_ environment, test it in Stable Baselines and then run the environment until it completes, which happens to occur in a single step, since we haven't yet written the 'step' function!
+
+
```

### Comparing `babyrobot-1.0.8/README.md` & `babyrobot-1.0.9/babyrobot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,33 @@
+Metadata-Version: 2.1
+Name: babyrobot
+Version: 1.0.9
+Summary: An OpenAI Gym Environment for BabyRobot
+Home-page: https://github.com/WhatIThinkAbout/BabyRobotGym
+Author: Steve Roberts
+Author-email: steve@steveroberts.name
+License: MIT
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # BabyRobotGym
 ### A Reinforcement Learning Gym Environment for Baby Robot
 
 
-<center><img src="notebooks/images/black_maze_run_opt.gif"/></center>
+<center><img src="https://github.com/WhatIThinkAbout/BabyRobotGym/blob/main/notebooks/images/black_maze_run_opt.gif/></center>
 
 
 The code in this repository accompanies the Towards Data Science article _[<b>Creating a Custom Gym Environment for Jupyter Notebooks</b> - <i>Part 1: Creating the framework</i>](https://towardsdatascience.com/creating-a-custom-gym-environment-for-jupyter-notebooks-e17024474617)_ and shows the steps required to create a custom gym environment with graphical output in a Jupyter notebook.
 
 
-<center><img src="notebooks/images/green_babyrobot_small.gif"/></center>
+<center><img src="https://github.com/WhatIThinkAbout/BabyRobotGym/blob/main/notebooks/images/green_babyrobot_small.gif"/></center>
 
 
 ## To install:
 
 ```
 pip install babyrobot
 ```
@@ -87,7 +102,9 @@
 To start this in a browser, just type:
 
 `jupyter notebook baby_robot_gym_test.ipynb`<br>
 
 (When running in jupyter notebook the current Conda environment will automatically be used and the required packages should all be available. It's also possible to run "<i>python -m ipykernel install --user --name=BabyRobotGym</i>" which will create a Jupyter Notebook kernel, that can then be selected from the notebook's menu.)
 
 Or else just open this file in VS Code and make sure _'BabyRobotGym'_ is selected as the kernel. This should make the _'BabyRobotEnv-v1'_ environment, test it in Stable Baselines and then run the environment until it completes, which happens to occur in a single step, since we haven't yet written the 'step' function!
+
+
```

### Comparing `babyrobot-1.0.8/babyrobot/__init__.py` & `babyrobot-1.0.9/babyrobot/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from gym.envs.registration import register
+from .lib.utils import make
 from ._version import __version__
 
+
 #
 # Release Gym Environments
 #
 
 
 register(
     id='BabyRobot-v0',
```

### Comparing `babyrobot-1.0.8/babyrobot/envs/__init__.py` & `babyrobot-1.0.9/babyrobot/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v1.py` & `babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v1.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v2.py` & `babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v2.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v3.py` & `babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v3.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v4.py` & `babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v4.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v5.py` & `babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v5.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v6.py` & `babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v6.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/baby_robot_env_v7.py` & `babyrobot-1.0.9/babyrobot/envs/baby_robot_env_v7.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/baby_robot_interface.py` & `babyrobot-1.0.9/babyrobot/envs/baby_robot_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .lib.actions import Actions
 
 
 class BabyRobotInterface(gym.Env):
     ''' Baby Robot Gym Environment Base Class '''
 
     def __init__(self, **kwargs):
-        super().__init__()    
+        super().__init__()
 
         # initially no actions are available      
         self.dynamic_action_space = Dynamic()          
 
         # dimensions of the grid
         self.width = kwargs.get('width',3)
         self.height = kwargs.get('height',3)
```

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/arrows.py` & `babyrobot-1.0.9/babyrobot/envs/lib/arrows.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/direction.py` & `babyrobot-1.0.9/babyrobot/envs/lib/direction.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/draw_grid.py` & `babyrobot-1.0.9/babyrobot/envs/lib/draw_grid.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/draw_info.py` & `babyrobot-1.0.9/babyrobot/envs/lib/draw_info.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/dynamic_space.py` & `babyrobot-1.0.9/babyrobot/envs/lib/dynamic_space.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/grid_base.py` & `babyrobot-1.0.9/babyrobot/envs/lib/grid_base.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/grid_info.py` & `babyrobot-1.0.9/babyrobot/envs/lib/grid_info.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/grid_level.py` & `babyrobot-1.0.9/babyrobot/envs/lib/grid_level.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/BabyRobot64_Sprites.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/BabyRobot64_Sprites.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_0.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_0.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_1.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_1.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_10.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_10.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_2.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_2.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_3.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_3.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_4.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_4.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_5.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_5.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_6.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_6.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_7.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_7.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_8.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_8.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/baby_robot_9.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/baby_robot_9.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/big_puddle.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/big_puddle.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/small_puddle.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/small_puddle.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/images/splash_2.png` & `babyrobot-1.0.9/babyrobot/envs/lib/images/splash_2.png`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/maze.py` & `babyrobot-1.0.9/babyrobot/envs/lib/maze.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/robot_draw.py` & `babyrobot-1.0.9/babyrobot/envs/lib/robot_draw.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/envs/lib/robot_position.py` & `babyrobot-1.0.9/babyrobot/envs/lib/robot_position.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/lib/policy.py` & `babyrobot-1.0.9/babyrobot/lib/policy.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/lib/policy_evaluation.py` & `babyrobot-1.0.9/babyrobot/lib/policy_evaluation.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot/lib/value_iteration.py` & `babyrobot-1.0.9/babyrobot/lib/value_iteration.py`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/babyrobot.egg-info/PKG-INFO` & `babyrobot-1.0.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,18 @@
-Metadata-Version: 2.1
-Name: babyrobot
-Version: 1.0.8
-Summary: An OpenAI Gym Environment for BabyRobot
-Home-page: https://github.com/WhatIThinkAbout/BabyRobotGym
-Author: Steve Roberts
-Author-email: steve@steveroberts.name
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BabyRobotGym
 ### A Reinforcement Learning Gym Environment for Baby Robot
 
 
-<center><img src="notebooks/images/black_maze_run_opt.gif"/></center>
+<center><img src="https://github.com/WhatIThinkAbout/BabyRobotGym/blob/main/notebooks/images/black_maze_run_opt.gif/></center>
 
 
 The code in this repository accompanies the Towards Data Science article _[<b>Creating a Custom Gym Environment for Jupyter Notebooks</b> - <i>Part 1: Creating the framework</i>](https://towardsdatascience.com/creating-a-custom-gym-environment-for-jupyter-notebooks-e17024474617)_ and shows the steps required to create a custom gym environment with graphical output in a Jupyter notebook.
 
 
-<center><img src="notebooks/images/green_babyrobot_small.gif"/></center>
+<center><img src="https://github.com/WhatIThinkAbout/BabyRobotGym/blob/main/notebooks/images/green_babyrobot_small.gif"/></center>
 
 
 ## To install:
 
 ```
 pip install babyrobot
 ```
```

### Comparing `babyrobot-1.0.8/babyrobot.egg-info/SOURCES.txt` & `babyrobot-1.0.9/babyrobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `babyrobot-1.0.8/setup.py` & `babyrobot-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,9 +35,9 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     packages = find_packages(exclude=("tests",)),
     include_package_data=True,
-    install_requires=['gym','ipycanvas==0.11']    
+    install_requires=['gym==0.25.2','ipycanvas==0.11']    
 )
```

