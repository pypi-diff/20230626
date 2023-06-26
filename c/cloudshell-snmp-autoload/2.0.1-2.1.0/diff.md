# Comparing `tmp/cloudshell-snmp-autoload-2.0.1.zip` & `tmp/cloudshell-snmp-autoload-2.1.0.zip`

## zipinfo {}

```diff
@@ -1,92 +1,98 @@
-Zip file size: 69088 bytes, number of entries: 90
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/
--rw-r--r--  2.0 unx    11358 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/LICENSE
--rw-r--r--  2.0 unx      304 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/PKG-INFO
--rw-r--r--  2.0 unx     1060 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tox.ini
--rw-r--r--  2.0 unx      854 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/setup.py
--rw-r--r--  2.0 unx       71 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/dev_requirements.txt
--rw-r--r--  2.0 unx       38 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/setup.cfg
--rw-r--r--  2.0 unx      781 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/README.md
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/version.txt
--rw-r--r--  2.0 unx       35 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/MANIFEST.in
--rw-r--r--  2.0 unx       25 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/requirements.txt
--rw-r--r--  2.0 unx       55 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/test_requirements.txt
--rw-r--r--  2.0 unx       26 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/requires.txt
--rw-r--r--  2.0 unx      304 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/top_level.txt
--rw-r--r--  2.0 unx     3297 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/__init__.py
--rw-r--r--  2.0 unx     7632 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/generic_snmp_autoload.py
--rw-r--r--  2.0 unx      364 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/__init__.py
--rw-r--r--  2.0 unx     1841 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/port_constants.py
--rw-r--r--  2.0 unx     1771 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/entity_constants.py
--rw-r--r--  2.0 unx      971 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
--rw-r--r--  2.0 unx     7000 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_helper.py
--rw-r--r--  2.0 unx    12017 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/module_helper.py
--rw-r--r--  2.0 unx      918 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/entity_helper.py
--rw-r--r--  2.0 unx     2502 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_parent_validator.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/__init__.py
--rw-r--r--  2.0 unx      256 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_name_helper.py
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/snmp_autoload_error.py
--rw-r--r--  2.0 unx     8359 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_table.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/__init__.py
--rw-r--r--  2.0 unx     4935 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/system_info_table.py
--rw-r--r--  2.0 unx    10402 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/physical_entities_table.py
--rw-r--r--  2.0 unx     3432 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_mapping_table.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/__init__.py
--rw-r--r--  2.0 unx     1515 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/snmpv2_data.py
--rw-r--r--  2.0 unx     2361 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py
--rw-r--r--  2.0 unx     2043 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/
--rw-r--r--  2.0 unx     1315 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py
--rw-r--r--  2.0 unx     1019 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/__init__.py
--rw-r--r--  2.0 unx     2892 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py
--rw-r--r--  2.0 unx     1633 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py
--rw-r--r--  2.0 unx      471 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_service_interface.py
--rw-r--r--  2.0 unx     7295 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py
--rw-r--r--  2.0 unx     4271 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_port_ip_tables.py
--rw-r--r--  2.0 unx     1569 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/__init__.py
--rw-r--r--  2.0 unx     1683 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_duplex_table.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/__init__.py
--rw-r--r--  2.0 unx   186031 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/port_snmp_data.py
--rw-r--r--  2.0 unx     1241 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/test_snmp_if_table.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/
--rw-r--r--  2.0 unx       76 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/__init__.py
--rw-r--r--  2.0 unx     3023 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_port_helper.py
--rw-r--r--  2.0 unx     6305 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_entity_helper.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/__init__.py
--rw-r--r--  2.0 unx     4657 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_module_helper.py
--rw-r--r--  2.0 unx     3425 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py
--rw-r--r--  2.0 unx     2742 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/__init__.py
--rw-r--r--  2.0 unx     1422 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/if_port_data.py
--rw-r--r--  2.0 unx    93295 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/physical_entities_data.py
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-10 15:21 cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/__init__.py
-90 files, 411648 bytes uncompressed, 48994 bytes compressed:  88.1%
+Zip file size: 73040 bytes, number of entries: 96
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/
+-rw-r--r--  2.0 unx      304 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/PKG-INFO
+-rw-r--r--  2.0 unx      781 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/README.md
+-rw-r--r--  2.0 unx        6 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/version.txt
+-rw-r--r--  2.0 unx       38 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/setup.cfg
+-rw-r--r--  2.0 unx      854 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/setup.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/LICENSE
+-rw-r--r--  2.0 unx       71 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/dev_requirements.txt
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/requirements.txt
+-rw-r--r--  2.0 unx       55 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/test_requirements.txt
+-rw-r--r--  2.0 unx       35 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/MANIFEST.in
+-rw-r--r--  2.0 unx     1060 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tox.ini
+-rw-r--r--  2.0 unx      304 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       26 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     3544 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/top_level.txt
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/exceptions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/__init__.py
+-rw-r--r--  2.0 unx     7723 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/generic_snmp_autoload.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/__init__.py
+-rw-r--r--  2.0 unx     1789 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/snmpv2_data.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/__init__.py
+-rw-r--r--  2.0 unx     2474 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/
+-rw-r--r--  2.0 unx     1019 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/__init__.py
+-rw-r--r--  2.0 unx     2892 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py
+-rw-r--r--  2.0 unx     1315 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py
+-rw-r--r--  2.0 unx     7297 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/__init__.py
+-rw-r--r--  2.0 unx      471 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_service_interface.py
+-rw-r--r--  2.0 unx     4740 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_port_ip_tables.py
+-rw-r--r--  2.0 unx     1633 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py
+-rw-r--r--  2.0 unx     1806 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py
+-rw-r--r--  2.0 unx     1945 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_duplex_table.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/types/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/__init__.py
+-rw-r--r--  2.0 unx      971 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
+-rw-r--r--  2.0 unx     7000 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/port_helper.py
+-rw-r--r--  2.0 unx      256 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/port_name_helper.py
+-rw-r--r--  2.0 unx    12017 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/module_helper.py
+-rw-r--r--  2.0 unx     1138 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/entity_helper.py
+-rw-r--r--  2.0 unx     2483 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/port_parent_validator.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/types/__init__.py
+-rw-r--r--  2.0 unx     1673 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/types/resource_model.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/exceptions/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/exceptions/snmp_autoload_error.py
+-rw-r--r--  2.0 unx       76 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/__init__.py
+-rw-r--r--  2.0 unx     1771 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/entity_constants.py
+-rw-r--r--  2.0 unx      364 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
+-rw-r--r--  2.0 unx     1841 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/port_constants.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/__init__.py
+-rw-r--r--  2.0 unx     3432 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/port_mapping_table.py
+-rw-r--r--  2.0 unx     5210 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/system_info_table.py
+-rw-r--r--  2.0 unx     8575 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/port_table.py
+-rw-r--r--  2.0 unx    10644 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/physical_entities_table.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/services/
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/__init__.py
+-rw-r--r--  2.0 unx     1220 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/test_snmp_if_table.py
+-rw-r--r--  2.0 unx   186031 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/port_snmp_data.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/__init__.py
+-rw-r--r--  2.0 unx     7040 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_entity_helper.py
+-rw-r--r--  2.0 unx     3425 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py
+-rw-r--r--  2.0 unx     4657 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_module_helper.py
+-rw-r--r--  2.0 unx     3023 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_port_helper.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/__init__.py
+-rw-r--r--  2.0 unx     1422 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/if_port_data.py
+-rw-r--r--  2.0 unx    93293 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/physical_entities_data.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/services/__init__.py
+-rw-r--r--  2.0 unx     3962 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
+-rw-r--r--  2.0 unx     5536 b- defN 23-Jun-26 16:34 cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/services/test_snmp_system_info.py
+96 files, 423114 bytes uncompressed, 51484 bytes compressed:  87.8%
```

