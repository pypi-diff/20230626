# Comparing `tmp/django-oasis4-1.1.2b2.tar.gz` & `tmp/django-oasis4-1.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-oasis4-1.1.2b2.tar", last modified: Wed Jun 14 21:07:08 2023, max compression
+gzip compressed data, was "django-oasis4-1.1.2rc0.tar", last modified: Mon Jun 26 19:18:35 2023, max compression
```

## Comparing `django-oasis4-1.1.2b2.tar` & `django-oasis4-1.1.2rc0.tar`

### file list

```diff
@@ -1,154 +1,155 @@
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.238859 django-oasis4-1.1.2b2/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-1.1.2b2/LICENSE
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-03-02 20:32:01.000000 django-oasis4-1.1.2b2/MANIFEST.in
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-06-14 21:07:08.238859 django-oasis4-1.1.2b2/PKG-INFO
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      217 2023-02-13 15:48:51.000000 django-oasis4-1.1.2b2/README.md
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.212860 django-oasis4-1.1.2b2/django_oasis4.egg-info/
--rw-r--r--   0 macercha  (1000) macercha  (1000)    13080 2023-06-14 21:07:08.000000 django-oasis4-1.1.2b2/django_oasis4.egg-info/PKG-INFO
--rw-r--r--   0 macercha  (1000) macercha  (1000)     4738 2023-06-14 21:07:08.000000 django-oasis4-1.1.2b2/django_oasis4.egg-info/SOURCES.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-14 21:07:08.000000 django-oasis4-1.1.2b2/django_oasis4.egg-info/dependency_links.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)       89 2023-06-14 21:07:08.000000 django-oasis4-1.1.2b2/django_oasis4.egg-info/requires.txt
--rw-r--r--   0 macercha  (1000) macercha  (1000)        6 2023-06-14 21:07:08.000000 django-oasis4-1.1.2b2/django_oasis4.egg-info/top_level.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.214860 django-oasis4-1.1.2b2/oasis/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-10 23:55:40.000000 django-oasis4-1.1.2b2/oasis/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1394 2023-03-18 18:38:34.000000 django-oasis4-1.1.2b2/oasis/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.214860 django-oasis4-1.1.2b2/oasis/coffee_offers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-22 14:19:30.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      686 2023-03-06 19:37:38.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/admin.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1253 2023-03-07 16:31:05.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/admin_views.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.215860 django-oasis4-1.1.2b2/oasis/coffee_offers/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-23 15:03:46.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.215860 django-oasis4-1.1.2b2/oasis/coffee_offers/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      683 2023-03-06 19:10:13.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      772 2023-02-23 15:21:03.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/api/serializers/coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1199 2023-03-06 20:11:27.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/api/serializers/offer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.215860 django-oasis4-1.1.2b2/oasis/coffee_offers/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-03-01 20:03:07.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    11195 2023-06-13 22:51:27.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/api/services/coffee_offers.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5245 2023-06-03 21:53:44.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.216859 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-26 20:27:18.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.216859 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      659 2023-06-10 20:14:20.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1137 2023-06-02 10:37:36.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/choices/coffee_offers_states.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      825 2023-06-10 20:14:20.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/choices/oasis_choices.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.216859 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/events/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      417 2023-03-16 21:48:47.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/events/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-03-16 21:48:47.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/events/on_post_save_offer.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.217860 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 21:38:01.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7775 2023-06-14 20:13:51.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/utils/offer_state_machine.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.218860 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/validators/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      757 2023-02-26 21:14:28.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/validators/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1336 2023-02-26 21:13:57.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/validators/date_validators.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      823 2023-02-26 20:45:48.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/lib/validators/oasis_statuses.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.206860 django-oasis4-1.1.2b2/oasis/coffee_offers/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.206860 django-oasis4-1.1.2b2/oasis/coffee_offers/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.218860 django-oasis4-1.1.2b2/oasis/coffee_offers/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6053 2023-06-13 22:51:27.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     8627 2023-06-13 22:51:27.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.218860 django-oasis4-1.1.2b2/oasis/coffee_offers/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 23:14:13.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1564 2023-06-03 21:35:38.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/tasks/sync_coffe_offers.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.219859 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1072 2023-03-08 13:40:32.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/change_status.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2023-03-08 13:40:32.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/change_status.txt
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.221859 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      845 2023-06-04 23:24:43.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/coffee_notification.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4553 2023-06-14 20:57:54.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/coffee_offer.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1723 2023-06-14 20:57:54.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/coffee_offers_base.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     8990 2023-06-13 22:51:27.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/contract_template.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     6218 2023-06-10 20:14:20.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/intention_letter.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2579 2023-06-10 20:14:20.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/promissory_note.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1984 2023-06-13 22:51:27.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/remittance_letter.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1054 2023-03-02 20:24:29.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/save_offer.html
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      785 2023-03-02 20:03:04.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/templates/save_offer.txt
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      981 2023-03-16 14:42:57.000000 django-oasis4-1.1.2b2/oasis/coffee_offers/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.221859 django-oasis4-1.1.2b2/oasis/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-11-16 14:55:35.000000 django-oasis4-1.1.2b2/oasis/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.221859 django-oasis4-1.1.2b2/oasis/lib/choices/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      582 2023-01-17 21:45:20.000000 django-oasis4-1.1.2b2/oasis/lib/choices/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      783 2023-03-18 17:17:41.000000 django-oasis4-1.1.2b2/oasis/lib/choices/customer_type.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.225859 django-oasis4-1.1.2b2/oasis/lib/managers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1525 2023-03-16 14:42:57.000000 django-oasis4-1.1.2b2/oasis/lib/managers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      780 2023-02-23 14:39:16.000000 django-oasis4-1.1.2b2/oasis/lib/managers/local_coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      682 2023-01-28 14:38:17.000000 django-oasis4-1.1.2b2/oasis/lib/managers/local_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1355 2023-01-18 02:07:35.000000 django-oasis4-1.1.2b2/oasis/lib/managers/local_document_type.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1578 2023-03-08 14:17:45.000000 django-oasis4-1.1.2b2/oasis/lib/managers/local_offer.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1212 2022-12-14 20:34:45.000000 django-oasis4-1.1.2b2/oasis/lib/managers/local_product.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2159 2023-03-16 14:42:57.000000 django-oasis4-1.1.2b2/oasis/lib/managers/local_state_machine.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1201 2023-03-02 21:35:32.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_associate_balance.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2701 2023-03-01 16:42:42.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_client.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1050 2023-01-27 03:47:52.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1390 2023-02-07 10:48:09.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     4007 2023-01-24 23:42:01.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_discount.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-01-24 23:42:01.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_geographic_location.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1452 2023-06-10 20:07:22.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_location.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     7130 2023-03-08 14:56:20.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_operation.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-02-06 19:28:19.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_periods.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      906 2022-12-19 16:49:04.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_product.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      730 2023-01-25 00:42:41.000000 django-oasis4-1.1.2b2/oasis/lib/managers/oasis_type_client.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.226859 django-oasis4-1.1.2b2/oasis/lib/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      658 2023-02-07 09:06:27.000000 django-oasis4-1.1.2b2/oasis/lib/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      789 2023-02-07 09:25:36.000000 django-oasis4-1.1.2b2/oasis/lib/serializers/oasis_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2022-12-14 20:01:00.000000 django-oasis4-1.1.2b2/oasis/lib/serializers/product.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.226859 django-oasis4-1.1.2b2/oasis/lib/utils/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      579 2023-03-03 19:38:17.000000 django-oasis4-1.1.2b2/oasis/lib/utils/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3275 2023-06-13 22:51:27.000000 django-oasis4-1.1.2b2/oasis/lib/utils/oasis_actions.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.207860 django-oasis4-1.1.2b2/oasis/locale/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.207860 django-oasis4-1.1.2b2/oasis/locale/es/
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.226859 django-oasis4-1.1.2b2/oasis/locale/es/LC_MESSAGES/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     2138 2023-05-24 03:50:25.000000 django-oasis4-1.1.2b2/oasis/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5606 2023-05-24 03:50:25.000000 django-oasis4-1.1.2b2/oasis/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.231859 django-oasis4-1.1.2b2/oasis/migrations/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    29691 2022-12-13 18:21:01.000000 django-oasis4-1.1.2b2/oasis/migrations/0001_initial.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    31003 2023-01-17 22:22:35.000000 django-oasis4-1.1.2b2/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    17130 2023-01-26 02:36:44.000000 django-oasis4-1.1.2b2/oasis/migrations/0003_oasiscompany_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     5814 2023-01-27 03:47:55.000000 django-oasis4-1.1.2b2/oasis/migrations/0004_account_vaccountingbalanceclient.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      515 2023-02-02 01:56:29.000000 django-oasis4-1.1.2b2/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1582 2023-02-05 00:32:58.000000 django-oasis4-1.1.2b2/oasis/migrations/0006_periods.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      949 2023-02-07 02:05:07.000000 django-oasis4-1.1.2b2/oasis/migrations/0007_cycle.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9373 2023-02-23 14:51:01.000000 django-oasis4-1.1.2b2/oasis/migrations/0008_location_coffeewarehouse_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3584 2023-03-01 16:44:41.000000 django-oasis4-1.1.2b2/oasis/migrations/0009_associatebalance.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)    47342 2023-03-03 23:16:58.000000 django-oasis4-1.1.2b2/oasis/migrations/0010_operation.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3905 2023-03-04 03:34:51.000000 django-oasis4-1.1.2b2/oasis/migrations/0011_offer_statemachine_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      442 2023-03-04 03:50:49.000000 django-oasis4-1.1.2b2/oasis/migrations/0012_offer_price.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1782 2023-03-06 20:01:57.000000 django-oasis4-1.1.2b2/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      832 2023-03-07 08:33:48.000000 django-oasis4-1.1.2b2/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      465 2023-03-07 08:43:20.000000 django-oasis4-1.1.2b2/oasis/migrations/0015_statemachine_update_oasis.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-03-16 14:42:57.000000 django-oasis4-1.1.2b2/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      571 2023-03-16 14:42:57.000000 django-oasis4-1.1.2b2/oasis/migrations/0017_statemachine_state_at_timeout.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1553 2023-03-16 21:48:47.000000 django-oasis4-1.1.2b2/oasis/migrations/0018_offermov.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/migrations/0019_stat.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      413 2023-06-10 19:30:28.000000 django-oasis4-1.1.2b2/oasis/migrations/0020_coffeewarehouse_city_name.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2022-12-10 21:43:40.000000 django-oasis4-1.1.2b2/oasis/migrations/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.231859 django-oasis4-1.1.2b2/oasis/models/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/models/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     9449 2023-06-10 19:26:11.000000 django-oasis4-1.1.2b2/oasis/models/local_models.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)   117483 2023-03-04 02:04:38.000000 django-oasis4-1.1.2b2/oasis/models/oasis_models.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.235859 django-oasis4-1.1.2b2/oasis/stats/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/stats/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      419 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/stats/admin.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.235859 django-oasis4-1.1.2b2/oasis/stats/api/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/stats/api/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.236859 django-oasis4-1.1.2b2/oasis/stats/api/serializers/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      329 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/stats/api/serializers/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/stats/api/serializers/stats.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.236859 django-oasis4-1.1.2b2/oasis/stats/api/services/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      327 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/stats/api/services/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     3684 2023-05-24 03:50:25.000000 django-oasis4-1.1.2b2/oasis/stats/api/services/stats.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      455 2023-05-19 21:49:17.000000 django-oasis4-1.1.2b2/oasis/stats/apps.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.236859 django-oasis4-1.1.2b2/oasis/stats/lib/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      477 2023-05-24 03:50:25.000000 django-oasis4-1.1.2b2/oasis/stats/lib/__init__.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.237859 django-oasis4-1.1.2b2/oasis/stats/lib/cursors/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      504 2023-05-24 03:50:25.000000 django-oasis4-1.1.2b2/oasis/stats/lib/cursors/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1917 2023-05-24 03:50:25.000000 django-oasis4-1.1.2b2/oasis/stats/lib/cursors/cursor.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      586 2023-05-24 03:50:25.000000 django-oasis4-1.1.2b2/oasis/stats/urls.py
-drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-14 21:07:08.238859 django-oasis4-1.1.2b2/oasis/tasks/
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-23 14:54:47.000000 django-oasis4-1.1.2b2/oasis/tasks/__init__.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1278 2023-06-10 20:10:04.000000 django-oasis4-1.1.2b2/oasis/tasks/sync_coffee_ware_house.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1474 2023-01-26 02:47:20.000000 django-oasis4-1.1.2b2/oasis/tasks/sync_company.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-01-18 02:09:04.000000 django-oasis4-1.1.2b2/oasis/tasks/sync_document_types.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)     1856 2023-03-01 20:00:10.000000 django-oasis4-1.1.2b2/oasis/tasks/sync_products.py
--rw-rw-r--   0 macercha  (1000) macercha  (1000)      883 2023-06-14 21:05:51.000000 django-oasis4-1.1.2b2/pyproject.toml
--rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-14 21:07:08.238859 django-oasis4-1.1.2b2/setup.cfg
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.089554 django-oasis4-1.1.2rc0/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11375 2023-01-23 20:26:24.000000 django-oasis4-1.1.2rc0/LICENSE
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      144 2023-03-02 20:32:01.000000 django-oasis4-1.1.2rc0/MANIFEST.in
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13081 2023-06-26 19:18:35.089554 django-oasis4-1.1.2rc0/PKG-INFO
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      217 2023-02-13 15:48:51.000000 django-oasis4-1.1.2rc0/README.md
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.064555 django-oasis4-1.1.2rc0/django_oasis4.egg-info/
+-rw-r--r--   0 macercha  (1000) macercha  (1000)    13081 2023-06-26 19:18:35.000000 django-oasis4-1.1.2rc0/django_oasis4.egg-info/PKG-INFO
+-rw-r--r--   0 macercha  (1000) macercha  (1000)     4801 2023-06-26 19:18:35.000000 django-oasis4-1.1.2rc0/django_oasis4.egg-info/SOURCES.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        1 2023-06-26 19:18:35.000000 django-oasis4-1.1.2rc0/django_oasis4.egg-info/dependency_links.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       89 2023-06-26 19:18:35.000000 django-oasis4-1.1.2rc0/django_oasis4.egg-info/requires.txt
+-rw-r--r--   0 macercha  (1000) macercha  (1000)        6 2023-06-26 19:18:35.000000 django-oasis4-1.1.2rc0/django_oasis4.egg-info/top_level.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.064555 django-oasis4-1.1.2rc0/oasis/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-12-10 23:55:40.000000 django-oasis4-1.1.2rc0/oasis/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1394 2023-03-18 18:38:34.000000 django-oasis4-1.1.2rc0/oasis/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.065555 django-oasis4-1.1.2rc0/oasis/coffee_offers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-02-22 14:19:30.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      686 2023-03-06 19:37:38.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/admin.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1253 2023-03-07 16:31:05.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/admin_views.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.065555 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-23 15:03:46.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.066555 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      683 2023-03-06 19:10:13.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      772 2023-02-23 15:21:03.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/serializers/coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1199 2023-03-06 20:11:27.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/serializers/offer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.066555 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      580 2023-03-01 20:03:07.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    11195 2023-06-13 22:51:27.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/api/services/coffee_offers.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5245 2023-06-03 21:53:44.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.066555 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      506 2023-02-26 20:27:18.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.067555 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      659 2023-06-10 20:14:20.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1137 2023-06-02 10:37:36.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/choices/coffee_offers_states.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      825 2023-06-10 20:14:20.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/choices/oasis_choices.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.067555 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/events/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      417 2023-03-16 21:48:47.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/events/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-03-16 21:48:47.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/events/on_post_save_offer.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.068555 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 21:38:01.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     8161 2023-06-26 19:09:34.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/utils/offer_state_machine.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.068555 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/validators/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      757 2023-02-26 21:14:28.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/validators/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1336 2023-02-26 21:13:57.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/validators/date_validators.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      823 2023-02-26 20:45:48.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/validators/oasis_statuses.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.060555 django-oasis4-1.1.2rc0/oasis/coffee_offers/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.060555 django-oasis4-1.1.2rc0/oasis/coffee_offers/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.072555 django-oasis4-1.1.2rc0/oasis/coffee_offers/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6053 2023-06-13 22:51:27.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     8627 2023-06-13 22:51:27.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.073555 django-oasis4-1.1.2rc0/oasis/coffee_offers/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      595 2023-03-06 23:14:13.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1565 2023-06-24 01:48:43.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/tasks/sync_coffe_offers.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.073555 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1072 2023-03-08 13:40:32.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/change_status.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2023-03-08 13:40:32.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/change_status.txt
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.075554 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      845 2023-06-04 23:24:43.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/coffee_notification.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4580 2023-06-26 13:45:29.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/coffee_offer.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1723 2023-06-14 20:57:54.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/coffee_offers_base.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     8990 2023-06-13 22:51:27.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/contract_template.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     6218 2023-06-10 20:14:20.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/intention_letter.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2579 2023-06-10 20:14:20.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/promissory_note.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1984 2023-06-13 22:51:27.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/remittance_letter.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1054 2023-03-02 20:24:29.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/save_offer.html
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      785 2023-03-02 20:03:04.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/save_offer.txt
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      981 2023-03-16 14:42:57.000000 django-oasis4-1.1.2rc0/oasis/coffee_offers/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.075554 django-oasis4-1.1.2rc0/oasis/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      508 2022-11-16 14:55:35.000000 django-oasis4-1.1.2rc0/oasis/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.076555 django-oasis4-1.1.2rc0/oasis/lib/choices/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      582 2023-01-17 21:45:20.000000 django-oasis4-1.1.2rc0/oasis/lib/choices/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      783 2023-03-18 17:17:41.000000 django-oasis4-1.1.2rc0/oasis/lib/choices/customer_type.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.079554 django-oasis4-1.1.2rc0/oasis/lib/managers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1525 2023-03-16 14:42:57.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      780 2023-02-23 14:39:16.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/local_coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      682 2023-01-28 14:38:17.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/local_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1355 2023-01-18 02:07:35.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/local_document_type.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1578 2023-03-08 14:17:45.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/local_offer.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1212 2022-12-14 20:34:45.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/local_product.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2159 2023-03-16 14:42:57.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/local_state_machine.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1201 2023-03-02 21:35:32.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_associate_balance.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2701 2023-03-01 16:42:42.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_client.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1050 2023-01-27 03:47:52.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1390 2023-02-07 10:48:09.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     4007 2023-01-24 23:42:01.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_discount.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1180 2023-01-24 23:42:01.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_geographic_location.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1452 2023-06-10 20:07:22.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_location.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     7648 2023-06-26 14:57:54.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_operation.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      939 2023-02-06 19:28:19.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_periods.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      906 2022-12-19 16:49:04.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_product.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      730 2023-01-25 00:42:41.000000 django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_type_client.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.080555 django-oasis4-1.1.2rc0/oasis/lib/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      658 2023-02-07 09:06:27.000000 django-oasis4-1.1.2rc0/oasis/lib/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      789 2023-02-07 09:25:36.000000 django-oasis4-1.1.2rc0/oasis/lib/serializers/oasis_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      803 2022-12-14 20:01:00.000000 django-oasis4-1.1.2rc0/oasis/lib/serializers/product.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.080555 django-oasis4-1.1.2rc0/oasis/lib/utils/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      579 2023-03-03 19:38:17.000000 django-oasis4-1.1.2rc0/oasis/lib/utils/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3275 2023-06-13 22:51:27.000000 django-oasis4-1.1.2rc0/oasis/lib/utils/oasis_actions.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.061555 django-oasis4-1.1.2rc0/oasis/locale/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.061555 django-oasis4-1.1.2rc0/oasis/locale/es/
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.080555 django-oasis4-1.1.2rc0/oasis/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     2138 2023-05-24 03:50:25.000000 django-oasis4-1.1.2rc0/oasis/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5606 2023-05-24 03:50:25.000000 django-oasis4-1.1.2rc0/oasis/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.084554 django-oasis4-1.1.2rc0/oasis/migrations/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    29691 2022-12-13 18:21:01.000000 django-oasis4-1.1.2rc0/oasis/migrations/0001_initial.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    31003 2023-01-17 22:22:35.000000 django-oasis4-1.1.2rc0/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    17130 2023-01-26 02:36:44.000000 django-oasis4-1.1.2rc0/oasis/migrations/0003_oasiscompany_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     5814 2023-01-27 03:47:55.000000 django-oasis4-1.1.2rc0/oasis/migrations/0004_account_vaccountingbalanceclient.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      515 2023-02-02 01:56:29.000000 django-oasis4-1.1.2rc0/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1582 2023-02-05 00:32:58.000000 django-oasis4-1.1.2rc0/oasis/migrations/0006_periods.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      949 2023-02-07 02:05:07.000000 django-oasis4-1.1.2rc0/oasis/migrations/0007_cycle.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9373 2023-02-23 14:51:01.000000 django-oasis4-1.1.2rc0/oasis/migrations/0008_location_coffeewarehouse_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3584 2023-03-01 16:44:41.000000 django-oasis4-1.1.2rc0/oasis/migrations/0009_associatebalance.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)    47342 2023-03-03 23:16:58.000000 django-oasis4-1.1.2rc0/oasis/migrations/0010_operation.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3905 2023-03-04 03:34:51.000000 django-oasis4-1.1.2rc0/oasis/migrations/0011_offer_statemachine_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      442 2023-03-04 03:50:49.000000 django-oasis4-1.1.2rc0/oasis/migrations/0012_offer_price.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1782 2023-03-06 20:01:57.000000 django-oasis4-1.1.2rc0/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      832 2023-03-07 08:33:48.000000 django-oasis4-1.1.2rc0/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      465 2023-03-07 08:43:20.000000 django-oasis4-1.1.2rc0/oasis/migrations/0015_statemachine_update_oasis.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      624 2023-03-16 14:42:57.000000 django-oasis4-1.1.2rc0/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      571 2023-03-16 14:42:57.000000 django-oasis4-1.1.2rc0/oasis/migrations/0017_statemachine_state_at_timeout.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1553 2023-03-16 21:48:47.000000 django-oasis4-1.1.2rc0/oasis/migrations/0018_offermov.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1009 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/migrations/0019_stat.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      413 2023-06-10 19:30:28.000000 django-oasis4-1.1.2rc0/oasis/migrations/0020_coffeewarehouse_city_name.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      641 2023-06-26 13:05:00.000000 django-oasis4-1.1.2rc0/oasis/migrations/0021_offer_confirmed_at_offer_confirmed_by.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)        0 2022-12-10 21:43:40.000000 django-oasis4-1.1.2rc0/oasis/migrations/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.085554 django-oasis4-1.1.2rc0/oasis/models/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1647 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/models/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     9660 2023-06-24 01:16:19.000000 django-oasis4-1.1.2rc0/oasis/models/local_models.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)   117487 2023-06-26 16:21:43.000000 django-oasis4-1.1.2rc0/oasis/models/oasis_models.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.086554 django-oasis4-1.1.2rc0/oasis/stats/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/stats/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      419 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/stats/admin.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.086554 django-oasis4-1.1.2rc0/oasis/stats/api/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      293 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/stats/api/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.087554 django-oasis4-1.1.2rc0/oasis/stats/api/serializers/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      329 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/stats/api/serializers/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      505 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/stats/api/serializers/stats.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.087554 django-oasis4-1.1.2rc0/oasis/stats/api/services/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      327 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/stats/api/services/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     3684 2023-05-24 03:50:25.000000 django-oasis4-1.1.2rc0/oasis/stats/api/services/stats.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      455 2023-05-19 21:49:17.000000 django-oasis4-1.1.2rc0/oasis/stats/apps.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.087554 django-oasis4-1.1.2rc0/oasis/stats/lib/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      477 2023-05-24 03:50:25.000000 django-oasis4-1.1.2rc0/oasis/stats/lib/__init__.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.088554 django-oasis4-1.1.2rc0/oasis/stats/lib/cursors/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      504 2023-05-24 03:50:25.000000 django-oasis4-1.1.2rc0/oasis/stats/lib/cursors/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1917 2023-05-24 03:50:25.000000 django-oasis4-1.1.2rc0/oasis/stats/lib/cursors/cursor.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      586 2023-05-24 03:50:25.000000 django-oasis4-1.1.2rc0/oasis/stats/urls.py
+drwxr-xr-x   0 macercha  (1000) macercha  (1000)        0 2023-06-26 19:18:35.089554 django-oasis4-1.1.2rc0/oasis/tasks/
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      812 2023-02-23 14:54:47.000000 django-oasis4-1.1.2rc0/oasis/tasks/__init__.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1278 2023-06-10 20:10:04.000000 django-oasis4-1.1.2rc0/oasis/tasks/sync_coffee_ware_house.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1474 2023-01-26 02:47:20.000000 django-oasis4-1.1.2rc0/oasis/tasks/sync_company.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1018 2023-01-18 02:09:04.000000 django-oasis4-1.1.2rc0/oasis/tasks/sync_document_types.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)     1856 2023-03-01 20:00:10.000000 django-oasis4-1.1.2rc0/oasis/tasks/sync_products.py
+-rw-rw-r--   0 macercha  (1000) macercha  (1000)      881 2023-06-26 19:18:23.000000 django-oasis4-1.1.2rc0/pyproject.toml
+-rw-r--r--   0 macercha  (1000) macercha  (1000)       38 2023-06-26 19:18:35.089554 django-oasis4-1.1.2rc0/setup.cfg
```

### Comparing `django-oasis4-1.1.2b2/LICENSE` & `django-oasis4-1.1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/PKG-INFO` & `django-oasis4-1.1.2rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4
-Version: 1.1.2b2
+Version: 1.1.2rc0
 Summary: OASIS4 Data Interfaces
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-1.1.2b2/django_oasis4.egg-info/PKG-INFO` & `django-oasis4-1.1.2rc0/django_oasis4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oasis4
-Version: 1.1.2b2
+Version: 1.1.2rc0
 Summary: OASIS4 Data Interfaces
 Author-email: Mario Cerón <mario.ceron@cqinversiones.co>
 License:                                     CQ INVERSIONES S.A.S.
                                       CONTRATO DE LICENCIA DE SOFTWARE
                                                     NO OEM
                                              (Version 2.0 - 2023)
