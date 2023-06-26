# Comparing `tmp/pan_analyzer-0.0.3.6.tar.gz` & `tmp/pan_analyzer-0.0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pan_analyzer-0.0.3.6.tar", last modified: Fri Mar 31 17:40:16 2023, max compression
+gzip compressed data, was "pan_analyzer-0.0.3.8.tar", last modified: Mon Jun 26 11:40:33 2023, max compression
```

## Comparing `pan_analyzer-0.0.3.6.tar` & `pan_analyzer-0.0.3.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:16.434026 pan_analyzer-0.0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-03-31 17:40:16.434026 pan_analyzer-0.0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 17:40:16.434026 pan_analyzer-0.0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:16.422025 pan_analyzer-0.0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:16.422025 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:16.422025 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/consolidate_equivalent_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/delete_disabled_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/delete_unused_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/disable_shadowed_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/fix_UnqualifiedFQDN.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/fix_bad_log_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/remove_redundant_rule_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/remove_redundant_rule_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/rename_unconventional_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/replace_ips_with_resolving_fqdns.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/pan_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/pan_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/pan_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:16.426025 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_categorization_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_delete_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_disable_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_dump_active_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_zone_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:16.430025 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/bad_group_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/bad_hostnames.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/bad_log_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/consolidatable_addresses_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/consolidatable_service_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/disabled_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/equivalent_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/fqdn_contains_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/group_replacements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/ip_with_resolving_fqdn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/misleading_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/redundant_rule_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/rules_missing_security_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/shadowing_addresses_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/shadowing_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/shadowing_services_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/similar_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/superseding_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unconventionally_named_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unqualified_fqdn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unused_addresses_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unused_security_profile_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unused_services_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    19922 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/zone_based_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:16.430025 pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-03-31 17:40:16.000000 pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-03-31 17:40:16.000000 pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 17:40:16.000000 pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-31 17:40:16.000000 pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-31 17:40:16.000000 pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-31 17:40:16.000000 pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 17:40:16.434026 pan_analyzer-0.0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_AddressesShouldBeGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_BadGroupProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_BadHostname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_BadLogSetting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_EquivalentObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_ExtraRules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_ExtraZones.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_FQDNContainsIP.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_FindConsolidatableAddressesAndGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_FindConsolidatableServicesAndGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_IPWithResolvingFQDN.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_MisleadingAddresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_MisleadingServices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_MissingZones.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_RedundantRuleMembers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_RedundantRuleServices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_RulesMissingSecurityProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_ServicesShouldBeGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_ShadowingAddressesAndGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_ShadowingObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_ShadowingRules.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_SimilarAddressesAndGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_SimilarServicesAndGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_SupersedingRules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_UnconventionallyNamedServices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_UnqualifiedFQDN.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_UnusedAddressesAndGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_UnusedSecurityProfileGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-03-31 17:40:07.000000 pan_analyzer-0.0.3.6/tests/test_UnusedServices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:33.098581 pan_analyzer-0.0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-06-26 11:40:33.098581 pan_analyzer-0.0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 11:40:33.098581 pan_analyzer-0.0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:33.078581 pan_analyzer-0.0.3.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:33.078581 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:33.082581 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/consolidate_equivalent_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/delete_disabled_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/delete_unused_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/disable_shadowed_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/fix_UnqualifiedFQDN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/fix_bad_log_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/remove_redundant_rule_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/remove_redundant_rule_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/rename_unconventional_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/replace_ips_with_resolving_fqdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/pan_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9555 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/pan_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/pan_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:33.082581 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8873 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_categorization_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_delete_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_disable_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_dump_active_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_zone_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:33.090581 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/bad_group_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/bad_hostnames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/bad_log_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/consolidatable_addresses_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/consolidatable_service_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/disabled_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/equivalent_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/fqdn_contains_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/group_replacements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/ip_with_resolving_fqdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/misleading_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/redundant_rule_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/rules_missing_security_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/shadowing_addresses_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/shadowing_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/shadowing_services_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/similar_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/superseding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unconventionally_named_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unqualified_fqdn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unused_addresses_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unused_security_profile_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unused_services_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19922 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/zone_based_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:33.090581 pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-06-26 11:40:33.000000 pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-26 11:40:33.000000 pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 11:40:33.000000 pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-26 11:40:33.000000 pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 11:40:33.000000 pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-26 11:40:33.000000 pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 11:40:33.098581 pan_analyzer-0.0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_AddressesShouldBeGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_BadGroupProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_BadHostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_BadLogSetting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_EquivalentObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_ExtraRules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_ExtraZones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_FQDNContainsIP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_FindConsolidatableAddressesAndGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_FindConsolidatableServicesAndGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_IPWithResolvingFQDN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_MisleadingAddresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_MisleadingServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_MissingZones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_RedundantRuleMembers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_RedundantRuleServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_RulesMissingSecurityProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_ServicesShouldBeGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_ShadowingAddressesAndGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_ShadowingObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4692 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_ShadowingRules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_SimilarAddressesAndGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_SimilarServicesAndGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_SupersedingRules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_UnconventionallyNamedServices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_UnqualifiedFQDN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_UnusedAddressesAndGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_UnusedSecurityProfileGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-06-26 11:40:18.000000 pan_analyzer-0.0.3.8/tests/test_UnusedServices.py
```

### Comparing `pan_analyzer-0.0.3.6/LICENSE` & `pan_analyzer-0.0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/PKG-INFO` & `pan_analyzer-0.0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan_analyzer
-Version: 0.0.3.6
+Version: 0.0.3.8
 Summary: Detect and remediate configuration issues in Palo Alto Networks firewalls
 Author-email: Moshe Kaplan <me@moshekaplan.com>
 License: CC0 1.0 Universal
         
         Statement of Purpose
         
         The laws of most jurisdictions throughout the world automatically confer
