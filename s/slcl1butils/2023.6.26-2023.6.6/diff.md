# Comparing `tmp/slcl1butils-2023.6.26.tar.gz` & `tmp/slcl1butils-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcl1butils-2023.6.26.tar", last modified: Mon Jun 26 14:28:24 2023, max compression
+gzip compressed data, was "slcl1butils-2023.6.6.tar", last modified: Tue Jun  6 07:44:42 2023, max compression
```

## Comparing `slcl1butils-2023.6.26.tar` & `slcl1butils-2023.6.6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.367036 slcl1butils-2023.6.26/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.359036 slcl1butils-2023.6.26/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.359036 slcl1butils-2023.6.26/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-26 14:28:24.367036 slcl1butils-2023.6.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.359036 slcl1butils-2023.6.26/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.363036 slcl1butils-2023.6.26/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.363036 slcl1butils-2023.6.26/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.359036 slcl1butils-2023.6.26/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.363036 slcl1butils-2023.6.26/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/_static/css/slcl1butils.css
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/atbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/cwave.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.363036 slcl1butils-2023.6.26/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/examples/display_a_IW_L1B_xspectra.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/get_polygons_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 14:28:24.367036 slcl1butils-2023.6.26/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.363036 slcl1butils-2023.6.26/slcl1butils/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.367036 slcl1butils-2023.6.26/slcl1butils/coloc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/coloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/coloc/coloc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.367036 slcl1butils-2023.6.26/slcl1butils/compute/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/compute/compute_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/compute/cwave.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/compute/macs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/compute/stack_iw_l1b.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/compute/stack_wv_l1c_monthly.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/conversion_polar_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/cwave_parameters_computation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/get_polygons_from_l1b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.367036 slcl1butils-2023.6.26/slcl1butils/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
--rw-r--r--   0 runner    (1001) docker     (123)    20529 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/plotting/display_one_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/plotting/display_xspectra_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/plotting/wallpaper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/raster_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.367036 slcl1butils-2023.6.26/slcl1butils/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3101 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/spectrum_clockwise_to_trigo.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/spectrum_rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/symmetrize_l1b_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-26 14:28:06.000000 slcl1butils-2023.6.26/slcl1butils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:28:24.363036 slcl1butils-2023.6.26/slcl1butils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-26 14:28:24.000000 slcl1butils-2023.6.26/slcl1butils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-26 14:28:24.000000 slcl1butils-2023.6.26/slcl1butils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:28:24.000000 slcl1butils-2023.6.26/slcl1butils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-26 14:28:24.000000 slcl1butils-2023.6.26/slcl1butils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-26 14:28:24.000000 slcl1butils-2023.6.26/slcl1butils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 14:28:24.000000 slcl1butils-2023.6.26/slcl1butils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.150562 slcl1butils-2023.6.6/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.154562 slcl1butils-2023.6.6/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/_static/css/slcl1butils.css
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/atbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/cwave.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/display_a_IW_L1B_xspectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    59687 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10438 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/get_polygons_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/slcl1butils/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/slcl1butils/coloc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/coloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/coloc/coloc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/slcl1butils/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/compute_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/cwave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/macs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/stack_iw_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/compute/stack_wv_l1c_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/conversion_polar_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/cwave_parameters_computation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/get_polygons_from_l1b.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/slcl1butils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/display_one_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/display_xspectra_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/plotting/wallpaper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.162562 slcl1butils-2023.6.6/slcl1butils/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    13169 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2435 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/spectrum_clockwise_to_trigo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/spectrum_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/symmetrize_l1b_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-06 07:44:26.000000 slcl1butils-2023.6.6/slcl1butils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:44:42.158562 slcl1butils-2023.6.6/slcl1butils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 07:44:42.000000 slcl1butils-2023.6.6/slcl1butils.egg-info/top_level.txt
```

### Comparing `slcl1butils-2023.6.26/.github/workflows/publish.yml` & `slcl1butils-2023.6.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/.gitignore` & `slcl1butils-2023.6.6/.gitignore`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/.pre-commit-config.yaml` & `slcl1butils-2023.6.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/LICENSE` & `slcl1butils-2023.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/PKG-INFO` & `slcl1butils-2023.6.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2023.6.26
+Version: 2023.6.6
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Documentation Status](https://readthedocs.org/projects/slcl1butils/badge/?version=latest)](https://slcl1butils.readthedocs.io/en/latest/?badge=latest) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/slcl1butils.svg)](https://anaconda.org/conda-forge/slcl1butils)
+[![Documentation Status](https://readthedocs.org/projects/slcl1butils/badge/?version=latest)](https://slcl1butils.readthedocs.io/en/latest/?badge=latest)
 
 # utils_xsarslc_l1b
 python tool to read/display/enrich Sentinel-1 SAR Level-1 B SLC products produced at IFREMER
 
 ## installation 
 
 ```bash
