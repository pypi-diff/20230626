# Comparing `tmp/qotto_auth_client-2.2.2a0.tar.gz` & `tmp/qotto_auth_client-2.2.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qotto_auth_client-2.2.2a0.tar", max compression
+gzip compressed data, was "qotto_auth_client-2.2.2a1.tar", max compression
```

## Comparing `qotto_auth_client-2.2.2a0.tar` & `qotto_auth_client-2.2.2a1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1062 2022-08-03 08:46:30.145586 qotto_auth_client-2.2.2a0/LICENSE
--rw-r--r--   0        0        0     1364 2022-11-22 08:13:56.153627 qotto_auth_client-2.2.2a0/README.md
--rw-r--r--   0        0        0     1166 2023-06-23 07:52:14.585403 qotto_auth_client-2.2.2a0/pyproject.toml
--rw-r--r--   0        0        0      782 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a0/qottoauth/__init__.py
--rw-r--r--   0        0        0      342 2022-11-23 14:46:03.536748 qotto_auth_client-2.2.2a0/qottoauth/api/__init__.py
--rw-r--r--   0        0        0     1516 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a0/qottoauth/api/base.py
--rw-r--r--   0        0        0     4088 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a0/qottoauth/api/cached.py
--rw-r--r--   0        0        0     5211 2023-02-22 20:08:40.637617 qotto_auth_client-2.2.2a0/qottoauth/api/gql.py
--rw-r--r--   0        0        0    37650 2023-06-23 07:50:30.514172 qotto_auth_client-2.2.2a0/qottoauth/api/test.py
--rw-r--r--   0        0        0     9525 2023-03-28 10:47:11.239832 qotto_auth_client-2.2.2a0/qottoauth/models.py
--rw-r--r--   0        0        0       27 2022-01-10 15:06:15.651000 qotto_auth_client-2.2.2a0/qottoauth/py.typed
--rw-r--r--   0        0        0    36482 2023-06-22 21:06:47.346705 qotto_auth_client-2.2.2a0/qottoauth/service.py
--rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 qotto_auth_client-2.2.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-08-03 08:46:30.145586 qotto_auth_client-2.2.2a1/LICENSE
+-rw-r--r--   0        0        0     1364 2022-11-22 08:13:56.153627 qotto_auth_client-2.2.2a1/README.md
+-rw-r--r--   0        0        0     1166 2023-06-23 12:40:07.735952 qotto_auth_client-2.2.2a1/pyproject.toml
+-rw-r--r--   0        0        0      782 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a1/qottoauth/__init__.py
+-rw-r--r--   0        0        0      342 2022-11-23 14:46:03.536748 qotto_auth_client-2.2.2a1/qottoauth/api/__init__.py
+-rw-r--r--   0        0        0     1516 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a1/qottoauth/api/base.py
+-rw-r--r--   0        0        0     4088 2023-01-20 08:10:36.504176 qotto_auth_client-2.2.2a1/qottoauth/api/cached.py
+-rw-r--r--   0        0        0     5211 2023-02-22 20:08:40.637617 qotto_auth_client-2.2.2a1/qottoauth/api/gql.py
+-rw-r--r--   0        0        0    37650 2023-06-23 07:50:30.514172 qotto_auth_client-2.2.2a1/qottoauth/api/test.py
+-rw-r--r--   0        0        0     9525 2023-03-28 10:47:11.239832 qotto_auth_client-2.2.2a1/qottoauth/models.py
+-rw-r--r--   0        0        0       27 2022-01-10 15:06:15.651000 qotto_auth_client-2.2.2a1/qottoauth/py.typed
+-rw-r--r--   0        0        0    36553 2023-06-23 12:39:29.140111 qotto_auth_client-2.2.2a1/qottoauth/service.py
+-rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 qotto_auth_client-2.2.2a1/PKG-INFO
```

### Comparing `qotto_auth_client-2.2.2a0/LICENSE` & `qotto_auth_client-2.2.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.2a0/README.md` & `qotto_auth_client-2.2.2a1/README.md`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.2a0/pyproject.toml` & `qotto_auth_client-2.2.2a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qotto-auth-client"
-version = "2.2.2a0"
+version = "2.2.2a1"
 description = "Qotto/QottoAuthClient"
 authors = ["Qotto Dev Team <dev@qotto.net>"]
 readme = "README.md"
 #homepage
 #repository = "https://gitlab.com/qotto/oss/eventy"
 #documentation = "https://qotto.gitlab.io/oss/eventy"
 #keywords
```

### Comparing `qotto_auth_client-2.2.2a0/qottoauth/__init__.py` & `qotto_auth_client-2.2.2a1/qottoauth/__init__.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.2a0/qottoauth/api/base.py` & `qotto_auth_client-2.2.2a1/qottoauth/api/base.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.2a0/qottoauth/api/cached.py` & `qotto_auth_client-2.2.2a1/qottoauth/api/cached.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.2a0/qottoauth/api/gql.py` & `qotto_auth_client-2.2.2a1/qottoauth/api/gql.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.2a0/qottoauth/api/test.py` & `qotto_auth_client-2.2.2a1/qottoauth/api/test.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.2a0/qottoauth/models.py` & `qotto_auth_client-2.2.2a1/qottoauth/models.py`

 * *Files identical despite different names*

### Comparing `qotto_auth_client-2.2.2a0/qottoauth/service.py` & `qotto_auth_client-2.2.2a1/qottoauth/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,24 +320,25 @@
         return Identity.from_dict(response)
 
     def identities(
             self,
             provider_id: str = None,
             name_contains: str = None, email_contains: str = None,
             user: Union[User, str] = None,
-            associated: bool = None, blocked: bool = None,
+            associated: bool = None, pending: bool = None, blocked: bool = None,
     ) -> list[Identity]:
         response = self.api.query(
             name='identities',
             variables=_filter_variables(
                 ('providerId', 'String', provider_id),
                 ('name_Icontains', 'String', name_contains),
                 ('email_Icontains', 'String', email_contains),
                 ('user_Id', 'String', user.id if isinstance(user, User) else user),
                 ('associated', 'Boolean', associated),
+                ('pending', 'Boolean', pending),
                 ('blocked', 'Boolean', blocked),
             ),
             body='edges { node { ' + Identity.body() + ' } }',
         )
         return [Identity.from_dict(edge['node']) for edge in response['edges']]
 
     def register_identity(self, provider_id: str, id_token: str) -> Identity:
```

### Comparing `qotto_auth_client-2.2.2a0/PKG-INFO` & `qotto_auth_client-2.2.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qotto-auth-client
-Version: 2.2.2a0
+Version: 2.2.2a1
 Summary: Qotto/QottoAuthClient
 Author: Qotto Dev Team
 Author-email: dev@qotto.net
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

