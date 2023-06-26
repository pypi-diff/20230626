# Comparing `tmp/ci-buildbot-0.7.3.tar.gz` & `tmp/ci-buildbot-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ci-buildbot-0.7.3.tar", last modified: Tue May 18 21:13:22 2021, max compression
+gzip compressed data, was "dist/ci-buildbot-0.9.0.tar", last modified: Mon Jun 26 17:24:19 2023, max compression
```

## Comparing `ci-buildbot-0.7.3.tar` & `ci-buildbot-0.9.0.tar`

### file list

```diff
@@ -1,47 +1,63 @@
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/
--rw-rw-r--   0 cmalek     (501) staff       (20)      100 2020-06-03 23:17:09.000000 ci-buildbot-0.7.3/MANIFEST.in
--rw-rw-r--   0 cmalek     (501) staff       (20)     3117 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/PKG-INFO
--rw-rw-r--   0 cmalek     (501) staff       (20)     2245 2020-09-15 21:46:06.000000 ci-buildbot-0.7.3/README.md
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot/
--rw-rw-r--   0 cmalek     (501) staff       (20)       22 2021-05-18 21:13:15.000000 ci-buildbot-0.7.3/ci_buildbot/__init__.py
--rw-rw-r--   0 cmalek     (501) staff       (20)    10822 2021-01-07 22:49:36.000000 ci-buildbot-0.7.3/ci_buildbot/cli.py
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot/messages/
--rw-rw-r--   0 cmalek     (501) staff       (20)      648 2021-01-07 00:08:07.000000 ci-buildbot-0.7.3/ci_buildbot/messages/__init__.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      245 2020-08-20 23:57:23.000000 ci-buildbot-0.7.3/ci_buildbot/messages/archive.py
--rw-rw-r--   0 cmalek     (501) staff       (20)        0 2020-06-03 18:15:32.000000 ci-buildbot-0.7.3/ci_buildbot/messages/base.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      570 2020-08-20 23:56:31.000000 ci-buildbot-0.7.3/ci_buildbot/messages/deployfish.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      623 2020-08-20 23:56:26.000000 ci-buildbot-0.7.3/ci_buildbot/messages/deployfish_tasks.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      566 2020-08-20 23:56:35.000000 ci-buildbot-0.7.3/ci_buildbot/messages/docker.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      894 2020-09-15 21:58:07.000000 ci-buildbot-0.7.3/ci_buildbot/messages/general.py
--rw-rw-r--   0 cmalek     (501) staff       (20)    14360 2021-05-18 21:12:43.000000 ci-buildbot-0.7.3/ci_buildbot/messages/mixins.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      545 2021-01-07 23:13:40.000000 ci-buildbot-0.7.3/ci_buildbot/messages/unittests.py
--rw-rw-r--   0 cmalek     (501) staff       (20)      850 2020-06-03 18:32:58.000000 ci-buildbot-0.7.3/ci_buildbot/settings.py
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot/templates/
--rw-rw-r--   0 cmalek     (501) staff       (20)      949 2020-06-04 00:25:48.000000 ci-buildbot-0.7.3/ci_buildbot/templates/archive.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      653 2020-07-15 23:30:13.000000 ci-buildbot-0.7.3/ci_buildbot/templates/deploy_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      609 2020-06-04 00:52:42.000000 ci-buildbot-0.7.3/ci_buildbot/templates/deploy_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      656 2020-07-15 23:30:01.000000 ci-buildbot-0.7.3/ci_buildbot/templates/deploy_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      672 2020-07-16 17:06:32.000000 ci-buildbot-0.7.3/ci_buildbot/templates/deploy_tasks_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      636 2020-07-16 17:06:29.000000 ci-buildbot-0.7.3/ci_buildbot/templates/deploy_tasks_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      673 2020-07-16 17:06:23.000000 ci-buildbot-0.7.3/ci_buildbot/templates/deploy_tasks_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      674 2020-07-15 23:31:55.000000 ci-buildbot-0.7.3/ci_buildbot/templates/docker_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      635 2020-07-15 23:32:00.000000 ci-buildbot-0.7.3/ci_buildbot/templates/docker_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      726 2020-07-15 23:30:24.000000 ci-buildbot-0.7.3/ci_buildbot/templates/docker_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      626 2020-09-16 20:45:40.000000 ci-buildbot-0.7.3/ci_buildbot/templates/general_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      592 2020-09-15 21:58:53.000000 ci-buildbot-0.7.3/ci_buildbot/templates/general_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      627 2020-09-15 21:59:06.000000 ci-buildbot-0.7.3/ci_buildbot/templates/general_success.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      667 2021-01-07 23:14:54.000000 ci-buildbot-0.7.3/ci_buildbot/templates/unittests_failed.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      597 2021-01-07 00:11:19.000000 ci-buildbot-0.7.3/ci_buildbot/templates/unittests_start.tpl
--rw-rw-r--   0 cmalek     (501) staff       (20)      669 2021-01-07 23:15:01.000000 ci-buildbot-0.7.3/ci_buildbot/templates/unittests_success.tpl
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot.egg-info/
--rw-rw-r--   0 cmalek     (501) staff       (20)     3117 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot.egg-info/PKG-INFO
--rw-rw-r--   0 cmalek     (501) staff       (20)     1318 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot.egg-info/SOURCES.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)        1 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot.egg-info/dependency_links.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)       51 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot.egg-info/entry_points.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)      133 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot.egg-info/requires.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)       12 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/ci_buildbot.egg-info/top_level.txt
-drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/etc/
--rw-rw-r--   0 cmalek     (501) staff       (20)      313 2020-06-03 21:28:58.000000 ci-buildbot-0.7.3/etc/environment.txt
--rw-rw-r--   0 cmalek     (501) staff       (20)     2647 2020-07-23 19:08:48.000000 ci-buildbot-0.7.3/requirements.txt
--rw-r--r--   0 cmalek     (501) staff       (20)      301 2021-05-18 21:13:22.000000 ci-buildbot-0.7.3/setup.cfg
--rw-rw-r--   0 cmalek     (501) staff       (20)     1020 2021-05-18 21:13:15.000000 ci-buildbot-0.7.3/setup.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      100 2020-06-03 23:17:09.000000 ci-buildbot-0.9.0/MANIFEST.in
+-rw-rw-r--   0 cmalek     (501) staff       (20)     3588 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) staff       (20)     2660 2022-08-12 23:28:44.000000 ci-buildbot-0.9.0/README.md
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot/
+-rw-rw-r--   0 cmalek     (501) staff       (20)       22 2023-06-26 17:23:45.000000 ci-buildbot-0.9.0/ci_buildbot/__init__.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)    12633 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/cli.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      366 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/__init__.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      564 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/base.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     3092 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/codebuild.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      881 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/deployfish.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1144 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/docker.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      489 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/generic.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     9516 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/git.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1773 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/project.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      617 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/sphinx.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1477 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/context_processors/unittest.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      116 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/exc.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot/messages/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      833 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/__init__.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      467 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/archive.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     2007 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/base.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1116 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/deployfish.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1165 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/deployfish_tasks.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1109 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/docker.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1008 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/docs.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      798 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/general.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      817 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/messages/unittests.py
+-rw-rw-r--   0 cmalek     (501) staff       (20)      834 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/settings.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot/templates/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      949 2020-06-04 00:25:48.000000 ci-buildbot-0.9.0/ci_buildbot/templates/archive.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      653 2020-07-15 23:30:13.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      609 2020-06-04 00:52:42.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      656 2020-07-15 23:30:01.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      672 2020-07-16 17:06:32.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      636 2020-07-16 17:06:29.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      673 2020-07-16 17:06:23.000000 ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      674 2020-07-15 23:31:55.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docker_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      635 2020-07-15 23:32:00.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docker_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      726 2020-07-15 23:30:24.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docker_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      623 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docs_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      584 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docs_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      649 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/docs_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      627 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/general_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      592 2020-09-15 21:58:53.000000 ci-buildbot-0.9.0/ci_buildbot/templates/general_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      628 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/templates/general_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      667 2021-01-07 23:14:54.000000 ci-buildbot-0.9.0/ci_buildbot/templates/unittests_failed.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      597 2021-01-07 00:11:19.000000 ci-buildbot-0.9.0/ci_buildbot/templates/unittests_start.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)      669 2021-01-07 23:15:01.000000 ci-buildbot-0.9.0/ci_buildbot/templates/unittests_success.tpl
+-rw-rw-r--   0 cmalek     (501) staff       (20)       63 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/ci_buildbot/typedefs.py
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/
+-rw-rw-r--   0 cmalek     (501) staff       (20)     3588 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/PKG-INFO
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1891 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)        1 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)       51 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/entry_points.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)      135 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/requires.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)       12 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/ci_buildbot.egg-info/top_level.txt
+drwxrwxr-x   0 cmalek     (501) staff       (20)        0 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/etc/
+-rw-rw-r--   0 cmalek     (501) staff       (20)      313 2020-06-03 21:28:58.000000 ci-buildbot-0.9.0/etc/environment.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)     2275 2023-06-26 17:23:34.000000 ci-buildbot-0.9.0/requirements.txt
+-rw-rw-r--   0 cmalek     (501) staff       (20)      986 2023-06-26 17:24:19.000000 ci-buildbot-0.9.0/setup.cfg
+-rw-rw-r--   0 cmalek     (501) staff       (20)     1040 2023-06-26 17:23:45.000000 ci-buildbot-0.9.0/setup.py
```

### Comparing `ci-buildbot-0.7.3/README.md` & `ci-buildbot-0.9.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,57 @@
 # ci-buildbot
 
 `ci-buildbot` is a command line tool to do slack messaging from CodePipelines.  `ci-buildbot` acts as a Slack App in
 order to do its work.
 
 To install:
 
