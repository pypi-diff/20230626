# Comparing `tmp/django-oasis4-1.1.1a2.tar.gz` & `tmp/django-oasis4-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-1.1.1a2.tar", last modified: Wed May 24 04:03:34 2023, max compression
+gzip compressed data, was "django-oasis4-1.1.2.tar", last modified: Mon Jun 26 19:39:15 2023, max compression
```

## Comparing `django-oasis4-1.1.1a2.tar` & `django-oasis4-1.1.2.tar`

### file list

```diff
@@ -1,149 +1,155 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.722520 django-oasis4-1.1.1a2/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-1.1.1a2/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-03-02 20:32:01.000000 django-oasis4-1.1.1a2/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-05-24 04:03:34.722520 django-oasis4-1.1.1a2/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      217 2023-02-13 15:48:51.000000 django-oasis4-1.1.1a2/README.md
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.704521 django-oasis4-1.1.1a2/django_oasis4.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4419 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       78 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        6 2023-05-24 04:03:34.000000 django-oasis4-1.1.1a2/django_oasis4.egg-info/top_level.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.704521 django-oasis4-1.1.1a2/oasis/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-10 23:55:40.000000 django-oasis4-1.1.1a2/oasis/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1394 2023-03-18 18:38:34.000000 django-oasis4-1.1.1a2/oasis/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.705520 django-oasis4-1.1.1a2/oasis/coffee_offers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-22 14:19:30.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      686 2023-03-06 19:37:38.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/admin.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1253 2023-03-07 16:31:05.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/admin_views.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.705520 django-oasis4-1.1.1a2/oasis/coffee_offers/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-23 15:03:46.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.706520 django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      683 2023-03-06 19:10:13.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      772 2023-02-23 15:21:03.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1199 2023-03-06 20:11:27.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/offer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.706520 django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-03-01 20:03:07.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11193 2023-04-03 19:11:07.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/coffee_offers.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4101 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.706520 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-26 20:27:18.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.707520 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      656 2023-02-26 20:35:07.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1137 2023-03-07 09:29:38.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/coffee_offers_states.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      739 2023-02-26 20:34:29.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/oasis_states.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.707520 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      417 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/events/on_post_save_offer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.708521 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 21:38:01.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3414 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/utils/offer_state_machine.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.708521 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      757 2023-02-26 21:14:28.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1336 2023-02-26 21:13:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/date_validators.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      823 2023-02-26 20:45:48.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/oasis_statuses.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.700521 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.700521 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.708521 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4521 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6279 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.709520 django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 23:14:13.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1365 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/sync_coffe_offers.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.710520 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1072 2023-03-08 13:40:32.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/change_status.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2023-03-08 13:40:32.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/change_status.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.710520 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/coffee_offers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/coffee_offers/contract_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/coffee_offers/promisory_note.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      123 2023-03-07 09:07:24.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/coffee_offers/terms_conditions.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1054 2023-03-02 20:24:29.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/save_offer.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      785 2023-03-02 20:03:04.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/templates/save_offer.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      981 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/coffee_offers/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.710520 django-oasis4-1.1.1a2/oasis/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-11-16 14:55:35.000000 django-oasis4-1.1.1a2/oasis/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.711520 django-oasis4-1.1.1a2/oasis/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      582 2023-01-17 21:45:20.000000 django-oasis4-1.1.1a2/oasis/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      783 2023-03-18 17:17:41.000000 django-oasis4-1.1.1a2/oasis/lib/choices/customer_type.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.714520 django-oasis4-1.1.1a2/oasis/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1525 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      780 2023-02-23 14:39:16.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      682 2023-01-28 14:38:17.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1355 2023-01-18 02:07:35.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_document_type.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1578 2023-03-08 14:17:45.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_offer.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1212 2022-12-14 20:34:45.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_product.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2159 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/lib/managers/local_state_machine.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1201 2023-03-02 21:35:32.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_associate_balance.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2701 2023-03-01 16:42:42.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_client.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1050 2023-01-27 03:47:52.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1390 2023-02-07 10:48:09.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4007 2023-01-24 23:42:01.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_discount.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-01-24 23:42:01.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_geographic_location.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      799 2023-02-23 14:57:09.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_location.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7130 2023-03-08 14:56:20.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_operation.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-02-06 19:28:19.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_periods.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      906 2022-12-19 16:49:04.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_product.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      730 2023-01-25 00:42:41.000000 django-oasis4-1.1.1a2/oasis/lib/managers/oasis_type_client.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.714520 django-oasis4-1.1.1a2/oasis/lib/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      658 2023-02-07 09:06:27.000000 django-oasis4-1.1.1a2/oasis/lib/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      789 2023-02-07 09:25:36.000000 django-oasis4-1.1.1a2/oasis/lib/serializers/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2022-12-14 20:01:00.000000 django-oasis4-1.1.1a2/oasis/lib/serializers/product.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.714520 django-oasis4-1.1.1a2/oasis/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      579 2023-03-03 19:38:17.000000 django-oasis4-1.1.1a2/oasis/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3274 2023-04-03 19:11:07.000000 django-oasis4-1.1.1a2/oasis/lib/utils/oasis_actions.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.701521 django-oasis4-1.1.1a2/oasis/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.701521 django-oasis4-1.1.1a2/oasis/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.715520 django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2138 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5606 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.718520 django-oasis4-1.1.1a2/oasis/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    29691 2022-12-13 18:21:01.000000 django-oasis4-1.1.1a2/oasis/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    31003 2023-01-17 22:22:35.000000 django-oasis4-1.1.1a2/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    17130 2023-01-26 02:36:44.000000 django-oasis4-1.1.1a2/oasis/migrations/0003_oasiscompany_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5814 2023-01-27 03:47:55.000000 django-oasis4-1.1.1a2/oasis/migrations/0004_account_vaccountingbalanceclient.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      515 2023-02-02 01:56:29.000000 django-oasis4-1.1.1a2/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1582 2023-02-05 00:32:58.000000 django-oasis4-1.1.1a2/oasis/migrations/0006_periods.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      949 2023-02-07 02:05:07.000000 django-oasis4-1.1.1a2/oasis/migrations/0007_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9373 2023-02-23 14:51:01.000000 django-oasis4-1.1.1a2/oasis/migrations/0008_location_coffeewarehouse_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3584 2023-03-01 16:44:41.000000 django-oasis4-1.1.1a2/oasis/migrations/0009_associatebalance.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    47342 2023-03-03 23:16:58.000000 django-oasis4-1.1.1a2/oasis/migrations/0010_operation.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3905 2023-03-04 03:34:51.000000 django-oasis4-1.1.1a2/oasis/migrations/0011_offer_statemachine_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      442 2023-03-04 03:50:49.000000 django-oasis4-1.1.1a2/oasis/migrations/0012_offer_price.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1782 2023-03-06 20:01:57.000000 django-oasis4-1.1.1a2/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      832 2023-03-07 08:33:48.000000 django-oasis4-1.1.1a2/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      465 2023-03-07 08:43:20.000000 django-oasis4-1.1.1a2/oasis/migrations/0015_statemachine_update_oasis.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      571 2023-03-16 14:42:57.000000 django-oasis4-1.1.1a2/oasis/migrations/0017_statemachine_state_at_timeout.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1553 2023-03-16 21:48:47.000000 django-oasis4-1.1.1a2/oasis/migrations/0018_offermov.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/migrations/0019_stat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2022-12-10 21:43:40.000000 django-oasis4-1.1.1a2/oasis/migrations/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.719520 django-oasis4-1.1.1a2/oasis/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9352 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/models/local_models.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)   117483 2023-03-04 02:04:38.000000 django-oasis4-1.1.1a2/oasis/models/oasis_models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.720520 django-oasis4-1.1.1a2/oasis/stats/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      419 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/admin.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.720520 django-oasis4-1.1.1a2/oasis/stats/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.720520 django-oasis4-1.1.1a2/oasis/stats/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      329 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/api/serializers/stats.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.720520 django-oasis4-1.1.1a2/oasis/stats/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      327 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3684 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/api/services/stats.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      455 2023-05-19 21:49:17.000000 django-oasis4-1.1.1a2/oasis/stats/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.721520 django-oasis4-1.1.1a2/oasis/stats/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      477 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.721520 django-oasis4-1.1.1a2/oasis/stats/lib/cursors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      504 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/lib/cursors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1917 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/lib/cursors/cursor.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      586 2023-05-24 03:50:25.000000 django-oasis4-1.1.1a2/oasis/stats/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-05-24 04:03:34.722520 django-oasis4-1.1.1a2/oasis/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-23 14:54:47.000000 django-oasis4-1.1.1a2/oasis/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1206 2023-02-23 14:46:31.000000 django-oasis4-1.1.1a2/oasis/tasks/sync_coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1474 2023-01-26 02:47:20.000000 django-oasis4-1.1.1a2/oasis/tasks/sync_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-01-18 02:09:04.000000 django-oasis4-1.1.1a2/oasis/tasks/sync_document_types.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1856 2023-03-01 20:00:10.000000 django-oasis4-1.1.1a2/oasis/tasks/sync_products.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      866 2023-05-24 03:51:17.000000 django-oasis4-1.1.1a2/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-05-24 04:03:34.722520 django-oasis4-1.1.1a2/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.179715 django-oasis4-1.1.2/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-1.1.2/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-03-02 20:32:01.000000 django-oasis4-1.1.2/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13078 2023-06-26 19:39:15.179715 django-oasis4-1.1.2/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      217 2023-02-13 15:48:51.000000 django-oasis4-1.1.2/README.md
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.158715 django-oasis4-1.1.2/django_oasis4.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13078 2023-06-26 19:39:15.000000 django-oasis4-1.1.2/django_oasis4.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     4801 2023-06-26 19:39:15.000000 django-oasis4-1.1.2/django_oasis4.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-26 19:39:15.000000 django-oasis4-1.1.2/django_oasis4.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       89 2023-06-26 19:39:15.000000 django-oasis4-1.1.2/django_oasis4.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        6 2023-06-26 19:39:15.000000 django-oasis4-1.1.2/django_oasis4.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.158715 django-oasis4-1.1.2/oasis/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-10 23:55:40.000000 django-oasis4-1.1.2/oasis/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1394 2023-03-18 18:38:34.000000 django-oasis4-1.1.2/oasis/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.159715 django-oasis4-1.1.2/oasis/coffee_offers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-22 14:19:30.000000 django-oasis4-1.1.2/oasis/coffee_offers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      686 2023-03-06 19:37:38.000000 django-oasis4-1.1.2/oasis/coffee_offers/admin.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1253 2023-03-07 16:31:05.000000 django-oasis4-1.1.2/oasis/coffee_offers/admin_views.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.160715 django-oasis4-1.1.2/oasis/coffee_offers/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-23 15:03:46.000000 django-oasis4-1.1.2/oasis/coffee_offers/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.160715 django-oasis4-1.1.2/oasis/coffee_offers/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      683 2023-03-06 19:10:13.000000 django-oasis4-1.1.2/oasis/coffee_offers/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      772 2023-02-23 15:21:03.000000 django-oasis4-1.1.2/oasis/coffee_offers/api/serializers/coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1199 2023-03-06 20:11:27.000000 django-oasis4-1.1.2/oasis/coffee_offers/api/serializers/offer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.160715 django-oasis4-1.1.2/oasis/coffee_offers/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-03-01 20:03:07.000000 django-oasis4-1.1.2/oasis/coffee_offers/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11195 2023-06-13 22:51:27.000000 django-oasis4-1.1.2/oasis/coffee_offers/api/services/coffee_offers.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5245 2023-06-03 21:53:44.000000 django-oasis4-1.1.2/oasis/coffee_offers/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.161715 django-oasis4-1.1.2/oasis/coffee_offers/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-26 20:27:18.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.161715 django-oasis4-1.1.2/oasis/coffee_offers/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      659 2023-06-10 20:14:20.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1137 2023-06-02 10:37:36.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/choices/coffee_offers_states.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      825 2023-06-10 20:14:20.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/choices/oasis_choices.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.161715 django-oasis4-1.1.2/oasis/coffee_offers/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      417 2023-03-16 21:48:47.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-03-16 21:48:47.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/events/on_post_save_offer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.162715 django-oasis4-1.1.2/oasis/coffee_offers/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 21:38:01.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     8161 2023-06-26 19:09:34.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/utils/offer_state_machine.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.162715 django-oasis4-1.1.2/oasis/coffee_offers/lib/validators/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      757 2023-02-26 21:14:28.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/validators/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1336 2023-02-26 21:13:57.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/validators/date_validators.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      823 2023-02-26 20:45:48.000000 django-oasis4-1.1.2/oasis/coffee_offers/lib/validators/oasis_statuses.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.155715 django-oasis4-1.1.2/oasis/coffee_offers/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.155715 django-oasis4-1.1.2/oasis/coffee_offers/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.163715 django-oasis4-1.1.2/oasis/coffee_offers/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6053 2023-06-13 22:51:27.000000 django-oasis4-1.1.2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     8627 2023-06-13 22:51:27.000000 django-oasis4-1.1.2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.163715 django-oasis4-1.1.2/oasis/coffee_offers/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 23:14:13.000000 django-oasis4-1.1.2/oasis/coffee_offers/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1565 2023-06-24 01:48:43.000000 django-oasis4-1.1.2/oasis/coffee_offers/tasks/sync_coffe_offers.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.164715 django-oasis4-1.1.2/oasis/coffee_offers/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1072 2023-03-08 13:40:32.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/change_status.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2023-03-08 13:40:32.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/change_status.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.165715 django-oasis4-1.1.2/oasis/coffee_offers/templates/coffee_offers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      845 2023-06-04 23:24:43.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/coffee_offers/coffee_notification.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4580 2023-06-26 13:45:29.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/coffee_offers/coffee_offer.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1723 2023-06-14 20:57:54.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/coffee_offers/coffee_offers_base.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     8990 2023-06-13 22:51:27.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/coffee_offers/contract_template.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6218 2023-06-10 20:14:20.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/coffee_offers/intention_letter.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2579 2023-06-10 20:14:20.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/coffee_offers/promissory_note.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1984 2023-06-13 22:51:27.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/coffee_offers/remittance_letter.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1054 2023-03-02 20:24:29.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/save_offer.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      785 2023-03-02 20:03:04.000000 django-oasis4-1.1.2/oasis/coffee_offers/templates/save_offer.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      981 2023-03-16 14:42:57.000000 django-oasis4-1.1.2/oasis/coffee_offers/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.165715 django-oasis4-1.1.2/oasis/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-11-16 14:55:35.000000 django-oasis4-1.1.2/oasis/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.166715 django-oasis4-1.1.2/oasis/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      582 2023-01-17 21:45:20.000000 django-oasis4-1.1.2/oasis/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      783 2023-03-18 17:17:41.000000 django-oasis4-1.1.2/oasis/lib/choices/customer_type.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.169715 django-oasis4-1.1.2/oasis/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1525 2023-03-16 14:42:57.000000 django-oasis4-1.1.2/oasis/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      780 2023-02-23 14:39:16.000000 django-oasis4-1.1.2/oasis/lib/managers/local_coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      682 2023-01-28 14:38:17.000000 django-oasis4-1.1.2/oasis/lib/managers/local_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1355 2023-01-18 02:07:35.000000 django-oasis4-1.1.2/oasis/lib/managers/local_document_type.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1578 2023-03-08 14:17:45.000000 django-oasis4-1.1.2/oasis/lib/managers/local_offer.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1212 2022-12-14 20:34:45.000000 django-oasis4-1.1.2/oasis/lib/managers/local_product.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2159 2023-03-16 14:42:57.000000 django-oasis4-1.1.2/oasis/lib/managers/local_state_machine.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1201 2023-03-02 21:35:32.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_associate_balance.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2701 2023-03-01 16:42:42.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_client.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1050 2023-01-27 03:47:52.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1390 2023-02-07 10:48:09.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4007 2023-01-24 23:42:01.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_discount.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-01-24 23:42:01.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_geographic_location.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1452 2023-06-10 20:07:22.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_location.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     7648 2023-06-26 14:57:54.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_operation.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-02-06 19:28:19.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_periods.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      906 2022-12-19 16:49:04.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_product.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      730 2023-01-25 00:42:41.000000 django-oasis4-1.1.2/oasis/lib/managers/oasis_type_client.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.170715 django-oasis4-1.1.2/oasis/lib/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      658 2023-02-07 09:06:27.000000 django-oasis4-1.1.2/oasis/lib/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      789 2023-02-07 09:25:36.000000 django-oasis4-1.1.2/oasis/lib/serializers/oasis_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2022-12-14 20:01:00.000000 django-oasis4-1.1.2/oasis/lib/serializers/product.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.170715 django-oasis4-1.1.2/oasis/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      579 2023-03-03 19:38:17.000000 django-oasis4-1.1.2/oasis/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3275 2023-06-13 22:51:27.000000 django-oasis4-1.1.2/oasis/lib/utils/oasis_actions.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.156715 django-oasis4-1.1.2/oasis/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.156715 django-oasis4-1.1.2/oasis/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.170715 django-oasis4-1.1.2/oasis/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2138 2023-05-24 03:50:25.000000 django-oasis4-1.1.2/oasis/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5606 2023-05-24 03:50:25.000000 django-oasis4-1.1.2/oasis/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.174715 django-oasis4-1.1.2/oasis/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    29691 2022-12-13 18:21:01.000000 django-oasis4-1.1.2/oasis/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    31003 2023-01-17 22:22:35.000000 django-oasis4-1.1.2/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    17130 2023-01-26 02:36:44.000000 django-oasis4-1.1.2/oasis/migrations/0003_oasiscompany_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5814 2023-01-27 03:47:55.000000 django-oasis4-1.1.2/oasis/migrations/0004_account_vaccountingbalanceclient.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      515 2023-02-02 01:56:29.000000 django-oasis4-1.1.2/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1582 2023-02-05 00:32:58.000000 django-oasis4-1.1.2/oasis/migrations/0006_periods.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      949 2023-02-07 02:05:07.000000 django-oasis4-1.1.2/oasis/migrations/0007_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9373 2023-02-23 14:51:01.000000 django-oasis4-1.1.2/oasis/migrations/0008_location_coffeewarehouse_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3584 2023-03-01 16:44:41.000000 django-oasis4-1.1.2/oasis/migrations/0009_associatebalance.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    47342 2023-03-03 23:16:58.000000 django-oasis4-1.1.2/oasis/migrations/0010_operation.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3905 2023-03-04 03:34:51.000000 django-oasis4-1.1.2/oasis/migrations/0011_offer_statemachine_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      442 2023-03-04 03:50:49.000000 django-oasis4-1.1.2/oasis/migrations/0012_offer_price.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1782 2023-03-06 20:01:57.000000 django-oasis4-1.1.2/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      832 2023-03-07 08:33:48.000000 django-oasis4-1.1.2/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      465 2023-03-07 08:43:20.000000 django-oasis4-1.1.2/oasis/migrations/0015_statemachine_update_oasis.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-03-16 14:42:57.000000 django-oasis4-1.1.2/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      571 2023-03-16 14:42:57.000000 django-oasis4-1.1.2/oasis/migrations/0017_statemachine_state_at_timeout.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1553 2023-03-16 21:48:47.000000 django-oasis4-1.1.2/oasis/migrations/0018_offermov.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/migrations/0019_stat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      413 2023-06-10 19:30:28.000000 django-oasis4-1.1.2/oasis/migrations/0020_coffeewarehouse_city_name.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      641 2023-06-26 13:05:00.000000 django-oasis4-1.1.2/oasis/migrations/0021_offer_confirmed_at_offer_confirmed_by.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2022-12-10 21:43:40.000000 django-oasis4-1.1.2/oasis/migrations/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.175715 django-oasis4-1.1.2/oasis/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9660 2023-06-24 01:16:19.000000 django-oasis4-1.1.2/oasis/models/local_models.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)   117487 2023-06-26 16:21:43.000000 django-oasis4-1.1.2/oasis/models/oasis_models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.176715 django-oasis4-1.1.2/oasis/stats/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/stats/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      419 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/stats/admin.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.176715 django-oasis4-1.1.2/oasis/stats/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/stats/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.176715 django-oasis4-1.1.2/oasis/stats/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      329 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/stats/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/stats/api/serializers/stats.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.177715 django-oasis4-1.1.2/oasis/stats/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      327 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/stats/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3684 2023-05-24 03:50:25.000000 django-oasis4-1.1.2/oasis/stats/api/services/stats.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      455 2023-05-19 21:49:17.000000 django-oasis4-1.1.2/oasis/stats/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.177715 django-oasis4-1.1.2/oasis/stats/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      477 2023-05-24 03:50:25.000000 django-oasis4-1.1.2/oasis/stats/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.177715 django-oasis4-1.1.2/oasis/stats/lib/cursors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      504 2023-05-24 03:50:25.000000 django-oasis4-1.1.2/oasis/stats/lib/cursors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1917 2023-05-24 03:50:25.000000 django-oasis4-1.1.2/oasis/stats/lib/cursors/cursor.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      586 2023-05-24 03:50:25.000000 django-oasis4-1.1.2/oasis/stats/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:39:15.178715 django-oasis4-1.1.2/oasis/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-23 14:54:47.000000 django-oasis4-1.1.2/oasis/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1278 2023-06-10 20:10:04.000000 django-oasis4-1.1.2/oasis/tasks/sync_coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1474 2023-01-26 02:47:20.000000 django-oasis4-1.1.2/oasis/tasks/sync_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-01-18 02:09:04.000000 django-oasis4-1.1.2/oasis/tasks/sync_document_types.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1856 2023-03-01 20:00:10.000000 django-oasis4-1.1.2/oasis/tasks/sync_products.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      876 2023-06-26 19:35:57.000000 django-oasis4-1.1.2/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-26 19:39:15.179715 django-oasis4-1.1.2/setup.cfg
```

### Comparing `django-oasis4-1.1.1a2/LICENSE` & `django-oasis4-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/PKG-INFO` & `django-oasis4-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4
-Version: 1.1.1a2
+Version: 1.1.2
 Summary: OASIS4 Data Interfaces
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-1.1.1a2/django_oasis4.egg-info/PKG-INFO` & `django-oasis4-1.1.2/django_oasis4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4
-Version: 1.1.1a2
+Version: 1.1.2
 Summary: OASIS4 Data Interfaces
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-1.1.1a2/django_oasis4.egg-info/SOURCES.txt` & `django-oasis4-1.1.2/django_oasis4.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 oasis/coffee_offers/api/serializers/coffee_ware_house.py
 oasis/coffee_offers/api/serializers/offer.py
 oasis/coffee_offers/api/services/__init__.py
 oasis/coffee_offers/api/services/coffee_offers.py
 oasis/coffee_offers/lib/__init__.py
 oasis/coffee_offers/lib/choices/__init__.py
 oasis/coffee_offers/lib/choices/coffee_offers_states.py
