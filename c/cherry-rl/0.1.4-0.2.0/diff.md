# Comparing `tmp/cherry-rl-0.1.4.tar.gz` & `tmp/cherry-rl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cherry-rl-0.1.4.tar", last modified: Fri May  1 15:13:14 2020, max compression
+gzip compressed data, was "cherry-rl-0.2.0.tar", last modified: Mon Jun 26 01:46:05 2023, max compression
```

## Comparing `cherry-rl-0.1.4.tar` & `cherry-rl-0.2.0.tar`

### file list

```diff
@@ -1,60 +1,215 @@
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6027 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/PKG-INFO
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4661 2020-02-14 20:05:02.000000 cherry-rl-0.1.4/README.md
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      455 2019-08-05 21:54:28.000000 cherry-rl-0.1.4/cherry/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3571 2020-02-14 19:41:41.000000 cherry-rl-0.1.4/cherry/_torch.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1122 2019-08-15 02:02:44.000000 cherry-rl-0.1.4/cherry/_utils.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       22 2020-05-01 15:11:24.000000 cherry-rl-0.1.4/cherry/_version.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry/algorithms/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      116 2019-08-15 23:16:00.000000 cherry-rl-0.1.4/cherry/algorithms/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2740 2019-08-17 19:04:24.000000 cherry-rl-0.1.4/cherry/algorithms/a2c.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      834 2019-08-17 09:09:03.000000 cherry-rl-0.1.4/cherry/algorithms/ddpg.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4083 2019-08-17 08:25:13.000000 cherry-rl-0.1.4/cherry/algorithms/ppo.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     8254 2019-09-09 21:48:32.000000 cherry-rl-0.1.4/cherry/algorithms/sac.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6847 2019-08-17 18:59:14.000000 cherry-rl-0.1.4/cherry/algorithms/trpo.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     4159 2019-08-17 08:14:01.000000 cherry-rl-0.1.4/cherry/debug.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6169 2020-02-27 01:17:17.000000 cherry-rl-0.1.4/cherry/distributions.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry/envs/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      742 2019-09-03 17:18:21.000000 cherry-rl-0.1.4/cherry/envs/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      292 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/envs/action_lambda_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1150 2019-09-02 16:32:56.000000 cherry-rl-0.1.4/cherry/envs/action_space_scaler_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1481 2020-02-27 01:17:17.000000 cherry-rl-0.1.4/cherry/envs/base.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5965 2019-11-05 00:09:36.000000 cherry-rl-0.1.4/cherry/envs/logger_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      689 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/envs/monitor_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5678 2019-08-19 19:15:30.000000 cherry-rl-0.1.4/cherry/envs/normalizer_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    11591 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/envs/openai_atari_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    10740 2019-08-21 15:42:26.000000 cherry-rl-0.1.4/cherry/envs/recorder_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1578 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/envs/reward_clipper_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2236 2019-09-03 23:03:14.000000 cherry-rl-0.1.4/cherry/envs/reward_normalizer_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5728 2019-08-31 16:17:42.000000 cherry-rl-0.1.4/cherry/envs/runner_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      315 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/envs/state_lambda_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2212 2019-09-03 23:01:58.000000 cherry-rl-0.1.4/cherry/envs/state_normalizer_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      849 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/envs/timestep_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2214 2020-04-30 16:20:17.000000 cherry-rl-0.1.4/cherry/envs/torch_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2417 2020-02-27 01:17:17.000000 cherry-rl-0.1.4/cherry/envs/utils.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     7935 2019-08-19 00:54:48.000000 cherry-rl-0.1.4/cherry/envs/visdom_logger_wrapper.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)    13167 2020-04-30 16:20:17.000000 cherry-rl-0.1.4/cherry/experience_replay.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry/models/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      137 2019-08-16 20:24:37.000000 cherry-rl-0.1.4/cherry/models/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3053 2019-07-29 22:29:45.000000 cherry-rl-0.1.4/cherry/models/atari.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     5248 2019-11-05 00:13:50.000000 cherry-rl-0.1.4/cherry/models/robotics.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3325 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/models/tabular.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1703 2020-05-01 15:11:24.000000 cherry-rl-0.1.4/cherry/models/utils.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry/nn/
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      144 2019-08-16 20:22:25.000000 cherry-rl-0.1.4/cherry/nn/__init__.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1567 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/nn/epsilon_greedy.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1883 2019-08-16 20:22:09.000000 cherry-rl-0.1.4/cherry/nn/init.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)      874 2019-08-17 05:01:43.000000 cherry-rl-0.1.4/cherry/nn/robotics_layers.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2758 2019-08-17 09:30:55.000000 cherry-rl-0.1.4/cherry/optim.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     2174 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/pg.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     6285 2019-06-09 01:14:11.000000 cherry-rl-0.1.4/cherry/plot.py
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     3085 2020-02-27 01:17:17.000000 cherry-rl-0.1.4/cherry/td.py
-drwxrwxr-x   0 seba-1511  (1000) seba-1511  (1000)        0 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry_rl.egg-info/
--rw-r--r--   0 seba-1511  (1000) seba-1511  (1000)     6027 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry_rl.egg-info/PKG-INFO
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1357 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry_rl.egg-info/SOURCES.txt
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        1 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry_rl.egg-info/dependency_links.txt
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       39 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry_rl.egg-info/requires.txt
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)        7 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/cherry_rl.egg-info/top_level.txt
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)       79 2020-05-01 15:13:14.000000 cherry-rl-0.1.4/setup.cfg
--rw-rw-r--   0 seba-1511  (1000) seba-1511  (1000)     1139 2019-09-07 17:05:58.000000 cherry-rl-0.1.4/setup.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.212963 cherry-rl-0.2.0/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.153901 cherry-rl-0.2.0/.github/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      457 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.154261 cherry-rl-0.2.0/.github/workflows/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1825 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/.github/workflows/python_unittest.yaml
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1498 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/.gitignore
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1677 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/.travis.yml
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1538 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/CHANGELOG.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11357 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/LICENSE
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1043 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/Makefile
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8167 2023-06-26 01:46:05.213067 cherry-rl-0.2.0/PKG-INFO
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7734 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/README.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.157649 cherry-rl-0.2.0/benchmarks/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3020 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/benchmarks/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4426 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/benchmarks/benchmark.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)        6 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/benchmarks/requirements.txt
+-rwxr--r--   0 seba-1511   (501) staff       (20)     1219 2019-06-26 21:47:21.000000 cherry-rl-0.2.0/benchmarks/run_atari.sh
+-rwxr--r--   0 seba-1511   (501) staff       (20)     1977 2019-06-26 21:47:21.000000 cherry-rl-0.2.0/benchmarks/run_pybullet.sh
+-rwxr--r--   0 seba-1511   (501) staff       (20)      756 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/benchmarks/run_spinup.sh
+-rwxr--r--   0 seba-1511   (501) staff       (20)      908 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/benchmarks/run_tabular.sh
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.164274 cherry-rl-0.2.0/cherry/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      478 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3645 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/_torch.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1589 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/cherry/_utils.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)       22 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/_version.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.166413 cherry-rl-0.2.0/cherry/algorithms/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      397 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3135 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/a2c.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1463 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/arguments.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1985 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/ddpg.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11818 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/drq.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6250 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/drqv2.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10514 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/ppo.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    16604 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/sac.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5660 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/td3.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10399 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/algorithms/trpo.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4286 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/debug.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9506 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/distributions.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.166692 cherry-rl-0.2.0/cherry/envs/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       45 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/envs/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3734 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/envs/utils.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    18982 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/experience_replay.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.167543 cherry-rl-0.2.0/cherry/models/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      137 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/cherry/models/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3352 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/models/atari.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6084 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/models/robotics.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3917 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/models/tabular.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1777 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/models/utils.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.169011 cherry-rl-0.2.0/cherry/nn/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      297 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2968 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/action_value.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1629 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/epsilon_greedy.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2083 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/init.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      600 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/misc.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1649 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/mlp.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3203 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/policy.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      933 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/robotics_layers.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      665 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/nn/state_value.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2797 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/optim.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2131 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/pg.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6387 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/plot.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3265 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/td.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.172001 cherry-rl-0.2.0/cherry/wrappers/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1089 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      300 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/action_lambda_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1170 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/action_space_scaler_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1957 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/base_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2053 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/closer.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6004 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/logger_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      689 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/monitor_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5480 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/normalizer_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11604 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/openai_atari_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10739 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/recorder_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1586 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/reward_clipper_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2225 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/reward_normalizer_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6467 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/runner_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      323 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/state_lambda_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2303 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/state_normalizer_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      857 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/timestep_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2207 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/torch_wrapper.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7931 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/cherry/wrappers/visdom_logger_wrapper.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.172627 cherry-rl-0.2.0/cherry_rl.egg-info/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8167 2023-06-26 01:46:04.000000 cherry-rl-0.2.0/cherry_rl.egg-info/PKG-INFO
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5513 2023-06-26 01:46:04.000000 cherry-rl-0.2.0/cherry_rl.egg-info/SOURCES.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)        1 2023-06-26 01:46:04.000000 cherry-rl-0.2.0/cherry_rl.egg-info/dependency_links.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)       46 2023-06-26 01:46:04.000000 cherry-rl-0.2.0/cherry_rl.egg-info/requires.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)        7 2023-06-26 01:46:04.000000 cherry-rl-0.2.0/cherry_rl.egg-info/top_level.txt
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.173008 cherry-rl-0.2.0/docs/
+-rw-r--r--   0 seba-1511   (501) staff       (20)       14 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/CNAME
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.174791 cherry-rl-0.2.0/docs/api/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1133 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.algorithms.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)       40 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.debug.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      551 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.distributions.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      161 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.envs.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      327 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1090 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.models.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)       85 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.nn.init.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      636 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.nn.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      122 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.optim.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)       50 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.pg.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)       76 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.plot.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)       72 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.td.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      794 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/api/cherry.wrappers.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.150111 cherry-rl-0.2.0/docs/assets/
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.174928 cherry-rl-0.2.0/docs/assets/css/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1671 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/css/custom.css
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.175703 cherry-rl-0.2.0/docs/assets/images/
+-rw-r--r--   0 seba-1511   (501) staff       (20)   136412 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/cherry.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)   106183 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/cherry_cropped.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    48284 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/cherry_full.png
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.179091 cherry-rl-0.2.0/docs/assets/images/favicons/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3361 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/apple-touch-icon-114x114.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3633 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/apple-touch-icon-120x120.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4833 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/apple-touch-icon-144x144.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5883 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/apple-touch-icon-152x152.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1525 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/apple-touch-icon-57x57.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1560 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/apple-touch-icon-60x60.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1920 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/apple-touch-icon-72x72.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2240 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/apple-touch-icon-76x76.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2753 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/favicon-128.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)      336 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/favicon-16x16.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9829 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/favicon-196x196.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)      599 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/favicon-32x32.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2463 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/favicon-96x96.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    34494 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/favicon.ico
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4833 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/mstile-144x144.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    23186 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/mstile-150x150.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)    40880 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/mstile-310x150.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)   108080 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/mstile-310x310.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2753 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/assets/images/favicons/mstile-70x70.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1538 2023-06-26 01:43:14.000000 cherry-rl-0.2.0/docs/changelog.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7734 2023-06-26 01:43:14.000000 cherry-rl-0.2.0/docs/index.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.179699 cherry-rl-0.2.0/docs/tutorials/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      388 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/tutorials/debugging_rl.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      178 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/tutorials/distributed_ppo.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)    12361 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/tutorials/getting_started.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      183 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/docs/tutorials/recurrent_a2c.md
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.181156 cherry-rl-0.2.0/examples/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3250 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/actor_critic_cartpole.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3262 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/actor_critic_gridworld.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.183668 cherry-rl-0.2.0/examples/atari/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      508 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/atari/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3298 2020-04-30 16:20:17.000000 cherry-rl-0.2.0/examples/atari/a2c_atari.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2319 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/atari/debug_atari.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3962 2020-04-30 16:20:17.000000 cherry-rl-0.2.0/examples/atari/dist_a2c_atari.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3662 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/atari/dqn_atari.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5337 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/atari/ppo_atari.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.184789 cherry-rl-0.2.0/examples/bsuite/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      603 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/bsuite/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/bsuite/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     9322 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/bsuite/trpo_v_random.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.186213 cherry-rl-0.2.0/examples/dmc/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1795 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/examples/dmc/Makefile
+-rw-r--r--   0 seba-1511   (501) staff       (20)      417 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/examples/dmc/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)      812 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/examples/dmc/dmc_sweep_proprioceptive.yaml
+-rw-r--r--   0 seba-1511   (501) staff       (20)      911 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/examples/dmc/dmc_sweep_vision.yaml
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10618 2023-06-26 01:42:29.000000 cherry-rl-0.2.0/examples/dmc/models.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.198036 cherry-rl-0.2.0/examples/dmc/results/
+-rw-r--r--   0 seba-1511   (501) staff       (20)  3146522 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/examples/dmc/results/all.png
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8034 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/examples/dmc/results/dmc_plot_results.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4418 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/examples/dmc/tasks.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7596 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/examples/dmc/train.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4134 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/examples/dmc/utils.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.198248 cherry-rl-0.2.0/examples/mujoco/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5083 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/examples/mujoco/offpolicy_training.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6361 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/ppo_pendulum_gpu.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.202603 cherry-rl-0.2.0/examples/pybullet/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      550 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/pybullet/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     8776 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/examples/pybullet/delayed_tsac_pybullet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5630 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/pybullet/dist_ppo_pybullet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5093 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/pybullet/ppo_pybullet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6517 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/pybullet/sac_pybullet.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     2740 2019-07-29 22:41:41.000000 cherry-rl-0.2.0/examples/reinforce_cartpole.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.205424 cherry-rl-0.2.0/examples/simple_rl/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      505 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/simple_rl/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4566 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/simple_rl/simple_q_mdp.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.208249 cherry-rl-0.2.0/examples/spinning-up/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      596 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/spinning-up/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4889 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/spinning-up/cherry_ddpg.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3493 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/spinning-up/cherry_dqn.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     5385 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/spinning-up/cherry_ppo.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7887 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/examples/spinning-up/cherry_sac.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4448 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/spinning-up/cherry_vpg.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.209099 cherry-rl-0.2.0/examples/tabular/
+-rw-r--r--   0 seba-1511   (501) staff       (20)      575 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/tabular/README.md
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1678 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/tabular/q_learning.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1630 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/examples/tabular/sarsa.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3051 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/mkdocs.yaml
+-rw-r--r--   0 seba-1511   (501) staff       (20)      234 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/requirements-dev.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)        2 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/requirements.txt
+-rw-r--r--   0 seba-1511   (501) staff       (20)       79 2023-06-26 01:46:05.213526 cherry-rl-0.2.0/setup.cfg
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1187 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/setup.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.209729 cherry-rl-0.2.0/tests/
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1082 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/tests/dummy_env.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.210387 cherry-rl-0.2.0/tests/integration/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/tests/integration/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7363 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/integration/actor_critic_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10444 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/integration/spinup_ddpg_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    11441 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/integration/spinup_ppo_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    13567 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/integration/spinup_sac_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    10290 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/integration/spinup_vpg_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     4827 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/memorize_digits.py
+drwxr-xr-x   0 seba-1511   (501) staff       (20)        0 2023-06-26 01:46:05.212836 cherry-rl-0.2.0/tests/unit/
+-rw-r--r--   0 seba-1511   (501) staff       (20)        0 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/tests/unit/__init__.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1601 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/tests/unit/_torch_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     3030 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/unit/algorithms_ppo_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1835 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/tests/unit/algorithms_trpo_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1990 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/unit/base_wrapper_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     1495 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/tests/unit/debug_logger_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)    21118 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/unit/experience_replay_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      894 2019-06-09 01:14:11.000000 cherry-rl-0.2.0/tests/unit/logger_wrapper_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)      428 2021-02-27 22:54:39.000000 cherry-rl-0.2.0/tests/unit/models_utils_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)   108746 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/unit/plot_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     6974 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/unit/rl_tests.py
+-rw-r--r--   0 seba-1511   (501) staff       (20)     7699 2023-06-26 01:42:30.000000 cherry-rl-0.2.0/tests/unit/runner_wrapper_tests.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cherry-rl-0.1.4/cherry/_torch.py` & `cherry-rl-0.2.0/cherry/_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,31 +35,32 @@
     ~~~
 
     """
     if dtype is None:
         dtype = th.get_default_dtype()
     if isinstance(array, (list, tuple)):
         array = th.cat([totensor(x) for x in array], dim=0)
-    if isinstance(array, int):
-        array = float(array)
-    if isinstance(array, float):
-        array = [array, ]
-    if isinstance(array, list):
-        array = np.array(array)
-    if isinstance(array, (np.ndarray,
-                          np.bool_,
-                          np.float32,
-                          np.float64,
-                          np.int32,
-                          np.int64)):
-        if array.dtype == np.bool_:
-            array = array.astype(np.uint8)
-        array = th.tensor(array, dtype=dtype)
-        array = array.unsqueeze(0)
-    while len(array.shape) < 2:
+    else:
+        if isinstance(array, int):
+            array = float(array)
+        if isinstance(array, float):
+            array = [array, ]
+        if isinstance(array, list):
+            array = np.array(array)
+        if isinstance(array, (np.ndarray,
+                              np.bool_,
+                              np.float32,
+                              np.float64,
+                              np.int32,
+                              np.int64)):
+            if array.dtype == np.bool_:
+                array = array.astype(np.uint8)
+        if not isinstance(array, th.Tensor):
+            array = th.tensor(array, dtype=dtype)
+    while array.ndim < 2:
         array = array.unsqueeze(0)
     return array
 
 
 def normalize(tensor, epsilon=EPS):
     """
     [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/_torch.py)
