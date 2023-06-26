# Comparing `tmp/open-prime-rando-0.8.0.tar.gz` & `tmp/open-prime-rando-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-prime-rando-0.8.0.tar", last modified: Sun Jun 25 17:27:49 2023, max compression
+gzip compressed data, was "open-prime-rando-0.9.0.tar", last modified: Mon Jun 26 08:24:27 2023, max compression
```

## Comparing `open-prime-rando-0.8.0.tar` & `open-prime-rando-0.9.0.tar`

### file list

```diff
@@ -1,123 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.676555 open-prime-rando-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.676555 open-prime-rando-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-25 17:27:49.696555 open-prime-rando-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.672555 open-prime-rando-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.676555 open-prime-rando-0.8.0/src/open_prime_rando/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/all_prime_dol_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/dol_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/beam_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/user_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.680554 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/dynamic_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.684555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.684555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/agon_wastes.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/great_temple.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m02_spires.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m04_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/temple_grounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/torvus_bog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.672555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.688555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst_emissive.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor_emissive.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack_emissive.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.688555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.688555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27306 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.688555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/elevator_rando.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/area_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/echo_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/rubiks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/specific_area_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes/vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/echoes_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/p1r_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/src/open_prime_rando/prime_remastered/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/prime_remastered/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/unique_area_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/src/open_prime_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.676555 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-25 17:27:49.000000 open-prime-rando-0.8.0/src/open_prime_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/tests/dol_patching/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/test_all_prime_dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/test_dol_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/test_echoes_dol_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/dol_patching/test_echoes_dol_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/tests/echoes/
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/echoes/test_echoes_dock_lock_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tests/test_echoes_custom_Assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:27:49.692555 open-prime-rando-0.8.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-25 17:27:32.000000 open-prime-rando-0.8.0/tools/asset_id_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.920370 open-prime-rando-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.920370 open-prime-rando-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.920370 open-prime-rando-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.924370 open-prime-rando-0.9.0/src/open_prime_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.924370 open-prime-rando-0.9.0/src/open_prime_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.924370 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/all_prime_dol_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.924370 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/corruption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/corruption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/corruption/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/corruption/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/dol_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.924370 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/beam_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/dol_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/user_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.924370 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/prime1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/prime1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/prime1/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/prime1/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/dynamic_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.924370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.928370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/agon_wastes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/great_temple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/m02_spires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/m04_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/temple_grounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/torvus_bog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.920370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_boost_ball.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_boost_ball_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_cannon_ball.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_cannon_ball_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_charge_beam.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_charge_beam_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_dark_visor.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_dark_visor_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_morph_ball_bombs.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_morph_ball_bombs_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screw_attack.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screw_attack_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonic_boom.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonic_boom_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/rubiks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27534 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13393 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/elevators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/elevators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/elevators/elevator_rando.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/inverted/
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/inverted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/inverted/area_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/echo_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/rubiks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/specific_area_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes/vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/echoes_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/p1r_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/src/open_prime_rando/prime_remastered/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/prime_remastered/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/unique_area_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/src/open_prime_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 08:24:27.000000 open-prime-rando-0.9.0/src/open_prime_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.924370 open-prime-rando-0.9.0/src/open_prime_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-26 08:24:27.000000 open-prime-rando-0.9.0/src/open_prime_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-26 08:24:27.000000 open-prime-rando-0.9.0/src/open_prime_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:24:27.000000 open-prime-rando-0.9.0/src/open_prime_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 08:24:27.000000 open-prime-rando-0.9.0/src/open_prime_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-26 08:24:27.000000 open-prime-rando-0.9.0/src/open_prime_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 08:24:27.000000 open-prime-rando-0.9.0/src/open_prime_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/tests/dol_patching/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tests/dol_patching/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18393 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tests/dol_patching/test_all_prime_dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tests/dol_patching/test_dol_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tests/dol_patching/test_echoes_dol_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17804 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tests/dol_patching/test_echoes_dol_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/tests/echoes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tests/echoes/test_echoes_dock_lock_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tests/test_echoes_custom_Assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:24:27.932370 open-prime-rando-0.9.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tools/asset_id_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-26 08:24:16.000000 open-prime-rando-0.9.0/tools/draw_objects.py
```

### Comparing `open-prime-rando-0.8.0/.github/dependabot.yml` & `open-prime-rando-0.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/.github/workflows/python.yml` & `open-prime-rando-0.9.0/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/.gitignore` & `open-prime-rando-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/LICENSE` & `open-prime-rando-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/PKG-INFO` & `open-prime-rando-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.8.0
+Version: 0.9.0
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/randovania/open-prime-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `open-prime-rando-0.8.0/pyproject.toml` & `open-prime-rando-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/cli.py` & `open-prime-rando-0.9.0/src/open_prime_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/all_prime_dol_patches.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/all_prime_dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/corruption/dol_versions.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/corruption/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/dol_version.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/dol_version.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/beam_configuration.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/beam_configuration.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_patcher.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/dol_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_patches.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/dol_versions.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/echoes/user_preferences.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/echoes/user_preferences.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/dol_patches.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/prime1/dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dol_patching/prime1/dol_versions.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dol_patching/prime1/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/dynamic_schema.py` & `open-prime-rando-0.9.0/src/open_prime_rando/dynamic_schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import copy
 
 import open_prime_rando.echoes.asset_ids.world
 from open_prime_rando.patcher_editor import PatcherEditor
-from open_prime_rando.unique_area_name import get_name_for_area
 
 
 def expand_schema(base_schema: dict, editor: PatcherEditor) -> dict:
     schema = copy.deepcopy(base_schema)
 
     world_props = schema["properties"]["worlds"]["properties"] = {}
     for world, mlvl_id in open_prime_rando.echoes.asset_ids.world.NAME_TO_ID_MLVL.items():
@@ -14,17 +13,21 @@
         world_props[world] = world_def
 
         mlvl = editor.get_mlvl(mlvl_id)
         area_props = {}
         world_def["properties"]["areas"] = {"type": "object", "additionalProperties": False, "properties": area_props}
 
         world_details = open_prime_rando.echoes.asset_ids.world.load_dedicated_file(world)
+        mrea_to_name: dict[int, str] = {
+            mrea: name
+            for name, mrea in world_details.NAME_TO_ID_MREA.items()
+        }
 
         for area in mlvl.areas:
-            area_name = get_name_for_area(area)
+            area_name = mrea_to_name[area.mrea_asset_id]
             area_def = copy.deepcopy(schema["$defs"]["area"])
             area_props[area_name] = area_def
 
             area_def["properties"]["docks"] = {
                 "type": "object",
                 "properties": {
                     dock_name: {"$ref": "#/$defs/dock"}
```

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/agon_wastes.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/agon_wastes.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/great_temple.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/great_temple.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/temple_grounds.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/temple_grounds.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/torvus_bog.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/torvus_bog.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/asset_ids/world.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/asset_ids/world.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst_emissive.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst_emissive.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor_emissive.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor_emissive.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screw_attack.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack_emissive.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screw_attack_emissive.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/custom_assets.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/custom_assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/__init__.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,21 @@
             data=f.read_bytes()
         )
         return editor.add_file(n, res)
 
     greyscale_emissive = get_txtr("custom_door_lock_greyscale_emissive.TXTR")
     template = editor.get_parsed_asset(0xF115F575, type_hint=Cmdl)
 