-oasis/coffee_offers/lib/choices/oasis_states.py
+oasis/coffee_offers/lib/choices/oasis_choices.py
 oasis/coffee_offers/lib/events/__init__.py
 oasis/coffee_offers/lib/events/on_post_save_offer.py
 oasis/coffee_offers/lib/utils/__init__.py
 oasis/coffee_offers/lib/utils/offer_state_machine.py
 oasis/coffee_offers/lib/validators/__init__.py
 oasis/coffee_offers/lib/validators/date_validators.py
 oasis/coffee_offers/lib/validators/oasis_statuses.py
@@ -35,17 +35,21 @@
 oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
 oasis/coffee_offers/tasks/__init__.py
 oasis/coffee_offers/tasks/sync_coffe_offers.py
 oasis/coffee_offers/templates/change_status.html
 oasis/coffee_offers/templates/change_status.txt
 oasis/coffee_offers/templates/save_offer.html
 oasis/coffee_offers/templates/save_offer.txt
+oasis/coffee_offers/templates/coffee_offers/coffee_notification.html
+oasis/coffee_offers/templates/coffee_offers/coffee_offer.html
+oasis/coffee_offers/templates/coffee_offers/coffee_offers_base.html
 oasis/coffee_offers/templates/coffee_offers/contract_template.html
