# Comparing `tmp/acore_soap_app-0.1.1.tar.gz` & `tmp/acore_soap_app-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_soap_app-0.1.1.tar", last modified: Wed Jun 21 15:46:35 2023, max compression
+gzip compressed data, was "acore_soap_app-0.2.1.tar", last modified: Mon Jun 26 04:09:41 2023, max compression
```

## Comparing `acore_soap_app-0.1.1.tar` & `acore_soap_app-0.2.1.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.041356 acore_soap_app-0.1.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5307 2023-06-21 15:46:35.041193 acore_soap_app-0.1.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4168 2023-06-21 15:43:46.000000 acore_soap_app-0.1.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.035238 acore_soap_app-0.1.1/acore_soap_app/
--rw-r--r--   0 sanhehu    (501) staff       (20)      413 2023-06-21 15:44:20.000000 acore_soap_app-0.1.1/acore_soap_app/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/acore_soap_app/_version.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.036723 acore_soap_app-0.1.1/acore_soap_app/agent/
--rw-r--r--   0 sanhehu    (501) staff       (20)      795 2023-06-21 01:55:28.000000 acore_soap_app-0.1.1/acore_soap_app/agent/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      731 2023-06-21 15:11:48.000000 acore_soap_app-0.1.1/acore_soap_app/agent/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      425 2023-05-10 15:07:05.000000 acore_soap_app-0.1.1/acore_soap_app/agent/execute-command.xml
--rw-r--r--   0 sanhehu    (501) staff       (20)    12691 2023-06-21 15:30:39.000000 acore_soap_app-0.1.1/acore_soap_app/agent/impl.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      314 2023-06-21 15:29:07.000000 acore_soap_app-0.1.1/acore_soap_app/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.037347 acore_soap_app-0.1.1/acore_soap_app/cli/
--rw-r--r--   0 sanhehu    (501) staff       (20)       67 2023-06-21 15:12:04.000000 acore_soap_app-0.1.1/acore_soap_app/cli/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2496 2023-06-21 15:12:16.000000 acore_soap_app-0.1.1/acore_soap_app/cli/impl.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1507 2023-06-21 15:39:23.000000 acore_soap_app-0.1.1/acore_soap_app/cli/main.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.037454 acore_soap_app-0.1.1/acore_soap_app/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/acore_soap_app/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      982 2023-06-21 01:09:10.000000 acore_soap_app-0.1.1/acore_soap_app/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      660 2023-06-20 12:56:41.000000 acore_soap_app-0.1.1/acore_soap_app/paths.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.038256 acore_soap_app-0.1.1/acore_soap_app/sdk/
--rw-r--r--   0 sanhehu    (501) staff       (20)      175 2023-06-21 01:56:33.000000 acore_soap_app-0.1.1/acore_soap_app/sdk/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      250 2023-06-21 15:15:19.000000 acore_soap_app-0.1.1/acore_soap_app/sdk/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4678 2023-06-21 15:21:55.000000 acore_soap_app-0.1.1/acore_soap_app/sdk/canned.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6272 2023-06-21 15:33:19.000000 acore_soap_app-0.1.1/acore_soap_app/sdk/core.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.038720 acore_soap_app-0.1.1/acore_soap_app/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/acore_soap_app/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/acore_soap_app/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-21 13:24:48.000000 acore_soap_app-0.1.1/acore_soap_app/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      646 2023-06-21 12:16:28.000000 acore_soap_app-0.1.1/acore_soap_app/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.040811 acore_soap_app-0.1.1/acore_soap_app/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/acore_soap_app/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/acore_soap_app/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.036104 acore_soap_app-0.1.1/acore_soap_app.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5307 2023-06-21 15:46:35.000000 acore_soap_app-0.1.1/acore_soap_app.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1113 2023-06-21 15:46:35.000000 acore_soap_app-0.1.1/acore_soap_app.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-21 15:46:35.000000 acore_soap_app-0.1.1/acore_soap_app.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       55 2023-06-21 15:46:35.000000 acore_soap_app-0.1.1/acore_soap_app.egg-info/entry_points.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      324 2023-06-21 15:46:35.000000 acore_soap_app-0.1.1/acore_soap_app.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-21 15:46:35.000000 acore_soap_app-0.1.1/acore_soap_app.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-06-21 13:24:55.000000 acore_soap_app-0.1.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      205 2023-06-21 14:19:13.000000 acore_soap_app-0.1.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-21 15:46:35.041397 acore_soap_app-0.1.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-06-20 13:22:31.000000 acore_soap_app-0.1.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 15:46:35.040977 acore_soap_app-0.1.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      226 2023-06-20 05:17:17.000000 acore_soap_app-0.1.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.102656 acore_soap_app-0.2.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1125 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5568 2023-06-26 04:09:41.102528 acore_soap_app-0.2.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4429 2023-06-26 04:04:32.000000 acore_soap_app-0.2.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.097341 acore_soap_app-0.2.1/acore_soap_app/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      413 2023-06-21 15:44:20.000000 acore_soap_app-0.2.1/acore_soap_app/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 04:02:21.000000 acore_soap_app-0.2.1/acore_soap_app/_version.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.099088 acore_soap_app-0.2.1/acore_soap_app/agent/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      795 2023-06-21 01:55:28.000000 acore_soap_app-0.2.1/acore_soap_app/agent/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      731 2023-06-21 15:11:48.000000 acore_soap_app-0.2.1/acore_soap_app/agent/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      425 2023-05-10 15:07:05.000000 acore_soap_app-0.2.1/acore_soap_app/agent/execute-command.xml
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12691 2023-06-21 15:30:39.000000 acore_soap_app-0.2.1/acore_soap_app/agent/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      314 2023-06-21 15:29:07.000000 acore_soap_app-0.2.1/acore_soap_app/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.099790 acore_soap_app-0.2.1/acore_soap_app/cli/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       67 2023-06-21 15:12:04.000000 acore_soap_app-0.2.1/acore_soap_app/cli/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3352 2023-06-26 03:30:48.000000 acore_soap_app-0.2.1/acore_soap_app/cli/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2004 2023-06-26 03:51:41.000000 acore_soap_app-0.2.1/acore_soap_app/cli/main.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.099987 acore_soap_app-0.2.1/acore_soap_app/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/acore_soap_app/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      982 2023-06-21 01:09:10.000000 acore_soap_app-0.2.1/acore_soap_app/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      660 2023-06-20 12:56:41.000000 acore_soap_app-0.2.1/acore_soap_app/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.100618 acore_soap_app-0.2.1/acore_soap_app/sdk/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      175 2023-06-21 01:56:33.000000 acore_soap_app-0.2.1/acore_soap_app/sdk/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      271 2023-06-26 03:14:10.000000 acore_soap_app-0.2.1/acore_soap_app/sdk/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.101288 acore_soap_app-0.2.1/acore_soap_app/sdk/canned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-26 03:12:13.000000 acore_soap_app-0.2.1/acore_soap_app/sdk/canned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      292 2023-06-26 03:14:58.000000 acore_soap_app-0.2.1/acore_soap_app/sdk/canned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4886 2023-06-26 03:14:28.000000 acore_soap_app-0.2.1/acore_soap_app/sdk/canned/impl.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6272 2023-06-21 15:33:19.000000 acore_soap_app-0.2.1/acore_soap_app/sdk/core.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.101853 acore_soap_app-0.2.1/acore_soap_app/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/acore_soap_app/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/acore_soap_app/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-21 13:24:48.000000 acore_soap_app-0.2.1/acore_soap_app/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      646 2023-06-21 12:16:28.000000 acore_soap_app-0.2.1/acore_soap_app/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.102202 acore_soap_app-0.2.1/acore_soap_app/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/acore_soap_app/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/acore_soap_app/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.098274 acore_soap_app-0.2.1/acore_soap_app.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5568 2023-06-26 04:09:41.000000 acore_soap_app-0.2.1/acore_soap_app.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1189 2023-06-26 04:09:41.000000 acore_soap_app-0.2.1/acore_soap_app.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 04:09:41.000000 acore_soap_app-0.2.1/acore_soap_app.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       55 2023-06-26 04:09:41.000000 acore_soap_app-0.2.1/acore_soap_app.egg-info/entry_points.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      324 2023-06-26 04:09:41.000000 acore_soap_app-0.2.1/acore_soap_app.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-26 04:09:41.000000 acore_soap_app-0.2.1/acore_soap_app.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      786 2023-06-26 04:03:12.000000 acore_soap_app-0.2.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-06-21 13:24:55.000000 acore_soap_app-0.2.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      205 2023-06-26 04:09:10.000000 acore_soap_app-0.2.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 04:09:41.102695 acore_soap_app-0.2.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7699 2023-06-20 13:22:31.000000 acore_soap_app-0.2.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 04:09:41.102340 acore_soap_app-0.2.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      226 2023-06-20 05:17:17.000000 acore_soap_app-0.2.1/tests/test_api.py
```

### Comparing `acore_soap_app-0.1.1/AUTHORS.rst` & `acore_soap_app-0.2.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/LICENSE.txt` & `acore_soap_app-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/PKG-INFO` & `acore_soap_app-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_soap_app
-Version: 0.1.1
+Version: 0.2.1
 Summary: Azerothcore World of Warcraft Soap Remote Access Python Library.
 Home-page: https://github.com/MacHu-GWU/acore_soap_app-project
