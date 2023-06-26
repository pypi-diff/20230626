# Comparing `tmp/taktile-auth-0.0.8.tar.gz` & `tmp/taktile-auth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taktile-auth-0.0.8.tar", max compression
+gzip compressed data, was "taktile-auth-0.0.9.tar", max compression
```

## Comparing `taktile-auth-0.0.8.tar` & `taktile-auth-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      689 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/PYPI.md
--rw-r--r--   0        0        0     1004 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      467 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/__init__.py
--rw-r--r--   0        0        0      711 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/assets/resources.yaml
--rw-r--r--   0        0        0     1946 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/assets/roles.yaml
--rw-r--r--   0        0        0     2862 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/client.py
--rw-r--r--   0        0        0      347 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/entities/__init__.py
--rw-r--r--   0        0        0     1547 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/entities/permission.py
--rw-r--r--   0        0        0     2129 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/entities/resource.py
--rw-r--r--   0        0        0     3478 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/entities/role.py
--rw-r--r--   0        0        0      449 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/enums.py
--rw-r--r--   0        0        0      177 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/exceptions.py
--rw-r--r--   0        0        0      426 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/parser/__init__.py
--rw-r--r--   0        0        0     1166 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/parser/utils.py
--rw-r--r--   0        0        0     2288 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/parser/yaml_parsing.py
--rw-r--r--   0        0        0        0 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/py.typed
--rw-r--r--   0        0        0        0 2022-07-06 13:38:20.776107 taktile-auth-0.0.8/taktile_auth/schemas/__init__.py
--rw-r--r--   0        0        0      420 2022-07-06 13:38:20.780107 taktile-auth-0.0.8/taktile_auth/schemas/session.py
--rw-r--r--   0        0        0     2021 2022-07-06 13:38:20.780107 taktile-auth-0.0.8/taktile_auth/schemas/token.py
--rw-r--r--   0        0        0      434 2022-07-06 13:38:20.780107 taktile-auth-0.0.8/taktile_auth/settings.py
--rw-r--r--   0        0        0        0 2022-07-06 13:38:20.780107 taktile-auth-0.0.8/taktile_auth/test_utils/__init__.py
--rw-r--r--   0        0        0     5462 2022-07-06 13:38:20.780107 taktile-auth-0.0.8/taktile_auth/test_utils/jwt_test_utils.py
--rw-r--r--   0        0        0        0 2022-07-06 13:38:20.780107 taktile-auth-0.0.8/taktile_auth/utils/__init__.py
--rw-r--r--   0        0        0     2257 2022-07-06 13:38:20.780107 taktile-auth-0.0.8/taktile_auth/utils/sqlalchemy.py
--rw-r--r--   0        0        0     1569 2022-07-06 13:38:59.904405 taktile-auth-0.0.8/setup.py
--rw-r--r--   0        0        0     1376 2022-07-06 13:38:59.904740 taktile-auth-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      689 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/PYPI.md
+-rw-r--r--   0        0        0     1004 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      467 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/__init__.py
+-rw-r--r--   0        0        0     1521 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/assets/resources.yaml
+-rw-r--r--   0        0        0     1512 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/assets/roles.yaml
+-rw-r--r--   0        0        0     2861 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/client.py
+-rw-r--r--   0        0        0      347 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/entities/__init__.py
+-rw-r--r--   0        0        0     1547 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/entities/permission.py
+-rw-r--r--   0        0        0     2129 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/entities/resource.py
+-rw-r--r--   0        0        0     3478 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/entities/role.py
+-rw-r--r--   0        0        0      449 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/enums.py
+-rw-r--r--   0        0        0      177 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/exceptions.py
+-rw-r--r--   0        0        0      426 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/parser/__init__.py
+-rw-r--r--   0        0        0     1166 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/parser/utils.py
+-rw-r--r--   0        0        0     2288 2022-08-30 11:34:22.953940 taktile-auth-0.0.9/taktile_auth/parser/yaml_parsing.py
+-rw-r--r--   0        0        0        0 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/py.typed
+-rw-r--r--   0        0        0        0 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/schemas/__init__.py
+-rw-r--r--   0        0        0      420 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/schemas/session.py
+-rw-r--r--   0        0        0     2021 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/schemas/token.py
+-rw-r--r--   0        0        0      434 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/settings.py
+-rw-r--r--   0        0        0        0 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/test_utils/__init__.py
+-rw-r--r--   0        0        0     5462 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/test_utils/jwt_test_utils.py
+-rw-r--r--   0        0        0        0 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/utils/__init__.py
+-rw-r--r--   0        0        0     2257 2022-08-30 11:34:22.957940 taktile-auth-0.0.9/taktile_auth/utils/sqlalchemy.py
+-rw-r--r--   0        0        0     1569 2022-08-30 11:35:06.496338 taktile-auth-0.0.9/setup.py
+-rw-r--r--   0        0        0     1376 2022-08-30 11:35:06.496691 taktile-auth-0.0.9/PKG-INFO
```

### Comparing `taktile-auth-0.0.8/PYPI.md` & `taktile-auth-0.0.9/PYPI.md`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/pyproject.toml` & `taktile-auth-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taktile-auth"
-version = "0.0.8"
+version = "0.0.9"
 description = "Auth Package for Taktile"
 readme = "PYPI.md"
 authors = ["Taktile GmbH <devops@taktile.com>"]
 license = "Apache-2.0"
 include = ["taktile_auth/assets/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `taktile-auth-0.0.8/taktile_auth/client.py` & `taktile-auth-0.0.9/taktile_auth/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,21 +59,19 @@
             public_key = self.get_public_key(key=key, kid=kid)
             payload = jwt.decode(
                 token,
                 public_key,
                 algorithms=[ALGORITHM],
                 audience=settings.ENV,
             )
