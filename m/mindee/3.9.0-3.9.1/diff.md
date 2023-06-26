# Comparing `tmp/mindee-3.9.0.tar.gz` & `tmp/mindee-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-3.9.0.tar", last modified: Tue Jun  6 14:06:05 2023, max compression
+gzip compressed data, was "mindee-3.9.1.tar", last modified: Wed Jun  7 15:55:05 2023, max compression
```

## Comparing `mindee-3.9.0.tar` & `mindee-3.9.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.666709 mindee-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-06 14:05:44.000000 mindee-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-06 14:06:05.666709 mindee-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-06 14:05:44.000000 mindee-3.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.650709 mindee-3.9.0/mindee/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/cropper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/cropper/cropper_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/custom/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/custom/custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/custom/custom_v1_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/eu/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/eu/license_plate/license_plate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/financial_document/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/financial_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/financial_document/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/financial_document/financial_document_v1_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/financial_document/financial_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/carte_grise/carte_grise_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/id_card/id_card_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/invoice_v4_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/invoice_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice_splitter/invoice_splitter_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/passport/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/passport/passport_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/proof_of_address/proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/receipt/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/receipt_v5_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/shipping_container/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/shipping_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/shipping_container/shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/response.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/version
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:05:48.000000 mindee-3.9.0/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 14:05:44.000000 mindee-3.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-06 14:06:05.666709 mindee-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-06 14:05:44.000000 mindee-3.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/tests/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/tests/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_financial_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_invoice_splitter_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/tests/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/us/test_bank_check_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.666709 mindee-3.9.0/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_pkg_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.219216 mindee-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-07 15:54:45.000000 mindee-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-07 15:55:05.219216 mindee-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-07 15:54:45.000000 mindee-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.203216 mindee-3.9.1/mindee/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/cropper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/cropper/cropper_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/custom/custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/custom/custom_v1_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/eu/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/eu/license_plate/license_plate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/financial_document/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/financial_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/financial_document/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/financial_document/financial_document_v1_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/financial_document/financial_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/carte_grise/carte_grise_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/fr/id_card/id_card_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/invoice/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/invoice/invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/invoice/invoice_v4_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/invoice/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/invoice_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/invoice_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/invoice_splitter/invoice_splitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/passport/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/passport/passport_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.207216 mindee-3.9.1/mindee/documents/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/proof_of_address/proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.211216 mindee-3.9.1/mindee/documents/receipt/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/receipt/receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/receipt/receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/receipt/receipt_v5_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.211216 mindee-3.9.1/mindee/documents/shipping_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/shipping_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/shipping_container/shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.211216 mindee-3.9.1/mindee/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.211216 mindee-3.9.1/mindee/documents/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/documents/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.211216 mindee-3.9.1/mindee/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.211216 mindee-3.9.1/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-07 15:54:45.000000 mindee-3.9.1/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.203216 mindee-3.9.1/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-07 15:55:05.000000 mindee-3.9.1/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-07 15:55:05.000000 mindee-3.9.1/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:55:05.000000 mindee-3.9.1/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 15:55:05.000000 mindee-3.9.1/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:54:49.000000 mindee-3.9.1/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-07 15:55:05.000000 mindee-3.9.1/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 15:55:05.000000 mindee-3.9.1/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-07 15:54:45.000000 mindee-3.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-07 15:55:05.219216 mindee-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 15:54:45.000000 mindee-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.215216 mindee-3.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.215216 mindee-3.9.1/tests/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.215216 mindee-3.9.1/tests/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/fr/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/fr/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/fr/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/fr/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_financial_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_invoice_splitter_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/test_shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.215216 mindee-3.9.1/tests/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/documents/us/test_bank_check_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:55:05.219216 mindee-3.9.1/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-07 15:54:45.000000 mindee-3.9.1/tests/test_pkg_versions.py
```

### Comparing `mindee-3.9.0/LICENSE` & `mindee-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/PKG-INFO` & `mindee-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.9.0
+Version: 3.9.1
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.9.0/README.md` & `mindee-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/cli.py` & `mindee-3.9.1/mindee/cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/client.py` & `mindee-3.9.1/mindee/client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/__init__.py` & `mindee-3.9.1/mindee/documents/__init__.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/base.py` & `mindee-3.9.1/mindee/documents/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/config.py` & `mindee-3.9.1/mindee/documents/config.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/cropper/cropper_v1.py` & `mindee-3.9.1/mindee/documents/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/custom/custom_v1.py` & `mindee-3.9.1/mindee/documents/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/custom/custom_v1_fields.py` & `mindee-3.9.1/mindee/documents/custom/custom_v1_fields.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/eu/license_plate/license_plate_v1.py` & `mindee-3.9.1/mindee/documents/eu/license_plate/license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/financial_document/financial_document_v1.py` & `mindee-3.9.1/mindee/documents/financial_document/financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/financial_document/financial_document_v1_line_item.py` & `mindee-3.9.1/mindee/documents/financial_document/financial_document_v1_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/financial_document/financial_v1.py` & `mindee-3.9.1/mindee/documents/financial_document/financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py` & `mindee-3.9.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/fr/carte_grise/carte_grise_v1.py` & `mindee-3.9.1/mindee/documents/fr/carte_grise/carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py` & `mindee-3.9.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/fr/id_card/id_card_v1.py` & `mindee-3.9.1/mindee/documents/fr/id_card/id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/invoice/checks.py` & `mindee-3.9.1/mindee/documents/invoice/checks.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/invoice/invoice_v3.py` & `mindee-3.9.1/mindee/documents/invoice/invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/invoice/invoice_v4.py` & `mindee-3.9.1/mindee/documents/invoice/invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/invoice/invoice_v4_line_item.py` & `mindee-3.9.1/mindee/documents/invoice/invoice_v4_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/invoice/reconstruct.py` & `mindee-3.9.1/mindee/documents/invoice/reconstruct.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/invoice_splitter/invoice_splitter_v1.py` & `mindee-3.9.1/mindee/documents/invoice_splitter/invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/passport/passport_v1.py` & `mindee-3.9.1/mindee/documents/passport/passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/proof_of_address/proof_of_address_v1.py` & `mindee-3.9.1/mindee/documents/proof_of_address/proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/receipt/receipt_v3.py` & `mindee-3.9.1/mindee/documents/receipt/receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/receipt/receipt_v4.py` & `mindee-3.9.1/mindee/documents/receipt/receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/receipt/receipt_v5.py` & `mindee-3.9.1/mindee/documents/receipt/receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/receipt/receipt_v5_line_item.py` & `mindee-3.9.1/mindee/documents/receipt/receipt_v5_line_item.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/shipping_container/shipping_container_v1.py` & `mindee-3.9.1/mindee/documents/shipping_container/shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/documents/us/bank_check/bank_check_v1.py` & `mindee-3.9.1/mindee/documents/us/bank_check/bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/endpoints.py` & `mindee-3.9.1/mindee/endpoints.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/amount.py` & `mindee-3.9.1/mindee/fields/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/base.py` & `mindee-3.9.1/mindee/fields/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/classification.py` & `mindee-3.9.1/mindee/fields/classification.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/company_registration.py` & `mindee-3.9.1/mindee/fields/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/date.py` & `mindee-3.9.1/mindee/fields/date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/locale.py` & `mindee-3.9.1/mindee/fields/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/ocr.py` & `mindee-3.9.1/mindee/fields/ocr.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 from typing import List, Optional
 
 from mindee.documents.base import TypeApiPrediction