-oasis/coffee_offers/templates/coffee_offers/promisory_note.html
-oasis/coffee_offers/templates/coffee_offers/terms_conditions.html
+oasis/coffee_offers/templates/coffee_offers/intention_letter.html
+oasis/coffee_offers/templates/coffee_offers/promissory_note.html
+oasis/coffee_offers/templates/coffee_offers/remittance_letter.html
 oasis/lib/__init__.py
 oasis/lib/choices/__init__.py
 oasis/lib/choices/customer_type.py
 oasis/lib/managers/__init__.py
 oasis/lib/managers/local_coffee_ware_house.py
 oasis/lib/managers/local_company.py
 oasis/lib/managers/local_document_type.py
@@ -85,14 +89,16 @@
 oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
 oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
 oasis/migrations/0015_statemachine_update_oasis.py
 oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
 oasis/migrations/0017_statemachine_state_at_timeout.py
 oasis/migrations/0018_offermov.py
 oasis/migrations/0019_stat.py
+oasis/migrations/0020_coffeewarehouse_city_name.py
+oasis/migrations/0021_offer_confirmed_at_offer_confirmed_by.py
 oasis/migrations/__init__.py
 oasis/models/__init__.py
 oasis/models/local_models.py
 oasis/models/oasis_models.py
 oasis/stats/__init__.py
 oasis/stats/admin.py
 oasis/stats/apps.py
