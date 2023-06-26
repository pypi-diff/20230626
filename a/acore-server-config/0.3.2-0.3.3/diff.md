# Comparing `tmp/acore_server_config-0.3.2.tar.gz` & `tmp/acore_server_config-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_config-0.3.2.tar", last modified: Thu Jun 22 04:14:39 2023, max compression
+gzip compressed data, was "acore_server_config-0.3.3.tar", last modified: Mon Jun 26 05:41:18 2023, max compression
```

## Comparing `acore_server_config-0.3.2.tar` & `acore_server_config-0.3.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.888080 acore_server_config-0.3.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-22 04:14:39.887931 acore_server_config-0.3.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.3.2/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.883260 acore_server_config-0.3.2/acore_server_config/
--rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.3.2/acore_server_config/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-22 03:51:17.000000 acore_server_config-0.3.2/acore_server_config/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      492 2023-06-19 16:52:37.000000 acore_server_config-0.3.2/acore_server_config/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1149 2023-06-22 03:51:05.000000 acore_server_config-0.3.2/acore_server_config/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.3.2/acore_server_config/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.884510 acore_server_config-0.3.2/acore_server_config/config/
--rw-r--r--   0 sanhehu    (501) staff       (20)       50 2023-06-19 17:13:43.000000 acore_server_config-0.3.2/acore_server_config/config/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.885243 acore_server_config-0.3.2/acore_server_config/config/define/
--rw-r--r--   0 sanhehu    (501) staff       (20)       98 2023-06-19 17:13:36.000000 acore_server_config-0.3.2/acore_server_config/config/define/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.3.2/acore_server_config/config/define/main.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1565 2023-06-19 17:35:38.000000 acore_server_config-0.3.2/acore_server_config/config/define/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.3.2/acore_server_config/config/init.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     8011 2023-06-19 17:03:54.000000 acore_server_config-0.3.2/acore_server_config/config/loader.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.885877 acore_server_config-0.3.2/acore_server_config/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3938 2023-06-19 16:51:35.000000 acore_server_config-0.3.2/acore_server_config/in_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.3.2/acore_server_config/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2300 2023-06-22 03:31:06.000000 acore_server_config-0.3.2/acore_server_config/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.886959 acore_server_config-0.3.2/acore_server_config/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      362 2023-06-19 16:31:24.000000 acore_server_config-0.3.2/acore_server_config/tests/dummy_config.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-19 16:26:34.000000 acore_server_config-0.3.2/acore_server_config/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.887480 acore_server_config-0.3.2/acore_server_config/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.883964 acore_server_config-0.3.2/acore_server_config.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      285 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2814 2023-06-22 03:52:00.000000 acore_server_config-0.3.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.3.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-06-19 16:26:45.000000 acore_server_config-0.3.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-22 03:48:21.000000 acore_server_config-0.3.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-22 04:14:39.888126 acore_server_config-0.3.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.887625 acore_server_config-0.3.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      501 2023-06-19 16:53:17.000000 acore_server_config-0.3.2/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.096253 acore_server_config-0.3.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5264 2023-06-26 05:41:18.096090 acore_server_config-0.3.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4102 2023-06-26 05:40:34.000000 acore_server_config-0.3.3/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.091722 acore_server_config-0.3.3/acore_server_config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.3.3/acore_server_config/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-26 05:38:27.000000 acore_server_config-0.3.3/acore_server_config/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      492 2023-06-19 16:52:37.000000 acore_server_config-0.3.3/acore_server_config/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1149 2023-06-22 03:51:05.000000 acore_server_config-0.3.3/acore_server_config/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.3.3/acore_server_config/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.093062 acore_server_config-0.3.3/acore_server_config/config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       50 2023-06-19 17:13:43.000000 acore_server_config-0.3.3/acore_server_config/config/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.093872 acore_server_config-0.3.3/acore_server_config/config/define/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       98 2023-06-19 17:13:36.000000 acore_server_config-0.3.3/acore_server_config/config/define/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.3.3/acore_server_config/config/define/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1565 2023-06-19 17:35:38.000000 acore_server_config-0.3.3/acore_server_config/config/define/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.3.3/acore_server_config/config/init.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8000 2023-06-26 05:34:11.000000 acore_server_config-0.3.3/acore_server_config/config/loader.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.094178 acore_server_config-0.3.3/acore_server_config/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4080 2023-06-26 05:35:57.000000 acore_server_config-0.3.3/acore_server_config/in_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.3.3/acore_server_config/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2300 2023-06-22 03:31:06.000000 acore_server_config-0.3.3/acore_server_config/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.095120 acore_server_config-0.3.3/acore_server_config/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      362 2023-06-19 16:31:24.000000 acore_server_config-0.3.3/acore_server_config/tests/dummy_config.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-19 16:26:34.000000 acore_server_config-0.3.3/acore_server_config/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.095574 acore_server_config-0.3.3/acore_server_config/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/acore_server_config/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.092421 acore_server_config-0.3.3/acore_server_config.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5264 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-26 05:41:18.000000 acore_server_config-0.3.3/acore_server_config.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2973 2023-06-26 05:38:11.000000 acore_server_config-0.3.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.3.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-06-19 16:26:45.000000 acore_server_config-0.3.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      201 2023-06-26 05:32:50.000000 acore_server_config-0.3.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-26 05:41:18.096303 acore_server_config-0.3.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.3.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-26 05:41:18.095758 acore_server_config-0.3.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      501 2023-06-19 16:53:17.000000 acore_server_config-0.3.3/tests/test_api.py
```

### Comparing `acore_server_config-0.3.2/AUTHORS.rst` & `acore_server_config-0.3.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/LICENSE.txt` & `acore_server_config-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/PKG-INFO` & `acore_server_config-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_config
-Version: 0.3.2
+Version: 0.3.3
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -75,18 +75,20 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/acore-server-config#files
 
 
 Welcome to ``acore_server_config`` Documentation
 ==============================================================================