-```
-pyenv virtualenv 3.6.5 ci-buildbot
+```bash
+pyenv virtualenv 3.8.5 ci-buildbot
 pyenv local ci-buildbot
 pip install -r requirements.txt
 pip install -e .
 ```
 
 Now set up the environment:
 
-```
+```bash
 cp etc/environment.text .env
 ```
 
-You'll need to know two things: 
+You'll need to know two things:
 
 * `SLACK_API_TOKEN`: this your Slack app's Oath token
-* `CHANNEL`: this is the channel you want `ci-buildbot` to post into.  Note that if this is a private channel, you'll
-	need to invite the `ci-buildbot` app into that channel before you'll see any messages.
+* `CHANNEL`: this is the channel you want `ci-buildbot` to post into.  Note that if this is a private channel, you'll need to invite the `ci-buildbot` app into that channel before you'll see any messages.
 
 Now you can run the main command, `buildbot`:
 
-```
+```bash
 buildbot --help
 ```
 
-# Icons
+## Icons
 
 I get the icons for the Slack messages here: https://iconmonstr.com.
 
-For the gray icons, I use #909090
-For the green icons, I use #0D6B19
-For the red icons, I use #801B0B
+Get them as .pngs, 64x64px, name them appropriately to the build steps they're going to be used in, and save them to `./icons/`
 
-# Testing: CodeBuild environment variables
+For the gray icons (`foo-start.png`), use #909090 as the icon color.
+For the green icons (`foo-success.png`), use #0D6B19 as the icon color.
+For the red icons (`foo-failure.png`), use #801B0B as the icon color.
 
+`ci-buildbot` tells slack to retrieve the icons from an S3 bucket: ads-utils-icons.s3.amanzonaws.com.  Do this to sync `./icons` to S3:
+
+```bash
+make icons
 ```
+
+## Testing: CodeBuild environment variables
+
+```bash
 export CODEBUILD_START_TIME=1594856732.3577878
 export CODEBUILD_VPC_AZ=us-west-2b
 export CODEBUILD_LAST_EXIT=0
 export CODEBUILD_START_TIME=1538752095466
 export CODEBUILD_BMR_URL=https://CODEBUILD_AGENT:3000
 export CODEBUILD_SOURCE_VERSION=arn:aws:s3:::bucket/pipeline/App/OGgJCVJ.zip
 export CODEBUILD_KMS_KEY_ID=arn:aws:kms:us-west-2:000000011111:alias/aws/s3