## zipnote {}

```diff
@@ -1,271 +1,289 @@
-Filename: cloudshell-snmp-autoload-2.0.1/
+Filename: cloudshell-snmp-autoload-2.1.0/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/
+Filename: cloudshell-snmp-autoload-2.1.0/tests/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/LICENSE
+Filename: cloudshell-snmp-autoload-2.1.0/PKG-INFO
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/PKG-INFO
+Filename: cloudshell-snmp-autoload-2.1.0/README.md
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tox.ini
+Filename: cloudshell-snmp-autoload-2.1.0/version.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/setup.py
+Filename: cloudshell-snmp-autoload-2.1.0/setup.cfg
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/dev_requirements.txt
+Filename: cloudshell-snmp-autoload-2.1.0/setup.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/setup.cfg
+Filename: cloudshell-snmp-autoload-2.1.0/LICENSE
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/README.md
+Filename: cloudshell-snmp-autoload-2.1.0/dev_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/version.txt
+Filename: cloudshell-snmp-autoload-2.1.0/requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/MANIFEST.in
+Filename: cloudshell-snmp-autoload-2.1.0/test_requirements.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/requirements.txt
+Filename: cloudshell-snmp-autoload-2.1.0/MANIFEST.in
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/test_requirements.txt
+Filename: cloudshell-snmp-autoload-2.1.0/tox.ini
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/requires.txt
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/PKG-INFO
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/PKG-INFO
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/requires.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/dependency_links.txt
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/dependency_links.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/top_level.txt
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/SOURCES.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/SOURCES.txt
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/top_level.txt
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/exceptions/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/generic_snmp_autoload.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/generic_snmp_autoload.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/port_constants.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/entity_constants.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/snmpv2_data.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/module_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/entity_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_parent_validator.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_name_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/exceptions/snmp_autoload_error.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_service_interface.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/system_info_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_port_ip_tables.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/physical_entities_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_mapping_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_duplex_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/types/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/snmpv2_data.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/port_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/port_name_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/module_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/entity_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/port_parent_validator.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/types/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/types/resource_model.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/exceptions/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/exceptions/snmp_autoload_error.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_service_interface.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/entity_constants.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_port_ip_tables.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/snmpv_v2_constants.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/port_constants.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_duplex_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/port_mapping_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/system_info_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/port_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/
+Filename: cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/physical_entities_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/
+Filename: cloudshell-snmp-autoload-2.1.0/tests/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/port_snmp_data.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/test_snmp_if_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_port_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/services/
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_entity_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_module_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/test_snmp_if_table.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/port_snmp_data.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/__init__.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/services/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_entity_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/if_port_data.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/physical_entities_data.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_module_helper.py
 Comment: 
 
-Filename: cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/__init__.py
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_port_helper.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/__init__.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/if_port_data.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/physical_entities_data.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/services/__init__.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
+Comment: 
+
+Filename: cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/services/test_snmp_system_info.py
 Comment: 
 
 Zip file comment:
```