```

### Comparing `django-oasis4-1.1.1a2/oasis/apps.py` & `django-oasis4-1.1.2/oasis/apps.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/admin.py` & `django-oasis4-1.1.2/oasis/coffee_offers/admin.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/admin_views.py` & `django-oasis4-1.1.2/oasis/coffee_offers/admin_views.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/__init__.py` & `django-oasis4-1.1.2/oasis/coffee_offers/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/coffee_ware_house.py` & `django-oasis4-1.1.2/oasis/coffee_offers/api/serializers/coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/serializers/offer.py` & `django-oasis4-1.1.2/oasis/coffee_offers/api/serializers/offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/__init__.py` & `django-oasis4-1.1.2/oasis/coffee_offers/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/api/services/coffee_offers.py` & `django-oasis4-1.1.2/oasis/coffee_offers/api/services/coffee_offers.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         Rest service for preload all data required for frontend operation.
         :param request: request object from HTTP
         :return: Response object
         """
         try:
             now = timezone.now()
             to_date = now + timedelta(days=settings.COFFEE_OFFERS_DAYS_DELTA)
-            product_list =[int(x) for x in settings.COFFEE_OFFERS_PRODUCT_LIST.split(",")]
+            product_list = [int(x) for x in settings.COFFEE_OFFERS_PRODUCT_LIST.split(",")]
             user = self._get_user(request)
             # Validate EXCLUDED
             if settings.COFFEE_OFFERS_LOCKED_SEGMENT != 0 and user.profile.segment == settings.COFFEE_OFFERS_LOCKED_SEGMENT:
                 raise ValidationError(_("The partner/client is locked for coffee offers."))
             # Load Price List
             price_qs = Price.objects.get_products_price_by_date(date_to_search=now, product_list=product_list)
             price_serializer = PriceListSerializer(instance=price_qs, many=True,
@@ -181,14 +181,15 @@
                 data_cache = code_generator.generate_dict()
                 cache_key = data_cache.pop("uuid").hex
                 data_cache["user"] = user
                 data_cache["data"] = {
                     "offer_id": request.data.get("offer_id"),
                     "status": request.data.get("status")
                 }
+
                 data_return = {
                     "token": cache_key
                 }
                 email_context = {
                     "customer_name": user.get_full_name(),
                     "customer_code": data_cache.get("code")
                 }
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/apps.py` & `django-oasis4-1.1.2/oasis/coffee_offers/apps.py`

 * *Files 15% similar despite different names*

```diff
@@ -59,17 +59,32 @@
         settings.COFFEE_OFFERS_LOAD_ALL = getattr(settings, "COFFEE_OFFERS_LOAD_ALL", False)
         # Round factor
         settings.COFFEE_OFFERS_ROUND_FACTOR = getattr(settings, "COFFEE_OFFERS_ROUND_FACTOR", 10)
         # Contract Template
         settings.COFFEE_OFFERS_CONTRACT_TEMPLATE = getattr(settings, "COFFEE_OFFERS_CONTRACT_TEMPLATE",
                                                            "contract_template.html")
         # Terms and conditions template
-        settings.COFFEE_OFFERS_TERMS_TEMPLATE = getattr(settings, "COFFEE_OFFERS_TERMS_TEMPLATE",
-                                                        "terms_conditions.html")
+        settings.COFFEE_OFFERS_OFFER_TEMPLATE = getattr(settings, "COFFEE_OFFERS_OFFER_TEMPLATE",
+                                                        "coffee_offer.html")
         # Promissory note
         settings.COFFEE_OFFERS_PROMISE_TEMPLATE = getattr(settings, "COFFEE_OFFERS_PROMISE_TEMPLATE",
-                                                          "promisory_note.html")
+                                                          "promissory_note.html")
+        # Intention Letter
+        settings.COFFEE_OFFERS_INTENTION_LETTER_TEMPLATE = getattr(settings, "COFFEE_OFFERS_INTENTION_LETTER_TEMPLATE",
+                                                                   "intention_letter.html")
+        # Remittance Letter
+        settings.COFFEE_OFFERS_REMITTANCE_EMAIL_TEMPLATE = getattr(settings,
+                                                                   "COFFEE_OFFERS_REMITTANCE_EMAIL_TEMPLATE",
+                                                                   "coffee_offers/remittance_letter.html")
+        # Notification template
+        settings.COFFEE_OFFERS_NOTIFICATION_EMAIL_TEMPLATE = getattr(settings,
+                                                                     "COFFEE_OFFERS_NOTIFICATION_EMAIL_TEMPLATE",
+                                                                     "coffee_offers/coffee_notification.html")
+        # Notifications EMails
+        settings.COFFEE_OFFERS_LEGAL_AREA_EMAIL = getattr(settings, "COFFEE_OFFERS_LEGAL_AREA_EMAIL", None)
+        settings.COFFEE_OFFERS_COFFEE_AREA_EMAIL = getattr(settings, "COFFEE_OFFERS_COFFEE_AREA_EMAIL", None)
+
         # Coffee factor for offers
         settings.COFFEE_OFFERS_FACTOR = getattr(settings, "COFFEE_OFFERS_FACTOR", 94)
         # Coffee Offers product list
         settings.COFFEE_OFFERS_PRODUCT_LIST = getattr(settings, "COFFEE_OFFERS_PRODUCT_LIST",
                                                       "2101,2102,2104,2106,2107,2109,2112,2113,2114,2126,2120,2134")
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/__init__.py` & `django-oasis4-1.1.2/oasis/coffee_offers/lib/choices/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 # Developed by: macercha
 # Date:         26/02/23 15:26
 # Project:      CFHL Transactional Backend
 # Module Name:  __init__.py
 # Description:
 # ****************************************************************
 from .coffee_offers_states import CoffeeOffersStates
-from .oasis_states import OasisStates
+from .oasis_choices import OasisChoices
 
 __all__ = [
     "CoffeeOffersStates",
-    "OasisStates"
+    "OasisChoices"
 ]
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/coffee_offers_states.py` & `django-oasis4-1.1.2/oasis/coffee_offers/lib/choices/coffee_offers_states.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/choices/oasis_states.py` & `django-oasis4-1.1.2/oasis/coffee_offers/tasks/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,20 +2,17 @@
 
 #  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
 #  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         26/02/23 15:31
+# Date:         6/03/23 15:44
 # Project:      CFHL Transactional Backend
-# Module Name:  oasis_states
+# Module Name:  __init__.py
 # Description:
 # ****************************************************************
-from django.utils.translation import gettext_lazy as _
-from zibanu.django.db import models
+from .sync_coffe_offers import sync_coffee_offers
 
-
-class OasisStates(models.TextChoices):
-    ACTIVE = "A", _("Active")
-    PROCESSED = "P", _("Processed")
-    CANCELED = "X", _("Canceled")
+__all__ = [
+    "sync_coffee_offers"
+]
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/events/on_post_save_offer.py` & `django-oasis4-1.1.2/oasis/coffee_offers/lib/events/on_post_save_offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/utils/__init__.py` & `django-oasis4-1.1.2/oasis/coffee_offers/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/__init__.py` & `django-oasis4-1.1.2/oasis/coffee_offers/lib/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/date_validators.py` & `django-oasis4-1.1.2/oasis/coffee_offers/lib/validators/date_validators.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/lib/validators/oasis_statuses.py` & `django-oasis4-1.1.2/oasis/coffee_offers/lib/validators/oasis_statuses.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po` & `django-oasis4-1.1.2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po`

 * *Files 23% similar despite different names*

```diff
@@ -4,53 +4,54 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-03-08 16:44-0500\n"
+"POT-Creation-Date: 2023-06-10 13:29-0500\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
 #: admin_views.py:22
 msgid "Status Section"
 msgstr "Sección de Estado"
 
 #: admin_views.py:30
 msgid "Notifications Section"
 msgstr "Sección de Notificaciones"
 
-#: api/services/coffee_offers.py:90 api/services/coffee_offers.py:135
+#: api/services/coffee_offers.py:91 api/services/coffee_offers.py:137
 msgid "The partner/client is locked for coffee offers."
 msgstr "El socio/cliente está bloqueado para realizar ofertas de café."
 
-#: api/services/coffee_offers.py:133
+#: api/services/coffee_offers.py:135
 msgid "The amount exceeds the quota available."
 msgstr "La cantidad excede el cupo asignado."
 
-#: api/services/coffee_offers.py:138
+#: api/services/coffee_offers.py:140
 #, python-format
 msgid "Delivery date is greater than %s days"
 msgstr "Fecha de envío es superior a %s días"
 
-#: api/services/coffee_offers.py:140
+#: api/services/coffee_offers.py:142
 msgid "You have reached max active offers quota."
 msgstr "Ud ha alcanzado el máximo número de ofertas activas posibles"
 
-#: api/services/coffee_offers.py:220
+#: api/services/coffee_offers.py:224
 msgid "Code or user does not match."
 msgstr "Código o usuario no coinciden"
 
-#: api/services/coffee_offers.py:222
+#: api/services/coffee_offers.py:226
 msgid "The code has expired. You have to create the offer again."
 msgstr "El código ha expirado. Debe crear la oferta nuevamente."
 
 #: apps.py:23
 msgid "Oasis4 Coffee Offer "
 msgstr "Ofertas de Café OASIS4"
 
@@ -66,35 +67,71 @@
 msgid "Signed"
 msgstr "Firmado"
 
 #: lib/choices/coffee_offers_states.py:22
 msgid "Partial"
 msgstr "Parcial"
 
-#: lib/choices/coffee_offers_states.py:23
+#: lib/choices/coffee_offers_states.py:23 lib/choices/oasis_choices.py:19
 msgid "Finished"
 msgstr "Finalizado"
 
 #: lib/choices/coffee_offers_states.py:24
 msgid "Rejected"
 msgstr "Rechazado"
 
-#: lib/choices/oasis_states.py:19
+#: lib/choices/oasis_choices.py:18
 msgid "Active"
 msgstr "Activa"
 
-#: lib/choices/oasis_states.py:20
+#: lib/choices/oasis_choices.py:18
 msgid "Processed"
 msgstr "Procesada"
 
-#: lib/choices/oasis_states.py:21
+#: lib/choices/oasis_choices.py:18 lib/choices/oasis_choices.py:19
 msgid "Canceled"
 msgstr "Cancelada"
 
+#: lib/choices/oasis_choices.py:19
+msgid "Pending"
+msgstr "Pendiente"
+
+#: lib/choices/oasis_choices.py:19
+msgid "Dispatched"
+msgstr "Despachada"
+
+#: lib/choices/oasis_choices.py:19
+msgid "For sign"
+msgstr "Para Firma"
+
+#: lib/utils/offer_state_machine.py:40
+msgid "User associated to offer does not exists."
+msgstr "El usuario asociado a la oferta no existe."
+
 #: lib/utils/offer_state_machine.py:57
+msgid "Coffee Offer"
+msgstr "Oferta de Café"
+
+#: lib/utils/offer_state_machine.py:58
+msgid "Coffee Offer Contract"
+msgstr "Contrato de Oferta de Café"
+
+#: lib/utils/offer_state_machine.py:59
+msgid "Promise"
+msgstr "Pagaré"
+
+#: lib/utils/offer_state_machine.py:60
+msgid "Intention Letter"
+msgstr "Carta de Instrucciones"
+
+#: lib/utils/offer_state_machine.py:103
+msgid "Coffee Offer Notification"
+msgstr ""
+
+#: lib/utils/offer_state_machine.py:155
 msgid "Error updating operation record"
 msgstr "Error actualizando el registro en oasis4"
 
 #: lib/validators/date_validators.py:25
 msgid "Received date is less than current date"
 msgstr "Fecha recibida es menor que la fecha actual"
 
@@ -103,27 +140,29 @@
 msgstr "La fecha recibida es menor o igual que la fecha actual"
 
 #: lib/validators/oasis_statuses.py:21
 msgid "Invalid Coffe Order - Oasis Status"
 msgstr "Orde de café inválida - Estado OASIS"
 
 #: templates/change_status.html:9 templates/change_status.txt:2
+#: templates/coffee_offers/coffee_notification.html:9
 #: templates/save_offer.html:9 templates/save_offer.txt:2
 msgid "Hello"
 msgstr "Hola"
 
 #: templates/change_status.html:10
 msgid ""
 "Thank you for use the <strong>CADEFIHUILA's</strong> transactional portal. "
 "To confirm that you are accepting the changes in the offer of coffee sale "
 "and sign it, please write the below code at the form of web page."
 msgstr ""
-"Gracias por utilizar el portal transaccional de <strong>CADEFIHUILA's</strong>, "
-"Para confirmar que usted ha aceptado los cambios en la oferta de venta de café "
-"y firmarla, por favor ingrese en la página web el código que encuentra abajo."
+"Gracias por utilizar el portal transaccional de <strong>CADEFIHUILA's</"
+"strong>, Para confirmar que usted ha aceptado los cambios en la oferta de "
+"venta de café y firmarla, por favor ingrese en la página web el código que "
+"encuentra abajo."
 
 #: templates/change_status.html:14 templates/change_status.txt:8
 #: templates/save_offer.html:14 templates/save_offer.txt:8
 #, python-format
 msgid "The code is valid for %(code_timeout)s minutes."
 msgstr "El codigo es valido por %(code_timeout)s minutos."
 
@@ -151,29 +190,69 @@
 #: templates/change_status.txt:4
 msgid ""
 "Thank you for use the CADEFIHUILA's transactional portal. To confirm that "
 "you are accepting the changes in the offer of coffee sale and sign it, "
 "please write the below code at the form of web page."
 msgstr ""
 "Gracias por usar el portal transacciona del CADEFIHUILA. Para confirmar que "
-"usted ha aceptado los cambios de la oferta de venta de cafe y firmarlo, "
-"por favor ingrese en la página web el código que encuentra abajo."
+"usted ha aceptado los cambios de la oferta de venta de cafe y firmarlo, por "
+"favor ingrese en la página web el código que encuentra abajo."
+
+#: templates/coffee_offers/coffee_notification.html:10
+msgid ""
+"Thank you for use the <strong>CADEFIHUILA's</strong> transactional portal."
+msgstr ""
+"Gracias por utilizar el portal transaccional de <strong>CADEFIHUILA</strong>."
+
+#: templates/coffee_offers/coffee_notification.html:11
+msgid "Through this email inform you that your Coffee Offer No. "
+msgstr ""
+"A través de este correo electrónico le informamos que su Oferta de Café No."
+
+#: templates/coffee_offers/coffee_notification.html:11
+#, python-format
+msgid ""
+"has changed from status <strong>%(from_status)s</strong> to <strong>"
+"%(new_status)s</strong> status."
+msgstr ""
+"ha cambiado del estado <strong>%(from_status)s</strong> a <strong>"
+"%(new_status)s</strong> estado."
+
+#: templates/coffee_offers/coffee_notification.html:15
+msgid ""
+"This email waw generated automatically at %(email_datetime)s with id "
+"%(email_id)s. Pleas do not answer it."
+msgstr ""
+"Este correo fue generado automáticamente el %(email_datetime)s con el id "
+"%(email_id)s. Por favor no lo responda."
+
+#: templates/coffee_offers/remittance_letter.html:36
+msgid ""
+"This email waw generated automatically at %(email_datetime)s with id "
+"%(email_id)s. Pleas\n"
+"            do not answer it.\n"
+"        "
+msgstr ""
+"Este correo fue generado automáticamente el %(email_datetime)s con el id "
+"%(email_id)s. Por favor\n"
+"            no lo responda.\n"
+"        "
 
 #: templates/save_offer.html:10
 msgid ""
 "Thank you for use the <strong>CADEFIHUILA's</strong> transactional portal. "
 "To confirm that you´re sending an offer of coffee sale and sign it, please "
 "write the below code at the form of web page."
 msgstr ""
-"Gracias por utilizar el portal transaccional de <strong>CADEFIHUILA</strong>. "
-"Para confirmar el envío de la oferta de venta de café y firmarla, por favor "
-"ingrese en la página web el código que encuentra abajo."
+"Gracias por utilizar el portal transaccional de <strong>CADEFIHUILA</"
+"strong>. Para confirmar el envío de la oferta de venta de café y firmarla, "
+"por favor ingrese en la página web el código que encuentra abajo."
 
 #: templates/save_offer.txt:4
 msgid ""
 "Thank you for use the CADEFIHUILA's transactional portal. To confirm that you"
 "´re sending an offer of coffee sale and sign it, please write the below code "
 "at the form of web page."
 msgstr ""
-"Gracias por utilizar el portal transaccional de CADEFIHUILA. Para confirmar que "
-"el envío de la oferta de venta de café y firmarla, por favor ingrese en la "
-"página web el codigo que encuentra abajo."
+"Gracias por utilizar el portal transaccional de CADEFIHUILA. Para confirmar "
+"que el envío de la oferta de venta de café y firmarla, por favor ingrese en "
+"la página web el codigo que encuentra abajo."
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/__init__.py` & `django-oasis4-1.1.2/oasis/lib/choices/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 
-#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
-#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
+#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2022. All rights reserved.
+#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2022. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         6/03/23 15:44
+# Date:         20/12/22 6:35 AM
 # Project:      CFHL Transactional Backend
 # Module Name:  __init__.py
 # Description:
 # ****************************************************************
-from .sync_coffe_offers import sync_coffee_offers
+from .customer_type import CustomerType
 
 __all__ = [
-    "sync_coffee_offers"
+    "CustomerType"
 ]
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/tasks/sync_coffe_offers.py` & `django-oasis4-1.1.2/oasis/coffee_offers/tasks/sync_coffe_offers.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # IDE:          PyCharm
 # Developed by: macercha
 # Date:         6/03/23 16:34
 # Project:      CFHL Transactional Backend
 # Module Name:  sync_coffe_offers
 # Description:
 # ****************************************************************
+import logging
 from core import celery_app
 from django.conf import settings
 from oasis.coffee_offers.lib.utils import OfferStateMachine
 from oasis.models import Offer
 from oasis.models import Operation
 from typing import Any
 
@@ -24,11 +25,17 @@
     document_id = settings.COFFEE_OFFERS_DOCUMENT
 
     offer_qs = Offer.objects.get_all_active_offers()
     for offer in offer_qs:
         operation = Operation.objects.get_by_operation_pk(document_id=document_id,
                                                           location_id=offer.warehouse.location_id,
                                                           number_id=offer.contract).first()
+
         if operation is not None:
-            state_machine = OfferStateMachine(offer, operation)
-            state_machine.run()
-            state_machine.validate_timeout()
+            try:
+                state_machine = OfferStateMachine(offer, operation)
+                state_machine.run()
+                state_machine.validate_timeout()
+            except ValueError as exc:
+                logging.debug(str(exc))
+            except Exception as exc:
+                logging.debug(str(exc))
```

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/templates/change_status.html` & `django-oasis4-1.1.2/oasis/coffee_offers/templates/change_status.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/templates/change_status.txt` & `django-oasis4-1.1.2/oasis/coffee_offers/templates/change_status.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/templates/save_offer.html` & `django-oasis4-1.1.2/oasis/coffee_offers/templates/save_offer.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/templates/save_offer.txt` & `django-oasis4-1.1.2/oasis/coffee_offers/templates/save_offer.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/coffee_offers/urls.py` & `django-oasis4-1.1.2/oasis/coffee_offers/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/choices/customer_type.py` & `django-oasis4-1.1.2/oasis/lib/choices/customer_type.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/__init__.py` & `django-oasis4-1.1.2/oasis/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_coffee_ware_house.py` & `django-oasis4-1.1.2/oasis/lib/managers/local_coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_company.py` & `django-oasis4-1.1.2/oasis/lib/managers/local_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_document_type.py` & `django-oasis4-1.1.2/oasis/lib/managers/local_document_type.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_offer.py` & `django-oasis4-1.1.2/oasis/lib/managers/local_offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_product.py` & `django-oasis4-1.1.2/oasis/lib/managers/local_product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/local_state_machine.py` & `django-oasis4-1.1.2/oasis/lib/managers/local_state_machine.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_associate_balance.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_associate_balance.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_client.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_client.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_company.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_cycle.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_discount.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_discount.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_geographic_location.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_geographic_location.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_location.py` & `django-oasis4-1.1.2/oasis/lib/serializers/oasis_cycle.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 #  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
 #  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         23/02/23 9:16
+# Date:         7/02/23 3:56
 # Project:      CFHL Transactional Backend
-# Module Name:  oasis_location
+# Module Name:  oasis_cycle
 # Description:
 # ****************************************************************
-from zibanu.django.db import models
+from oasis.models import Cycle
+from zibanu.django.rest_framework import serializers
 
 
-class OasisLocation(models.Manager):
+class CycleSerializer(serializers.ModelSerializer):
     """