```

### Comparing `pan_analyzer-0.0.3.6/README.md` & `pan_analyzer-0.0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/pyproject.toml` & `pan_analyzer-0.0.3.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pan_analyzer"
-version = "0.0.3.6"
+version = "0.0.3.8"
 authors = [
   { name="Moshe Kaplan", email="me@moshekaplan.com" },
 ]
 description = "Detect and remediate configuration issues in Palo Alto Networks firewalls"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
```

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/core.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/core.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/consolidate_equivalent_objects.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/consolidate_equivalent_objects.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/delete_disabled_policies.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/delete_disabled_policies.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/delete_unused_objects.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/delete_unused_objects.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/disable_shadowed_rules.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/disable_shadowed_rules.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/fix_UnqualifiedFQDN.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/fix_UnqualifiedFQDN.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/fix_bad_log_setting.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/fix_bad_log_setting.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/remove_redundant_rule_addresses.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/remove_redundant_rule_addresses.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/remove_redundant_rule_services.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/remove_redundant_rule_services.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/rename_unconventional_objects.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/rename_unconventional_objects.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/fixers/replace_ips_with_resolving_fqdns.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/fixers/replace_ips_with_resolving_fqdns.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/pan_api.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/pan_api.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/pan_config.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/pan_config.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/pan_helpers.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/pan_helpers.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_analyzer.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_analyzer.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_categorization_lookup.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_categorization_lookup.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_delete_addresses.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_delete_addresses.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_disable_rules.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_disable_rules.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_dump_active_sessions.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_dump_active_sessions.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_run_command.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_run_command.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/scripts/pan_zone_lookup.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/scripts/pan_zone_lookup.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/__init__.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/bad_group_profile.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/bad_group_profile.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/bad_hostnames.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/bad_hostnames.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/bad_log_setting.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/bad_log_setting.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/consolidatable_addresses_and_groups.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/consolidatable_addresses_and_groups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/consolidatable_service_and_groups.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/consolidatable_service_and_groups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/disabled_policies.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/disabled_policies.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/equivalent_objects.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/equivalent_objects.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/fqdn_contains_ip.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/fqdn_contains_ip.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/group_replacements.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/group_replacements.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/ip_with_resolving_fqdn.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/ip_with_resolving_fqdn.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/misleading_objects.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/misleading_objects.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,17 @@
                 continue
 
             entry_value = address_dict['entry'][entry_type]
 
             # The exact strategy will depend on the content type
             # For FQDNs, the domain should be present in the name
             if entry_type == 'fqdn':
-                if entry_value.lower().split('.', 1)[0] not in entry_name.lower():
+                # FQDNs can be up to 255 characters, but names are limited to 63 characters
+                # As such, skip FQDNs that are 63 or more characters, to avoid false positives
+                if len(entry_value) < 63 and entry_value.lower().split('.', 1)[0] not in entry_name.lower():
                     text = f"Device Group {device_group}'s Address {entry_name} has a misleading value of {entry_value}, because the FQDN's domain is not present in the name"
                     badentries.append(BadEntry(data=address_entry, text=text, device_group=device_group, entry_type='Addresses'))
             # For IPs, the IP should be present in the name, if the name 'looks' like it contains an IP (based on regex):
             elif entry_type == 'ip-netmask':
                 # This can optionally include a '/'
                 ip_address = entry_value.split('/', 1)[0]
                 if ip_address not in entry_name and re.search(IP_REGEX, entry_name) is not None:
```

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/redundant_rule_members.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/redundant_rule_members.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/rules_missing_security_profile.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/rules_missing_security_profile.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/shadowing_addresses_and_groups.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/shadowing_addresses_and_groups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/shadowing_rules.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/shadowing_rules.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/shadowing_services_and_groups.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/shadowing_services_and_groups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/similar_objects.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/similar_objects.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/superseding_rules.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/superseding_rules.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unconventionally_named_objects.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unconventionally_named_objects.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unqualified_fqdn.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unqualified_fqdn.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unused_addresses_and_groups.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unused_addresses_and_groups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unused_security_profile_groups.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unused_security_profile_groups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/unused_services_and_groups.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/unused_services_and_groups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/palo_alto_firewall_analyzer/validators/zone_based_checks.py` & `pan_analyzer-0.0.3.8/src/palo_alto_firewall_analyzer/validators/zone_based_checks.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/PKG-INFO` & `pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pan-analyzer
-Version: 0.0.3.6
+Version: 0.0.3.8
 Summary: Detect and remediate configuration issues in Palo Alto Networks firewalls
 Author-email: Moshe Kaplan <me@moshekaplan.com>
 License: CC0 1.0 Universal
         
         Statement of Purpose
         
         The laws of most jurisdictions throughout the world automatically confer