-            token_data = TaktileIdToken(**payload)
-        except jwt.ExpiredSignatureError:
-            raise InvalidAuthException("signature-expired")
-        except (jwt.PyJWTError, ValidationError):
-            raise InvalidAuthException("could-not-validate")
-
-        return token_data
+            return TaktileIdToken(**payload)
+        except jwt.ExpiredSignatureError as exc:
+            raise InvalidAuthException("signature-expired") from exc
+        except (jwt.PyJWTError, ValidationError) as exc:
+            raise InvalidAuthException("could-not-validate") from exc
 
     def get_access(
         self,
         *,
         session_state: SessionState,
         key: t.Optional[str] = None,
         kid: str = "taktile-service",
```

### Comparing `taktile-auth-0.0.8/taktile_auth/entities/permission.py` & `taktile-auth-0.0.9/taktile_auth/entities/permission.py`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/taktile_auth/entities/resource.py` & `taktile-auth-0.0.9/taktile_auth/entities/resource.py`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/taktile_auth/entities/role.py` & `taktile-auth-0.0.9/taktile_auth/entities/role.py`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/taktile_auth/parser/utils.py` & `taktile-auth-0.0.9/taktile_auth/parser/utils.py`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/taktile_auth/parser/yaml_parsing.py` & `taktile-auth-0.0.9/taktile_auth/parser/yaml_parsing.py`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/taktile_auth/schemas/token.py` & `taktile-auth-0.0.9/taktile_auth/schemas/token.py`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/taktile_auth/test_utils/jwt_test_utils.py` & `taktile-auth-0.0.9/taktile_auth/test_utils/jwt_test_utils.py`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/taktile_auth/utils/sqlalchemy.py` & `taktile-auth-0.0.9/taktile_auth/utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `taktile-auth-0.0.8/setup.py` & `taktile-auth-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'PyYAML>=6.0,<7.0',
  'SQLAlchemy==1.3.16',
  'pydantic>=1.8.2,<2.0.0',
  'requests==2.27.1']
 
 setup_kwargs = {
     'name': 'taktile-auth',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Auth Package for Taktile',
     'long_description': '# Taktile Auth\n\n[![pypi status](https://img.shields.io/pypi/v/taktile-auth.svg)](https://pypi.python.org/pypi/taktile-auth)\n[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)\n\nThis package is part of the Taktile ecosystem.\n\nTaktile enables data science teams to industrialize, scale, and maintain machine learning models. Our ML development platform makes it easy to create your own end-to-end ML applications:\n\n- Turn models into auto-scaling APIs in a few lines of code\n- Easily add model tests\n- Create and share model explanations through the Taktile UI\n\nFind more information in our [docs](https://docs.taktile.com).\n',
     'author': 'Taktile GmbH',
     'author_email': 'devops@taktile.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `taktile-auth-0.0.8/PKG-INFO` & `taktile-auth-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taktile-auth
-Version: 0.0.8
+Version: 0.0.9
 Summary: Auth Package for Taktile
 License: Apache-2.0
 Author: Taktile GmbH
 Author-email: devops@taktile.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