```

### Comparing `ci-buildbot-0.7.3/ci_buildbot/cli.py` & `ci-buildbot-0.9.0/ci_buildbot/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 import ci_buildbot
 from .settings import Settings
 from .messages import (
     ArchiveCodeMessage,
     DockerFailureMessage,
     DockerStartMessage,
     DockerSuccessMessage,
+    DocsFailureMessage,
+    DocsStartMessage,
+    DocsSuccessMessage,
     DeployfishDeployFailureMessage,
     DeployfishDeployStartMessage,
     DeployfishDeploySuccessMessage,
     DeployfishTasksDeployFailureMessage,
     DeployfishTasksDeployStartMessage,
     DeployfishTasksDeploySuccessMessage,
     GeneralFailureMessage,
@@ -85,18 +88,19 @@
 
 @report.group('docker', short_help="A group of commands that report about a Docker bmage build step")
 def report_docker():
     pass
 
 
 @report_docker.command('start', short_help="Report about starting a docker build")
+@click.option('--changelog/--no-changelog', default=False, help="Include the git changelog.")
 @click.argument('image')
 @click.pass_context
-def report_docker_start(ctx, image):
-    blocks = DockerStartMessage(image=image).format()
+def report_docker_start(ctx, image: str, changelog: bool):
+    blocks = DockerStartMessage().format(image=image, changelog=changelog)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -104,15 +108,15 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_docker.command('success', short_help="Report a successful docker build")
 @click.argument('image')
 @click.pass_context
 def report_docker_success(ctx, image):
-    blocks = DockerSuccessMessage(image=image).format()
+    blocks = DockerSuccessMessage().format(image=image)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -120,15 +124,15 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_docker.command('failure', short_help="Report a failed docker build")
 @click.argument('image')
 @click.pass_context
 def report_docker_failure(ctx, image):
-    blocks = DockerFailureMessage(image=image).format()
+    blocks = DockerFailureMessage().format(image=image)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -156,15 +160,15 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_unittests.command('success', short_help="Report a successful test runner build")
 @click.argument('report_group')
 @click.pass_context
 def report_unittests_success(ctx, report_group):
-    blocks = UnittestsSuccessMessage(report_group=report_group).format()
+    blocks = UnittestsSuccessMessage().format(report_group=report_group)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -172,15 +176,15 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_unittests.command('failure', short_help="Report a failed test runner build")
 @click.argument('report_group')
 @click.pass_context
 def report_unittests_failure(ctx, report_group):
-    blocks = UnittestsFailureMessage(report_group=report_group).format()
+    blocks = UnittestsFailureMessage().format(report_group=report_group)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -193,15 +197,15 @@
     pass
 
 
 @report_deployfish.command('start', short_help="Report about starting a deployfish service deploy")
 @click.argument('service')
 @click.pass_context
 def report_deployfish_start(ctx, service):
-    blocks = DeployfishDeployStartMessage(service=service).format()
+    blocks = DeployfishDeployStartMessage().format(service=service)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -209,15 +213,15 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_deployfish.command('success', short_help="Report a successful deployfish service deploy")
 @click.argument('service')
 @click.pass_context
 def report_deployfish_success(ctx, service):
-    blocks = DeployfishDeploySuccessMessage(service=service).format()
+    blocks = DeployfishDeploySuccessMessage().format(service=service)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -225,15 +229,15 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_deployfish.command('failure', short_help="Report a failed deployfish service deploy")
 @click.argument('service')
 @click.pass_context
 def report_deployfish_failure(ctx, service):
-    blocks = DeployfishDeployFailureMessage(service=service).format()
+    blocks = DeployfishDeployFailureMessage().format(service=service)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -249,15 +253,15 @@
     pass
 
 
 @report_deployfish_tasks.command('start', short_help="Report about starting a deployfish one-off tasks deploy")
 @click.argument('tasks', nargs=-1, required=True)
 @click.pass_context
 def report_deployfish_tasks_start(ctx, tasks):
-    blocks = DeployfishTasksDeployStartMessage(tasks=tasks).format()
+    blocks = DeployfishTasksDeployStartMessage().format(tasks=tasks)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -265,15 +269,15 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_deployfish_tasks.command('success', short_help="Report a successful deployfish one-off tasks deploy")
 @click.argument('tasks', nargs=-1, required=True)
 @click.pass_context
 def report_deployfish_tasks_success(ctx, tasks):
-    blocks = DeployfishTasksDeploySuccessMessage(tasks=tasks).format()
+    blocks = DeployfishTasksDeploySuccessMessage().format(tasks=tasks)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -281,15 +285,66 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_deployfish_tasks.command('failure', short_help="Report a failed deployfish one-off tasks deploy")
 @click.argument('tasks', nargs=-1, required=True)
 @click.pass_context
 def report_deployfish_tasks_failure(ctx, tasks):
-    blocks = DeployfishTasksDeployFailureMessage(tasks=tasks).format()
+    blocks = DeployfishTasksDeployFailureMessage().format(tasks=tasks)
+    client = ctx.obj['slack']
+    try:
+        client.chat_postMessage(
+            channel=ctx.obj['settings'].channel,
+            blocks=blocks,
+            as_user=True
+        )
+    except SlackApiError as e:
+        print(f"Got an error: {e.response['error']}")
+
+
+@report.group('docs', short_help="A group of commands that report about a Deployfish service build step")
+def report_docs():
+    pass
+
+
+@report_docs.command('start', short_help="Report about starting a Sphinx docs build and deploy")
+@click.pass_context
+def report_docs_start(ctx):
+    blocks = DocsStartMessage().format()
+    client = ctx.obj['slack']
+    try:
+        client.chat_postMessage(
+            channel=ctx.obj['settings'].channel,
+            blocks=blocks,
+            as_user=True
+        )
+    except SlackApiError as e:
+        print(f"Got an error: {e.response['error']}")
+
+
+@report_docs.command('success', short_help="Report a successful Sphinx docs build and deploy")
+@click.argument('url')
+@click.pass_context
+def report_docs_success(ctx, url):
+    blocks = DocsSuccessMessage().format(url=url)
+    client = ctx.obj['slack']
+    try:
+        client.chat_postMessage(
+            channel=ctx.obj['settings'].channel,
+            blocks=blocks,
+            as_user=True
+        )
+    except SlackApiError as e:
+        print(f"Got an error: {e.response['error']}")
+
+
+@report_docs.command('failure', short_help="Report a failed Sphinx docs build and deploy")
+@click.pass_context
+def report_docs_failure(ctx):
+    blocks = DocsFailureMessage().format()
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -302,15 +357,15 @@
     pass
 
 
 @report_general.command('start', short_help="Report about starting a general service deploy")
 @click.argument('label')
 @click.pass_context
 def report_general_start(ctx, label):
-    blocks = GeneralStartMessage(label=label).format()
+    blocks = GeneralStartMessage().format(label=label)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -318,15 +373,15 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_general.command('success', short_help="Report a successful general service deploy")
 @click.argument('label')
 @click.pass_context
 def report_general_success(ctx, label):
-    blocks = GeneralSuccessMessage(label=label).format()
+    blocks = GeneralSuccessMessage().format(label=label)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
@@ -334,25 +389,25 @@
         print(f"Got an error: {e.response['error']}")
 
 
 @report_general.command('failure', short_help="Report a failed general service deploy")
 @click.argument('label')
 @click.pass_context
 def report_general_failure(ctx, label):
-    blocks = GeneralFailureMessage(label=label).format()
+    blocks = GeneralFailureMessage().format(label=label)
     client = ctx.obj['slack']
     try:
         client.chat_postMessage(
             channel=ctx.obj['settings'].channel,
             blocks=blocks,
             as_user=True
         )
     except SlackApiError as e:
         print(f"Got an error: {e.response['error']}")
 
 
 def main():
-    cli(obj={})
+    cli(obj={})  # pylint: disable=no-value-for-parameter,unexpected-keyword-arg
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `ci-buildbot-0.7.3/ci_buildbot/messages/__init__.py` & `ci-buildbot-0.9.0/ci_buildbot/messages/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-from .archive import (
+from .archive import (  # noqa: F401
     ArchiveCodeMessage
 )
-from .docker import (
+from .docker import (  # noqa: F401
     DockerFailureMessage,
     DockerSuccessMessage,
     DockerStartMessage
 )
-from .deployfish import (
+from .docs import (  # noqa: F401
+    DocsFailureMessage,
+    DocsSuccessMessage,
+    DocsStartMessage
+)
+from .deployfish import (  # noqa:F401
     DeployfishDeployFailureMessage,
     DeployfishDeploySuccessMessage,
     DeployfishDeployStartMessage
 )
-from .deployfish_tasks import (
+from .deployfish_tasks import (  # noqa:F401
     DeployfishTasksDeployFailureMessage,
     DeployfishTasksDeploySuccessMessage,
     DeployfishTasksDeployStartMessage
 )
-from .general import (
+from .general import (  # noqa:F401
     GeneralFailureMessage,
     GeneralSuccessMessage,
     GeneralStartMessage
 )
-from .unittests import (
+from .unittests import (  # noqa:F401
     UnittestsFailureMessage,
     UnittestsSuccessMessage,
     UnittestsStartMessage
 )
```

### Comparing `ci-buildbot-0.7.3/ci_buildbot/settings.py` & `ci-buildbot-0.9.0/ci_buildbot/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pathlib import Path  # python3 only
-#from typing import Union, List, Dict
+from pathlib import Path
+from typing import Optional
 
 from jinja2 import FileSystemLoader, Environment
 from pydantic import BaseSettings
 
 
 templates_path = Path(__file__).parent / 'templates'
 jinja_env = Environment(
@@ -11,15 +11,15 @@
 )
 
 
 class Settings(BaseSettings):
     """
     See https://pydantic-docs.helpmanual.io/#settings for details on using and overriding this.
     """
-    api_token: str = None
+    api_token: Optional[str] = None
 
     debug: bool = False
 
     channel: str = "jenkins"
 
     statsd_host: str = 'scope.cloud.caltech.edu'
     statsd_port: int = 8125
```

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/archive.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/archive.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/deploy_failed.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/deploy_start.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/deploy_success.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/deploy_tasks_failed.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/deploy_tasks_start.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/deploy_tasks_success.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/deploy_tasks_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/docker_failed.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/docker_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/docker_start.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/docker_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/docker_success.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/docker_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/general_failed.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/general_failed.tpl`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {'1': "{'text': {'text': '*{{ last_version_url }}*: {{ label }} *FAILED*\\n*Pipeline*: {{ "*

 * *      "pipeline_url }}\\n*Build log*: {{ build_status_url }}\\n*Elapsed time*: {{ build_time }}'}}"}*

```diff
@@ -5,15 +5,15 @@
     {
         "accessory": {
             "alt_text": "General build step failed",
             "image_url": "https://ads-utils-icons.s3-us-west-2.amazonaws.com/ci-buildbot/general-failure.png",
             "type": "image"
         },
         "text": {
-            "text": "*{{ last_version_url }}*: {{ label }}*FAILED*\n*Pipeline*: {{ pipeline_url }}\n*Build log*: {{ build_status_url }}\n*Elapsed time*: {{ build_time }}",
+            "text": "*{{ last_version_url }}*: {{ label }} *FAILED*\n*Pipeline*: {{ pipeline_url }}\n*Build log*: {{ build_status_url }}\n*Elapsed time*: {{ build_time }}",
             "type": "mrkdwn"
         },
         "type": "section"
     },
     {
         "elements": [
             {
```

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/general_start.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/general_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/general_success.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/general_success.tpl`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9861111111111112%*

 * *Differences: {'1': "{'text': {'text': '*{{ last_version_url }}*: {{ label }} *SUCCESS*\\n*Pipeline*: "*

 * *      '{{pipeline_url}}\\nBuild log*: {{ build_status_url }}\\n*Elapsed time*: {{ build_time '*

 * *      "}}\\n'}}"}*

```diff
@@ -5,15 +5,15 @@
     {
         "accessory": {
             "alt_text": "General build step success",
             "image_url": "https://ads-utils-icons.s3-us-west-2.amazonaws.com/ci-buildbot/general-success.png",
             "type": "image"
         },
         "text": {
-            "text": "*{{ last_version_url }}*: {{ label }}*SUCCESS*\n*Pipeline*: {{pipeline_url}}\nBuild log*: {{ build_status_url }}\n*Elapsed time*: {{ build_time }}\n",
+            "text": "*{{ last_version_url }}*: {{ label }} *SUCCESS*\n*Pipeline*: {{pipeline_url}}\nBuild log*: {{ build_status_url }}\n*Elapsed time*: {{ build_time }}\n",
             "type": "mrkdwn"
         },
         "type": "section"
     },
     {
         "elements": [
             {
```

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/unittests_failed.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/unittests_failed.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/unittests_start.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/unittests_start.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot/templates/unittests_success.tpl` & `ci-buildbot-0.9.0/ci_buildbot/templates/unittests_success.tpl`

 * *Files identical despite different names*

### Comparing `ci-buildbot-0.7.3/ci_buildbot.egg-info/SOURCES.txt` & `ci-buildbot-0.9.0/ci_buildbot.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,55 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 ci_buildbot/__init__.py
 ci_buildbot/cli.py
+ci_buildbot/exc.py
 ci_buildbot/settings.py
+ci_buildbot/typedefs.py
 ci_buildbot.egg-info/PKG-INFO
 ci_buildbot.egg-info/SOURCES.txt
 ci_buildbot.egg-info/dependency_links.txt
 ci_buildbot.egg-info/entry_points.txt
 ci_buildbot.egg-info/requires.txt
 ci_buildbot.egg-info/top_level.txt
+ci_buildbot/context_processors/__init__.py
+ci_buildbot/context_processors/base.py
+ci_buildbot/context_processors/codebuild.py
+ci_buildbot/context_processors/deployfish.py
+ci_buildbot/context_processors/docker.py
+ci_buildbot/context_processors/generic.py
+ci_buildbot/context_processors/git.py
+ci_buildbot/context_processors/project.py
+ci_buildbot/context_processors/sphinx.py
+ci_buildbot/context_processors/unittest.py
 ci_buildbot/messages/__init__.py
 ci_buildbot/messages/archive.py
 ci_buildbot/messages/base.py
 ci_buildbot/messages/deployfish.py
 ci_buildbot/messages/deployfish_tasks.py
 ci_buildbot/messages/docker.py
+ci_buildbot/messages/docs.py
 ci_buildbot/messages/general.py
-ci_buildbot/messages/mixins.py
 ci_buildbot/messages/unittests.py
 ci_buildbot/templates/archive.tpl
 ci_buildbot/templates/deploy_failed.tpl
 ci_buildbot/templates/deploy_start.tpl
 ci_buildbot/templates/deploy_success.tpl
 ci_buildbot/templates/deploy_tasks_failed.tpl
 ci_buildbot/templates/deploy_tasks_start.tpl
 ci_buildbot/templates/deploy_tasks_success.tpl
 ci_buildbot/templates/docker_failed.tpl
 ci_buildbot/templates/docker_start.tpl
 ci_buildbot/templates/docker_success.tpl
+ci_buildbot/templates/docs_failed.tpl
+ci_buildbot/templates/docs_start.tpl
+ci_buildbot/templates/docs_success.tpl
 ci_buildbot/templates/general_failed.tpl
 ci_buildbot/templates/general_start.tpl
 ci_buildbot/templates/general_success.tpl
 ci_buildbot/templates/unittests_failed.tpl
 ci_buildbot/templates/unittests_start.tpl
 ci_buildbot/templates/unittests_success.tpl
 etc/environment.txt
```

### Comparing `ci-buildbot-0.7.3/requirements.txt` & `ci-buildbot-0.9.0/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 slackclient==2.5.0                            # https://github.com/slackapi/python-slackclient
 docker==4.2.1                                 # https://github.com/docker/docker-py/
 gitpython==3.1.0                              # https://github.com/gitpython-developers/GitPython
 giturlparse==0.9.2                            # https://github.com/nephila/giturlparse
 jinja2==2.11.1                                # https://github.com/pallets/jinja
-click==7.0                                    # https://github.com/pallets/click
+click>=7.0                                    # https://github.com/pallets/click
 pydantic==1.4                                 # https://github.com/samuelcolvin/pydantic
 pydantic[dotenv]==1.3
 python-dotenv==0.11.0                         # https://github.com/theskumar/python-dotenv
 sh==1.13.1                                    # https://github.com/amoffat/sh
 
 # Other utils
 # ------------------------------------------------------------------------------
 colorama==0.3.7                               # https://github.com/tartley/colorama
 pytz==2019.1                                  # https://github.com/stub42/pytz
 
 # Deployment
 # ------------------------------------------------------------------------------
-bumpversion==0.5.3                            # https://github.com/peritus/bumpversion
-Sphinx==2.0.1                                 # https://github.com/sphinx-doc/sphinx
-ipython==7.1.0                                # https://github.com/ipython/ipython
+bump2version==1.0.1                           # https://github.com/peritus/bumpversion
+ipython>=7.13.0                               # https://github.com/ipython/ipython
 twine                                         # https://github.com/pypa/twine/
 tox                                           # https://github.com/tox-dev/to
 wheel                                         # https://github.com/pypa/wheel
-# ---- Purposely unpinned ----
-awscli                                        # https://github.com/aws/aws-cli
 
 # Development
 # ------------------------------------------------------------------------------
-autopep8==1.4.4                               # https://github.com/hhatto/autopep8
-flake8==3.7.9                                 # https://github.com/PyCQA/flake8
-pycodestyle==2.5.0                            # https://github.com/PyCQA/pycodestyle
-python-language-server==0.31.4                # https://github.com/palantir/python-language-server
+autopep8                                      # https://github.com/hhatto/autopep8
+flake8                                        # https://github.com/PyCQA/flake8
+mypy                                          # https://github.com/python/mypy
+pylint
 
 # Testing
 # ------------------------------------------------------------------------------
 coverage==4.5.3                               # https://github.com/nedbat/coveragepy
-mypy==0.701                                   # https://github.com/python/mypy
 pydevd-pycharm~=192.6817.19                   # https://github.com/JetBrains/intellij-community
 testfixtures==6.10.0                          # https://github.com/Simplistix/testfixtures
```

### Comparing `ci-buildbot-0.7.3/setup.py` & `ci-buildbot-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="ci-buildbot",
-    version='0.7.3',
+    version='0.9.0',
     description="Slack client for reporting on CodePipeline runs",
     url="https://github.com/caltechads/ci-buildbot",
     author="Caltech IMSS ADS",
     author_email="imss-ads-staff@caltech.edu",
     packages=find_packages(exclude=["*.test", "*.test.*", "test.*", "test", "bin", "*.pyc"]),
     include_package_data=True,
     long_description=long_description,
@@ -22,12 +22,12 @@
     install_requires=[
         "slackclient >= 2.5.0",
         "docker >= 4.2.1",
         "gitpython >= 3.1.0",
         "giturlparse >= 0.9.2",
         "click >= 7.0",
         "jinja2 >= 2.11.1",
-        "pydantic == 1.4",
+        "pydantic >= 1.6.2",
         "pytz == 2019.1",
         "sh == 1.13.1"
     ],
 )
```