-    for name in ("darkburst", "sunburst", "sonicboom", "screwattack", "echo_visor"):
+    for door_type in DOCK_TYPES.values():
+        if not (
+            isinstance(door_type, dock_type.BlastShieldDoorType)
+            and isinstance(door_type.shield_model, str)
+        ):
+            continue
+        name = door_type.shield_model
         txtr = get_txtr(f"custom_door_lock_{name}.TXTR")
         emissive = get_txtr(f"custom_door_lock_{name}_emissive.TXTR", must_exist=False)
         if emissive is None:
             emissive = greyscale_emissive
 
         cmdl = Container(template.raw)
         cmdl.material_sets[0].texture_file_ids[0] = txtr
```

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,18 @@
         memory relay connections:
             ACTV -> door, RSET
             ACTV -> blast shield, DCTV
         """
         super().patch_door(editor, world_name, area_name, dock_name, low_memory)
         area = self.get_area(editor, world_name, area_name)
         door = self.get_door_from_dock_index(area, self.get_dock_index(world_name, area_name, dock_name))
-        door_transform = door.get_properties_as(Door).editor_properties.transform
+
+        with door.edit_properties(Door) as _door:
+            door_transform = _door.editor_properties.transform
+            _door.vulnerability = resist_all_vuln
 
         default = area.get_layer("Default")
 
         sound = default.add_instance_with(Sound(
             editor_properties=EditorProperties(
                 name="Metal Door Lock Breaking",
                 transform=door_transform
@@ -262,15 +265,19 @@
             song_file="/audio/evt_x_event_00.dsp",
             fade_in_time=0.01,
             volume=65,
             software_channel=1,
             unknown=False
         ))
 
-        model = editor._resolve_asset_id(self.shield_model)
+        shield_model = self.shield_model
+        if isinstance(shield_model, str):
+            shield_model = f"custom_door_lock_{shield_model}.CMDL"
+        model = editor._resolve_asset_id(shield_model)
+
         lock = default.add_instance_with(Actor(
             editor_properties=EditorProperties(
                 name=f"{self.name} Blast Shield Lock",
                 transform=door_transform
             ),
             collision_box=self.shield_collision_box,
             collision_offset=self.shield_collision_offset,
```

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -120,28 +120,28 @@
         shell_model=normal_door_model,
         shell_color=Color(0.93, 0.58, 0.83, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. The Screw Attack may damage it."
         ),
         map_icon=DoorMapIcon.ScrewAttack,