## Comparing `cloudshell-snmp-autoload-2.0.1/LICENSE` & `cloudshell-snmp-autoload-2.1.0/LICENSE`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/tox.ini` & `cloudshell-snmp-autoload-2.1.0/tox.ini`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/setup.py` & `cloudshell-snmp-autoload-2.1.0/setup.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/README.md` & `cloudshell-snmp-autoload-2.1.0/README.md`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell_snmp_autoload.egg-info/SOURCES.txt` & `cloudshell-snmp-autoload-2.1.0/cloudshell_snmp_autoload.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 cloudshell/snmp/autoload/helper/__init__.py
 cloudshell/snmp/autoload/helper/entity_helper.py
 cloudshell/snmp/autoload/helper/module_helper.py
 cloudshell/snmp/autoload/helper/port_helper.py
 cloudshell/snmp/autoload/helper/port_name_helper.py
 cloudshell/snmp/autoload/helper/port_parent_validator.py
 cloudshell/snmp/autoload/helper/snmp_autoload_helper.py
+cloudshell/snmp/autoload/helper/types/__init__.py
+cloudshell/snmp/autoload/helper/types/resource_model.py
 cloudshell/snmp/autoload/services/__init__.py
 cloudshell/snmp/autoload/services/physical_entities_table.py
 cloudshell/snmp/autoload/services/port_mapping_table.py
 cloudshell/snmp/autoload/services/port_table.py
 cloudshell/snmp/autoload/services/system_info_table.py
 cloudshell/snmp/autoload/snmp/__init__.py
 cloudshell/snmp/autoload/snmp/snmpv2_data.py
@@ -49,20 +51,22 @@
 cloudshell_snmp_autoload.egg-info/SOURCES.txt
 cloudshell_snmp_autoload.egg-info/dependency_links.txt
 cloudshell_snmp_autoload.egg-info/requires.txt
 cloudshell_snmp_autoload.egg-info/top_level.txt
 tests/__init__.py
 tests/cloudshell/__init__.py
 tests/cloudshell/snmp/__init__.py
-tests/cloudshell/snmp/port_snmp_data.py
-tests/cloudshell/snmp/test_snmp_if_table.py
 tests/cloudshell/snmp/autoload/__init__.py
 tests/cloudshell/snmp/autoload/data/__init__.py
 tests/cloudshell/snmp/autoload/data/if_port_data.py
 tests/cloudshell/snmp/autoload/data/physical_entities_data.py
 tests/cloudshell/snmp/autoload/helper/__init__.py
 tests/cloudshell/snmp/autoload/helper/test_entity_helper.py
 tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py
 tests/cloudshell/snmp/autoload/helper/test_module_helper.py
 tests/cloudshell/snmp/autoload/helper/test_port_helper.py
 tests/cloudshell/snmp/autoload/services/__init__.py
-tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
+tests/cloudshell/snmp/autoload/services/test_physical_entities_table.py
+tests/cloudshell/snmp/autoload/services/test_snmp_system_info.py
+tests/cloudshell/snmp/autoload/snmp/__init__.py
+tests/cloudshell/snmp/autoload/snmp/port_snmp_data.py
+tests/cloudshell/snmp/autoload/snmp/test_snmp_if_table.py
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/generic_snmp_autoload.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/generic_snmp_autoload.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,30 +18,30 @@
 from cloudshell.snmp.autoload.snmp.tables.snmp_ports_table import SnmpPortsTable
 
 if TYPE_CHECKING:
     from logging import Logger
 
     from cloudshell.snmp.core.snmp_service import SnmpService
 
