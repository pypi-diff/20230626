# Comparing `tmp/yop-python-sdk-4.2.2.tar.gz` & `tmp/yop-python-sdk-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yop-python-sdk-4.2.2.tar", last modified: Fri Jun 24 03:57:36 2022, max compression
+gzip compressed data, was "yop-python-sdk-4.2.3.tar", last modified: Mon Jun 26 12:17:04 2023, max compression
```

## Comparing `yop-python-sdk-4.2.2.tar` & `yop-python-sdk-4.2.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.220846 yop-python-sdk-4.2.2/
--rw-r--r--   0 yp-21074   (501) staff       (20)    11357 2021-10-08 03:08:42.000000 yop-python-sdk-4.2.2/LICENSE
--rw-r--r--   0 yp-21074   (501) staff       (20)     3639 2022-06-24 03:57:36.220705 yop-python-sdk-4.2.2/PKG-INFO
--rw-r--r--   0 yp-21074   (501) staff       (20)       38 2022-06-24 03:57:36.220897 yop-python-sdk-4.2.2/setup.cfg
--rw-r--r--   0 yp-21074   (501) staff       (20)     1706 2022-06-24 03:56:13.000000 yop-python-sdk-4.2.2/setup.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.215382 yop-python-sdk-4.2.2/tests/
--rw-r--r--   0 yp-21074   (501) staff       (20)     2291 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/tests/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)      817 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/tests/assertion.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     1393 2022-06-20 08:41:22.000000 yop-python-sdk-4.2.2/tests/conftest.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     7555 2022-06-20 09:00:12.000000 yop-python-sdk-4.2.2/tests/test_download.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     3594 2022-06-20 08:27:30.000000 yop-python-sdk-4.2.2/tests/test_get.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     4443 2022-06-20 08:27:33.000000 yop-python-sdk-4.2.2/tests/test_post_json.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     9691 2022-06-20 08:41:50.000000 yop-python-sdk-4.2.2/tests/test_rsa_envelope.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     4183 2022-06-20 08:14:34.000000 yop-python-sdk-4.2.2/tests/test_rsaencryptor.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     1468 2022-06-20 08:14:30.000000 yop-python-sdk-4.2.2/tests/test_smencryptor.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     4701 2022-06-20 10:51:56.000000 yop-python-sdk-4.2.2/tests/test_upload.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.215492 yop-python-sdk-4.2.2/yop_python_sdk/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/__init__.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.216149 yop-python-sdk-4.2.2/yop_python_sdk/auth/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/auth/__init__.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.216486 yop-python-sdk-4.2.2/yop_python_sdk/auth/certloader/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/auth/certloader/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)      811 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/auth/certloader/yopcertloader.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.216850 yop-python-sdk-4.2.2/yop_python_sdk/auth/v3signer/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/auth/v3signer/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)    11321 2022-06-20 10:47:46.000000 yop-python-sdk-4.2.2/yop_python_sdk/auth/v3signer/auth.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     1793 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/auth/v3signer/credentials.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.217271 yop-python-sdk-4.2.2/yop_python_sdk/client/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 08:17:08.000000 yop-python-sdk-4.2.2/yop_python_sdk/client/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     4533 2022-06-20 08:26:08.000000 yop-python-sdk-4.2.2/yop_python_sdk/client/client_config.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     4317 2022-06-20 08:41:50.000000 yop-python-sdk-4.2.2/yop_python_sdk/client/yop_client_config.py
--rw-r--r--   0 yp-21074   (501) staff       (20)    12659 2022-06-24 03:56:13.000000 yop-python-sdk-4.2.2/yop_python_sdk/client/yopclient.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.217608 yop-python-sdk-4.2.2/yop_python_sdk/security/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     1699 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/crc64.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     6509 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/crc64_combine.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.218230 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     3023 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/curve.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     5930 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/math.py
--rw-r--r--   0 yp-21074   (501) staff       (20)      382 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/point.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     4855 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/privateKey.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     4631 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/publicKey.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.218886 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)      550 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/base.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     1634 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/binary.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     3093 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/compatibility.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     8092 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/der.py
--rw-r--r--   0 yp-21074   (501) staff       (20)      379 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/integer.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.219354 yop-python-sdk-4.2.2/yop_python_sdk/security/encryptor/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/encryptor/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)      895 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/encryptor/encryptor.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     5538 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/encryptor/rsaencryptor.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     2824 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/encryptor/smencryptor.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.220028 yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/__init__.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     1323 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/func.py
--rw-r--r--   0 yp-21074   (501) staff       (20)    12916 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/sm2.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     5195 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/sm3.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     8615 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/sm4.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     6467 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/utils.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.220524 yop-python-sdk-4.2.2/yop_python_sdk/utils/
--rw-r--r--   0 yp-21074   (501) staff       (20)       24 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/utils/__init__.py
--rw-r-----   0 yp-21074   (501) staff       (20)     4283 2022-06-24 03:55:17.000000 yop-python-sdk-4.2.2/yop_python_sdk/utils/yop_cashier_util.py
--rw-r--r--   0 yp-21074   (501) staff       (20)      849 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/utils/yop_logger.py
--rw-r--r--   0 yp-21074   (501) staff       (20)     2149 2022-06-20 07:41:28.000000 yop-python-sdk-4.2.2/yop_python_sdk/utils/yop_security_utils.py
-drwxr-xr-x   0 yp-21074   (501) staff       (20)        0 2022-06-24 03:57:36.216038 yop-python-sdk-4.2.2/yop_python_sdk.egg-info/
--rw-r--r--   0 yp-21074   (501) staff       (20)     3639 2022-06-24 03:57:35.000000 yop-python-sdk-4.2.2/yop_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yp-21074   (501) staff       (20)     2059 2022-06-24 03:57:36.000000 yop-python-sdk-4.2.2/yop_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yp-21074   (501) staff       (20)        1 2022-06-24 03:57:36.000000 yop-python-sdk-4.2.2/yop_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yp-21074   (501) staff       (20)      121 2022-06-24 03:57:36.000000 yop-python-sdk-4.2.2/yop_python_sdk.egg-info/requires.txt
--rw-r--r--   0 yp-21074   (501) staff       (20)       21 2022-06-24 03:57:36.000000 yop-python-sdk-4.2.2/yop_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.607091 yop-python-sdk-4.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/test_post_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/test_rsa_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/test_rsaencryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/test_smencryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.607091 yop-python-sdk-4.2.3/yop_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.607091 yop-python-sdk-4.2.3/yop_python_sdk/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.607091 yop-python-sdk-4.2.3/yop_python_sdk/auth/certloader/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/auth/certloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/auth/certloader/yopcertloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.607091 yop-python-sdk-4.2.3/yop_python_sdk/auth/v3signer/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/auth/v3signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11321 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/auth/v3signer/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/auth/v3signer/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/yop_python_sdk/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/client/client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/client/yop_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14575 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/client/yopclient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/yop_python_sdk/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/crc64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/crc64_combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/privateKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/publicKey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/der.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/integer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/yop_python_sdk/security/encryptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/encryptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/encryptor/encryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/encryptor/rsaencryptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/encryptor/smencryptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.611091 yop-python-sdk-4.2.3/yop_python_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/utils/yop_cashier_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/utils/yop_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-26 12:16:53.000000 yop-python-sdk-4.2.3/yop_python_sdk/utils/yop_security_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 12:17:04.607091 yop-python-sdk-4.2.3/yop_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-26 12:17:04.000000 yop-python-sdk-4.2.3/yop_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-26 12:17:04.000000 yop-python-sdk-4.2.3/yop_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 12:17:04.000000 yop-python-sdk-4.2.3/yop_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 12:17:04.000000 yop-python-sdk-4.2.3/yop_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 12:17:04.000000 yop-python-sdk-4.2.3/yop_python_sdk.egg-info/top_level.txt
```

### Comparing `yop-python-sdk-4.2.2/LICENSE` & `yop-python-sdk-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/PKG-INFO` & `yop-python-sdk-4.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: yop-python-sdk
-Version: 4.2.2
+Version: 4.2.3
 Summary: YOP SDK based on the YOP Common Runtime
 Home-page: https://github.com/yop-platform/yop-python-sdk
 Author: YOP Team
 Author-email: yop@yeepay.com
 License: Apache License
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yop-python-sdk
 
 本软件是易宝开放平台（YOP）的 Python 语言 SDK，力争同时支持 Python2/3。
 
 ## Installation 安装方法
 
 ### Minimum Requirements 最小系统要求
 