```

### Comparing `django-oasis4-1.1.2b2/django_oasis4.egg-info/SOURCES.txt` & `django-oasis4-1.1.2rc0/django_oasis4.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py
 oasis/migrations/0015_statemachine_update_oasis.py
 oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py
 oasis/migrations/0017_statemachine_state_at_timeout.py
 oasis/migrations/0018_offermov.py
 oasis/migrations/0019_stat.py
 oasis/migrations/0020_coffeewarehouse_city_name.py
+oasis/migrations/0021_offer_confirmed_at_offer_confirmed_by.py
 oasis/migrations/__init__.py
 oasis/models/__init__.py
 oasis/models/local_models.py
 oasis/models/oasis_models.py
 oasis/stats/__init__.py
 oasis/stats/admin.py
 oasis/stats/apps.py
```

### Comparing `django-oasis4-1.1.2b2/oasis/apps.py` & `django-oasis4-1.1.2rc0/oasis/apps.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/admin.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/admin.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/admin_views.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/admin_views.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/api/serializers/__init__.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/api/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/api/serializers/coffee_ware_house.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/api/serializers/coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/api/serializers/offer.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/api/serializers/offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/api/services/__init__.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/api/services/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/api/services/coffee_offers.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/api/services/coffee_offers.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/apps.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/apps.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/choices/__init__.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/choices/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/choices/coffee_offers_states.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/choices/coffee_offers_states.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/choices/oasis_choices.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/choices/oasis_choices.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/events/on_post_save_offer.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/events/on_post_save_offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/utils/__init__.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/utils/offer_state_machine.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/utils/offer_state_machine.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from django.utils import timezone
 from django.db import DatabaseError
 from django.utils.translation import gettext_lazy as _
 from oasis.models import Operation, Company
 from oasis.models import StateMachine
 from zibanu.django.repository.lib.utils import DocumentGenerator
 from zibanu.django.utils import Email