```

### Comparing `cherry-rl-0.1.4/cherry/_utils.py` & `cherry-rl-0.2.0/cherry/_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,14 +21,27 @@
              np.bool_,
              th.Tensor)
     if isinstance(array, types):
         return True
     return False
 
 
+def _parameters_to_vector(parameters):
+    """
+    This fix is required for pytorch >= 1.6.0, due to the change
+    in memory format promotion rule.
+    For more info, check:
+    * https://github.com/pytorch/pytorch/pull/37968
+    * https://github.com/pytorch/pytorch/releases/tag/v1.6.0
+      and search "Note: BC-breaking memory format changes"
+    """
+    parameters = [p.contiguous() for p in parameters]
+    return th.nn.utils.parameters_to_vector(parameters)
+
+
 def _min_size(tensor):
     """
     [[Source]]()
 
     **Description**
 
     Returns the minimium viewable size of a tensor.
```

### Comparing `cherry-rl-0.1.4/cherry/algorithms/a2c.py` & `cherry-rl-0.2.0/cherry/algorithms/a2c.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,98 +1,107 @@
 #!/usr/bin/env python3
 
-"""
-**Description**
+import dataclasses
+import torch as th
+from cherry import debug
 
-Helper functions for implementing A2C.
+from .arguments import AlgorithmArguments
 
-A2C simply computes the gradient of the policy as follows:
 
-$$
-\\mathbb{E} \\left[ (Q(s, a) - V(s)) \\cdot \\nabla_\\theta \\log \\pi_\\theta (a \\vert s) \\right].
-$$
-"""
+@dataclasses.dataclass
+class A2C(AlgorithmArguments):
 
-import torch as th
-from cherry import debug
+    """
+    <a href="https://github.com/learnables/cherry/blob/master/cherry/algorithms/a2c.py" class="source-link">[Source]</a>
 
+    ## Description
 
-def policy_loss(log_probs, advantages):
+    Helper functions for implementing A2C.
+
+    A2C simply computes the gradient of the policy as follows:
+
+    $$
+    \\mathbb{E} \\left[ (Q(s, a) - V(s)) \\cdot \\nabla_\\theta \\log \\pi_\\theta (a \\vert s) \\right].
+    $$
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/algorithms/a2c.py)
 
-    **Description**
+    @staticmethod
+    def policy_loss(log_probs, advantages):
+        """
+        ## Description
 
-    The policy loss of the Advantage Actor-Critic.
+        The policy loss of the Advantage Actor-Critic.
 
-    This function simply performs an element-wise multiplication and a mean reduction.
+        This function simply performs an element-wise multiplication and a mean reduction.
 
-    **References**
+        ## References
 
-    1. Mnih et al. 2016. “Asynchronous Methods for Deep Reinforcement Learning.” arXiv [cs.LG].
+        1. Mnih et al. 2016. “Asynchronous Methods for Deep Reinforcement Learning.” arXiv [cs.LG].
 
-    **Arguments**
+        ## Arguments
 
-    * **log_probs** (tensor) - Log-density of the selected actions.
-    * **advantages** (tensor) - Advantage of the action-state pairs.
+        * `log_probs` (tensor) - Log-density of the selected actions.
+        * `advantages` (tensor) - Advantage of the action-state pairs.
 
-    **Returns**
+        ## Returns
 
-    * (tensor) - The policy loss for the given arguments.
+        * (tensor) - The policy loss for the given arguments.
 
-    **Example**
+        ## Example
 
-    ~~~python
-    advantages = replay.advantage()
-    log_probs = replay.log_prob()
-    loss = a2c.policy_loss(log_probs, advantages)
-    ~~~
-    """
-    msg = 'log_probs and advantages must have equal size.'
-    assert log_probs.size() == advantages.size(), msg
-    if debug.IS_DEBUGGING:
-        if advantages.requires_grad:
-            debug.logger.warning('A2C:policy_loss: advantages.requires_grad is True.')
-        if not log_probs.requires_grad:
-            debug.logger.warning('A2C:policy_loss: log_probs.requires_grad is False.')
-    return -th.mean(log_probs * advantages)
+        ~~~python
+        advantages = replay.advantage()
+        log_probs = replay.log_prob()
+        loss = a2c.policy_loss(log_probs, advantages)
+        ~~~
+        """
+        msg = 'log_probs and advantages must have equal size.'
+        assert log_probs.size() == advantages.size(), msg
+        if debug.IS_DEBUGGING:
+            if advantages.requires_grad:
+                debug.logger.warning('A2C:policy_loss: advantages.requires_grad is True.')
+            if not log_probs.requires_grad:
+                debug.logger.warning('A2C:policy_loss: log_probs.requires_grad is False.')
+        return -th.mean(log_probs * advantages)
 
+    @staticmethod
+    def state_value_loss(values, rewards):
+        """
+        ## Description
 
-def state_value_loss(values, rewards):
-    """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/algorithms/a2c.py)
+        The state-value loss of the Advantage Actor-Critic.
 
-    **Description**
+        This function is equivalent to a MSELoss.
 
-    The state-value loss of the Advantage Actor-Critic.
+        ## References
 
-    This function is equivalent to a MSELoss.
+        1. Mnih et al. 2016. “Asynchronous Methods for Deep Reinforcement Learning.” arXiv [cs.LG].
 
-    **References**
+        ## Arguments
 
-    1. Mnih et al. 2016. “Asynchronous Methods for Deep Reinforcement Learning.” arXiv [cs.LG].
+        * `values` (tensor) - Predicted values for some states.
+        * `rewards` (tensor) - Observed rewards for those states.
 
-    **Arguments**
+        ## Returns
 
-    * **values** (tensor) - Predicted values for some states.
-    * **rewards** (tensor) - Observed rewards for those states.
+        * (tensor) - The value loss for the given arguments.
 
-    **Returns**
+        ## Example
 
-    * (tensor) - The value loss for the given arguments.
+        ~~~python
+        values = replay.value()
+        rewards = replay.reward()
+        loss = a2c.state_value_loss(values, rewards)
+        ~~~
+        """
+        msg = 'values and rewards must have equal size.'
+        assert values.size() == rewards.size(), msg
+        if debug.IS_DEBUGGING:
+            if rewards.requires_grad:
+                debug.logger.warning('A2C:state_value_loss: rewards.requires_grad is True.')
+            if not values.requires_grad:
+                debug.logger.warning('A2C:state_value_loss: values.requires_grad is False.')
+        return (rewards - values).pow(2).mean()
 
-    **Example**
 
-    ~~~python
-    values = replay.value()
-    rewards = replay.reward()
-    loss = a2c.state_value_loss(values, rewards)
-    ~~~
-    """
-    msg = 'values and rewards must have equal size.'
-    assert values.size() == rewards.size(), msg
-    if debug.IS_DEBUGGING:
-        if rewards.requires_grad:
-            debug.logger.warning('A2C:state_value_loss: rewards.requires_grad is True.')
-        if not values.requires_grad:
-            debug.logger.warning('A2C:state_value_loss: values.requires_grad is False.')
-    return (rewards - values).pow(2).mean()
+policy_loss = A2C.policy_loss
+state_value_loss = A2C.state_value_loss
```

### Comparing `cherry-rl-0.1.4/cherry/algorithms/sac.py` & `cherry-rl-0.2.0/cherry/algorithms/ppo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,229 +1,294 @@
 #!/usr/bin/env python3
 
-"""
-**Description**
+import dataclasses
+import torch
+import cherry
+import dotmap
 
-Helper functions for implementing Soft-Actor Critic.
-
-You should update the function approximators according to the following order.
-
-1. Entropy weight update.
-2. Action-value update.
-3. State-value update. (Optional, c.f. below)
-4. Policy update.
-
-Note that most recent implementations of SAC omit step 3. above by using
-the Bellman residual instead of modelling a state-value function.
-For an example of such implementation refer to
-[this link](https://github.com/seba-1511/cherry/blob/master/examples/pybullet/delayed_tsac_pybullet.py).
-
-"""
-
-import torch as th
-from torch.nn import functional as F
 from cherry import debug
+from .arguments import AlgorithmArguments
 
 
-def policy_loss(log_probs, q_curr, alpha=1.0):
-    """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/algorithms/sac.py)
-
-    **Description**
-
-    The policy loss of the Soft Actor-Critic.
-
-    New actions are sampled from the target policy, and those are used to compute the Q-values.
-    While we should back-propagate through the Q-values to the policy parameters, we shouldn't
-    use that gradient to optimize the Q parameters.
-    This is often avoided by either using a target Q function, or by zero-ing out the gradients
-    of the Q function parameters.
-
-    **References**
-
-    1. Haarnoja et al. 2018. “Soft Actor-Critic: Off-Policy Maximum Entropy Deep Reinforcement Learning with a Stochastic Actor.” arXiv [cs.LG].
-    2. Haarnoja et al. 2018. “Soft Actor-Critic Algorithms and Applications.” arXiv [cs.LG].
-
-    **Arguments**
-
-    * **log_probs** (tensor) - Log-density of the selected actions.
-    * **q_curr** (tensor) - Q-values of state-action pairs.
-    * **alpha** (float, *optional*, default=1.0) - Entropy weight.
+@dataclasses.dataclass
+class PPO(AlgorithmArguments):
 
-    **Returns**
-
-    * (tensor) - The policy loss for the given arguments.
-
-    **Example**
-
-    ~~~python
-    densities = policy(batch.state())
-    actions = densities.sample()
-    log_probs = densities.log_prob(actions)
-    q_curr = q_function(batch.state(), actions)
-    loss = policy_loss(log_probs, q_curr, alpha=0.1)
-    ~~~
-
-    """
-    msg = 'log_probs and q_curr must have equal size.'
-    assert log_probs.size() == q_curr.size(), msg
-    return th.mean(alpha * log_probs - q_curr)
-
-
-def action_value_loss(value, next_value, rewards, dones, gamma):
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/algorithms/sac.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/algorithms/ppo.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
-    The action-value loss of the Soft Actor-Critic.
+    Utilities to implement PPO from [1].
 
-    `value` should be the value of the current state-action pair, estimated via the Q-function.
-    `next_value` is the expected value of the next state; it can be estimated via a V-function,
-    or alternatively by computing the Q-value of the next observed state-action pair.
-    In the latter case, make sure that the action is sampled according to the current policy,
-    not the one used to gather the data.
+    The idea behing PPO is to cheaply approximate TRPO's trust-region with the following objective:
 
-    **References**
+    $$
+    \\mathbb{E}[\\min(
+        \\frac{\\pi_{\\theta}}{\\pi_{\\textrm{old}}} \\cdot A,
+        \\mathrm{clip}(\\frac{\\pi_{\\theta}}{\\pi_{\\textrm{old}}} \\cdot A, 1-\\epsilon, 1+\\epsilon)
+    )],
+    $$
 
-    1. Haarnoja et al. 2018. “Soft Actor-Critic: Off-Policy Maximum Entropy Deep Reinforcement Learning with a Stochastic Actor.” arXiv [cs.LG].
-    2. Haarnoja et al. 2018. “Soft Actor-Critic Algorithms and Applications.” arXiv [cs.LG].
+    where \(\\pi_{\\theta}\) is the current policy and \(\\pi_{\\mathrm{old}}\) is the policy used to collect the online replay's data.
 
-    **Arguments**
+    ## References
 
-    * **value** (tensor) - Action values of the actual transition.
-    * **next_value** (tensor) - State values of the resulting state.
-    * **rewards** (tensor) - Observed rewards of the transition.
-    * **dones** (tensor) - Which states were terminal.
-    * **gamma** (float) - Discount factor.
+    1. Schulman et al., “Proximal Policy Optimization Algorithms”, ArXiv 2017.
 
-    **Returns**
+    ## Arguments
 
-    * (tensor) - The policy loss for the given arguments.
+    Note: the following arguments were optimized for continuous control on PyBullet / MuJoCo.
 
-    **Example**
-
-    ~~~python
-    value = qf(batch.state(), batch.action().detach())
-    next_value = targe_vf(batch.next_state())
-    loss = action_value_loss(value,
-                             next_value,
-                             batch.reward(),
-                             batch.done(),
-                             gamma=0.99)
-    ~~~
-
-    """
-    msg = 'next_value, rewards, and dones must have equal size.'
-    assert rewards.size() == dones.size() == next_value.size(), msg
-    if debug.IS_DEBUGGING:
-        if rewards.requires_grad:
-            debug.logger.warning('SAC:action_value_loss: rewards.requires_grad is True.')
-        if next_value.requires_grad:
-            debug.logger.warning('SAC:action_value_loss: next_value.requires_grad is True.')
-        if not value.requires_grad:
-            debug.logger.warning('SAC:action_value_loss: value.requires_grad is False.')
-    q_target = rewards + (1.0 - dones) * gamma * next_value
-    return F.mse_loss(value, q_target)
-
-
-def state_value_loss(v_value, log_probs, q_value, alpha=1.0):
+    * `num_steps` (int, *optional*, default=320) - Number of of PPO gradient steps in a single update.
+    * `batch_size` (int, *optional*, default=512) - Number of samples to get from the replay.
+    * `policy_clip` (float, *optional*, default=0.2) - Clip constant for the policy.
+    * `value_clip` (float, *optional*, default=0.2) - Clip constant for state value function.
+    * `value_weight` (float, *optional*, default=0.5) - Scaling factor fo the state value function penalty.
+    * `entropy_weight` (float, *optional*, default=0.0) - Scaling factor of the entropy penalty.
+    * `discount` (float, *optional*, default=0.99) - Discount factor.
+    * `gae_tau` (float, *optional*, default=0.95) - Bias-variance trade-off for the generalized advantage estimator.
+    * `gradient_norm` (float, *optional*, default=0.5) - Maximum gradient norm.
+    * `eps` (float, *optional*, default=0.5) - Numerical stability constant.
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/algorithms/sac.py)
-
-    **Description**
 