```

### Comparing `slcl1butils-2023.6.26/README.md` & `slcl1butils-2023.6.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Documentation Status](https://readthedocs.org/projects/slcl1butils/badge/?version=latest)](https://slcl1butils.readthedocs.io/en/latest/?badge=latest) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/slcl1butils.svg)](https://anaconda.org/conda-forge/slcl1butils)
+[![Documentation Status](https://readthedocs.org/projects/slcl1butils/badge/?version=latest)](https://slcl1butils.readthedocs.io/en/latest/?badge=latest)
 
 # utils_xsarslc_l1b
 python tool to read/display/enrich Sentinel-1 SAR Level-1 B SLC products produced at IFREMER
 
 ## installation 
 
 ```bash
```

### Comparing `slcl1butils-2023.6.26/ci/requirements/environment.yaml` & `slcl1butils-2023.6.6/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/Makefile` & `slcl1butils-2023.6.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/conf.py` & `slcl1butils-2023.6.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/cwave.rst` & `slcl1butils-2023.6.6/docs/cwave.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 .. _cwave:
 
 ================================
 Computation of CWAVE parameters
 ================================
 
-This section refers to :
-
-.. py:function:: slcl1butils.compute.cwave.compute_cwave_parameters()
 
 CWAVE parmeters are based on the SAR image x-spectrum.
 
 The spectral information of the normalized x-spectrum is decomposed according to orthonormal functions :math:`H_{ij}` defined as tensor products of Gegenbauer polynomial :math:`G_i(\alpha_k(k_x,k_y))` and harmonic :math:`F_j(\alpha_\phi(k_x,k_y))` functions defined in the azimuth :math:`k_y` and range :math:`k_y` wave-number space, following XXX work.
 
 This yields to the general formulation of CWAVE parameters :math:`C_{ij}`:
```

### Comparing `slcl1butils-2023.6.26/docs/examples/display_a_IW_L1B_xspectra.ipynb` & `slcl1butils-2023.6.6/docs/examples/display_a_IW_L1B_xspectra.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb` & `slcl1butils-2023.6.6/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.6.6/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.6.6/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/index.rst` & `slcl1butils-2023.6.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/installing.rst` & `slcl1butils-2023.6.6/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/docs/oceanspectrumSAR.png` & `slcl1butils-2023.6.6/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/get_polygons_from_l1b.py` & `slcl1butils-2023.6.6/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/pyproject.toml` & `slcl1butils-2023.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/coloc/coloc.py` & `slcl1butils-2023.6.6/slcl1butils/coloc/coloc.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/compute/compute_from_l1b.py` & `slcl1butils-2023.6.6/slcl1butils/compute/compute_from_l1b.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,17 @@
 import logging
 
 
 def compute_xs_from_l1b(_file, burst_type='intra', time_separation='2tau'):
     """
 
     Args:
-        _file
-              (str) full path L1B nc file
-        burst_type
-              (str) intra or inter
-        time_separation
-              (str) 2tau or 1tau...
+        _file: str full path L1B nc file
+        burst_type: str intra or inter
+        time_separation: str 2tau or 1tau...
 
     Returns:
 
     """
     # Reading the l1b file
     # Loading the specified burst group
     # dt = datatree.open_datatree(_file)
```

### Comparing `slcl1butils-2023.6.26/slcl1butils/compute/cwave.py` & `slcl1butils-2023.6.6/slcl1butils/compute/cwave.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/compute/macs.py` & `slcl1butils-2023.6.6/slcl1butils/compute/macs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import xarray as xr
 import numpy as np
 
 
 def compute_macs(xs, lambda_range_max=[50.]):
     """
     Parameters:
-        xs xarray.Dataset
-           cartesian cross spectra described on a grid 'k_az' and 'k_rg'
-        lambda_range_max list
-             list of floats to set maximum value for the area where MACS integral is computed
-    Return:
-        macs xarray.Dataset
-           dataset containing imaginary and real part of MACS
+        xs: xarray.Dataset
+        lambda_range_max: list of float
+    :return:
+        macs : xarray.Dataset containing imaginary and real part of MACS
     """
     # IMACS fix limits from Li et al., JGR 2019
     k_az_max = 2 * np.pi / 600.
     k_az_min = -2 * np.pi / 600.
 
     k_rg_max = 2 * np.pi / 15.
     # k_rg_min = 2*np.pi/lambda_range[1]#20 # 20
```

### Comparing `slcl1butils-2023.6.26/slcl1butils/compute/stack_iw_l1b.py` & `slcl1butils-2023.6.6/slcl1butils/compute/stack_iw_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/compute/stack_wv_l1c_monthly.py` & `slcl1butils-2023.6.6/slcl1butils/compute/stack_wv_l1c_monthly.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     dsu['wvmode'] = xr.DataArray(tmpsubswath)
     tmpdate = datetime.datetime.strptime(dsu.attrs['start_date'],
                                          '%Y-%m-%d %H:%M:%S.%f')
     #dsu['sardate'] = xr.DataArray(tmpdate)
     dsu = dsu.isel(freq_sample=slice(0, indkrg), freq_line=slice(indkaz_bo, indkaz_up))
     dsu = dsu.assign_coords({'k_rg': k_rg_ref.values, 'k_az': k_az_ref.values})
     dsu = dsu.assign_coords({'nc_number':nc_number})
-    dsu = dsu.assign_coords({'sardate': np.datetime64(tmpdate,'s').astype('datetime64[ns]')})
+    dsu = dsu.assign_coords({'sardate': tmpdate})
     if 'xspectra_0tau_Re' in dsu:
         for tautau in range(3):
             dsu['xspectra_%stau' % tautau] = dsu['xspectra_%stau_Re' % tautau] + 1j * dsu['xspectra_%stau_Im' % tautau]
             dsu = dsu.drop(['xspectra_%stau_Re' % tautau, 'xspectra_%stau_Im' % tautau])
     return dsu
```

### Comparing `slcl1butils-2023.6.26/slcl1butils/conversion_polar_cartesian.py` & `slcl1butils-2023.6.6/slcl1butils/conversion_polar_cartesian.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/cwave_parameters_computation_example.ipynb` & `slcl1butils-2023.6.6/slcl1butils/cwave_parameters_computation_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/get_config.py` & `slcl1butils-2023.6.6/slcl1butils/get_config.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/get_polygons_from_l1b.py` & `slcl1butils-2023.6.6/slcl1butils/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/plotting/display_one_spectra.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/display_one_spectra.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,23 +24,14 @@
     0.06384707, 0.06796645, 0.0723516, 0.07701967, 0.08198893, 0.08727881,
     0.09290998, 0.09890447, 0.1052857, 0.1120787, 0.1193099, 0.1270077,
     0.1352022, 0.1439253, 0.1532113, 0.1630964, 0.1736193, 0.1848211,
     0.1967456, 0.2094395])
 
 def core_plot_part(crossSpectraRePol,heading,fig=None,ax=None,thecmap=None,limit_display_wv=100,title='x spec',
                    tauval=2,azimuth_cutoffSAR=None,vmin=None,vmax=None,add_colorbar=True):
-    """
-    Parameters
-    ----------
-        crossSpectraRePol xarray.core.Dataset
-    Returns
-    -------
-
-
-    """
     # partie display plot
     if fig is None :
         plt.figure(figsize=(20,8),dpi=100)
     if ax is None :
         ax = plt.subplot(1,1,1,polar=True)
 
         ax.set_theta_direction(-1)  # theta increasing clockwise
```

### Comparing `slcl1butils-2023.6.26/slcl1butils/plotting/display_xspectra_grid.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/display_xspectra_grid.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2023.6.6/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2023.6.6/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/plotting/wallpaper.py` & `slcl1butils-2023.6.6/slcl1butils/plotting/wallpaper.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/raster_readers.py` & `slcl1butils-2023.6.6/slcl1butils/raster_readers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             if 'xspectra_Re' in ds_inter:
                 save_l1c_to_netcdf(l1c_full_path, ds_intra, ds_inter,version=version)
                 cpt['saved_in_nc'] += 1
             else:
                 logging.info('there is no xspectra in this subswath -> the L1C will not be saved')
                 cpt['L1B_without_spectra'] += 1
     logging.info('cpt: %s',cpt)
-    return l1c_full_path
+    return 0
 
 
 def enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=None, cwave=True, macs=True, colocat=True,
                            time_separation='2tau'):
 
     logging.info('File in: %s', l1b_fullpath)
     if ancillary_list is None:
