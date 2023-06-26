# Comparing `tmp/google-cloud-storage-2.8.0.tar.gz` & `tmp/google-cloud-storage-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-storage-2.8.0.tar", last modified: Wed Mar 29 21:21:14 2023, max compression
+gzip compressed data, was "google-cloud-storage-2.9.0.tar", last modified: Thu May  4 17:56:42 2023, max compression
```

## Comparing `google-cloud-storage-2.8.0.tar` & `google-cloud-storage-2.9.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.610366 google-cloud-storage-2.8.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5711 2023-03-29 21:21:14.610366 google-cloud-storage-2.8.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     4770 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.590364 google-cloud-storage-2.8.0/google/
--rw-rw-r--   0 root         (0)     1003      747 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.590364 google-cloud-storage-2.8.0/google/cloud/
--rw-rw-r--   0 root         (0)     1003      747 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.594364 google-cloud-storage-2.8.0/google/cloud/storage/
--rw-rw-r--   0 root         (0)     1003     1459 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/__init__.py
--rw-rw-r--   0 root         (0)     1003    20975 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/_helpers.py
--rw-rw-r--   0 root         (0)     1003     3097 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/_http.py
--rw-rw-r--   0 root         (0)     1003    25540 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/_signing.py
--rw-rw-r--   0 root         (0)     1003    25375 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/acl.py
--rw-rw-r--   0 root         (0)     1003    11433 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/batch.py
--rw-rw-r--   0 root         (0)     1003   173911 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/blob.py
--rw-rw-r--   0 root         (0)     1003   130111 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/bucket.py
--rw-rw-r--   0 root         (0)     1003    67467 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/client.py
--rw-rw-r--   0 root         (0)     1003     4347 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/constants.py
--rw-rw-r--   0 root         (0)     1003    20444 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/fileio.py
--rw-rw-r--   0 root         (0)     1003     9767 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/hmac_key.py
--rw-rw-r--   0 root         (0)     1003     2802 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/iam.py
--rw-rw-r--   0 root         (0)     1003    15546 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/notification.py
--rw-rw-r--   0 root         (0)     1003     6343 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/retry.py
--rw-rw-r--   0 root         (0)     1003    39067 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/transfer_manager.py
--rw-rw-r--   0 root         (0)     1003      597 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/google/cloud/storage/version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.594364 google-cloud-storage-2.8.0/google_cloud_storage.egg-info/
--rw-r--r--   0 root         (0)     1003     5711 2023-03-29 21:21:14.000000 google-cloud-storage-2.8.0/google_cloud_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2168 2023-03-29 21:21:14.000000 google-cloud-storage-2.8.0/google_cloud_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-29 21:21:14.000000 google-cloud-storage-2.8.0/google_cloud_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-29 21:21:14.000000 google-cloud-storage-2.8.0/google_cloud_storage.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-29 21:21:14.000000 google-cloud-storage-2.8.0/google_cloud_storage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      214 2023-03-29 21:21:14.000000 google-cloud-storage-2.8.0/google_cloud_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-29 21:21:14.000000 google-cloud-storage-2.8.0/google_cloud_storage.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-29 21:21:14.610366 google-cloud-storage-2.8.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3047 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.594364 google-cloud-storage-2.8.0/tests/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.594364 google-cloud-storage-2.8.0/tests/conformance/
--rw-rw-r--   0 root         (0)     1003     1736 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/conformance/README.md
--rw-rw-r--   0 root         (0)     1003      843 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/conformance/__init__.py
--rw-rw-r--   0 root         (0)     1003     3881 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/conformance/conftest.py
--rw-rw-r--   0 root         (0)     1003    15946 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/conformance/retry_strategy_test_data.json
--rw-rw-r--   0 root         (0)     1003    34779 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/conformance/test_conformance.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.602365 google-cloud-storage-2.8.0/tests/data/
--rw-rw-r--   0 root         (0)     1003     9587 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/data/CloudPlatform_128px_Retina.png
--rw-rw-r--   0 root         (0)     1003  5253120 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/data/five-point-one-mb-file.zip
--rw-rw-r--   0 root         (0)     1003       28 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/data/simple.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.602365 google-cloud-storage-2.8.0/tests/perf/
--rw-rw-r--   0 root         (0)     1003     3148 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/perf/README.md
--rw-rw-r--   0 root         (0)     1003     7393 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/perf/_perf_utils.py
--rw-rw-r--   0 root         (0)     1003     5076 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/perf/benchmarking.py
--rw-rw-r--   0 root         (0)     1003     6784 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/perf/profile_w1r3.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.606366 google-cloud-storage-2.8.0/tests/system/
--rw-rw-r--   0 root         (0)     1003        0 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/__init__.py
--rw-rw-r--   0 root         (0)     1003     3865 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/_helpers.py
--rw-rw-r--   0 root         (0)     1003     5492 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/conftest.py
--rw-rw-r--   0 root         (0)     1003    13261 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test__signing.py
--rw-rw-r--   0 root         (0)     1003    34707 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test_blob.py
--rw-rw-r--   0 root         (0)     1003    32417 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test_bucket.py
--rw-rw-r--   0 root         (0)     1003     5779 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test_client.py
--rw-rw-r--   0 root         (0)     1003     2786 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test_fileio.py
--rw-rw-r--   0 root         (0)     1003     2643 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test_hmac_key_metadata.py
--rw-rw-r--   0 root         (0)     1003     8469 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test_kms_integration.py
--rw-rw-r--   0 root         (0)     1003     6518 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test_notification.py
--rw-rw-r--   0 root         (0)     1003     5811 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/system/test_transfer_manager.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-29 21:21:14.610366 google-cloud-storage-2.8.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      843 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/__init__.py
--rw-rw-r--   0 root         (0)     1003    25751 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test__helpers.py
--rw-rw-r--   0 root         (0)     1003     9528 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test__http.py
--rw-rw-r--   0 root         (0)     1003    31936 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test__signing.py
--rw-rw-r--   0 root         (0)     1003    34930 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_acl.py
--rw-rw-r--   0 root         (0)     1003    24937 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_batch.py
--rw-rw-r--   0 root         (0)     1003   222245 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_blob.py
--rw-rw-r--   0 root         (0)     1003   156309 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_bucket.py
--rw-rw-r--   0 root         (0)     1003   105486 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_client.py
--rw-rw-r--   0 root         (0)     1003    36908 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_fileio.py
--rw-rw-r--   0 root         (0)     1003    16748 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_hmac_key.py
--rw-rw-r--   0 root         (0)     1003    23059 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_notification.py
--rw-rw-r--   0 root         (0)     1003     8709 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_retry.py
--rw-rw-r--   0 root         (0)     1003    23190 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/test_transfer_manager.py
--rw-rw-r--   0 root         (0)     1003     2339 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/url_signer_v4_test_account.json
--rw-rw-r--   0 root         (0)     1003    43155 2023-03-29 21:18:24.000000 google-cloud-storage-2.8.0/tests/unit/url_signer_v4_test_data.json
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.208798 google-cloud-storage-2.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5711 2023-05-04 17:56:42.208798 google-cloud-storage-2.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     4770 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.184785 google-cloud-storage-2.9.0/google/
+-rw-rw-r--   0 root         (0)     1003      747 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.184785 google-cloud-storage-2.9.0/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      747 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.188787 google-cloud-storage-2.9.0/google/cloud/storage/
+-rw-rw-r--   0 root         (0)     1003     1459 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20975 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     3097 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/_http.py
+-rw-rw-r--   0 root         (0)     1003    25540 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/_signing.py
+-rw-rw-r--   0 root         (0)     1003    25375 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/acl.py
+-rw-rw-r--   0 root         (0)     1003    11433 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/batch.py
+-rw-rw-r--   0 root         (0)     1003   173899 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/blob.py
+-rw-rw-r--   0 root         (0)     1003   129648 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/bucket.py
+-rw-rw-r--   0 root         (0)     1003    67506 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/client.py
+-rw-rw-r--   0 root         (0)     1003     4347 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/constants.py
+-rw-rw-r--   0 root         (0)     1003    20444 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/fileio.py
+-rw-rw-r--   0 root         (0)     1003     9767 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/hmac_key.py
+-rw-rw-r--   0 root         (0)     1003     2802 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/iam.py
+-rw-rw-r--   0 root         (0)     1003    15546 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/notification.py
+-rw-rw-r--   0 root         (0)     1003     6343 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/retry.py
+-rw-rw-r--   0 root         (0)     1003    39075 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/transfer_manager.py
+-rw-rw-r--   0 root         (0)     1003      597 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/google/cloud/storage/version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.188787 google-cloud-storage-2.9.0/google_cloud_storage.egg-info/
+-rw-r--r--   0 root         (0)     1003     5711 2023-05-04 17:56:42.000000 google-cloud-storage-2.9.0/google_cloud_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2168 2023-05-04 17:56:42.000000 google-cloud-storage-2.9.0/google_cloud_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-04 17:56:42.000000 google-cloud-storage-2.9.0/google_cloud_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-04 17:56:42.000000 google-cloud-storage-2.9.0/google_cloud_storage.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-04 17:56:42.000000 google-cloud-storage-2.9.0/google_cloud_storage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      214 2023-05-04 17:56:42.000000 google-cloud-storage-2.9.0/google_cloud_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-04 17:56:42.000000 google-cloud-storage-2.9.0/google_cloud_storage.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-04 17:56:42.208798 google-cloud-storage-2.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3047 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.192789 google-cloud-storage-2.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003        0 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.192789 google-cloud-storage-2.9.0/tests/conformance/
+-rw-rw-r--   0 root         (0)     1003     1736 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/conformance/README.md
+-rw-rw-r--   0 root         (0)     1003      843 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/conformance/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3881 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/conformance/conftest.py
+-rw-rw-r--   0 root         (0)     1003    15460 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/conformance/retry_strategy_test_data.json
+-rw-rw-r--   0 root         (0)     1003    34779 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/conformance/test_conformance.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.200793 google-cloud-storage-2.9.0/tests/data/
+-rw-rw-r--   0 root         (0)     1003     9587 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/data/CloudPlatform_128px_Retina.png
+-rw-rw-r--   0 root         (0)     1003  5253120 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/data/five-point-one-mb-file.zip
+-rw-rw-r--   0 root         (0)     1003       28 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/data/simple.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.200793 google-cloud-storage-2.9.0/tests/perf/
+-rw-rw-r--   0 root         (0)     1003     3175 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/perf/README.md
+-rw-rw-r--   0 root         (0)     1003     7828 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/perf/_perf_utils.py
+-rw-rw-r--   0 root         (0)     1003     5380 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/perf/benchmarking.py
+-rw-rw-r--   0 root         (0)     1003     6784 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/perf/profile_w1r3.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.204795 google-cloud-storage-2.9.0/tests/system/
+-rw-rw-r--   0 root         (0)     1003        0 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3865 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/_helpers.py
+-rw-rw-r--   0 root         (0)     1003     5492 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/conftest.py
+-rw-rw-r--   0 root         (0)     1003    13261 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test__signing.py
+-rw-rw-r--   0 root         (0)     1003    34707 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test_blob.py
+-rw-rw-r--   0 root         (0)     1003    32417 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test_bucket.py
+-rw-rw-r--   0 root         (0)     1003     5779 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test_client.py
+-rw-rw-r--   0 root         (0)     1003     2786 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test_fileio.py
+-rw-rw-r--   0 root         (0)     1003     2643 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test_hmac_key_metadata.py
+-rw-rw-r--   0 root         (0)     1003     8469 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test_kms_integration.py
+-rw-rw-r--   0 root         (0)     1003     6518 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test_notification.py
+-rw-rw-r--   0 root         (0)     1003     5811 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/system/test_transfer_manager.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-04 17:56:42.208798 google-cloud-storage-2.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      843 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25751 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test__helpers.py
+-rw-rw-r--   0 root         (0)     1003     9528 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test__http.py
+-rw-rw-r--   0 root         (0)     1003    31936 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test__signing.py
+-rw-rw-r--   0 root         (0)     1003    34930 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_acl.py
+-rw-rw-r--   0 root         (0)     1003    24937 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_batch.py
+-rw-rw-r--   0 root         (0)     1003   222245 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_blob.py
+-rw-rw-r--   0 root         (0)     1003   155719 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_bucket.py
+-rw-rw-r--   0 root         (0)     1003   105486 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_client.py
+-rw-rw-r--   0 root         (0)     1003    36908 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_fileio.py
+-rw-rw-r--   0 root         (0)     1003    16748 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_hmac_key.py
+-rw-rw-r--   0 root         (0)     1003    23059 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_notification.py
+-rw-rw-r--   0 root         (0)     1003     8709 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_retry.py
+-rw-rw-r--   0 root         (0)     1003    23190 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/test_transfer_manager.py
+-rw-rw-r--   0 root         (0)     1003     2339 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/url_signer_v4_test_account.json
+-rw-rw-r--   0 root         (0)     1003    43155 2023-05-04 17:53:57.000000 google-cloud-storage-2.9.0/tests/unit/url_signer_v4_test_data.json
```

### Comparing `google-cloud-storage-2.8.0/LICENSE` & `google-cloud-storage-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/MANIFEST.in` & `google-cloud-storage-2.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/PKG-INFO` & `google-cloud-storage-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage
-Version: 2.8.0
+Version: 2.9.0
 Summary: Google Cloud Storage API client library
 Home-page: https://github.com/googleapis/python-storage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-storage-2.8.0/README.rst` & `google-cloud-storage-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/__init__.py` & `google-cloud-storage-2.9.0/google/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/__init__.py` & `google-cloud-storage-2.9.0/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/__init__.py` & `google-cloud-storage-2.9.0/google/cloud/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/_helpers.py` & `google-cloud-storage-2.9.0/google/cloud/storage/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/_http.py` & `google-cloud-storage-2.9.0/google/cloud/storage/_http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/_signing.py` & `google-cloud-storage-2.9.0/google/cloud/storage/_signing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/acl.py` & `google-cloud-storage-2.9.0/google/cloud/storage/acl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/batch.py` & `google-cloud-storage-2.9.0/google/cloud/storage/batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/blob.py` & `google-cloud-storage-2.9.0/google/cloud/storage/blob.py`

 * *Files 0% similar despite different names*

```diff
@@ -1020,15 +1020,15 @@
         if_generation_not_match=None,
         if_metageneration_match=None,
         if_metageneration_not_match=None,
         timeout=_DEFAULT_TIMEOUT,
         checksum="md5",
         retry=DEFAULT_RETRY,
     ):
-        """DEPRECATED. Download the contents of this blob into a file-like object.
+        """Download the contents of this blob into a file-like object.
 
         .. note::
 
            If the server-set property, :attr:`media_link`, is not yet
            initialized, makes an additional API request to load it.
 
         If the :attr:`chunk_size` of a current blob is `None`, will download data
```

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/bucket.py` & `google-cloud-storage-2.9.0/google/cloud/storage/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -918,18 +918,15 @@
         project=None,
         location=None,
         predefined_acl=None,
         predefined_default_object_acl=None,
         timeout=_DEFAULT_TIMEOUT,
         retry=DEFAULT_RETRY,
     ):
-        """DEPRECATED. Creates current bucket.
-
-        .. note::
-          Direct use of this method is deprecated. Use ``Client.create_bucket()`` instead.
+        """Creates current bucket.
 
         If the bucket already exists, will raise
         :class:`google.cloud.exceptions.Conflict`.
 
         This implements "storage.buckets.insert".
 
         If :attr:`user_project` is set, bills the API request to that project.