-    Manager class of Location class entity
+    Cycle serializer for obtain availables cycles by type
     """
-    def get_coffe_ware_houses(self):
-        qs = self.get_queryset().filter(businessid__exact=1, level__exact=2, pointofsales__exact=1)
-        return qs
-
 
+    class Meta:
+        model = Cycle
+        fields = ("year", "cycle")
```

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_operation.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,36 @@
 
     def __get_cursor(self):
         return connections[self.connection_name].cursor()
 
     def __get_connection(self):
         return connections[self.connection_name]
 
-    def get_by_operation_pk(self, document_id: str, location_id: int, number_id: int) -> models.QuerySet:
+    def get_by_operation_pk(self, document_id: str, location_id: int, number_id: int) -> dict:
         """
         Return an operation with oasis pk filter
         :param document_id: Document id
         :param location_id: Location id
         :param number_id: Document number id
         :return: Queryset
         """
-        return self.filter(companyid__exact=settings.OASIS_DEFAULT_COMPANY, locationid__exact=location_id,
-                           numberid__exact=number_id, documentid__startswith=document_id)
+        # Se cambia el filtro aplicado al modelo para que se ejecute mediante un annotate, incluyendo un subquery.
+        # By Macercha - 2023/06/26
+        qs = self.filter(
+            companyid__exact=settings.OASIS_DEFAULT_COMPANY,
+            locationid__exact=location_id,
+            numberid__exact=number_id,
+            documentid__startswith=document_id
+        ).annotate(
+            confirmed_by=models.Subquery(
+                oasis_models.Client.objects.filter(clientid__exact=models.OuterRef("confirmby")).values("clientname")[:1]
+            )
+        ).values("state", "status", "quantity", "otherif", "finaldate", "numberid", "confirmby", "confirmdate",
+                 "confirmed_by")
+        return qs
 
     def operation_insert(self, user: Any, product_id: int, location_id: int, amount: float, price: float, to_date: str):
         """
         Method to insert an operation record in OASIS4
         :param user:
         :param product_id:
         :param location_id:
@@ -158,8 +170,7 @@
             "company_id": company_id,
             "location_id": location_id,
             "number_id": number_id,
             "document_id": document_id
         })
 
         return cursor.rowcount == 1
-
```

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_periods.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_periods.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_product.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/managers/oasis_type_client.py` & `django-oasis4-1.1.2/oasis/lib/managers/oasis_type_client.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/serializers/__init__.py` & `django-oasis4-1.1.2/oasis/lib/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/serializers/oasis_cycle.py` & `django-oasis4-1.1.2/oasis/lib/serializers/product.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 
-#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2023. All rights reserved.
-#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2023. Todos los derechos reservado
+#  Developed by CQ Inversiones SAS. Copyright ©. 2019 - 2022. All rights reserved.
+#  Desarrollado por CQ Inversiones SAS. Copyright ©. 2019 - 2022. Todos los derechos reservado
 
 # ****************************************************************
 # IDE:          PyCharm
 # Developed by: macercha
-# Date:         7/02/23 3:56
+# Date:         14/12/22 2:55 PM
 # Project:      CFHL Transactional Backend
-# Module Name:  oasis_cycle
+# Module Name:  product
 # Description:
 # ****************************************************************
-from oasis.models import Cycle
+from oasis import models
 from zibanu.django.rest_framework import serializers
 
 
-class CycleSerializer(serializers.ModelSerializer):
+class ProductListSerializer(serializers.ModelSerializer):
     """
-    Cycle serializer for obtain availables cycles by type
+    Serializer class for list of products for frontend choices.
     """
 
     class Meta:
-        model = Cycle
-        fields = ("year", "cycle")
+        model = models.Product
+        fields = ("id", "name")
+
```

