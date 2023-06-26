# Comparing `tmp/EncroX-1.0.5.tar.gz` & `tmp/EncroX-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EncroX-1.0.5.tar", last modified: Sat Jun 24 08:57:36 2023, max compression
+gzip compressed data, was "EncroX-1.0.6.tar", last modified: Mon Jun 26 13:47:59 2023, max compression
```

## Comparing `EncroX-1.0.5.tar` & `EncroX-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 08:57:36.496373 EncroX-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-06-24 08:57:36.482862 EncroX-1.0.5/EncroX/
--rw-rw-rw-   0        0        0       48 2023-06-23 18:24:36.000000 EncroX-1.0.5/EncroX/__init__.py
--rw-rw-rw-   0        0        0     2975 2023-06-23 18:24:36.000000 EncroX-1.0.5/EncroX/aes.py
--rw-rw-rw-   0        0        0      861 2023-06-23 18:24:36.000000 EncroX-1.0.5/EncroX/aes.pyi
--rw-rw-rw-   0        0        0     5011 2023-06-24 08:55:15.000000 EncroX-1.0.5/EncroX/ecc.py
--rw-rw-rw-   0        0        0     1445 2023-06-23 18:24:36.000000 EncroX-1.0.5/EncroX/ecc.pyi
--rw-rw-rw-   0        0        0     5191 2023-06-24 08:15:30.000000 EncroX-1.0.5/EncroX/rsa.py
--rw-rw-rw-   0        0        0     1389 2023-06-23 18:24:36.000000 EncroX-1.0.5/EncroX/rsa.pyi
-drwxrwxrwx   0        0        0        0 2023-06-24 08:57:36.496373 EncroX-1.0.5/EncroX.egg-info/
--rw-rw-rw-   0        0        0     7726 2023-06-24 08:57:36.000000 EncroX-1.0.5/EncroX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-06-24 08:57:36.000000 EncroX-1.0.5/EncroX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 08:57:36.000000 EncroX-1.0.5/EncroX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-24 08:57:36.000000 EncroX-1.0.5/EncroX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 08:57:36.000000 EncroX-1.0.5/EncroX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35184 2023-06-23 18:04:53.000000 EncroX-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     7726 2023-06-24 08:57:36.496373 EncroX-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6970 2023-06-24 05:25:29.000000 EncroX-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 08:57:36.496373 EncroX-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-06-24 08:55:43.000000 EncroX-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 13:47:59.383264 EncroX-1.0.6/
+drwxrwxrwx   0        0        0        0 2023-06-26 13:47:59.373133 EncroX-1.0.6/EncroX/
+-rw-rw-rw-   0        0        0       48 2023-06-23 18:24:36.000000 EncroX-1.0.6/EncroX/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-06-23 18:24:36.000000 EncroX-1.0.6/EncroX/aes.py
+-rw-rw-rw-   0        0        0      861 2023-06-23 18:24:36.000000 EncroX-1.0.6/EncroX/aes.pyi
+-rw-rw-rw-   0        0        0     5087 2023-06-26 13:34:31.000000 EncroX-1.0.6/EncroX/ecc.py
+-rw-rw-rw-   0        0        0     1445 2023-06-23 18:24:36.000000 EncroX-1.0.6/EncroX/ecc.pyi
+-rw-rw-rw-   0        0        0     5191 2023-06-24 08:15:30.000000 EncroX-1.0.6/EncroX/rsa.py
+-rw-rw-rw-   0        0        0     1389 2023-06-23 18:24:36.000000 EncroX-1.0.6/EncroX/rsa.pyi
+drwxrwxrwx   0        0        0        0 2023-06-26 13:47:59.380019 EncroX-1.0.6/EncroX.egg-info/
+-rw-rw-rw-   0        0        0     7726 2023-06-26 13:47:59.000000 EncroX-1.0.6/EncroX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-26 13:47:59.000000 EncroX-1.0.6/EncroX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 13:47:59.000000 EncroX-1.0.6/EncroX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-26 13:47:59.000000 EncroX-1.0.6/EncroX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-26 13:47:59.000000 EncroX-1.0.6/EncroX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35184 2023-06-23 18:04:53.000000 EncroX-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     7726 2023-06-26 13:47:59.381263 EncroX-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6970 2023-06-24 05:25:29.000000 EncroX-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 13:47:59.383264 EncroX-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      751 2023-06-26 13:47:31.000000 EncroX-1.0.6/setup.py
```

### Comparing `EncroX-1.0.5/EncroX/aes.py` & `EncroX-1.0.6/EncroX/aes.py`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.5/EncroX/aes.pyi` & `EncroX-1.0.6/EncroX/aes.pyi`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.5/EncroX/ecc.py` & `EncroX-1.0.6/EncroX/ecc.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,18 @@
     # 检查 data 类型并进行必要的转换
     if isinstance(data, str):
         data = data.encode()
         data_str = True
     else:
         data_str = False
 
-    shared_key = private_key.exchange(ec.ECDH(), public_key)
+    try:
+        shared_key = private_key.exchange(ec.ECDH(), public_key)
+    except:
+        raise Exception("密钥curve不匹配")
 
     # Hash the shared key to get a 32-byte (256-bit) key
     shared_key_hash = hashes.Hash(hashes.SHA256())
     shared_key_hash.update(shared_key)
     derived_key = base64.urlsafe_b64encode(shared_key_hash.finalize())
 
     f = Fernet(derived_key)
```

### Comparing `EncroX-1.0.5/EncroX/ecc.pyi` & `EncroX-1.0.6/EncroX/ecc.pyi`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.5/EncroX/rsa.py` & `EncroX-1.0.6/EncroX/rsa.py`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.5/EncroX/rsa.pyi` & `EncroX-1.0.6/EncroX/rsa.pyi`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.5/EncroX.egg-info/PKG-INFO` & `EncroX-1.0.6/EncroX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EncroX
-Version: 1.0.5
+Version: 1.0.6
 Summary: EncroX是一个强大的加密拓展工具，旨在为您的应用程序和系统提供可靠的加密和解密功能。通过集成各种密码学算法和密钥管理方法，EncroX使您能够轻松地进行数据加密、解密和安全通信。
 Home-page: https://github.com/KindLittleTurtle/EncroX
 Author: 核善的小兲
 Author-email: hsdxt@mwtour.cn
 License: AGPL3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `EncroX-1.0.5/LICENSE` & `EncroX-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.5/PKG-INFO` & `EncroX-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EncroX
-Version: 1.0.5
+Version: 1.0.6
 Summary: EncroX是一个强大的加密拓展工具，旨在为您的应用程序和系统提供可靠的加密和解密功能。通过集成各种密码学算法和密钥管理方法，EncroX使您能够轻松地进行数据加密、解密和安全通信。
 Home-page: https://github.com/KindLittleTurtle/EncroX
 Author: 核善的小兲
 Author-email: hsdxt@mwtour.cn
 License: AGPL3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `EncroX-1.0.5/README.md` & `EncroX-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `EncroX-1.0.5/setup.py` & `EncroX-1.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='EncroX',
-    version='1.0.5',
+    version='1.0.6',
     packages=['EncroX'],
     url='https://github.com/KindLittleTurtle/EncroX',
     license='AGPL3.0',
     author='核善的小兲',
     author_email='hsdxt@mwtour.cn',
     description='EncroX是一个强大的加密拓展工具，旨在为您的应用程序和系统提供可靠的加密和解密功能。通过集成各种密码学算法和密钥管理方法，EncroX使您能够轻松地进行数据加密、解密和安全通信。',
     install_requires=['cryptography'],
```

