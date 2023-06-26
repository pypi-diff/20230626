# Comparing `tmp/google-auth-2.9.0.tar.gz` & `tmp/google-auth-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-auth-2.9.0.tar", last modified: Wed Jun 29 03:41:23 2022, max compression
+gzip compressed data, was "google-auth-2.9.1.tar", last modified: Tue Jul 12 22:52:23 2022, max compression
```

## Comparing `google-auth-2.9.0.tar` & `google-auth-2.9.1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.803471 google-auth-2.9.0/
--rw-rw-r--   0 root         (0)     1003    11357 2022-06-29 03:38:41.000000 google-auth-2.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      100 2022-06-29 03:38:41.000000 google-auth-2.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3113 2022-06-29 03:41:23.803471 google-auth-2.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     1931 2022-06-29 03:38:41.000000 google-auth-2.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.779471 google-auth-2.9.0/google/
--rw-rw-r--   0 root         (0)     1003      796 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.783471 google-auth-2.9.0/google/auth/
--rw-rw-r--   0 root         (0)     1003      988 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/__init__.py
--rw-rw-r--   0 root         (0)     1003     5272 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/_cloud_sdk.py
--rw-rw-r--   0 root         (0)     1003     6841 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/_credentials_async.py
--rw-rw-r--   0 root         (0)     1003    25524 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/_default.py
--rw-rw-r--   0 root         (0)     1003    11588 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/_default_async.py
--rw-rw-r--   0 root         (0)     1003     7129 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/_helpers.py
--rw-rw-r--   0 root         (0)     1003     5972 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/_jwt_async.py
--rw-rw-r--   0 root         (0)     1003     5879 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/_oauth2client.py
--rw-rw-r--   0 root         (0)     1003     2781 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/_service_account_info.py
--rw-rw-r--   0 root         (0)     1003     6026 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/app_engine.py
--rw-rw-r--   0 root         (0)     1003    30616 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/aws.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.783471 google-auth-2.9.0/google/auth/compute_engine/
--rw-rw-r--   0 root         (0)     1003      804 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/compute_engine/__init__.py
--rw-rw-r--   0 root         (0)     1003     9413 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/compute_engine/_metadata.py
--rw-rw-r--   0 root         (0)     1003    15833 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/compute_engine/credentials.py
--rw-rw-r--   0 root         (0)     1003    13082 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/credentials.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.787471 google-auth-2.9.0/google/auth/crypt/
--rw-rw-r--   0 root         (0)     1003     3356 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/crypt/__init__.py
--rw-rw-r--   0 root         (0)     1003     4564 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/crypt/_cryptography_rsa.py
--rw-rw-r--   0 root         (0)     1003        0 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/crypt/_helpers.py
--rw-rw-r--   0 root         (0)     1003     6069 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/crypt/_python_rsa.py
--rw-rw-r--   0 root         (0)     1003     4203 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/crypt/base.py
--rw-rw-r--   0 root         (0)     1003     5657 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/crypt/es256.py
--rw-rw-r--   0 root         (0)     1003     1109 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/crypt/rsa.py
--rw-rw-r--   0 root         (0)     1003    21157 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/downscoped.py
--rw-rw-r--   0 root         (0)     1003     3156 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/environment_vars.py
--rw-rw-r--   0 root         (0)     1003     1968 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/exceptions.py
--rw-rw-r--   0 root         (0)     1003    20222 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/external_account.py
--rw-rw-r--   0 root         (0)     1003     3652 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/iam.py
--rw-rw-r--   0 root         (0)     1003    11757 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/identity_pool.py
--rw-rw-r--   0 root         (0)     1003    15773 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/impersonated_credentials.py
--rw-rw-r--   0 root         (0)     1003    30037 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/jwt.py
--rw-rw-r--   0 root         (0)     1003    13205 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/pluggable.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.787471 google-auth-2.9.0/google/auth/transport/
--rw-rw-r--   0 root         (0)     1003     3438 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/__init__.py
--rw-rw-r--   0 root         (0)     1003    14400 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/_aiohttp_requests.py
--rw-rw-r--   0 root         (0)     1003     8400 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/_custom_tls_signer.py
--rw-rw-r--   0 root         (0)     1003     3739 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/_http_client.py
--rw-rw-r--   0 root         (0)     1003     9086 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/_mtls_helper.py
--rw-rw-r--   0 root         (0)     1003    13995 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/grpc.py
--rw-rw-r--   0 root         (0)     1003     3817 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/mtls.py
--rw-rw-r--   0 root         (0)     1003    22877 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/requests.py
--rw-rw-r--   0 root         (0)     1003    15812 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/transport/urllib3.py
--rw-rw-r--   0 root         (0)     1003      597 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/auth/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.791471 google-auth-2.9.0/google/oauth2/
--rw-rw-r--   0 root         (0)     1003      619 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/__init__.py
--rw-rw-r--   0 root         (0)     1003    12831 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/_client.py
--rw-rw-r--   0 root         (0)     1003     9374 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/_client_async.py
--rw-rw-r--   0 root         (0)     1003     4257 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/_credentials_async.py
--rw-rw-r--   0 root         (0)     1003    10147 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/_id_token_async.py
--rw-rw-r--   0 root         (0)     1003    11655 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/_reauth_async.py
--rw-rw-r--   0 root         (0)     1003     5131 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/_service_account_async.py
--rw-rw-r--   0 root         (0)     1003     6101 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/challenges.py
--rw-rw-r--   0 root         (0)     1003    19467 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/credentials.py
--rw-rw-r--   0 root         (0)     1003     9007 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/gdch_credentials.py
--rw-rw-r--   0 root         (0)     1003    12072 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/id_token.py
--rw-rw-r--   0 root         (0)     1003    12074 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/reauth.py
--rw-rw-r--   0 root         (0)     1003    25930 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/service_account.py
--rw-rw-r--   0 root         (0)     1003     6058 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/sts.py
--rw-rw-r--   0 root         (0)     1003     6344 2022-06-29 03:38:41.000000 google-auth-2.9.0/google/oauth2/utils.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.791471 google-auth-2.9.0/google_auth.egg-info/
--rw-r--r--   0 root         (0)     1003     3113 2022-06-29 03:41:22.000000 google-auth-2.9.0/google_auth.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     4315 2022-06-29 03:41:23.000000 google-auth-2.9.0/google_auth.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-06-29 03:41:23.000000 google-auth-2.9.0/google_auth.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        7 2022-06-29 03:41:23.000000 google-auth-2.9.0/google_auth.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003      385 2022-06-29 03:41:23.000000 google-auth-2.9.0/google_auth.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-06-29 03:41:23.000000 google-auth-2.9.0/google_auth.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-06-29 03:41:23.807471 google-auth-2.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3127 2022-06-29 03:38:41.000000 google-auth-2.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.795471 google-auth-2.9.0/tests/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.795471 google-auth-2.9.0/tests/compute_engine/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/compute_engine/__init__.py
--rw-rw-r--   0 root         (0)     1003    10852 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/compute_engine/test__metadata.py
--rw-rw-r--   0 root         (0)     1003    30393 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/compute_engine/test_credentials.py
--rw-rw-r--   0 root         (0)     1003     1604 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/conftest.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.795471 google-auth-2.9.0/tests/crypt/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/crypt/__init__.py
--rw-rw-r--   0 root         (0)     1003     6520 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/crypt/test__cryptography_rsa.py
--rw-rw-r--   0 root         (0)     1003     7598 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/crypt/test__python_rsa.py
--rw-rw-r--   0 root         (0)     1003     1914 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/crypt/test_crypt.py
--rw-rw-r--   0 root         (0)     1003     5718 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/crypt/test_es256.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.799471 google-auth-2.9.0/tests/data/
--rw-rw-r--   0 root         (0)     1003      122 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/authorized_user.json
--rw-rw-r--   0 root         (0)     1003      191 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/authorized_user_cloud_sdk.json
--rw-rw-r--   0 root         (0)     1003      233 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/authorized_user_cloud_sdk_with_quota_project_id.json
--rw-rw-r--   0 root         (0)     1003      160 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/authorized_user_with_rapt_token.json
--rw-rw-r--   0 root         (0)     1003      442 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/client_secrets.json
--rw-rw-r--   0 root         (0)     1003      433 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/cloud_sdk_config.json
--rw-rw-r--   0 root         (0)     1003      172 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/context_aware_metadata.json
--rw-rw-r--   0 root         (0)     1003       18 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/enterprise_cert_invalid.json
--rw-rw-r--   0 root         (0)     1003      122 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/enterprise_cert_valid.json
--rw-rw-r--   0 root         (0)     1003      227 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/es256_privatekey.pem
--rw-rw-r--   0 root         (0)     1003      440 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/es256_public_cert.pem
--rw-rw-r--   0 root         (0)     1003      178 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/es256_publickey.pem
--rw-rw-r--   0 root         (0)     1003      535 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/es256_service_account.json
--rw-rw-r--   0 root         (0)     1003       62 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/external_subject_token.json
--rw-rw-r--   0 root         (0)     1003       38 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/external_subject_token.txt
--rw-rw-r--   0 root         (0)     1003      532 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/gdch_service_account.json
--rw-rw-r--   0 root         (0)     1003      463 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/impersonated_service_account_authorized_user_source.json
--rw-rw-r--   0 root         (0)     1003     2376 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/impersonated_service_account_service_account_source.json
--rw-rw-r--   0 root         (0)     1003      504 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/impersonated_service_account_with_quota_project.json
--rw-rw-r--   0 root         (0)     1003      283 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/old_oauth_credentials_py3.pickle
--rw-rw-r--   0 root         (0)     1003     2041 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/other_cert.pem
--rw-rw-r--   0 root         (0)     1003     1850 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/pem_from_pkcs12.pem
--rw-rw-r--   0 root         (0)     1003     2452 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/privatekey.p12
--rw-rw-r--   0 root         (0)     1003     1679 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/privatekey.pem
--rw-rw-r--   0 root         (0)     1003      426 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/privatekey.pub
--rw-rw-r--   0 root         (0)     1003     1147 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/public_cert.pem
--rw-rw-r--   0 root         (0)     1003     2011 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/data/service_account.json
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.803471 google-auth-2.9.0/tests/oauth2/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/__init__.py
--rw-rw-r--   0 root         (0)     1003    10371 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test__client.py
--rw-rw-r--   0 root         (0)     1003     5299 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test_challenges.py
--rw-rw-r--   0 root         (0)     1003    32414 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test_credentials.py
--rw-rw-r--   0 root         (0)     1003     6648 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test_gdch_credentials.py
--rw-rw-r--   0 root         (0)     1003    11104 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test_id_token.py
--rw-rw-r--   0 root         (0)     1003    11497 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test_reauth.py
--rw-rw-r--   0 root         (0)     1003    20208 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test_service_account.py
--rw-rw-r--   0 root         (0)     1003    15057 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test_sts.py
--rw-rw-r--   0 root         (0)     1003     9405 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/oauth2/test_utils.py
--rw-rw-r--   0 root         (0)     1003     5977 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test__cloud_sdk.py
--rw-rw-r--   0 root         (0)     1003    43979 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test__default.py
--rw-rw-r--   0 root         (0)     1003     4522 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test__helpers.py
--rw-rw-r--   0 root         (0)     1003     5544 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test__oauth2client.py
--rw-rw-r--   0 root         (0)     1003     2636 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test__service_account_info.py
--rw-rw-r--   0 root         (0)     1003     7423 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_app_engine.py
--rw-rw-r--   0 root         (0)     1003    70608 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_aws.py
--rw-rw-r--   0 root         (0)     1003     5444 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_credentials.py
--rw-rw-r--   0 root         (0)     1003    27374 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_downscoped.py
--rw-rw-r--   0 root         (0)     1003    71686 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_external_account.py
--rw-rw-r--   0 root         (0)     1003     3273 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_iam.py
--rw-rw-r--   0 root         (0)     1003    44116 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_identity_pool.py
--rw-rw-r--   0 root         (0)     1003    20132 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_impersonated_credentials.py
--rw-rw-r--   0 root         (0)     1003    22800 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_jwt.py
--rw-rw-r--   0 root         (0)     1003    30000 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/test_pluggable.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-29 03:41:23.803471 google-auth-2.9.0/tests/transport/
--rw-rw-r--   0 root         (0)     1003        0 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/__init__.py
--rw-rw-r--   0 root         (0)     1003     3742 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/compliance.py
--rw-rw-r--   0 root         (0)     1003     8690 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/test__custom_tls_signer.py
--rw-rw-r--   0 root         (0)     1003     1126 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/test__http_client.py
--rw-rw-r--   0 root         (0)     1003    17281 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/test__mtls_helper.py
--rw-rw-r--   0 root         (0)     1003    18477 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/test_grpc.py
--rw-rw-r--   0 root         (0)     1003     3394 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/test_mtls.py
--rw-rw-r--   0 root         (0)     1003    21891 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/test_requests.py
--rw-rw-r--   0 root         (0)     1003    11469 2022-06-29 03:38:41.000000 google-auth-2.9.0/tests/transport/test_urllib3.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.927952 google-auth-2.9.1/
+-rw-rw-r--   0 root         (0)     1003    11357 2022-07-12 22:49:37.000000 google-auth-2.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      100 2022-07-12 22:49:37.000000 google-auth-2.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3113 2022-07-12 22:52:23.927952 google-auth-2.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     1931 2022-07-12 22:49:37.000000 google-auth-2.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.903953 google-auth-2.9.1/google/
+-rw-rw-r--   0 root         (0)     1003      796 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.907953 google-auth-2.9.1/google/auth/
+-rw-rw-r--   0 root         (0)     1003      988 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5272 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/_cloud_sdk.py
+-rw-rw-r--   0 root         (0)     1003     6841 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/_credentials_async.py
+-rw-rw-r--   0 root         (0)     1003    25524 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/_default.py
+-rw-rw-r--   0 root         (0)     1003    11588 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/_default_async.py
+-rw-rw-r--   0 root         (0)     1003     7129 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     5972 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/_jwt_async.py
+-rw-rw-r--   0 root         (0)     1003     5879 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/_oauth2client.py
+-rw-rw-r--   0 root         (0)     1003     2781 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/_service_account_info.py
+-rw-rw-r--   0 root         (0)     1003     6026 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/app_engine.py
+-rw-rw-r--   0 root         (0)     1003    30616 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/aws.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.907953 google-auth-2.9.1/google/auth/compute_engine/
+-rw-rw-r--   0 root         (0)     1003      804 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/compute_engine/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9413 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/compute_engine/_metadata.py
+-rw-rw-r--   0 root         (0)     1003    15833 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/compute_engine/credentials.py
+-rw-rw-r--   0 root         (0)     1003    13082 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/credentials.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.911952 google-auth-2.9.1/google/auth/crypt/
+-rw-rw-r--   0 root         (0)     1003     3356 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/crypt/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4564 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/crypt/_cryptography_rsa.py
+-rw-rw-r--   0 root         (0)     1003        0 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/crypt/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     6069 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/crypt/_python_rsa.py
+-rw-rw-r--   0 root         (0)     1003     4203 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/crypt/base.py
+-rw-rw-r--   0 root         (0)     1003     5657 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/crypt/es256.py
+-rw-rw-r--   0 root         (0)     1003     1109 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/crypt/rsa.py
+-rw-rw-r--   0 root         (0)     1003    21157 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/downscoped.py
+-rw-rw-r--   0 root         (0)     1003     3156 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/environment_vars.py
+-rw-rw-r--   0 root         (0)     1003     1968 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    20222 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/external_account.py
+-rw-rw-r--   0 root         (0)     1003     3652 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/iam.py
+-rw-rw-r--   0 root         (0)     1003    11757 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/identity_pool.py
+-rw-rw-r--   0 root         (0)     1003    15779 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/impersonated_credentials.py
+-rw-rw-r--   0 root         (0)     1003    30037 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/jwt.py
+-rw-rw-r--   0 root         (0)     1003    13205 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/pluggable.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.911952 google-auth-2.9.1/google/auth/transport/
+-rw-rw-r--   0 root         (0)     1003     3438 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14400 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/_aiohttp_requests.py
+-rw-rw-r--   0 root         (0)     1003     8400 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/_custom_tls_signer.py
+-rw-rw-r--   0 root         (0)     1003     3739 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/_http_client.py
+-rw-rw-r--   0 root         (0)     1003     9086 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/_mtls_helper.py
+-rw-rw-r--   0 root         (0)     1003    13995 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/grpc.py
+-rw-rw-r--   0 root         (0)     1003     3817 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/mtls.py
+-rw-rw-r--   0 root         (0)     1003    22877 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/requests.py
+-rw-rw-r--   0 root         (0)     1003    15812 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/transport/urllib3.py
+-rw-rw-r--   0 root         (0)     1003      597 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/auth/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.915952 google-auth-2.9.1/google/oauth2/
+-rw-rw-r--   0 root         (0)     1003      619 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    12831 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/_client.py
+-rw-rw-r--   0 root         (0)     1003     9374 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/_client_async.py
+-rw-rw-r--   0 root         (0)     1003     4257 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/_credentials_async.py
+-rw-rw-r--   0 root         (0)     1003    10147 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/_id_token_async.py
+-rw-rw-r--   0 root         (0)     1003    11655 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/_reauth_async.py
+-rw-rw-r--   0 root         (0)     1003     5131 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/_service_account_async.py
+-rw-rw-r--   0 root         (0)     1003     6101 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/challenges.py
+-rw-rw-r--   0 root         (0)     1003    19467 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/credentials.py
+-rw-rw-r--   0 root         (0)     1003     9007 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/gdch_credentials.py
+-rw-rw-r--   0 root         (0)     1003    12072 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/id_token.py
+-rw-rw-r--   0 root         (0)     1003    12074 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/reauth.py
+-rw-rw-r--   0 root         (0)     1003    25930 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/service_account.py
+-rw-rw-r--   0 root         (0)     1003     6058 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/sts.py
+-rw-rw-r--   0 root         (0)     1003     6344 2022-07-12 22:49:37.000000 google-auth-2.9.1/google/oauth2/utils.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.915952 google-auth-2.9.1/google_auth.egg-info/
+-rw-r--r--   0 root         (0)     1003     3113 2022-07-12 22:52:23.000000 google-auth-2.9.1/google_auth.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     4315 2022-07-12 22:52:23.000000 google-auth-2.9.1/google_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-07-12 22:52:23.000000 google-auth-2.9.1/google_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-07-12 22:52:23.000000 google-auth-2.9.1/google_auth.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003      385 2022-07-12 22:52:23.000000 google-auth-2.9.1/google_auth.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-07-12 22:52:23.000000 google-auth-2.9.1/google_auth.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-07-12 22:52:23.927952 google-auth-2.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3127 2022-07-12 22:49:37.000000 google-auth-2.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.919952 google-auth-2.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003        0 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.919952 google-auth-2.9.1/tests/compute_engine/
+-rw-rw-r--   0 root         (0)     1003        0 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/compute_engine/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10852 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/compute_engine/test__metadata.py
+-rw-rw-r--   0 root         (0)     1003    30393 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/compute_engine/test_credentials.py
+-rw-rw-r--   0 root         (0)     1003     1604 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/conftest.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.919952 google-auth-2.9.1/tests/crypt/
+-rw-rw-r--   0 root         (0)     1003        0 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/crypt/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6520 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/crypt/test__cryptography_rsa.py
+-rw-rw-r--   0 root         (0)     1003     7598 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/crypt/test__python_rsa.py
+-rw-rw-r--   0 root         (0)     1003     1914 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/crypt/test_crypt.py
+-rw-rw-r--   0 root         (0)     1003     5718 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/crypt/test_es256.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.923952 google-auth-2.9.1/tests/data/
+-rw-rw-r--   0 root         (0)     1003      122 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/authorized_user.json
+-rw-rw-r--   0 root         (0)     1003      191 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/authorized_user_cloud_sdk.json
+-rw-rw-r--   0 root         (0)     1003      233 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/authorized_user_cloud_sdk_with_quota_project_id.json
+-rw-rw-r--   0 root         (0)     1003      160 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/authorized_user_with_rapt_token.json
+-rw-rw-r--   0 root         (0)     1003      442 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/client_secrets.json
+-rw-rw-r--   0 root         (0)     1003      433 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/cloud_sdk_config.json
+-rw-rw-r--   0 root         (0)     1003      172 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/context_aware_metadata.json
+-rw-rw-r--   0 root         (0)     1003       18 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/enterprise_cert_invalid.json
+-rw-rw-r--   0 root         (0)     1003      122 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/enterprise_cert_valid.json
+-rw-rw-r--   0 root         (0)     1003      227 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/es256_privatekey.pem
+-rw-rw-r--   0 root         (0)     1003      440 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/es256_public_cert.pem
+-rw-rw-r--   0 root         (0)     1003      178 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/es256_publickey.pem
+-rw-rw-r--   0 root         (0)     1003      535 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/es256_service_account.json
+-rw-rw-r--   0 root         (0)     1003       62 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/external_subject_token.json
+-rw-rw-r--   0 root         (0)     1003       38 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/external_subject_token.txt
+-rw-rw-r--   0 root         (0)     1003      532 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/gdch_service_account.json
+-rw-rw-r--   0 root         (0)     1003      463 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/impersonated_service_account_authorized_user_source.json
+-rw-rw-r--   0 root         (0)     1003     2376 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/impersonated_service_account_service_account_source.json
+-rw-rw-r--   0 root         (0)     1003      504 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/impersonated_service_account_with_quota_project.json
+-rw-rw-r--   0 root         (0)     1003      283 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/old_oauth_credentials_py3.pickle
+-rw-rw-r--   0 root         (0)     1003     2041 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/other_cert.pem
+-rw-rw-r--   0 root         (0)     1003     1850 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/pem_from_pkcs12.pem
+-rw-rw-r--   0 root         (0)     1003     2452 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/privatekey.p12
+-rw-rw-r--   0 root         (0)     1003     1679 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/privatekey.pem
+-rw-rw-r--   0 root         (0)     1003      426 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/privatekey.pub
+-rw-rw-r--   0 root         (0)     1003     1147 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/public_cert.pem
+-rw-rw-r--   0 root         (0)     1003     2011 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/data/service_account.json
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.927952 google-auth-2.9.1/tests/oauth2/
+-rw-rw-r--   0 root         (0)     1003        0 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10371 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test__client.py
+-rw-rw-r--   0 root         (0)     1003     5299 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test_challenges.py
+-rw-rw-r--   0 root         (0)     1003    32414 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test_credentials.py
+-rw-rw-r--   0 root         (0)     1003     6648 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test_gdch_credentials.py
+-rw-rw-r--   0 root         (0)     1003    11104 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test_id_token.py
+-rw-rw-r--   0 root         (0)     1003    11497 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test_reauth.py
+-rw-rw-r--   0 root         (0)     1003    20208 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test_service_account.py
+-rw-rw-r--   0 root         (0)     1003    15057 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test_sts.py
+-rw-rw-r--   0 root         (0)     1003     9405 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/oauth2/test_utils.py
+-rw-rw-r--   0 root         (0)     1003     5977 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test__cloud_sdk.py
+-rw-rw-r--   0 root         (0)     1003    43979 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test__default.py
+-rw-rw-r--   0 root         (0)     1003     4522 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003     5544 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test__oauth2client.py
+-rw-rw-r--   0 root         (0)     1003     2636 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test__service_account_info.py
+-rw-rw-r--   0 root         (0)     1003     7423 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_app_engine.py
+-rw-rw-r--   0 root         (0)     1003    70608 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_aws.py
+-rw-rw-r--   0 root         (0)     1003     5444 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_credentials.py
+-rw-rw-r--   0 root         (0)     1003    27374 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_downscoped.py
+-rw-rw-r--   0 root         (0)     1003    71686 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_external_account.py
+-rw-rw-r--   0 root         (0)     1003     3273 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_iam.py
+-rw-rw-r--   0 root         (0)     1003    44116 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_identity_pool.py
+-rw-rw-r--   0 root         (0)     1003    20132 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_impersonated_credentials.py
+-rw-rw-r--   0 root         (0)     1003    22800 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_jwt.py
+-rw-rw-r--   0 root         (0)     1003    30000 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/test_pluggable.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-12 22:52:23.927952 google-auth-2.9.1/tests/transport/
+-rw-rw-r--   0 root         (0)     1003        0 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3742 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/compliance.py
+-rw-rw-r--   0 root         (0)     1003     8690 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/test__custom_tls_signer.py
+-rw-rw-r--   0 root         (0)     1003     1126 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/test__http_client.py
+-rw-rw-r--   0 root         (0)     1003    17281 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/test__mtls_helper.py
+-rw-rw-r--   0 root         (0)     1003    18477 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/test_grpc.py
+-rw-rw-r--   0 root         (0)     1003     3394 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/test_mtls.py
+-rw-rw-r--   0 root         (0)     1003    21891 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/test_requests.py
+-rw-rw-r--   0 root         (0)     1003    11469 2022-07-12 22:49:37.000000 google-auth-2.9.1/tests/transport/test_urllib3.py
```

### Comparing `google-auth-2.9.0/LICENSE` & `google-auth-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/PKG-INFO` & `google-auth-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-auth
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Authentication Library
 Home-page: https://github.com/googleapis/google-auth-library-python
 Author: Google Cloud Platform
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Keywords: google auth oauth client
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-auth-2.9.0/README.rst` & `google-auth-2.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/__init__.py` & `google-auth-2.9.1/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/__init__.py` & `google-auth-2.9.1/google/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/_cloud_sdk.py` & `google-auth-2.9.1/google/auth/_cloud_sdk.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/_credentials_async.py` & `google-auth-2.9.1/google/auth/_credentials_async.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/_default.py` & `google-auth-2.9.1/google/auth/_default.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/_default_async.py` & `google-auth-2.9.1/google/auth/_default_async.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/_helpers.py` & `google-auth-2.9.1/google/auth/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/_jwt_async.py` & `google-auth-2.9.1/google/auth/_jwt_async.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/_oauth2client.py` & `google-auth-2.9.1/google/auth/_oauth2client.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/_service_account_info.py` & `google-auth-2.9.1/google/auth/_service_account_info.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/app_engine.py` & `google-auth-2.9.1/google/auth/app_engine.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/aws.py` & `google-auth-2.9.1/google/auth/aws.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/compute_engine/__init__.py` & `google-auth-2.9.1/google/auth/compute_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/compute_engine/_metadata.py` & `google-auth-2.9.1/google/auth/compute_engine/_metadata.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/compute_engine/credentials.py` & `google-auth-2.9.1/google/auth/compute_engine/credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/credentials.py` & `google-auth-2.9.1/google/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/crypt/__init__.py` & `google-auth-2.9.1/google/auth/crypt/__init__.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/crypt/_cryptography_rsa.py` & `google-auth-2.9.1/google/auth/crypt/_cryptography_rsa.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/crypt/_python_rsa.py` & `google-auth-2.9.1/google/auth/crypt/_python_rsa.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/crypt/base.py` & `google-auth-2.9.1/google/auth/crypt/base.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/crypt/es256.py` & `google-auth-2.9.1/google/auth/crypt/es256.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/crypt/rsa.py` & `google-auth-2.9.1/google/auth/crypt/rsa.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/downscoped.py` & `google-auth-2.9.1/google/auth/downscoped.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/environment_vars.py` & `google-auth-2.9.1/google/auth/environment_vars.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/exceptions.py` & `google-auth-2.9.1/google/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/external_account.py` & `google-auth-2.9.1/google/auth/external_account.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/iam.py` & `google-auth-2.9.1/google/auth/iam.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/identity_pool.py` & `google-auth-2.9.1/google/auth/identity_pool.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/impersonated_credentials.py` & `google-auth-2.9.1/google/auth/impersonated_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     response_body = (
         response.data.decode("utf-8")
         if hasattr(response.data, "decode")
         else response.data
     )
 
     if response.status != http_client.OK:
-        exceptions.RefreshError(_REFRESH_ERROR, response_body)
+        raise exceptions.RefreshError(_REFRESH_ERROR, response_body)
 
     try:
         token_response = json.loads(response_body)
         token = token_response["accessToken"]
         expiry = datetime.strptime(token_response["expireTime"], "%Y-%m-%dT%H:%M:%SZ")
 
         return token, expiry
```

### Comparing `google-auth-2.9.0/google/auth/jwt.py` & `google-auth-2.9.1/google/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/pluggable.py` & `google-auth-2.9.1/google/auth/pluggable.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/__init__.py` & `google-auth-2.9.1/google/auth/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/_aiohttp_requests.py` & `google-auth-2.9.1/google/auth/transport/_aiohttp_requests.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/_custom_tls_signer.py` & `google-auth-2.9.1/google/auth/transport/_custom_tls_signer.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/_http_client.py` & `google-auth-2.9.1/google/auth/transport/_http_client.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/_mtls_helper.py` & `google-auth-2.9.1/google/auth/transport/_mtls_helper.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/grpc.py` & `google-auth-2.9.1/google/auth/transport/grpc.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/mtls.py` & `google-auth-2.9.1/google/auth/transport/mtls.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/requests.py` & `google-auth-2.9.1/google/auth/transport/requests.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/transport/urllib3.py` & `google-auth-2.9.1/google/auth/transport/urllib3.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/auth/version.py` & `google-auth-2.9.1/google/auth/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.9.0"
+__version__ = "2.9.1"
```

### Comparing `google-auth-2.9.0/google/oauth2/__init__.py` & `google-auth-2.9.1/google/oauth2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/_client.py` & `google-auth-2.9.1/google/oauth2/_client.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/_client_async.py` & `google-auth-2.9.1/google/oauth2/_client_async.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/_credentials_async.py` & `google-auth-2.9.1/google/oauth2/_credentials_async.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/_id_token_async.py` & `google-auth-2.9.1/google/oauth2/_id_token_async.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/_reauth_async.py` & `google-auth-2.9.1/google/oauth2/_reauth_async.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/_service_account_async.py` & `google-auth-2.9.1/google/oauth2/_service_account_async.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/challenges.py` & `google-auth-2.9.1/google/oauth2/challenges.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/credentials.py` & `google-auth-2.9.1/google/oauth2/credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/gdch_credentials.py` & `google-auth-2.9.1/google/oauth2/gdch_credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/id_token.py` & `google-auth-2.9.1/google/oauth2/id_token.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/reauth.py` & `google-auth-2.9.1/google/oauth2/reauth.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/service_account.py` & `google-auth-2.9.1/google/oauth2/service_account.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/sts.py` & `google-auth-2.9.1/google/oauth2/sts.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google/oauth2/utils.py` & `google-auth-2.9.1/google/oauth2/utils.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/google_auth.egg-info/PKG-INFO` & `google-auth-2.9.1/google_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-auth
-Version: 2.9.0
+Version: 2.9.1
 Summary: Google Authentication Library
 Home-page: https://github.com/googleapis/google-auth-library-python
 Author: Google Cloud Platform
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Keywords: google auth oauth client
 Classifier: Programming Language :: Python :: 3