-- Python 2.7+
 - Python 3.5+
+- Python 2.7+ (不能保证停止维护的Python版本有效，请参考https://www.python.org/doc/sunset-python-2/)
 
 ### Install from PyPI 从 PyPI 安装
 
 ## 生成虚拟环境
 
 以 virtualenv 为例
 
@@ -46,34 +48,30 @@
 
 ```shell
 # rm -rf ~/python3
 /usr/bin/env /usr/bin/python3 -m virtualenv ~/python3
 source ~/python3/bin/activate
 ```
 
-### For python2
-
-```shell
-# rm -rf ~/python2
-/usr/bin/env /usr/bin/python -m virtualenv -p ~/python2
-source ~/python2/bin/activate
-```
-
 ## 安装 yop-python-sdk
 
 ### 从仓库安装最新版本
 
 ```shell
 python -m pip install yop-python-sdk
+
+# crypto 相关的报错如何解决
+python -m pip uninstall crypto pycrypto pycryptodome yop-python-sdk
+python -m pip install pycryptodome
 ```
 
 ### 从指定仓库安装指定的版本
 
 ```shell
-python -m pip install --upgrade --index-url https://pypi.org/simple yop-python-sdk==3.3.12
+python -m pip install --upgrade --index-url https://pypi.org/simple yop-python-sdk==4.2.3
 ```
 
 ### Install from source 从源码安装(不推荐)
 
 ```shell
 python -m pip install git+https://github.com/yop-platform/yop-python-sdk.git
 ```
@@ -123,21 +121,14 @@
 }
 credentials = YopCredentials(appKey='<appKey>', cert_type='SM2|RSA2048', priKey='<私钥>')
 res = client.get(api=api, params=params, credentials=credentials)
 ```
 
 更多用法，请参考 test 目录下面的单元测试。
 
-### crypto 相关的报错如何解决
-
-```shell
-python -m pip uninstall crypto pycrypto pycryptodome yop-python-sdk
-python -m pip install pycryptodome
-```
-
 ### ImportError: bad magic number in 'xxx'
 
 ```shell
 rm -Rf **/*.pyc
 ```
 
 ## Contributing
```

### Comparing `yop-python-sdk-4.2.2/setup.py` & `yop-python-sdk-4.2.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages, setup
 
 with open("README.MD", "r") as f:
     long_description = f.read()
 
 setup(
     name='yop-python-sdk',
-    version='4.2.2',
+    version='4.2.3',
     description='YOP SDK based on the YOP Common Runtime',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='YOP Team',
     author_email='yop@yeepay.com',
     url='https://github.com/yop-platform/yop-python-sdk',
     license='Apache License',
@@ -22,26 +22,29 @@
     packages=find_packages(),
     classifiers=[
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Natural Language :: Chinese (Simplified)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries'
     ],
     # 务必删除 crypto 和 pycrypto
     # pip3 uninstall crypto
     # pip3 uninstall pycrypto
     # pip3 install pycryptodome
     install_requires=[
+        'crcmod>=1.7',
         'future>=0.18.2',
         'pycryptodome>=3.14.1',
         'pyOpenSSL>=22.0.0',
         'python-dateutil>=2.8.2',
         'requests_toolbelt>=0.9.1',
         'simplejson>=3.17.6',
     ],
```

### Comparing `yop-python-sdk-4.2.2/tests/__init__.py` & `yop-python-sdk-4.2.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/tests/assertion.py` & `yop-python-sdk-4.2.3/tests/assertion.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/tests/conftest.py` & `yop-python-sdk-4.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/tests/test_download.py` & `yop-python-sdk-4.2.3/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/tests/test_get.py` & `yop-python-sdk-4.2.3/tests/test_get.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,7 +60,29 @@
         params = {
             'name': '张三',
             'bankCardNo': '6214830128005989',
             'goods': ['苹果', '香蕉', '草莓']
         }
         res = client.get(api, params)
         assertion.failure(res, '40042')
+
+    def test_get_with_http_param(self, client):
+        """
+        Run the get test with http parameters.
+
+        Args:
+            self: write your description
+            client: write your description
+        """
+        api = '/rest/v1.0/cnppay/bank-limit/query'
+        params = {'merchantNo': '10000470992'}
+        http_param = {'connect_timeout': 1000,
+                      'read_timeout': 1000}
+        res = client.get(api, params, http_param=http_param)
+        if 'prod' == client.env:
+            if 'sm' == client.cert_type:
+                assertion.failure(res, '40029')
+            else:
+                assertion.success(res)
+                assert '00000' == res['result']['code']
+        else:
+            assert '40042' == res['code']
```

### Comparing `yop-python-sdk-4.2.2/tests/test_post_json.py` & `yop-python-sdk-4.2.3/tests/test_post_json.py`

 * *Files 19% similar despite different names*

```diff
@@ -84,7 +84,27 @@
             '10000470992',
             'orderId': ['苹果', '香蕉', '草莓'],
             'productInfo':
             '[{\"productCode\":\"MERCHANT_SCAN_ALIPAY_OFFLINE\",\"rateType\":\"SINGLE_PERCENT\",\"percentRate\":\"0.1\"},{\"productCode\":\"MERCHANT_SCAN_UNIONPAY_CREDIT\",\"rateType\":\"SINGLE_FIXED\",\"fixedRate\":\"1\"}]'
         }
         res = client.post_json(api, params)
         assertion.failure(res, '40020')
+
+    def test_post_json_with_http_param(self, client):
+        """
+        Test POST JSON response with http parameters.
+
+        Args:
+            self: write your description
+            client: write your description
+        """
+        api = '/rest/v1.0/std/eaccount/topupquery'
+        params = {
+            'parentMerchantNo': '10000470992',
+            'merchantNo': '10000470992',
+            'orderId': '12345'
+        }
+        http_param = {'connect_timeout': 1000,
+                      'read_timeout': 1000}
+        res = client.post_json(api, params, http_param=http_param)
+        if 'qa' == client.env and '40020' != res.get('code'):
+            assertion.success(res)
```

### Comparing `yop-python-sdk-4.2.2/tests/test_rsa_envelope.py` & `yop-python-sdk-4.2.3/tests/test_rsa_envelope.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/tests/test_rsaencryptor.py` & `yop-python-sdk-4.2.3/tests/test_rsaencryptor.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/tests/test_smencryptor.py` & `yop-python-sdk-4.2.3/tests/test_smencryptor.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/tests/test_upload.py` & `yop-python-sdk-4.2.3/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/auth/certloader/yopcertloader.py` & `yop-python-sdk-4.2.3/yop_python_sdk/auth/certloader/yopcertloader.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/auth/v3signer/auth.py` & `yop-python-sdk-4.2.3/yop_python_sdk/auth/v3signer/auth.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/auth/v3signer/credentials.py` & `yop-python-sdk-4.2.3/yop_python_sdk/auth/v3signer/credentials.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/client/client_config.py` & `yop-python-sdk-4.2.3/yop_python_sdk/client/client_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from yop_python_sdk.security.ecdsa.privateKey import PrivateKey
 import OpenSSL
 from yop_python_sdk.auth.v3signer.credentials import YopCredentials
 import yop_python_sdk.utils.yop_logger as yop_logger
 from Crypto.PublicKey import RSA
 
 
-class ClientConfig:
+class ClientConfig(object):
 
     def __init__(self):
         """
         Initializes the SDK.
 
         Args:
             self: write your description
@@ -67,14 +67,38 @@
                 yop_public_key = PublicKey.fromPem(yop_public_key).toStr()
         else:
             self.logger.warn('暂时不支持的密钥类型 {}'.format(store_type))
             yop_public_key = None
 
         return yop_public_key, cert_type, serial_no
 
+    def _parse_http_client(self, connect_timeout, read_timeout, max_conn_total, max_conn_per_route):
+        """
+        Parse the http client key from a config file.
+
+        Args:
+            self: write your description
+            config: write your description
+        """
+        try:
+            connect_timeout = self.check_is_number(connect_timeout)
+            read_timeout = self.check_is_number(read_timeout)
+            max_conn_total = self.check_is_number(max_conn_total)
+            max_conn_per_route = self.check_is_number(max_conn_per_route)
+        except Exception as e:
+            self.logger.error(e)
+            raise e
+        return connect_timeout, read_timeout, max_conn_total, max_conn_per_route
+
+    def check_is_number(self, value):
+        if (isinstance(value, int) or isinstance(value, float)) and value > 0:
+            return value
+        else:
+            raise Exception("value must be int or float type and > 0, value: {}".format(value))
+
     def cer_analysis(self, ceradd):
         '''
         解析证书文件
         '''
         file = open(ceradd)
         file_context = file.read()
         cert = OpenSSL.crypto.load_certificate(OpenSSL.crypto.FILETYPE_PEM,
```

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/client/yop_client_config.py` & `yop-python-sdk-4.2.3/yop_python_sdk/client/yop_client_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -55,44 +55,78 @@
                     app_key, isv_private_key)
                 credentials_dict[credentials.appKey] = credentials
                 # 仅支持一个私钥，避免请求时不知道用哪个私钥签名
                 if credentials is not None:
                     sdk_config['credentials'] = credentials_dict
                     break
 
+            # http client
+            http_client_dict = sdk_config['http_client']
+            connect_timeout, read_timeout, max_conn_total, max_conn_per_route = self._parse_http_client(http_client_dict)
+            http_client_dict['connect_timeout'] = connect_timeout
+            http_client_dict['read_timeout'] = read_timeout
+            http_client_dict['max_conn_total'] = max_conn_total
+            http_client_dict['max_conn_per_route'] = max_conn_per_route
+            sdk_config['http_client'] = http_client_dict
+
         return sdk_config
 
     def _parse_isv_private_key(self, appKey, config):
         """
         Parse the isv private key and return YopCredentials object.
 
         Args:
             self: write your description
             appKey: write your description
             config: write your description
         """
         store_type = config.get('store_type', 'string')
         cert_type = config.get('cert_type', 'RSA2048')
         appKey = config.get('app_key', appKey)
-        return super()._parse_isv_pri_key(appKey, config['value'], store_type,
-                                          cert_type)
+        return super(YopClientConfig, self)._parse_isv_pri_key(appKey, config['value'], store_type,
+                                                               cert_type)
 
     def _parse_yop_public_key(self, config):
         """
         Parse the yop public key from a config file.
 
         Args:
             self: write your description
             config: write your description
         """
         store_type = config.get('store_type', 'string')
         cert_type = config.get('cert_type', 'RSA2048')
         serial_no = config.get('serial_no', 'unknown')
-        return super()._parse_yop_pub_key(config['value'], store_type,
-                                          cert_type, serial_no)
+        return super(YopClientConfig, self)._parse_yop_pub_key(config['value'],
+                                                               store_type,
+                                                               cert_type,
+                                                               serial_no)
+
+    def _parse_http_client(self, config):
+        """
+        Parse the http client from a config file.
+
+        Args:
+            self: write your description
+            config: write your description
+        """
+        connect_timeout = config.get('connect_timeout', 10000)
+        read_timeout = config.get('read_timeout', 30000)
+        max_conn_total = config.get('max_conn_total', 200)
+        max_conn_per_route = config.get('max_conn_per_route', 100)
+        return super(YopClientConfig, self)._parse_http_client(connect_timeout,
+                                                               read_timeout,
+                                                               max_conn_total,
+                                                               max_conn_per_route)
+
+    def get_http_client(self):
+        """
+        docstring
+        """
+        return self.sdk_config['http_client']
 
     def get_server_root(self):
         """
         docstring
         """
         return self.sdk_config['server_root']
```

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/client/yopclient.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/sm2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,341 +1,347 @@
 # -*- coding: utf-8 -*-
 
-import os
-from yop_python_sdk.security.encryptor.rsaencryptor import RsaEncryptor
-from yop_python_sdk.security.encryptor.smencryptor import SmEncryptor
-import simplejson
-from simplejson.decoder import JSONDecodeError
-import platform
-import locale
-from yop_python_sdk.auth.v3signer.auth import SigV3AuthProvider
-import requests
-from requests_toolbelt.multipart.encoder import MultipartEncoder
-from yop_python_sdk.client.yop_client_config import YopClientConfig
-import yop_python_sdk.utils.yop_logger as yop_logger
-
-SDK_VERSION = '4.2.2'
-platform_info = platform.platform().split("-")
-python_compiler = platform.python_compiler().split(' ')
-locale_info = locale.getdefaultlocale()
-locale_lang = locale_info[0]
-if locale_lang is None:
-    locale_lang = 'zh-CN'
-USER_AGENT = "/".join([
-    'python', SDK_VERSION, platform_info[0], platform_info[1],
-    python_compiler[0], python_compiler[1],
-    platform.python_version(), locale_lang
-])
-
-
-class YopClient:
-    clientConfig = None
-
-    def __init__(self, clientConfig=None, cert_type=None, env=None):
-        """
-        Yop的
-
-        Args:
-            self: write your description
-            clientConfig: write your description
-            cert_type: write your description
-            env: write your description
-        """
-        self.logger = yop_logger.get_logger()
-        self.env = env
-        self.cert_type = cert_type
-        if clientConfig is None:
-            clientConfig = YopClientConfig()
-
-        # 同时支持RSA、SM两种加密机
-        self.yop_encryptor_dict = {}
-        for cert_type, yop_public_key_dict in clientConfig.sdk_config[
-                'yop_public_key'].items():
-            if len(yop_public_key_dict) > 0:
-                self.yop_encryptor_dict[cert_type] = self.get_encryptor(
-                    cert_type, yop_public_key_dict)
-
-        self.clientConfig = clientConfig
-        self.authProvider = SigV3AuthProvider(self.yop_encryptor_dict)
-
-    def get_encryptor(self, cert_type, yop_public_key_dict):
-        """
-        Returns the appropriate encryptor depending on the cert_type.
+import binascii
+from . import sm3, func
+
+# 选择素域，设置椭圆曲线参数
+
+default_ecc_table = {
+    'n': 'FFFFFFFEFFFFFFFFFFFFFFFFFFFFFFFF7203DF6B21C6052B53BBF40939D54123',
+    'p': 'FFFFFFFEFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF00000000FFFFFFFFFFFFFFFF',
+    'g': '32c4ae2c1f1981195f9904466a39c9948fe30bbff2660be1715a4589334c74c7'
+         'bc3736a2f4f6779c59bdcee36b692153d0a9877cc62a474002df32e52139f0a0',
+    'a': 'FFFFFFFEFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFFF00000000FFFFFFFFFFFFFFFC',
+    'b': '28E9FA9E9D9F5E344D5A9E4BCF6509A7F39789F515AB8F92DDBCBD414D940E93',
+}
+
+
+class CryptSM2(object):
+    def __init__(self, ecc_table=default_ecc_table):
+        """
+        Initializes the class with the ecc_table
 
         Args:
             self: write your description
-            cert_type: write your description
-            yop_public_key_dict: write your description
+            ecc_table: write your description
+            default_ecc_table: write your description
         """
-        if 'SM2' == cert_type:
-            return SmEncryptor(public_key_dict=yop_public_key_dict)
-        else:
-            return RsaEncryptor(
-                public_key=list(yop_public_key_dict.values())[0])
+        self.para_len = len(ecc_table['n'])
+        self.ecc_a3 = (
+            int(ecc_table['a'], base=16) + 3) % int(ecc_table['p'], base=16)
+        self.ecc_table = ecc_table
 
-    def get(self, api, query_params={}, credentials=None, basePath=None):
+    def _kg(self, k, Point):  # kP运算
         """
-        Make a GET request to the API.
+        Kruskal s k - th point
 
         Args:
             self: write your description
-            api: write your description
-            query_params: write your description
-            credentials: write your description
-            basePath: write your description
-        """
-        if credentials is None:
-            credentials = self.clientConfig.get_credentials()
-
-        if basePath is None:
-            basePath = self.clientConfig.get_server_root()
-
-        authorization = self.authProvider.new_authenticator()
-        headers = authorization.generate_signature(url=api,
-                                                   http_method='GET',
-                                                   query_params=query_params,
-                                                   credentials=credentials)
-        headers['user-agent'] = USER_AGENT
-
-        # for k, v in query_params.items():
-        #         query_params[k] = quote(str(v), 'utf-8')
-
-        url = ''.join([basePath, api])
-        res = self._get_request(url,
-                                query_params=query_params,
-                                headers=headers)
-        self.logger.info(
-            'request:\nGET {}\nheaders:{}\nparams:{}\nresponse:\nheaders:{}\nbody:{}\ntime:{}ms\n'
-            .format(url, headers, query_params, res.headers, res.text,
-                    res.elapsed.microseconds / 1000.))
-
-        if res.status_code == 400:
-            raise Exception("isv.service.not-exists")
-
-        authorization._verify_res(res, credentials.get_cert_type())
-        try:
-            return simplejson.loads(res.text)
-        except JSONDecodeError as e:
-            self.logger.warn(res.text)
-            raise e
-
-    def download(self,
-                 api,
-                 query_params={},
-                 credentials=None,
-                 basePath=None,
-                 file_path=None):
-        """
-        Downloads the specified API from the server.
-
-        Args:
-            self: write your description
-            api: write your description
-            query_params: write your description
-            credentials: write your description
-            basePath: write your description
-            file_path: write your description
-        """
-        if credentials is None:
-            credentials = self.clientConfig.get_credentials()
-
-        if basePath is None:
-            basePath = self.clientConfig.get_server_root()
-
-        authorization = self.authProvider.new_authenticator()
-        headers = authorization.generate_signature(url=api,
-                                                   http_method='GET',
-                                                   query_params=query_params,
-                                                   credentials=credentials)
-        headers['user-agent'] = USER_AGENT
-
-        # for k, v in query_params.items():
-        #         query_params[k] = quote(str(v), 'utf-8')
-
-        url = ''.join([basePath, api])
-        res = self._get_request(url,
-                                query_params=query_params,
-                                headers=headers)
-        self.logger.debug(
-            'request:\nGET {}\nheaders:{}\nparams:{}\nresponse:\nheaders:{}\ntime:{}ms\n'
-            .format(url, headers, query_params, res.headers,
-                    res.elapsed.microseconds / 1000.))
-
-        if res.status_code == 400:
-            raise Exception("isv.service.not-exists")
-        if res.status_code >= 500:
-            authorization._verify_res(res, credentials.get_cert_type())
-            try:
-                return simplejson.loads(res.text)
-            except JSONDecodeError as e:
-                self.logger.warn(res.text)
-                raise e
-
-        filename = res.headers['Content-Disposition'].split('; ')[1].replace(
-            'filename=', '')
-        filename = filename[filename.rindex('/') + 1:len(filename)]
-
-        try:
-            if not os.path.exists(file_path):
-                os.mkdir(file_path)
-            full_filename = file_path + '/' + filename
-            with open(full_filename, "wb+") as file:
-                file.write(res.content)
-                authorization._verify_res_download(res,
-                                                   credentials.get_cert_type(),
-                                                   file)
-            return 0
-        except OSError as e:
-            self.logger.warn('找不到文件路径:{}'.format(file_path))
-            raise e
-        else:
-            return 1
+            k: write your description
+            Point: write your description
+        """
+        Point = '%s%s' % (Point, '1')
+        mask_str = '8'
+        for i in range(self.para_len - 1):
+            mask_str += '0'
+        mask = int(mask_str, 16)
+        Temp = Point
+        flag = False
+        for n in range(self.para_len * 4):
+            if (flag):
+                Temp = self._double_point(Temp)
+            if (k & mask) != 0:
+                if (flag):
+                    Temp = self._add_point(Temp, Point)
+                else:
+                    flag = True
+                    Temp = Point
+            k = k << 1
+        return self._convert_jacb_to_nor(Temp)
 
-    def _get_request(self, url, query_params={}, headers={}):
+    def _double_point(self, Point):  # 倍点
         """
-        Wrapper for requests. get that handles the headers and returns the response.
+        Returns the double point form of the given point.
 
         Args:
             self: write your description
-            url: write your description
-            query_params: write your description
-            headers: write your description
+            Point: write your description
         """
-        res = requests.get(url=url, params=query_params, headers=headers)
-        return res
+        l = len(Point)
+        len_2 = 2 * self.para_len
+        if l < self.para_len * 2:
+            return None
+        else:
+            x1 = int(Point[0:self.para_len], 16)
+            y1 = int(Point[self.para_len:len_2], 16)
+            if l == len_2:
+                z1 = 1
+            else:
+                z1 = int(Point[len_2:], 16)
+
+            T6 = (z1 * z1) % int(self.ecc_table['p'], base=16)
+            T2 = (y1 * y1) % int(self.ecc_table['p'], base=16)
+            T3 = (x1 + T6) % int(self.ecc_table['p'], base=16)
+            T4 = (x1 - T6) % int(self.ecc_table['p'], base=16)
+            T1 = (T3 * T4) % int(self.ecc_table['p'], base=16)
+            T3 = (y1 * z1) % int(self.ecc_table['p'], base=16)
+            T4 = (T2 * 8) % int(self.ecc_table['p'], base=16)
+            T5 = (x1 * T4) % int(self.ecc_table['p'], base=16)
+            T1 = (T1 * 3) % int(self.ecc_table['p'], base=16)
+            T6 = (T6 * T6) % int(self.ecc_table['p'], base=16)
+            T6 = (self.ecc_a3 * T6) % int(self.ecc_table['p'], base=16)
+            T1 = (T1 + T6) % int(self.ecc_table['p'], base=16)
+            z3 = (T3 + T3) % int(self.ecc_table['p'], base=16)
+            T3 = (T1 * T1) % int(self.ecc_table['p'], base=16)
+            T2 = (T2 * T4) % int(self.ecc_table['p'], base=16)
+            x3 = (T3 - T5) % int(self.ecc_table['p'], base=16)
+
+            if (T5 % 2) == 1:
+                T4 = (T5 + ((T5 + int(self.ecc_table['p'], base=16)) >> 1) - T3) % int(self.ecc_table['p'], base=16)
+            else:
+                T4 = (T5 + (T5 >> 1) - T3) % int(self.ecc_table['p'], base=16)
+
+            T1 = (T1 * T4) % int(self.ecc_table['p'], base=16)
+            y3 = (T1 - T2) % int(self.ecc_table['p'], base=16)
+
+            form = '%%0%dx' % self.para_len
+            form = form * 3
+            return form % (x3, y3, z3)
 
-    def post_json(self, api, post_params={}, credentials=None, basePath=None):
+    def _add_point(self, P1, P2):  # 点加函数，P2点为仿射坐标即z=1，P1为Jacobian加重射影坐标
         """
-        POST the specified post params to the specified API
+        Add a point to the ecc table
 
         Args:
             self: write your description
-            api: write your description
-            post_params: write your description
-            credentials: write your description
-            basePath: write your description
+            P1: write your description
+            P2: write your description
         """
-        return self.post(api,
-                         post_params,
-                         credentials,
-                         basePath=basePath,
-                         json_param=True)
+        len_2 = 2 * self.para_len
+        l1 = len(P1)
+        l2 = len(P2)
+        if (l1 < len_2) or (l2 < len_2):
+            return None
+        else:
+            X1 = int(P1[0:self.para_len], 16)
+            Y1 = int(P1[self.para_len:len_2], 16)
+            if (l1 == len_2):
+                Z1 = 1
+            else:
+                Z1 = int(P1[len_2:], 16)
+            x2 = int(P2[0:self.para_len], 16)
+            y2 = int(P2[self.para_len:len_2], 16)
+
+            T1 = (Z1 * Z1) % int(self.ecc_table['p'], base=16)
+            T2 = (y2 * Z1) % int(self.ecc_table['p'], base=16)
+            T3 = (x2 * T1) % int(self.ecc_table['p'], base=16)
+            T1 = (T1 * T2) % int(self.ecc_table['p'], base=16)
+            T2 = (T3 - X1) % int(self.ecc_table['p'], base=16)
+            T3 = (T3 + X1) % int(self.ecc_table['p'], base=16)
+            T4 = (T2 * T2) % int(self.ecc_table['p'], base=16)
+            T1 = (T1 - Y1) % int(self.ecc_table['p'], base=16)
+            Z3 = (Z1 * T2) % int(self.ecc_table['p'], base=16)
+            T2 = (T2 * T4) % int(self.ecc_table['p'], base=16)
+            T3 = (T3 * T4) % int(self.ecc_table['p'], base=16)
+            T5 = (T1 * T1) % int(self.ecc_table['p'], base=16)
+            T4 = (X1 * T4) % int(self.ecc_table['p'], base=16)
+            X3 = (T5 - T3) % int(self.ecc_table['p'], base=16)
+            T2 = (Y1 * T2) % int(self.ecc_table['p'], base=16)
+            T3 = (T4 - X3) % int(self.ecc_table['p'], base=16)
+            T1 = (T1 * T3) % int(self.ecc_table['p'], base=16)
+            Y3 = (T1 - T2) % int(self.ecc_table['p'], base=16)
+
+            form = '%%0%dx' % self.para_len
+            form = form * 3
+            return form % (X3, Y3, Z3)
 
-    def post(self,
-             api,
-             post_params={},
-             credentials=None,
-             basePath=None,
-             json_param=False):
+    def _convert_jacb_to_nor(self, Point):  # Jacobian加重射影坐标转换成仿射坐标
         """
-        Make a POST request to the API.
+        Convert the point from Jacobian to nor.
 
         Args:
             self: write your description
-            api: write your description
-            post_params: write your description
-            credentials: write your description
-            basePath: write your description
-            json_param: write your description
+            Point: write your description
         """
-        if credentials is None:
-            credentials = self.clientConfig.get_credentials()
+        len_2 = 2 * self.para_len
+        x = int(Point[0:self.para_len], 16)
+        y = int(Point[self.para_len:len_2], 16)
+        z = int(Point[len_2:], 16)
+        z_inv = pow(z, int(self.ecc_table['p'], base=16) - 2, int(self.ecc_table['p'], base=16))
+        z_invSquar = (z_inv * z_inv) % int(self.ecc_table['p'], base=16)
+        z_invQube = (z_invSquar * z_inv) % int(self.ecc_table['p'], base=16)
+        x_new = (x * z_invSquar) % int(self.ecc_table['p'], base=16)
+        y_new = (y * z_invQube) % int(self.ecc_table['p'], base=16)
+        z_new = (z * z_inv) % int(self.ecc_table['p'], base=16)
+        if z_new == 1:
+            form = '%%0%dx' % self.para_len
+            form = form * 2
+            return form % (x_new, y_new)
+        else:
+            return None
 
-        if basePath is None:
-            basePath = self.clientConfig.get_server_root()
+    def sign(self, data, private_key, K):  # 签名函数, data消息的hash，private_key私钥，K随机数，均为16进制字符串
+        """
+        Sign data with private_key.
 
-        authorization = self.authProvider.new_authenticator()
-        headers = authorization.generate_signature(url=api,
-                                                   http_method='POST',
-                                                   post_params=post_params,
-                                                   credentials=credentials,
-                                                   json_param=json_param)
-        headers['user-agent'] = USER_AGENT
+        Args:
+            self: write your description
+            data: write your description
+            private_key: write your description
+            K: write your description
+        """
+        E = binascii.hexlify(data)  # 消息转化为16进制字符串
+        e = int(E, 16)
+
+        d = int(private_key, 16)
+        k = int(K, 16)
+
+        P1 = self._kg(k, self.ecc_table['g'])
+
+        x = int(P1[0:self.para_len], 16)
+        R = ((e + x) % int(self.ecc_table['n'], base=16))
+        if R == 0 or R + k == int(self.ecc_table['n'], base=16):
+            return None
+        d_1 = pow(d + 1, int(self.ecc_table['n'], base=16) - 2, int(self.ecc_table['n'], base=16))
+        S = (d_1 * (k + R) - R) % int(self.ecc_table['n'], base=16)
+        if S == 0:
+            return None
+        else:
+            return '%064x%064x' % (R, S)
 
-        # for k, v in post_params.items():
-        #         post_params[k] = quote(str(v), 'utf-8')
+    def verify(self, Sign, data, public_key):
+        """
+        Verify the signature of data with the public key public_key.
 
-        url = ''.join([basePath, api])
+        Args:
+            self: write your description
+            Sign: write your description
+            data: write your description
+            public_key: write your description
+        """
+        # 验签函数，sign签名r||s，E消息hash，public_key公钥
+        r = int(Sign[0:self.para_len], 16)
+        s = int(Sign[self.para_len:2 * self.para_len], 16)
+        e = int(binascii.hexlify(data), 16)
+        t = (r + s) % int(self.ecc_table['n'], base=16)
+        if t == 0:
+            return 0
 
-        if json_param:
-            headers['content-type'] = 'application/json'
-            data = simplejson.dumps(post_params,
-                                    sort_keys=True,
-                                    indent=4,
-                                    separators=(',', ': '),
-                                    ensure_ascii=True).encode("latin-1")
-            res = self._post_request(url, payload=data, headers=headers)
+        P1 = self._kg(s, self.ecc_table['g'])
+        P2 = self._kg(t, public_key)
+        # print(P1)
+        # print(P2)
+        if P1 == P2:
+            P1 = '%s%s' % (P1, 1)
+            P1 = self._double_point(P1)
         else:
-            res = self._post_request(url, params=post_params, headers=headers)
+            P1 = '%s%s' % (P1, 1)
+            P1 = self._add_point(P1, P2)
+            P1 = self._convert_jacb_to_nor(P1)
 
-        if res.status_code == 400:
-            raise Exception("isv.service.not-exists")
+        x = int(P1[0:self.para_len], 16)
+        return (r == ((e + x) % int(self.ecc_table['n'], base=16)))
 
-        authorization._verify_res(res, credentials.get_cert_type())
-        try:
-            return simplejson.loads(res.text)
-        except JSONDecodeError as e:
-            self.logger.warn(res.text)
-            raise e
-
-    def upload(self, api, post_params={}, credentials=None, basePath=None):
+    def encrypt(self, data, public_key):
         """
-        Upload a new file to Yos.
+        Encrypt data with public_key.
 
         Args:
             self: write your description
-            api: write your description
-            post_params: write your description
-            credentials: write your description
-            basePath: write your description
+            data: write your description
+            public_key: write your description
         """
-        if credentials is None:
-            credentials = self.clientConfig.get_credentials()
-
-        if basePath is None:
-            basePath = self.clientConfig.get_yos_server_root()
-
-        authorization = self.authProvider.new_authenticator()
-        headers = authorization.generate_signature(url=api,
-                                                   http_method='POST',
-                                                   post_params=post_params,
-                                                   credentials=credentials)
-        headers['user-agent'] = USER_AGENT
+        # 加密函数，data消息(bytes)
+        msg = data.hex()  # 消息转化为16进制字符串
+        k = func.random_hex(self.para_len)
+        C1 = self._kg(int(k, 16), self.ecc_table['g'])
+        xy = self._kg(int(k, 16), public_key)
+        x2 = xy[0:self.para_len]
+        y2 = xy[self.para_len:2 * self.para_len]
+        ml = len(msg)
+        t = sm3.sm3_kdf(xy.encode('utf8'), ml / 2)
+        if int(t, 16) == 0:
+            return None
+        else:
+            form = '%%0%dx' % ml
+            C2 = form % (int(msg, 16) ^ int(t, 16))
+            C3 = sm3.sm3_hash([
+                i for i in bytes.fromhex('%s%s%s' % (x2, msg, y2))
+            ])
+            return bytes.fromhex('%s%s%s' % (C1, C3, C2))
 
-        # 封装文件上传编码器
-        multipart = MultipartEncoder(fields=post_params)
-        headers['content-type'] = multipart.content_type
+    def decrypt(self, data, private_key):
+        """
+        Decrypt data with private key.
 
-        url = ''.join([basePath, api])
-        res = self._post_request(url, payload=multipart, headers=headers)
+        Args:
+            self: write your description
+            data: write your description
+            private_key: write your description
+        """
+        # 解密函数，data密文（bytes）
+        data = data.hex()
+        len_2 = 2 * self.para_len
+        len_3 = len_2 + 64
+        C1 = data[0:len_2]
+        # C3 = data[len_2:len_3]
+        C2 = data[len_3:]
+        xy = self._kg(int(private_key, 16), C1)
+        # print('xy = %s' % xy)
+        # x2 = xy[0:self.para_len]
+        # y2 = xy[self.para_len:len_2]
+        cl = len(C2)
+        t = sm3.sm3_kdf(xy.encode('utf8'), cl / 2)
+        if int(t, 16) == 0:
+            return None
+        else:
+            form = '%%0%dx' % cl
+            M = form % (int(C2, 16) ^ int(t, 16))
+            # u = sm3.sm3_hash([
+            #     i for i in bytes.fromhex('%s%s%s' % (x2, M, y2))
+            # ])
+            return bytes.fromhex(M)
+
+    def _sm3_z(self, data, public_key):
+        """
+        SM3WITHSM2 签名规则:  SM2.sign(SM3(Z+MSG)，PrivateKey)
+        其中: z = Hash256(Len(ID) + ID + a + b + xG + yG + xA + yA)
+        """
+        # sm3withsm2 的 z 值
+        z = '0080' + '31323334353637383132333435363738' + \
+            self.ecc_table['a'] + self.ecc_table['b'] + self.ecc_table['g'] + \
+            public_key
+        z = binascii.a2b_hex(z)
+        Za = sm3.sm3_hash(func.bytes_to_list(z))
+        M_ = (Za + binascii.hexlify(data)).encode('utf-8')
+        e = sm3.sm3_hash(func.bytes_to_list(binascii.a2b_hex(M_)))
+        return e
 
-        if res.status_code == 400:
-            raise Exception("isv.service.not-exists")
+    def sign_with_sm3(self, data, public_key, private_key, random_hex_str=None):
+        """
+        Sign data with SM3 - compressed format.
 
-        authorization._verify_res_upload(res, credentials.get_cert_type(),
-                                         post_params)
-        try:
-            return simplejson.loads(res.text)
-        except JSONDecodeError as e:
-            self.logger.warn(res.text)
-            raise e
+        Args:
+            self: write your description
+            data: write your description
+            public_key: write your description
+            private_key: write your description
+            random_hex_str: write your description
+        """
+        sign_data = binascii.a2b_hex(self._sm3_z(data, public_key).encode('utf-8'))
+        if random_hex_str is None:
+            random_hex_str = func.random_hex(self.para_len)
+        sign = self.sign(sign_data, private_key, random_hex_str)  # 16进制
+        return sign
 
-    def _post_request(self, url, payload=None, params=None, headers={}):
+    def verify_with_sm3(self, sign, data, public_key):
         """
-        Perform a POST request.
+        Verify the signature on the data using the SM3 algorithm.
 
         Args:
             self: write your description
-            url: write your description
-            payload: write your description
-            params: write your description
-            headers: write your description
+            sign: write your description
+            data: write your description
+            public_key: write your description
         """
-        res = requests.post(url=url,
-                            headers=headers,
-                            data=payload,
-                            params=params)
-        self.logger.debug(
-            'request:\nPOST {}\nheaders:{}\nparams:{}\nresponse:\nheaders:{}\nbody:{}\ntime:{}ms\n'
-            .format(url, headers, params, res.headers, res.text,
-                    res.elapsed.microseconds / 1000.))
-        return res
+        sign_data = binascii.a2b_hex(self._sm3_z(data, public_key).encode('utf-8'))
+        return self.verify(sign, sign_data, public_key)
```

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/crc64.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/crc64.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/crc64_combine.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/crc64_combine.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/curve.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/curve.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/math.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/math.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/privateKey.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/privateKey.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/publicKey.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/publicKey.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/base.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/base.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/binary.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/binary.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/compatibility.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/ecdsa/utils/der.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/ecdsa/utils/der.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/encryptor/encryptor.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/encryptor/encryptor.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/encryptor/rsaencryptor.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/encryptor/rsaencryptor.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/encryptor/smencryptor.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/encryptor/smencryptor.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/func.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/func.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/sm3.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/sm3.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/sm4.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/sm4.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/security/gmssl/utils.py` & `yop-python-sdk-4.2.3/yop_python_sdk/security/gmssl/utils.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/utils/yop_cashier_util.py` & `yop-python-sdk-4.2.3/yop_python_sdk/utils/yop_cashier_util.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/utils/yop_logger.py` & `yop-python-sdk-4.2.3/yop_python_sdk/utils/yop_logger.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk/utils/yop_security_utils.py` & `yop-python-sdk-4.2.3/yop_python_sdk/utils/yop_security_utils.py`

 * *Files identical despite different names*

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk.egg-info/PKG-INFO` & `yop-python-sdk-4.2.3/yop_python_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: yop-python-sdk
-Version: 4.2.2
+Version: 4.2.3
 Summary: YOP SDK based on the YOP Common Runtime
 Home-page: https://github.com/yop-platform/yop-python-sdk
 Author: YOP Team
 Author-email: yop@yeepay.com
 License: Apache License
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yop-python-sdk
 
 本软件是易宝开放平台（YOP）的 Python 语言 SDK，力争同时支持 Python2/3。
 
 ## Installation 安装方法
 
 ### Minimum Requirements 最小系统要求
 
-- Python 2.7+
 - Python 3.5+
+- Python 2.7+ (不能保证停止维护的Python版本有效，请参考https://www.python.org/doc/sunset-python-2/)
 
 ### Install from PyPI 从 PyPI 安装
 
 ## 生成虚拟环境
 
 以 virtualenv 为例
 
@@ -46,34 +48,30 @@
 
 ```shell
 # rm -rf ~/python3
 /usr/bin/env /usr/bin/python3 -m virtualenv ~/python3
 source ~/python3/bin/activate
 ```
 
-### For python2
-
-```shell
-# rm -rf ~/python2
-/usr/bin/env /usr/bin/python -m virtualenv -p ~/python2
-source ~/python2/bin/activate
-```
-
 ## 安装 yop-python-sdk
 
 ### 从仓库安装最新版本
 
 ```shell
 python -m pip install yop-python-sdk
+
+# crypto 相关的报错如何解决
+python -m pip uninstall crypto pycrypto pycryptodome yop-python-sdk
+python -m pip install pycryptodome
 ```
 
 ### 从指定仓库安装指定的版本
 
 ```shell
-python -m pip install --upgrade --index-url https://pypi.org/simple yop-python-sdk==3.3.12
+python -m pip install --upgrade --index-url https://pypi.org/simple yop-python-sdk==4.2.3
 ```
 
 ### Install from source 从源码安装(不推荐)
 
 ```shell
 python -m pip install git+https://github.com/yop-platform/yop-python-sdk.git
 ```
@@ -123,21 +121,14 @@
 }
 credentials = YopCredentials(appKey='<appKey>', cert_type='SM2|RSA2048', priKey='<私钥>')
 res = client.get(api=api, params=params, credentials=credentials)
 ```
 
 更多用法，请参考 test 目录下面的单元测试。
 
-### crypto 相关的报错如何解决
-
-```shell
-python -m pip uninstall crypto pycrypto pycryptodome yop-python-sdk
-python -m pip install pycryptodome
-```
-
 ### ImportError: bad magic number in 'xxx'
 
 ```shell
 rm -Rf **/*.pyc
 ```
 
 ## Contributing
```

### Comparing `yop-python-sdk-4.2.2/yop_python_sdk.egg-info/SOURCES.txt` & `yop-python-sdk-4.2.3/yop_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