+📔 `完整文档点这里 <https://acore-server-config.readthedocs.io/en/latest/>`_
+
 **项目背景**
 
 在生产环境中一个 "魔兽世界服务器" 通常有多个 "大区", 亚洲, 北美, 美国西部, 美国东部等. 每个 "大区" 下有多组服务器, 一个服务器也就是我们在选择服务器见面看到的 Realm, 比如国服著名的 "山丘之王", "洛萨" 等. 每个服务器都有自己的配置, 例如数据库账号密码等. 那么如何对这么多服务器的配置进行管理呢? 本项目就是为了解决这个问题而生的.
 
 下面我们来看看具体需求.
 
 1. **从开发者的角度看, 我们需要对服务器集群配置进行批量管理和部署. 而我们希望将服务器本身和配置数据分离, 以便于在不重新部署服务器的情况下更新配置**. 根据上一段提到的服务器层级架构, 我们需要一个树状的数据结构来定义这些服务器的配置. 例如一个大区有它默认设置. 在这个大区下的所有服务器如果没有特别说明, 则沿用大区默认设置. 如果有特别说明则用特别说明的设置. 所以我们这个项目需要解决批量管理的功能. 幸运的是, 我以前为企业做的一个项目中有一个按树状结构, 批量管理多个环境的配置的模块 `config_patterns <https://github.com/MacHu-GWU/config_patterns-project>`_ 刚好可以解决这一问题.
 
 2. **而从服务器的角度看, 出于安全考虑, 每个服务器只要知道自己的配置即可, 不需要知道其他服务器的配置. 所以我们需要一个脚本用于** "自省" **(自己判断自己是谁, 去哪里读取配置数据) 并读取属于自己这个服务器的配置数据**. 这个脚本只需要能在服务器上运行即可.
 
-为了解决以上两个需求, 我创建了这一项目. 请阅读完整文档 (点击 Document 标签) 做进一步了解.
+为了解决以上两个需求, 我创建了这一项目. 请阅读完整文档做进一步了解.
```

### Comparing `acore_server_config-0.3.2/README.rst` & `acore_server_config-0.3.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -43,18 +43,20 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/acore-server-config#files
 
 
 Welcome to ``acore_server_config`` Documentation
 ==============================================================================