-Download-URL: https://pypi.python.org/pypi/acore_soap_app/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_soap_app/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -78,21 +78,29 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/acore-soap-app#files
 
 
 Welcome to ``acore_soap_app`` Documentation
 ==============================================================================
+📔 `完整文档点这里 <https://acore-soap-app.readthedocs.io/en/latest/>`_
+
 魔兽世界服务器 worldserver 自带一个交互式的 Console. GM 可以在里面输入命令来创建账号, 修改密码, 封禁账号等. 你如果用 GM 账号登录游戏, 你也可以在游戏内聊天框输入 GM 命令, 本质是一样的. 但是你需要 SSH 到服务器上才能访问这个 Console 界面, 又或是要登录游戏才能输入 GM 命令, 且这些命令必须要人类手动输入. 简而言之, 这套系统是给人类用的. 但是作为服务器维护者, 你会有需要用程序扫描数据库, 日志分析用户行为, 并且进行自动化维护, 例如封号, 发邮件等等. 这些自动化运维的脚本可能是在游戏服务器上运行, 也可能是在其他地方运行, 例如其他 EC2, 容器, Lambda. 这时我们就需要一套机制能安全地 (仅让有权限的人或机器) 远程执行 GM 命令. 这个需求对于长期的正式运营非常重要. 例如你需要玩家能登录你的服务器官网注册账号, 交易物品等等. 那么你就需要你的官网 Web 服务器能远程执行一些 GM 命令.
 
 该项目是一个针对这个需求的完整解决方案, 它包含两个组件 Agent 和 SDK.
 
 - Agent: 提供了一个部署在游戏服务器 EC2 上的命令行程序, 作为外部 API 调用的桥梁. 使得外部有权限的开发者可以通过 AWS SSM Run Command 远程调用这个命令行程序, 从而实现远程执行 GM 命令.
 - SDK: 提供了一套远程运行服务器命令的 SDK, 并提供了很多高级功能例如批量执行, 错误处理等功能. 使得开发者可以很方便的编写出基于 GM 命令的应用程序.
 
