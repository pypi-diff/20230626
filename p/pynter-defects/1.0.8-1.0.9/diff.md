# Comparing `tmp/pynter-defects-1.0.8.tar.gz` & `tmp/pynter-defects-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynter-defects-1.0.8.tar", last modified: Tue Jun 20 15:23:26 2023, max compression
+gzip compressed data, was "pynter-defects-1.0.9.tar", last modified: Tue Jun 20 15:39:02 2023, max compression
```

## Comparing `pynter-defects-1.0.8.tar` & `pynter-defects-1.0.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/automations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/automations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/automations/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/automations/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/defects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/hpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/inputs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/materials_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/phase_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/config_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.567437 pynter-defects-1.0.8/pynter/data/database/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/database/creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/database/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    29513 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/data/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/defects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45918 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/defects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/elasticity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/defects/pmg/
--rwxr-xr-x   0 runner    (1001) docker     (123)    24611 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    39163 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    60074 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39933 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/pmg/pmg_dos.py
--rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    19877 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/phase_diagram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/phase_diagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/phase_diagram/chempots.py
--rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/phase_diagram/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/phase_diagram/thermodynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/slurm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/slurm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/slurm/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/slurm/job_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/slurm/job_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/defects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/phase_diagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/testing/vasp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.571437 pynter-defects-1.0.8/pynter/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/materials_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/pynter/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/default_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/pynter/vasp/pmg/
--rw-r--r--   0 runner    (1001) docker     (123)   183623 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-06-20 15:23:16.000000 pynter-defects-1.0.8/pynter/vasp/schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 15:23:17.000000 pynter-defects-1.0.8/pynter/vasp/vasp_default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/pynter_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:23:26.000000 pynter-defects-1.0.8/pynter_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:23:26.575437 pynter-defects-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-20 15:23:17.000000 pynter-defects-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.982175 pynter-defects-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 15:39:02.982175 pynter-defects-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.974175 pynter-defects-1.0.9/pynter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.974175 pynter-defects-1.0.9/pynter/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/automations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/automations/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20887 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/automations/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7007 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17275 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/hpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/inputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/phase_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/config_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/data/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/data/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/data/database/creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/data/database/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29513 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/data/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45918 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/elasticity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/defects/pmg/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24611 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/pmg/pmg_defects_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39163 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/pmg/pmg_defects_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60074 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/pmg/pmg_defects_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39933 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/pmg/pmg_dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12053 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19877 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/phase_diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/phase_diagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32437 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/phase_diagram/chempots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/phase_diagram/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/phase_diagram/thermodynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/slurm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/slurm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/slurm/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10376 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/slurm/job_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/slurm/job_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/testing/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/testing/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/testing/defects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/testing/phase_diagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/testing/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/testing/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/testing/vasp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.978175 pynter-defects-1.0.9/pynter/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/tools/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/tools/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/tools/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/tools/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.982175 pynter-defects-1.0.9/pynter/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/vasp/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/vasp/default_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36606 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/vasp/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/vasp/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.982175 pynter-defects-1.0.9/pynter/vasp/pmg/
+-rw-r--r--   0 runner    (1001) docker     (123)   183623 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/vasp/pmg/pmg_electronic_structure_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51327 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/vasp/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/pynter/vasp/vasp_default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:39:02.982175 pynter-defects-1.0.9/pynter_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-20 15:39:02.000000 pynter-defects-1.0.9/pynter_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-20 15:39:02.000000 pynter-defects-1.0.9/pynter_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:39:02.000000 pynter-defects-1.0.9/pynter_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 15:39:02.000000 pynter-defects-1.0.9/pynter_defects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-20 15:39:02.000000 pynter-defects-1.0.9/pynter_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:39:02.000000 pynter-defects-1.0.9/pynter_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:39:02.982175 pynter-defects-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-20 15:38:52.000000 pynter-defects-1.0.9/setup.py
```

### Comparing `pynter-defects-1.0.8/PKG-INFO` & `pynter-defects-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynter-defects
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tools for atomistic calculations, provides features for point-defect calculations with VASP
 Author: Lorenzo Villa
 Description-Content-Type: text/markdown
 
 # pynter
 Tools for atomistic calculations. Uses pymatgen package (https://pymatgen.org). The main features are designed to systematically run, analyse and plot DFT point defect calculations with VASP.
```

### Comparing `pynter-defects-1.0.8/README.md` & `pynter-defects-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/__init__.py` & `pynter-defects-1.0.9/pynter/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/automations/core.py` & `pynter-defects-1.0.9/pynter/automations/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/automations/vasp.py` & `pynter-defects-1.0.9/pynter/automations/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/analysis.py` & `pynter-defects-1.0.9/pynter/cli/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/automations.py` & `pynter-defects-1.0.9/pynter/cli/automations.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/config.py` & `pynter-defects-1.0.9/pynter/cli/config.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/defects.py` & `pynter-defects-1.0.9/pynter/cli/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/hpc.py` & `pynter-defects-1.0.9/pynter/cli/hpc.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/inputs.py` & `pynter-defects-1.0.9/pynter/cli/inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/main.py` & `pynter-defects-1.0.9/pynter/cli/main.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/materials_project.py` & `pynter-defects-1.0.9/pynter/cli/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/phase_diagram.py` & `pynter-defects-1.0.9/pynter/cli/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/plotter.py` & `pynter-defects-1.0.9/pynter/cli/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/slurm.py` & `pynter-defects-1.0.9/pynter/cli/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/cli/utils.py` & `pynter-defects-1.0.9/pynter/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/config_default.yml` & `pynter-defects-1.0.9/pynter/config_default.yml`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/data/database/creator.py` & `pynter-defects-1.0.9/pynter/data/database/creator.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/data/database/query.py` & `pynter-defects-1.0.9/pynter/data/database/query.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/data/datasets.py` & `pynter-defects-1.0.9/pynter/data/datasets.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/data/jobs.py` & `pynter-defects-1.0.9/pynter/data/jobs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/analysis.py` & `pynter-defects-1.0.9/pynter/defects/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/corrections.py` & `pynter-defects-1.0.9/pynter/defects/corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/defects.py` & `pynter-defects-1.0.9/pynter/defects/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/elasticity.py` & `pynter-defects-1.0.9/pynter/defects/elasticity.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/entries.py` & `pynter-defects-1.0.9/pynter/defects/entries.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/plotter.py` & `pynter-defects-1.0.9/pynter/defects/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_core.py` & `pynter-defects-1.0.9/pynter/defects/pmg/pmg_defects_core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_corrections.py` & `pynter-defects-1.0.9/pynter/defects/pmg/pmg_defects_corrections.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/pmg/pmg_defects_utils.py` & `pynter-defects-1.0.9/pynter/defects/pmg/pmg_defects_utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/pmg/pmg_dos.py` & `pynter-defects-1.0.9/pynter/defects/pmg/pmg_dos.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/structure.py` & `pynter-defects-1.0.9/pynter/defects/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/thermodynamics.py` & `pynter-defects-1.0.9/pynter/defects/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/defects/utils.py` & `pynter-defects-1.0.9/pynter/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/phase_diagram/chempots.py` & `pynter-defects-1.0.9/pynter/phase_diagram/chempots.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/phase_diagram/plotter.py` & `pynter-defects-1.0.9/pynter/phase_diagram/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/phase_diagram/thermodynamics.py` & `pynter-defects-1.0.9/pynter/phase_diagram/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/slurm/interface.py` & `pynter-defects-1.0.9/pynter/slurm/interface.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/slurm/job_script.py` & `pynter-defects-1.0.9/pynter/slurm/job_script.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/slurm/job_status.py` & `pynter-defects-1.0.9/pynter/slurm/job_status.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/testing/__init__.py` & `pynter-defects-1.0.9/pynter/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/testing/core.py` & `pynter-defects-1.0.9/pynter/testing/core.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/testing/data.py` & `pynter-defects-1.0.9/pynter/testing/data.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/testing/defects.py` & `pynter-defects-1.0.9/pynter/testing/defects.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/testing/phase_diagram.py` & `pynter-defects-1.0.9/pynter/testing/phase_diagram.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/testing/slurm.py` & `pynter-defects-1.0.9/pynter/testing/slurm.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/testing/structure.py` & `pynter-defects-1.0.9/pynter/testing/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/testing/vasp.py` & `pynter-defects-1.0.9/pynter/testing/vasp.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/tools/format.py` & `pynter-defects-1.0.9/pynter/tools/format.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/tools/materials_project.py` & `pynter-defects-1.0.9/pynter/tools/materials_project.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/tools/structure.py` & `pynter-defects-1.0.9/pynter/tools/structure.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/tools/utils.py` & `pynter-defects-1.0.9/pynter/tools/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     PhaseDiagram object.
 
     """
     if op.isfile(path_or_string):
         with open(path_or_string) as file:
             d = json.load(file)
     else:
-        d = json.load(path_or_string)
+        d = json.loads(path_or_string)
 
     return cls.from_dict(d)
 
 
 def save_object_as_json(object,path,sanitize=False,cls=MontyEncoder):
     """
     Save class object as json string or file. The class must posses the 'as_dict' method.
```

### Comparing `pynter-defects-1.0.8/pynter/vasp/analysis.py` & `pynter-defects-1.0.9/pynter/vasp/analysis.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/vasp/default_inputs.py` & `pynter-defects-1.0.9/pynter/vasp/default_inputs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/vasp/jobs.py` & `pynter-defects-1.0.9/pynter/vasp/jobs.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/vasp/plotter.py` & `pynter-defects-1.0.9/pynter/vasp/plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/vasp/pmg/pmg_electronic_structure_plotter.py` & `pynter-defects-1.0.9/pynter/vasp/pmg/pmg_electronic_structure_plotter.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/vasp/schemes.py` & `pynter-defects-1.0.9/pynter/vasp/schemes.py`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter/vasp/vasp_default.yml` & `pynter-defects-1.0.9/pynter/vasp/vasp_default.yml`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/pynter_defects.egg-info/PKG-INFO` & `pynter-defects-1.0.9/pynter_defects.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynter-defects
-Version: 1.0.8
+Version: 1.0.9
 Summary: Tools for atomistic calculations, provides features for point-defect calculations with VASP
 Author: Lorenzo Villa
 Description-Content-Type: text/markdown
 
 # pynter
 Tools for atomistic calculations. Uses pymatgen package (https://pymatgen.org). The main features are designed to systematically run, analyse and plot DFT point defect calculations with VASP.
```

### Comparing `pynter-defects-1.0.8/pynter_defects.egg-info/SOURCES.txt` & `pynter-defects-1.0.9/pynter_defects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynter-defects-1.0.8/setup.py` & `pynter-defects-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md") as file:
     long_description = file.read()
 
 setup(
     name='pynter-defects',
-    version='1.0.8',
+    version='1.0.9',
     author='Lorenzo Villa',
     description='Tools for atomistic calculations, provides features for point-defect calculations with VASP',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_namespace_packages(exclude=["pynter.*.tests", "pynter.*.*.tests"]),
     install_requires=[
         'ase',
```