+from mindee.fields.base import FieldPositionMixin
 from mindee.geometry import (
-    Polygon,
     get_centroid,
     get_min_max_x,
     get_min_max_y,
     is_point_in_polygon_y,
-    polygon_from_prediction,
 )
 
 
-class Word:
+class OcrWord(FieldPositionMixin):
     """A single word."""
 
     confidence: float
-    polygon: Polygon
+    """The confidence score."""
     text: str
+    """The extracted text."""
 
     def __init__(self, prediction: TypeApiPrediction):
         self.confidence = prediction["confidence"]
-        self.polygon = polygon_from_prediction(prediction["polygon"])
         self.text = prediction["text"]
+        self._set_position(prediction)
 
     def __str__(self) -> str:
         return self.text
 
 
-class OcrLine(List[Word]):
+class OcrLine(List[OcrWord]):
     """A list of words which are on the same line."""
 
     def sort_on_x(self) -> None:
         """Sort the words on the line from left to right."""
         self.sort(key=lambda item: get_min_max_x(item.polygon).min)
 
     def __str__(self) -> str:
         return " ".join([word.text for word in self])
 
 
 class OcrPage:
     """OCR extraction for a single page."""
 
-    all_words: List[Word]
+    all_words: List[OcrWord]
     """All the words on the page, in semi-random order."""
     _lines: List[OcrLine]
 
     def __init__(self, prediction: TypeApiPrediction):
         self.all_words = [
-            Word(word_prediction) for word_prediction in prediction["all_words"]
+            OcrWord(word_prediction) for word_prediction in prediction["all_words"]
         ]
         self._lines = []
 
     @staticmethod
-    def _are_words_on_same_line(current_word: Word, next_word: Word) -> bool:
+    def _are_words_on_same_line(current_word: OcrWord, next_word: OcrWord) -> bool:
         """Determine if two words are on the same line."""
         current_in_next = is_point_in_polygon_y(
             get_centroid(current_word.polygon),
             next_word.polygon,
         )
         next_in_current = is_point_in_polygon_y(
             get_centroid(next_word.polygon), current_word.polygon
         )
         # We need to check both to eliminate any issues due to word order.
         return current_in_next or next_in_current
 
     def _to_lines(self) -> List[OcrLine]:
         """Order all the words on the page into lines."""