+    from cloudshell.snmp.autoload.helper.types.resource_model import ResourceModelProto
+
 
 class GenericSNMPAutoload:
     def __init__(
         self,
         snmp_handler: SnmpService,
         logger: Logger,
-        resource_model,
+        resource_model: ResourceModelProto,
     ):
         """Basic init with snmp handler and logger.
 
         :param snmp_handler: Snmp handler for general communication
         :param logger: Logger
         :param resource_model: Represents Resource Model according to a standard
         :type resource_model: cloudshell.shell.standards.autoload_generic_models.GenericResourceModel  # noqa: E501
-
-        :return:
         """
         self.snmp_handler = snmp_handler
         self.logger = logger
         self.elements = {}
         self._entity_table = None
         self._port_snmp_table = None
         self._if_table = None
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/port_constants.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/port_constants.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/constants/entity_constants.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/constants/entity_constants.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/snmp_autoload_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_helper.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/port_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/module_helper.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/module_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/entity_helper.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/entity_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,32 @@
+from abc import ABC, abstractmethod
+
 from cloudshell.snmp.autoload.constants.entity_constants import (
     ENTITY_VENDOR_TYPE_TO_CLASS_MAP,
 )
 from cloudshell.snmp.autoload.snmp.entities.snmp_entity_base import BaseEntity
 
 
-class EntityHelper:
+class EntityHelperAbc(ABC):
+    @abstractmethod
+    def get_physical_class(self, entity: BaseEntity) -> str:
+        raise NotImplementedError
+
+
+class EntityHelper(EntityHelperAbc):
     ENTITY_SAFE_CLASS_LIST = ["port", "powersupply"]
 
-    def get_physical_class(self, entity: BaseEntity):
+    def get_physical_class(self, entity: BaseEntity) -> str:
         entity_class = entity.entity_class
         if not entity_class or "other" in entity_class:
             if not entity.vendor_type:
                 if entity.position_id == "-1" and (
                     "chassis" in entity.name.lower()
                     or "chassis" in entity.description.lower()
                 ):
                     return "chassis"
                 return ""
             for key, value in ENTITY_VENDOR_TYPE_TO_CLASS_MAP.items():
-                if key.search(entity.vendor_type):
+                if key.search(entity.vendor_type_label):
                     entity_class = value
 
         return entity_class
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/helper/port_parent_validator.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/helper/port_parent_validator.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
     def validate_port_parent_ids(self, port):
         name = port.if_entity.if_name or port.if_entity.if_descr_name
         self._logger.debug(f"Start port {name} parent modules id validation")
         parent_ids = port.parent.full_id  # ["0", "11"]
         parent_ids_list = parent_ids.split("/")
         if re.search(parent_ids, name, re.IGNORECASE):
             self._logger.debug(f"Port {name} parent modules ids are valid.")
-            return
         else:
             parent_ids_from_port_match = re.search(r"\d+(/\d+)*$", name, re.IGNORECASE)
             if parent_ids_from_port_match:
                 parent_ids_from_port = (
                     parent_ids_from_port_match.group()
                 )  # ["0", "7", "0", "0"]
                 parent_ids_from_port_list = parent_ids_from_port.split("/")
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_table.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/port_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,25 @@
+from __future__ import annotations
+
 import re
 from functools import lru_cache
 from logging import Logger
-from typing import Dict
+from typing import TYPE_CHECKING
 
 from cloudshell.snmp.autoload.helper.port_name_helper import convert_port_name
 from cloudshell.snmp.autoload.snmp.entities.snmp_if_entity import SnmpIfEntity
 from cloudshell.snmp.autoload.snmp.tables.snmp_ports_table import SnmpPortsTable
 
+if TYPE_CHECKING:
+    from cloudshell.snmp.autoload.helper.types.resource_model import (
+        ResourceModelPortChanelProto,
+        ResourceModelPortProto,
+        ResourceModelProto,
+    )
+
 
 class PortsTable:
     ALLOWED_PORT_MODEL_NAME = ["GenericPort"]
     ALLOWED_PORT_CHANNEL_MODEL_NAME = ["GenericPortChannel"]
     PORT_CHANNEL_NAME_LIST = [
         r"^ae\d+",
         r"^port-channel\d+",
@@ -27,30 +36,26 @@
         r"stack|engine|management|mgmt|null|voice",
         r"control\s*ethernet\s*port|console\s*port",
     ]
     PORT_CHANNEL_EXCLUDE_LIST = []
 
     def __init__(
         self,
-        resource_model,
+        resource_model: ResourceModelProto,
         ports_snmp_table: SnmpPortsTable,
         logger: Logger,
     ):