+在 EC2 上安装完 Agent 之后, 你可以用下面的命令测试.
+
+.. code-block:: bash
+
+    /home/ubuntu/git_repos/acore_soap_app-project/.venv/bin/acsoap gm ".server info"
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``acore_soap_app`` is released on PyPI, so all you need is to:
```

### Comparing `acore_soap_app-0.1.1/README.rst` & `acore_soap_app-0.2.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -46,21 +46,29 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/acore-soap-app#files
 
 
 Welcome to ``acore_soap_app`` Documentation
 ==============================================================================
+📔 `完整文档点这里 <https://acore-soap-app.readthedocs.io/en/latest/>`_
+
 魔兽世界服务器 worldserver 自带一个交互式的 Console. GM 可以在里面输入命令来创建账号, 修改密码, 封禁账号等. 你如果用 GM 账号登录游戏, 你也可以在游戏内聊天框输入 GM 命令, 本质是一样的. 但是你需要 SSH 到服务器上才能访问这个 Console 界面, 又或是要登录游戏才能输入 GM 命令, 且这些命令必须要人类手动输入. 简而言之, 这套系统是给人类用的. 但是作为服务器维护者, 你会有需要用程序扫描数据库, 日志分析用户行为, 并且进行自动化维护, 例如封号, 发邮件等等. 这些自动化运维的脚本可能是在游戏服务器上运行, 也可能是在其他地方运行, 例如其他 EC2, 容器, Lambda. 这时我们就需要一套机制能安全地 (仅让有权限的人或机器) 远程执行 GM 命令. 这个需求对于长期的正式运营非常重要. 例如你需要玩家能登录你的服务器官网注册账号, 交易物品等等. 那么你就需要你的官网 Web 服务器能远程执行一些 GM 命令.
 
 该项目是一个针对这个需求的完整解决方案, 它包含两个组件 Agent 和 SDK.
 
 - Agent: 提供了一个部署在游戏服务器 EC2 上的命令行程序, 作为外部 API 调用的桥梁. 使得外部有权限的开发者可以通过 AWS SSM Run Command 远程调用这个命令行程序, 从而实现远程执行 GM 命令.
 - SDK: 提供了一套远程运行服务器命令的 SDK, 并提供了很多高级功能例如批量执行, 错误处理等功能. 使得开发者可以很方便的编写出基于 GM 命令的应用程序.
 