### Comparing `django-oasis4-1.1.1a2/oasis/lib/utils/__init__.py` & `django-oasis4-1.1.2/oasis/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/lib/utils/oasis_actions.py` & `django-oasis4-1.1.2/oasis/lib/utils/oasis_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,14 +67,15 @@
                 offer = Offer.objects.get_by_pk(pk=offer_id).get()
                 operation = Operation.objects.get_by_operation_pk(document_id=document_id,
                                                                   location_id=offer.warehouse.location_id,
                                                                   number_id=offer.contract).first()
                 if operation is not None:
                     state_machine = OfferStateMachine(offer=offer, operation=operation)
                     state_machine.set(new_state=new_state)
+
                 else:
                     raise Operation.DoesNotExist(_("Operation record does not exist!"))
             else:
                 raise ValidationError(_("Error changing state. Required data not found."))
         except Exception as exc:
             raise
         else:
```

### Comparing `django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-1.1.2/oasis/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/locale/es/LC_MESSAGES/django.po` & `django-oasis4-1.1.2/oasis/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0001_initial.py` & `django-oasis4-1.1.2/oasis/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py` & `django-oasis4-1.1.2/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0003_oasiscompany_company.py` & `django-oasis4-1.1.2/oasis/migrations/0003_oasiscompany_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0004_account_vaccountingbalanceclient.py` & `django-oasis4-1.1.2/oasis/migrations/0004_account_vaccountingbalanceclient.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py` & `django-oasis4-1.1.2/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0006_periods.py` & `django-oasis4-1.1.2/oasis/migrations/0006_periods.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0007_cycle.py` & `django-oasis4-1.1.2/oasis/migrations/0007_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0008_location_coffeewarehouse_and_more.py` & `django-oasis4-1.1.2/oasis/migrations/0008_location_coffeewarehouse_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0009_associatebalance.py` & `django-oasis4-1.1.2/oasis/migrations/0009_associatebalance.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0010_operation.py` & `django-oasis4-1.1.2/oasis/migrations/0010_operation.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0011_offer_statemachine_and_more.py` & `django-oasis4-1.1.2/oasis/migrations/0011_offer_statemachine_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py` & `django-oasis4-1.1.2/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py` & `django-oasis4-1.1.2/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py` & `django-oasis4-1.1.2/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0017_statemachine_state_at_timeout.py` & `django-oasis4-1.1.2/oasis/migrations/0017_statemachine_state_at_timeout.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0018_offermov.py` & `django-oasis4-1.1.2/oasis/migrations/0018_offermov.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/migrations/0019_stat.py` & `django-oasis4-1.1.2/oasis/migrations/0019_stat.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/models/__init__.py` & `django-oasis4-1.1.2/oasis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/models/local_models.py` & `django-oasis4-1.1.2/oasis/models/local_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 
 class CoffeeWareHouse(models.Model):
     """
     Model class to represent CoffeeWareHouse entity
     """
     location_id = models.IntegerField(null=False, blank=False, verbose_name=_("Location ID"))
     location_name = models.CharField(max_length=150, blank=False, null=False, verbose_name=_("Location Name"))