-        """Init.
-
-        :type resource_model: cloudshell.shell.standards.autoload_generic_models.GenericResourceModel  # noqa: E501
-        """
         self._resource_model = resource_model
         self._if_table = {}
         self._if_entity = SnmpIfEntity
         self._duplex_table = {}
         self._adjacent_table = {}
         self._auto_negotiation = {}
-        self._if_port_dict = {}
-        self._if_port_channels_dict = {}
+        self._if_port_dict: dict[str, ResourceModelPortProto] = {}
+        self._if_port_channels_dict: dict[str, ResourceModelPortChanelProto] = {}
         self.port_name_to_object_map = {}
         self._unmapped_ports_list = []
         self.ports_tables = ports_snmp_table
         self._logger = logger
 
     @property
     @lru_cache()
@@ -99,15 +104,15 @@
         """
         if not self._if_port_dict:
             self._get_if_entities()
             self._if_port_dict = dict(sorted(self._if_port_dict.items()))
         return self._if_port_dict
 
     @property
-    def port_channels_dict(self) -> Dict[str, object]:
+    def port_channels_dict(self) -> dict[str, ResourceModelPortChanelProto]:
         """Port index to Port Channel object map.
 
         Port Channel object is the one defined in the standard's resource_model.
         Usually, ifIndex is used by various vendors as a mapping key, between
         interface table and other tables.
         """
         if not self._if_port_channels_dict:
@@ -211,12 +216,12 @@
 
     def _get_if_name_by_index(self, if_index):
         if if_index in self._if_port_dict:
             return self._if_port_dict.get(if_index).name
         snmp_port_data = self.load_if_port(if_index)
         return snmp_port_data.port_name
 
-    def is_wrong_port(self, port_name):
+    def is_wrong_port(self, port_name: str):
         return self.port_exclude_re.search(port_name.lower())
 
     def is_wrong_port_channel(self, port_name):
         return self.port_channel_exclude_re.search(port_name.lower())
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/system_info_table.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/system_info_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+from __future__ import annotations
+
 import re
 
+from cloudshell.snmp.core.domain.snmp_response import SnmpResponse
+
 from cloudshell.snmp.autoload.snmp.snmpv2_data import SnmpV2MibData
 
 
 class SnmpSystemInfo:
     DEVICE_MODEL_PATTERN = re.compile(r"::(?P<model>\S+$)")
     VENDOR_OID_PATTERN = re.compile(r"1.3.6.1.4.1.\d+")
     OS_VERSION_PATTERN = re.compile(r"Version (?P<os_version>[^\s,]+)")
@@ -95,41 +99,45 @@
             if oid_match:
                 self._vendor = self._snmp_handler.translate_oid(
                     oid_match.group()
                 ).capitalize()
 
         return self._vendor
 
-    def _get_device_os_version(self):
-        """Get device OS Version form snmp SNMPv2 mib.
-
-        :return: device model
-        :rtype: str
-        """
+    def _get_device_os_version(self) -> str:
+        """Get device OS Version form snmp SNMPv2 mib."""
         result = ""
         matched = self._os_version_pattern.search(
-            str(self._snmp_v2_obj.get_system_description())
+            self._snmp_v2_obj.get_system_description()
         )
         if matched:
             result = matched.groupdict().get("os_version", "")
         return result
 
     def fill_attributes(self, resource):
         """Get root element attributes.
 
         :type resource: cloudshell.shell_standards.autoload_generic_models.GenericResourceModel  # noqa: E501
         """
         self._logger.debug("Building Root started")
 
-        resource.contact_name = self._snmp_v2_obj.get_system_contact()
-        resource.system_name = self._snmp_v2_obj.get_system_name()
-        resource.location = self._snmp_v2_obj.get_system_location()
+        resource.contact_name = self._get_val(self._snmp_v2_obj.get_system_contact())
+        resource.system_name = self._get_val(self._snmp_v2_obj.get_system_name())
+        resource.location = self._get_val(self._snmp_v2_obj.get_system_location())
         resource.os_version = self._get_device_os_version()
         vendor = self._get_vendor()
         resource.vendor = vendor
 
         raw_model = self._get_device_model()
         model = re.sub(rf"^{vendor}", "", raw_model, flags=re.IGNORECASE)
         resource.model = model.capitalize()
         resource.model_name = model.capitalize()
 
         self._logger.info("Building Root completed")
+
+    @staticmethod
+    def _get_val(resp: SnmpResponse | None) -> str:
+        if resp is None:
+            val = ""
+        else:
+            val = resp.safe_value
+        return val
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/physical_entities_table.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/physical_entities_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,61 +3,70 @@
 import re
 from collections import defaultdict
 from logging import Logger
 from threading import Thread
 from typing import TYPE_CHECKING
 
 from cloudshell.snmp.autoload.exceptions.snmp_autoload_error import GeneralAutoloadError
-from cloudshell.snmp.autoload.helper.entity_helper import EntityHelper
+from cloudshell.snmp.autoload.helper.entity_helper import EntityHelper, EntityHelperAbc
 from cloudshell.snmp.autoload.helper.port_name_helper import convert_port_name
 from cloudshell.snmp.autoload.snmp.entities.snmp_entity_base import BaseEntity
 from cloudshell.snmp.autoload.snmp.tables.snmp_entity_table import SnmpEntityTable
 
 if TYPE_CHECKING:
+    from cloudshell.snmp.autoload.helper.types.resource_model import (
+        ResourceModelChassisProto,
+        ResourceModelProto,
+    )
+
     PhysId = str
 
 
 class PhysicalTable:
     MODULE_EXCLUDE_LIST = ["fan", "cpu"]
     MODULE_TO_CONTAINER_LIST = []
+    DUMMY_CHASSIS_ID = "0"
 
     def __init__(
         self,
         entity_table: SnmpEntityTable,
         logger: Logger,
-        resource_model,
+        resource_model: ResourceModelProto,
+        entity_helper: EntityHelperAbc = EntityHelper(),
     ):
-        """Init PhysicalTable.
-
-        :type resource_model: cloudshell.shell.standards.autoload_generic_models.GenericResourceModel  # noqa: E501
-        """
         self.entity_table = entity_table
         self._logger = logger
         self._resource_model = resource_model
         self._physical_structure_table = {}
         self._module_exclude_pattern = None
         self.power_port_exclude_pattern = None
         self.chassis_exclude_pattern = None
         self._port_list = []
         self._power_port_dict = {}
         self._chassis_dict = {}
         self.parent_dict = {}
         self.port_parent_dict = {}
         self._modules_hierarchy_dict = defaultdict(list)
         self.chassis_ids_dict = {}
-        self.chassis_helper = EntityHelper()
+        self._chassis_helper = entity_helper
         self._snmp_physical_structure_table = (
             self.entity_table.physical_structure_snmp_table
         )
         self._thread = Thread(
             name=self.__class__.__name__, target=self._get_entity_table
         )
         self._thread.start()
 
     @property
+    def chassis_helper(self) -> EntityHelperAbc:
+        if not self._chassis_helper:
+            self._chassis_helper = EntityHelper()
+        return self._chassis_helper
+
+    @property
     def module_exclude_pattern(self):
         pattern = "|".join(self.MODULE_EXCLUDE_LIST)
         return re.compile(pattern, re.IGNORECASE)
 
     @property
     def physical_ports_list(self):
         self._thread.join()
@@ -70,22 +79,19 @@
         :rtype: dict[PhysId,
         cloudshell.shell.standards.autoload_generic_models.AbstractResource]
         """
         self._thread.join()
         return self._power_port_dict
 
     @property
