# Comparing `tmp/duffy-3.3.6rc1.tar.gz` & `tmp/duffy-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duffy-3.3.6rc1.tar", max compression
+gzip compressed data, was "duffy-3.3.7.tar", max compression
```

## Comparing `duffy-3.3.6rc1.tar` & `duffy-3.3.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     1062 2022-04-01 09:18:05.729280 duffy-3.3.6rc1/LICENSE
--rw-r--r--   0        0        0     2614 2022-03-17 11:36:00.362316 duffy-3.3.6rc1/README.md
--rw-r--r--   0        0        0        0 2021-11-04 19:37:25.052374 duffy-3.3.6rc1/duffy/__init__.py
--rw-r--r--   0        0        0     3797 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/admin.py
--rw-r--r--   0        0        0      763 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/__init__.py
--rw-r--r--   0        0        0      438 2022-05-05 09:39:16.752260 duffy-3.3.6rc1/duffy/api_models/common.py
--rw-r--r--   0        0        0      901 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/node.py
--rw-r--r--   0        0        0      785 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/pool.py
--rw-r--r--   0        0        0     1276 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/session.py
--rw-r--r--   0        0        0     2168 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/api_models/tenant.py
--rw-r--r--   0        0        0        0 2021-11-04 19:37:25.053374 duffy-3.3.6rc1/duffy/app/__init__.py
--rw-r--r--   0        0        0     1478 2021-12-23 11:53:40.419878 duffy-3.3.6rc1/duffy/app/auth.py
--rw-r--r--   0        0        0        0 2021-12-09 12:35:44.361777 duffy-3.3.6rc1/duffy/app/controllers/__init__.py
--rw-r--r--   0        0        0     2393 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/controllers/node.py
--rw-r--r--   0        0        0     2003 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/controllers/pool.py
--rw-r--r--   0        0        0    13631 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/controllers/session.py
--rw-r--r--   0        0        0     5820 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/controllers/tenant.py
--rw-r--r--   0        0        0      438 2023-06-13 10:45:34.117491 duffy-3.3.6rc1/duffy/app/database.py
--rw-r--r--   0        0        0     1763 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/app/main.py
--rw-r--r--   0        0        0     1301 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/app/util.py
--rw-r--r--   0        0        0    22150 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/cli.py
--rw-r--r--   0        0        0       96 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/client/__init__.py
--rw-r--r--   0        0        0     4287 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/client/formatter.py
--rw-r--r--   0        0        0     4201 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/client/main.py
--rw-r--r--   0        0        0       71 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/configuration/__init__.py
--rw-r--r--   0        0        0     1736 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/configuration/main.py
--rw-r--r--   0        0        0     4804 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/configuration/validation.py
--rw-r--r--   0        0        0     2675 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/database/__init__.py
--rw-r--r--   0        0        0     1840 2022-02-14 16:30:16.414977 duffy-3.3.6rc1/duffy/database/migrations/env.py
--rw-r--r--   0        0        0     2512 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/database/migrations/main.py
--rw-r--r--   0        0        0      530 2022-02-23 17:54:04.381223 duffy-3.3.6rc1/duffy/database/migrations/script.py.mako
--rw-r--r--   0        0        0        0 2021-11-23 15:11:13.761517 duffy-3.3.6rc1/duffy/database/migrations/versions/.empty
--rw-r--r--   0        0        0      611 2023-06-13 10:45:34.118491 duffy-3.3.6rc1/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py
--rw-r--r--   0        0        0      134 2022-01-31 09:33:13.840537 duffy-3.3.6rc1/duffy/database/model/__init__.py
--rw-r--r--   0        0        0     3032 2023-04-17 12:35:31.798781 duffy-3.3.6rc1/duffy/database/model/node.py
--rw-r--r--   0        0        0     1082 2022-03-14 11:18:18.016981 duffy-3.3.6rc1/duffy/database/model/session.py
--rw-r--r--   0        0        0     2845 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/database/model/tenant.py
--rw-r--r--   0        0        0     3811 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/database/setup.py
--rw-r--r--   0        0        0      281 2022-02-14 16:30:16.414977 duffy-3.3.6rc1/duffy/database/types.py
--rw-r--r--   0        0        0     4590 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/database/util.py
--rw-r--r--   0        0        0      358 2021-11-24 14:21:28.066307 duffy-3.3.6rc1/duffy/exceptions.py
--rw-r--r--   0        0        0        0 2022-02-07 13:59:09.420061 duffy-3.3.6rc1/duffy/legacy/__init__.py
--rw-r--r--   0        0        0       99 2022-02-07 13:59:09.420061 duffy-3.3.6rc1/duffy/legacy/api_models.py
--rw-r--r--   0        0        0      949 2022-02-07 13:59:09.420061 duffy-3.3.6rc1/duffy/legacy/auth.py
--rw-r--r--   0        0        0     8273 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/legacy/main.py
--rw-r--r--   0        0        0     3163 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/misc.py
--rw-r--r--   0        0        0        0 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/__init__.py
--rw-r--r--   0        0        0     2862 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/context.py
--rw-r--r--   0        0        0      102 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/mechanisms/__init__.py
--rw-r--r--   0        0        0     4076 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/mechanisms/ansible.py
--rw-r--r--   0        0        0     1210 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/mechanisms/main.py
--rw-r--r--   0        0        0     3855 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/nodes/pools.py
--rw-r--r--   0        0        0     2175 2022-05-03 12:14:31.685232 duffy-3.3.6rc1/duffy/shell.py
--rw-r--r--   0        0        0      293 2022-03-14 11:18:18.016981 duffy-3.3.6rc1/duffy/tasks/__init__.py
--rw-r--r--   0        0        0      171 2022-02-14 16:30:16.414977 duffy-3.3.6rc1/duffy/tasks/base.py
--rw-r--r--   0        0        0     7168 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/tasks/deprovision.py
--rw-r--r--   0        0        0     1221 2022-03-15 09:19:01.122691 duffy-3.3.6rc1/duffy/tasks/expire.py
--rw-r--r--   0        0        0      417 2022-03-15 09:19:01.122691 duffy-3.3.6rc1/duffy/tasks/locking.py
--rw-r--r--   0        0        0     1326 2023-06-13 10:45:34.119491 duffy-3.3.6rc1/duffy/tasks/main.py
--rw-r--r--   0        0        0    11136 2023-06-13 10:45:34.120491 duffy-3.3.6rc1/duffy/tasks/provision.py
--rw-r--r--   0        0        0     7004 2023-06-13 10:45:34.120491 duffy-3.3.6rc1/duffy/util.py
--rw-r--r--   0        0        0       72 2023-06-13 10:45:34.120491 duffy-3.3.6rc1/duffy/version.py
--rw-r--r--   0        0        0     4299 2023-06-13 11:10:33.330273 duffy-3.3.6rc1/pyproject.toml
--rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 duffy-3.3.6rc1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-04-01 09:18:05.729280 duffy-3.3.7/LICENSE
+-rw-r--r--   0        0        0     2614 2022-03-17 11:36:00.362316 duffy-3.3.7/README.md
+-rw-r--r--   0        0        0        0 2021-11-04 19:37:25.052374 duffy-3.3.7/duffy/__init__.py
+-rw-r--r--   0        0        0     3797 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/admin.py
+-rw-r--r--   0        0        0      763 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/__init__.py
+-rw-r--r--   0        0        0      438 2022-05-05 09:39:16.752260 duffy-3.3.7/duffy/api_models/common.py
+-rw-r--r--   0        0        0      901 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/node.py
+-rw-r--r--   0        0        0      785 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/pool.py
+-rw-r--r--   0        0        0     1276 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/session.py
+-rw-r--r--   0        0        0     2168 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/api_models/tenant.py
+-rw-r--r--   0        0        0        0 2021-11-04 19:37:25.053374 duffy-3.3.7/duffy/app/__init__.py
+-rw-r--r--   0        0        0     1478 2021-12-23 11:53:40.419878 duffy-3.3.7/duffy/app/auth.py
+-rw-r--r--   0        0        0        0 2021-12-09 12:35:44.361777 duffy-3.3.7/duffy/app/controllers/__init__.py
+-rw-r--r--   0        0        0     2393 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/controllers/node.py
+-rw-r--r--   0        0        0     2003 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/controllers/pool.py
+-rw-r--r--   0        0        0    13631 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/controllers/session.py
+-rw-r--r--   0        0        0     5820 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/controllers/tenant.py
+-rw-r--r--   0        0        0      438 2023-06-13 10:45:34.117491 duffy-3.3.7/duffy/app/database.py
+-rw-r--r--   0        0        0     1763 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/app/main.py
+-rw-r--r--   0        0        0     1301 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/app/util.py
+-rw-r--r--   0        0        0    22150 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/cli.py
+-rw-r--r--   0        0        0       96 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/client/__init__.py
+-rw-r--r--   0        0        0     4287 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/client/formatter.py
+-rw-r--r--   0        0        0     4201 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/client/main.py
+-rw-r--r--   0        0        0       71 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/configuration/__init__.py
+-rw-r--r--   0        0        0     1736 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/configuration/main.py
+-rw-r--r--   0        0        0     4804 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/configuration/validation.py
+-rw-r--r--   0        0        0     2675 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/database/__init__.py
+-rw-r--r--   0        0        0     1840 2022-02-14 16:30:16.414977 duffy-3.3.7/duffy/database/migrations/env.py
+-rw-r--r--   0        0        0     2512 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/database/migrations/main.py
+-rw-r--r--   0        0        0      530 2022-02-23 17:54:04.381223 duffy-3.3.7/duffy/database/migrations/script.py.mako
+-rw-r--r--   0        0        0        0 2021-11-23 15:11:13.761517 duffy-3.3.7/duffy/database/migrations/versions/.empty
+-rw-r--r--   0        0        0      611 2023-06-13 10:45:34.118491 duffy-3.3.7/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py
+-rw-r--r--   0        0        0      134 2022-01-31 09:33:13.840537 duffy-3.3.7/duffy/database/model/__init__.py
+-rw-r--r--   0        0        0     3032 2023-04-17 12:35:31.798781 duffy-3.3.7/duffy/database/model/node.py
+-rw-r--r--   0        0        0     1082 2022-03-14 11:18:18.016981 duffy-3.3.7/duffy/database/model/session.py
+-rw-r--r--   0        0        0     2845 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/database/model/tenant.py
+-rw-r--r--   0        0        0     3811 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/database/setup.py
+-rw-r--r--   0        0        0      281 2022-02-14 16:30:16.414977 duffy-3.3.7/duffy/database/types.py
+-rw-r--r--   0        0        0     4590 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/database/util.py
+-rw-r--r--   0        0        0      358 2021-11-24 14:21:28.066307 duffy-3.3.7/duffy/exceptions.py
+-rw-r--r--   0        0        0        0 2022-02-07 13:59:09.420061 duffy-3.3.7/duffy/legacy/__init__.py
+-rw-r--r--   0        0        0       99 2022-02-07 13:59:09.420061 duffy-3.3.7/duffy/legacy/api_models.py
+-rw-r--r--   0        0        0      949 2022-02-07 13:59:09.420061 duffy-3.3.7/duffy/legacy/auth.py
+-rw-r--r--   0        0        0     8273 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/legacy/main.py
+-rw-r--r--   0        0        0     3163 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/misc.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/__init__.py
+-rw-r--r--   0        0        0     2862 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/context.py
+-rw-r--r--   0        0        0      102 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/mechanisms/__init__.py
+-rw-r--r--   0        0        0     4076 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/mechanisms/ansible.py
+-rw-r--r--   0        0        0     1210 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/mechanisms/main.py
+-rw-r--r--   0        0        0     3855 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/nodes/pools.py
+-rw-r--r--   0        0        0     2175 2022-05-03 12:14:31.685232 duffy-3.3.7/duffy/shell.py
+-rw-r--r--   0        0        0      293 2022-03-14 11:18:18.016981 duffy-3.3.7/duffy/tasks/__init__.py
+-rw-r--r--   0        0        0      171 2022-02-14 16:30:16.414977 duffy-3.3.7/duffy/tasks/base.py
+-rw-r--r--   0        0        0     7168 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/tasks/deprovision.py
+-rw-r--r--   0        0        0     1221 2022-03-15 09:19:01.122691 duffy-3.3.7/duffy/tasks/expire.py
+-rw-r--r--   0        0        0      417 2022-03-15 09:19:01.122691 duffy-3.3.7/duffy/tasks/locking.py
+-rw-r--r--   0        0        0     1326 2023-06-13 10:45:34.119491 duffy-3.3.7/duffy/tasks/main.py
+-rw-r--r--   0        0        0    11136 2023-06-13 10:45:34.120491 duffy-3.3.7/duffy/tasks/provision.py
+-rw-r--r--   0        0        0     7004 2023-06-13 10:45:34.120491 duffy-3.3.7/duffy/util.py
+-rw-r--r--   0        0        0       72 2023-06-13 10:45:34.120491 duffy-3.3.7/duffy/version.py
+-rw-r--r--   0        0        0     4296 2023-06-26 11:04:46.069607 duffy-3.3.7/pyproject.toml
+-rw-r--r--   0        0        0     5714 1970-01-01 00:00:00.000000 duffy-3.3.7/PKG-INFO
```

### Comparing `duffy-3.3.6rc1/LICENSE` & `duffy-3.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/README.md` & `duffy-3.3.7/README.md`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/admin.py` & `duffy-3.3.7/duffy/admin.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/api_models/__init__.py` & `duffy-3.3.7/duffy/api_models/__init__.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/api_models/node.py` & `duffy-3.3.7/duffy/api_models/node.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/api_models/pool.py` & `duffy-3.3.7/duffy/api_models/pool.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/api_models/session.py` & `duffy-3.3.7/duffy/api_models/session.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/api_models/tenant.py` & `duffy-3.3.7/duffy/api_models/tenant.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/app/auth.py` & `duffy-3.3.7/duffy/app/auth.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/app/controllers/node.py` & `duffy-3.3.7/duffy/app/controllers/node.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/app/controllers/pool.py` & `duffy-3.3.7/duffy/app/controllers/pool.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/app/controllers/session.py` & `duffy-3.3.7/duffy/app/controllers/session.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/app/controllers/tenant.py` & `duffy-3.3.7/duffy/app/controllers/tenant.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/app/main.py` & `duffy-3.3.7/duffy/app/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/app/util.py` & `duffy-3.3.7/duffy/app/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/cli.py` & `duffy-3.3.7/duffy/cli.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/client/formatter.py` & `duffy-3.3.7/duffy/client/formatter.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/client/main.py` & `duffy-3.3.7/duffy/client/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/configuration/main.py` & `duffy-3.3.7/duffy/configuration/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/configuration/validation.py` & `duffy-3.3.7/duffy/configuration/validation.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/__init__.py` & `duffy-3.3.7/duffy/database/__init__.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/migrations/env.py` & `duffy-3.3.7/duffy/database/migrations/env.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/migrations/main.py` & `duffy-3.3.7/duffy/database/migrations/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/migrations/script.py.mako` & `duffy-3.3.7/duffy/database/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py` & `duffy-3.3.7/duffy/database/migrations/versions/ce2e575cb800_add_tenant_session_lifetimes.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/model/node.py` & `duffy-3.3.7/duffy/database/model/node.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/model/session.py` & `duffy-3.3.7/duffy/database/model/session.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/model/tenant.py` & `duffy-3.3.7/duffy/database/model/tenant.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/setup.py` & `duffy-3.3.7/duffy/database/setup.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/database/util.py` & `duffy-3.3.7/duffy/database/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/legacy/auth.py` & `duffy-3.3.7/duffy/legacy/auth.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/legacy/main.py` & `duffy-3.3.7/duffy/legacy/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/misc.py` & `duffy-3.3.7/duffy/misc.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/nodes/context.py` & `duffy-3.3.7/duffy/nodes/context.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/nodes/mechanisms/ansible.py` & `duffy-3.3.7/duffy/nodes/mechanisms/ansible.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/nodes/mechanisms/main.py` & `duffy-3.3.7/duffy/nodes/mechanisms/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/nodes/pools.py` & `duffy-3.3.7/duffy/nodes/pools.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/shell.py` & `duffy-3.3.7/duffy/shell.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/tasks/deprovision.py` & `duffy-3.3.7/duffy/tasks/deprovision.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/tasks/expire.py` & `duffy-3.3.7/duffy/tasks/expire.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/tasks/main.py` & `duffy-3.3.7/duffy/tasks/main.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/tasks/provision.py` & `duffy-3.3.7/duffy/tasks/provision.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/duffy/util.py` & `duffy-3.3.7/duffy/util.py`

 * *Files identical despite different names*