+    city_name = models.CharField(max_length=150, blank=False, null=True, verbose_name=_("City"))
     # Default Manager
     objects = managers.CoffeeWareHouse()
 
     class Meta:
         constraints = [
             models.UniqueConstraint(fields=("location_id",), name="UNQ_coffee_ware_house_location_id")
         ]
@@ -139,14 +140,16 @@
                                       verbose_name=_("Kg Received"))
     price = models.DecimalField(max_digits=7, decimal_places=2, blank=False, null=False, default=0,
                                 verbose_name=_("Price"))
     status = models.IntegerField(choices=CoffeeOffersStates.choices, default=CoffeeOffersStates.NEW, null=False,
                                  blank=False, verbose_name=_("Status"))
     delivery_date = models.DateField(blank=False, null=False, verbose_name=_("Delivery Date"),
                                      validators=[greater_than_today])
+    confirmed_at = models.DateField(blank=True, null=True, verbose_name=_("Confirmed at"))
+    confirmed_by = models.CharField(max_length=150, blank=True, null=False, default="", verbose_name=_("Confirmed by"))
     # Set default Manager
     objects = managers.Offer()
 
     @property
     def is_active(self) -> bool:
         return self.status in [CoffeeOffersStates.NEW, CoffeeOffersStates.SIGNED, CoffeeOffersStates.PARTIAL]
```

### Comparing `django-oasis4-1.1.1a2/oasis/models/oasis_models.py` & `django-oasis4-1.1.2/oasis/models/oasis_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1362,15 +1362,15 @@
     cashid = models.IntegerField(blank=True, null=True)
     warehouseid = models.IntegerField(blank=True, null=True)
     invstate = models.BooleanField(blank=True, null=True)
     inventory = models.BooleanField(blank=True, null=True)
     destinylocationid = models.IntegerField(blank=True, null=True)
     box = models.IntegerField(blank=True, null=True)
     formpaymentid = models.IntegerField(blank=True, null=True)
-    confirmdate = models.DateField(blank=True, null=True)
+    confirmdate = models.DateTimeField(blank=True, null=True)
     confirmhour = models.DateField(blank=True, null=True)
     printdate = models.DateField(blank=True, null=True)
     printhour = models.DateField(blank=True, null=True)
     prefix = models.CharField(max_length=10, blank=True, null=True)
     currencyid = models.IntegerField(blank=True, null=True)
     exchangerate = models.DecimalField(max_digits=19, decimal_places=4, blank=True, null=True)
     saledate = models.DateField(blank=True, null=True)
```

### Comparing `django-oasis4-1.1.1a2/oasis/stats/api/services/stats.py` & `django-oasis4-1.1.2/oasis/stats/api/services/stats.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/stats/lib/cursors/cursor.py` & `django-oasis4-1.1.2/oasis/stats/lib/cursors/cursor.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/stats/urls.py` & `django-oasis4-1.1.2/oasis/stats/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/__init__.py` & `django-oasis4-1.1.2/oasis/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/sync_coffee_ware_house.py` & `django-oasis4-1.1.2/oasis/tasks/sync_coffee_ware_house.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,16 +22,17 @@
     Background task to sync coffe warehouse
     :param app: Any
     :return: None
     """
     location_qs = models.Location.objects.get_coffe_ware_houses()
     warehouse_model = models.CoffeeWareHouse
     for location in location_qs:
-        warehouse = warehouse_model.objects.get_by_location_id(location.locationid).first()
+        warehouse = warehouse_model.objects.get_by_location_id(location.get("locationid")).first()
         if warehouse is None:
             warehouse = warehouse_model()
-            warehouse.location_id = location.locationid
-        warehouse.location_name = location.locationname
+            warehouse.location_id = location.get("locationid")
+        warehouse.location_name = location.get("locationname")
+        warehouse.city_name = location.get("city")
         warehouse.save()
```

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/sync_company.py` & `django-oasis4-1.1.2/oasis/tasks/sync_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/sync_document_types.py` & `django-oasis4-1.1.2/oasis/tasks/sync_document_types.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/oasis/tasks/sync_products.py` & `django-oasis4-1.1.2/oasis/tasks/sync_products.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.1a2/pyproject.toml` & `django-oasis4-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "django-oasis4"
-version = "1.1.1-alpha.2"
+version = "1.1.2"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "OASIS4 Data Interfaces"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
@@ -26,13 +26,14 @@
     "Topic :: Internet :: WWW/HTTP"
 ]
 dependencies = [
     "Django>=4.1",
     "cx-Oracle",
     "celery>=5.2.7",
     "django-celery-beat",
-    "zibanu-django>=1.0.0a8"
+    "zibanu-django>=1.2.0a11",
+    "num2words"
 ]
 keywords = [
     "django",
     "cadefihuila"
 ]
```