-        shield_model="custom_door_lock_screwattack.CMDL",
+        shield_model="screw_attack",
     ),
     "Bomb": dock_type.BlastShieldDoorType(
         name="Bomb",
         vulnerability=dataclasses.replace(resist_all_vuln, bomb=vulnerable),
         shell_model=normal_door_model,
         shell_color=Color(1/3, 1/3, 0.5, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A Morph Ball Bomb blast may damage it."
         ),
         map_icon=DoorMapIcon.Bomb,
-        shield_model="custom_door_lock_sonicboom.CMDL",
+        shield_model="morph_ball_bombs",
     ),
     "Boost": dock_type.BlastShieldDoorType(
         name="Boost",
         vulnerability=dataclasses.replace(
             resist_all_vuln,
             boost_ball=vulnerable,
             cannon_ball=vulnerable_no_splash
@@ -149,15 +149,15 @@
         shell_model=normal_door_model,
         shell_color=Color(1, 1/3, 0, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. The Boost Ball may damage it."
         ),
         map_icon=DoorMapIcon.Boost,
-        shield_model=0xBFB4A8EE,
+        shield_model="boost_ball",
     ),
     "Grapple": dock_type.GrappleDoorType(
         name="Grapple",
         vulnerability=resist_all_vuln,
         shell_model=annihilator_door_model,
         shell_color=Color(1, 0, 0, 1),
         scan_text=(
@@ -175,41 +175,41 @@
         shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A massive burst of dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Dark,
-        shield_model="custom_door_lock_darkburst.CMDL",
+        shield_model="darkburst",
     ),
     "Sunburst": dock_type.BlastShieldDoorType(
         name="Sunburst",
         vulnerability=dataclasses.replace(resist_all_vuln, sunburst=vulnerable),
         shell_model=normal_door_model,
         shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A massive burst of light energy may damage it."
         ),
         map_icon=DoorMapIcon.Light,
-        shield_model="custom_door_lock_sunburst.CMDL",
+        shield_model="sunburst",
     ),
     "SonicBoom": dock_type.BlastShieldDoorType(
         name="SonicBoom",
         vulnerability=dataclasses.replace(resist_all_vuln, imploder=vulnerable),
         shell_model=annihilator_door_model,
         shell_color=Color(1, 1, 1, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
             "A massive burst of light and dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Annihilator,
-        shield_model="custom_door_lock_sonicboom.CMDL",
+        shield_model="sonic_boom",
     ),
     "AgonEnergy": dock_type.PlanetaryEnergyDoorType(
         name="AgonEnergy",
         vulnerability=resist_all_vuln,
         shell_color=Color(0.64, 0.34, 0, 1),
         scan_text=(
             "There is a Luminoth barrier on the door blocking access. ",
@@ -245,31 +245,76 @@
     "EchoVisor": dock_type.EchoVisorDoorType(
         name="EchoVisor",
         vulnerability=normal_vuln,
         shell_model=dark_door_model,
         shell_color=Color(1/16, 1/16, 1/16, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Sonic detection gear needed to interface with this system."
+            "Sonic detection gear needed to interface with this system. "
             "Neutralizing the control emitter may disable it."
         ),
         map_icon=DoorMapIcon.EchoVisor,
-        shield_model="custom_door_lock_echo_visor.CMDL",
+        shield_model="echo_visor",
         visor_flags=VisorFlags.Echo,
         player_controller_proxy=8,
     ),
     "DarkVisor": dock_type.DarkVisorDoorType(
         name="DarkVisor",
         vulnerability=normal_vuln,
         shell_model=dark_door_model,
         shell_color=Color(1, 0, 0, 1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Scans indicate presence of a control system."
+            "Scans indicate presence of a control system. "
             "Interface method unknown. Control units not present in the visible spectrum or current timespace. "
         ),
         map_icon=DoorMapIcon.DarkVisor,
-        shield_model=0xBFB4A8EE,
+        shield_model="dark_visor",
         visor_flags=VisorFlags.Dark,
         player_controller_proxy=7,
+    ),
+    "Cannon": dock_type.BlastShieldDoorType(
+        name="Cannon",
+        vulnerability=dataclasses.replace(
+            resist_all_vuln,
+            cannon_ball=vulnerable_no_splash
+        ),
+        shell_model=normal_door_model,
+        shell_color=Color(1, 1/3, 0, 1),
+        scan_text=(
+            "There is a Blast Shield on the door blocking access. ",
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. The Cannon Ball may damage it."
+        ),
+        map_icon=DoorMapIcon.Boost,
+        shield_model="cannon_ball",
+    ),
+    "Charge": dock_type.BlastShieldDoorType(
+        name="Charge",
+        vulnerability=dataclasses.replace(
+            resist_all_vuln,
+            power_charge=vulnerable,
+            entangler=vulnerable,
+            light_blast=vulnerable,
+            sonic_boom=vulnerable,
+        ),
+        shell_model=normal_door_model,
+        shell_color=Color(0, 1, 1, 1),
+        scan_text=(
+            "There is a Blast Shield on the door blocing access. ",
+            "Analysis indicates that the Blast Shield is invulnerable to normal beam fire. "
+            "The Charge Beam may damage it."
+        ),
+        map_icon=DoorMapIcon.Normal,
+        shield_model="charge_beam"
+    ),
+    "Power": dock_type.NormalDoorType(
+        name="Power",
+        vulnerability=dataclasses.replace(resist_all_vuln, power=vulnerable),
+        shell_color=Color(1, 0.8, 0, 1),
+        scan_text=(
+            "There is a Blast Shield on the door blocking access. ",
+            "Analysis indicates that the Blast Shield is invulnerable to light and dark energy. "
+            "The Power Beam may damage it."
+        ),
+        map_icon=DoorMapIcon.PowerBomb # TODO: give it its own?
     )
 }
```

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/elevators/elevator_rando.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/elevators/elevator_rando.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/__init__.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/inverted/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/inverted/area_pairs.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/inverted/area_pairs.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/schema.json` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997395833333332%*

 * *Differences: {"'$defs'": "{'dock_type': {'enum': {insert: [(21, 'Cannon'), (22, 'Charge'), (23, 'Power')]}}}"}*

```diff
@@ -128,15 +128,18 @@
                 "Darkburst",
                 "Sunburst",
                 "SonicBoom",
                 "AgonEnergy",
                 "TorvusEnergy",
                 "SanctuaryEnergy",
                 "DarkVisor",
-                "EchoVisor"
+                "EchoVisor",
+                "Cannon",
+                "Charge",
+                "Power"
             ],
             "type": "string"
         },
         "world": {
             "$comment": "The list of areas is replaced in runtime with the existing areas of each specific world.",
             "additionalProperties": false,
             "properties": {
```

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/__init__.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/echo_locks.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/echo_locks.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/small_randomizations/rubiks.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/small_randomizations/rubiks.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/specific_area_patches.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/specific_area_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes/vulnerabilities.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/echoes_patcher.py` & `open-prime-rando-0.9.0/src/open_prime_rando/echoes_patcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from open_prime_rando import dynamic_schema
 from open_prime_rando.echoes import asset_ids, dock_lock_rando, specific_area_patches
 from open_prime_rando.echoes.elevators import auto_enabled_elevator_patches
 from open_prime_rando.echoes.elevators.elevator_rando import patch_elevator
 from open_prime_rando.echoes.inverted import apply_inverted
 from open_prime_rando.echoes.small_randomizations import apply_small_randomizations
 from open_prime_rando.patcher_editor import PatcherEditor
-from open_prime_rando.unique_area_name import get_name_for_area
 from open_prime_rando.validator_with_default import DefaultValidatingDraft7Validator
 
 LOG = logging.getLogger("echoes_patcher")
 
 
 def _read_schema():
     with Path(__file__).parent.joinpath("echoes", "schema.json").open() as f:
@@ -32,16 +31,21 @@
     num_areas = sum(len(world_config["areas"]) for world_config in configuration.values())
     areas_processed = 0.0
 
     for world_name, world_config in configuration.items():
         world_meta = asset_ids.world.load_dedicated_file(world_name)
         mlvl = editor.get_mlvl(asset_ids.world.NAME_TO_ID_MLVL[world_name])
 
+        mrea_to_name: dict[int, str] = {
+            mrea: name
+            for name, mrea in world_meta.NAME_TO_ID_MREA.items()
+        }
+
         areas_by_name: dict[str, Area] = {
-            get_name_for_area(area): area
+            mrea_to_name[area.mrea_asset_id]: area
             for area in mlvl.areas
         }
 
         for i, (area_name, area) in enumerate(areas_by_name.items()):
             if area_name not in world_config["areas"]:
                 continue
 
@@ -119,14 +123,15 @@
 
 
 def patch_paks(file_provider: FileProvider,
                output_path: Path,
                configuration: dict,
                status_update: Callable[[str, float], None] = lambda s, _: LOG.info(s)):
     status_update(f"Will patch files at {file_provider}", 0)
+    output_path.joinpath("files", "opr_patcher_data.json").write_text(json.dumps(configuration))
 
     editor = PatcherEditor(file_provider, Game.ECHOES)
 
     status_update("Preparing schema", 0)
     schema = dynamic_schema.expand_schema(_read_schema(), editor)
 
     status_update("Validating schema", 0)
```

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/p1r_patcher.py` & `open-prime-rando-0.9.0/src/open_prime_rando/p1r_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/patcher_editor.py` & `open-prime-rando-0.9.0/src/open_prime_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando/validator_with_default.py` & `open-prime-rando-0.9.0/src/open_prime_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando.egg-info/PKG-INFO` & `open-prime-rando-0.9.0/src/open_prime_rando.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.8.0
+Version: 0.9.0
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/randovania/open-prime-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `open-prime-rando-0.8.0/src/open_prime_rando.egg-info/SOURCES.txt` & `open-prime-rando-0.9.0/src/open_prime_rando.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -55,23 +55,35 @@
 src/open_prime_rando/echoes/asset_ids/m04_pipeline.py
 src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
 src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
 src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
 src/open_prime_rando/echoes/asset_ids/temple_grounds.py
 src/open_prime_rando/echoes/asset_ids/torvus_bog.py
 src/open_prime_rando/echoes/asset_ids/world.py
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_boost_ball.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_boost_ball_emissive.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_cannon_ball.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_cannon_ball_emissive.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_charge_beam.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_charge_beam_emissive.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_dark_visor.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_dark_visor_emissive.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst_emissive.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_echo_visor_emissive.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
-src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack.TXTR
-src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screwattack_emissive.TXTR
-src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_morph_ball_bombs.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_morph_ball_bombs_emissive.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screw_attack.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_screw_attack_emissive.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonic_boom.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonic_boom_emissive.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
+src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst_emissive.TXTR
 src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
 src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
 src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
 src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
 src/open_prime_rando/echoes/dock_lock_rando/__init__.py
 src/open_prime_rando/echoes/dock_lock_rando/dock_type.py
 src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
@@ -90,8 +102,9 @@
 tests/test_echoes_custom_Assets.py
 tests/dol_patching/conftest.py
 tests/dol_patching/test_all_prime_dol_patches.py
 tests/dol_patching/test_dol_version.py
 tests/dol_patching/test_echoes_dol_patcher.py
 tests/dol_patching/test_echoes_dol_patches.py
 tests/echoes/test_echoes_dock_lock_rando.py
-tools/asset_id_files.py
+tools/asset_id_files.py
+tools/draw_objects.py
```

### Comparing `open-prime-rando-0.8.0/tests/conftest.py` & `open-prime-rando-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/tests/dol_patching/conftest.py` & `open-prime-rando-0.9.0/tests/dol_patching/conftest.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/tests/dol_patching/test_all_prime_dol_patches.py` & `open-prime-rando-0.9.0/tests/dol_patching/test_all_prime_dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/tests/dol_patching/test_dol_version.py` & `open-prime-rando-0.9.0/tests/dol_patching/test_dol_version.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/tests/dol_patching/test_echoes_dol_patcher.py` & `open-prime-rando-0.9.0/tests/dol_patching/test_echoes_dol_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/tests/dol_patching/test_echoes_dol_patches.py` & `open-prime-rando-0.9.0/tests/dol_patching/test_echoes_dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/tests/test_echoes_custom_Assets.py` & `open-prime-rando-0.9.0/tests/test_echoes_custom_Assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.8.0/tools/asset_id_files.py` & `open-prime-rando-0.9.0/tools/asset_id_files.py`

 * *Files identical despite different names*