@@ -304,17 +304,16 @@
                             datefmt='%d/%m/%Y %H:%M:%S',force=True)
     else:
         logging.basicConfig(level=logging.INFO, format=fmt,
                             datefmt='%d/%m/%Y %H:%M:%S',force=True)
     t0 = time.time()
     logging.info('product version to produce: %s', args.version)
     logging.info('outputdir will be: %s', args.outputdir)
-    final_L1C_path = do_L1C_SAFE_from_L1B_SAFE(args.l1bsafe,version=args.version,outputdir=args.outputdir, cwave=True, macs=True, colocat=True,
+    do_L1C_SAFE_from_L1B_SAFE(args.l1bsafe,version=args.version,outputdir=args.outputdir, cwave=True, macs=True, colocat=True,
                                   time_separation='2tau', overwrite=args.overwrite,dev=args.dev)
-    logging.info('%s successfully written',final_L1C_path)
     logging.info('peak memory usage: %s ', get_memory_usage())
     logging.info('done in %1.3f min', (time.time() - t0) / 60.)
 
 
 if __name__ == '__main__':
     root = logging.getLogger()
     if root.handlers:
```

### Comparing `slcl1butils-2023.6.26/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,16 @@
     else:
         logging.basicConfig(level=logging.INFO, format='%(asctime)s %(levelname)-5s %(message)s',
                             datefmt='%d/%m/%Y %H:%M:%S')
     prunexe = '/appli/prun/bin/prun'
     listing = '/home/datawork-cersat-public/project/sarwave/data/listings/iw_l1b_safe_1.4k.txt' # 5781 SAFE, 632Go en L1B
     listing = '/home/datawork-cersat-public/project/sarwave/data/listings/iw_l1b_safe_1.4k_v2.txt' 
     listing = '/home/datawork-cersat-public/project/sarwave/data/listings/iw_l1b_safe_1.4k_v3.txt' # the most complete for SAFE 1.4k L1B
-    listing = '/home/datawork-cersat-public/project/sarwave/data/listings/iw_l1b_safe_2.1.txt' #2km decimated with negative overlap
-   # listing = '/home/datawork-cersat-public/project/sarwave/data/listings/L1B_L1C_listing_safe_missing_IW_1.4k_operational.txt'
-   # listing = '/home/datawork-cersat-public/project/sarwave/data/listings/L1B_L1C_listing_safe_missing_IW_1.4j.txt'
+    listing = '/home/datawork-cersat-public/project/sarwave/data/listings/L1B_L1C_listing_safe_missing_IW_1.4k_operational.txt'
+    listing = '/home/datawork-cersat-public/project/sarwave/data/listings/L1B_L1C_listing_safe_missing_IW_1.4j.txt'
     # listing = '/home/datawork-cersat-public/project/sarwave/data/listings/iw_l1b_safe_1.4k_test.txt'
     logging.info('outputdir : %s',args.outputdir)
     # modify initial listing with more args
     listing2 = listing + '.modified'
     fid = open(listing2, 'w')
     content = open(listing).readlines()
     taille = len(content)
```

### Comparing `slcl1butils-2023.6.26/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,25 +84,25 @@
     cpt_ancillary_products_found = 0
     for ii in pbar:
         pbar.set_description('sucess: %s/%s ancillary : %s, already: %s' % (
         cpt_success, len(files), cpt_ancillary_products_found, cpt_already))
         l1b_fullpath = files[ii]
         l1c_full_path, l1b_product_version = get_l1c_filepath(l1b_fullpath, version=version, outputdir=outputdir)
         if os.path.exists(l1c_full_path) and overwrite is False:
-            logging.info('%s already exists', l1c_full_path)
+            logging.debug('%s already exists', l1c_full_path)
             cpt_already += 1
         else:
             ds_intra, ancillary_product_found = enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=ancillary_list,
                                                                        cwave=cwave, macs=macs,
                                                                        colocat=colocat,
                                                                        time_separation=time_separation)
             if ancillary_product_found:
                 cpt_ancillary_products_found += 1
             save_l1c_to_netcdf(l1c_full_path, ds_intra, version=version, version_L1B=l1b_product_version)