-    def physical_chassis_dict(self):
-        """Chassis dict based on Entity-MIB.
-
-        :rtype: dict[PhysId, cloudshell.shell.standards.autoload_generic_models.AbstractResource]
-        """
+    def physical_chassis_dict(self) -> dict[PhysId, ResourceModelChassisProto]:
+        """Chassis dict based on Entity-MIB."""
         self._thread.join()
         if not self._chassis_dict:
-            self._add_dummy_chassis("0")
+            self._add_dummy_chassis(self.DUMMY_CHASSIS_ID)
         return self._chassis_dict
 
     @property
     def physical_structure_table(self):
         """Entities table based on Entity-MIB.
 
         :rtype: dict[PhysId,
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/services/port_mapping_table.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/services/port_mapping_table.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/snmp_entity_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import re
+
 from cloudshell.snmp.autoload.constants.entity_constants import (
     ENTITY_CLASS,
     ENTITY_DESCRIPTION,
     ENTITY_HW_VERSION,
     ENTITY_MODEL,
     ENTITY_NAME,
     ENTITY_OS_VERSION,
@@ -61,14 +63,18 @@
 
     @property
     def vendor_type(self):
         result = self.entity_row_response.get(ENTITY_VENDOR_TYPE.object_name)
         return result.safe_value if result else ""
 
     @property
+    def vendor_type_label(self):
+        return re.sub(r"^.+::", "", self.vendor_type)
+
+    @property
     def model(self):
         result = self.entity_row_response.get(ENTITY_MODEL.object_name)
         return result.safe_value if result else ""
 
     @property
     def serial_number(self):
         result = self.entity_row_response.get(ENTITY_SERIAL.object_name)
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/entities/snmp_if_entity.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_entity_table.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_port_mapping_table.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/snmp_ports_table.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_associated_ports.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_neighbors_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from cloudshell.snmp.autoload.snmp.tables.port_attrs_snmp_tables.snmp_service_interface import (
     PortAttributesServiceInterface,
 )
 
 
 class PortNeighbours(PortAttributesServiceInterface):
     ADJACENT_TEMPLATE = "{remote_host} through {remote_port}"
-    LLDP_INDEX_PATTERN = re.compile(r".\d+.")
+    LLDP_INDEX_PATTERN = re.compile(r"\.\d+\.")
     LLDP_LOC_INTERFACE_NAME = "interfacename"
     LLDP_LOC_NETWORK_ADDR = "networkaddress"
     LLDP_LOC_MAC_ADDR = "macaddress"
     LLDP_LOC_INTERFACE_ALIAS = "interfacealias"
     PORT_NAME_PATTERN = r"{name}\b"
 
     def __init__(self, snmp_service: SnmpService, logger: Logger):
```

## Comparing `cloudshell-snmp-autoload-2.0.1/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py` & `cloudshell-snmp-autoload-2.1.0/cloudshell/snmp/autoload/snmp/tables/port_attrs_snmp_tables/snmp_ports_auto_negotioation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from logging import Logger
 from threading import Thread
 
+from pysnmp.proto.errind import RequestTimedOut
+
 from cloudshell.snmp.core.snmp_service import SnmpService
 
 from cloudshell.snmp.autoload.constants import port_constants
 from cloudshell.snmp.autoload.snmp.tables.port_attrs_snmp_tables.snmp_service_interface import (
     PortAttributesServiceInterface,
 )
 
@@ -14,15 +16,20 @@
         super().__init__(snmp_service, logger)
         self._snmp = snmp_service
         self._logger = logger
         self._auto_negotiation = {}
         self._snmp_auto_negotiation = {}
 
     def load_snmp_table(self):
-        self._snmp_auto_negotiation = self._snmp.get_table(port_constants.PORT_AUTO_NEG)
+        try:
+            table = self._snmp.get_table(port_constants.PORT_AUTO_NEG)
+        except RequestTimedOut:
+            self._logger.error(f"Failed to load {port_constants.PORT_AUTO_NEG} table")
+            table = {}
+        self._snmp_auto_negotiation = table
         if self._snmp_auto_negotiation:
             thread = Thread(
                 target=self._convert_auto_neg_table, name="Auto Negotiation converter"
             )
             thread.start()
             self._thread_list.append(thread)
```

## Comparing `cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/port_snmp_data.py` & `cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/port_snmp_data.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/test_snmp_if_table.py` & `cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/snmp/test_snmp_if_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from unittest.mock import Mock
 
 import pytest
 
 from cloudshell.shell.standards.networking.autoload_model import NetworkingResourceModel
 
+from .port_snmp_data import PORT_SNMP_DATA
+
 from cloudshell.snmp.autoload.services.port_table import PortsTable
 from cloudshell.snmp.autoload.snmp.tables.snmp_ports_table import SnmpPortsTable
 
-from tests.cloudshell.snmp.port_snmp_data import PORT_SNMP_DATA
-
 API = Mock(
     DecryptPassword=lambda x: Mock(Value=x),
     GetResourceDetails=lambda x: Mock(UniqueIdentifier="uniq id", ChildResources=[]),
 )
 
 
 @pytest.mark.parametrize(
```

## Comparing `cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_port_helper.py` & `cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_port_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_entity_helper.py` & `cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_entity_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from unittest.mock import Mock, create_autospec
 
 from cloudshell.snmp.autoload.constants.entity_constants import (
     CHASSIS_MATCH_PATTERN,
+    ENTITY_CLASS,
+    ENTITY_VENDOR_TYPE,
     ENTITY_VENDOR_TYPE_TO_CLASS_MAP,
 )
 from cloudshell.snmp.autoload.helper.entity_helper import EntityHelper
 from cloudshell.snmp.autoload.snmp.entities.snmp_entity_base import BaseEntity
 
 """
 Code Analysis:
@@ -59,56 +61,79 @@
         result = EntityHelper().get_physical_class(entity)
 
         # Assert
         assert result == "chassis"
 
     def test_get_physical_class_entity_class_not_defined(self):
         # Arrange
-        entity = create_autospec(BaseEntity)
-        entity.entity_class = ""
         expected_result = "chassis"
-        entity.vendor_type = f"UnknownDevice{expected_result.title()}"
+        entity = BaseEntity(
+            "1",
+            {
+                ENTITY_VENDOR_TYPE.object_name: Mock(
+                    safe_value=f"UnknownDevice{expected_result.title()}"
+                ),
+                ENTITY_CLASS.object_name: Mock(safe_value=""),
+            },
+        )
+        expected_result = "chassis"
 
         # Act
         result = EntityHelper().get_physical_class(entity)
 
         # Assert
         assert result == expected_result
 
     def test_get_physical_class_entity_class_is_other(self):
         # Arrange
         expected_result = "module"
-        entity = create_autospec(BaseEntity)
-        entity.entity_class = "other"
-        entity.vendor_type = f"UnknownDevice{expected_result.title()}"
+        entity = BaseEntity(
+            "1",
+            {
+                ENTITY_VENDOR_TYPE.object_name: Mock(
+                    safe_value=f"UnknownDevice{expected_result.title()}"
+                ),
+                ENTITY_CLASS.object_name: Mock(safe_value="other"),
+            },
+        )
 
         # Act
         result = EntityHelper().get_physical_class(entity)
 
         # Assert
         assert result == expected_result
 
     def test_get_physical_class_entity_vendor_type_does_not_match_known_physical_class(
         self,
     ):
         # Arrange
         expected_result = ""