+在 EC2 上安装完 Agent 之后, 你可以用下面的命令测试.
+
+.. code-block:: bash
+
+    /home/ubuntu/git_repos/acore_soap_app-project/.venv/bin/acsoap gm ".server info"
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``acore_soap_app`` is released on PyPI, so all you need is to:
```

### Comparing `acore_soap_app-0.1.1/acore_soap_app/agent/__init__.py` & `acore_soap_app-0.2.1/acore_soap_app/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app/agent/api.py` & `acore_soap_app-0.2.1/acore_soap_app/agent/api.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app/agent/impl.py` & `acore_soap_app-0.2.1/acore_soap_app/agent/impl.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app/cli/main.py` & `acore_soap_app-0.2.1/acore_soap_app/cli/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,56 @@
 """
 
 import typing as T
 import fire
 
 from .impl import (
     gm,
+    count_online_players,
 )
 
 
+class Canned:
+    """
+    A collection of canned SOAP Agent commands.
+    """
+    def count_online_players(
+        self,
+        user: T.Optional[str] = None,
+        pwd: T.Optional[str] = None,
+    ):
+        """
+        Get the online players and characters in world. Also, you can use this
+         command to check whether server is online.
+
+        Example::
+
+            acsoap canned count-online-players --help
+
+            acsoap canned count-online-players
+        """
+        count_online_players(
+            username=user,
+            password=pwd,
+        )
+
+
 class Command:
     """
-    Acore Soap Agent command line interface.
+    Acore Soap Agent command line interface. All these commands can only be
+    used on EC2.
 
     Example:
 
     - acsoap
     """
-    # --------------------------------------------------------------------------
-    # These two command can only be used on EC2
-    # --------------------------------------------------------------------------
+
+    def __init__(self):
+        self.canned = Canned()
+
     def gm(
         self,
         cmd: str,
         user: T.Optional[str] = None,
         pwd: T.Optional[str] = None,
         raises: bool = True,
         s3uri: T.Optional[str] = None,
```

### Comparing `acore_soap_app-0.1.1/acore_soap_app/exc.py` & `acore_soap_app-0.2.1/acore_soap_app/exc.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app/paths.py` & `acore_soap_app-0.2.1/acore_soap_app/paths.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app/sdk/canned.py` & `acore_soap_app-0.2.1/acore_soap_app/sdk/canned/impl.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,32 @@
 - https://www.azerothcore.org/wiki/gm-commands
 """
 
 import typing as T
 import re
 from boto_session_manager import BotoSesManager
 
-from ..exc import SOAPResponseParseError, SOAPCommandFailedError
-from .core import run_soap_command
+from ...exc import SOAPResponseParseError, SOAPCommandFailedError
+from ..core import run_soap_command
+
+
+def extract_online_players(message: str) -> T.Tuple[int, int]:
+    res = re.findall(r"Connected players: (\d+)", message)
+    if len(res) == 1:
+        connected_players = int(res[0])
+    else:  # pragma: no cover
+        raise SOAPResponseParseError(message)
+
+    res = re.findall(r"Characters in world: (\d+)", message)
+    if len(res) == 1:
+        characters_in_world = int(res[0])
+    else:  # pragma: no cover
+        raise SOAPResponseParseError(message)
+
+    return connected_players, characters_in_world
 
 
 def get_online_players(
     bsm: BotoSesManager,
     server_id: str,
     raises: bool = True,
 ) -> T.Dict[str, int]:
@@ -36,25 +52,15 @@
     response = run_soap_command(
         bsm=bsm,
         server_id=server_id,
         request_like=".server info",
         raises=raises,
     )[0]
 
-    res = re.findall(r"Connected players: (\d+)", response.message)
-    if len(res) == 1:
-        connected_players = int(res[0])
-    else:
-        raise SOAPResponseParseError(response.message)
-
-    res = re.findall(r"Characters in world: (\d+)", response.message)
-    if len(res) == 1:
-        characters_in_world = int(res[0])
-    else:
-        raise SOAPResponseParseError(response.message)
+    connected_players, characters_in_world = extract_online_players(response.message)
 
     return {
         "connected_players": connected_players,
         "characters_in_world": characters_in_world,
     }