+from zibanu.django.utils import change_timezone
 from oasis.coffee_offers.lib.choices import OasisChoices
 from num2words import num2words
 
 
 class OfferStateMachine:
     PREFIX = "coffee_offers"
 
@@ -114,32 +115,37 @@
 
     def run(self) -> None:
         """
         Run a machine state to get and assign next state value.
         :return:
         """
         # TODO: Unify run and set methods.
-        oasis_state = self.__operation.state
-        oasis_status = self.__operation.status
+        oasis_state = self.__operation.get("state")
+        oasis_status = self.__operation.get("status")
         state = StateMachine.objects.get_next_state(from_state=self.__from_status, oasis_state=oasis_state,
                                                     oasis_status=oasis_status)
         if state is not None:
             self.__offer.status = state.state
 
+            # Change confirmed by
+            if self.__operation.get("confirmby") != 0:
+                self.__offer.confirmed_by = self.__operation.get("confirmed_by")
+                self.__offer.confirmed_at = change_timezone(self.__operation.get("confirmdate"))
+
             # Change kg received
-            if self.__offer.kg_received != self.__operation.quantity:
-                self.__offer.kg_received = self.__operation.quantity
+            if self.__offer.kg_received != self.__operation.get("quantity"):
+                self.__offer.kg_received = self.__operation.get("quantity")
 
             if state.is_changed:
                 # Change kg offered