-    The state-value loss of the Soft Actor-Critic.
+    num_steps: int = 320
+    batch_size: float = 64
+    policy_clip: float = 0.2
+    value_clip: float = 0.2
+    value_weight: float = 0.5
+    entropy_weight: float = 0.0
+    discount: float = 0.99
+    gae_tau: float = 0.95
+    gradient_norm: float = 0.5  # no clipping if 0
+    eps: float = 1e-8
+
+    @staticmethod
+    def policy_loss(new_log_probs, old_log_probs, advantages, clip=0.1):
+        """
+        ## Description
+
+        The clipped policy loss of Proximal Policy Optimization.
+
+        ## Arguments
+
+        * `new_log_probs` (tensor) - The log-density of actions from the target policy.
+        * `old_log_probs` (tensor) - The log-density of actions from the behaviour policy.
+        * `advantages` (tensor) - Advantage of the actions.
+        * `clip` (float, *optional*, default=0.1) - The clipping coefficient.
+
+        ## Returns
+
+        * loss (tensor) - The clipped policy loss for the given arguments.
+
+        **Example**
+
+        ~~~python
+        advantage = ch.pg.generalized_advantage(
+            GAMMA,
+            TAU,
+            replay.reward(),
+            replay.done(),
+            replay.value(),
+            next_state_value,
+        )
+        new_densities = policy(replay.state())
+        new_logprobs = new_densities.log_prob(replay.action())
+        loss = policy_loss(
+            new_logprobs,
+            replay.logprob().detach(),
+            advantage.detach(),
+            clip=0.2,
+        )
+        ~~~
+        """
+        msg = 'new_log_probs, old_log_probs and advantages must have equal size.'
+        assert new_log_probs.size() == old_log_probs.size() == advantages.size(),\
+            msg
+        if debug.IS_DEBUGGING:
+            if old_log_probs.requires_grad:
+                debug.logger.warning('PPO:policy_loss: old_log_probs.requires_grad is True.')
+            if advantages.requires_grad:
+                debug.logger.warning('PPO:policy_loss: advantages.requires_grad is True.')
+            if not new_log_probs.requires_grad:
+                debug.logger.warning('PPO:policy_loss: new_log_probs.requires_grad is False.')
+        ratios = torch.exp(new_log_probs - old_log_probs)
+        obj = ratios * advantages
+        obj_clip = ratios.clamp(1.0 - clip, 1.0 + clip) * advantages
+        return - torch.min(obj, obj_clip).mean()
+
+    @staticmethod
+    def state_value_loss(new_values, old_values, rewards, clip=0.1):
+        """
+        ## Description
+
+        The clipped state-value loss of Proximal Policy Optimization.
+
+        ## Arguments
+
+        * `new_values` (tensor) - State values from the optimized value function.
+        * `old_values` (tensor) - State values from the reference value function.
+        * `rewards` (tensor) -  Observed rewards.
+        * `clip` (float, *optional*, default=0.1) - The clipping coefficient.
+
+        ## Returns
+
+        * loss (tensor) - The clipped value loss for the given arguments.
+
+        ## Example
+
+        ~~~python
+        values = v_function(batch.state())
+        value_loss = ppo.state_value_loss(
+            values,
+            batch.value().detach(),
+            batch.reward(),
+            clip=0.2,
+        )
+        ~~~
+        """
+        msg = 'new_values, old_values, and rewards must have equal size.'
+        assert new_values.size() == old_values.size() == rewards.size(), msg
+        if debug.IS_DEBUGGING:
+            if old_values.requires_grad:
+                debug.logger.warning('PPO:state_value_loss: old_values.requires_grad is True.')
+            if rewards.requires_grad:
+                debug.logger.warning('PPO:state_value_loss: rewards.requires_grad is True.')
+            if not new_values.requires_grad:
+                debug.logger.warning('PPO:state_value_loss: new_values.requires_grad is False.')
+        loss = (rewards - new_values)**2
+        clipped_values = old_values + (new_values - old_values).clamp(-clip, clip)
+        clipped_loss = (rewards - clipped_values)**2
+        return 0.5 * torch.max(loss, clipped_loss).mean()
+
+    @staticmethod
+    def _mean(elements):
+        length = len(elements)
+        if length > 0:
+            return sum(elements) / float(length)
+        return 0.0
+
+    def update(
+        self,
+        replay,
+        policy,
+        optimizer,
+        state_value,
+        **kwargs,
+    ):
+        """
+        ## Description
+
+        Implements a single PPO update.
+
+        ## Arguments
+
+        * `replay` (cherry.ExperienceReplay) - Online replay to sample transitions from.
+        * `policy` (cherry.nn.Policy) - Policy to optimize.
+        * `state_value` (cherry.nn.StateValue) - State value function \(V(s)\).
+        * `optimizer` (torch.optim.Optimizer) - Optimizer for the `policy`.
+        """
+        # Log debugging values
+        stats = dotmap.DotMap()
+
+        # Unpack arguments and variables
+        config = self.unpack_config(self, kwargs)
+        vectorized = replay.vectorized
+
+        # Process replay
+        all_states = replay.state()
+        all_actions = replay.action()
+        all_dones = replay.done()
+        all_rewards = replay.reward()
+        with torch.no_grad():
+            if vectorized:
+                state_shape = all_states.shape[2:]
+                action_shape = all_actions.shape[2:]
+                all_log_probs = policy.log_prob(
+                    all_states.reshape(-1, *state_shape),
+                    all_actions.reshape(-1, *action_shape)
+                )
+                # reshape to -1 here because maybe Normal distribution.
+                all_log_probs = all_log_probs.reshape(*all_states.shape[:2], -1)
+                all_values = state_value(all_states.reshape(-1, *state_shape))
+                all_values = all_values.reshape(*all_states.shape[:2], 1)
+            else:
+                all_log_probs = policy.log_prob(all_states, all_actions)
+                all_values = state_value(all_states)
+
+        # Compute advantages and returns
+        next_state_value = state_value(replay[-1].next_state)
+        all_advantages = cherry.pg.generalized_advantage(
+            config.discount,
+            config.gae_tau,
+            all_rewards,
+            all_dones,
+            all_values,
+            next_state_value,
+        )
+
+        returns = all_advantages + all_values
+        all_advantages = cherry.normalize(all_advantages, epsilon=config.eps)
+
+        for i, sars in enumerate(replay):
+            sars.log_prob = cherry.totensor(all_log_probs[i].detach())
+            sars.value = cherry.totensor(all_values[i].detach())
+            sars.advantage = cherry.totensor(all_advantages[i].detach())
+            sars.retur = cherry.totensor(returns[i].detach())
+
+        # Logging
+        policy_losses = []
+        entropies = []
+        value_losses = []
+
+        # avoids the weird shapes later in the loop and extra forward passes.
+        replay = replay.flatten()
+
+        # Perform some optimization steps
+        for step in range(config.num_steps):
+            batch = replay.sample(config.batch_size)
+            states = batch.state()
+            advantages = batch.advantage()
+
+            new_densities = policy(states)
+            new_values = state_value(states)
+
+            # Compute losses
+            new_log_probs = new_densities.log_prob(batch.action())
+            entropy = new_densities.entropy().mean()
+            policy_loss = PPO.policy_loss(
+                new_log_probs,
+                batch.log_prob(),
+                advantages,
+                clip=config.policy_clip,
+            )
+            value_loss = PPO.state_value_loss(
+                new_values,
+                batch.value(),
+                batch.retur(),
+                clip=config.value_clip,
+            )
+            loss = policy_loss
+            loss = loss + config.value_weight * value_loss
+            loss = loss - config.entropy_weight * entropy
+
+            # Take optimization step
+            optimizer.zero_grad()
+            loss.backward()
+            torch.nn.utils.clip_grad_norm_(
+                policy.parameters(),
+                config.gradient_norm,
+            )
+            optimizer.step()
+
+            policy_losses.append(policy_loss)
+            entropies.append(entropy)
+            value_losses.append(value_loss)
+
+        # Log metrics
+        stats['ppo/policy_loss'] = PPO._mean(policy_losses)
+        stats['ppo/entropies'] = PPO._mean(entropies)
+        stats['ppo/value_loss'] = PPO._mean(value_losses)
+        return stats
 
-    This update is computed "on-policy": states are sampled from a replay but the state values,
-    action values, and log-densities are computed using the current value functions and policy.
 
-    **References**
-
-    1. Haarnoja et al. 2018. “Soft Actor-Critic: Off-Policy Maximum Entropy Deep Reinforcement Learning with a Stochastic Actor.” arXiv [cs.LG].
-    2. Haarnoja et al. 2018. “Soft Actor-Critic Algorithms and Applications.” arXiv [cs.LG].
-
-    **Arguments**
-
-    * **v_value** (tensor) - State values for some observed states.
-    * **log_probs** (tensor) - Log-density of actions sampled from the current policy.
-    * **q_value** (tensor) - Action values of the actions for the current policy.
-    * **alpha** (float, *optional*, default=1.0) - Entropy weight.
-
-    **Returns**
-
-    * (tensor) - The state value loss for the given arguments.
-
-    **Example**
-
-    ~~~python
-    densities = policy(batch.state())
-    actions = densities.sample()
-    log_probs = densities.log_prob(actions)
-    q_value = qf(batch.state(), actions)
-    v_value = vf(batch.state())
-    loss = state_value_loss(v_value,
-                            log_probs,
-                            q_value,
-                            alpha=0.1)
-    ~~~
-
-    """
-    msg = 'v_value, q_value, and log_probs must have equal size.'
-    assert v_value.size() == q_value.size() == log_probs.size(), msg
-    if debug.IS_DEBUGGING:
-        if log_probs.requires_grad:
-            debug.logger.warning('SAC:state_value_loss: log_probs.requires_grad is True.')
-        if q_value.requires_grad:
-            debug.logger.warning('SAC:state_value_loss: q_value.requires_grad is True.')
-        if not v_value.requires_grad:
-            debug.logger.warning('SAC:state_value_loss: v_value.requires_grad is False.')
-    v_target = q_value - alpha * log_probs
-    return F.mse_loss(v_value, v_target)
-
-
-def entropy_weight_loss(log_alpha, log_probs, target_entropy):
-    """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/algorithms/sac.py)
-
-    **Description**
-
-    Loss of the entropy weight, to automatically tune it.
-
-    The target entropy needs to be manually tuned.
-    However, a popular heuristic for TanhNormal policies is to use the negative of the action-space
-    dimensionality. (e.g. -4 when operating the voltage of a quad-rotor.)
-
-    **References**
-
-    1. Haarnoja et al. 2018. “Soft Actor-Critic Algorithms and Applications.” arXiv [cs.LG].
-
-    **Arguments**
-
-    * **log_alpha** (tensor) - Log of the entropy weight.
-    * **log_probs** (tensor) - Log-density of policy actions.
-    * **target_entropy** (float) - Target of the entropy value.
-
-    **Returns**
-
-    * (tensor) - The state value loss for the given arguments.
-
-    **Example**
-
-    ~~~python
-    densities = policy(batch.state())
-    actions = densities.sample()
-    log_probs = densities.log_prob(actions)
-    target_entropy = -np.prod(env.action_space.shape).item()
-    loss = entropy_weight_loss(alpha.log(),
-                               log_probs,
-                               target_entropy)
-    ~~~
-
-    """
-    if debug.IS_DEBUGGING:
-        if log_probs.requires_grad:
-            debug.logger.warning('SAC:entropy_weight_loss: log_probs.requires_grad is True.')
-        if not log_alpha.requires_grad:
-            debug.logger.warning('SAC:entropy_weight_loss: log_alpha.requires_grad is False.')
-    loss = -(log_alpha * (log_probs + target_entropy))
-    return loss.mean()
+policy_loss = PPO.policy_loss
+state_value_loss = PPO.state_value_loss
```

### Comparing `cherry-rl-0.1.4/cherry/debug.py` & `cherry-rl-0.2.0/cherry/debug.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,35 +28,39 @@
 print_handler.setFormatter(fmt)
 print_handler.setLevel(logging.INFO)
 logger.addHandler(print_handler)
 
 
 def debug(log_dir='./'):
     """
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/debug.py" class="source-link">[Source]</a>
+
+    ## Description
+
     Enables some debugging utilities for logging and pdb.
 
     Includes:
 
     * Automatically dropping into a post-mortem pdb debugger session
     whenever an exception is raised.
     * Enables fast DEBUG logging to a logging file via QueueHandler.
     * Copies all stdout output to the logging file. (Experimental)
 