### Comparing `duffy-3.3.6rc1/pyproject.toml` & `duffy-3.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "duffy"
-version = "3.3.6rc1"
+version = "3.3.7"
 description = "CentOS CI provisioner"
 authors = ["Nils Philippsen <nils@redhat.com>", "Vipul Siddharth <siddharthvipul1@gmail.com>", "Akashdeep Dhar <akashdeep@redhat.com>", "Ben Capper <bcapper@redhat.com>"]
 license = "MIT"
 maintainers = ["Nils Philippsen <nils@redhat.com>", "Vipul Siddharth <siddharthvipul1@gmail.com>", "Akashdeep Dhar <akashdeep@redhat.com>", "Ben Capper <bcapper@redhat.com>"]
 readme = "README.md"
 homepage = "https://github.com/CentOS/duffy"
 repository = "https://github.com/CentOS/duffy"
```

### Comparing `duffy-3.3.6rc1/PKG-INFO` & `duffy-3.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duffy
-Version: 3.3.6rc1
+Version: 3.3.7
 Summary: CentOS CI provisioner
 Home-page: https://github.com/CentOS/duffy
 License: MIT
 Keywords: baremetal,ci,vm,opennebula,centos
 Author: Nils Philippsen
 Author-email: nils@redhat.com
 Maintainer: Nils Philippsen
```