-                if self.__offer.kg_offered != self.__operation.otherif:
-                    self.__offer.kg_offered = self.__operation.otherif
+                if self.__offer.kg_offered != self.__operation.get("otherif"):
+                    self.__offer.kg_offered = self.__operation.get("otherif")
                 # Change delivery date
-                if self.__offer.delivery_date != self.__operation.finaldate:
-                    self.__offer.delivery_date = self.__operation.finaldate
+                if self.__offer.delivery_date != self.__operation.get("finaldate"):
+                    self.__offer.delivery_date = self.__operation.get("finaldate")
 
             self.__offer.save()
             self.__execute_flags(state)
 
     def set(self, new_state: int) -> None:
         """
         Set a new state and assign state and status in oasis operation entity
@@ -162,12 +168,12 @@
     def validate_timeout(self) -> None:
         """
         Validate a state timeout and set a new state.
         :return:
         """
         now = timezone.now()
         state = StateMachine.objects.get_current_state(current_state=self.__offer.status,
-                                                       oasis_state=self.__operation.state,
-                                                       oasis_status=self.__operation.status)
+                                                       oasis_state=self.__operation.get("state"),
+                                                       oasis_status=self.__operation.get("status"))
         if state is not None and state.timeout > 0:
             if (now - self.__offer.modified_at) > timedelta(hours=state.timeout):
                 self.set(state.state_at_timeout)
```

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/validators/__init__.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/validators/date_validators.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/validators/date_validators.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/lib/validators/oasis_statuses.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/lib/validators/oasis_statuses.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/tasks/__init__.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/tasks/sync_coffe_offers.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/tasks/sync_coffe_offers.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     document_id = settings.COFFEE_OFFERS_DOCUMENT
 
     offer_qs = Offer.objects.get_all_active_offers()
     for offer in offer_qs:
         operation = Operation.objects.get_by_operation_pk(document_id=document_id,
                                                           location_id=offer.warehouse.location_id,
                                                           number_id=offer.contract).first()
+
         if operation is not None:
             try:
                 state_machine = OfferStateMachine(offer, operation)
                 state_machine.run()
                 state_machine.validate_timeout()
             except ValueError as exc:
                 logging.debug(str(exc))
```

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/change_status.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/change_status.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/change_status.txt` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/change_status.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/coffee_notification.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/coffee_notification.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/coffee_offer.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/coffee_offer.html`

 * *Files 2% similar despite different names*

```diff
@@ -126,11 +126,11 @@
     <br>
     <br>
 
 {% endblock %}
 
 {% block footer_offers %}
     <div style="text-align: right">
-        <p>Confirmó: FORERO SANCHEZ EDERLETH</p>
-        <p>Fecha Confirmación: 07/03/2023 14:47:52</p>
+        <p>Confirmó: {{ offer.confirmed_by }}</p>
+        <p>Fecha Confirmación: {{ offer.confirmed_at|date:"d/m/Y h:i:s A" }}</p>
     </div>
 {% endblock %}
```

#### html2text {}

```diff
@@ -34,10 +34,10 @@
 Municipio de Entrega:  {{ offer.warehouse.city_name }}
 Fecha MÃ¡xima Entrega{{ offer.delivery_date }}
 Observaciones: PRUEBA DE OFERTA EN LINEA OA-{{ offer.warehouse.location_id }}-{
                { offer.contract }}
 
 
 {% endblock %} {% block footer_offers %}
-ConfirmÃ³: FORERO SANCHEZ EDERLETH
-Fecha ConfirmaciÃ³n: 07/03/2023 14:47:52
+ConfirmÃ³: {{ offer.confirmed_by }}
+Fecha ConfirmaciÃ³n: {{ offer.confirmed_at|date:"d/m/Y h:i:s A" }}
 {% endblock %}
```

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/coffee_offers_base.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/coffee_offers_base.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/contract_template.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/contract_template.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/intention_letter.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/intention_letter.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/promissory_note.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/promissory_note.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/coffee_offers/remittance_letter.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/coffee_offers/remittance_letter.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/save_offer.html` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/save_offer.html`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/templates/save_offer.txt` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/templates/save_offer.txt`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/coffee_offers/urls.py` & `django-oasis4-1.1.2rc0/oasis/coffee_offers/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/choices/__init__.py` & `django-oasis4-1.1.2rc0/oasis/lib/choices/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/choices/customer_type.py` & `django-oasis4-1.1.2rc0/oasis/lib/choices/customer_type.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/__init__.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/local_coffee_ware_house.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/local_coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/local_company.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/local_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/local_document_type.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/local_document_type.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/local_offer.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/local_offer.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/local_product.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/local_product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/local_state_machine.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/local_state_machine.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_associate_balance.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_associate_balance.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_client.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_client.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_company.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_cycle.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_discount.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_discount.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_geographic_location.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_geographic_location.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_location.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_location.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_operation.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_operation.py`

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

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_periods.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_periods.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_product.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/managers/oasis_type_client.py` & `django-oasis4-1.1.2rc0/oasis/lib/managers/oasis_type_client.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/serializers/__init__.py` & `django-oasis4-1.1.2rc0/oasis/lib/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/serializers/oasis_cycle.py` & `django-oasis4-1.1.2rc0/oasis/lib/serializers/oasis_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/serializers/product.py` & `django-oasis4-1.1.2rc0/oasis/lib/serializers/product.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/utils/__init__.py` & `django-oasis4-1.1.2rc0/oasis/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/lib/utils/oasis_actions.py` & `django-oasis4-1.1.2rc0/oasis/lib/utils/oasis_actions.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/locale/es/LC_MESSAGES/django.mo` & `django-oasis4-1.1.2rc0/oasis/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/locale/es/LC_MESSAGES/django.po` & `django-oasis4-1.1.2rc0/oasis/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0001_initial.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0002_geographiclocation_typeclient_documenttype_client_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0003_oasiscompany_company.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0003_oasiscompany_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0004_account_vaccountingbalanceclient.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0004_account_vaccountingbalanceclient.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0005_delete_vaccountingbalanceclient_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0006_periods.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0006_periods.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0007_cycle.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0007_cycle.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0008_location_coffeewarehouse_and_more.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0008_location_coffeewarehouse_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0009_associatebalance.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0009_associatebalance.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0010_operation.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0010_operation.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0011_offer_statemachine_and_more.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0011_offer_statemachine_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0013_statemachine_is_final_statemachine_is_initial_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0014_remove_statemachine_unq_coffeeoffer_statemachine_and_more.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0016_statemachine_is_changed_statemachine_timeout.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0017_statemachine_state_at_timeout.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0017_statemachine_state_at_timeout.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0018_offermov.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0018_offermov.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/migrations/0019_stat.py` & `django-oasis4-1.1.2rc0/oasis/migrations/0019_stat.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/models/__init__.py` & `django-oasis4-1.1.2rc0/oasis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/models/local_models.py` & `django-oasis4-1.1.2rc0/oasis/models/local_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,16 @@
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

### Comparing `django-oasis4-1.1.2b2/oasis/models/oasis_models.py` & `django-oasis4-1.1.2rc0/oasis/models/oasis_models.py`

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

### Comparing `django-oasis4-1.1.2b2/oasis/stats/api/services/stats.py` & `django-oasis4-1.1.2rc0/oasis/stats/api/services/stats.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/stats/lib/cursors/cursor.py` & `django-oasis4-1.1.2rc0/oasis/stats/lib/cursors/cursor.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/stats/urls.py` & `django-oasis4-1.1.2rc0/oasis/stats/urls.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/tasks/__init__.py` & `django-oasis4-1.1.2rc0/oasis/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/tasks/sync_coffee_ware_house.py` & `django-oasis4-1.1.2rc0/oasis/tasks/sync_coffee_ware_house.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/tasks/sync_company.py` & `django-oasis4-1.1.2rc0/oasis/tasks/sync_company.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/tasks/sync_document_types.py` & `django-oasis4-1.1.2rc0/oasis/tasks/sync_document_types.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/oasis/tasks/sync_products.py` & `django-oasis4-1.1.2rc0/oasis/tasks/sync_products.py`

 * *Files identical despite different names*

### Comparing `django-oasis4-1.1.2b2/pyproject.toml` & `django-oasis4-1.1.2rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel",
 ]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "django-oasis4"
-version = "1.1.2-beta.2"
+version = "1.1.2-rc.0"
 authors = [
     {name="Mario Cerón", email="mario.ceron@cqinversiones.co"}
 ]
 description = "OASIS4 Data Interfaces"
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">=3.9"
```