-    **References**
+    ## References
 
     1. Automatically start the debugger on an exception (Python recipe), Thomas Heller, 2001,
         [Link](http://code.activestate.com/recipes/65287-automatically-start-the-debugger-on-an-exception/)
     2. Dealing with handlers that block, Python Documentation, 2019.
         [Link](https://docs.python.org/3/howto/logging-cookbook.html#dealing-with-handlers-that-block)
 
-    **Arguments**
+    ## Arguments
 
-    * **log_dir** (str, *optional*, Default: './') - Location to store the log files.
+    * `log_dir` (str, *optional*, Default: './') - Location to store the log files.
 
-    **Example**
+    ## Example
 
     ~~~python
     ch.debug.debug()
     raise Exception('My exception')
     -> raise('My exception')
     (Pdb)
     ~~~
```

### Comparing `cherry-rl-0.1.4/cherry/distributions.py` & `cherry-rl-0.2.0/cherry/distributions.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,52 +7,135 @@
 
 """
 
 import torch as th
 import torch.nn as nn
 import cherry as ch
 
-from torch.distributions import (Categorical,
-                                 Normal,
-                                 Distribution)
+from torch.distributions import Distribution
 
-from gym.spaces import Discrete
+
+class Categorical(th.distributions.Categorical):
+
+    """
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/distributions.py" class="source-link">[Source]</a>
+
+    ## Description
+
+    Similar to `torch.nn.Categorical`, but reshapes tensors of N
+    samples into (N, 1)-shaped tensors.
+
+    ## Arguments
+
+    Identical to `torch.distribution.Categorical`.
+
+    ## Example
+
+    ~~~python
+    dist = Categorical(logits=torch.randn(bsz, action_size))
+    actions = dist.sample()  # shape: bsz x 1
+    log_probs = dist.log_prob(actions)  # shape: bsz x 1
+    deterministic_action = action.mode()
+    ~~~
+    """
+
+    def sample(self):
+        samples = super(Categorical, self).sample()
+        return samples.unsqueeze(-1)
+
+    def log_prob(self, x):
+        log_prob = super(Categorical, self).log_prob(x.reshape(-1))
+        return log_prob.reshape_as(x)
+
+    def mode(self):
+        """
+        ## Description
+
+        Returns the model of normal distribution (ie, argmax over probabilities).
+        """
+        return self.probs.argmax(dim=-1, keepdim=True)
+
+
+class Normal(th.distributions.Normal):
+
+    """
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/distributions.py" class="source-link">[Source]</a>
+
+    ## Description
+
+    Similar to PyTorch's `Independent(Normal(loc, std))`: when computing log-densities or the entropy,
+    we sum over the last dimension.
+
+    This is typically used to compute log-probabilities of N-dimensional actions
+    sampled from a multivariate Gaussian with diagional covariance.
+
+    ## Arguments
+
+    Identical to `torch.distribution.Normal`.
+
+    ## Example
+
+    ~~~python
+    normal = Normal(torch.zeros(bsz, action_size), torch.ones(bsz, action_size))
+    actions = normal.sample()
+    log_probs = normal.log_prob(actions)  # shape: bsz x 1
+    entropies = normal.entropy()  # shape: bsz x 1
+    deterministic_action = action.mode()
+    ~~~
+    """
+
+    def log_prob(self, x):
+        log_prob = super(Normal, self).log_prob(x)
+        return log_prob.sum(-1, keepdim=True)
+
+    def entropy(self):
+        entropy = super(Normal, self).entropy().sum(dim=-1, keepdim=True)
+        return entropy
+
+    def mode(self):
+        """
+        ## Description
+
+        Returns the model of normal distribution (ie, its mean).
+        """
+        return self.mean
 
 
 class Reparameterization(object):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/distributions.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/distributions.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Unifies interface for distributions that support `rsample` and those that do not.
 
     When calling `sample()`, this class checks whether `density` has a `rsample()` member,
     and defaults to call `sample()` if it does not.
 
-    **References**
+    ## References
 
     1. Kingma and Welling. 2013. “Auto-Encoding Variational Bayes.” arXiv [stat.ML].
 
-    **Arguments**
-
-    * **density** (Distribution) - The distribution to wrap.
-
-    **Example**
+    ## Example
 
     ~~~python
     density = Normal(mean, std)
     reparam = Reparameterization(density)
     sample = reparam.sample()  # Uses Normal.rsample()
     ~~~
 
     """
 
     def __init__(self, density):
+        """
+        ## Arguments
+
+        * `density` (Distribution) - The distribution to wrap.
+        """
         self.density = density
 
     def sample(self, *args, **kwargs):
         if self.density.has_rsample:
             return self.density.rsample(*args, **kwargs)
         return self.density.sample(*args, **kwargs)
 
@@ -64,47 +147,45 @@
 
     def __str__(self):
         return 'Reparameterization(' + str(self.density) + ')'
 
 
 class ActionDistribution(nn.Module):
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/distributions.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/distributions.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     A helper module to automatically choose the proper policy distribution,
     based on the Gym environment `action_space`.
 
     For `Discrete` action spaces, it uses a `Categorical` distribution, otherwise
     it uses a `Normal` which uses a diagonal covariance matrix.
 
     This class enables to write single version policy body that will be compatible
     with a variety of environments.
 
-    **Arguments**
-
-    * **env** (Environment) - Gym environment for which actions will be sampled.
-    * **logstd** (float/tensor, *optional*, default=0) - The log standard
-    deviation for the `Normal` distribution.
-    * **use_probs** (bool, *optional*, default=False) - Whether to use probabilities or logits
-    for the `Categorical` case.
-    * **reparam** (bool, *optional*, default=False) - Whether to use reparameterization in the
-    `Normal` case.
-
-    **Example**
+    ## Example
 
     ~~~python
     env = gym.make('CartPole-v1')
     action_dist = ActionDistribution(env)
     ~~~
 
     """
 
     def __init__(self, env, logstd=None, use_probs=False, reparam=False):
+        """
+        ## Arguments
+
+        * `env` (Environment) - Gym environment for which actions will be sampled.
+        * `logstd` (float/tensor, *optional*, default=0) - The log standard deviation for the `Normal` distribution.
+        * `use_probs` (bool, *optional*, default=False) - Whether to use probabilities or logits for the `Categorical` case.
+        * `reparam` (bool, *optional*, default=False) - Whether to use reparameterization in the `Normal` case.
+        """
         super(ActionDistribution, self).__init__()
         self.use_probs = use_probs
         self.reparam = reparam
         self.is_discrete = ch.envs.is_discrete(env.action_space)
         if not self.is_discrete:
             if logstd is None:
                 action_size = ch.envs.get_space_dimension(env.action_space,
@@ -125,52 +206,49 @@
                 density = Reparameterization(density)
             return density
 
 
 class TanhNormal(Distribution):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/tabular.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/distributions.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Implements a Normal distribution followed by a Tanh, often used with the Soft Actor-Critic.
 
     This implementation also exposes `sample_and_log_prob` and `rsample_and_log_prob`,
     which returns both samples and log-densities.
     The log-densities are computed using the pre-activation values for numerical stability.
 
-    **Credit**
-
-    Adapted from Vitchyr Pong's RLkit:
-    https://github.com/vitchyr/rlkit/blob/master/rlkit/torch/distributions.py
-
-    **References**
+    ## References
 
     1. Haarnoja et al. 2018. “Soft Actor-Critic: Off-Policy Maximum Entropy Deep Reinforcement Learning with a Stochastic Actor.” arXiv [cs.LG].
     2. Haarnoja et al. 2018. “Soft Actor-Critic Algorithms and Applications.” arXiv [cs.LG].
-
-    **Arguments**
-
-    * **normal_mean** (tensor) - Mean of the Normal distribution.
-    * **normal_std** (tensor) - Standard deviation of the Normal distribution.
+    3. Vitchyr Pong's [RLkit](https://github.com/vitchyr/rlkit/blob/master/rlkit/torch/distributions.py).
 
     **Example**
     ~~~python
     mean = th.zeros(5)
     std = th.ones(5)
     dist = TanhNormal(mean, std)
     samples = dist.rsample()
     logprobs = dist.log_prob(samples)  # Numerically unstable :(
     samples, logprobs = dist.rsample_and_log_prob()  # Stable :)
     ~~~
 
     """
 
     def __init__(self, normal_mean, normal_std):
+        """
+        ## Arguments
+
+        * `normal_mean` (tensor) - Mean of the Normal distribution.
+        * `normal_std` (tensor) - Standard deviation of the Normal distribution.
+        """
         self.normal_mean = normal_mean
         self.normal_std = normal_std
         self.normal = Normal(normal_mean, normal_std)
 
     def sample_n(self, n):
         z = self.normal.sample_n(n)
         return th.tanh(z)
@@ -180,22 +258,61 @@
         offset = th.log1p(-value**2 + 1e-6)
         return self.normal.log_prob(pre_tanh_value) - offset
 
     def sample(self):
         z = self.normal.sample().detach()
         return th.tanh(z)
 
+    def mean(self):
+        """
+        ## Description
+
+        Returns the mean of the TanhDistribution (ie, tan(normal.mean)).
+        """
+        return th.tanh(self.normal.mean)
+
+    def mode(self):
+        """
+        ## Description
+
+        Returns the mode of the TanhDistribution (ie, its mean).
+        """
+        return self.mean()
+
     def sample_and_log_prob(self):
+        """
+        ## Description
+
+        Samples from the TanhNormal and computes the log-density of the
+        samples in a numerically stable way.
+
+        ## Returns
+
+        * `value` (tensor) - samples from the TanhNormal.
+        * `log_prob` (tensor) - log-probabilities of the samples.
+
+        ## Example
+
+        ~~~python
+        tanh_normal = TanhNormal(torch.zeros(bsz, action_size), torch.ones(bsz, action_size))
+        actions, log_probs = tanh_normal.sample_and_log_prob()
+        ~~~
+        """
         z = self.normal.sample().detach()
         value = th.tanh(z)
         offset = th.log1p(-value**2 + 1e-6)
         log_prob = self.normal.log_prob(z) - offset
         return value, log_prob
 
     def rsample_and_log_prob(self):
+        """
+        ## Description
+
+        Similar to `sample_and_log_prob` but with reparameterized samples.
+        """
         z = self.normal.rsample()
         value = th.tanh(z)
         offset = th.log1p(-value**2 + 1e-6)
         log_prob = self.normal.log_prob(z) - offset
         return value, log_prob
 
     def rsample(self):
```

### Comparing `cherry-rl-0.1.4/cherry/envs/__init__.py` & `cherry-rl-0.2.0/cherry/wrappers/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,31 @@
-#!/usr/bin/env python3
+# -*- coding=utf-8 -*-
 
-from .utils import *
-from .base import Wrapper
+# keep
+from .base_wrapper import Wrapper
 from .runner_wrapper import Runner
-from .logger_wrapper import Logger
 from .torch_wrapper import Torch
+from .timestep_wrapper import AddTimestep
+from .visdom_logger_wrapper import VisdomLogger
+from .action_space_scaler_wrapper import ActionSpaceScaler
+
+# eventually discard
+from .logger_wrapper import Logger
 from .openai_atari_wrapper import OpenAIAtari
 from .reward_clipper_wrapper import RewardClipper
-from .timestep_wrapper import AddTimestep
-from .monitor_wrapper import Monitor
 from .recorder_wrapper import Recorder
 from .normalizer_wrapper import Normalizer
 from .state_normalizer_wrapper import StateNormalizer
 from .reward_normalizer_wrapper import RewardNormalizer
 from .state_lambda_wrapper import StateLambda
 from .action_lambda_wrapper import ActionLambda
-from .action_space_scaler_wrapper import ActionSpaceScaler
-from .visdom_logger_wrapper import VisdomLogger
+
+# monkey-patch old functionalities
+import cherry
+
+setattr(cherry.envs, 'Wrapper', Wrapper)
+setattr(cherry.envs, 'Runner', Runner)
+setattr(cherry.envs, 'Torch', Torch)
+setattr(cherry.envs, 'AddTimestep', AddTimestep)
+setattr(cherry.envs, 'VisdomLogger', VisdomLogger)
+setattr(cherry.envs, 'ActionSpaceScaler', ActionSpaceScaler)
+setattr(cherry.envs, 'Logger', Logger)
```

### Comparing `cherry-rl-0.1.4/cherry/envs/action_space_scaler_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/action_space_scaler_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 import gym
 import numpy as np
 
-from .base import Wrapper
+from .base_wrapper import Wrapper
 
 
 class ActionSpaceScaler(Wrapper):
 
     """
     Scales the action space to be in the range (-clip, clip).
 
@@ -24,15 +24,15 @@
 
     def reset(self, *args, **kwargs):
         return self.env.reset(*args, **kwargs)
 
     def _normalize(self, action):
         lb = self.env.action_space.low
         ub = self.env.action_space.high
-        scaled_action = lb + (action + self.clip) * 0.5 * (ub - lb)
+        scaled_action = lb + (action + self.clip) / (2 * self.clip) * (ub - lb)
         scaled_action = np.clip(scaled_action, lb, ub)
         return scaled_action
 
     def step(self, action):
         if self.is_vectorized:
             action = [self._normalize(a) for a in action]
         else:
```

### Comparing `cherry-rl-0.1.4/cherry/envs/logger_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/logger_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
 from statistics import mean, pstdev
 
-from .base import Wrapper
+from .base_wrapper import Wrapper
 
 import cherry as ch
+import numpy as np
 
 
 class Logger(Wrapper):
 
     """
     Tracks and prints some common statistics about the environment.
     """
@@ -151,13 +152,13 @@
             if self.is_vectorized:
                 info[0]['logger_steps_stats'] = steps_stats
                 info[0]['logger_ep_stats'] = ep_stats
             else:
                 info['logger_steps_stats'] = steps_stats
                 info['logger_ep_stats'] = ep_stats
             self.logger.info(msg)
-        if isinstance(done, bool):
+        if isinstance(done, (bool, np.bool_)):
             if done:
                 self.num_episodes += 1
         else:
             self.num_episodes += sum(done)
         return state, reward, done, info
```

### Comparing `cherry-rl-0.1.4/cherry/envs/monitor_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/monitor_wrapper.py`

 * *Files identical despite different names*

### Comparing `cherry-rl-0.1.4/cherry/envs/normalizer_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/normalizer_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 import numpy as np
-from .base import Wrapper
+from .base_wrapper import Wrapper
 
 """
 Code adapted from OpenAI Baslines, under the following license.
 
 The MIT License
 
 Copyright (c) 2017 OpenAI (http://openai.com)
@@ -41,20 +41,21 @@
         batch_mean = np.mean(x, axis=0)
         batch_var = np.var(x, axis=0)
         batch_count = x.shape[0]
         self.update_from_moments(batch_mean, batch_var, batch_count)
 
     def update_from_moments(self, batch_mean, batch_var, batch_count):
         self.mean, self.var, self.count = update_mean_var_count_from_moments(
-                                                self.mean,
-                                                self.var,
-                                                self.count,
-                                                batch_mean,
-                                                batch_var,
-                                                batch_count)
+            self.mean,
+            self.var,
+            self.count,
+            batch_mean,
+            batch_var,
+            batch_count,
+        )
 
 
 def update_mean_var_count_from_moments(mean,
                                        var,
                                        count,
                                        batch_mean,
                                        batch_var,
```

### Comparing `cherry-rl-0.1.4/cherry/envs/openai_atari_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/openai_atari_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import cherry as ch
 import gym
 from gym import spaces
 from collections import deque
 
-from .base import Wrapper
+from .base_wrapper import Wrapper
 
 try:
     import cv2
     cv2.ocl.setUseOpenCL(False)
 except ImportError:
     cv2 = ch._utils._ImportRaiser('OpenCV2', 'pip install opencv-python')
 
@@ -95,14 +95,15 @@
         return obs
 
     def step(self, ac):
         return self.env.step(ac)
 
 
 class EpisodicLifeEnv(Wrapper):
+
     def __init__(self, env):
         """Make end-of-life == end-of-episode, but only reset on true game over.
         Done by DeepMind for the DQN and co. since it helps value estimation.
         """
         Wrapper.__init__(self, env)
         self.lives = 0
         self.was_real_done = True
@@ -214,16 +215,16 @@
         self.k = k
         self.frames = deque([], maxlen=k)
         shp = env.observation_space.shape
         self.observation_space = spaces.Box(low=0, high=255, shape=(shp[0] * k, shp[1], shp[2]), dtype=np.uint8)
 
     def reset(self):
         ob = self.env.reset()
-        for _ in range(self.k-1):
-            self.frames.append(ob*0.0)
+        for _ in range(self.k - 1):
+            self.frames.append(ob * 0.0)
         self.frames.append(ob)
         # The above is similar to ikostrikov's implementation
         # Below initializes everything with the same initial frame
         # for _ in range(self.k):
         #     self.frames.append(ob)
         return self._get_ob()
 
@@ -309,36 +310,36 @@
 class TransposeImage(Wrapper, gym.ObservationWrapper):
     def __init__(self, env=None):
         super(TransposeImage, self).__init__(env)
         obs_shape = self.observation_space.shape
         self.observation_space = spaces.Box(
             self.observation_space.low[0, 0, 0],
             self.observation_space.high[0, 0, 0],
-            [obs_shape[2], obs_shape[1], obs_shape[0]],
+            [obs_shape[-1], obs_shape[0], obs_shape[1]],
             dtype=self.observation_space.dtype)
 
     def observation(self, observation):
         return observation.transpose(2, 0, 1)
 
 
 class OpenAIAtari(Wrapper):
 
     def __init__(self, env):
         env = NoopResetEnv(env, noop_max=30)
         env = MaxAndSkipEnv(env, skip=4)
         env = wrap_deepmind(env,
                             episode_life=True,
                             clip_rewards=True,
-                            frame_stack=False,
+                            frame_stack=True,
                             scale=False,
                             )
-        obs_shape = env.observation_space.shape
-        if len(obs_shape) == 3:
-            env = TransposeImage(env)
-        env = FrameStack(env, 4)
+#        obs_shape = env.observation_space.shape
+#        if len(obs_shape) == 3:
+        env = TransposeImage(env)
+        # env = FrameStack(env, 4)
         super(OpenAIAtari, self).__init__(env)
 
     def step(self, action):
         state, reward, done, info = self.env.step(action)
         return np.array(state), reward, done, info
 
     def reset(self, *args, **kwargs):
```

### Comparing `cherry-rl-0.1.4/cherry/envs/recorder_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/recorder_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import os
 import six
 import time
 import subprocess
 import tempfile
 
 from gym import error
-from gym.utils import closer
 from gym.wrappers.monitoring import video_recorder as GymVideoRecorder
 from datetime import datetime
 
-from .base import Wrapper
+from .base_wrapper import Wrapper
+from .closer import Closer
 
 
 def touch(path):
     open(path, 'a').close()
 
 
 class VideoRecorder(GymVideoRecorder.VideoRecorder):
@@ -315,8 +315,8 @@
         # Make sure we've closed up shop when garbage collecting
         self.close()
 
     def get_video_paths(self):
         return self.output_files
 
 
-recorder_closer = closer.Closer()
+recorder_closer = Closer()
```

### Comparing `cherry-rl-0.1.4/cherry/envs/reward_clipper_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/reward_clipper_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 import gym
 import numpy as np
 
-from .base import Wrapper
+from .base_wrapper import Wrapper
 
 """
 Taken from OpenAI's baselines:
 
 https://github.com/openai/baselines/blob/master/baselines/common/atari_wrappers.py
 
 The MIT License
```

### Comparing `cherry-rl-0.1.4/cherry/envs/reward_normalizer_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/reward_normalizer_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python3
 
 import numpy as np
-from .base import Wrapper
+
+from cherry.envs.utils import num_envs
+from .base_wrapper import Wrapper
 
 
 class RewardNormalizer(Wrapper):
 
     """
     [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/envs/normalizer_wrapper.py)
 
@@ -35,35 +37,33 @@
     ~~~
     """
 
     def __init__(self, env, statistics=None, beta=0.99, eps=1e-8):
         super(RewardNormalizer, self).__init__(env)
         self.beta = beta
         self.eps = eps
+        nenvs = num_envs(self.env)
         if statistics is not None and 'mean' in statistics:
             self._reward_mean = np.copy(statistics['mean'])
         else:
-            self._reward_mean = np.zeros(self.observation_space.shape)
+            self._reward_mean = np.zeros(nenvs)
 
         if statistics is not None and 'var' in statistics:
             self._reward_var = np.copy(statistics['var'])
         else:
-            self._reward_var = np.ones(self.observation_space.shape)
+            self._reward_var = np.ones(nenvs)
 
     @property
     def statistics(self):
         return {
             'mean': self._reward_mean,
             'var': self._reward_var,
         }
 
     def _reward_normalize(self, reward):
         self._reward_mean = self.beta * self._reward_mean + (1.0 - self.beta) * reward
-        self._reward_var = self.beta * self._reward_var + (1.0 - self.beta) * np.square(reward, self._reward_mean)
-
-    def reset(self, *args, **kwargs):
-        reward = self.env.reset(*args, **kwargs)
-        return self._reward_normalize(reward)
+        self._reward_var = self.beta * self._reward_var + (1.0 - self.beta) * np.square(reward - self._reward_mean)
+        return (reward - self._reward_mean) / (np.sqrt(self._reward_var) + self.eps)
 
     def step(self, *args, **kwargs):
         state, reward, done, infos = self.env.step(*args, **kwargs)
         return state, self._reward_normalize(reward), done, infos
```

### Comparing `cherry-rl-0.1.4/cherry/envs/runner_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/runner_wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 #!/usr/bin/env python3
 
 import cherry as ch
 from cherry._utils import _min_size, _istensorable
-from .base import Wrapper
-from .utils import is_vectorized
+from cherry.envs.utils import is_vectorized
+from .base_wrapper import Wrapper
 
 from collections.abc import Iterable
 
 
 def flatten_episodes(replay, episodes, num_workers):
-    """
-    TODO: This implementation is not efficient.
+    #  TODO: This implementation is not efficient.
 
-    NOTE: Additional info (other than a transition's default fields) is simply copied.
-    To know from which worker the data was gathered, you can access sars.runner_id
-    TODO: This is not great. What is the best behaviour with infos here ?
-    """
+    #  NOTE: Additional info (other than a transition's default fields) is simply copied.
+    #  To know from which worker the data was gathered, you can access sars.runner_id
+    #  TODO: This is not great. What is the best behaviour with infos here ?
     flat_replay = ch.ExperienceReplay()
     worker_replays = [ch.ExperienceReplay() for w in range(num_workers)]
     flat_episodes = 0
     for sars in replay:
         state = sars.state.view(_min_size(sars.state))
         action = sars.action.view(_min_size(sars.action))
         reward = sars.reward.view(_min_size(sars.reward))
         next_state = sars.next_state.view(_min_size(sars.next_state))
         done = sars.done.view(_min_size(sars.done))
-        fields = set(sars._Transition__fields) - {'state', 'action', 'reward', 'next_state', 'done'}
+        fields = set(sars._fields) - {'state', 'action', 'reward', 'next_state', 'done'}
         infos = {f: getattr(sars, f) for f in fields}
         for worker in range(num_workers):
             infos['runner_id'] = worker
             # The following attemps to split additional infos. (WIP. Remove ?)
             # infos = {}
             # for f in fields:
             #     value = getattr(sars, f)
@@ -58,19 +56,33 @@
             break
     return flat_replay
 
 
 class Runner(Wrapper):
 
     """
-    Runner wrapper.
+    <a href="" class="source-link">[Source]</a>
+
+    ## Description
+
+    Helps collect transitions, given a `get_action` function.
+
+    ## Example
+
+    ~~~python
+    env = MyEnv()
+    env = Runner(env)
+    replay = env.run(lambda x: policy(x), steps=100)
+    # or
+    replay = env.run(lambda x: policy(x), episodes=5)
+    ~~~
 
-    TODO: When is_vectorized and using episodes=n, use the parallel
-    environmnents to sample n episodes, and stack them inside a flat replay.
     """
+    #  TODO: When is_vectorized and using episodes=n, use the parallel
+    #  environmnents to sample n episodes, and stack them inside a flat replay.
 
     def __init__(self, env):
         super(Runner, self).__init__(env)
         self.env = env
         self._needs_reset = True
         self._current_state = None
 
@@ -85,28 +97,39 @@
 
     def run(self,
             get_action,
             steps=None,
             episodes=None,
             render=False):
         """
+        ## Description
+
         Runner wrapper's run method.
+
+        !!! info
+            Either use the `steps` OR the `episodes` argument.
+
+        ## Arguments
+
+        * `get_action` (function) - Given a state, returns the action to be taken.
+        * `steps` (int, *optional*, default=None) - The number of steps to be collected.
+        * `episodes` (int, *optional*, default=None) - The number of episodes to be collected.
         """
 
         if steps is None:
             steps = float('inf')
             if self.is_vectorized:
                 self._needs_reset = True
         elif episodes is None:
             episodes = float('inf')
         else:
             msg = 'Either steps or episodes should be set.'
             raise Exception(msg)
 
-        replay = ch.ExperienceReplay()
+        replay = ch.ExperienceReplay(vectorized=self.is_vectorized)
         collected_episodes = 0
         collected_steps = 0
         while True:
             if collected_steps >= steps or collected_episodes >= episodes:
                 if self.is_vectorized and collected_episodes >= episodes:
                     replay = flatten_episodes(replay, episodes, self.num_envs)
                     self._needs_reset = True
```

### Comparing `cherry-rl-0.1.4/cherry/envs/state_normalizer_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/state_normalizer_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 import numpy as np
-from .base import Wrapper
+from .base_wrapper import Wrapper
 
 
 class StateNormalizer(Wrapper):
 
     """
     [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/envs/normalizer_wrapper.py)
 
@@ -54,15 +54,16 @@
         return {
             'mean': self._state_mean,
             'var': self._state_var,
         }
 
     def _state_normalize(self, state):
         self._state_mean = self.beta * self._state_mean + (1.0 - self.beta) * state
-        self._state_var = self.beta * self._state_var + (1.0 - self.beta) * np.square(state, self._state_mean)
+        self._state_var = self.beta * self._state_var + (1.0 - self.beta) * np.square(state - self._state_mean)
+        return (state - self._state_mean) / (np.sqrt(self._state_var) + self.eps)
 
     def reset(self, *args, **kwargs):
         state = self.env.reset(*args, **kwargs)
         return self._state_normalize(state)
 
     def step(self, *args, **kwargs):
         state, reward, done, infos = self.env.step(*args, **kwargs)
```

### Comparing `cherry-rl-0.1.4/cherry/envs/timestep_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/timestep_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 import numpy as np
 
 from gym import ObservationWrapper
 from gym.spaces import Box
 
-from .base import Wrapper
+from .base_wrapper import Wrapper
 
 
 class AddTimestep(Wrapper, ObservationWrapper):
 
     """
     Adds a timestep information to the state input.
```

### Comparing `cherry-rl-0.1.4/cherry/envs/torch_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/torch_wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 #!/usr/bin/env python3
 
 import numpy as np
 import torch as th
 import cherry as ch
 
-from gym.spaces import Discrete
-
-from .base import Wrapper
-from .utils import is_vectorized
+from .base_wrapper import Wrapper
 
 
 class Torch(Wrapper):
 
     """
     This wrapper converts
         * actions from Tensors to numpy,
         * states from lists/numpy to Tensors.
 
     Example:
         action = Categorical(Tensor([1, 2, 3])).sample()
         env.step(action)
     """
 
+    def __init__(self, env, device=None, env_device=None):
+        super(Torch, self).__init__(env)
+        self.device = device
+        self.env_device = env_device
+
     def _convert_state(self, state):
-        if isinstance(state, (float, int)):
-            state = ch.totensor(state)
         if isinstance(state, dict):
             state = {k: self._convert_state(state[k]) for k in state}
-        if isinstance(state, np.ndarray):
+        else:
             state = ch.totensor(state)
-        # we need to check for num_envs because self.is_vectorized returns
-        # False when the num_envs=1, but the state still needs squeezing.
-        if hasattr(self, 'num_envs') and isinstance(state, th.Tensor):
-            state = state.squeeze(0)
         return state
 
     def _convert_atomic_action(self, action):
         if isinstance(action, th.Tensor):
+            if self.env_device is not None:
+                action = action.to(self.env_device)
             action = action.view(-1).cpu().detach().numpy()
         if self.discrete_action:
             if not isinstance(action, (int, float)):
                 action = action[0]
             action = int(action)
         return action
 
@@ -55,16 +53,20 @@
             action = self._convert_atomic_action(action)
         return action
 
     def step(self, action):
         action = self._convert_action(action)
         state, reward, done, info = self.env.step(action)
         state = self._convert_state(state)
+        if self.device is not None:
+            state = state.to(self.device)
         return state, reward, done, info
 
     def reset(self, *args, **kwargs):
         state = self.env.reset(*args, **kwargs)
         state = self._convert_state(state)
+        if self.device is not None:
+            state = state.to(self.device)
         return state
 
     def seed(self, *args, **kwargs):
         return self.env.seed(*args, **kwargs)
```

### Comparing `cherry-rl-0.1.4/cherry/envs/utils.py` & `cherry-rl-0.2.0/cherry/envs/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,39 +4,72 @@
 **Description**
 
 Helper functions for OpenAI Gym environments.
 """
 
 
 import operator
+import numpy as np
 
 from functools import reduce
 from collections import OrderedDict
 
-from gym.spaces import Box, Discrete, Dict, Tuple
+from gym.spaces import Box, Discrete, Dict, Tuple, MultiDiscrete
+
+
+def num_envs(env):
+    """
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/envs/utils.py" class="source-link">[Source]</a>
+
+    ## Description
+
+    Heuristic that returns the number of parallel workers in a vectorized environment.
+
+    Warning: functionality is experimental, mostly tested with `gym.vector`.
+    """
+    if hasattr(env, 'num_envs'):
+        return env.num_envs
+    if hasattr(env, 'envs'):
+        return len(env.envs)
+    if hasattr(env, 'processes'):
+        return len(env.processes)
+    return 1
 
 
 def is_vectorized(env):
-    return hasattr(env, 'num_envs') and env.num_envs > 1
+    """
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/envs/utils.py" class="source-link">[Source]</a>
+
+    ## Description
+
+    Heuristic that returns whether an environment is vectorized or not.
+
+    Warning: functionality is experimental, mostly tested with `gym.vector`.
+    """
+    return num_envs(env) > 1
 
 
 def is_discrete(space, vectorized=False):
     """
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/envs/utils.py" class="source-link">[Source]</a>
+
+    ## Description
+
     Returns whether a space is discrete.
 
-    **Arguments**
+    ## Arguments
 
-    * **space** - The space.
-    * **vectorized** - Whether to return the discreteness for the
+    * `space` - The space.
+    * `vectorized` - Whether to return the discreteness for the
         vectorized environments (True) or just the discreteness of
         the underlying environment (False).
     """
     msg = 'Space type not supported.'
-    assert isinstance(space, (Box, Discrete, Dict, Tuple)), msg
-    if isinstance(space, Discrete):
+    assert isinstance(space, (Box, Discrete, Dict, Tuple, MultiDiscrete)), msg
+    if isinstance(space, (Discrete, MultiDiscrete)):
         return True
     if isinstance(space, Box):
         return False
     if isinstance(space, Dict):
         dimensions = {
             k[0]: is_discrete(k[1], vectorized) for k in space.spaces.items()
         }
@@ -48,27 +81,35 @@
             is_discrete(s) for s in space
         )
         return discrete
 
 
 def get_space_dimension(space, vectorized_dims=False):
     """
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/envs/utils.py" class="source-link">[Source]</a>
+
+    ## Description
+
     Returns the number of elements of a space sample, when unrolled.
 
-    **Arguments**
+    ## Arguments
 
-    * **space** - The space.
-    * **vectorized_dims** - Whether to return the full dimension for vectorized
+    * `space` - The space.
+    * `vectorized_dims` - Whether to return the full dimension for vectorized
         environments (True) or just the dimension for the underlying
         environment (False).
     """
     msg = 'Space type not supported.'
-    assert isinstance(space, (Box, Discrete, Dict, Tuple)), msg
+    assert isinstance(space, (Box, Discrete, Dict, Tuple, MultiDiscrete)), msg
     if isinstance(space, Discrete):
         return space.n
+    if isinstance(space, MultiDiscrete):
+        if vectorized_dims:
+            return reduce(operator.mul, space.nvec, 1)
+        return int(space.nvec[0])
     if isinstance(space, Box):
         if len(space.shape) > 1 and not vectorized_dims:
             return reduce(operator.mul, space.shape[1:], 1)
         return reduce(operator.mul, space.shape, 1)
     if isinstance(space, Dict):
         dimensions = {
             k[0]: get_space_dimension(k[1], vectorized_dims) for k in space.spaces.items()
```

### Comparing `cherry-rl-0.1.4/cherry/envs/visdom_logger_wrapper.py` & `cherry-rl-0.2.0/cherry/wrappers/visdom_logger_wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import uuid
 import numpy as np
 import cherry as ch
 
 from gym.spaces import Discrete
 
-from .base import Wrapper
+from .base_wrapper import Wrapper
 from .logger_wrapper import Logger
 
 try:
     import visdom
 except ImportError:
     visdom = ch._utils._ImportRaiser('Visdom', 'pip install visdom')
 
@@ -21,15 +21,14 @@
     Enables logging and debug values to Visdom.
 
     Arguments
 
     * env: The environment to wrap.
     * interval: (int) Update frequency for episodes.
 
-
     """
 
     def __init__(self,
                  env,
                  interval=1000,
                  episode_interval=10,
                  render=True,
@@ -94,15 +93,15 @@
         for i in range(num_actions):
             x_in = [None] * num_steps
             y_in = [None] * num_steps
             z_in = [None] * num_steps
             z_buff = float(ribbon_data[0][i])
 
             for j, step_action in enumerate(ribbon_data):
-                x_in[j] = [i*2, i*2 + 1]
+                x_in[j] = [i * 2, i * 2 + 1]
                 y_in[j] = [j, j]
                 z_buff = 0.5 * z_buff + 0.5 * float(step_action[i])
                 z_in[j] = [z_buff, z_buff]
 
             trace = dict(x=x_in,
                          y=y_in,
                          z=z_in,
@@ -170,21 +169,22 @@
         return state, reward, done, info
 
     def log(self, key, value, opts=None):
         super(VisdomLogger, self).log(key=key, value=value)
         # Create the plot
         if key not in self.values_plots:
             if opts is None:
-                opts = {'title': key,
-                        'layoutopts': {
-                            'plotly': {
-                                'xaxis': {'title': 'Log'},
-                            }
-                            }
+                opts = {
+                    'title': key,
+                    'layoutopts': {
+                        'plotly': {
+                            'xaxis': {'title': 'Log'},
                         }
+                    }
+                }
             elif 'title' not in opts:
                 opts['title'] = key
             self.values_plots[key] = self.visdom.line(X=np.empty(1),
                                                       Y=np.empty(1),
                                                       opts=opts)
 
     def update_steps_plots(self, stats):
@@ -199,15 +199,15 @@
                                  win=self.values_plots[key],
                                  update=update)
 
     def update_ep_plots(self, stats):
         num_logs = len(self.all_rewards) // self.interval
         update = 'replace' if num_logs <= 1 else 'append'
         for key in stats:
-            if key is not 'num_episodes':
+            if key != 'num_episodes':
                 x_values = np.zeros((1,)) + num_logs
                 y_values = np.array([np.mean(stats[key])])
                 self.visdom.line(X=x_values,
                                  Y=y_values,
                                  win=self.values_plots[key],
                                  update=update)
```

### Comparing `cherry-rl-0.1.4/cherry/experience_replay.py` & `cherry-rl-0.2.0/cherry/experience_replay.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,79 +11,113 @@
 """
 
 
 class Transition(object):
 
     """
 
-    **Description**
+    <a href="https://github.com/learnables/cherry/blob/master/cherry/experience_replay.py" class="source-link">[Source]</a>
+
+    ## Description
 
     Represents a (s, a, r, s', d) tuple.
 
     All attributes (including the ones in infos) are accessible via
     `transition.name_of_attr`.
     (e.g. `transition.log_prob` if `log_prob` is in `infos`.)
 
-    **Arguments**
-
-    * **state** (tensor) - Originating state.
-    * **action** (tensor) - Executed action.
-    * **reward** (tensor) - Observed reward.
-    * **next_state** (tensor) - Resulting state.
-    * **done** (tensor) - Is `next_state` a terminal (absorbing) state ?
-    * **infos** (dict, *optional*, default=None) - Additional information on
-      the transition.
-
-    **Example**
+    ## Example
 
     ~~~python
     for transition in replay:
         print(transition.state)
     ~~~
     """
 
+    _reserved_names = ('device', '_fields')
+
     def __init__(self,
                  state,
                  action,
                  reward,
                  next_state,
                  done,
                  device=None,
                  **infos):
-        self.__fields = ['state', 'action', 'reward', 'next_state', 'done']
-        values = [state, action, reward, next_state, done]
-        for key, val in zip(self.__fields, values):
-            setattr(self, key, val)
-        info_keys = infos.keys()
-        self.__fields += info_keys
-        for key in info_keys:
-            setattr(self, key, infos[key])
-        self.device = device
+        """
+
+        ## Arguments
+
+        * `state` (tensor) - Originating state.
+        * `action` (tensor) - Executed action.
+        * `reward` (tensor) - Observed reward.
+        * `next_state` (tensor) - Resulting state.
+        * `done` (tensor) - Is `next_state` a terminal (absorbing) state ?
+        * `infos` (dict, *optional*, default=None) - Additional information on
+          the transition.
+
+        """
+        super(Transition, self).__setattr__('device', device)
+        super(Transition, self).__setattr__(
+            '_fields',
+            ['state', 'action', 'reward', 'next_state', 'done']
+        )
+        values = [state, action, reward, next_state, done, device]
+        for key, val in zip(self._fields, values):
+            super(Transition, self).__setattr__(key, val)
+
+        if infos:
+            info_keys = infos.keys()
+            self._fields += info_keys
+            for key in info_keys:
+                setattr(self, key, infos[key])
+
+    def __setattr__(self, name, value):
+        if name not in self._reserved_names:
+            fields = getattr(self, '_fields')
+            if name not in fields:
+                self._fields.append(name)
+        return super(Transition, self).__setattr__(name, value)
 
     def __str__(self):
-        string = 'Transition(' + ', '.join(self.__fields)
+        string = 'Transition(' + ', '.join(self._fields)
         if self.device is not None:
             string += ', device=\'' + str(self.device) + '\''
         string += ')'
         return string
 
     def __repr__(self):
         return str(self)
 
+    def __getstate__(self):
+        state = {
+            key: getattr(self, key) for key in self._fields
+        }
+        state['device'] = self.device
+        return state
+
+    def __setstate__(self, state):
+        self._fields = ['state', 'action', 'reward', 'next_state', 'done']
+        for key, value in state.items():
+            setattr(self, key, value)
+            if key not in self._fields:
+                self._fields.append(key)
+        self.device = state['device']
+
     def cpu(self):
         return self.to('cpu')
 
     def cuda(self, device=0, *args, **kwargs):
         return self.to('cuda:' + str(device), *args, **kwargs)
 
     def _apply(self, fn, device=None):
         if device is None:
             device = self.device
         new_transition = {'device': device}
-        for field in self.__fields:
+        for field in self._fields:
             value = getattr(self, field)
             if isinstance(value, th.Tensor):
                 new_transition[field] = fn(value)
             else:
                 new_transition[field] = value
         return Transition(**new_transition)
 
@@ -119,46 +153,36 @@
     def double(self):
         return self._apply(lambda t: t.double() if t.is_floating_point() else t)
 
 
 class ExperienceReplay(list):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/experience_replay.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/experience_replay.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Experience replay buffer to store, retrieve, and sample past transitions.
 
     `ExperienceReplay` behaves like a list of transitions, .
     It also support accessing specific properties, such as states, actions,
     rewards, next_states, and informations.
     The first four are returned as tensors, while `infos` is returned as
     a list of dicts.
     The properties of infos can be accessed directly by appending an `s` to
     their dictionary key -- see Examples below.
     In this case, if the values of the infos are tensors, they will be returned
     as a concatenated Tensor.
     Otherwise, they default to a list of values.
 
-    **Arguments**
-
-    * **states** (Tensor, *optional*, default=None) - Tensor of states.
-    * **actions** (Tensor, *optional*, default=None) - Tensor of actions.
-    * **rewards** (Tensor, *optional*, default=None) - Tensor of rewards.
-    * **next_states** (Tensor, *optional*, default=None) - Tensor of
-      next_states.
-    * **dones** (Tensor, *optional*, default=None) - Tensor of dones.
-    * **infos** (list, *optional*, default=None) - List of infos.
-
-    **References**
+    ## References
 
     1. Lin, Long-Ji. 1992. “Self-Improving Reactive Agents Based on Reinforcement Learning, Planning and Teaching.” Machine Learning 8 (3): 293–321.
 
-    **Example**
+    ## Example
 
     ~~~python
     replay = ch.ExperienceReplay()  # Instanciate a new replay
     replay.append(state,  # Add experience to the replay
                   action,
                   reward,
                   next_state,
@@ -175,49 +199,80 @@
     new_replay = replay[-10:]  # Last 10 transitions in new_replay
 
     #Sample some previous experience
     batch = replay.sample(32, contiguous=True)
     ~~~
     """
 
-    def __init__(self, storage=None, device=None):
+    def __init__(self, storage=None, device=None, vectorized=False):
+        """
+        ## Arguments
+
+        * `storage` (list, *optional*, default=None) - A list of Transitions.
+        * `device` (torch.device, *optional*, default=None) - The device of the replay.
+        * `vectorized` (bool, *optional*, default=False) - Whether the transitions are vectorized or not.
+
+        """
         list.__init__(self)
         if storage is None:
             storage = []
         self._storage = storage
+        self.vectorized = vectorized
         self.device = device
 
     def _access_property(self, name):
         try:
             values = [getattr(sars, name) for sars in self._storage]
         except AttributeError:
             msg = 'Attribute ' + name + ' not in replay.'
             raise AttributeError(msg)
-        true_size = _min_size(values[0])
-        return th.cat(values, dim=0).view(len(values), *true_size)
+        if values:
+            true_size = _min_size(values[0])
+            return th.cat(values, dim=0).view(len(values), *true_size)
+        return th.empty(0)
+
+    def __getstate__(self):
+        return {
+            'storage': self._storage,
+            'vectorized': self.vectorized,
+            'device': self.device,
+        }
+
+    def __setstate__(self, state):
+        self._storage = state['storage']
+        self.vectorized = state['vectorized']
+        self.device = state['device']
 
     def __getslice__(self, i, j):
         return self.__getitem__(slice(i, j))
 
     def __len__(self):
         return len(self._storage)
 
     def __str__(self):
         string = 'ExperienceReplay(' + str(len(self))
         if self.device is not None:
             string += ', device=\'' + str(self.device) + '\''
+        if self.vectorized:
+            string += ', vectorized=\'' + str(self.vectorized) + '\''
         string += ')'
         return string
 
     def __repr__(self):
         return str(self)
 
     def __add__(self, other):
+        assert self.vectorized == other.vectorized, \
+            'Cannot add vectorized and non-vectorized replays.'
         storage = self._storage + other._storage
-        return ExperienceReplay(storage)
+        return ExperienceReplay(
+            storage,
+            device=self.device,
+            vectorized=self.vectorized
+        )
 
     def __iadd__(self, other):
         self._storage += other._storage
         return self
 
     def __iter__(self):
         for i in range(len(self)):
@@ -225,124 +280,149 @@
 
     def __getattr__(self, attr):
         return lambda: self._access_property(attr)
 
     def __getitem__(self, key):
         value = self._storage[key]
         if isinstance(key, slice):
-            return ExperienceReplay(value)
+            return ExperienceReplay(
+                storage=value,
+                device=self.device,
+                vectorized=self.vectorized,
+            )
         return value
 
     def save(self, path):
         """
-        **Description**
+        ## Description
 
         Serializes and saves the ExperienceReplay into the given path.
 
-        **Arguments**
+        ## Arguments
 
-        * **path** (str) - File path.
+        * `path` (str) - File path.
+
+        ## Example
 
-        **Example**
         ~~~python
         replay.save('my_replay_file.pt')
         ~~~
         """
-        th.save(self._storage, path)
+        state = self.__getstate__()
+        th.save(state, path)
 
     def load(self, path):
         """
-        **Description**
+        ## Description
 
         Loads data from a serialized ExperienceReplay.
 
-        **Arguments**
+        ## Arguments
 
-        * **path** (str) - File path of serialized ExperienceReplay.
+        * `path` (str) - File path of serialized ExperienceReplay.
+
+        ## Example
 
-        **Example**
         ~~~python
         replay.load('my_replay_file.pt')
         ~~~
         """
-        self._storage = th.load(path)
+        state = th.load(path)
+        self.__setstate__(state)
 
     def append(self,
                state=None,
                action=None,
                reward=None,
                next_state=None,
                done=None,
                **infos):
         """
-        **Description**
+        ## Description
 
         Appends new data to the list ExperienceReplay.
 
-        **Arguments**
+        ## Arguments
 
-        * **state** (tensor/ndarray/list) - Originating state.
-        * **action** (tensor/ndarray/list) - Executed action.
-        * **reward** (tensor/ndarray/list) - Observed reward.
-        * **next_state** (tensor/ndarray/list) - Resulting state.
-        * **done** (tensor/bool) - Is `next_state` a terminal (absorbing)
-          state ?
-        * **infos** (dict, *optional*, default=None) - Additional information
-          on the transition.
+        * `state` (tensor/ndarray/list) - Originating state.
+        * `action` (tensor/ndarray/list) - Executed action.
+        * `reward` (tensor/ndarray/list) - Observed reward.
+        * `next_state` (tensor/ndarray/list) - Resulting state.
+        * `done` (tensor/bool) - Is `next_state` a terminal (absorbing) state ?
+        * infos` (dict, *optional*, default=None) - Additional information on the transition.
+
+        ## Example
 
-        **Example**
         ~~~python
         replay.append(state, action, reward, next_state, done, info={
             'density': density,
             'log_prob': density.log_prob(action),
         })
         ~~~
         """
         for key in infos:
             if _istensorable(infos[key]):
                 infos[key] = ch.totensor(infos[key])
-        sars = Transition(ch.totensor(state),
-                          ch.totensor(action),
-                          ch.totensor(reward),
-                          ch.totensor(next_state),
-                          ch.totensor(done),
-                          **infos)
+        state = ch.totensor(state)
+        action = ch.totensor(action)
+        reward = ch.totensor(reward)
+        next_state = ch.totensor(next_state)
+        done = ch.totensor(done)
+        if self.vectorized:
+            num_envs = state.shape[0]
+            action = action.reshape(num_envs, -1)
+            reward = reward.reshape(num_envs, -1)
+            done = done.reshape(num_envs, -1)
+        sars = Transition(
+            state=state,
+            action=action,
+            reward=reward,
+            next_state=next_state,
+            done=done,
+            **infos,
+        )
         self._storage.append(sars.to(self.device))
 
-    def sample(self, size=1, contiguous=False, episodes=False):
+    def sample(self, size=1, contiguous=False, episodes=False, nsteps=1, discount=1.0):
         """
         Samples from the Experience replay.
 
-        **Arguments**
+        ## Arguments
 
-        * **size** (int, *optional*, default=1) - The number of samples.
-        * **contiguous** (bool, *optional*, default=False) - Whether to sample
-          contiguous transitions.
-        * **episodes** (bool, *optional*, default=False) - Sample full
-          episodes, instead of transitions.
+        * `size` (int, *optional*, default=1) - The number of samples.
+        * `contiguous` (bool, *optional*, default=False) - Whether to sample contiguous transitions.
+        * `episodes` (bool, *optional*, default=False) - Sample full episodes, instead of transitions.
+        * `nsteps` (int, *optional*, default=1) - Steps to compute the n-steps returns.
+        * `discount` (float, *optional*, default=1.0) - Discount for n-steps returns.
 
-        **Return**
+        ## Returns
 
-        * ExperienceReplay - New ExperienceReplay containing the sampled
-          transitions.
+        * `ExperienceReplay` - New ExperienceReplay containing the sampled transitions.
         """
         if len(self) < 1 or size < 1:
-            return ExperienceReplay()
+            return ExperienceReplay(vectorized=self.vectorized)
 
         indices = []
         if episodes:
+            assert not self.vectorized, 'Cannot sample episodes from vectorized replay yet.'
             if size > 1 and not contiguous:
                 replay = ExperienceReplay()
-                return sum([self.sample(1, episodes=True) for _ in range(size)], replay)
+                return sum([self.sample(
+                    size=1,
+                    episodes=True,
+                    contiguous=False,
+                    nsteps=nsteps,
+                    discount=discount,
+                ) for _ in range(size)], replay)
             else:  # Sample 'size' contiguous episodes
-                num_episodes = self.done().sum().int().item()
-                end = random.randint(size-1, num_episodes-size)
+                dones = self.done()
+                num_episodes = dones.sum().int().item()
+                end = random.randint(0, num_episodes - size)
                 # Find idx of the end-th done
                 count = 0
-                dones = self.done()
                 for idx, d in reversed(list(enumerate(dones))):
                     if bool(d):
                         if count >= end:
                             end_idx = idx
                             break
                         count += 1
                 # Fill indices
@@ -359,65 +439,148 @@
             if contiguous:
                 start = random.randint(0, length - size)
                 indices = list(range(start, start + size))
             else:
                 indices = [random.randint(0, length) for _ in range(size)]
 
         # Fill the sample
-        storage = [self[idx] for idx in indices]
-        return ExperienceReplay(storage)
+        if nsteps == 1:
+            storage = [self[idx] for idx in indices]
+        else:
+            assert not self.vectorized, \
+                'Cannot sample n-steps with vectorized replays yet.'
+            assert nsteps > 0, 'Invalid nsteps < 1.'
+            # TODO: These two loops are quite slow.
+            enum_steps = list(range(1, nsteps))
+            replay_size = len(self)
+            for idx, index in enumerate(indices):
+                sars = self._storage[index]
+                state = sars.state
+                action = sars.action
+                next_state = sars.next_state
+                done = sars.done
+                reward = sars.reward
+                for i in enum_steps:
+                    j = i + index
+                    if done or j >= replay_size:
+                        break
+                    next_sars = self._storage[j]
+                    reward = reward + discount**i * next_sars.reward
+                    done = next_sars.done
+                    next_state = next_sars.next_state
+                new_sars = Transition(
+                    state=state,
+                    action=action,
+                    reward=reward,
+                    next_state=next_state,
+                    done=done,
+                )
+                for field in sars._fields[5:]:
+                    super(Transition, new_sars).__setattr__(
+                        field,
+                        getattr(sars, field),
+                    )
+                indices[idx] = new_sars
+            storage = indices
+        return ExperienceReplay(
+            storage=storage,
+            device=self.device,
+            vectorized=self.vectorized,
+        )
 
     def empty(self):
         """
-        **Description**
+        ## Description
 
         Removes all data from an ExperienceReplay.
 
-        **Example**
+        ## Example
+
         ~~~python
         replay.empty()
         ~~~
         """
         self._storage = []
 
+    def flatten(self):
+        """
+        ## Description
+
+        Returns a "flattened" version of the replay, where each transition only contains one timestep.
+
+        Assuming the original replay has N transitions each with M timesteps -- i.e. sars.state
+        with shapes (M, *state_size) -- this method returns a new replay with N*M transitions (and
+        the states have shape (*state_size)).
+
+        Note: This method breaks the timestep orders, so transitions are not consecutive anymore.
+
+        Note: No-op if not vectorized.
+
+        ## Example
+
+        ~~~python
+        flat_replay = replay.flatten()
+        ~~~
+        """
+        if not self.vectorized:
+            return self
+        flat_replay = ch.ExperienceReplay(device=self.device, vectorized=False)
+        storage = []
+        for sars in self._storage:
+            vec_num = sars.done.shape[0]
+            transitions = [{} for _ in range(vec_num)]
+            for field in sars._fields:
+                values = getattr(sars, field)
+                if isinstance(values, th.Tensor):
+                    values = values.chunk(vec_num, dim=0)
+                for trans, val in zip(transitions, values):
+                    trans[field] = val
+            transitions = [ch.Transition(**trans) for trans in transitions]
+            storage += transitions
+        return ch.ExperienceReplay(
+            storage=storage,
+            device=self.device,
+            vectorized=False,
+        )
+
     def cpu(self):
         return self.to('cpu')
 
     def cuda(self, device=0, *args, **kwargs):
         return self.to('cuda:' + str(device), *args, **kwargs)
 
     def to(self, *args, **kwargs):
         """
-        **Description**
+        ## Description
 
         Calls `.to()` on all transitions of the experience replay, moving them to the
         desired device and casting the to the desired format.
 
         Note: This return a new experience replay, but the transitions are modified in-place.
 
-        **Arguments**
+        ## Arguments
 
-        * **device** (device, *optional*, default=None) - The device to move the data to.
-        * **dtype** (dtype, *optional*, default=None) - The torch.dtype format to cast to.
-        * **non_blocking** (bool, *optional*, default=False) - Whether to perform the move asynchronously.
+        * `device` (device, *optional*, default=None) - The device to move the data to.
+        * `dtype` (dtype, *optional*, default=None) - The torch.dtype format to cast to.
+        * `non_blocking` (bool, *optional*, default=False) - Whether to perform the move asynchronously.
 
-        **Example**
+        ## Example
 
         ~~~python
         replay.to('cuda:1')
         policy.to('cuda:1')
         for sars in replay:
             cuda_action = policy(sars.state).sample()
         ~~~
 
         """
         device, dtype, non_blocking, *_ = th._C._nn._parse_to(*args, **kwargs)
         storage = [sars.to(*args, **kwargs) for sars in self._storage]
-        return ExperienceReplay(storage, device=device)
+        return ExperienceReplay(storage, device=device, vectorized=self.vectorized)
 
     def half(self):
         storage = [sars.half() for sars in self._storage]
-        return ExperienceReplay(storage, device=self.device)
+        return ExperienceReplay(storage, device=self.device, vectorized=self.vectorized)
 
     def double(self):
         storage = [sars.double() for sars in self._storage]
-        return ExperienceReplay(storage, device=self.device)
+        return ExperienceReplay(storage, device=self.device, vectorized=self.vectorized)
```

### Comparing `cherry-rl-0.1.4/cherry/models/atari.py` & `cherry-rl-0.2.0/cherry/models/atari.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,100 +14,105 @@
     def forward(self, x):
         return x.view(x.size(0), -1)
 
 
 class NatureFeatures(nn.Sequential):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/atari.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/atari.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     The convolutional body of the DQN architecture.
 
-    **References**
+    ## References
 
     1. Mnih et al. 2015. “Human-Level Control through Deep Reinforcement Learning.”
     2. Mnih et al. 2016. “Asynchronous Methods for Deep Reinforcement Learning.”
 
-    **Credit**
+    ## Credit
 
     Adapted from Ilya Kostrikov's implementation.
 
-    **Arguments**
-
-    * **input_size** (int) - Number of channels.
-      (Stacked frames in original implementation.)
-    * **output_size** (int, *optional*, default=512) - Size of the output
-      representation.
     """
 
-    def __init__(self, input_size=4, hidden_size=512):
+    def __init__(self, input_size=4, output_size=512, hidden_size=64 * 7 * 7):
+        """
+        ## Arguments
+
+        * `input_size` (int) - Number of channels.
+          (Stacked frames in original implementation.)
+        * `output_size` (int, *optional*, default=512) - Size of the output
+          representation.
+        * `hidden_size` (int, *optional*, default=1568) - Size of the representation
+          after the convolutional layers
+        """
         super(NatureFeatures, self).__init__(
             atari_init_(nn.Conv2d(input_size, 32, 8, stride=4, padding=0)),
             nn.ReLU(),
             atari_init_(nn.Conv2d(32, 64, 4, stride=2, padding=0)),
             nn.ReLU(),
-            atari_init_(nn.Conv2d(64, 32, 3, stride=1, padding=0)),
+            atari_init_(nn.Conv2d(64, 64, 3, stride=1, padding=0)),
             nn.ReLU(),
             Flatten(),
-            atari_init_(nn.Linear(32 * 7 * 7, hidden_size)),
+            atari_init_(nn.Linear(hidden_size, output_size)),
             nn.ReLU()
         )
 
 
 class NatureActor(nn.Linear):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/atari.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/atari.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     The actor head of the A3C architecture.
 
-    **References**
+    ## References
 
     1. Mnih et al. 2015. “Human-Level Control through Deep Reinforcement Learning.”
     2. Mnih et al. 2016. “Asynchronous Methods for Deep Reinforcement Learning.”
 
-    **Credit**
+    ## Credit
 
     Adapted from Ilya Kostrikov's implementation.
 
-    **Arguments**
+    ## Arguments
 
-    * **input_size** (int) - Size of input of the fully connected layers
-    * **output_size** (int) - Size of the action space.
+    * `input_size` (int) - Size of input of the fully connected layers
+    * `output_size` (int) - Size of the action space.
     """
 
     def __init__(self, input_size, output_size):
         super(NatureActor, self).__init__(input_size, output_size)
         atari_init_(self, gain=0.01)
 
 
 class NatureCritic(nn.Linear):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/atari.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/atari.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     The critic head of the A3C architecture.
 
-    **References**
+    ## References
 
     1. Mnih et al. 2015. “Human-Level Control through Deep Reinforcement Learning.”
     2. Mnih et al. 2016. “Asynchronous Methods for Deep Reinforcement Learning.”
 
-    **Credit**
+    ## Credit
 
     Adapted from Ilya Kostrikov's implementation.
-
-    **Arguments**
-
-    * **input_size** (int) - Size of input of the fully connected layers
-    * **output_size** (int, *optional*, default=1) - Size of the value.
     """
 
     def __init__(self, input_size, output_size=1):
+        """
+        ## Arguments
+
+        * `input_size` (int) - Size of input of the fully connected layers
+        * `output_size` (int, *optional*, default=1) - Size of the value.
+        """
         super(NatureCritic, self).__init__(input_size, output_size)
         atari_init_(self, gain=1.0)
```

### Comparing `cherry-rl-0.1.4/cherry/models/robotics.py` & `cherry-rl-0.2.0/cherry/models/robotics.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,41 +5,43 @@
 
 from cherry.nn import RoboticsLinear
 
 
 class RoboticsMLP(nn.Module):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/robotics.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/robotics.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     A multi-layer perceptron with proper initialization for robotic control.
 
-    **Credit**
+    ## Credit
 
     Adapted from Ilya Kostrikov's implementation.
 
-    **Arguments**
+    ## Example
 
-    * **inputs_size** (int) - Size of input.
-    * **output_size** (int) - Size of output.
-    * **layer_sizes** (list, *optional*, default=None) - A list of ints,
-      each indicating the size of a hidden layer.
-      (Defaults to two hidden layers of 64 units.)
-
-    **Example**
     ~~~python
     target_qf = ch.models.robotics.RoboticsMLP(23,
                                              34,
                                              layer_sizes=[32, 32])
     ~~~
     """
 
     def __init__(self, input_size, output_size, layer_sizes=None):
+        """
+        ## Arguments
+
+        * `inputs_size` (int) - Size of input.
+        * `output_size` (int) - Size of output.
+        * `layer_sizes` (list, *optional*, default=None) - A list of ints,
+          each indicating the size of a hidden layer.
+          (Defaults to two hidden layers of 64 units.)
+        """
         super(RoboticsMLP, self).__init__()
         if layer_sizes is None:
             layer_sizes = [64, 64]
         if len(layer_sizes) > 0:
             layers = [RoboticsLinear(input_size, layer_sizes[0]),
                       nn.Tanh()]
             for in_, out_ in zip(layer_sizes[:-1], layer_sizes[1:]):
@@ -53,42 +55,44 @@
     def forward(self, x):
         return self.layers(x)
 
 
 class RoboticsActor(RoboticsMLP):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/robotics.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/robotics.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     A multi-layer perceptron with initialization designed for choosing
     actions in continuous robotic environments.
 
-    **Credit**
+    ## Credit
 
     Adapted from Ilya Kostrikov's implementation.
 
-    **Arguments**
+    ## Example
 
-    * **inputs_size** (int) - Size of input.
-    * **output_size** (int) - Size of action size.
-    * **layer_sizes** (list, *optional*, default=None) - A list of ints,
-      each indicating the size of a hidden layer.
-      (Defaults to two hidden layers of 64 units.)
-
-    **Example**
     ~~~python
     policy_mean = ch.models.robotics.Actor(28,
                                           8,
                                           layer_sizes=[64, 32, 16])
     ~~~
     """
 
     def __init__(self, input_size, output_size, layer_sizes=None):
+        """
+        ## Arguments
+
+        * `inputs_size` (int) - Size of input.
+        * `output_size` (int) - Size of action size.
+        * `layer_sizes` (list, *optional*, default=None) - A list of ints,
+          each indicating the size of a hidden layer.
+          (Defaults to two hidden layers of 64 units.)
+        """
         super(RoboticsMLP, self).__init__()
         if layer_sizes is None:
             layer_sizes = [64, 64]
         if len(layer_sizes) > 0:
             layers = [RoboticsLinear(input_size, layer_sizes[0]),
                       nn.Tanh()]
             for in_, out_ in zip(layer_sizes[:-1], layer_sizes[1:]):
@@ -101,66 +105,89 @@
             layers = [RoboticsLinear(input_size, output_size, gain=1.0)]
         self.layers = nn.Sequential(*layers)
 
 
 class LinearValue(nn.Module):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/robotics.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/robotics.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     A linear state-value function, whose parameters are found by minimizing
     least-squares.
 
-    **Credit**
+    ## Credit
 
     Adapted from Tristan Deleu's implementation.
 
-    **References**
+    ## References
 
     1. Duan et al. 2016. “Benchmarking Deep Reinforcement Learning for Continuous Control.”
     2. [https://github.com/tristandeleu/pytorch-maml-rl](https://github.com/tristandeleu/pytorch-maml-rl)
 
-    **Arguments**
+    ## Example
 
-    * **inputs_size** (int) - Size of input.
-    * **reg** (float, *optional*, default=1e-5) - Regularization coefficient.
-
-    **Example**
     ~~~python
     states = replay.state()
     rewards = replay.reward()
     dones = replay.done()
     returns = ch.td.discount(gamma, rewards, dones)
     baseline = LinearValue(input_size)
     baseline.fit(states, returns)
     next_values = baseline(replay.next_states())
     ~~~
     """
 
     def __init__(self, input_size, reg=1e-5):
+        """
+        ## Arguments
+
+        * `inputs_size` (int) - Size of input.
+        * `reg` (float, *optional*, default=1e-5) - Regularization coefficient.
+        """
         super(LinearValue, self).__init__()
         self.linear = nn.Linear(2 * input_size + 4, 1, bias=False)
         self.reg = reg
 
     def _features(self, states):
         length = states.size(0)
         ones = th.ones(length, 1).to(states.device)
         al = th.arange(length, dtype=th.float32, device=states.device).view(-1, 1) / 100.0
         return th.cat([states, states**2, al, al**2, al**3, ones], dim=1)
 
     def fit(self, states, returns):
+        """
+        ## Description
+
+        Fits the parameters of the linear model by the method of least-squares.
+
+        ## Arguments
+
+        * `states` (tensor) - States collected with the policy to evaluate.
+        * `returns` (tensor) - Returns associated with those states (ie, discounted rewards).
+        """
         features = self._features(states)
         reg = self.reg * th.eye(features.size(1))
         reg = reg.to(states.device)
         A = features.t() @ features + reg
         b = features.t() @ returns
-        if hasattr(th, 'lstsq'):  # Required for torch < 1.3.0
+        if hasattr(th, 'linalg') and hasattr(th.linalg, 'lstsq'):
+            coeffs = th.linalg.lstsq(A, b).solution
+        elif hasattr(th, 'lstsq'):  # Required for torch < 1.3.0
             coeffs, _ = th.lstsq(b, A)
         else:
             coeffs, _ = th.gels(b, A)
         self.linear.weight.data = coeffs.data.t()
 
-    def forward(self, states):
-        features = self._features(states)
+    def forward(self, state):
+        """
+        ## Description
+
+        Computes the value of a state using the linear function approximator.
+
+        ## Arguments
+
+        * `state` (Tensor) - The state to evaluate.
+        """
+        features = self._features(state)
         return self.linear(features)
```

### Comparing `cherry-rl-0.1.4/cherry/models/tabular.py` & `cherry-rl-0.2.0/cherry/models/tabular.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,130 @@
 #!/usr/bin/env python3
 
-import torch as th
+import cherry
+import torch
 import torch.nn as nn
 
 
 class StateValueFunction(nn.Module):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/tabular.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/tabular.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Stores a table of state values, V(s), one for each state.
 
     Assumes that the states are one-hot encoded.
     Also, the returned values are differentiable and can be used in
     conjunction with PyTorch's optimizers.
 
-    **Arguments**
-
-    * **state_size** (int) - The number of states in the environment.
-    * **init** (function, *optional*, default=None) - The initialization
-      scheme for the values in the table. (Default is 0.)
-
-    **References**
+    ## References
 
     1. Sutton, Richard, and Andrew Barto. 2018. Reinforcement Learning, Second Edition. The MIT Press.
 
-    **Example**
+    ## Example
+
     ~~~python
     vf = StateValueFunction(env.state_size)
     state = env.reset()
     state = ch.onehot(state, env.state_size)
     state_value = vf(state)
     ~~~
 
     """
 
     def __init__(self, state_size, init=None):
+        """
+        ## Arguments
+
+        * `state_size` (int) - The number of states in the environment.
+        * `init` (function, *optional*, default=None) - The initialization scheme for
+            the values in the table. (Default is 0.)
+        """
         super(StateValueFunction, self).__init__()
-        self.values = nn.Parameter(th.zeros((state_size, 1)))
+        self.values = nn.Parameter(torch.zeros((state_size, 1)))
         self.state_size = state_size
         if init is not None:
-            if isinstance(init, (float, int, th.Tensor)):
+            if isinstance(init, (float, int, torch.Tensor)):
                 self.values.data.add_(init)
             else:
                 init(self.values)
 
     def forward(self, state):
+        """
+        ## Description
+
+        Returns the state value of a one-hot encoded state.
+
+        ## Arguments
+
+        * `state` (Tensor) - State to be evaluated.
+        """
         return state.view(-1, self.state_size) @ self.values
 
 
-class ActionValueFunction(nn.Module):
+class ActionValueFunction(cherry.nn.ActionValue):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/tabular.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/tabular.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Stores a table of action values, Q(s, a), one for each
     (state, action) pair.
 
     Assumes that the states and actions are one-hot encoded.
     Also, the returned values are differentiable and can be used in
     conjunction with PyTorch's optimizers.
 
-    **Arguments**
+    ## References
 
-    * **state_size** (int) - The number of states in the environment.
-    * **action_size** (int) - The number of actions per state.
-    * **init** (function, *optional*, default=None) - The initialization
-      scheme for the values in the table. (Default is 0.)
+    1. Richard Sutton and Andrew Barto. 2018. Reinforcement Learning, Second Edition. The MIT Press.
 
-    **References**
+    ## Example
 
-    1. Sutton, Richard, and Andrew Barto. 2018. Reinforcement Learning, Second Edition. The MIT Press.
-
-    **Example**
     ~~~python
     qf = ActionValueFunction(env.state_size, env.action_size)
     state = env.reset()
     state = ch.onehot(state, env.state_size)
     all_action_values = qf(state)
     action = ch.onehot(0, env.action_size)
     action_value = qf(state, action)
     ~~~
 
     """
 
     def __init__(self, state_size, action_size, init=None):
+        """
+        ## Arguments
+
+        * `state_size` (int) - The number of states in the environment.
+        * `action_size` (int) - The number of actions per state.
+        * `init` (function, *optional*, default=None) - The initialization scheme for the values in the table. (Default is 0.)
+        """
         super(ActionValueFunction, self).__init__()
-        self.values = nn.Parameter(th.zeros((state_size, action_size),
-                                            requires_grad=True))
+        self.values = nn.Parameter(torch.zeros((state_size, action_size),
+                                   requires_grad=True))
         self.state_size = state_size
         self.action_size = action_size
         if init is not None:
-            if isinstance(init, (float, int, th.Tensor)):
+            if isinstance(init, (float, int, torch.Tensor)):
                 self.values.data.add_(init)
             else:
                 init(self.values)
 
     def forward(self, state, action=None):
+        """
+        ## Description
+
+        Returns the action value of a one-hot encoded state and one-hot encoded action.
+
+        ## Arguments
+
+        * `state` (Tensor) - State to be evaluated.
+        * `action` (Tensor) - Action to be evaluated.
+        """
         action_values = (state @ self.values).view(-1, self.action_size)
         if action is None:
             return action_values
-        return th.sum(action * action_values, dim=1, keepdim=True)
+        return torch.sum(action * action_values, dim=1, keepdim=True)
```

### Comparing `cherry-rl-0.1.4/cherry/models/utils.py` & `cherry-rl-0.2.0/cherry/models/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,62 +2,65 @@
 
 from torch import nn
 
 
 class RandomPolicy(nn.Module):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/utils.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/utils.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Policy that randomly samples actions from the environment action space.
 
-    **Arguments**
+    ## Example
 
-    * **env** (Environment) - Environment from which to sample actions.
-
-    **Example**
     ~~~python
     policy = ch.models.RandomPolicy(env)
     env = envs.Runner(env)
     replay = env.run(policy, steps=2048)
     ~~~
     """
 
     def __init__(self, env, *args, **kwargs):
+        """
+        ## Arguments
+
+        * `env` (Environment) - Environment from which to sample actions.
+        """
         super(RandomPolicy, self).__init__()
         self.env = env
 
     def forward(self, *args, **kwargs):
         return self.env.action_space.sample()
 
 
 def polyak_average(source, target, alpha):
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/models/utils.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/models/utils.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Shifts the parameters of source towards those of target.
 
     Note: the parameter `alpha` indicates the convex combination weight of the source.
     (i.e. the old parameters are kept at a rate of `alpha`.)
 
-    **References**
+    ## References
 
     1. Polyak, B., and A. Juditsky. 1992. “Acceleration of Stochastic Approximation by Averaging.”
 
-    **Arguments**
+    ## Arguments
+
+    * `source` (Module) - The module to be shifted.
+    * `target` (Module) - The module indicating the shift direction.
+    * `alpha` (float) - Strength of the shift.
 
-    * **source** (nn.Module) - The module to be shifted.
-    * **target** (nn.Module) - The module indicating the shift direction.
-    * **alpha** (float) - Strength of the shift.
+    ## Example
 
-    **Example**
     ~~~python
     target_qf = nn.Linear(23, 34)
     qf = nn.Linear(23, 34)
     ch.models.polyak_average(target_qf, qf, alpha=0.9)
     ~~~
     """
     for s, t in zip(source.parameters(), target.parameters()):
```

### Comparing `cherry-rl-0.1.4/cherry/nn/epsilon_greedy.py` & `cherry-rl-0.2.0/cherry/nn/epsilon_greedy.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,42 +4,43 @@
 from torch import nn
 from torch.distributions import Bernoulli, Categorical
 
 
 class EpsilonGreedy(nn.Module):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/nn/epsilon_greedy.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/nn/epsilon_greedy.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Samples actions from a uniform distribution with probability `epsilon` or
     the one maximizing the input with probability `1 - epsilon`.
 
-    **References**
+    ## References
 
     1. Sutton, Richard, and Andrew Barto. 2018. Reinforcement Learning, Second Edition. The MIT Press.
 
-    **Arguments**
-
-    * **epsilon** (float, *optional*, default=0.05) - The epsilon factor.
-    * **learnable** (bool, *optional*, default=False) - Whether the epsilon
-    factor is a learnable parameter or not.
-
-    **Example**
+    ## Example
 
     ~~~python
     egreedy = EpsilonGreedy()
     q_values = q_value(state)  # NxM tensor
     actions = egreedy(q_values)  # Nx1 tensor of longs
     ~~~
 
     """
 
     def __init__(self, epsilon=0.05, learnable=False):
+        """
+        ## Arguments
+
+        * `epsilon` (float, *optional*, default=0.05) - The epsilon factor.
+        * `learnable` (bool, *optional*, default=False) - Whether the epsilon
+        factor is a learnable parameter or not.
+        """
         super(EpsilonGreedy, self).__init__()
         msg = 'EpsilonGreedy: epsilon is not in a valid range.'
         assert epsilon >= 0.0 and epsilon <= 1.0, msg
         if learnable:
             epsilon = nn.Parameter(th.Tensor([epsilon]))
         self.epsilon = epsilon
```

### Comparing `cherry-rl-0.1.4/cherry/nn/init.py` & `cherry-rl-0.2.0/cherry/nn/init.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,77 +3,81 @@
 import torch as th
 import numpy as np
 import torch.nn as nn
 
 
 def robotics_init_(module, gain=None):
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/nn/init.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/nn/init.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Default initialization for robotic control.
 
-    **Credit**
+    ## Credit
 
     Adapted from Ilya Kostrikov's implementation, itself inspired from OpenAI Baslines.
 
-    **Arguments**
+    ## Arguments
 
-    * **module** (nn.Module) - Module to initialize.
-    * **gain** (float, *optional*, default=sqrt(2.0)) - Gain of orthogonal initialization.
+    * `module` (nn.Module) - Module to initialize.
+    * `gain` (float, *optional*, default=sqrt(2.0)) - Gain of orthogonal initialization.
 
-    **Returns**
+    ## Returns
 
     * Module, whose weight and bias have been modified in-place.
 
-    **Example**
+    ## Example
 
     ~~~python
     linear = nn.Linear(23, 5)
     kostrikov_robotics_(linear)
     ~~~
 
     """
     with th.no_grad():
         if gain is None:
             gain = np.sqrt(2.0)
-        nn.init.orthogonal_(module.weight.data, gain=gain)
-        nn.init.constant_(module.bias.data, 0.0)
+        if hasattr(module, 'weight'):
+            nn.init.orthogonal_(module.weight.data, gain=gain)
+        if hasattr(module, 'bias'):
+            nn.init.constant_(module.bias.data, 0.0)
         return module
 
 
 def atari_init_(module, gain=None):
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/nn/init.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/nn/init.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Default initialization for Atari environments.
 
-    **Credit**
+    ## Credit
 
     Adapted from Ilya Kostrikov's implementation, itself inspired from OpenAI Baslines.
 
-    **Arguments**
+    ## Arguments
 
-    * **module** (nn.Module) - Module to initialize.
-    * **gain** (float, *optional*, default=None) - Gain of orthogonal initialization.
+    * `module` (nn.Module) - Module to initialize.
+    * `gain` (float, *optional*, default=None) - Gain of orthogonal initialization.
     Default is computed for ReLU activation with `torch.nn.init.calculate_gain('relu')`.
 
-    **Returns**
+    ## Returns
 
     * Module, whose weight and bias have been modified in-place.
 
-    **Example**
+    ## Example
 
     ~~~python
     linear = nn.Linear(23, 5)
     atari_init_(linear)
     ~~~
 
     """
     if gain is None:
         gain = nn.init.calculate_gain('relu')
-    nn.init.orthogonal_(module.weight.data, gain=gain)
-    nn.init.constant_(module.bias.data, 0.0)
+    if hasattr(module, 'weight'):
+        nn.init.orthogonal_(module.weight.data, gain=gain)
+    if hasattr(module, 'bias'):
+        nn.init.constant_(module.bias.data, 0.0)
     return module
```

### Comparing `cherry-rl-0.1.4/cherry/nn/robotics_layers.py` & `cherry-rl-0.2.0/cherry/nn/robotics_layers.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 import torch.nn as nn
 import cherry as ch
 
 
 class RoboticsLinear(nn.Linear):
 
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/nn/robotics_layers.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/nn/robotics_layers.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Akin to `nn.Linear`, but with proper initialization for robotic control.
 
-    **Credit**
+    ## Credit
 
     Adapted from Ilya Kostrikov's implementation.
 
-    **Arguments**
-
-
-    * **gain** (float, *optional*) - Gain factor passed to `robotics_init_` initialization.
-    * This class extends `nn.Linear` and supports all of its arguments.
-
-    **Example**
+    ## Example
 
     ~~~python
     linear = ch.nn.Linear(23, 5, bias=True)
     action_mean = linear(state)
     ~~~
 
     """
 
     def __init__(self, *args, **kwargs):
+        """
+        ## Arguments
+
+        * `gain` (float, *optional*) - Gain factor passed to `robotics_init_` initialization.
+        * This class extends `nn.Linear` and supports all of its arguments.
+        """
         gain = kwargs.pop('gain', None)
         super(RoboticsLinear, self).__init__(*args, **kwargs)
         ch.nn.init.robotics_init_(self, gain=gain)
```

### Comparing `cherry-rl-0.1.4/cherry/optim.py` & `cherry-rl-0.2.0/cherry/optim.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,78 +3,77 @@
 """
 **Description**
 
 Optimization utilities for scalable, high-performance reinforcement learning.
 """
 
 import torch.distributed as dist
-from torch.optim.optimizer import Optimizer, required
+from torch.optim.optimizer import Optimizer
 
 
 class Distributed(Optimizer):
 
     """
 
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/optim.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/optim.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Synchronizes the gradients of a model across replicas.
 
     At every step, `Distributed` averages the gradient across all replicas
     before calling the wrapped optimizer.
     The `sync` parameters determines how frequently the parameters are
     synchronized between replicas, to minimize numerical divergences.
     This is done by calling the `sync_parameters()` method.
     If `sync is None`, this never happens except upon initialization of the
     class.
 
-    **Arguments**
-
-    * **params** (iterable) - Iterable of parameters.
-    * **opt** (Optimizer) - The optimizer to wrap and synchronize.
-    * **sync** (int, *optional*, default=None) - Parameter
-      synchronization frequency.
-
-    **References**
+    ## References
 
     1. Zinkevich et al. 2010. “Parallelized Stochastic Gradient Descent.”
 
-    **Example**
+    ## Example
 
     ~~~python
     opt = optim.Adam(model.parameters())
     opt = Distributed(model.parameters(), opt, sync=1)
 
     opt.step()
     opt.sync_parameters()
     ~~~
 
     """
 
     def __init__(self, params, opt, sync=None):
+        """
+        ## Arguments
+
+        * `params` (iterable) - Iterable of parameters.
+        * `opt` (Optimizer) - The optimizer to wrap and synchronize.
+        * `sync` (int, *optional*, default=None) - Parameter synchronization frequency.
+        """
         self.world_size = dist.get_world_size()
         self.rank = dist.get_rank()
         self.opt = opt
         self.sync = sync
         self.iter = 0
         defaults = {}
         super(Distributed, self).__init__(params, defaults)
         self.sync_parameters()
 
     def sync_parameters(self, root=0):
         """
-        **Description**
+        ## Description
 
         Broadcasts all parameters of root to all other replicas.
 
-        **Arguments**
-
-        * **root** (int, *optional*, default=0) - Rank of root replica.
+        ## Arguments
 
+        * `root` (int, *optional*, default=0) - Rank of root replica.
         """
         if self.world_size > 1:
             for group in self.param_groups:
                 for p in group['params']:
                     dist.broadcast(p.data, src=root)
 
     def step(self):
```

### Comparing `cherry-rl-0.1.4/cherry/pg.py` & `cherry-rl-0.2.0/cherry/pg.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,46 +8,49 @@
 
 import torch as th
 import cherry as ch
 
 from cherry._utils import _reshape_helper
 
 
-def generalized_advantage(gamma,
-                          tau,
-                          rewards,
-                          dones,
-                          values,
-                          next_value):
+def generalized_advantage(
+    gamma,
+    tau,
+    rewards,
+    dones,
+    values,
+    next_value,
+):
     """
-    **Description**
+    ## Description
 
     Computes the generalized advantage estimator. (GAE)
 
-    **References**
+    ## References
 
     1. Schulman et al. 2015. “High-Dimensional Continuous Control Using Generalized Advantage Estimation”
     2. https://github.com/joschu/modular_rl/blob/master/modular_rl/core.py#L49
 
-    **Arguments**
+    ## Arguments
 
-    * **gamma** (float) - Discount factor.
-    * **tau** (float) - Bias-variance trade-off.
-    * **rewards** (tensor) - Tensor of rewards.
-    * **dones** (tensor) - Tensor indicating episode termination.
+    * `gamma` (float) - Discount factor.
+    * `tau` (float) - Bias-variance trade-off.
+    * `rewards` (tensor) - Tensor of rewards.
+    * `dones` (tensor) - Tensor indicating episode termination.
       Entry is 1 if the transition led to a terminal (absorbing) state, 0 else.
-    * **values** (tensor) - Values for the states producing the rewards.
-    * **next_value** (tensor) - Value of the state obtained after the
+    * `values` (tensor) - Values for the states producing the rewards.
+    * `next_value` (tensor) - Value of the state obtained after the
       transition from the state used to compute the last value in `values`.
 
-    **Returns**
+    ## Returns
 
     * tensor - Tensor of advantages.
 
-    **Example**
+    ## Example
+
     ~~~python
     mass, next_value = policy(replay[-1].next_state)
     advantages = generalized_advantage(0.99,
                                        0.95,
                                        replay.reward(),
                                        replay.value(),
                                        replay.done(),
@@ -55,14 +58,15 @@
     ~~~
     """
 
     rewards = _reshape_helper(rewards)
     dones = _reshape_helper(dones)
     values = _reshape_helper(values)
     next_value = _reshape_helper(next_value)
+    next_value = ch.totensor(next_value).reshape_as(values[0].unsqueeze(0))
 
     msg = 'rewards, values, and dones must have equal length.'
     assert len(values) == len(rewards) == len(dones), msg
 
     next_values = th.cat((values[1:], next_value), dim=0)
     td_errors = ch.temporal_difference(gamma, rewards, dones, values, next_values)
     advantages = ch.discount(tau * gamma, td_errors, dones)
```

### Comparing `cherry-rl-0.1.4/cherry/plot.py` & `cherry-rl-0.2.0/cherry/plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,30 +10,31 @@
 import torch as th
 import numpy as np
 from statistics import mean, stdev
 
 
 def ci95(values):
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/plot.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/plot.py" class="source-link">[Source]</a>
 
-    **Description**
+    ## Description
 
     Computes the 95% confidence interval around the given values.
 
-    **Arguments**
+    ## Arguments
 
-    * **values** (list) - List of values for which to compute the
+    * `values` (list) - List of values for which to compute the
       95% confidence interval.
 
-    **Returns**
+    ## Returns
 
-    * **(float, float)** The lower and upper bounds of the confidence interval.
+    * `(float, float)` The lower and upper bounds of the confidence interval.
+
+    ## Example
 
-    **Example**
     ~~~python
     from statistics import mean
     smoothed = []
     for replay in replays:
         rewards = replay.rewards.view(-1).tolist()
         y_smoothed = ch.plot.smooth(rewards)
         smoothed.append(y_smoothed)
@@ -42,128 +43,128 @@
     lower_bound = [conf[0] for conf in confidences]
     upper_bound = [conf[1] for conf in confidences]
     ~~~
     """
     mu = mean(values)
     sigma = stdev(values, xbar=mu)
     N = len(values)
-    bound = 2.0 * sigma / math.sqrt(N)
+    bound = 1.96 * sigma / math.sqrt(N)
     lower = mu - bound
     upper = mu + bound
     return lower, upper
 
 
 def _one_sided_smoothing(x_before, y_before, smoothing_temperature=1.0):
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/plot.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/plot.py" class="source-link">[Source]</a>
 
-    **Decription**
+    ## Decription
 
     One side (regular) exponential moving average for smoothing a curve
 
     It evenly resamples points baesd on x-axis and then averages y values with
     weighting factor decreasing exponentially.
 
-    **Arguments**
+    ## Credit
 
-    * **x_before** (ndarray) - x values. Required to be in accending order.
-    * **y_before** (ndarray) - y values. Required to have same size as x_before.
-    * **smoothing_temperature** (float, *optional*, default=1.0) - the number of previous
-      steps trusted. Used to calculate the decay factor.
+    Adapted from OpenAI's baselines implementation.
+
+    ## Arguments
 
-    **Return**
+    * `x_before` (ndarray) - x values. Required to be in accending order.
+    * `y_before` (ndarray) - y values. Required to have same size as x_before.
+    * `smoothing_temperature` (float, *optional*, default=1.0) - the number of previous
+      steps trusted. Used to calculate the decay factor.
 
-    * **x_after** (ndarray) - x values after resampling.
-    * **y_after** (ndarray) - y values after smoothing.
-    * **y_count** (ndarray) - decay values at each steps.
+    ## Return
 
-    **Credit**
+    * `x_after` (ndarray) - x values after resampling.
+    * `y_after` (ndarray) - y values after smoothing.
+    * `y_count` (ndarray) - decay values at each steps.
 
-    Adapted from OpenAI's baselines implementation.
+    ## Example
 
-    **Example**
     ~~~python
     from cherry.plot import _one_sided_smoothing as osmooth
     x_smoothed, y_smoothed, y_counts = osmooth(x_original,
                                                y_original,
                                                smoothing_temperature=1.0)
     ~~~
     """
 
     if x_before is None:
         x_before = np.arange(len(y_before))
 
     assert len(x_before) == len(y_before), \
         'x_before and y_before must have equal length.'
-    assert all(x_before[i] <= x_before[i+1] for i in range(len(x_before)-1)), \
+    assert all(x_before[i] <= x_before[i + 1] for i in range(len(x_before) - 1)), \
         'x_before needs to be sorted in ascending order.'
 
     # Resampling
     size = len(x_before)
     x_after = np.linspace(x_before[0], x_before[-1], size)
     y_after = np.zeros(size, dtype=float)
     y_count = np.zeros(size, dtype=float)
 
     # Weighting factor for data of previous steps
-    alpha = np.exp(-1./smoothing_temperature)
+    alpha = np.exp(-1. / smoothing_temperature)
     x_before_length = x_before[-1] - x_before[0]
     x_before_index = 0
-    decay_period = x_before_length/(size-1)*smoothing_temperature
+    decay_period = x_before_length / (size - 1) * smoothing_temperature
 
     for i in range(len(x_after)):
         # Compute current EMA value based on the value of previous time step
-        if(i != 0):
-            y_after[i] = alpha * y_after[i-1]
-            y_count[i] = alpha * y_count[i-1]
+        if not i == 0:
+            y_after[i] = alpha * y_after[i - 1]
+            y_count[i] = alpha * y_count[i - 1]
 
         # Compute current EMA value by adding weighted average of old points
         # covered by the new point
         while x_before_index < size:
             if x_after[i] >= x_before[x_before_index]:
                 difference = x_after[i] - x_before[x_before_index]
                 # Weighting factor for y value of each old points
-                beta = np.exp(-(difference/decay_period))
+                beta = np.exp(- difference / decay_period)
                 y_after[i] += y_before[x_before_index] * beta
                 y_count[i] += beta
                 x_before_index += 1
             else:
                 break
 
-    y_after = y_after/y_count
+    y_after = y_after / y_count
     return x_after, y_after, y_count
 
 
 def exponential_smoothing(x, y=None, temperature=1.0):
     """
-    [[Source]](https://github.com/seba-1511/cherry/blob/master/cherry/plot.py)
+    <a href="https://github.com/seba-1511/cherry/blob/master/cherry/plot.py" class="source-link">[Source]</a>
 
-    **Decription**
+    ## Decription
 
     Two-sided exponential moving average for smoothing a curve.
 
     It performs regular exponential moving average twice from two different
     sides and then combines the results together.
 
-    **Arguments**
+    ## Credit
 
-    * **x** (ndarray/tensor/list) - x values, in accending order.
-    * **y** (ndarray/tensor/list) - y values.
-    * **temperature** (float, *optional*, default=1.0) - The higher,
-      the smoother.
+    Adapted from OpenAI's baselines implementation.
 
-    **Return**
+    ## Arguments
 
-    * ndarray - x values after resampling.
-    * ndarray - y values after smoothing.
+    * `x` (ndarray/tensor/list) - x values, in accending order.
+    * `y` (ndarray/tensor/list) - y values.
+    * `temperature` (float, *optional*, default=1.0) - The higher, the smoother.
 
-    **Credit**
+    ## Return
 
-    Adapted from OpenAI's baselines implementation.
+    * x_smoothed (ndarray) - x values after resampling.
+    * y_smoothed (ndarray) - y values after smoothing.
 
-    **Example**
+    ## Example
 
     ~~~python
     from cherry.plot import exponential_smoothing
     x_smoothed, y_smoothed, _ = exponential_smoothing(x_original,
                                                       y_original,
                                                       temperature=3.)
     ~~~
```

### Comparing `cherry-rl-0.1.4/cherry/td.py` & `cherry-rl-0.2.0/cherry/td.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,103 +3,108 @@
 """
 **Description**
 
 Utilities to implement temporal difference algorithms.
 """
 
 import torch as th
+import cherry as ch
 
 from cherry._utils import _reshape_helper
 
 
 def discount(gamma, rewards, dones, bootstrap=0.0):
     """
-    **Description**
+    ## Description
 
     Discounts rewards at an rate of gamma.
 
-    **References**
+    ## References
 
     1. Sutton, Richard, and Andrew Barto. 2018. Reinforcement Learning, Second Edition. The MIT Press.
 
-    **Arguments**
+    ## Arguments
 
-    * **gamma** (float) - Discount factor.
-    * **rewards** (tensor) - Tensor of rewards.
-    * **dones** (tensor) - Tensor indicating episode termination.
+    * `gamma` (float) - Discount factor.
+    * `rewards` (tensor) - Tensor of rewards.
+    * `dones` (tensor) - Tensor indicating episode termination.
       Entry is 1 if the transition led to a terminal (absorbing) state, 0 else.
-    * **bootstrap** (float, *optional*, default=0.0) - Bootstrap the last
+    * `bootstrap` (float, *optional*, default=0.0) - Bootstrap the last
       reward with this value.
 
-    **Returns**
+    ## Returns
 
     * tensor - Tensor of discounted rewards.
 
-    **Example**
+    ## Example
 
     ~~~python
     rewards = th.ones(23, 1) * 8
     dones = th.zeros_like(rewards)
     dones[-1] += 1.0
     discounted = ch.rl.discount(0.99,
                                 rewards,
                                 dones,
                                 bootstrap=1.0)
     ~~~
 
     """
     rewards = _reshape_helper(rewards)
-    dones = _reshape_helper(dones)
+    dones = _reshape_helper(dones).reshape_as(rewards)
 
     msg = 'dones and rewards must have equal length.'
     assert rewards.size(0) == dones.size(0), msg
+
+    if not isinstance(bootstrap, (int, float)):
+        bootstrap = ch.totensor(bootstrap).reshape_as(rewards[0].unsqueeze(0))
+
     R = th.zeros_like(rewards) + bootstrap
     discounted = th.zeros_like(rewards)
     length = discounted.size(0)
     for t in reversed(range(length)):
         R = R * (1.0 - dones[t])
         R = rewards[t] + gamma * R
         discounted[t] += R[0]
     return discounted
 
 
 def temporal_difference(gamma, rewards, dones, values, next_values):
     """
-    **Description**
+    ## Description
 
     Returns the temporal difference residual.
 
-    **Reference**
+    ## Reference
 
     1. Sutton, Richard S. 1988. “Learning to Predict by the Methods of Temporal Differences.” Machine Learning 3 (1): 9–44.
     2. Sutton, Richard, and Andrew Barto. 2018. Reinforcement Learning, Second Edition. The MIT Press.
 
-    **Arguments**
+    ## Arguments
 
-    * **gamma** (float) - Discount factor.
-    * **rewards** (tensor) - Tensor of rewards.
-    * **dones** (tensor) - Tensor indicating episode termination.
+    * `gamma` (float) - Discount factor.
+    * `rewards` (tensor) - Tensor of rewards.
+    * `dones` (tensor) - Tensor indicating episode termination.
       Entry is 1 if the transition led to a terminal (absorbing) state, 0 else.
-    * **values** (tensor) - Values for the states producing the rewards.
-    * **next_values** (tensor) - Values of the state obtained after the
+    * `values` (tensor) - Values for the states producing the rewards.
+    * `next_values` (tensor) - Values of the state obtained after the
       transition from the state used to compute the last value in `values`.
 
-    **Example**
+    ## Example
 
     ~~~python
     values = vf(replay.states())
     next_values = vf(replay.next_states())
     td_errors = temporal_difference(0.99,
                                     replay.reward(),
                                     replay.done(),
                                     values,
                                     next_values)
     ~~~
     """
 
-    rewards = _reshape_helper(rewards)
-    dones = _reshape_helper(dones)
     values = _reshape_helper(values)
     next_values = _reshape_helper(next_values)
+    rewards = _reshape_helper(rewards).reshape_as(values)
+    dones = _reshape_helper(dones).reshape_as(values)
 
     not_dones = 1.0 - dones
     return rewards + gamma * not_dones * next_values - values
```

### Comparing `cherry-rl-0.1.4/setup.py` & `cherry-rl-0.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python3
 
+from encodings import utf_8
 import re
 from setuptools import (
-        setup,
-        find_packages,
-        )
+    setup,
+    find_packages,
+)
 
 # Parses version number: https://stackoverflow.com/a/7071358
 VERSIONFILE = 'cherry/_version.py'
 verstrline = open(VERSIONFILE, "rt").read()
 VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
 mo = re.search(VSRE, verstrline, re.M)
 if mo:
@@ -18,22 +19,23 @@
 
 # Installs the package
 setup(
     name='cherry-rl',
     packages=find_packages(),
     version=VERSION,
     description='PyTorch Reinforcement Learning Framework for Researchers',
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding='UTF-8').read(),
     long_description_content_type='text/markdown',
     author='Seb Arnold',
     author_email='smr.arnold@gmail.com',
     url='https://learnables.github.com/cherry',
     download_url='https://github.com/learnables/cherry/archive/' + str(VERSION) + '.zip',
     license='License :: OSI Approved :: Apache Software License',
     classifiers=[],
     scripts=[],
     install_requires=[
         'numpy>=1.15.4',
         'gym>=0.10.9',
         'torch>=1.0.0',
+        'dotmap',
     ],
 )
```