+📔 `完整文档点这里 <https://acore-server-config.readthedocs.io/en/latest/>`_
+
 **项目背景**
 
 在生产环境中一个 "魔兽世界服务器" 通常有多个 "大区", 亚洲, 北美, 美国西部, 美国东部等. 每个 "大区" 下有多组服务器, 一个服务器也就是我们在选择服务器见面看到的 Realm, 比如国服著名的 "山丘之王", "洛萨" 等. 每个服务器都有自己的配置, 例如数据库账号密码等. 那么如何对这么多服务器的配置进行管理呢? 本项目就是为了解决这个问题而生的.
 
 下面我们来看看具体需求.
 
 1. **从开发者的角度看, 我们需要对服务器集群配置进行批量管理和部署. 而我们希望将服务器本身和配置数据分离, 以便于在不重新部署服务器的情况下更新配置**. 根据上一段提到的服务器层级架构, 我们需要一个树状的数据结构来定义这些服务器的配置. 例如一个大区有它默认设置. 在这个大区下的所有服务器如果没有特别说明, 则沿用大区默认设置. 如果有特别说明则用特别说明的设置. 所以我们这个项目需要解决批量管理的功能. 幸运的是, 我以前为企业做的一个项目中有一个按树状结构, 批量管理多个环境的配置的模块 `config_patterns <https://github.com/MacHu-GWU/config_patterns-project>`_ 刚好可以解决这一问题.
 
 2. **而从服务器的角度看, 出于安全考虑, 每个服务器只要知道自己的配置即可, 不需要知道其他服务器的配置. 所以我们需要一个脚本用于** "自省" **(自己判断自己是谁, 去哪里读取配置数据) 并读取属于自己这个服务器的配置数据**. 这个脚本只需要能在服务器上运行即可.
 
-为了解决以上两个需求, 我创建了这一项目. 请阅读完整文档 (点击 Document 标签) 做进一步了解.
+为了解决以上两个需求, 我创建了这一项目. 请阅读完整文档做进一步了解.
```

### Comparing `acore_server_config-0.3.2/acore_server_config/boto_ses.py` & `acore_server_config-0.3.3/acore_server_config/boto_ses.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/acore_server_config/config/define/main.py` & `acore_server_config-0.3.3/acore_server_config/config/define/main.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/acore_server_config/config/define/server.py` & `acore_server_config-0.3.3/acore_server_config/config/define/server.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/acore_server_config/config/init.py` & `acore_server_config-0.3.3/acore_server_config/config/init.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/acore_server_config/config/loader.py` & `acore_server_config-0.3.3/acore_server_config/config/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 import dataclasses
 import typing as T
 
 from s3pathlib import S3Path
 from simple_aws_ec2.api import Ec2Instance
-from acore_server_metadata.api import settings
+from acore_constants.api import TagKey
 
 from ..boto_ses import bsm as default_bsm
 
 from .define import EnvEnum, Env, Config, Server
 
 
 if T.TYPE_CHECKING:  # pragma: no cover
@@ -51,15 +51,15 @@
 
 def get_this_server_id(bsm: "BotoSesManager") -> str:  # pragma: no cover
     """
     在 EC2 上通过 "自省", 获得这个服务器的 server_id. 它的 naming convention 是
     ``${env_name}-${server_name}``.
     """
     ec2_inst = Ec2Instance.from_ec2_inside(bsm.ec2_client)
-    server_id = ec2_inst.tags[settings.ID_TAG_KEY]
+    server_id = ec2_inst.tags[TagKey.SERVER_ID]
     return server_id
 
 
 def parse_server_id(server_id: str) -> T.Tuple[str, str]:
     """
     解析 server_id, 返回 (env_name, server_name) 的 tuple.
     """
```

### Comparing `acore_server_config-0.3.2/acore_server_config/in_ec2.py` & `acore_server_config-0.3.3/acore_server_config/in_ec2.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 import typing as T
 import warnings
 
 from s3pathlib import S3Path
 from simple_aws_ec2.api import Ec2Instance
-from acore_server_metadata.api import settings
+from acore_constants.api import TagKey
 
 from .boto_ses import bsm as default_bsm
 from .config.define import EnvEnum, Env, Config, Server
 
 if T.TYPE_CHECKING:
     from boto_session_manager import BotoSesManager
 