```

### Comparing `pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/SOURCES.txt` & `pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/src/pan_analyzer.egg-info/entry_points.txt` & `pan_analyzer-0.0.3.8/src/pan_analyzer.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_AddressesShouldBeGroups.py` & `pan_analyzer-0.0.3.8/tests/test_AddressesShouldBeGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_BadGroupProfile.py` & `pan_analyzer-0.0.3.8/tests/test_BadGroupProfile.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_BadHostname.py` & `pan_analyzer-0.0.3.8/tests/test_BadHostname.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_BadLogSetting.py` & `pan_analyzer-0.0.3.8/tests/test_BadLogSetting.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_EquivalentObjects.py` & `pan_analyzer-0.0.3.8/tests/test_EquivalentObjects.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_ExtraRules.py` & `pan_analyzer-0.0.3.8/tests/test_ExtraRules.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_ExtraZones.py` & `pan_analyzer-0.0.3.8/tests/test_ExtraZones.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_FQDNContainsIP.py` & `pan_analyzer-0.0.3.8/tests/test_FQDNContainsIP.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_FindConsolidatableAddressesAndGroups.py` & `pan_analyzer-0.0.3.8/tests/test_FindConsolidatableAddressesAndGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_FindConsolidatableServicesAndGroups.py` & `pan_analyzer-0.0.3.8/tests/test_FindConsolidatableServicesAndGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_IPWithResolvingFQDN.py` & `pan_analyzer-0.0.3.8/tests/test_IPWithResolvingFQDN.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_MisleadingAddresses.py` & `pan_analyzer-0.0.3.8/tests/test_MisleadingAddresses.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_MisleadingServices.py` & `pan_analyzer-0.0.3.8/tests/test_MisleadingServices.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_MissingZones.py` & `pan_analyzer-0.0.3.8/tests/test_MissingZones.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_RedundantRuleMembers.py` & `pan_analyzer-0.0.3.8/tests/test_RedundantRuleMembers.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_RedundantRuleServices.py` & `pan_analyzer-0.0.3.8/tests/test_RedundantRuleServices.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_RulesMissingSecurityProfile.py` & `pan_analyzer-0.0.3.8/tests/test_RulesMissingSecurityProfile.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_ServicesShouldBeGroups.py` & `pan_analyzer-0.0.3.8/tests/test_ServicesShouldBeGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_ShadowingAddressesAndGroups.py` & `pan_analyzer-0.0.3.8/tests/test_ShadowingAddressesAndGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_ShadowingObjects.py` & `pan_analyzer-0.0.3.8/tests/test_ShadowingObjects.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_ShadowingRules.py` & `pan_analyzer-0.0.3.8/tests/test_ShadowingRules.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_SimilarAddressesAndGroups.py` & `pan_analyzer-0.0.3.8/tests/test_SimilarAddressesAndGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_SimilarServicesAndGroups.py` & `pan_analyzer-0.0.3.8/tests/test_SimilarServicesAndGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_SupersedingRules.py` & `pan_analyzer-0.0.3.8/tests/test_SupersedingRules.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_UnconventionallyNamedServices.py` & `pan_analyzer-0.0.3.8/tests/test_UnconventionallyNamedServices.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_UnqualifiedFQDN.py` & `pan_analyzer-0.0.3.8/tests/test_UnqualifiedFQDN.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_UnusedAddressesAndGroups.py` & `pan_analyzer-0.0.3.8/tests/test_UnusedAddressesAndGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_UnusedSecurityProfileGroups.py` & `pan_analyzer-0.0.3.8/tests/test_UnusedSecurityProfileGroups.py`

 * *Files identical despite different names*

### Comparing `pan_analyzer-0.0.3.6/tests/test_UnusedServices.py` & `pan_analyzer-0.0.3.8/tests/test_UnusedServices.py`

 * *Files identical despite different names*