@@ -966,20 +963,14 @@
             (Optional) The amount of time, in seconds, to wait
             for the server response.  See: :ref:`configuring_timeouts`
 
         :type retry: google.api_core.retry.Retry or google.cloud.storage.retry.ConditionalRetryPolicy
         :param retry:
             (Optional) How to retry the RPC. See: :ref:`configuring_retries`
         """
-        warnings.warn(
-            "Bucket.create() is deprecated and will be removed in future."
-            "Use Client.create_bucket() instead.",
-            PendingDeprecationWarning,
-            stacklevel=1,
-        )
 
         client = self._require_client(client)
         client.create_bucket(
             bucket_or_name=self,
             project=project,
             user_project=self.user_project,
             location=location,
@@ -1296,18 +1287,15 @@
         versions=None,
         projection="noAcl",
         fields=None,
         client=None,
         timeout=_DEFAULT_TIMEOUT,
         retry=DEFAULT_RETRY,
     ):
-        """DEPRECATED. Return an iterator used to find blobs in the bucket.
-
-        .. note::
-          Direct use of this method is deprecated. Use ``Client.list_blobs`` instead.
+        """Return an iterator used to find blobs in the bucket.
 
         If :attr:`user_project` is set, bills the API request to that project.
 
         :type max_results: int
         :param max_results:
             (Optional) The maximum number of blobs to return.
```

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/client.py` & `google-cloud-storage-2.9.0/google/cloud/storage/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,18 +126,19 @@
             project = "<none>"
         else:
             no_project = False
 
         if project is _marker:
             project = None
 
-        # Save the initial value of client_info and client_options before they
+        # Save the initial value of constructor arguments before they
         # are passed along, for use in __reduce__ defined elsewhere.
         self._initial_client_info = client_info
         self._initial_client_options = client_options
+        self._initial_credentials = credentials
 
         kw_args = {"client_info": client_info}
 
         # `api_endpoint` should be only set by the user via `client_options`,
         # or if the _get_storage_host() returns a non-default value (_is_emulator_set).
         # `api_endpoint` plays an important role for mTLS, if it is not set,
         # then mTLS logic will be applied to decide which endpoint will be used.
```

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/constants.py` & `google-cloud-storage-2.9.0/google/cloud/storage/constants.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/fileio.py` & `google-cloud-storage-2.9.0/google/cloud/storage/fileio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/hmac_key.py` & `google-cloud-storage-2.9.0/google/cloud/storage/hmac_key.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/iam.py` & `google-cloud-storage-2.9.0/google/cloud/storage/iam.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/notification.py` & `google-cloud-storage-2.9.0/google/cloud/storage/notification.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/retry.py` & `google-cloud-storage-2.9.0/google/cloud/storage/retry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/transfer_manager.py` & `google-cloud-storage-2.9.0/google/cloud/storage/transfer_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -875,15 +875,15 @@
 
 
 def _reduce_client(cl):
     """Replicate a Client by constructing a new one with the same params."""
 
     client_object_id = id(cl)
     project = cl.project
-    credentials = cl._credentials
+    credentials = cl._initial_credentials
     _http = None  # Can't carry this over
     client_info = cl._initial_client_info
     client_options = cl._initial_client_options
 
     return _LazyClient, (
         client_object_id,
         project,
```

### Comparing `google-cloud-storage-2.8.0/google/cloud/storage/version.py` & `google-cloud-storage-2.9.0/google/cloud/storage/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "2.8.0"
+__version__ = "2.9.0"
```

### Comparing `google-cloud-storage-2.8.0/google_cloud_storage.egg-info/PKG-INFO` & `google-cloud-storage-2.9.0/google_cloud_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage
-Version: 2.8.0
+Version: 2.9.0
 Summary: Google Cloud Storage API client library
 Home-page: https://github.com/googleapis/python-storage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-storage-2.8.0/google_cloud_storage.egg-info/SOURCES.txt` & `google-cloud-storage-2.9.0/google_cloud_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/setup.py` & `google-cloud-storage-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/conformance/README.md` & `google-cloud-storage-2.9.0/tests/conformance/README.md`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/conformance/__init__.py` & `google-cloud-storage-2.9.0/tests/conformance/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/conformance/conftest.py` & `google-cloud-storage-2.9.0/tests/conformance/conftest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/conformance/retry_strategy_test_data.json` & `google-cloud-storage-2.9.0/tests/conformance/retry_strategy_test_data.json`

 * *Files 1% similar despite different names*

```diff
@@ -1,997 +1,967 @@
-00000000: efbb bf7b 0a20 2020 2022 7265 7472 7954  ...{.    "retryT
-00000010: 6573 7473 223a 205b 0a20 2020 2020 207b  ests": [.      {
-00000020: 0a20 2020 2020 2020 2022 6964 223a 2031  .        "id": 1
-00000030: 2c0a 2020 2020 2020 2020 2264 6573 6372  ,.        "descr
-00000040: 6970 7469 6f6e 223a 2022 616c 7761 7973  iption": "always
-00000050: 5f69 6465 6d70 6f74 656e 7422 2c0a 2020  _idempotent",.  
-00000060: 2020 2020 2020 2263 6173 6573 223a 205b        "cases": [
-00000070: 0a20 2020 2020 2020 2020 207b 0a20 2020  .          {.   
-00000080: 2020 2020 2020 2020 2022 696e 7374 7275           "instru
-00000090: 6374 696f 6e73 223a 205b 2272 6574 7572  ctions": ["retur
-000000a0: 6e2d 3530 3322 2c20 2272 6574 7572 6e2d  n-503", "return-
-000000b0: 3530 3322 5d0a 2020 2020 2020 2020 2020  503"].          
-000000c0: 7d2c 0a20 2020 2020 2020 2020 207b 0a20  },.          {. 
-000000d0: 2020 2020 2020 2020 2020 2022 696e 7374             "inst
-000000e0: 7275 6374 696f 6e73 223a 205b 2272 6574  ructions": ["ret
-000000f0: 7572 6e2d 7265 7365 742d 636f 6e6e 6563  urn-reset-connec
-00000100: 7469 6f6e 222c 2022 7265 7475 726e 2d72  tion", "return-r
-00000110: 6573 6574 2d63 6f6e 6e65 6374 696f 6e22  eset-connection"
-00000120: 5d0a 2020 2020 2020 2020 2020 7d2c 0a20  ].          },. 
-00000130: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00000140: 2020 2020 2020 2022 696e 7374 7275 6374         "instruct
-00000150: 696f 6e73 223a 205b 2272 6574 7572 6e2d  ions": ["return-
-00000160: 7265 7365 742d 636f 6e6e 6563 7469 6f6e  reset-connection
-00000170: 222c 2022 7265 7475 726e 2d35 3033 225d  ", "return-503"]
-00000180: 0a20 2020 2020 2020 2020 207d 0a20 2020  .          }.   
-00000190: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-000001a0: 226d 6574 686f 6473 223a 205b 0a20 2020  "methods": [.   
-000001b0: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-000001c0: 2273 746f 7261 6765 2e62 7563 6b65 745f  "storage.bucket_
-000001d0: 6163 6c2e 6765 7422 2c20 2020 2020 2020  acl.get",       
-000001e0: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-000001f0: 6365 7322 3a20 5b22 4255 434b 4554 225d  ces": ["BUCKET"]
-00000200: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00000210: 616d 6522 3a20 2273 746f 7261 6765 2e62  ame": "storage.b
-00000220: 7563 6b65 745f 6163 6c2e 6c69 7374 222c  ucket_acl.list",
-00000230: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000240: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00000250: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
-00000260: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00000270: 7261 6765 2e62 7563 6b65 7473 2e64 656c  rage.buckets.del
-00000280: 6574 6522 2c20 2020 2020 2020 2020 2020  ete",           
-00000290: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-000002a0: 3a20 5b22 4255 434b 4554 225d 7d2c 0a20  : ["BUCKET"]},. 
-000002b0: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-000002c0: 3a20 2273 746f 7261 6765 2e62 7563 6b65  : "storage.bucke
-000002d0: 7473 2e67 6574 222c 2020 2020 2020 2020  ts.get",        
-000002e0: 2020 2020 2020 2020 2020 2022 7265 736f             "reso
-000002f0: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00000300: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-00000310: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00000320: 2e62 7563 6b65 7473 2e67 6574 4961 6d50  .buckets.getIamP
-00000330: 6f6c 6963 7922 2c20 2020 2020 2020 2020  olicy",         
-00000340: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00000350: 4255 434b 4554 225d 7d2c 0a20 2020 2020  BUCKET"]},.     
-00000360: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00000370: 746f 7261 6765 2e62 7563 6b65 7473 2e69  torage.buckets.i
-00000380: 6e73 6572 7422 2c20 2020 2020 2020 2020  nsert",         
-00000390: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-000003a0: 7322 3a20 5b5d 7d2c 0a20 2020 2020 2020  s": []},.       
-000003b0: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-000003c0: 7261 6765 2e62 7563 6b65 7473 2e6c 6973  rage.buckets.lis
-000003d0: 7422 2c20 2020 2020 2020 2020 2020 2020  t",             
-000003e0: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-000003f0: 3a20 5b22 4255 434b 4554 225d 7d2c 0a20  : ["BUCKET"]},. 
-00000400: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00000410: 3a20 2273 746f 7261 6765 2e62 7563 6b65  : "storage.bucke
-00000420: 7473 2e6c 6f63 6b52 6574 656e 7469 6f6e  ts.lockRetention
-00000430: 506f 6c69 6379 222c 2020 2022 7265 736f  Policy",   "reso
-00000440: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00000450: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-00000460: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00000470: 2e62 7563 6b65 7473 2e74 6573 7449 616d  .buckets.testIam
-00000480: 5065 726d 6973 7369 6f6e 7322 2c20 2020  Permissions",   
-00000490: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-000004a0: 4255 434b 4554 225d 7d2c 0a20 2020 2020  BUCKET"]},.     
-000004b0: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-000004c0: 746f 7261 6765 2e64 6566 6175 6c74 5f6f  torage.default_o
-000004d0: 626a 6563 745f 6163 6c2e 6765 7422 2c20  bject_acl.get", 
-000004e0: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-000004f0: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
-00000500: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00000510: 6522 3a20 2273 746f 7261 6765 2e64 6566  e": "storage.def
-00000520: 6175 6c74 5f6f 626a 6563 745f 6163 6c2e  ault_object_acl.
-00000530: 6c69 7374 222c 2020 2020 2020 2022 7265  list",       "re
-00000540: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00000550: 4554 225d 7d2c 0a20 2020 2020 2020 2020  ET"]},.         
-00000560: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00000570: 6765 2e68 6d61 634b 6579 2e64 656c 6574  ge.hmacKey.delet
-00000580: 6522 2c20 2020 2020 2020 2020 2020 2020  e",             
-00000590: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-000005a0: 5b22 484d 4143 5f4b 4559 225d 7d2c 0a20  ["HMAC_KEY"]},. 
-000005b0: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-000005c0: 3a20 2273 746f 7261 6765 2e68 6d61 634b  : "storage.hmacK
-000005d0: 6579 2e67 6574 222c 2020 2020 2020 2020  ey.get",        
-000005e0: 2020 2020 2020 2020 2020 2022 7265 736f             "reso
-000005f0: 7572 6365 7322 3a20 5b22 484d 4143 5f4b  urces": ["HMAC_K
-00000600: 4559 225d 7d2c 0a20 2020 2020 2020 2020  EY"]},.         
-00000610: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00000620: 6765 2e68 6d61 634b 6579 2e6c 6973 7422  ge.hmacKey.list"
-00000630: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00000640: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00000650: 5b22 484d 4143 5f4b 4559 225d 7d2c 0a20  ["HMAC_KEY"]},. 
-00000660: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00000670: 3a20 2273 746f 7261 6765 2e6e 6f74 6966  : "storage.notif
-00000680: 6963 6174 696f 6e73 2e64 656c 6574 6522  ications.delete"
-00000690: 2c20 2020 2020 2020 2020 2022 7265 736f  ,          "reso
-000006a0: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-000006b0: 222c 2022 4e4f 5449 4649 4341 5449 4f4e  ", "NOTIFICATION
-000006c0: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-000006d0: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-000006e0: 2e6e 6f74 6966 6963 6174 696f 6e73 2e67  .notifications.g
-000006f0: 6574 222c 2020 2020 2020 2020 2020 2020  et",            
-00000700: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00000710: 4255 434b 4554 222c 2022 4e4f 5449 4649  BUCKET", "NOTIFI
-00000720: 4341 5449 4f4e 225d 7d2c 0a20 2020 2020  CATION"]},.     
-00000730: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00000740: 746f 7261 6765 2e6e 6f74 6966 6963 6174  torage.notificat
-00000750: 696f 6e73 2e6c 6973 7422 2c20 2020 2020  ions.list",     
-00000760: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-00000770: 7322 3a20 5b22 4255 434b 4554 222c 2022  s": ["BUCKET", "
-00000780: 4e4f 5449 4649 4341 5449 4f4e 225d 7d2c  NOTIFICATION"]},
-00000790: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-000007a0: 6522 3a20 2273 746f 7261 6765 2e6f 626a  e": "storage.obj
-000007b0: 6563 745f 6163 6c2e 6765 7422 2c20 2020  ect_acl.get",   
-000007c0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-000007d0: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-000007e0: 4554 222c 2022 4f42 4a45 4354 225d 7d2c  ET", "OBJECT"]},
-000007f0: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00000800: 6522 3a20 2273 746f 7261 6765 2e6f 626a  e": "storage.obj
-00000810: 6563 745f 6163 6c2e 6c69 7374 222c 2020  ect_acl.list",  
-00000820: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00000830: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00000840: 4554 222c 2022 4f42 4a45 4354 225d 7d2c  ET", "OBJECT"]},
-00000850: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00000860: 6522 3a20 2273 746f 7261 6765 2e6f 626a  e": "storage.obj
-00000870: 6563 7473 2e67 6574 222c 2020 2020 2020  ects.get",      
-00000880: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00000890: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-000008a0: 4554 222c 2022 4f42 4a45 4354 225d 7d2c  ET", "OBJECT"]},
-000008b0: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-000008c0: 6522 3a20 2273 746f 7261 6765 2e6f 626a  e": "storage.obj
-000008d0: 6563 7473 2e6c 6973 7422 2c20 2020 2020  ects.list",     
-000008e0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-000008f0: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00000900: 4554 222c 2022 4f42 4a45 4354 225d 7d2c  ET", "OBJECT"]},
-00000910: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00000920: 6522 3a20 2273 746f 7261 6765 2e73 6572  e": "storage.ser
-00000930: 7669 6365 6163 636f 756e 742e 6765 7422  viceaccount.get"
-00000940: 2c20 2020 2020 2020 2020 2020 2022 7265  ,            "re
-00000950: 736f 7572 6365 7322 3a20 5b5d 7d0a 2020  sources": []}.  
-00000960: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00000970: 2022 7072 6563 6f6e 6469 7469 6f6e 5072   "preconditionPr
-00000980: 6f76 6964 6564 223a 2066 616c 7365 2c0a  ovided": false,.
-00000990: 2020 2020 2020 2020 2265 7870 6563 7453          "expectS
-000009a0: 7563 6365 7373 223a 2074 7275 650a 2020  uccess": true.  
-000009b0: 2020 2020 7d2c 0a20 2020 2020 207b 0a20      },.      {. 
-000009c0: 2020 2020 2020 2022 6964 223a 2032 2c0a         "id": 2,.
-000009d0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-000009e0: 7469 6f6e 223a 2022 636f 6e64 6974 696f  tion": "conditio
-000009f0: 6e61 6c6c 795f 6964 656d 706f 7465 6e74  nally_idempotent
-00000a00: 5f72 6574 7269 6573 5f77 6865 6e5f 7072  _retries_when_pr
-00000a10: 6563 6f6e 6469 7469 6f6e 5f69 735f 7072  econdition_is_pr
-00000a20: 6573 656e 7422 2c0a 2020 2020 2020 2020  esent",.        
-00000a30: 2263 6173 6573 223a 205b 0a20 2020 2020  "cases": [.     
-00000a40: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00000a50: 2020 2022 696e 7374 7275 6374 696f 6e73     "instructions
-00000a60: 223a 205b 2272 6574 7572 6e2d 3530 3322  ": ["return-503"
-00000a70: 2c20 2272 6574 7572 6e2d 3530 3322 5d0a  , "return-503"].
-00000a80: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00000a90: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00000aa0: 2020 2020 2022 696e 7374 7275 6374 696f       "instructio
-00000ab0: 6e73 223a 205b 2272 6574 7572 6e2d 7265  ns": ["return-re
-00000ac0: 7365 742d 636f 6e6e 6563 7469 6f6e 222c  set-connection",
-00000ad0: 2022 7265 7475 726e 2d72 6573 6574 2d63   "return-reset-c
-00000ae0: 6f6e 6e65 6374 696f 6e22 5d0a 2020 2020  onnection"].    
-00000af0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00000b00: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00000b10: 2022 696e 7374 7275 6374 696f 6e73 223a   "instructions":
-00000b20: 205b 2272 6574 7572 6e2d 7265 7365 742d   ["return-reset-
-00000b30: 636f 6e6e 6563 7469 6f6e 222c 2022 7265  connection", "re
-00000b40: 7475 726e 2d35 3033 225d 0a20 2020 2020  turn-503"].     
-00000b50: 2020 2020 207d 0a20 2020 2020 2020 205d       }.        ]
-00000b60: 2c0a 2020 2020 2020 2020 226d 6574 686f  ,.        "metho
-00000b70: 6473 223a 205b 0a20 2020 2020 2020 2020  ds": [.         
-00000b80: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00000b90: 6765 2e62 7563 6b65 7473 2e70 6174 6368  ge.buckets.patch
-00000ba0: 222c 2020 2020 2020 2020 2022 7265 736f  ",         "reso
-00000bb0: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00000bc0: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-00000bd0: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00000be0: 2e62 7563 6b65 7473 2e73 6574 4961 6d50  .buckets.setIamP
-00000bf0: 6f6c 6963 7922 2c20 2022 7265 736f 7572  olicy",  "resour
-00000c00: 6365 7322 3a20 5b22 4255 434b 4554 225d  ces": ["BUCKET"]
-00000c10: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00000c20: 616d 6522 3a20 2273 746f 7261 6765 2e62  ame": "storage.b
-00000c30: 7563 6b65 7473 2e75 7064 6174 6522 2c20  uckets.update", 
-00000c40: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-00000c50: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
-00000c60: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00000c70: 6522 3a20 2273 746f 7261 6765 2e68 6d61  e": "storage.hma
-00000c80: 634b 6579 2e75 7064 6174 6522 2c20 2020  cKey.update",   
-00000c90: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00000ca0: 3a20 5b22 484d 4143 5f4b 4559 225d 7d2c  : ["HMAC_KEY"]},
-00000cb0: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00000cc0: 6522 3a20 2273 746f 7261 6765 2e6f 626a  e": "storage.obj
-00000cd0: 6563 7473 2e63 6f6d 706f 7365 222c 2020  ects.compose",  
-00000ce0: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00000cf0: 3a20 5b22 4255 434b 4554 222c 2022 4f42  : ["BUCKET", "OB
-00000d00: 4a45 4354 225d 7d2c 0a20 2020 2020 2020  JECT"]},.       
-00000d10: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00000d20: 7261 6765 2e6f 626a 6563 7473 2e63 6f70  rage.objects.cop
-00000d30: 7922 2c20 2020 2020 2020 2020 2022 7265  y",          "re
-00000d40: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00000d50: 4554 222c 2022 4f42 4a45 4354 225d 7d2c  ET", "OBJECT"]},
-00000d60: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00000d70: 6522 3a20 2273 746f 7261 6765 2e6f 626a  e": "storage.obj
-00000d80: 6563 7473 2e64 656c 6574 6522 2c20 2020  ects.delete",   
-00000d90: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00000da0: 3a20 5b22 4255 434b 4554 222c 2022 4f42  : ["BUCKET", "OB
-00000db0: 4a45 4354 225d 7d2c 0a20 2020 2020 2020  JECT"]},.       
-00000dc0: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00000dd0: 7261 6765 2e6f 626a 6563 7473 2e69 6e73  rage.objects.ins
-00000de0: 6572 7422 2c20 2020 2020 2020 2022 7265  ert",        "re
-00000df0: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00000e00: 4554 225d 7d2c 0a20 2020 2020 2020 2020  ET"]},.         
-00000e10: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00000e20: 6765 2e6f 626a 6563 7473 2e70 6174 6368  ge.objects.patch
-00000e30: 222c 2020 2020 2020 2020 2022 7265 736f  ",         "reso
-00000e40: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00000e50: 222c 2022 4f42 4a45 4354 225d 7d2c 0a20  ", "OBJECT"]},. 
-00000e60: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00000e70: 3a20 2273 746f 7261 6765 2e6f 626a 6563  : "storage.objec
-00000e80: 7473 2e72 6577 7269 7465 222c 2020 2020  ts.rewrite",    
-00000e90: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00000ea0: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
-00000eb0: 4354 225d 7d2c 0a20 2020 2020 2020 2020  CT"]},.         
-00000ec0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00000ed0: 6765 2e6f 626a 6563 7473 2e75 7064 6174  ge.objects.updat
-00000ee0: 6522 2c20 2020 2020 2020 2022 7265 736f  e",        "reso
-00000ef0: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00000f00: 222c 2022 4f42 4a45 4354 225d 7d0a 2020  ", "OBJECT"]}.  
-00000f10: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00000f20: 2022 7072 6563 6f6e 6469 7469 6f6e 5072   "preconditionPr
-00000f30: 6f76 6964 6564 223a 2074 7275 652c 0a20  ovided": true,. 
-00000f40: 2020 2020 2020 2022 6578 7065 6374 5375         "expectSu
-00000f50: 6363 6573 7322 3a20 7472 7565 0a20 2020  ccess": true.   
-00000f60: 2020 207d 2c0a 2020 2020 2020 7b0a 2020     },.      {.  
-00000f70: 2020 2020 2020 2269 6422 3a20 332c 0a20        "id": 3,. 
-00000f80: 2020 2020 2020 2022 6465 7363 7269 7074         "descript
-00000f90: 696f 6e22 3a20 2263 6f6e 6469 7469 6f6e  ion": "condition
-00000fa0: 616c 6c79 5f69 6465 6d70 6f74 656e 745f  ally_idempotent_
-00000fb0: 6e6f 5f72 6574 7269 6573 5f77 6865 6e5f  no_retries_when_
-00000fc0: 7072 6563 6f6e 6469 7469 6f6e 5f69 735f  precondition_is_
-00000fd0: 6162 7365 6e74 222c 0a20 2020 2020 2020  absent",.       
-00000fe0: 2022 6361 7365 7322 3a20 5b0a 2020 2020   "cases": [.    
-00000ff0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00001000: 2020 2020 2269 6e73 7472 7563 7469 6f6e      "instruction
-00001010: 7322 3a20 5b22 7265 7475 726e 2d35 3033  s": ["return-503
-00001020: 225d 0a20 2020 2020 2020 2020 207d 2c0a  "].          },.
-00001030: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00001040: 2020 2020 2020 2020 2269 6e73 7472 7563          "instruc
-00001050: 7469 6f6e 7322 3a20 5b22 7265 7475 726e  tions": ["return
-00001060: 2d72 6573 6574 2d63 6f6e 6e65 6374 696f  -reset-connectio
-00001070: 6e22 5d0a 2020 2020 2020 2020 2020 7d0a  n"].          }.
-00001080: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-00001090: 2020 2022 6d65 7468 6f64 7322 3a20 5b0a     "methods": [.
-000010a0: 2020 2020 2020 2020 2020 7b22 6e61 6d65            {"name
-000010b0: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
-000010c0: 6574 732e 7061 7463 6822 2c20 2020 2020  ets.patch",     
-000010d0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
-000010e0: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
-000010f0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-00001100: 2022 7374 6f72 6167 652e 6275 636b 6574   "storage.bucket
-00001110: 732e 7365 7449 616d 506f 6c69 6379 222c  s.setIamPolicy",
-00001120: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
-00001130: 2242 5543 4b45 5422 5d7d 2c0a 2020 2020  "BUCKET"]},.    
-00001140: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
-00001150: 7374 6f72 6167 652e 6275 636b 6574 732e  storage.buckets.
-00001160: 7570 6461 7465 222c 2020 2020 2020 2020  update",        
-00001170: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
-00001180: 5543 4b45 5422 5d7d 2c0a 2020 2020 2020  UCKET"]},.      
-00001190: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
-000011a0: 6f72 6167 652e 686d 6163 4b65 792e 7570  orage.hmacKey.up
-000011b0: 6461 7465 222c 2020 2020 2020 2020 2272  date",        "r
-000011c0: 6573 6f75 7263 6573 223a 205b 2248 4d41  esources": ["HMA
-000011d0: 435f 4b45 5922 5d7d 2c0a 2020 2020 2020  C_KEY"]},.      
-000011e0: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
-000011f0: 6f72 6167 652e 6f62 6a65 6374 732e 636f  orage.objects.co
-00001200: 6d70 6f73 6522 2c20 2020 2020 2020 2272  mpose",       "r
-00001210: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
-00001220: 4b45 5422 2c20 224f 424a 4543 5422 5d7d  KET", "OBJECT"]}
-00001230: 2c0a 2020 2020 2020 2020 2020 7b22 6e61  ,.          {"na
-00001240: 6d65 223a 2022 7374 6f72 6167 652e 6f62  me": "storage.ob
-00001250: 6a65 6374 732e 636f 7079 222c 2020 2020  jects.copy",    
-00001260: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
-00001270: 223a 205b 2242 5543 4b45 5422 2c20 224f  ": ["BUCKET", "O
-00001280: 424a 4543 5422 5d7d 2c0a 2020 2020 2020  BJECT"]},.      
-00001290: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
-000012a0: 6f72 6167 652e 6f62 6a65 6374 732e 6465  orage.objects.de
-000012b0: 6c65 7465 222c 2020 2020 2020 2020 2272  lete",        "r
-000012c0: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
-000012d0: 4b45 5422 2c20 224f 424a 4543 5422 5d7d  KET", "OBJECT"]}
-000012e0: 2c0a 2020 2020 2020 2020 2020 7b22 6e61  ,.          {"na
-000012f0: 6d65 223a 2022 7374 6f72 6167 652e 6f62  me": "storage.ob
-00001300: 6a65 6374 732e 696e 7365 7274 222c 2020  jects.insert",  
-00001310: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
-00001320: 223a 205b 2242 5543 4b45 5422 5d7d 2c0a  ": ["BUCKET"]},.
-00001330: 2020 2020 2020 2020 2020 7b22 6e61 6d65            {"name
-00001340: 223a 2022 7374 6f72 6167 652e 6f62 6a65  ": "storage.obje
-00001350: 6374 732e 7061 7463 6822 2c20 2020 2020  cts.patch",     
-00001360: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
-00001370: 205b 2242 5543 4b45 5422 2c20 224f 424a   ["BUCKET", "OBJ
-00001380: 4543 5422 5d7d 2c0a 2020 2020 2020 2020  ECT"]},.        
-00001390: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
-000013a0: 6167 652e 6f62 6a65 6374 732e 7265 7772  age.objects.rewr
-000013b0: 6974 6522 2c20 2020 2020 2020 2272 6573  ite",       "res
-000013c0: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
-000013d0: 5422 2c20 224f 424a 4543 5422 5d7d 2c0a  T", "OBJECT"]},.
-000013e0: 2020 2020 2020 2020 2020 7b22 6e61 6d65            {"name
-000013f0: 223a 2022 7374 6f72 6167 652e 6f62 6a65  ": "storage.obje
-00001400: 6374 732e 7570 6461 7465 222c 2020 2020  cts.update",    
-00001410: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
-00001420: 205b 2242 5543 4b45 5422 2c20 224f 424a   ["BUCKET", "OBJ
-00001430: 4543 5422 5d7d 0a20 2020 2020 2020 205d  ECT"]}.        ]
-00001440: 2c0a 2020 2020 2020 2020 2270 7265 636f  ,.        "preco
-00001450: 6e64 6974 696f 6e50 726f 7669 6465 6422  nditionProvided"
-00001460: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00001470: 2022 6578 7065 6374 5375 6363 6573 7322   "expectSuccess"
-00001480: 3a20 6661 6c73 650a 2020 2020 2020 7d2c  : false.      },
-00001490: 0a20 2020 2020 207b 0a20 2020 2020 2020  .      {.       
-000014a0: 2022 6964 223a 2034 2c0a 2020 2020 2020   "id": 4,.      
-000014b0: 2020 2264 6573 6372 6970 7469 6f6e 223a    "description":
-000014c0: 2022 6e6f 6e5f 6964 656d 706f 7465 6e74   "non_idempotent
-000014d0: 222c 0a20 2020 2020 2020 2022 6361 7365  ",.        "case
-000014e0: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
-000014f0: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
-00001500: 6e73 7472 7563 7469 6f6e 7322 3a20 5b22  nstructions": ["
-00001510: 7265 7475 726e 2d35 3033 225d 0a20 2020  return-503"].   
-00001520: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00001530: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00001540: 2020 2269 6e73 7472 7563 7469 6f6e 7322    "instructions"
-00001550: 3a20 5b22 7265 7475 726e 2d72 6573 6574  : ["return-reset
-00001560: 2d63 6f6e 6e65 6374 696f 6e22 5d0a 2020  -connection"].  
-00001570: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00001580: 2020 5d2c 0a20 2020 2020 2020 2022 6d65    ],.        "me
-00001590: 7468 6f64 7322 3a20 5b0a 2020 2020 2020  thods": [.      
-000015a0: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
-000015b0: 6f72 6167 652e 6275 636b 6574 5f61 636c  orage.bucket_acl
-000015c0: 2e64 656c 6574 6522 2c20 2020 2020 2020  .delete",       
-000015d0: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
-000015e0: 223a 205b 2242 5543 4b45 5422 5d7d 2c0a  ": ["BUCKET"]},.
-000015f0: 2020 2020 2020 2020 2020 7b22 6e61 6d65            {"name
-00001600: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
-00001610: 6574 5f61 636c 2e69 6e73 6572 7422 2c20  et_acl.insert", 
-00001620: 2020 2020 2020 2020 2020 2020 2272 6573              "res
-00001630: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
-00001640: 5422 5d7d 2c0a 2020 2020 2020 2020 2020  T"]},.          
-00001650: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
-00001660: 652e 6275 636b 6574 5f61 636c 2e70 6174  e.bucket_acl.pat
-00001670: 6368 222c 2020 2020 2020 2020 2020 2020  ch",            
-00001680: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
-00001690: 2242 5543 4b45 5422 5d7d 2c0a 2020 2020  "BUCKET"]},.    
-000016a0: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
-000016b0: 7374 6f72 6167 652e 6275 636b 6574 5f61  storage.bucket_a
-000016c0: 636c 2e75 7064 6174 6522 2c20 2020 2020  cl.update",     
-000016d0: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
-000016e0: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
-000016f0: 2c0a 2020 2020 2020 2020 2020 7b22 6e61  ,.          {"na
-00001700: 6d65 223a 2022 7374 6f72 6167 652e 6465  me": "storage.de
-00001710: 6661 756c 745f 6f62 6a65 6374 5f61 636c  fault_object_acl
-00001720: 2e64 656c 6574 6522 2c20 2020 2020 2272  .delete",     "r
-00001730: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
-00001740: 4b45 5422 5d7d 2c0a 2020 2020 2020 2020  KET"]},.        
-00001750: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
-00001760: 6167 652e 6465 6661 756c 745f 6f62 6a65  age.default_obje
-00001770: 6374 5f61 636c 2e69 6e73 6572 7422 2c20  ct_acl.insert", 
-00001780: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
-00001790: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
-000017a0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-000017b0: 2022 7374 6f72 6167 652e 6465 6661 756c   "storage.defaul
-000017c0: 745f 6f62 6a65 6374 5f61 636c 2e70 6174  t_object_acl.pat
-000017d0: 6368 222c 2020 2020 2020 2272 6573 6f75  ch",      "resou
-000017e0: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
-000017f0: 5d7d 2c0a 2020 2020 2020 2020 2020 7b22  ]},.          {"
-00001800: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
-00001810: 6465 6661 756c 745f 6f62 6a65 6374 5f61  default_object_a
-00001820: 636c 2e75 7064 6174 6522 2c20 2020 2020  cl.update",     
-00001830: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
-00001840: 5543 4b45 5422 5d7d 2c0a 2020 2020 2020  UCKET"]},.      
-00001850: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
-00001860: 6f72 6167 652e 686d 6163 4b65 792e 6372  orage.hmacKey.cr
-00001870: 6561 7465 222c 2020 2020 2020 2020 2020  eate",          
-00001880: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
-00001890: 223a 205b 5d7d 2c0a 2020 2020 2020 2020  ": []},.        
-000018a0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
-000018b0: 6167 652e 6e6f 7469 6669 6361 7469 6f6e  age.notification
-000018c0: 732e 696e 7365 7274 222c 2020 2020 2020  s.insert",      
-000018d0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
-000018e0: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
-000018f0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-00001900: 2022 7374 6f72 6167 652e 6f62 6a65 6374   "storage.object
-00001910: 5f61 636c 2e64 656c 6574 6522 2c20 2020  _acl.delete",   
-00001920: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
-00001930: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
-00001940: 2c20 224f 424a 4543 5422 5d7d 2c0a 2020  , "OBJECT"]},.  
-00001950: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-00001960: 2022 7374 6f72 6167 652e 6f62 6a65 6374   "storage.object
-00001970: 5f61 636c 2e69 6e73 6572 7422 2c20 2020  _acl.insert",   
-00001980: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
-00001990: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
-000019a0: 2c20 224f 424a 4543 5422 5d7d 2c0a 2020  , "OBJECT"]},.  
-000019b0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-000019c0: 2022 7374 6f72 6167 652e 6f62 6a65 6374   "storage.object
-000019d0: 5f61 636c 2e70 6174 6368 222c 2020 2020  _acl.patch",    
-000019e0: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
-000019f0: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
-00001a00: 2c20 224f 424a 4543 5422 5d7d 2c0a 2020  , "OBJECT"]},.  
-00001a10: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
-00001a20: 2022 7374 6f72 6167 652e 6f62 6a65 6374   "storage.object
-00001a30: 5f61 636c 2e75 7064 6174 6522 2c20 2020  _acl.update",   
-00001a40: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
-00001a50: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
-00001a60: 2c20 224f 424a 4543 5422 5d7d 0a20 2020  , "OBJECT"]}.   
-00001a70: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00001a80: 2270 7265 636f 6e64 6974 696f 6e50 726f  "preconditionPro
-00001a90: 7669 6465 6422 3a20 6661 6c73 652c 0a20  vided": false,. 
-00001aa0: 2020 2020 2020 2022 6578 7065 6374 5375         "expectSu
-00001ab0: 6363 6573 7322 3a20 6661 6c73 650a 2020  ccess": false.  
-00001ac0: 2020 2020 7d2c 0a20 2020 2020 207b 0a20      },.      {. 
-00001ad0: 2020 2020 2020 2022 6964 223a 2035 2c0a         "id": 5,.
-00001ae0: 2020 2020 2020 2020 2264 6573 6372 6970          "descrip
-00001af0: 7469 6f6e 223a 2022 6e6f 6e5f 7265 7472  tion": "non_retr
-00001b00: 7961 626c 655f 6572 726f 7273 222c 0a20  yable_errors",. 
-00001b10: 2020 2020 2020 2022 6361 7365 7322 3a20         "cases": 
-00001b20: 5b0a 2020 2020 2020 2020 2020 7b0a 2020  [.          {.  
-00001b30: 2020 2020 2020 2020 2020 2269 6e73 7472            "instr
-00001b40: 7563 7469 6f6e 7322 3a20 5b22 7265 7475  uctions": ["retu
-00001b50: 726e 2d34 3030 225d 0a20 2020 2020 2020  rn-400"].       
-00001b60: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00001b70: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
-00001b80: 6e73 7472 7563 7469 6f6e 7322 3a20 5b22  nstructions": ["
-00001b90: 7265 7475 726e 2d34 3031 225d 0a20 2020  return-401"].   
-00001ba0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00001bb0: 205d 2c0a 2020 2020 2020 2020 226d 6574   ],.        "met
-00001bc0: 686f 6473 223a 205b 0a20 2020 2020 2020  hods": [.       
-00001bd0: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00001be0: 7261 6765 2e62 7563 6b65 745f 6163 6c2e  rage.bucket_acl.
-00001bf0: 6465 6c65 7465 222c 2020 2020 2020 2020  delete",        
-00001c00: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00001c10: 3a20 5b22 4255 434b 4554 225d 7d2c 0a20  : ["BUCKET"]},. 
-00001c20: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00001c30: 3a20 2273 746f 7261 6765 2e62 7563 6b65  : "storage.bucke
-00001c40: 745f 6163 6c2e 6765 7422 2c20 2020 2020  t_acl.get",     
-00001c50: 2020 2020 2020 2020 2020 2022 7265 736f             "reso
-00001c60: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00001c70: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-00001c80: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00001c90: 2e62 7563 6b65 745f 6163 6c2e 696e 7365  .bucket_acl.inse
-00001ca0: 7274 222c 2020 2020 2020 2020 2020 2020  rt",            
-00001cb0: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00001cc0: 4255 434b 4554 225d 7d2c 0a20 2020 2020  BUCKET"]},.     
-00001cd0: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00001ce0: 746f 7261 6765 2e62 7563 6b65 745f 6163  torage.bucket_ac
-00001cf0: 6c2e 6c69 7374 222c 2020 2020 2020 2020  l.list",        
-00001d00: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-00001d10: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
-00001d20: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00001d30: 6522 3a20 2273 746f 7261 6765 2e62 7563  e": "storage.buc
-00001d40: 6b65 745f 6163 6c2e 7061 7463 6822 2c20  ket_acl.patch", 
-00001d50: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00001d60: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00001d70: 4554 225d 7d2c 0a20 2020 2020 2020 2020  ET"]},.         
-00001d80: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00001d90: 6765 2e62 7563 6b65 745f 6163 6c2e 7570  ge.bucket_acl.up
-00001da0: 6461 7465 222c 2020 2020 2020 2020 2020  date",          
-00001db0: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00001dc0: 5b22 4255 434b 4554 225d 7d2c 0a20 2020  ["BUCKET"]},.   
-00001dd0: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00001de0: 2273 746f 7261 6765 2e62 7563 6b65 7473  "storage.buckets
-00001df0: 2e64 656c 6574 6522 2c20 2020 2020 2020  .delete",       
-00001e00: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-00001e10: 6365 7322 3a20 5b22 4255 434b 4554 225d  ces": ["BUCKET"]
-00001e20: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00001e30: 616d 6522 3a20 2273 746f 7261 6765 2e62  ame": "storage.b
-00001e40: 7563 6b65 7473 2e67 6574 222c 2020 2020  uckets.get",    
-00001e50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00001e60: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00001e70: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
-00001e80: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00001e90: 7261 6765 2e62 7563 6b65 7473 2e67 6574  rage.buckets.get
-00001ea0: 4961 6d50 6f6c 6963 7922 2c20 2020 2020  IamPolicy",     
-00001eb0: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00001ec0: 3a20 5b22 4255 434b 4554 225d 7d2c 0a20  : ["BUCKET"]},. 
-00001ed0: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00001ee0: 3a20 2273 746f 7261 6765 2e62 7563 6b65  : "storage.bucke
-00001ef0: 7473 2e69 6e73 6572 7422 2c20 2020 2020  ts.insert",     
-00001f00: 2020 2020 2020 2020 2020 2022 7265 736f             "reso
-00001f10: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00001f20: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-00001f30: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00001f40: 2e62 7563 6b65 7473 2e6c 6973 7422 2c20  .buckets.list", 
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00001f70: 4255 434b 4554 225d 7d2c 0a20 2020 2020  BUCKET"]},.     
-00001f80: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00001f90: 746f 7261 6765 2e62 7563 6b65 7473 2e6c  torage.buckets.l
-00001fa0: 6f63 6b52 6574 656e 7469 6f6e 506f 6c69  ockRetentionPoli
-00001fb0: 6379 222c 2020 2022 7265 736f 7572 6365  cy",   "resource
-00001fc0: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
-00001fd0: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00001fe0: 6522 3a20 2273 746f 7261 6765 2e62 7563  e": "storage.buc
-00001ff0: 6b65 7473 2e70 6174 6368 222c 2020 2020  kets.patch",    
-00002000: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00002010: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00002020: 4554 225d 7d2c 0a20 2020 2020 2020 2020  ET"]},.         
-00002030: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00002040: 6765 2e62 7563 6b65 7473 2e73 6574 4961  ge.buckets.setIa
-00002050: 6d50 6f6c 6963 7922 2c20 2020 2020 2020  mPolicy",       
-00002060: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00002070: 5b22 4255 434b 4554 225d 7d2c 0a20 2020  ["BUCKET"]},.   
-00002080: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00002090: 2273 746f 7261 6765 2e62 7563 6b65 7473  "storage.buckets
-000020a0: 2e74 6573 7449 616d 5065 726d 6973 7369  .testIamPermissi
-000020b0: 6f6e 7322 2c20 2020 2022 7265 736f 7572  ons",    "resour
-000020c0: 6365 7322 3a20 5b22 4255 434b 4554 225d  ces": ["BUCKET"]
-000020d0: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-000020e0: 616d 6522 3a20 2273 746f 7261 6765 2e62  ame": "storage.b
-000020f0: 7563 6b65 7473 2e75 7064 6174 6522 2c20  uckets.update", 
-00002100: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002110: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00002120: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
-00002130: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00002140: 7261 6765 2e64 6566 6175 6c74 5f6f 626a  rage.default_obj
-00002150: 6563 745f 6163 6c2e 6465 6c65 7465 222c  ect_acl.delete",
-00002160: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00002170: 3a20 5b22 4255 434b 4554 225d 7d2c 0a20  : ["BUCKET"]},. 
-00002180: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00002190: 3a20 2273 746f 7261 6765 2e64 6566 6175  : "storage.defau
-000021a0: 6c74 5f6f 626a 6563 745f 6163 6c2e 6765  lt_object_acl.ge
-000021b0: 7422 2c20 2020 2020 2020 2022 7265 736f  t",        "reso
-000021c0: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-000021d0: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-000021e0: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-000021f0: 2e64 6566 6175 6c74 5f6f 626a 6563 745f  .default_object_
-00002200: 6163 6c2e 696e 7365 7274 222c 2020 2020  acl.insert",    
-00002210: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00002220: 4255 434b 4554 225d 7d2c 0a20 2020 2020  BUCKET"]},.     
-00002230: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00002240: 746f 7261 6765 2e64 6566 6175 6c74 5f6f  torage.default_o
-00002250: 626a 6563 745f 6163 6c2e 6c69 7374 222c  bject_acl.list",
-00002260: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-00002270: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
-00002280: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00002290: 6522 3a20 2273 746f 7261 6765 2e64 6566  e": "storage.def
-000022a0: 6175 6c74 5f6f 626a 6563 745f 6163 6c2e  ault_object_acl.
-000022b0: 7061 7463 6822 2c20 2020 2020 2022 7265  patch",      "re
-000022c0: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-000022d0: 4554 225d 7d2c 0a20 2020 2020 2020 2020  ET"]},.         
-000022e0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-000022f0: 6765 2e64 6566 6175 6c74 5f6f 626a 6563  ge.default_objec
-00002300: 745f 6163 6c2e 7570 6461 7465 222c 2020  t_acl.update",  
-00002310: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00002320: 5b22 4255 434b 4554 225d 7d2c 0a20 2020  ["BUCKET"]},.   
-00002330: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00002340: 2273 746f 7261 6765 2e68 6d61 634b 6579  "storage.hmacKey
-00002350: 2e63 7265 6174 6522 2c20 2020 2020 2020  .create",       
-00002360: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-00002370: 6365 7322 3a20 5b5d 7d2c 0a20 2020 2020  ces": []},.     
-00002380: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00002390: 746f 7261 6765 2e68 6d61 634b 6579 2e64  torage.hmacKey.d
-000023a0: 656c 6574 6522 2c20 2020 2020 2020 2020  elete",         
-000023b0: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-000023c0: 7322 3a20 5b22 484d 4143 5f4b 4559 225d  s": ["HMAC_KEY"]
-000023d0: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-000023e0: 616d 6522 3a20 2273 746f 7261 6765 2e68  ame": "storage.h
-000023f0: 6d61 634b 6579 2e67 6574 222c 2020 2020  macKey.get",    
-00002400: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002410: 7265 736f 7572 6365 7322 3a20 5b22 484d  resources": ["HM
-00002420: 4143 5f4b 4559 225d 7d2c 0a20 2020 2020  AC_KEY"]},.     
-00002430: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00002440: 746f 7261 6765 2e68 6d61 634b 6579 2e6c  torage.hmacKey.l
-00002450: 6973 7422 2c20 2020 2020 2020 2020 2020  ist",           
-00002460: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-00002470: 7322 3a20 5b22 484d 4143 5f4b 4559 225d  s": ["HMAC_KEY"]
-00002480: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00002490: 616d 6522 3a20 2273 746f 7261 6765 2e68  ame": "storage.h
-000024a0: 6d61 634b 6579 2e75 7064 6174 6522 2c20  macKey.update", 
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000024c0: 7265 736f 7572 6365 7322 3a20 5b22 484d  resources": ["HM
-000024d0: 4143 5f4b 4559 225d 7d2c 0a20 2020 2020  AC_KEY"]},.     
-000024e0: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-000024f0: 746f 7261 6765 2e6e 6f74 6966 6963 6174  torage.notificat
-00002500: 696f 6e73 2e64 656c 6574 6522 2c20 2020  ions.delete",   
-00002510: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-00002520: 7322 3a20 5b22 4255 434b 4554 222c 2022  s": ["BUCKET", "
-00002530: 4e4f 5449 4649 4341 5449 4f4e 225d 7d2c  NOTIFICATION"]},
-00002540: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00002550: 6522 3a20 2273 746f 7261 6765 2e6e 6f74  e": "storage.not
-00002560: 6966 6963 6174 696f 6e73 2e67 6574 222c  ifications.get",
-00002570: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-00002580: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00002590: 4554 222c 2022 4e4f 5449 4649 4341 5449  ET", "NOTIFICATI
-000025a0: 4f4e 225d 7d2c 0a20 2020 2020 2020 2020  ON"]},.         
-000025b0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-000025c0: 6765 2e6e 6f74 6966 6963 6174 696f 6e73  ge.notifications
-000025d0: 2e69 6e73 6572 7422 2c20 2020 2020 2020  .insert",       
-000025e0: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-000025f0: 5b22 4255 434b 4554 222c 2022 4e4f 5449  ["BUCKET", "NOTI
-00002600: 4649 4341 5449 4f4e 225d 7d2c 0a20 2020  FICATION"]},.   
-00002610: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00002620: 2273 746f 7261 6765 2e6e 6f74 6966 6963  "storage.notific
-00002630: 6174 696f 6e73 2e6c 6973 7422 2c20 2020  ations.list",   
-00002640: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-00002650: 6365 7322 3a20 5b22 4255 434b 4554 222c  ces": ["BUCKET",
-00002660: 2022 4e4f 5449 4649 4341 5449 4f4e 225d   "NOTIFICATION"]
-00002670: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00002680: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-00002690: 626a 6563 745f 6163 6c2e 6465 6c65 7465  bject_acl.delete
-000026a0: 222c 2020 2020 2020 2020 2020 2020 2022  ",             "
-000026b0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-000026c0: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-000026d0: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-000026e0: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-000026f0: 626a 6563 745f 6163 6c2e 6765 7422 2c20  bject_acl.get", 
-00002700: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002710: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00002720: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-00002730: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00002740: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-00002750: 626a 6563 745f 6163 6c2e 696e 7365 7274  bject_acl.insert
-00002760: 222c 2020 2020 2020 2020 2020 2020 2022  ",             "
-00002770: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00002780: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-00002790: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-000027a0: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-000027b0: 626a 6563 745f 6163 6c2e 6c69 7374 222c  bject_acl.list",
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000027d0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-000027e0: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-000027f0: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00002800: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-00002810: 626a 6563 745f 6163 6c2e 7061 7463 6822  bject_acl.patch"
-00002820: 2c20 2020 2020 2020 2020 2020 2020 2022  ,              "
-00002830: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00002840: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-00002850: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00002860: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-00002870: 626a 6563 745f 6163 6c2e 7570 6461 7465  bject_acl.update
-00002880: 222c 2020 2020 2020 2020 2020 2020 2022  ",             "
-00002890: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-000028a0: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-000028b0: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-000028c0: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-000028d0: 626a 6563 7473 2e63 6f6d 706f 7365 222c  bjects.compose",
-000028e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000028f0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00002900: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-00002910: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00002920: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-00002930: 626a 6563 7473 2e63 6f70 7922 2c20 2020  bjects.copy",   
-00002940: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002950: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00002960: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-00002970: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00002980: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-00002990: 626a 6563 7473 2e64 656c 6574 6522 2c20  bjects.delete", 
-000029a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000029b0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-000029c0: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-000029d0: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-000029e0: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-000029f0: 626a 6563 7473 2e67 6574 222c 2020 2020  bjects.get",    
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002a10: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00002a20: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
-00002a30: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-00002a40: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
-00002a50: 626a 6563 7473 2e69 6e73 6572 7422 2c20  bjects.insert", 
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002a70: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-00002a80: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
-00002a90: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00002aa0: 7261 6765 2e6f 626a 6563 7473 2e6c 6973  rage.objects.lis
-00002ab0: 7422 2c20 2020 2020 2020 2020 2020 2020  t",             
-00002ac0: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00002ad0: 3a20 5b22 4255 434b 4554 222c 2022 4f42  : ["BUCKET", "OB
-00002ae0: 4a45 4354 225d 7d2c 0a20 2020 2020 2020  JECT"]},.       
-00002af0: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00002b00: 7261 6765 2e6f 626a 6563 7473 2e70 6174  rage.objects.pat
-00002b10: 6368 222c 2020 2020 2020 2020 2020 2020  ch",            
-00002b20: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00002b30: 3a20 5b22 4255 434b 4554 222c 2022 4f42  : ["BUCKET", "OB
-00002b40: 4a45 4354 225d 7d2c 0a20 2020 2020 2020  JECT"]},.       
-00002b50: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00002b60: 7261 6765 2e6f 626a 6563 7473 2e72 6577  rage.objects.rew
-00002b70: 7269 7465 222c 2020 2020 2020 2020 2020  rite",          
-00002b80: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00002b90: 3a20 5b22 4255 434b 4554 222c 2022 4f42  : ["BUCKET", "OB
-00002ba0: 4a45 4354 225d 7d2c 0a20 2020 2020 2020  JECT"]},.       
-00002bb0: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00002bc0: 7261 6765 2e6f 626a 6563 7473 2e75 7064  rage.objects.upd
-00002bd0: 6174 6522 2c20 2020 2020 2020 2020 2020  ate",           
-00002be0: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00002bf0: 3a20 5b22 4255 434b 4554 222c 2022 4f42  : ["BUCKET", "OB
-00002c00: 4a45 4354 225d 7d2c 0a20 2020 2020 2020  JECT"]},.       
-00002c10: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00002c20: 7261 6765 2e73 6572 7669 6365 6163 636f  rage.serviceacco
-00002c30: 756e 742e 6765 7422 2c20 2020 2020 2020  unt.get",       
-00002c40: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00002c50: 3a20 5b5d 7d0a 2020 2020 2020 2020 5d2c  : []}.        ],
-00002c60: 0a20 2020 2020 2020 2022 7072 6563 6f6e  .        "precon
-00002c70: 6469 7469 6f6e 5072 6f76 6964 6564 223a  ditionProvided":
-00002c80: 2066 616c 7365 2c0a 2020 2020 2020 2020   false,.        
-00002c90: 2265 7870 6563 7453 7563 6365 7373 223a  "expectSuccess":
-00002ca0: 2066 616c 7365 0a20 2020 2020 207d 2c0a   false.      },.
-00002cb0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00002cc0: 2269 6422 3a20 362c 0a20 2020 2020 2020  "id": 6,.       
-00002cd0: 2022 6465 7363 7269 7074 696f 6e22 3a20   "description": 
-00002ce0: 226d 6978 5f72 6574 7279 6162 6c65 5f6e  "mix_retryable_n
-00002cf0: 6f6e 5f72 6574 7279 6162 6c65 5f65 7272  on_retryable_err
-00002d00: 6f72 7322 2c0a 2020 2020 2020 2020 2263  ors",.        "c
-00002d10: 6173 6573 223a 205b 0a20 2020 2020 2020  ases": [.       
-00002d20: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00002d30: 2022 696e 7374 7275 6374 696f 6e73 223a   "instructions":
-00002d40: 205b 2272 6574 7572 6e2d 3530 3322 2c20   ["return-503", 
-00002d50: 2272 6574 7572 6e2d 3430 3022 5d0a 2020  "return-400"].  
-00002d60: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002d70: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00002d80: 2020 2022 696e 7374 7275 6374 696f 6e73     "instructions
-00002d90: 223a 205b 2272 6574 7572 6e2d 7265 7365  ": ["return-rese
-00002da0: 742d 636f 6e6e 6563 7469 6f6e 222c 2022  t-connection", "
-00002db0: 7265 7475 726e 2d34 3031 225d 0a20 2020  return-401"].   
-00002dc0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00002dd0: 205d 2c0a 2020 2020 2020 2020 226d 6574   ],.        "met
-00002de0: 686f 6473 223a 205b 0a20 2020 2020 2020  hods": [.       
-00002df0: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00002e00: 7261 6765 2e62 7563 6b65 745f 6163 6c2e  rage.bucket_acl.
-00002e10: 6765 7422 2c20 2020 2020 2020 2020 2020  get",           
-00002e20: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00002e30: 3a20 5b22 4255 434b 4554 225d 7d2c 0a20  : ["BUCKET"]},. 
-00002e40: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00002e50: 3a20 2273 746f 7261 6765 2e62 7563 6b65  : "storage.bucke
-00002e60: 745f 6163 6c2e 6c69 7374 222c 2020 2020  t_acl.list",    
-00002e70: 2020 2020 2020 2020 2020 2022 7265 736f             "reso
-00002e80: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00002e90: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-00002ea0: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00002eb0: 2e62 7563 6b65 7473 2e64 656c 6574 6522  .buckets.delete"
-00002ec0: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00002ed0: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00002ee0: 4255 434b 4554 225d 7d2c 0a20 2020 2020  BUCKET"]},.     
-00002ef0: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00002f00: 746f 7261 6765 2e62 7563 6b65 7473 2e67  torage.buckets.g
-00002f10: 6574 222c 2020 2020 2020 2020 2020 2020  et",            
-00002f20: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-00002f30: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
-00002f40: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-00002f50: 6522 3a20 2273 746f 7261 6765 2e62 7563  e": "storage.buc
-00002f60: 6b65 7473 2e67 6574 4961 6d50 6f6c 6963  kets.getIamPolic
-00002f70: 7922 2c20 2020 2020 2020 2020 2022 7265  y",          "re
-00002f80: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00002f90: 4554 225d 7d2c 0a20 2020 2020 2020 2020  ET"]},.         
-00002fa0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00002fb0: 6765 2e62 7563 6b65 7473 2e69 6e73 6572  ge.buckets.inser
-00002fc0: 7422 2c20 2020 2020 2020 2020 2020 2020  t",             
-00002fd0: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00002fe0: 5b5d 7d2c 0a20 2020 2020 2020 2020 207b  []},.          {
-00002ff0: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00003000: 2e62 7563 6b65 7473 2e6c 6973 7422 2c20  .buckets.list", 
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00003030: 4255 434b 4554 225d 7d2c 0a20 2020 2020  BUCKET"]},.     
-00003040: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00003050: 746f 7261 6765 2e62 7563 6b65 7473 2e6c  torage.buckets.l
-00003060: 6f63 6b52 6574 656e 7469 6f6e 506f 6c69  ockRetentionPoli
-00003070: 6379 222c 2020 2022 7265 736f 7572 6365  cy",   "resource
-00003080: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
-00003090: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-000030a0: 6522 3a20 2273 746f 7261 6765 2e62 7563  e": "storage.buc
-000030b0: 6b65 7473 2e70 6174 6368 222c 2020 2020  kets.patch",    
-000030c0: 2020 2020 2020 2020 2020 2020 2022 7265               "re
-000030d0: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-000030e0: 4554 225d 7d2c 0a20 2020 2020 2020 2020  ET"]},.         
-000030f0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00003100: 6765 2e62 7563 6b65 7473 2e73 6574 4961  ge.buckets.setIa
-00003110: 6d50 6f6c 6963 7922 2c20 2020 2020 2020  mPolicy",       
-00003120: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00003130: 5b22 4255 434b 4554 225d 7d2c 0a20 2020  ["BUCKET"]},.   
-00003140: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00003150: 2273 746f 7261 6765 2e62 7563 6b65 7473  "storage.buckets
-00003160: 2e74 6573 7449 616d 5065 726d 6973 7369  .testIamPermissi
-00003170: 6f6e 7322 2c20 2020 2022 7265 736f 7572  ons",    "resour
-00003180: 6365 7322 3a20 5b22 4255 434b 4554 225d  ces": ["BUCKET"]
-00003190: 7d2c 0a20 2020 2020 2020 2020 207b 226e  },.          {"n
-000031a0: 616d 6522 3a20 2273 746f 7261 6765 2e62  ame": "storage.b
-000031b0: 7563 6b65 7473 2e75 7064 6174 6522 2c20  uckets.update", 
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000031d0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
-000031e0: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
-000031f0: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
-00003200: 7261 6765 2e64 6566 6175 6c74 5f6f 626a  rage.default_obj
-00003210: 6563 745f 6163 6c2e 6765 7422 2c20 2020  ect_acl.get",   
-00003220: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
-00003230: 3a20 5b22 4255 434b 4554 225d 7d2c 0a20  : ["BUCKET"]},. 
-00003240: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00003250: 3a20 2273 746f 7261 6765 2e64 6566 6175  : "storage.defau
-00003260: 6c74 5f6f 626a 6563 745f 6163 6c2e 6c69  lt_object_acl.li
-00003270: 7374 222c 2020 2020 2020 2022 7265 736f  st",       "reso
-00003280: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
-00003290: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-000032a0: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-000032b0: 2e68 6d61 634b 6579 2e64 656c 6574 6522  .hmacKey.delete"
-000032c0: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-000032d0: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-000032e0: 484d 4143 5f4b 4559 225d 7d2c 0a20 2020  HMAC_KEY"]},.   
-000032f0: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00003300: 2273 746f 7261 6765 2e68 6d61 634b 6579  "storage.hmacKey
-00003310: 2e67 6574 222c 2020 2020 2020 2020 2020  .get",          
-00003320: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-00003330: 6365 7322 3a20 5b22 484d 4143 5f4b 4559  ces": ["HMAC_KEY
-00003340: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-00003350: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00003360: 2e68 6d61 634b 6579 2e6c 6973 7422 2c20  .hmacKey.list", 
-00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003380: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00003390: 484d 4143 5f4b 4559 225d 7d2c 0a20 2020  HMAC_KEY"]},.   
-000033a0: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-000033b0: 2273 746f 7261 6765 2e68 6d61 634b 6579  "storage.hmacKey
-000033c0: 2e75 7064 6174 6522 2c20 2020 2020 2020  .update",       
-000033d0: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-000033e0: 6365 7322 3a20 5b22 484d 4143 5f4b 4559  ces": ["HMAC_KEY
-000033f0: 225d 7d2c 0a20 2020 2020 2020 2020 207b  "]},.          {
-00003400: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
-00003410: 2e6e 6f74 6966 6963 6174 696f 6e73 2e64  .notifications.d
-00003420: 656c 6574 6522 2c20 2020 2020 2020 2020  elete",         
-00003430: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00003440: 4255 434b 4554 222c 2022 4e4f 5449 4649  BUCKET", "NOTIFI
-00003450: 4341 5449 4f4e 225d 7d2c 0a20 2020 2020  CATION"]},.     
-00003460: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
-00003470: 746f 7261 6765 2e6e 6f74 6966 6963 6174  torage.notificat
-00003480: 696f 6e73 2e67 6574 222c 2020 2020 2020  ions.get",      
-00003490: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-000034a0: 7322 3a20 5b22 4255 434b 4554 222c 2022  s": ["BUCKET", "
-000034b0: 4e4f 5449 4649 4341 5449 4f4e 225d 7d2c  NOTIFICATION"]},
-000034c0: 0a20 2020 2020 2020 2020 207b 226e 616d  .          {"nam
-000034d0: 6522 3a20 2273 746f 7261 6765 2e6e 6f74  e": "storage.not
-000034e0: 6966 6963 6174 696f 6e73 2e6c 6973 7422  ifications.list"
-000034f0: 2c20 2020 2020 2020 2020 2020 2022 7265  ,            "re
-00003500: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
-00003510: 4554 222c 2022 4e4f 5449 4649 4341 5449  ET", "NOTIFICATI
-00003520: 4f4e 225d 7d2c 0a20 2020 2020 2020 2020  ON"]},.         
-00003530: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00003540: 6765 2e6f 626a 6563 745f 6163 6c2e 6765  ge.object_acl.ge
-00003550: 7422 2c20 2020 2020 2020 2020 2020 2020  t",             
-00003560: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00003570: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
-00003580: 4354 225d 7d2c 0a20 2020 2020 2020 2020  CT"]},.         
-00003590: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-000035a0: 6765 2e6f 626a 6563 745f 6163 6c2e 6c69  ge.object_acl.li
-000035b0: 7374 222c 2020 2020 2020 2020 2020 2020  st",            
-000035c0: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-000035d0: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
-000035e0: 4354 225d 7d2c 0a20 2020 2020 2020 2020  CT"]},.         
-000035f0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00003600: 6765 2e6f 626a 6563 7473 2e63 6f6d 706f  ge.objects.compo
-00003610: 7365 222c 2020 2020 2020 2020 2020 2020  se",            
-00003620: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00003630: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
-00003640: 4354 225d 7d2c 0a20 2020 2020 2020 2020  CT"]},.         
-00003650: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00003660: 6765 2e6f 626a 6563 7473 2e63 6f70 7922  ge.objects.copy"
+00000000: 7b0a 2020 2272 6574 7279 5465 7374 7322  {.  "retryTests"
+00000010: 3a20 5b0a 2020 2020 7b0a 2020 2020 2020  : [.    {.      
+00000020: 2269 6422 3a20 312c 0a20 2020 2020 2022  "id": 1,.      "
+00000030: 6465 7363 7269 7074 696f 6e22 3a20 2261  description": "a
+00000040: 6c77 6179 735f 6964 656d 706f 7465 6e74  lways_idempotent
+00000050: 222c 0a20 2020 2020 2022 6361 7365 7322  ",.      "cases"
+00000060: 3a20 5b0a 2020 2020 2020 2020 7b0a 2020  : [.        {.  
+00000070: 2020 2020 2020 2020 2269 6e73 7472 7563          "instruc
+00000080: 7469 6f6e 7322 3a20 5b22 7265 7475 726e  tions": ["return
+00000090: 2d35 3033 222c 2022 7265 7475 726e 2d35  -503", "return-5
+000000a0: 3033 225d 0a20 2020 2020 2020 207d 2c0a  03"].        },.
+000000b0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000000c0: 2020 2020 2269 6e73 7472 7563 7469 6f6e      "instruction
+000000d0: 7322 3a20 5b22 7265 7475 726e 2d72 6573  s": ["return-res
+000000e0: 6574 2d63 6f6e 6e65 6374 696f 6e22 2c20  et-connection", 
+000000f0: 2272 6574 7572 6e2d 7265 7365 742d 636f  "return-reset-co
+00000100: 6e6e 6563 7469 6f6e 225d 0a20 2020 2020  nnection"].     
+00000110: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00000120: 2020 2020 2020 2020 2020 2269 6e73 7472            "instr
+00000130: 7563 7469 6f6e 7322 3a20 5b22 7265 7475  uctions": ["retu
+00000140: 726e 2d72 6573 6574 2d63 6f6e 6e65 6374  rn-reset-connect
+00000150: 696f 6e22 2c20 2272 6574 7572 6e2d 3530  ion", "return-50
+00000160: 3322 5d0a 2020 2020 2020 2020 7d0a 2020  3"].        }.  
+00000170: 2020 2020 5d2c 0a20 2020 2020 2022 6d65      ],.      "me
+00000180: 7468 6f64 7322 3a20 5b0a 2020 2020 2020  thods": [.      
+00000190: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000001a0: 6167 652e 6275 636b 6574 5f61 636c 2e67  age.bucket_acl.g
+000001b0: 6574 222c 2020 2020 2020 2020 2020 2020  et",            
+000001c0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+000001d0: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
+000001e0: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+000001f0: 7374 6f72 6167 652e 6275 636b 6574 5f61  storage.bucket_a
+00000200: 636c 2e6c 6973 7422 2c20 2020 2020 2020  cl.list",       
+00000210: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00000220: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
+00000230: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00000240: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
+00000250: 6574 732e 6465 6c65 7465 222c 2020 2020  ets.delete",    
+00000260: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+00000270: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00000280: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00000290: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+000002a0: 6275 636b 6574 732e 6765 7422 2c20 2020  buckets.get",   
+000002b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000002c0: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+000002d0: 5543 4b45 5422 5d7d 2c0a 2020 2020 2020  UCKET"]},.      
+000002e0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000002f0: 6167 652e 6275 636b 6574 732e 6765 7449  age.buckets.getI
+00000300: 616d 506f 6c69 6379 222c 2020 2020 2020  amPolicy",      
+00000310: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+00000320: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
+00000330: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00000340: 7374 6f72 6167 652e 6275 636b 6574 732e  storage.buckets.
+00000350: 696e 7365 7274 222c 2020 2020 2020 2020  insert",        
+00000360: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00000370: 6573 223a 205b 5d7d 2c0a 2020 2020 2020  es": []},.      
+00000380: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+00000390: 6167 652e 6275 636b 6574 732e 6c69 7374  age.buckets.list
+000003a0: 222c 2020 2020 2020 2020 2020 2020 2020  ",              
+000003b0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+000003c0: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
+000003d0: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+000003e0: 7374 6f72 6167 652e 6275 636b 6574 732e  storage.buckets.
+000003f0: 6c6f 636b 5265 7465 6e74 696f 6e50 6f6c  lockRetentionPol
+00000400: 6963 7922 2c20 2020 2272 6573 6f75 7263  icy",   "resourc
+00000410: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
+00000420: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00000430: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
+00000440: 6574 732e 7465 7374 4961 6d50 6572 6d69  ets.testIamPermi
+00000450: 7373 696f 6e73 222c 2020 2020 2272 6573  ssions",    "res
+00000460: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00000470: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00000480: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00000490: 6465 6661 756c 745f 6f62 6a65 6374 5f61  default_object_a
+000004a0: 636c 2e67 6574 222c 2020 2020 2020 2020  cl.get",        
+000004b0: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+000004c0: 5543 4b45 5422 5d7d 2c0a 2020 2020 2020  UCKET"]},.      
+000004d0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000004e0: 6167 652e 6465 6661 756c 745f 6f62 6a65  age.default_obje
+000004f0: 6374 5f61 636c 2e6c 6973 7422 2c20 2020  ct_acl.list",   
+00000500: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+00000510: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
+00000520: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00000530: 7374 6f72 6167 652e 686d 6163 4b65 792e  storage.hmacKey.
+00000540: 6465 6c65 7465 222c 2020 2020 2020 2020  delete",        
+00000550: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00000560: 6573 223a 205b 2248 4d41 435f 4b45 5922  es": ["HMAC_KEY"
+00000570: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00000580: 6d65 223a 2022 7374 6f72 6167 652e 686d  me": "storage.hm
+00000590: 6163 4b65 792e 6765 7422 2c20 2020 2020  acKey.get",     
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+000005b0: 6573 6f75 7263 6573 223a 205b 2248 4d41  esources": ["HMA
+000005c0: 435f 4b45 5922 5d7d 2c0a 2020 2020 2020  C_KEY"]},.      
+000005d0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000005e0: 6167 652e 686d 6163 4b65 792e 6c69 7374  age.hmacKey.list
+000005f0: 222c 2020 2020 2020 2020 2020 2020 2020  ",              
+00000600: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+00000610: 205b 2248 4d41 435f 4b45 5922 5d7d 2c0a   ["HMAC_KEY"]},.
+00000620: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00000630: 2022 7374 6f72 6167 652e 6e6f 7469 6669   "storage.notifi
+00000640: 6361 7469 6f6e 732e 6465 6c65 7465 222c  cations.delete",
+00000650: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00000660: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+00000670: 2c20 224e 4f54 4946 4943 4154 494f 4e22  , "NOTIFICATION"
+00000680: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00000690: 6d65 223a 2022 7374 6f72 6167 652e 6e6f  me": "storage.no
+000006a0: 7469 6669 6361 7469 6f6e 732e 6765 7422  tifications.get"
+000006b0: 2c20 2020 2020 2020 2020 2020 2020 2272  ,             "r
+000006c0: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+000006d0: 4b45 5422 2c20 224e 4f54 4946 4943 4154  KET", "NOTIFICAT
+000006e0: 494f 4e22 5d7d 2c0a 2020 2020 2020 2020  ION"]},.        
+000006f0: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00000700: 652e 6e6f 7469 6669 6361 7469 6f6e 732e  e.notifications.
+00000710: 6c69 7374 222c 2020 2020 2020 2020 2020  list",          
+00000720: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00000730: 2242 5543 4b45 5422 2c20 224e 4f54 4946  "BUCKET", "NOTIF
+00000740: 4943 4154 494f 4e22 5d7d 2c0a 2020 2020  ICATION"]},.    
+00000750: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00000760: 6f72 6167 652e 6f62 6a65 6374 5f61 636c  orage.object_acl
+00000770: 2e67 6574 222c 2020 2020 2020 2020 2020  .get",          
+00000780: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00000790: 223a 205b 2242 5543 4b45 5422 2c20 224f  ": ["BUCKET", "O
+000007a0: 424a 4543 5422 5d7d 2c0a 2020 2020 2020  BJECT"]},.      
+000007b0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000007c0: 6167 652e 6f62 6a65 6374 5f61 636c 2e6c  age.object_acl.l
+000007d0: 6973 7422 2c20 2020 2020 2020 2020 2020  ist",           
+000007e0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+000007f0: 205b 2242 5543 4b45 5422 2c20 224f 424a   ["BUCKET", "OBJ
+00000800: 4543 5422 5d7d 2c0a 2020 2020 2020 2020  ECT"]},.        
+00000810: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00000820: 652e 6f62 6a65 6374 732e 6765 7422 2c20  e.objects.get", 
+00000830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000840: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00000850: 2242 5543 4b45 5422 2c20 224f 424a 4543  "BUCKET", "OBJEC
+00000860: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00000870: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00000880: 6f62 6a65 6374 732e 6c69 7374 222c 2020  objects.list",  
+00000890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008a0: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+000008b0: 5543 4b45 5422 2c20 224f 424a 4543 5422  UCKET", "OBJECT"
+000008c0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+000008d0: 6d65 223a 2022 7374 6f72 6167 652e 7365  me": "storage.se
+000008e0: 7276 6963 6561 6363 6f75 6e74 2e67 6574  rviceaccount.get
+000008f0: 222c 2020 2020 2020 2020 2020 2020 2272  ",            "r
+00000900: 6573 6f75 7263 6573 223a 205b 5d7d 0a20  esources": []}. 
+00000910: 2020 2020 205d 2c0a 2020 2020 2020 2270       ],.      "p
+00000920: 7265 636f 6e64 6974 696f 6e50 726f 7669  reconditionProvi
+00000930: 6465 6422 3a20 6661 6c73 652c 0a20 2020  ded": false,.   
+00000940: 2020 2022 6578 7065 6374 5375 6363 6573     "expectSucces
+00000950: 7322 3a20 7472 7565 0a20 2020 207d 2c0a  s": true.    },.
+00000960: 2020 2020 7b0a 2020 2020 2020 2269 6422      {.      "id"
+00000970: 3a20 322c 0a20 2020 2020 2022 6465 7363  : 2,.      "desc
+00000980: 7269 7074 696f 6e22 3a20 2263 6f6e 6469  ription": "condi
+00000990: 7469 6f6e 616c 6c79 5f69 6465 6d70 6f74  tionally_idempot
+000009a0: 656e 745f 7265 7472 6965 735f 7768 656e  ent_retries_when
+000009b0: 5f70 7265 636f 6e64 6974 696f 6e5f 6973  _precondition_is
+000009c0: 5f70 7265 7365 6e74 222c 0a20 2020 2020  _present",.     
+000009d0: 2022 6361 7365 7322 3a20 5b0a 2020 2020   "cases": [.    
+000009e0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+000009f0: 2269 6e73 7472 7563 7469 6f6e 7322 3a20  "instructions": 
+00000a00: 5b22 7265 7475 726e 2d35 3033 222c 2022  ["return-503", "
+00000a10: 7265 7475 726e 2d35 3033 225d 0a20 2020  return-503"].   
+00000a20: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000a30: 7b0a 2020 2020 2020 2020 2020 2269 6e73  {.          "ins
+00000a40: 7472 7563 7469 6f6e 7322 3a20 5b22 7265  tructions": ["re
+00000a50: 7475 726e 2d72 6573 6574 2d63 6f6e 6e65  turn-reset-conne
+00000a60: 6374 696f 6e22 2c20 2272 6574 7572 6e2d  ction", "return-
+00000a70: 7265 7365 742d 636f 6e6e 6563 7469 6f6e  reset-connection
+00000a80: 225d 0a20 2020 2020 2020 207d 2c0a 2020  "].        },.  
+00000a90: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00000aa0: 2020 2269 6e73 7472 7563 7469 6f6e 7322    "instructions"
+00000ab0: 3a20 5b22 7265 7475 726e 2d72 6573 6574  : ["return-reset
+00000ac0: 2d63 6f6e 6e65 6374 696f 6e22 2c20 2272  -connection", "r
+00000ad0: 6574 7572 6e2d 3530 3322 5d0a 2020 2020  eturn-503"].    
+00000ae0: 2020 2020 7d0a 2020 2020 2020 5d2c 0a20      }.      ],. 
+00000af0: 2020 2020 2022 6d65 7468 6f64 7322 3a20       "methods": 
+00000b00: 5b0a 2020 2020 2020 2020 7b22 6e61 6d65  [.        {"name
+00000b10: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
+00000b20: 6574 732e 7061 7463 6822 2c20 2020 2020  ets.patch",     
+00000b30: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+00000b40: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
+00000b50: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00000b60: 7374 6f72 6167 652e 6275 636b 6574 732e  storage.buckets.
+00000b70: 7365 7449 616d 506f 6c69 6379 222c 2020  setIamPolicy",  
+00000b80: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+00000b90: 5543 4b45 5422 5d7d 2c0a 2020 2020 2020  UCKET"]},.      
+00000ba0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+00000bb0: 6167 652e 6275 636b 6574 732e 7570 6461  age.buckets.upda
+00000bc0: 7465 222c 2020 2020 2020 2020 2272 6573  te",        "res
+00000bd0: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00000be0: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00000bf0: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00000c00: 686d 6163 4b65 792e 7570 6461 7465 222c  hmacKey.update",
+00000c10: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00000c20: 6573 223a 205b 2248 4d41 435f 4b45 5922  es": ["HMAC_KEY"
+00000c30: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00000c40: 6d65 223a 2022 7374 6f72 6167 652e 6f62  me": "storage.ob
+00000c50: 6a65 6374 732e 636f 6d70 6f73 6522 2c20  jects.compose", 
+00000c60: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00000c70: 223a 205b 2242 5543 4b45 5422 2c20 224f  ": ["BUCKET", "O
+00000c80: 424a 4543 5422 5d7d 2c0a 2020 2020 2020  BJECT"]},.      
+00000c90: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+00000ca0: 6167 652e 6f62 6a65 6374 732e 636f 7079  age.objects.copy
+00000cb0: 222c 2020 2020 2020 2020 2020 2272 6573  ",          "res
+00000cc0: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00000cd0: 5422 2c20 224f 424a 4543 5422 5d7d 2c0a  T", "OBJECT"]},.
+00000ce0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00000cf0: 2022 7374 6f72 6167 652e 6f62 6a65 6374   "storage.object
+00000d00: 732e 6465 6c65 7465 222c 2020 2020 2020  s.delete",      
+00000d10: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00000d20: 2242 5543 4b45 5422 2c20 224f 424a 4543  "BUCKET", "OBJEC
+00000d30: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00000d40: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00000d50: 6f62 6a65 6374 732e 696e 7365 7274 222c  objects.insert",
+00000d60: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00000d70: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
+00000d80: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00000d90: 223a 2022 7374 6f72 6167 652e 6f62 6a65  ": "storage.obje
+00000da0: 6374 732e 7061 7463 6822 2c20 2020 2020  cts.patch",     
+00000db0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+00000dc0: 205b 2242 5543 4b45 5422 2c20 224f 424a   ["BUCKET", "OBJ
+00000dd0: 4543 5422 5d7d 2c0a 2020 2020 2020 2020  ECT"]},.        
+00000de0: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00000df0: 652e 6f62 6a65 6374 732e 7265 7772 6974  e.objects.rewrit
+00000e00: 6522 2c20 2020 2020 2020 2272 6573 6f75  e",       "resou
+00000e10: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+00000e20: 2c20 224f 424a 4543 5422 5d7d 2c0a 2020  , "OBJECT"]},.  
+00000e30: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00000e40: 7374 6f72 6167 652e 6f62 6a65 6374 732e  storage.objects.
+00000e50: 7570 6461 7465 222c 2020 2020 2020 2020  update",        
+00000e60: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+00000e70: 5543 4b45 5422 2c20 224f 424a 4543 5422  UCKET", "OBJECT"
+00000e80: 5d7d 0a20 2020 2020 205d 2c0a 2020 2020  ]}.      ],.    
+00000e90: 2020 2270 7265 636f 6e64 6974 696f 6e50    "preconditionP
+00000ea0: 726f 7669 6465 6422 3a20 7472 7565 2c0a  rovided": true,.
+00000eb0: 2020 2020 2020 2265 7870 6563 7453 7563        "expectSuc
+00000ec0: 6365 7373 223a 2074 7275 650a 2020 2020  cess": true.    
+00000ed0: 7d2c 0a20 2020 207b 0a20 2020 2020 2022  },.    {.      "
+00000ee0: 6964 223a 2033 2c0a 2020 2020 2020 2264  id": 3,.      "d
+00000ef0: 6573 6372 6970 7469 6f6e 223a 2022 636f  escription": "co
+00000f00: 6e64 6974 696f 6e61 6c6c 795f 6964 656d  nditionally_idem
+00000f10: 706f 7465 6e74 5f6e 6f5f 7265 7472 6965  potent_no_retrie
+00000f20: 735f 7768 656e 5f70 7265 636f 6e64 6974  s_when_precondit
+00000f30: 696f 6e5f 6973 5f61 6273 656e 7422 2c0a  ion_is_absent",.
+00000f40: 2020 2020 2020 2263 6173 6573 223a 205b        "cases": [
+00000f50: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00000f60: 2020 2020 2022 696e 7374 7275 6374 696f       "instructio
+00000f70: 6e73 223a 205b 2272 6574 7572 6e2d 3530  ns": ["return-50
+00000f80: 3322 5d0a 2020 2020 2020 2020 7d2c 0a20  3"].        },. 
+00000f90: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000fa0: 2020 2022 696e 7374 7275 6374 696f 6e73     "instructions
+00000fb0: 223a 205b 2272 6574 7572 6e2d 7265 7365  ": ["return-rese
+00000fc0: 742d 636f 6e6e 6563 7469 6f6e 225d 0a20  t-connection"]. 
+00000fd0: 2020 2020 2020 207d 0a20 2020 2020 205d         }.      ]
+00000fe0: 2c0a 2020 2020 2020 226d 6574 686f 6473  ,.      "methods
+00000ff0: 223a 205b 0a20 2020 2020 2020 207b 226e  ": [.        {"n
+00001000: 616d 6522 3a20 2273 746f 7261 6765 2e62  ame": "storage.b
+00001010: 7563 6b65 7473 2e70 6174 6368 222c 2020  uckets.patch",  
+00001020: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
+00001030: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
+00001040: 0a20 2020 2020 2020 207b 226e 616d 6522  .        {"name"
+00001050: 3a20 2273 746f 7261 6765 2e62 7563 6b65  : "storage.bucke
+00001060: 7473 2e73 6574 4961 6d50 6f6c 6963 7922  ts.setIamPolicy"
+00001070: 2c20 2022 7265 736f 7572 6365 7322 3a20  ,  "resources": 
+00001080: 5b22 4255 434b 4554 225d 7d2c 0a20 2020  ["BUCKET"]},.   
+00001090: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
+000010a0: 746f 7261 6765 2e62 7563 6b65 7473 2e75  torage.buckets.u
+000010b0: 7064 6174 6522 2c20 2020 2020 2020 2022  pdate",        "
+000010c0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
+000010d0: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
+000010e0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
+000010f0: 6765 2e68 6d61 634b 6579 2e75 7064 6174  ge.hmacKey.updat
+00001100: 6522 2c20 2020 2020 2020 2022 7265 736f  e",        "reso
+00001110: 7572 6365 7322 3a20 5b22 484d 4143 5f4b  urces": ["HMAC_K
+00001120: 4559 225d 7d2c 0a20 2020 2020 2020 207b  EY"]},.        {
+00001130: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
+00001140: 2e6f 626a 6563 7473 2e63 6f6d 706f 7365  .objects.compose
+00001150: 222c 2020 2020 2020 2022 7265 736f 7572  ",       "resour
+00001160: 6365 7322 3a20 5b22 4255 434b 4554 222c  ces": ["BUCKET",
+00001170: 2022 4f42 4a45 4354 225d 7d2c 0a20 2020   "OBJECT"]},.   
+00001180: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
+00001190: 746f 7261 6765 2e6f 626a 6563 7473 2e63  torage.objects.c
+000011a0: 6f70 7922 2c20 2020 2020 2020 2020 2022  opy",          "
+000011b0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
+000011c0: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
+000011d0: 7d2c 0a20 2020 2020 2020 207b 226e 616d  },.        {"nam
+000011e0: 6522 3a20 2273 746f 7261 6765 2e6f 626a  e": "storage.obj
+000011f0: 6563 7473 2e64 656c 6574 6522 2c20 2020  ects.delete",   
+00001200: 2020 2020 2022 7265 736f 7572 6365 7322       "resources"
+00001210: 3a20 5b22 4255 434b 4554 222c 2022 4f42  : ["BUCKET", "OB
+00001220: 4a45 4354 225d 7d2c 0a20 2020 2020 2020  JECT"]},.       
+00001230: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
+00001240: 6765 2e6f 626a 6563 7473 2e69 6e73 6572  ge.objects.inser
+00001250: 7422 2c20 2020 2020 2020 2022 7265 736f  t",        "reso
+00001260: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
+00001270: 225d 7d2c 0a20 2020 2020 2020 207b 226e  "]},.        {"n
+00001280: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
+00001290: 626a 6563 7473 2e70 6174 6368 222c 2020  bjects.patch",  
+000012a0: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
+000012b0: 7322 3a20 5b22 4255 434b 4554 222c 2022  s": ["BUCKET", "
+000012c0: 4f42 4a45 4354 225d 7d2c 0a20 2020 2020  OBJECT"]},.     
+000012d0: 2020 207b 226e 616d 6522 3a20 2273 746f     {"name": "sto
+000012e0: 7261 6765 2e6f 626a 6563 7473 2e72 6577  rage.objects.rew
+000012f0: 7269 7465 222c 2020 2020 2020 2022 7265  rite",       "re
+00001300: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
+00001310: 4554 222c 2022 4f42 4a45 4354 225d 7d2c  ET", "OBJECT"]},
+00001320: 0a20 2020 2020 2020 207b 226e 616d 6522  .        {"name"
+00001330: 3a20 2273 746f 7261 6765 2e6f 626a 6563  : "storage.objec
+00001340: 7473 2e75 7064 6174 6522 2c20 2020 2020  ts.update",     
+00001350: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
+00001360: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
+00001370: 4354 225d 7d0a 2020 2020 2020 5d2c 0a20  CT"]}.      ],. 
+00001380: 2020 2020 2022 7072 6563 6f6e 6469 7469       "preconditi
+00001390: 6f6e 5072 6f76 6964 6564 223a 2066 616c  onProvided": fal
+000013a0: 7365 2c0a 2020 2020 2020 2265 7870 6563  se,.      "expec
+000013b0: 7453 7563 6365 7373 223a 2066 616c 7365  tSuccess": false
+000013c0: 0a20 2020 207d 2c0a 2020 2020 7b0a 2020  .    },.    {.  
+000013d0: 2020 2020 2269 6422 3a20 342c 0a20 2020      "id": 4,.   
+000013e0: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
+000013f0: 3a20 226e 6f6e 5f69 6465 6d70 6f74 656e  : "non_idempoten
+00001400: 7422 2c0a 2020 2020 2020 2263 6173 6573  t",.      "cases
+00001410: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+00001420: 2020 2020 2020 2020 2022 696e 7374 7275           "instru
+00001430: 6374 696f 6e73 223a 205b 2272 6574 7572  ctions": ["retur
+00001440: 6e2d 3530 3322 5d0a 2020 2020 2020 2020  n-503"].        
+00001450: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00001460: 2020 2020 2020 2022 696e 7374 7275 6374         "instruct
+00001470: 696f 6e73 223a 205b 2272 6574 7572 6e2d  ions": ["return-
+00001480: 7265 7365 742d 636f 6e6e 6563 7469 6f6e  reset-connection
+00001490: 225d 0a20 2020 2020 2020 207d 0a20 2020  "].        }.   
+000014a0: 2020 205d 2c0a 2020 2020 2020 226d 6574     ],.      "met
+000014b0: 686f 6473 223a 205b 0a20 2020 2020 2020  hods": [.       
+000014c0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
+000014d0: 6765 2e62 7563 6b65 745f 6163 6c2e 6465  ge.bucket_acl.de
+000014e0: 6c65 7465 222c 2020 2020 2020 2020 2020  lete",          
+000014f0: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
+00001500: 5b22 4255 434b 4554 225d 7d2c 0a20 2020  ["BUCKET"]},.   
+00001510: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
+00001520: 746f 7261 6765 2e62 7563 6b65 745f 6163  torage.bucket_ac
+00001530: 6c2e 696e 7365 7274 222c 2020 2020 2020  l.insert",      
+00001540: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
+00001550: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
+00001560: 0a20 2020 2020 2020 207b 226e 616d 6522  .        {"name"
+00001570: 3a20 2273 746f 7261 6765 2e62 7563 6b65  : "storage.bucke
+00001580: 745f 6163 6c2e 7061 7463 6822 2c20 2020  t_acl.patch",   
+00001590: 2020 2020 2020 2020 2020 2022 7265 736f             "reso
+000015a0: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
+000015b0: 225d 7d2c 0a20 2020 2020 2020 207b 226e  "]},.        {"n
+000015c0: 616d 6522 3a20 2273 746f 7261 6765 2e62  ame": "storage.b
+000015d0: 7563 6b65 745f 6163 6c2e 7570 6461 7465  ucket_acl.update
+000015e0: 222c 2020 2020 2020 2020 2020 2020 2022  ",             "
+000015f0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
+00001600: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
+00001610: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
+00001620: 6765 2e64 6566 6175 6c74 5f6f 626a 6563  ge.default_objec
+00001630: 745f 6163 6c2e 6465 6c65 7465 222c 2020  t_acl.delete",  
+00001640: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
+00001650: 5b22 4255 434b 4554 225d 7d2c 0a20 2020  ["BUCKET"]},.   
+00001660: 2020 2020 207b 226e 616d 6522 3a20 2273       {"name": "s
+00001670: 746f 7261 6765 2e64 6566 6175 6c74 5f6f  torage.default_o
+00001680: 626a 6563 745f 6163 6c2e 696e 7365 7274  bject_acl.insert
+00001690: 222c 2020 2020 2022 7265 736f 7572 6365  ",     "resource
+000016a0: 7322 3a20 5b22 4255 434b 4554 225d 7d2c  s": ["BUCKET"]},
+000016b0: 0a20 2020 2020 2020 207b 226e 616d 6522  .        {"name"
+000016c0: 3a20 2273 746f 7261 6765 2e64 6566 6175  : "storage.defau
+000016d0: 6c74 5f6f 626a 6563 745f 6163 6c2e 7061  lt_object_acl.pa
+000016e0: 7463 6822 2c20 2020 2020 2022 7265 736f  tch",      "reso
+000016f0: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
+00001700: 225d 7d2c 0a20 2020 2020 2020 207b 226e  "]},.        {"n
+00001710: 616d 6522 3a20 2273 746f 7261 6765 2e64  ame": "storage.d
+00001720: 6566 6175 6c74 5f6f 626a 6563 745f 6163  efault_object_ac
+00001730: 6c2e 7570 6461 7465 222c 2020 2020 2022  l.update",     "
+00001740: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
+00001750: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
+00001760: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
+00001770: 6765 2e68 6d61 634b 6579 2e63 7265 6174  ge.hmacKey.creat
+00001780: 6522 2c20 2020 2020 2020 2020 2020 2020  e",             
+00001790: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
+000017a0: 5b5d 7d2c 0a20 2020 2020 2020 207b 226e  []},.        {"n
+000017b0: 616d 6522 3a20 2273 746f 7261 6765 2e6e  ame": "storage.n
+000017c0: 6f74 6966 6963 6174 696f 6e73 2e69 6e73  otifications.ins
+000017d0: 6572 7422 2c20 2020 2020 2020 2020 2022  ert",          "
+000017e0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
+000017f0: 434b 4554 225d 7d2c 0a20 2020 2020 2020  CKET"]},.       
+00001800: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
+00001810: 6765 2e6f 626a 6563 745f 6163 6c2e 6465  ge.object_acl.de
+00001820: 6c65 7465 222c 2020 2020 2020 2020 2020  lete",          
+00001830: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
+00001840: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
+00001850: 4354 225d 7d2c 0a20 2020 2020 2020 207b  CT"]},.        {
+00001860: 226e 616d 6522 3a20 2273 746f 7261 6765  "name": "storage
+00001870: 2e6f 626a 6563 745f 6163 6c2e 696e 7365  .object_acl.inse
+00001880: 7274 222c 2020 2020 2020 2020 2020 2020  rt",            
+00001890: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
+000018a0: 4255 434b 4554 222c 2022 4f42 4a45 4354  BUCKET", "OBJECT
+000018b0: 225d 7d2c 0a20 2020 2020 2020 207b 226e  "]},.        {"n
+000018c0: 616d 6522 3a20 2273 746f 7261 6765 2e6f  ame": "storage.o
+000018d0: 626a 6563 745f 6163 6c2e 7061 7463 6822  bject_acl.patch"
+000018e0: 2c20 2020 2020 2020 2020 2020 2020 2022  ,              "
+000018f0: 7265 736f 7572 6365 7322 3a20 5b22 4255  resources": ["BU
+00001900: 434b 4554 222c 2022 4f42 4a45 4354 225d  CKET", "OBJECT"]
+00001910: 7d2c 0a20 2020 2020 2020 207b 226e 616d  },.        {"nam
+00001920: 6522 3a20 2273 746f 7261 6765 2e6f 626a  e": "storage.obj
+00001930: 6563 745f 6163 6c2e 7570 6461 7465 222c  ect_acl.update",
+00001940: 2020 2020 2020 2020 2020 2020 2022 7265               "re
+00001950: 736f 7572 6365 7322 3a20 5b22 4255 434b  sources": ["BUCK
+00001960: 4554 222c 2022 4f42 4a45 4354 225d 7d0a  ET", "OBJECT"]}.
+00001970: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
+00001980: 7072 6563 6f6e 6469 7469 6f6e 5072 6f76  preconditionProv
+00001990: 6964 6564 223a 2066 616c 7365 2c0a 2020  ided": false,.  
+000019a0: 2020 2020 2265 7870 6563 7453 7563 6365      "expectSucce
+000019b0: 7373 223a 2066 616c 7365 0a20 2020 207d  ss": false.    }
+000019c0: 2c0a 2020 2020 7b0a 2020 2020 2020 2269  ,.    {.      "i
+000019d0: 6422 3a20 352c 0a20 2020 2020 2022 6465  d": 5,.      "de
+000019e0: 7363 7269 7074 696f 6e22 3a20 226e 6f6e  scription": "non
+000019f0: 2d72 6574 7279 6162 6c65 2065 7272 6f72  -retryable error
+00001a00: 7322 2c0a 2020 2020 2020 2263 6173 6573  s",.      "cases
+00001a10: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+00001a20: 2020 2020 2020 2020 2022 696e 7374 7275           "instru
+00001a30: 6374 696f 6e73 223a 205b 2272 6574 7572  ctions": ["retur
+00001a40: 6e2d 3430 3022 5d0a 2020 2020 2020 2020  n-400"].        
+00001a50: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00001a60: 2020 2020 2020 2022 696e 7374 7275 6374         "instruct
+00001a70: 696f 6e73 223a 205b 2272 6574 7572 6e2d  ions": ["return-
+00001a80: 3430 3122 5d0a 2020 2020 2020 2020 7d0a  401"].        }.
+00001a90: 2020 2020 2020 5d2c 0a20 2020 2020 2022        ],.      "
+00001aa0: 6d65 7468 6f64 7322 3a20 5b0a 2020 2020  methods": [.    
+00001ab0: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00001ac0: 6f72 6167 652e 6275 636b 6574 5f61 636c  orage.bucket_acl
+00001ad0: 2e64 656c 6574 6522 2c20 2020 2020 2020  .delete",       
+00001ae0: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00001af0: 223a 205b 2242 5543 4b45 5422 5d7d 2c0a  ": ["BUCKET"]},.
+00001b00: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00001b10: 2022 7374 6f72 6167 652e 6275 636b 6574   "storage.bucket
+00001b20: 5f61 636c 2e67 6574 222c 2020 2020 2020  _acl.get",      
+00001b30: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00001b40: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+00001b50: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00001b60: 6d65 223a 2022 7374 6f72 6167 652e 6275  me": "storage.bu
+00001b70: 636b 6574 5f61 636c 2e69 6e73 6572 7422  cket_acl.insert"
+00001b80: 2c20 2020 2020 2020 2020 2020 2020 2272  ,             "r
+00001b90: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00001ba0: 4b45 5422 5d7d 2c0a 2020 2020 2020 2020  KET"]},.        
+00001bb0: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00001bc0: 652e 6275 636b 6574 5f61 636c 2e6c 6973  e.bucket_acl.lis
+00001bd0: 7422 2c20 2020 2020 2020 2020 2020 2020  t",             
+00001be0: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00001bf0: 2242 5543 4b45 5422 5d7d 2c0a 2020 2020  "BUCKET"]},.    
+00001c00: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00001c10: 6f72 6167 652e 6275 636b 6574 5f61 636c  orage.bucket_acl
+00001c20: 2e70 6174 6368 222c 2020 2020 2020 2020  .patch",        
+00001c30: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00001c40: 223a 205b 2242 5543 4b45 5422 5d7d 2c0a  ": ["BUCKET"]},.
+00001c50: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00001c60: 2022 7374 6f72 6167 652e 6275 636b 6574   "storage.bucket
+00001c70: 5f61 636c 2e75 7064 6174 6522 2c20 2020  _acl.update",   
+00001c80: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00001c90: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+00001ca0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00001cb0: 6d65 223a 2022 7374 6f72 6167 652e 6275  me": "storage.bu
+00001cc0: 636b 6574 732e 6465 6c65 7465 222c 2020  ckets.delete",  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00001ce0: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00001cf0: 4b45 5422 5d7d 2c0a 2020 2020 2020 2020  KET"]},.        
+00001d00: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00001d10: 652e 6275 636b 6574 732e 6765 7422 2c20  e.buckets.get", 
+00001d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d30: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00001d40: 2242 5543 4b45 5422 5d7d 2c0a 2020 2020  "BUCKET"]},.    
+00001d50: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00001d60: 6f72 6167 652e 6275 636b 6574 732e 6765  orage.buckets.ge
+00001d70: 7449 616d 506f 6c69 6379 222c 2020 2020  tIamPolicy",    
+00001d80: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00001d90: 223a 205b 2242 5543 4b45 5422 5d7d 2c0a  ": ["BUCKET"]},.
+00001da0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00001db0: 2022 7374 6f72 6167 652e 6275 636b 6574   "storage.bucket
+00001dc0: 732e 696e 7365 7274 222c 2020 2020 2020  s.insert",      
+00001dd0: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00001de0: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+00001df0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00001e00: 6d65 223a 2022 7374 6f72 6167 652e 6275  me": "storage.bu
+00001e10: 636b 6574 732e 6c69 7374 222c 2020 2020  ckets.list",    
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00001e30: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00001e40: 4b45 5422 5d7d 2c0a 2020 2020 2020 2020  KET"]},.        
+00001e50: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00001e60: 652e 6275 636b 6574 732e 6c6f 636b 5265  e.buckets.lockRe
+00001e70: 7465 6e74 696f 6e50 6f6c 6963 7922 2c20  tentionPolicy", 
+00001e80: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00001e90: 2242 5543 4b45 5422 5d7d 2c0a 2020 2020  "BUCKET"]},.    
+00001ea0: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00001eb0: 6f72 6167 652e 6275 636b 6574 732e 7061  orage.buckets.pa
+00001ec0: 7463 6822 2c20 2020 2020 2020 2020 2020  tch",           
+00001ed0: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00001ee0: 223a 205b 2242 5543 4b45 5422 5d7d 2c0a  ": ["BUCKET"]},.
+00001ef0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00001f00: 2022 7374 6f72 6167 652e 6275 636b 6574   "storage.bucket
+00001f10: 732e 7365 7449 616d 506f 6c69 6379 222c  s.setIamPolicy",
+00001f20: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00001f30: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+00001f40: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00001f50: 6d65 223a 2022 7374 6f72 6167 652e 6275  me": "storage.bu
+00001f60: 636b 6574 732e 7465 7374 4961 6d50 6572  ckets.testIamPer
+00001f70: 6d69 7373 696f 6e73 222c 2020 2020 2272  missions",    "r
+00001f80: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00001f90: 4b45 5422 5d7d 2c0a 2020 2020 2020 2020  KET"]},.        
+00001fa0: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00001fb0: 652e 6275 636b 6574 732e 7570 6461 7465  e.buckets.update
+00001fc0: 222c 2020 2020 2020 2020 2020 2020 2020  ",              
+00001fd0: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00001fe0: 2242 5543 4b45 5422 5d7d 2c0a 2020 2020  "BUCKET"]},.    
+00001ff0: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00002000: 6f72 6167 652e 6465 6661 756c 745f 6f62  orage.default_ob
+00002010: 6a65 6374 5f61 636c 2e64 656c 6574 6522  ject_acl.delete"
+00002020: 2c20 2020 2020 2272 6573 6f75 7263 6573  ,     "resources
+00002030: 223a 205b 2242 5543 4b45 5422 5d7d 2c0a  ": ["BUCKET"]},.
+00002040: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00002050: 2022 7374 6f72 6167 652e 6465 6661 756c   "storage.defaul
+00002060: 745f 6f62 6a65 6374 5f61 636c 2e67 6574  t_object_acl.get
+00002070: 222c 2020 2020 2020 2020 2272 6573 6f75  ",        "resou
+00002080: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+00002090: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+000020a0: 6d65 223a 2022 7374 6f72 6167 652e 6465  me": "storage.de
+000020b0: 6661 756c 745f 6f62 6a65 6374 5f61 636c  fault_object_acl
+000020c0: 2e69 6e73 6572 7422 2c20 2020 2020 2272  .insert",     "r
+000020d0: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+000020e0: 4b45 5422 5d7d 2c0a 2020 2020 2020 2020  KET"]},.        
+000020f0: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00002100: 652e 6465 6661 756c 745f 6f62 6a65 6374  e.default_object
+00002110: 5f61 636c 2e6c 6973 7422 2c20 2020 2020  _acl.list",     
+00002120: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00002130: 2242 5543 4b45 5422 5d7d 2c0a 2020 2020  "BUCKET"]},.    
+00002140: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00002150: 6f72 6167 652e 6465 6661 756c 745f 6f62  orage.default_ob
+00002160: 6a65 6374 5f61 636c 2e70 6174 6368 222c  ject_acl.patch",
+00002170: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00002180: 223a 205b 2242 5543 4b45 5422 5d7d 2c0a  ": ["BUCKET"]},.
+00002190: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+000021a0: 2022 7374 6f72 6167 652e 6465 6661 756c   "storage.defaul
+000021b0: 745f 6f62 6a65 6374 5f61 636c 2e75 7064  t_object_acl.upd
+000021c0: 6174 6522 2c20 2020 2020 2272 6573 6f75  ate",     "resou
+000021d0: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+000021e0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+000021f0: 6d65 223a 2022 7374 6f72 6167 652e 686d  me": "storage.hm
+00002200: 6163 4b65 792e 6372 6561 7465 222c 2020  acKey.create",  
+00002210: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00002220: 6573 6f75 7263 6573 223a 205b 5d7d 2c0a  esources": []},.
+00002230: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00002240: 2022 7374 6f72 6167 652e 686d 6163 4b65   "storage.hmacKe
+00002250: 792e 6465 6c65 7465 222c 2020 2020 2020  y.delete",      
+00002260: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00002270: 7263 6573 223a 205b 2248 4d41 435f 4b45  rces": ["HMAC_KE
+00002280: 5922 5d7d 2c0a 2020 2020 2020 2020 7b22  Y"]},.        {"
+00002290: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+000022a0: 686d 6163 4b65 792e 6765 7422 2c20 2020  hmacKey.get",   
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2272 6573 6f75 7263 6573 223a 205b 2248  "resources": ["H
+000022d0: 4d41 435f 4b45 5922 5d7d 2c0a 2020 2020  MAC_KEY"]},.    
+000022e0: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+000022f0: 6f72 6167 652e 686d 6163 4b65 792e 6c69  orage.hmacKey.li
+00002300: 7374 222c 2020 2020 2020 2020 2020 2020  st",            
+00002310: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00002320: 223a 205b 2248 4d41 435f 4b45 5922 5d7d  ": ["HMAC_KEY"]}
+00002330: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00002340: 223a 2022 7374 6f72 6167 652e 686d 6163  ": "storage.hmac
+00002350: 4b65 792e 7570 6461 7465 222c 2020 2020  Key.update",    
+00002360: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+00002370: 6f75 7263 6573 223a 205b 2248 4d41 435f  ources": ["HMAC_
+00002380: 4b45 5922 5d7d 2c0a 2020 2020 2020 2020  KEY"]},.        
+00002390: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+000023a0: 652e 6e6f 7469 6669 6361 7469 6f6e 732e  e.notifications.
+000023b0: 6465 6c65 7465 222c 2020 2020 2020 2020  delete",        
+000023c0: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+000023d0: 2242 5543 4b45 5422 2c20 224e 4f54 4946  "BUCKET", "NOTIF
+000023e0: 4943 4154 494f 4e22 5d7d 2c0a 2020 2020  ICATION"]},.    
+000023f0: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00002400: 6f72 6167 652e 6e6f 7469 6669 6361 7469  orage.notificati
+00002410: 6f6e 732e 6765 7422 2c20 2020 2020 2020  ons.get",       
+00002420: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00002430: 223a 205b 2242 5543 4b45 5422 2c20 224e  ": ["BUCKET", "N
+00002440: 4f54 4946 4943 4154 494f 4e22 5d7d 2c0a  OTIFICATION"]},.
+00002450: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00002460: 2022 7374 6f72 6167 652e 6e6f 7469 6669   "storage.notifi
+00002470: 6361 7469 6f6e 732e 696e 7365 7274 222c  cations.insert",
+00002480: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00002490: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+000024a0: 2c20 224e 4f54 4946 4943 4154 494f 4e22  , "NOTIFICATION"
+000024b0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+000024c0: 6d65 223a 2022 7374 6f72 6167 652e 6e6f  me": "storage.no
+000024d0: 7469 6669 6361 7469 6f6e 732e 6c69 7374  tifications.list
+000024e0: 222c 2020 2020 2020 2020 2020 2020 2272  ",            "r
+000024f0: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00002500: 4b45 5422 2c20 224e 4f54 4946 4943 4154  KET", "NOTIFICAT
+00002510: 494f 4e22 5d7d 2c0a 2020 2020 2020 2020  ION"]},.        
+00002520: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00002530: 652e 6f62 6a65 6374 5f61 636c 2e64 656c  e.object_acl.del
+00002540: 6574 6522 2c20 2020 2020 2020 2020 2020  ete",           
+00002550: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00002560: 2242 5543 4b45 5422 2c20 224f 424a 4543  "BUCKET", "OBJEC
+00002570: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00002580: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00002590: 6f62 6a65 6374 5f61 636c 2e67 6574 222c  object_acl.get",
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+000025c0: 5543 4b45 5422 2c20 224f 424a 4543 5422  UCKET", "OBJECT"
+000025d0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+000025e0: 6d65 223a 2022 7374 6f72 6167 652e 6f62  me": "storage.ob
+000025f0: 6a65 6374 5f61 636c 2e69 6e73 6572 7422  ject_acl.insert"
+00002600: 2c20 2020 2020 2020 2020 2020 2020 2272  ,             "r
+00002610: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00002620: 4b45 5422 2c20 224f 424a 4543 5422 5d7d  KET", "OBJECT"]}
+00002630: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00002640: 223a 2022 7374 6f72 6167 652e 6f62 6a65  ": "storage.obje
+00002650: 6374 5f61 636c 2e6c 6973 7422 2c20 2020  ct_acl.list",   
+00002660: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+00002670: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00002680: 5422 2c20 224f 424a 4543 5422 5d7d 2c0a  T", "OBJECT"]},.
+00002690: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+000026a0: 2022 7374 6f72 6167 652e 6f62 6a65 6374   "storage.object
+000026b0: 5f61 636c 2e70 6174 6368 222c 2020 2020  _acl.patch",    
+000026c0: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+000026d0: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+000026e0: 2c20 224f 424a 4543 5422 5d7d 2c0a 2020  , "OBJECT"]},.  
+000026f0: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00002700: 7374 6f72 6167 652e 6f62 6a65 6374 5f61  storage.object_a
+00002710: 636c 2e75 7064 6174 6522 2c20 2020 2020  cl.update",     
+00002720: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00002730: 6573 223a 205b 2242 5543 4b45 5422 2c20  es": ["BUCKET", 
+00002740: 224f 424a 4543 5422 5d7d 2c0a 2020 2020  "OBJECT"]},.    
+00002750: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00002760: 6f72 6167 652e 6f62 6a65 6374 732e 636f  orage.objects.co
+00002770: 6d70 6f73 6522 2c20 2020 2020 2020 2020  mpose",         
+00002780: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+00002790: 223a 205b 2242 5543 4b45 5422 2c20 224f  ": ["BUCKET", "O
+000027a0: 424a 4543 5422 5d7d 2c0a 2020 2020 2020  BJECT"]},.      
+000027b0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000027c0: 6167 652e 6f62 6a65 6374 732e 636f 7079  age.objects.copy
+000027d0: 222c 2020 2020 2020 2020 2020 2020 2020  ",              
+000027e0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+000027f0: 205b 2242 5543 4b45 5422 2c20 224f 424a   ["BUCKET", "OBJ
+00002800: 4543 5422 5d7d 2c0a 2020 2020 2020 2020  ECT"]},.        
+00002810: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00002820: 652e 6f62 6a65 6374 732e 6465 6c65 7465  e.objects.delete
+00002830: 222c 2020 2020 2020 2020 2020 2020 2020  ",              
+00002840: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00002850: 2242 5543 4b45 5422 2c20 224f 424a 4543  "BUCKET", "OBJEC
+00002860: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00002870: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00002880: 6f62 6a65 6374 732e 6765 7422 2c20 2020  objects.get",   
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+000028b0: 5543 4b45 5422 2c20 224f 424a 4543 5422  UCKET", "OBJECT"
+000028c0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+000028d0: 6d65 223a 2022 7374 6f72 6167 652e 6f62  me": "storage.ob
+000028e0: 6a65 6374 732e 696e 7365 7274 222c 2020  jects.insert",  
+000028f0: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00002900: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00002910: 4b45 5422 5d7d 2c0a 2020 2020 2020 2020  KET"]},.        
+00002920: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00002930: 652e 6f62 6a65 6374 732e 6c69 7374 222c  e.objects.list",
+00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002950: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00002960: 2242 5543 4b45 5422 2c20 224f 424a 4543  "BUCKET", "OBJEC
+00002970: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00002980: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00002990: 6f62 6a65 6374 732e 7061 7463 6822 2c20  objects.patch", 
+000029a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029b0: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+000029c0: 5543 4b45 5422 2c20 224f 424a 4543 5422  UCKET", "OBJECT"
+000029d0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+000029e0: 6d65 223a 2022 7374 6f72 6167 652e 6f62  me": "storage.ob
+000029f0: 6a65 6374 732e 7265 7772 6974 6522 2c20  jects.rewrite", 
+00002a00: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00002a10: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00002a20: 4b45 5422 2c20 224f 424a 4543 5422 5d7d  KET", "OBJECT"]}
+00002a30: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00002a40: 223a 2022 7374 6f72 6167 652e 6f62 6a65  ": "storage.obje
+00002a50: 6374 732e 7570 6461 7465 222c 2020 2020  cts.update",    
+00002a60: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+00002a70: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00002a80: 5422 2c20 224f 424a 4543 5422 5d7d 2c0a  T", "OBJECT"]},.
+00002a90: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+00002aa0: 2022 7374 6f72 6167 652e 7365 7276 6963   "storage.servic
+00002ab0: 6561 6363 6f75 6e74 2e67 6574 222c 2020  eaccount.get",  
+00002ac0: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00002ad0: 7263 6573 223a 205b 5d7d 0a20 2020 2020  rces": []}.     
+00002ae0: 205d 2c0a 2020 2020 2020 2270 7265 636f   ],.      "preco
+00002af0: 6e64 6974 696f 6e50 726f 7669 6465 6422  nditionProvided"
+00002b00: 3a20 6661 6c73 652c 0a20 2020 2020 2022  : false,.      "
+00002b10: 6578 7065 6374 5375 6363 6573 7322 3a20  expectSuccess": 
+00002b20: 6661 6c73 650a 2020 2020 7d2c 0a20 2020  false.    },.   
+00002b30: 207b 0a20 2020 2020 2022 6964 223a 2036   {.      "id": 6
+00002b40: 2c0a 2020 2020 2020 2264 6573 6372 6970  ,.      "descrip
+00002b50: 7469 6f6e 223a 2022 6d69 785f 7265 7472  tion": "mix_retr
+00002b60: 7961 626c 655f 6e6f 6e5f 7265 7472 7961  yable_non_retrya
+00002b70: 626c 655f 6572 726f 7273 222c 0a20 2020  ble_errors",.   
+00002b80: 2020 2022 6361 7365 7322 3a20 5b0a 2020     "cases": [.  
+00002b90: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00002ba0: 2020 2269 6e73 7472 7563 7469 6f6e 7322    "instructions"
+00002bb0: 3a20 5b22 7265 7475 726e 2d35 3033 222c  : ["return-503",
+00002bc0: 2022 7265 7475 726e 2d34 3030 225d 0a20   "return-400"]. 
+00002bd0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00002be0: 2020 7b0a 2020 2020 2020 2020 2020 2269    {.          "i
+00002bf0: 6e73 7472 7563 7469 6f6e 7322 3a20 5b22  nstructions": ["
+00002c00: 7265 7475 726e 2d72 6573 6574 2d63 6f6e  return-reset-con
+00002c10: 6e65 6374 696f 6e22 2c20 2272 6574 7572  nection", "retur
+00002c20: 6e2d 3430 3122 5d0a 2020 2020 2020 2020  n-401"].        
+00002c30: 7d0a 2020 2020 2020 5d2c 0a20 2020 2020  }.      ],.     
+00002c40: 2022 6d65 7468 6f64 7322 3a20 5b0a 2020   "methods": [.  
+00002c50: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00002c60: 7374 6f72 6167 652e 6275 636b 6574 5f61  storage.bucket_a
+00002c70: 636c 2e67 6574 222c 2020 2020 2020 2020  cl.get",        
+00002c80: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00002c90: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
+00002ca0: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00002cb0: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
+00002cc0: 6574 5f61 636c 2e6c 6973 7422 2c20 2020  et_acl.list",   
+00002cd0: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+00002ce0: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00002cf0: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00002d00: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00002d10: 6275 636b 6574 732e 6465 6c65 7465 222c  buckets.delete",
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d30: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+00002d40: 5543 4b45 5422 5d7d 2c0a 2020 2020 2020  UCKET"]},.      
+00002d50: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+00002d60: 6167 652e 6275 636b 6574 732e 6765 7422  age.buckets.get"
+00002d70: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+00002d80: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+00002d90: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
+00002da0: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00002db0: 7374 6f72 6167 652e 6275 636b 6574 732e  storage.buckets.
+00002dc0: 6765 7449 616d 506f 6c69 6379 222c 2020  getIamPolicy",  
+00002dd0: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00002de0: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
+00002df0: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00002e00: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
+00002e10: 6574 732e 696e 7365 7274 222c 2020 2020  ets.insert",    
+00002e20: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+00002e30: 6f75 7263 6573 223a 205b 5d7d 2c0a 2020  ources": []},.  
+00002e40: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00002e50: 7374 6f72 6167 652e 6275 636b 6574 732e  storage.buckets.
+00002e60: 6c69 7374 222c 2020 2020 2020 2020 2020  list",          
+00002e70: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00002e80: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
+00002e90: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00002ea0: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
+00002eb0: 6574 732e 6c6f 636b 5265 7465 6e74 696f  ets.lockRetentio
+00002ec0: 6e50 6f6c 6963 7922 2c20 2020 2272 6573  nPolicy",   "res
+00002ed0: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00002ee0: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00002ef0: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00002f00: 6275 636b 6574 732e 7061 7463 6822 2c20  buckets.patch", 
+00002f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f20: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+00002f30: 5543 4b45 5422 5d7d 2c0a 2020 2020 2020  UCKET"]},.      
+00002f40: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+00002f50: 6167 652e 6275 636b 6574 732e 7365 7449  age.buckets.setI
+00002f60: 616d 506f 6c69 6379 222c 2020 2020 2020  amPolicy",      
+00002f70: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+00002f80: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
+00002f90: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00002fa0: 7374 6f72 6167 652e 6275 636b 6574 732e  storage.buckets.
+00002fb0: 7465 7374 4961 6d50 6572 6d69 7373 696f  testIamPermissio
+00002fc0: 6e73 222c 2020 2020 2272 6573 6f75 7263  ns",    "resourc
+00002fd0: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
+00002fe0: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00002ff0: 223a 2022 7374 6f72 6167 652e 6275 636b  ": "storage.buck
+00003000: 6574 732e 7570 6461 7465 222c 2020 2020  ets.update",    
+00003010: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+00003020: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+00003030: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+00003040: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00003050: 6465 6661 756c 745f 6f62 6a65 6374 5f61  default_object_a
+00003060: 636c 2e67 6574 222c 2020 2020 2020 2020  cl.get",        
+00003070: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+00003080: 5543 4b45 5422 5d7d 2c0a 2020 2020 2020  UCKET"]},.      
+00003090: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000030a0: 6167 652e 6465 6661 756c 745f 6f62 6a65  age.default_obje
+000030b0: 6374 5f61 636c 2e6c 6973 7422 2c20 2020  ct_acl.list",   
+000030c0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+000030d0: 205b 2242 5543 4b45 5422 5d7d 2c0a 2020   ["BUCKET"]},.  
+000030e0: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+000030f0: 7374 6f72 6167 652e 686d 6163 4b65 792e  storage.hmacKey.
+00003100: 6465 6c65 7465 222c 2020 2020 2020 2020  delete",        
+00003110: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00003120: 6573 223a 205b 2248 4d41 435f 4b45 5922  es": ["HMAC_KEY"
+00003130: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00003140: 6d65 223a 2022 7374 6f72 6167 652e 686d  me": "storage.hm
+00003150: 6163 4b65 792e 6765 7422 2c20 2020 2020  acKey.get",     
+00003160: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00003170: 6573 6f75 7263 6573 223a 205b 2248 4d41  esources": ["HMA
+00003180: 435f 4b45 5922 5d7d 2c0a 2020 2020 2020  C_KEY"]},.      
+00003190: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000031a0: 6167 652e 686d 6163 4b65 792e 6c69 7374  age.hmacKey.list
+000031b0: 222c 2020 2020 2020 2020 2020 2020 2020  ",              
+000031c0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+000031d0: 205b 2248 4d41 435f 4b45 5922 5d7d 2c0a   ["HMAC_KEY"]},.
+000031e0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+000031f0: 2022 7374 6f72 6167 652e 686d 6163 4b65   "storage.hmacKe
+00003200: 792e 7570 6461 7465 222c 2020 2020 2020  y.update",      
+00003210: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00003220: 7263 6573 223a 205b 2248 4d41 435f 4b45  rces": ["HMAC_KE
+00003230: 5922 5d7d 2c0a 2020 2020 2020 2020 7b22  Y"]},.        {"
+00003240: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+00003250: 6e6f 7469 6669 6361 7469 6f6e 732e 6465  notifications.de
+00003260: 6c65 7465 222c 2020 2020 2020 2020 2020  lete",          
+00003270: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+00003280: 5543 4b45 5422 2c20 224e 4f54 4946 4943  UCKET", "NOTIFIC
+00003290: 4154 494f 4e22 5d7d 2c0a 2020 2020 2020  ATION"]},.      
+000032a0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000032b0: 6167 652e 6e6f 7469 6669 6361 7469 6f6e  age.notification
+000032c0: 732e 6765 7422 2c20 2020 2020 2020 2020  s.get",         
+000032d0: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+000032e0: 205b 2242 5543 4b45 5422 2c20 224e 4f54   ["BUCKET", "NOT
+000032f0: 4946 4943 4154 494f 4e22 5d7d 2c0a 2020  IFICATION"]},.  
+00003300: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00003310: 7374 6f72 6167 652e 6e6f 7469 6669 6361  storage.notifica
+00003320: 7469 6f6e 732e 6c69 7374 222c 2020 2020  tions.list",    
+00003330: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00003340: 6573 223a 205b 2242 5543 4b45 5422 2c20  es": ["BUCKET", 
+00003350: 224e 4f54 4946 4943 4154 494f 4e22 5d7d  "NOTIFICATION"]}
+00003360: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00003370: 223a 2022 7374 6f72 6167 652e 6f62 6a65  ": "storage.obje
+00003380: 6374 5f61 636c 2e67 6574 222c 2020 2020  ct_acl.get",    
+00003390: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+000033a0: 6f75 7263 6573 223a 205b 2242 5543 4b45  ources": ["BUCKE
+000033b0: 5422 2c20 224f 424a 4543 5422 5d7d 2c0a  T", "OBJECT"]},.
+000033c0: 2020 2020 2020 2020 7b22 6e61 6d65 223a          {"name":
+000033d0: 2022 7374 6f72 6167 652e 6f62 6a65 6374   "storage.object
+000033e0: 5f61 636c 2e6c 6973 7422 2c20 2020 2020  _acl.list",     
+000033f0: 2020 2020 2020 2020 2020 2272 6573 6f75            "resou
+00003400: 7263 6573 223a 205b 2242 5543 4b45 5422  rces": ["BUCKET"
+00003410: 2c20 224f 424a 4543 5422 5d7d 2c0a 2020  , "OBJECT"]},.  
+00003420: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00003430: 7374 6f72 6167 652e 6f62 6a65 6374 732e  storage.objects.
+00003440: 636f 6d70 6f73 6522 2c20 2020 2020 2020  compose",       
+00003450: 2020 2020 2020 2020 2272 6573 6f75 7263          "resourc
+00003460: 6573 223a 205b 2242 5543 4b45 5422 2c20  es": ["BUCKET", 
+00003470: 224f 424a 4543 5422 5d7d 2c0a 2020 2020  "OBJECT"]},.    
+00003480: 2020 2020 7b22 6e61 6d65 223a 2022 7374      {"name": "st
+00003490: 6f72 6167 652e 6f62 6a65 6374 732e 636f  orage.objects.co
+000034a0: 7079 222c 2020 2020 2020 2020 2020 2020  py",            
+000034b0: 2020 2020 2020 2272 6573 6f75 7263 6573        "resources
+000034c0: 223a 205b 2242 5543 4b45 5422 2c20 224f  ": ["BUCKET", "O
+000034d0: 424a 4543 5422 5d7d 2c0a 2020 2020 2020  BJECT"]},.      
+000034e0: 2020 7b22 6e61 6d65 223a 2022 7374 6f72    {"name": "stor
+000034f0: 6167 652e 6f62 6a65 6374 732e 6465 6c65  age.objects.dele
+00003500: 7465 222c 2020 2020 2020 2020 2020 2020  te",            
+00003510: 2020 2020 2272 6573 6f75 7263 6573 223a      "resources":
+00003520: 205b 2242 5543 4b45 5422 2c20 224f 424a   ["BUCKET", "OBJ
+00003530: 4543 5422 5d7d 2c0a 2020 2020 2020 2020  ECT"]},.        
+00003540: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00003550: 652e 6f62 6a65 6374 732e 6765 7422 2c20  e.objects.get", 
+00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003570: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00003580: 2242 5543 4b45 5422 2c20 224f 424a 4543  "BUCKET", "OBJEC
+00003590: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+000035a0: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+000035b0: 6f62 6a65 6374 732e 6c69 7374 222c 2020  objects.list",  
+000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035d0: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+000035e0: 5543 4b45 5422 2c20 224f 424a 4543 5422  UCKET", "OBJECT"
+000035f0: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00003600: 6d65 223a 2022 7374 6f72 6167 652e 6f62  me": "storage.ob
+00003610: 6a65 6374 732e 696e 7365 7274 222c 2020  jects.insert",  
+00003620: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00003630: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00003640: 4b45 5422 5d7d 2c0a 2020 2020 2020 2020  KET"]},.        
+00003650: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+00003660: 652e 6f62 6a65 6374 732e 7061 7463 6822  e.objects.patch"
 00003670: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-00003680: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00003690: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
-000036a0: 4354 225d 7d2c 0a20 2020 2020 2020 2020  CT"]},.         
-000036b0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-000036c0: 6765 2e6f 626a 6563 7473 2e64 656c 6574  ge.objects.delet
-000036d0: 6522 2c20 2020 2020 2020 2020 2020 2020  e",             
-000036e0: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-000036f0: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
-00003700: 4354 225d 7d2c 0a20 2020 2020 2020 2020  CT"]},.         
-00003710: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00003720: 6765 2e6f 626a 6563 7473 2e67 6574 222c  ge.objects.get",
-00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00003750: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
-00003760: 4354 225d 7d2c 0a20 2020 2020 2020 2020  CT"]},.         
-00003770: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00003780: 6765 2e6f 626a 6563 7473 2e6c 6973 7422  ge.objects.list"
-00003790: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
-000037a0: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-000037b0: 5b22 4255 434b 4554 222c 2022 4f42 4a45  ["BUCKET", "OBJE
-000037c0: 4354 225d 7d2c 0a20 2020 2020 2020 2020  CT"]},.         
-000037d0: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-000037e0: 6765 2e6f 626a 6563 7473 2e69 6e73 6572  ge.objects.inser
-000037f0: 7422 2c20 2020 2020 2020 2020 2020 2020  t",             
-00003800: 2020 2022 7265 736f 7572 6365 7322 3a20     "resources": 
-00003810: 5b22 4255 434b 4554 225d 7d2c 0a20 2020  ["BUCKET"]},.   
-00003820: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00003830: 2273 746f 7261 6765 2e6f 626a 6563 7473  "storage.objects
-00003840: 2e70 6174 6368 222c 2020 2020 2020 2020  .patch",        
-00003850: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-00003860: 6365 7322 3a20 5b22 4255 434b 4554 222c  ces": ["BUCKET",
-00003870: 2022 4f42 4a45 4354 225d 7d2c 0a20 2020   "OBJECT"]},.   
-00003880: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00003890: 2273 746f 7261 6765 2e6f 626a 6563 7473  "storage.objects
-000038a0: 2e72 6577 7269 7465 222c 2020 2020 2020  .rewrite",      
-000038b0: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-000038c0: 6365 7322 3a20 5b22 4255 434b 4554 222c  ces": ["BUCKET",
-000038d0: 2022 4f42 4a45 4354 225d 7d2c 0a20 2020   "OBJECT"]},.   
-000038e0: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-000038f0: 2273 746f 7261 6765 2e6f 626a 6563 7473  "storage.objects
-00003900: 2e75 7064 6174 6522 2c20 2020 2020 2020  .update",       
-00003910: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-00003920: 6365 7322 3a20 5b22 4255 434b 4554 222c  ces": ["BUCKET",
-00003930: 2022 4f42 4a45 4354 225d 7d2c 0a20 2020   "OBJECT"]},.   
-00003940: 2020 2020 2020 207b 226e 616d 6522 3a20         {"name": 
-00003950: 2273 746f 7261 6765 2e73 6572 7669 6365  "storage.service
-00003960: 6163 636f 756e 742e 6765 7422 2c20 2020  account.get",   
-00003970: 2020 2020 2020 2020 2022 7265 736f 7572           "resour
-00003980: 6365 7322 3a20 5b5d 7d0a 2020 2020 2020  ces": []}.      
-00003990: 2020 5d2c 0a20 2020 2020 2020 2022 7072    ],.        "pr
-000039a0: 6563 6f6e 6469 7469 6f6e 5072 6f76 6964  econditionProvid
-000039b0: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-000039c0: 2020 2022 6578 7065 6374 5375 6363 6573     "expectSucces
-000039d0: 7322 3a20 6661 6c73 650a 2020 2020 2020  s": false.      
-000039e0: 7d2c 0a20 2020 2020 207b 0a20 2020 2020  },.      {.     
-000039f0: 2020 2022 6964 223a 2037 2c0a 2020 2020     "id": 7,.    
-00003a00: 2020 2020 2264 6573 6372 6970 7469 6f6e      "description
-00003a10: 223a 2022 7265 7375 6d61 626c 655f 7570  ": "resumable_up
-00003a20: 6c6f 6164 735f 6861 6e64 6c65 5f63 6f6d  loads_handle_com
-00003a30: 706c 6578 5f72 6574 7269 6573 222c 0a20  plex_retries",. 
-00003a40: 2020 2020 2020 2022 6361 7365 7322 3a20         "cases": 
-00003a50: 5b0a 2020 2020 2020 2020 2020 7b0a 2020  [.          {.  
-00003a60: 2020 2020 2020 2020 2020 2269 6e73 7472            "instr
-00003a70: 7563 7469 6f6e 7322 3a20 5b22 7265 7475  uctions": ["retu
-00003a80: 726e 2d72 6573 6574 2d63 6f6e 6e65 6374  rn-reset-connect
-00003a90: 696f 6e22 2c20 2272 6574 7572 6e2d 3530  ion", "return-50
-00003aa0: 3322 5d0a 2020 2020 2020 2020 2020 7d2c  3"].          },
-00003ab0: 0a20 2020 2020 2020 2020 207b 0a20 2020  .          {.   
-00003ac0: 2020 2020 2020 2020 2022 696e 7374 7275           "instru
-00003ad0: 6374 696f 6e73 223a 205b 2272 6574 7572  ctions": ["retur
-00003ae0: 6e2d 3530 332d 6166 7465 722d 3235 364b  n-503-after-256K
-00003af0: 225d 0a20 2020 2020 2020 2020 207d 2c0a  "].          },.
-00003b00: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00003b10: 2020 2020 2020 2020 2269 6e73 7472 7563          "instruc
-00003b20: 7469 6f6e 7322 3a20 5b22 7265 7475 726e  tions": ["return
-00003b30: 2d35 3033 2d61 6674 6572 2d38 3139 324b  -503-after-8192K
-00003b40: 225d 0a20 2020 2020 2020 2020 207d 0a20  "].          }. 
-00003b50: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00003b60: 2020 226d 6574 686f 6473 223a 205b 0a20    "methods": [. 
-00003b70: 2020 2020 2020 2020 207b 226e 616d 6522           {"name"
-00003b80: 3a20 2273 746f 7261 6765 2e6f 626a 6563  : "storage.objec
-00003b90: 7473 2e69 6e73 6572 7422 2c20 2267 726f  ts.insert", "gro
-00003ba0: 7570 223a 2022 7374 6f72 6167 652e 7265  up": "storage.re
-00003bb0: 7375 6d61 626c 652e 7570 6c6f 6164 222c  sumable.upload",
-00003bc0: 2022 7265 736f 7572 6365 7322 3a20 5b22   "resources": ["
-00003bd0: 4255 434b 4554 225d 7d0a 2020 2020 2020  BUCKET"]}.      
-00003be0: 2020 5d2c 0a20 2020 2020 2020 2022 7072    ],.        "pr
-00003bf0: 6563 6f6e 6469 7469 6f6e 5072 6f76 6964  econditionProvid
-00003c00: 6564 223a 2074 7275 652c 0a20 2020 2020  ed": true,.     
-00003c10: 2020 2022 6578 7065 6374 5375 6363 6573     "expectSucces
-00003c20: 7322 3a20 7472 7565 0a20 2020 2020 207d  s": true.      }
-00003c30: 2c0a 2020 2020 2020 7b0a 2020 2020 2020  ,.      {.      
-00003c40: 2020 2269 6422 3a20 382c 0a20 2020 2020    "id": 8,.     
-00003c50: 2020 2022 6465 7363 7269 7074 696f 6e22     "description"
-00003c60: 3a20 2264 6f77 6e6c 6f61 6473 5f68 616e  : "downloads_han
-00003c70: 646c 655f 636f 6d70 6c65 785f 7265 7472  dle_complex_retr
-00003c80: 6965 7322 2c0a 2020 2020 2020 2020 2263  ies",.        "c
-00003c90: 6173 6573 223a 205b 0a20 2020 2020 2020  ases": [.       
-00003ca0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00003cb0: 2022 696e 7374 7275 6374 696f 6e73 223a   "instructions":
-00003cc0: 205b 2272 6574 7572 6e2d 6272 6f6b 656e   ["return-broken
-00003cd0: 2d73 7472 6561 6d22 2c20 2272 6574 7572  -stream", "retur
-00003ce0: 6e2d 6272 6f6b 656e 2d73 7472 6561 6d22  n-broken-stream"
-00003cf0: 5d0a 2020 2020 2020 2020 2020 7d2c 0a20  ].          },. 
-00003d00: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00003d10: 2020 2020 2020 2022 696e 7374 7275 6374         "instruct
-00003d20: 696f 6e73 223a 205b 2272 6574 7572 6e2d  ions": ["return-
-00003d30: 6272 6f6b 656e 2d73 7472 6561 6d2d 6166  broken-stream-af
-00003d40: 7465 722d 3235 364b 225d 0a20 2020 2020  ter-256K"].     
-00003d50: 2020 2020 207d 0a20 2020 2020 2020 205d       }.        ]
-00003d60: 2c0a 2020 2020 2020 2020 226d 6574 686f  ,.        "metho
-00003d70: 6473 223a 205b 0a20 2020 2020 2020 2020  ds": [.         
-00003d80: 207b 226e 616d 6522 3a20 2273 746f 7261   {"name": "stora
-00003d90: 6765 2e6f 626a 6563 7473 2e67 6574 222c  ge.objects.get",
-00003da0: 2022 6772 6f75 7022 3a20 2273 746f 7261   "group": "stora
-00003db0: 6765 2e6f 626a 6563 7473 2e64 6f77 6e6c  ge.objects.downl
-00003dc0: 6f61 6422 2c20 2272 6573 6f75 7263 6573  oad", "resources
-00003dd0: 223a 205b 2242 5543 4b45 5422 2c20 224f  ": ["BUCKET", "O
-00003de0: 424a 4543 5422 5d7d 0a20 2020 2020 2020  BJECT"]}.       
-00003df0: 205d 2c0a 2020 2020 2020 2020 2270 7265   ],.        "pre
-00003e00: 636f 6e64 6974 696f 6e50 726f 7669 6465  conditionProvide
-00003e10: 6422 3a20 6661 6c73 652c 0a20 2020 2020  d": false,.     
-00003e20: 2020 2022 6578 7065 6374 5375 6363 6573     "expectSucces
-00003e30: 7322 3a20 7472 7565 0a20 2020 2020 207d  s": true.      }
-00003e40: 0a20 2020 205d 0a20 207d                 .    ].  }
+00003680: 2020 2272 6573 6f75 7263 6573 223a 205b    "resources": [
+00003690: 2242 5543 4b45 5422 2c20 224f 424a 4543  "BUCKET", "OBJEC
+000036a0: 5422 5d7d 2c0a 2020 2020 2020 2020 7b22  T"]},.        {"
+000036b0: 6e61 6d65 223a 2022 7374 6f72 6167 652e  name": "storage.
+000036c0: 6f62 6a65 6374 732e 7265 7772 6974 6522  objects.rewrite"
+000036d0: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+000036e0: 2272 6573 6f75 7263 6573 223a 205b 2242  "resources": ["B
+000036f0: 5543 4b45 5422 2c20 224f 424a 4543 5422  UCKET", "OBJECT"
+00003700: 5d7d 2c0a 2020 2020 2020 2020 7b22 6e61  ]},.        {"na
+00003710: 6d65 223a 2022 7374 6f72 6167 652e 6f62  me": "storage.ob
+00003720: 6a65 6374 732e 7570 6461 7465 222c 2020  jects.update",  
+00003730: 2020 2020 2020 2020 2020 2020 2020 2272                "r
+00003740: 6573 6f75 7263 6573 223a 205b 2242 5543  esources": ["BUC
+00003750: 4b45 5422 2c20 224f 424a 4543 5422 5d7d  KET", "OBJECT"]}
+00003760: 2c0a 2020 2020 2020 2020 7b22 6e61 6d65  ,.        {"name
+00003770: 223a 2022 7374 6f72 6167 652e 7365 7276  ": "storage.serv
+00003780: 6963 6561 6363 6f75 6e74 2e67 6574 222c  iceaccount.get",
+00003790: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+000037a0: 6f75 7263 6573 223a 205b 5d7d 0a20 2020  ources": []}.   
+000037b0: 2020 205d 2c0a 2020 2020 2020 2270 7265     ],.      "pre
+000037c0: 636f 6e64 6974 696f 6e50 726f 7669 6465  conditionProvide
+000037d0: 6422 3a20 7472 7565 2c0a 2020 2020 2020  d": true,.      
+000037e0: 2265 7870 6563 7453 7563 6365 7373 223a  "expectSuccess":
+000037f0: 2066 616c 7365 0a20 2020 207d 2c0a 2020   false.    },.  
+00003800: 2020 7b0a 2020 2020 2020 2269 6422 3a20    {.      "id": 
+00003810: 372c 0a20 2020 2020 2022 6465 7363 7269  7,.      "descri
+00003820: 7074 696f 6e22 3a20 2272 6573 756d 6162  ption": "resumab
+00003830: 6c65 5f75 706c 6f61 6473 5f68 616e 646c  le_uploads_handl
+00003840: 655f 636f 6d70 6c65 785f 7265 7472 6965  e_complex_retrie
+00003850: 7322 2c0a 2020 2020 2020 2263 6173 6573  s",.      "cases
+00003860: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+00003870: 2020 2020 2020 2020 2022 696e 7374 7275           "instru
+00003880: 6374 696f 6e73 223a 205b 2272 6574 7572  ctions": ["retur
+00003890: 6e2d 7265 7365 742d 636f 6e6e 6563 7469  n-reset-connecti
+000038a0: 6f6e 222c 2022 7265 7475 726e 2d35 3033  on", "return-503
+000038b0: 225d 0a20 2020 2020 2020 207d 2c0a 2020  "].        },.  
+000038c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000038d0: 2020 2269 6e73 7472 7563 7469 6f6e 7322    "instructions"
+000038e0: 3a20 5b22 7265 7475 726e 2d34 3038 225d  : ["return-408"]
+000038f0: 0a20 2020 2020 2020 207d 2c0a 2020 2020  .        },.    
+00003900: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00003910: 2269 6e73 7472 7563 7469 6f6e 7322 3a20  "instructions": 
+00003920: 5b22 7265 7475 726e 2d35 3033 2d61 6674  ["return-503-aft
+00003930: 6572 2d32 3536 4b22 5d0a 2020 2020 2020  er-256K"].      
+00003940: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00003950: 2020 2020 2020 2020 2022 696e 7374 7275           "instru
+00003960: 6374 696f 6e73 223a 205b 2272 6574 7572  ctions": ["retur
+00003970: 6e2d 3530 332d 6166 7465 722d 3831 3932  n-503-after-8192
+00003980: 4b22 2c20 2272 6574 7572 6e2d 3430 3822  K", "return-408"
+00003990: 5d0a 2020 2020 2020 2020 7d0a 2020 2020  ].        }.    
+000039a0: 2020 5d2c 0a20 2020 2020 2022 6d65 7468    ],.      "meth
+000039b0: 6f64 7322 3a20 5b0a 2020 2020 2020 2020  ods": [.        
+000039c0: 7b22 6e61 6d65 223a 2022 7374 6f72 6167  {"name": "storag
+000039d0: 652e 6f62 6a65 6374 732e 696e 7365 7274  e.objects.insert
+000039e0: 222c 2022 6772 6f75 7022 3a20 2273 746f  ", "group": "sto
+000039f0: 7261 6765 2e72 6573 756d 6162 6c65 2e75  rage.resumable.u
+00003a00: 706c 6f61 6422 2c20 2272 6573 6f75 7263  pload", "resourc
+00003a10: 6573 223a 205b 2242 5543 4b45 5422 5d7d  es": ["BUCKET"]}
+00003a20: 0a20 2020 2020 205d 2c0a 2020 2020 2020  .      ],.      
+00003a30: 2270 7265 636f 6e64 6974 696f 6e50 726f  "preconditionPro
+00003a40: 7669 6465 6422 3a20 7472 7565 2c0a 2020  vided": true,.  
+00003a50: 2020 2020 2265 7870 6563 7453 7563 6365      "expectSucce
+00003a60: 7373 223a 2074 7275 650a 2020 2020 7d2c  ss": true.    },
+00003a70: 0a20 2020 207b 0a20 2020 2020 2022 6964  .    {.      "id
+00003a80: 223a 2038 2c0a 2020 2020 2020 2264 6573  ": 8,.      "des
+00003a90: 6372 6970 7469 6f6e 223a 2022 646f 776e  cription": "down
+00003aa0: 6c6f 6164 735f 6861 6e64 6c65 5f63 6f6d  loads_handle_com
+00003ab0: 706c 6578 5f72 6574 7269 6573 222c 0a20  plex_retries",. 
+00003ac0: 2020 2020 2022 6361 7365 7322 3a20 5b0a       "cases": [.
+00003ad0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00003ae0: 2020 2020 2269 6e73 7472 7563 7469 6f6e      "instruction
+00003af0: 7322 3a20 5b22 7265 7475 726e 2d62 726f  s": ["return-bro
+00003b00: 6b65 6e2d 7374 7265 616d 222c 2022 7265  ken-stream", "re
+00003b10: 7475 726e 2d62 726f 6b65 6e2d 7374 7265  turn-broken-stre
+00003b20: 616d 225d 0a20 2020 2020 2020 207d 2c0a  am"].        },.
+00003b30: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00003b40: 2020 2020 2269 6e73 7472 7563 7469 6f6e      "instruction
+00003b50: 7322 3a20 5b22 7265 7475 726e 2d62 726f  s": ["return-bro
+00003b60: 6b65 6e2d 7374 7265 616d 2d61 6674 6572  ken-stream-after
+00003b70: 2d32 3536 4b22 5d0a 2020 2020 2020 2020  -256K"].        
+00003b80: 7d0a 2020 2020 2020 5d2c 0a20 2020 2020  }.      ],.     
+00003b90: 2022 6d65 7468 6f64 7322 3a20 5b0a 2020   "methods": [.  
+00003ba0: 2020 2020 2020 7b22 6e61 6d65 223a 2022        {"name": "
+00003bb0: 7374 6f72 6167 652e 6f62 6a65 6374 732e  storage.objects.
+00003bc0: 6765 7422 2c20 2267 726f 7570 223a 2022  get", "group": "
+00003bd0: 7374 6f72 6167 652e 6f62 6a65 6374 732e  storage.objects.
+00003be0: 646f 776e 6c6f 6164 222c 2022 7265 736f  download", "reso
+00003bf0: 7572 6365 7322 3a20 5b22 4255 434b 4554  urces": ["BUCKET
+00003c00: 222c 2022 4f42 4a45 4354 225d 7d0a 2020  ", "OBJECT"]}.  
+00003c10: 2020 2020 5d2c 0a20 2020 2020 2022 7072      ],.      "pr
+00003c20: 6563 6f6e 6469 7469 6f6e 5072 6f76 6964  econditionProvid
+00003c30: 6564 223a 2066 616c 7365 2c0a 2020 2020  ed": false,.    
+00003c40: 2020 2265 7870 6563 7453 7563 6365 7373    "expectSuccess
+00003c50: 223a 2074 7275 650a 2020 2020 7d0a 2020  ": true.    }.  
+00003c60: 5d0a 7d0a                                ].}.
```

### Comparing `google-cloud-storage-2.8.0/tests/conformance/test_conformance.py` & `google-cloud-storage-2.9.0/tests/conformance/test_conformance.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/data/CloudPlatform_128px_Retina.png` & `google-cloud-storage-2.9.0/tests/data/CloudPlatform_128px_Retina.png`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/data/five-point-one-mb-file.zip` & `google-cloud-storage-2.9.0/tests/data/five-point-one-mb-file.zip`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/perf/README.md` & `google-cloud-storage-2.9.0/tests/perf/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 **This is not an officially supported Google product**
 
 This benchmarking script is used by Storage client library maintainers to benchmark various workloads and collect metrics in order to improve performance of the library.
 Currently the benchmarking runs a Write-1-Read-3 workload and measures the usual two QoS performance attributes, latency and throughput.
 
 ## Run example:
-This runs 10K iterations of Write-1-Read-3 on 5KiB to 16KiB files, and generates output to a default csv file `benchmarking<TIMESTAMP>.csv`:
+This runs 10K iterations of Write-1-Read-3 on 5KiB to 16KiB files, and generates output to a default csv file `output_bench<TIMESTAMP>.csv`:
 ```bash
 $ cd python-storage
 $ pip install -e . # install google.cloud.storage locally
 $ cd tests/perf
-$ python3 benchmarking.py --num_samples 10000 --max_size 16384
+$ python3 benchmarking.py --num_samples 10000 --object_size 5120..16384 --output_type csv
 ```
 
 ## CLI parameters
 
 | Parameter | Description | Possible values | Default |
 | --------- | ----------- | --------------- |:-------:|
 | --project | GCP project identifier | a project id| * |
```

### Comparing `google-cloud-storage-2.8.0/tests/perf/_perf_utils.py` & `google-cloud-storage-2.9.0/tests/perf/_perf_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,18 +119,22 @@
 
 
 def convert_to_cloud_monitoring(bucket_name, results, workers):
     # Benchmarking main script uses Multiprocessing Pool.map(),
     # thus results is structured as List[List[Dict[str, any]]].
     for result in results:
         for res in result:
+            # Only output successful benchmarking runs to cloud monitoring.
+            status = res.get("Status").pop()  # convert ["OK"] --> "OK"
+            if status != "OK":
+                continue
+
             range_read_size = res.get("RangeReadSize", 0)
             object_size = res.get("ObjectSize")
             elapsed_time_us = res.get("ElapsedTimeUs")
-            status = res.get("Status").pop()  # convert ["OK"] --> "OK"
 
             # Handle range reads and calculate throughput using range_read_size.
             if range_read_size > 0:
                 size = range_read_size
             else:
                 size = object_size
 
@@ -210,7 +214,21 @@
         min_size = int(object_size)
         max_size = int(object_size)
     else:
         split_sizes = object_size.split("..")
         min_size = int(split_sizes[0])
         max_size = int(split_sizes[1])
     return min_size, max_size
+
+
+class logCount(logging.Handler):
+    class LogType:
+        def __init__(self):
+            self.errors = 0
+
+    def __init__(self):
+        super().__init__()
+        self.count = self.LogType()
+
+    def emit(self, record):
+        if record.levelname == "ERROR":
+            self.count.errors += 1
```

### Comparing `google-cloud-storage-2.8.0/tests/perf/benchmarking.py` & `google-cloud-storage-2.9.0/tests/perf/benchmarking.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,35 @@
 # limitations under the License.
 
 """Performance benchmarking main script. This is not an officially supported Google product."""
 
 import argparse
 import logging
 import multiprocessing
+import sys
 
 from google.cloud import storage
 
 import _perf_utils as _pu
 import profile_w1r3 as w1r3
 
 
 ##### PROFILE BENCHMARKING TEST TYPES #####
 PROFILE_WRITE_ONE_READ_THREE = "w1r3"
 PROFILE_RANGE_READ = "range"
 
 
 def main(args):
-    logging.info("Start benchmarking main script")
+    # Track error logging for BBMC reporting.
+    counter = _pu.logCount()
+    logging.basicConfig(
+        level=logging.ERROR,
+        handlers=[counter, logging.StreamHandler(sys.stderr)],
+    )
+
     # Create a storage bucket to run benchmarking.
     if args.project is not None:
         client = storage.Client(project=args.project)
     else:
         client = storage.Client()
 
     bucket = client.bucket(args.bucket)
@@ -71,14 +78,18 @@
         logging.info(
             f"Succesfully ran benchmarking. Please find your output log at {args.output_file}"
         )
 
     # Cleanup and delete blobs.
     _pu.cleanup_bucket(bucket)
 
+    # BBMC will not surface errors unless the process is terminated with a non zero code.
+    if counter.count.errors != 0:
+        sys.exit(1)
+
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--project",
         type=str,
         default=None,
```

### Comparing `google-cloud-storage-2.8.0/tests/perf/profile_w1r3.py` & `google-cloud-storage-2.9.0/tests/perf/profile_w1r3.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/_helpers.py` & `google-cloud-storage-2.9.0/tests/system/_helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/conftest.py` & `google-cloud-storage-2.9.0/tests/system/conftest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test__signing.py` & `google-cloud-storage-2.9.0/tests/system/test__signing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test_blob.py` & `google-cloud-storage-2.9.0/tests/system/test_blob.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test_bucket.py` & `google-cloud-storage-2.9.0/tests/system/test_bucket.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test_client.py` & `google-cloud-storage-2.9.0/tests/system/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test_fileio.py` & `google-cloud-storage-2.9.0/tests/system/test_fileio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test_hmac_key_metadata.py` & `google-cloud-storage-2.9.0/tests/system/test_hmac_key_metadata.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test_kms_integration.py` & `google-cloud-storage-2.9.0/tests/system/test_kms_integration.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test_notification.py` & `google-cloud-storage-2.9.0/tests/system/test_notification.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/system/test_transfer_manager.py` & `google-cloud-storage-2.9.0/tests/system/test_transfer_manager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/__init__.py` & `google-cloud-storage-2.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test__helpers.py` & `google-cloud-storage-2.9.0/tests/unit/test__helpers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test__http.py` & `google-cloud-storage-2.9.0/tests/unit/test__http.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test__signing.py` & `google-cloud-storage-2.9.0/tests/unit/test__signing.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_acl.py` & `google-cloud-storage-2.9.0/tests/unit/test_acl.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_batch.py` & `google-cloud-storage-2.9.0/tests/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_blob.py` & `google-cloud-storage-2.9.0/tests/unit/test_blob.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_bucket.py` & `google-cloud-storage-2.9.0/tests/unit/test_bucket.py`

 * *Files 0% similar despite different names*

```diff
@@ -2942,16 +2942,15 @@
 
     def test_versioning_enabled_getter(self):
         NAME = "name"
         before = {"versioning": {"enabled": True}}
         bucket = self._make_one(name=NAME, properties=before)
         self.assertEqual(bucket.versioning_enabled, True)
 
-    @mock.patch("warnings.warn")
-    def test_create_w_defaults_deprecated(self, mock_warn):
+    def test_create_w_defaults(self):
         bucket_name = "bucket-name"
         api_response = {"name": bucket_name}
         client = mock.Mock(spec=["create_bucket"])
         client.create_bucket.return_value = api_response
         bucket = self._make_one(client=client, name=bucket_name)
 
         bucket.create()
@@ -2963,23 +2962,15 @@
             location=None,
             predefined_acl=None,
             predefined_default_object_acl=None,
             timeout=self._get_default_timeout(),
             retry=DEFAULT_RETRY,
         )
 
-        mock_warn.assert_called_with(
-            "Bucket.create() is deprecated and will be removed in future."
-            "Use Client.create_bucket() instead.",
-            PendingDeprecationWarning,
-            stacklevel=1,
-        )
-
-    @mock.patch("warnings.warn")
-    def test_create_w_explicit_deprecated(self, mock_warn):
+    def test_create_w_explicit(self):
         project = "PROJECT"
         location = "eu"
         user_project = "USER_PROJECT"
         bucket_name = "bucket-name"
         predefined_acl = "authenticatedRead"
         predefined_default_object_acl = "bucketOwnerFullControl"
         api_response = {"name": bucket_name}
@@ -3007,21 +2998,14 @@
             location=location,
             predefined_acl=predefined_acl,
             predefined_default_object_acl=predefined_default_object_acl,
             timeout=timeout,
             retry=retry,
         )
 
-        mock_warn.assert_called_with(
-            "Bucket.create() is deprecated and will be removed in future."
-            "Use Client.create_bucket() instead.",
-            PendingDeprecationWarning,
-            stacklevel=1,
-        )
-
     def test_versioning_enabled_setter(self):
         NAME = "name"
         bucket = self._make_one(name=NAME)
         self.assertFalse(bucket.versioning_enabled)
         bucket.versioning_enabled = True
         self.assertTrue(bucket.versioning_enabled)
```

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_client.py` & `google-cloud-storage-2.9.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_fileio.py` & `google-cloud-storage-2.9.0/tests/unit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_hmac_key.py` & `google-cloud-storage-2.9.0/tests/unit/test_hmac_key.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_notification.py` & `google-cloud-storage-2.9.0/tests/unit/test_notification.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_retry.py` & `google-cloud-storage-2.9.0/tests/unit/test_retry.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/test_transfer_manager.py` & `google-cloud-storage-2.9.0/tests/unit/test_transfer_manager.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/url_signer_v4_test_account.json` & `google-cloud-storage-2.9.0/tests/unit/url_signer_v4_test_account.json`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-2.8.0/tests/unit/url_signer_v4_test_data.json` & `google-cloud-storage-2.9.0/tests/unit/url_signer_v4_test_data.json`

 * *Files identical despite different names*