-            logging.info('successfully wrote  %s', l1c_full_path)
+            logging.debug('successfully wrote  %s', l1c_full_path)
             cpt_success += 1
     return 0
 
 
 def enrich_onesubswath_l1b(l1b_fullpath, ancillary_list=None, cwave=True, macs=True, colocat=True,
                            time_separation='2tau'):
     """
@@ -281,15 +281,14 @@
     dt.attrs['processor'] = __file__
     dt.attrs['generation_date'] = datetime.today().strftime('%Y-%b-%d')
     dt.attrs['L1B_product_version'] = version_L1B
 
     #
     # Saving the results in netCDF
     dt.to_netcdf(l1c_full_path)
-    logging.info('output file written successfully: %s',l1c_full_path)
 
 
 def main():
     """
 
     Returns
     -------
```

### Comparing `slcl1butils-2023.6.26/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py` & `slcl1butils-2023.6.6/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/spectrum_clockwise_to_trigo.py` & `slcl1butils-2023.6.6/slcl1butils/spectrum_clockwise_to_trigo.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/spectrum_rotation.py` & `slcl1butils-2023.6.6/slcl1butils/spectrum_rotation.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/symmetrize_l1b_spectra.py` & `slcl1butils-2023.6.6/slcl1butils/symmetrize_l1b_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils/utils.py` & `slcl1butils-2023.6.6/slcl1butils/utils.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2023.6.26/slcl1butils.egg-info/PKG-INFO` & `slcl1butils-2023.6.6/slcl1butils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2023.6.26
+Version: 2023.6.6
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Documentation Status](https://readthedocs.org/projects/slcl1butils/badge/?version=latest)](https://slcl1butils.readthedocs.io/en/latest/?badge=latest) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/slcl1butils.svg)](https://anaconda.org/conda-forge/slcl1butils)
+[![Documentation Status](https://readthedocs.org/projects/slcl1butils/badge/?version=latest)](https://slcl1butils.readthedocs.io/en/latest/?badge=latest)
 
 # utils_xsarslc_l1b
 python tool to read/display/enrich Sentinel-1 SAR Level-1 B SLC products produced at IFREMER
 
 ## installation 
 
 ```bash
```

### Comparing `slcl1butils-2023.6.26/slcl1butils.egg-info/SOURCES.txt` & `slcl1butils-2023.6.6/slcl1butils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