-        current: Optional[Word] = None
+        current: Optional[OcrWord] = None
         indexes: List[int] = []
         lines: List[OcrLine] = []
 
         # make sure words are sorted from top to bottom
         self.all_words.sort(
             key=lambda item: get_min_max_y(item.polygon).min, reverse=False
         )
@@ -106,27 +106,29 @@
         return "\n".join(str(line) for line in self.all_lines) + "\n"
 
 
 class MVisionV1:
     """Mindee Vision V1."""
 
     pages: List[OcrPage]
+    """List of pages."""
 
     def __init__(self, prediction: TypeApiPrediction):
         self.pages = [
             OcrPage(page_prediction) for page_prediction in prediction["pages"]
         ]
 
     def __str__(self) -> str:
         return "\n".join([str(page) for page in self.pages])
 
 
 class Ocr:
     """OCR extraction from the entire document."""
 
     mvision_v1: MVisionV1
+    """Mindee Vision v1 results."""
 
     def __init__(self, prediction: TypeApiPrediction):
         self.mvision_v1 = MVisionV1(prediction["mvision-v1"])
 
     def __str__(self) -> str:
         return str(self.mvision_v1)
```

### Comparing `mindee-3.9.0/mindee/fields/orientation.py` & `mindee-3.9.1/mindee/fields/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/payment_details.py` & `mindee-3.9.1/mindee/fields/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/position.py` & `mindee-3.9.1/mindee/fields/position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/tax.py` & `mindee-3.9.1/mindee/fields/tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/fields/text.py` & `mindee-3.9.1/mindee/fields/text.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/geometry.py` & `mindee-3.9.1/mindee/geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/input/page_options.py` & `mindee-3.9.1/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/input/sources.py` & `mindee-3.9.1/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/response.py` & `mindee-3.9.1/mindee/response.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee/versions.py` & `mindee-3.9.1/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/mindee.egg-info/PKG-INFO` & `mindee-3.9.1/mindee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.9.0
+Version: 3.9.1
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.9.0/mindee.egg-info/SOURCES.txt` & `mindee-3.9.1/mindee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/pyproject.toml` & `mindee-3.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/setup.cfg` & `mindee-3.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/fr/test_bank_account_details_v1.py` & `mindee-3.9.1/tests/documents/fr/test_bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/fr/test_carte_grise_v1.py` & `mindee-3.9.1/tests/documents/fr/test_carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/fr/test_carte_vitale_v1.py` & `mindee-3.9.1/tests/documents/fr/test_carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/fr/test_id_card_v1.py` & `mindee-3.9.1/tests/documents/fr/test_id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_cropper_v1.py` & `mindee-3.9.1/tests/documents/test_cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_custom_v1.py` & `mindee-3.9.1/tests/documents/test_custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_financial_document_v1.py` & `mindee-3.9.1/tests/documents/test_financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_financial_v1.py` & `mindee-3.9.1/tests/documents/test_financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_invoice_splitter_v1.py` & `mindee-3.9.1/tests/documents/test_invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_invoice_v3.py` & `mindee-3.9.1/tests/documents/test_invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_invoice_v4.py` & `mindee-3.9.1/tests/documents/test_invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_passport_v1.py` & `mindee-3.9.1/tests/documents/test_passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_proof_of_address_v1.py` & `mindee-3.9.1/tests/documents/test_proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_receipt_v3.py` & `mindee-3.9.1/tests/documents/test_receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_receipt_v4.py` & `mindee-3.9.1/tests/documents/test_receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_receipt_v5.py` & `mindee-3.9.1/tests/documents/test_receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/test_shipping_container_v1.py` & `mindee-3.9.1/tests/documents/test_shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/documents/us/test_bank_check_v1.py` & `mindee-3.9.1/tests/documents/us/test_bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/fields/test_amount.py` & `mindee-3.9.1/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/fields/test_date.py` & `mindee-3.9.1/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/fields/test_field.py` & `mindee-3.9.1/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/fields/test_locale.py` & `mindee-3.9.1/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/fields/test_orientation.py` & `mindee-3.9.1/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/fields/test_payment_details.py` & `mindee-3.9.1/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/fields/test_position.py` & `mindee-3.9.1/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/fields/test_tax.py` & `mindee-3.9.1/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/test_cli.py` & `mindee-3.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/test_client.py` & `mindee-3.9.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/test_geometry.py` & `mindee-3.9.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/test_inputs.py` & `mindee-3.9.1/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-3.9.0/tests/test_pkg_versions.py` & `mindee-3.9.1/tests/test_pkg_versions.py`

 * *Files identical despite different names*