```

### Comparing `acore_soap_app-0.1.1/acore_soap_app/sdk/core.py` & `acore_soap_app-0.2.1/acore_soap_app/sdk/core.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app/tests/mock_aws.py` & `acore_soap_app-0.2.1/acore_soap_app/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app/utils.py` & `acore_soap_app-0.2.1/acore_soap_app/utils.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app/vendor/pytest_cov_helper.py` & `acore_soap_app-0.2.1/acore_soap_app/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/acore_soap_app.egg-info/PKG-INFO` & `acore_soap_app-0.2.1/acore_soap_app.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-soap-app
-Version: 0.1.1
+Version: 0.2.1
 Summary: Azerothcore World of Warcraft Soap Remote Access Python Library.
 Home-page: https://github.com/MacHu-GWU/acore_soap_app-project
-Download-URL: https://pypi.python.org/pypi/acore_soap_app/0.1.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_soap_app/0.2.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -78,21 +78,29 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/acore-soap-app#files
 
 
 Welcome to ``acore_soap_app`` Documentation
 ==============================================================================
+📔 `完整文档点这里 <https://acore-soap-app.readthedocs.io/en/latest/>`_
+
 魔兽世界服务器 worldserver 自带一个交互式的 Console. GM 可以在里面输入命令来创建账号, 修改密码, 封禁账号等. 你如果用 GM 账号登录游戏, 你也可以在游戏内聊天框输入 GM 命令, 本质是一样的. 但是你需要 SSH 到服务器上才能访问这个 Console 界面, 又或是要登录游戏才能输入 GM 命令, 且这些命令必须要人类手动输入. 简而言之, 这套系统是给人类用的. 但是作为服务器维护者, 你会有需要用程序扫描数据库, 日志分析用户行为, 并且进行自动化维护, 例如封号, 发邮件等等. 这些自动化运维的脚本可能是在游戏服务器上运行, 也可能是在其他地方运行, 例如其他 EC2, 容器, Lambda. 这时我们就需要一套机制能安全地 (仅让有权限的人或机器) 远程执行 GM 命令. 这个需求对于长期的正式运营非常重要. 例如你需要玩家能登录你的服务器官网注册账号, 交易物品等等. 那么你就需要你的官网 Web 服务器能远程执行一些 GM 命令.
 
 该项目是一个针对这个需求的完整解决方案, 它包含两个组件 Agent 和 SDK.
 
 - Agent: 提供了一个部署在游戏服务器 EC2 上的命令行程序, 作为外部 API 调用的桥梁. 使得外部有权限的开发者可以通过 AWS SSM Run Command 远程调用这个命令行程序, 从而实现远程执行 GM 命令.
 - SDK: 提供了一套远程运行服务器命令的 SDK, 并提供了很多高级功能例如批量执行, 错误处理等功能. 使得开发者可以很方便的编写出基于 GM 命令的应用程序.
 
+在 EC2 上安装完 Agent 之后, 你可以用下面的命令测试.
+
+.. code-block:: bash
+
+    /home/ubuntu/git_repos/acore_soap_app-project/.venv/bin/acsoap gm ".server info"
+
 
 .. _install:
 
 Install
 ------------------------------------------------------------------------------
 
 ``acore_soap_app`` is released on PyPI, so all you need is to:
```

### Comparing `acore_soap_app-0.1.1/acore_soap_app.egg-info/SOURCES.txt` & `acore_soap_app-0.2.1/acore_soap_app.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 acore_soap_app/agent/impl.py
 acore_soap_app/cli/__init__.py
 acore_soap_app/cli/impl.py
 acore_soap_app/cli/main.py
 acore_soap_app/docs/__init__.py
 acore_soap_app/sdk/__init__.py
 acore_soap_app/sdk/api.py
-acore_soap_app/sdk/canned.py
 acore_soap_app/sdk/core.py
+acore_soap_app/sdk/canned/__init__.py
+acore_soap_app/sdk/canned/api.py
+acore_soap_app/sdk/canned/impl.py
 acore_soap_app/tests/__init__.py
 acore_soap_app/tests/helper.py
 acore_soap_app/tests/mock_aws.py
 acore_soap_app/vendor/__init__.py
 acore_soap_app/vendor/pytest_cov_helper.py
 tests/test_api.py
```

### Comparing `acore_soap_app-0.1.1/requirements-doc.txt` & `acore_soap_app-0.2.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_soap_app-0.1.1/setup.py` & `acore_soap_app-0.2.1/setup.py`

 * *Files identical despite different names*