@@ -57,14 +57,19 @@
     server_id: T.Optional[str] = None,
 ) -> Server:
     """
     在 EC2 上通过 "自省", 获得属于这个服务器的配置数据.
 
     配置数据的详细数据结构请参考 :class:`acore_server_config.config.define.server.Server`.
 
+    .. note::
+    
+        从 0.3.1 开始, 该函数被 Ec2ConfigLoader 和 ConfigLoader 所替代, 该函数仍然保留
+        但不建议使用.
+
     :param bsm: BotoSesManager 实例. 默认使用 EC2 上 IAM Role 所对应的.
     :param parameter_name_prefix: the parameter name prefix, the full name will
         be ${parameter_name_prefix}-${env_name}.
     :param use_s3: 是否从 S3 读取配置数据, 默认使用 S3, 因为配置数据可能会很大.
     :param use_parameter_store: 是否从 AWS Parameter Store 读取配置数据
     :param s3folder_config: S3 配置数据的根目录, 默认为
         s3://aws_account_id}-{aws_region}-artifacts/projects/acore_server_config/config/
@@ -78,15 +83,15 @@
     if sum([use_s3, use_parameter_store]) != 1:
         raise ValueError(
             "Only one of use_s3 and use_parameter_store can be True at the same time."
         )
 
     if server_id is None:
         ec2_inst = Ec2Instance.from_ec2_inside(bsm.ec2_client)
-        server_id = ec2_inst.tags[settings.ID_TAG_KEY]
+        server_id = ec2_inst.tags[TagKey.SERVER_ID]
     env_name, server_name = server_id.split("-", 1)
     if parameter_name_prefix is None:
         parameter_name_prefix = _get_default_parameter_name_prefix()
     parameter_name = f"{parameter_name_prefix}-{env_name}"
 
     if use_s3:
         if s3folder_config is None:
```

### Comparing `acore_server_config-0.3.2/acore_server_config/paths.py` & `acore_server_config-0.3.3/acore_server_config/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/acore_server_config/runtime.py` & `acore_server_config-0.3.3/acore_server_config/runtime.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/acore_server_config/tests/mock_aws.py` & `acore_server_config-0.3.3/acore_server_config/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/acore_server_config/vendor/pytest_cov_helper.py` & `acore_server_config-0.3.3/acore_server_config/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/acore_server_config.egg-info/PKG-INFO` & `acore_server_config-0.3.3/acore_server_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-config
-Version: 0.3.2
+Version: 0.3.3
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.2#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -75,18 +75,20 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/acore-server-config#files
 
 
 Welcome to ``acore_server_config`` Documentation
 ==============================================================================
+📔 `完整文档点这里 <https://acore-server-config.readthedocs.io/en/latest/>`_
+
 **项目背景**
 
 在生产环境中一个 "魔兽世界服务器" 通常有多个 "大区", 亚洲, 北美, 美国西部, 美国东部等. 每个 "大区" 下有多组服务器, 一个服务器也就是我们在选择服务器见面看到的 Realm, 比如国服著名的 "山丘之王", "洛萨" 等. 每个服务器都有自己的配置, 例如数据库账号密码等. 那么如何对这么多服务器的配置进行管理呢? 本项目就是为了解决这个问题而生的.
 
 下面我们来看看具体需求.
 
 1. **从开发者的角度看, 我们需要对服务器集群配置进行批量管理和部署. 而我们希望将服务器本身和配置数据分离, 以便于在不重新部署服务器的情况下更新配置**. 根据上一段提到的服务器层级架构, 我们需要一个树状的数据结构来定义这些服务器的配置. 例如一个大区有它默认设置. 在这个大区下的所有服务器如果没有特别说明, 则沿用大区默认设置. 如果有特别说明则用特别说明的设置. 所以我们这个项目需要解决批量管理的功能. 幸运的是, 我以前为企业做的一个项目中有一个按树状结构, 批量管理多个环境的配置的模块 `config_patterns <https://github.com/MacHu-GWU/config_patterns-project>`_ 刚好可以解决这一问题.
 
 2. **而从服务器的角度看, 出于安全考虑, 每个服务器只要知道自己的配置即可, 不需要知道其他服务器的配置. 所以我们需要一个脚本用于** "自省" **(自己判断自己是谁, 去哪里读取配置数据) 并读取属于自己这个服务器的配置数据**. 这个脚本只需要能在服务器上运行即可.
 
-为了解决以上两个需求, 我创建了这一项目. 请阅读完整文档 (点击 Document 标签) 做进一步了解.
+为了解决以上两个需求, 我创建了这一项目. 请阅读完整文档做进一步了解.
```

### Comparing `acore_server_config-0.3.2/acore_server_config.egg-info/SOURCES.txt` & `acore_server_config-0.3.3/acore_server_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/release-history.rst` & `acore_server_config-0.3.3/release-history.rst`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.3 (2023-06-26)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Miscellaneous**
+
+- upgrade dependencies, no API changes.
+
+
 0.3.2 (2023-06-21)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Minor Improvements**
 
 - add support to use this in AWS CodeBuild and AWS Lambda.
```

### Comparing `acore_server_config-0.3.2/requirements-doc.txt` & `acore_server_config-0.3.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.2/setup.py` & `acore_server_config-0.3.3/setup.py`

 * *Files identical despite different names*