```

### Comparing `google-auth-2.9.0/google_auth.egg-info/SOURCES.txt` & `google-auth-2.9.1/google_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/setup.py` & `google-auth-2.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/compute_engine/test__metadata.py` & `google-auth-2.9.1/tests/compute_engine/test__metadata.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/compute_engine/test_credentials.py` & `google-auth-2.9.1/tests/compute_engine/test_credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/conftest.py` & `google-auth-2.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/crypt/test__cryptography_rsa.py` & `google-auth-2.9.1/tests/crypt/test__cryptography_rsa.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/crypt/test__python_rsa.py` & `google-auth-2.9.1/tests/crypt/test__python_rsa.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/crypt/test_crypt.py` & `google-auth-2.9.1/tests/crypt/test_crypt.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/crypt/test_es256.py` & `google-auth-2.9.1/tests/crypt/test_es256.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/es256_service_account.json` & `google-auth-2.9.1/tests/data/es256_service_account.json`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/gdch_service_account.json` & `google-auth-2.9.1/tests/data/gdch_service_account.json`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/impersonated_service_account_service_account_source.json` & `google-auth-2.9.1/tests/data/impersonated_service_account_service_account_source.json`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/other_cert.pem` & `google-auth-2.9.1/tests/data/other_cert.pem`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/pem_from_pkcs12.pem` & `google-auth-2.9.1/tests/data/pem_from_pkcs12.pem`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/privatekey.p12` & `google-auth-2.9.1/tests/data/privatekey.p12`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/privatekey.pem` & `google-auth-2.9.1/tests/data/privatekey.pem`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/public_cert.pem` & `google-auth-2.9.1/tests/data/public_cert.pem`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/data/service_account.json` & `google-auth-2.9.1/tests/data/service_account.json`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test__client.py` & `google-auth-2.9.1/tests/oauth2/test__client.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test_challenges.py` & `google-auth-2.9.1/tests/oauth2/test_challenges.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test_credentials.py` & `google-auth-2.9.1/tests/oauth2/test_credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test_gdch_credentials.py` & `google-auth-2.9.1/tests/oauth2/test_gdch_credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test_id_token.py` & `google-auth-2.9.1/tests/oauth2/test_id_token.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test_reauth.py` & `google-auth-2.9.1/tests/oauth2/test_reauth.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test_service_account.py` & `google-auth-2.9.1/tests/oauth2/test_service_account.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test_sts.py` & `google-auth-2.9.1/tests/oauth2/test_sts.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/oauth2/test_utils.py` & `google-auth-2.9.1/tests/oauth2/test_utils.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test__cloud_sdk.py` & `google-auth-2.9.1/tests/test__cloud_sdk.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test__default.py` & `google-auth-2.9.1/tests/test__default.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test__helpers.py` & `google-auth-2.9.1/tests/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test__oauth2client.py` & `google-auth-2.9.1/tests/test__oauth2client.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test__service_account_info.py` & `google-auth-2.9.1/tests/test__service_account_info.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_app_engine.py` & `google-auth-2.9.1/tests/test_app_engine.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_aws.py` & `google-auth-2.9.1/tests/test_aws.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_credentials.py` & `google-auth-2.9.1/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_downscoped.py` & `google-auth-2.9.1/tests/test_downscoped.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_external_account.py` & `google-auth-2.9.1/tests/test_external_account.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_iam.py` & `google-auth-2.9.1/tests/test_iam.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_identity_pool.py` & `google-auth-2.9.1/tests/test_identity_pool.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_impersonated_credentials.py` & `google-auth-2.9.1/tests/test_impersonated_credentials.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_jwt.py` & `google-auth-2.9.1/tests/test_jwt.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/test_pluggable.py` & `google-auth-2.9.1/tests/test_pluggable.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/transport/compliance.py` & `google-auth-2.9.1/tests/transport/compliance.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/transport/test__custom_tls_signer.py` & `google-auth-2.9.1/tests/transport/test__custom_tls_signer.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/transport/test__http_client.py` & `google-auth-2.9.1/tests/transport/test__http_client.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/transport/test__mtls_helper.py` & `google-auth-2.9.1/tests/transport/test__mtls_helper.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/transport/test_grpc.py` & `google-auth-2.9.1/tests/transport/test_grpc.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/transport/test_mtls.py` & `google-auth-2.9.1/tests/transport/test_mtls.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/transport/test_requests.py` & `google-auth-2.9.1/tests/transport/test_requests.py`

 * *Files identical despite different names*

### Comparing `google-auth-2.9.0/tests/transport/test_urllib3.py` & `google-auth-2.9.1/tests/transport/test_urllib3.py`

 * *Files identical despite different names*