-        entity = create_autospec(BaseEntity)
-        entity.entity_class = ""
-        entity.vendor_type = f"UnknownDevice{expected_result.title()}"
+        entity = BaseEntity(
+            "1",
+            {
+                ENTITY_VENDOR_TYPE.object_name: Mock(safe_value="UnknownDevice"),
+                ENTITY_CLASS.object_name: Mock(safe_value=""),
+            },
+        )
 
         # Act
         result = EntityHelper().get_physical_class(entity)
 
         # Assert
-        assert result == entity.entity_class
+        assert result == expected_result
 
     def test_get_physical_class_entity_vendor_type_matches_known_physical_class(self):
         # Arrange
-        entity = Mock(spec=BaseEntity, vendor_type="cevChassis", entity_class="")
+        entity = BaseEntity(
+            "1",
+            {
+                ENTITY_VENDOR_TYPE.object_name: Mock(safe_value="cevChassis"),
+                ENTITY_CLASS.object_name: Mock(safe_value=""),
+            },
+        )
 
         # Act
         result = EntityHelper().get_physical_class(entity)
 
         # Assert
         assert result == ENTITY_VENDOR_TYPE_TO_CLASS_MAP[CHASSIS_MATCH_PATTERN]
 
@@ -124,14 +149,20 @@
         # Assert
         assert result == entity.entity_class
 
     def test_get_phys_cl_physical_class_cannot_be_determined(
         self,
     ):
         # Arrange
-        entity = Mock(spec=BaseEntity, vendor_type="cevUnknown", entity_class="")
+        entity = BaseEntity(
+            "1",
+            {
+                ENTITY_VENDOR_TYPE.object_name: Mock(safe_value="cevUnknown"),
+                ENTITY_CLASS.object_name: Mock(safe_value=""),
+            },
+        )
 
         # Act
         result = EntityHelper().get_physical_class(entity)
 
         # Assert
         assert result == ""
```

## Comparing `cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_module_helper.py` & `cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_module_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py` & `cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/helper/test_int_module_helper.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/if_port_data.py` & `cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/if_port_data.py`

 * *Files identical despite different names*

## Comparing `cloudshell-snmp-autoload-2.0.1/tests/cloudshell/snmp/autoload/data/physical_entities_data.py` & `cloudshell-snmp-autoload-2.1.0/tests/cloudshell/snmp/autoload/data/physical_entities_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 MOCK_BAD_CHASSIS_SNMP_RESPONSE = {
     "1": {
         "entPhysicalParentRelPos": Mock(safe_value="-1"),
         "entPhysicalDescr": Mock(
             safe_value="Cisco 2500 Series Wireless LAN Controller"
         ),
         "entPhysicalName": Mock(safe_value="Chassis"),
-        "entPhysicalContainedIn": Mock(safe_value="4015"),
+        "entPhysicalContainedIn": Mock(safe_value="-1"),
         "entPhysicalClass": Mock(safe_value=""),
         "entPhysicalVendorType": Mock(safe_value=""),
         "entPhysicalModelName": Mock(safe_value="AIR-CT2504-K9"),
         "entPhysicalSerialNum": Mock(safe_value="PSZ19201CDR"),
         "entPhysicalSoftwareRev": Mock(safe_value="8.2.100.0"),
         "entPhysicalHardwareRev": Mock(safe_value=""),
     },
```

