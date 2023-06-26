# Comparing `tmp/acoular-22.3.tar.gz` & `tmp/acoular-23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/acoular-22.3.tar", last modified: Mon Mar 28 17:49:59 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `acoular-22.3.tar` & `acoular-23.6.tar`

### file list

```diff
@@ -1,76 +1,185 @@
-drwxrwxr-x   0 sarradj   (1000) sarradj   (1000)        0 2022-03-28 17:49:59.882727 acoular-22.3/
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)      382 2021-04-29 17:26:46.000000 acoular-22.3/AUTHORS.rst
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     1528 2021-05-06 13:30:59.000000 acoular-22.3/LICENSE
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)      101 2019-02-26 17:23:00.000000 acoular-22.3/MANIFEST.in
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     2050 2022-03-28 17:49:59.882727 acoular-22.3/PKG-INFO
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     1132 2021-05-06 13:30:59.000000 acoular-22.3/README.rst
-drwxrwxr-x   0 sarradj   (1000) sarradj   (1000)        0 2022-03-28 17:49:59.874727 acoular-22.3/acoular/
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     2510 2022-03-28 14:49:27.000000 acoular-22.3/acoular/__init__.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     2655 2022-03-28 14:49:27.000000 acoular-22.3/acoular/calib.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     5657 2022-03-28 14:49:27.000000 acoular-22.3/acoular/configuration.py
-drwxrwxr-x   0 sarradj   (1000) sarradj   (1000)        0 2022-03-28 17:49:59.878727 acoular-22.3/acoular/demo/
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)      251 2022-03-28 14:49:27.000000 acoular-22.3/acoular/demo/__init__.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     2801 2022-03-28 14:49:27.000000 acoular-22.3/acoular/demo/acoular_demo.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    20887 2022-03-28 14:49:27.000000 acoular-22.3/acoular/environments.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    64561 2022-03-28 14:49:27.000000 acoular-22.3/acoular/fastFuncs.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)   107123 2022-03-28 14:49:27.000000 acoular-22.3/acoular/fbeamform.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    13285 2022-03-28 14:49:27.000000 acoular-22.3/acoular/fileimport.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    42862 2022-03-28 14:49:27.000000 acoular-22.3/acoular/grids.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     4700 2022-03-28 14:49:27.000000 acoular-22.3/acoular/h5cache.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     6476 2022-03-28 14:49:27.000000 acoular-22.3/acoular/h5files.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)      689 2022-03-28 14:49:27.000000 acoular-22.3/acoular/internal.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     4341 2022-03-28 14:49:27.000000 acoular-22.3/acoular/microphones.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    10702 2022-03-28 14:49:27.000000 acoular-22.3/acoular/nidaqimport.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     4344 2022-03-28 14:49:27.000000 acoular-22.3/acoular/sdinput.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    11865 2022-03-28 14:49:27.000000 acoular-22.3/acoular/signals.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    48365 2022-03-28 14:49:27.000000 acoular-22.3/acoular/sources.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    20752 2022-03-28 14:49:27.000000 acoular-22.3/acoular/spectra.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    30903 2022-03-28 14:49:27.000000 acoular-22.3/acoular/tbeamform.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     7499 2022-03-28 14:49:27.000000 acoular-22.3/acoular/tfastfuncs.py
--rwxrwxr-x   0 sarradj   (1000) sarradj   (1000)     9356 2022-03-28 14:49:27.000000 acoular-22.3/acoular/tools.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    90890 2022-03-28 14:49:27.000000 acoular-22.3/acoular/tprocess.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)    17655 2022-03-28 14:49:27.000000 acoular-22.3/acoular/traitsviews.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     4203 2022-03-28 14:49:27.000000 acoular-22.3/acoular/trajectory.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)      391 2022-03-28 14:49:27.000000 acoular-22.3/acoular/version.py
-drwxrwxr-x   0 sarradj   (1000) sarradj   (1000)        0 2022-03-28 17:49:59.878727 acoular-22.3/acoular/xml/
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     5127 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/HW90D240_f10.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     5283 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/W90_D105_f10.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     1993 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/acousticam_2c.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     1949 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/acousticam_4c.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     2363 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array38.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     5874 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array92x.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     3428 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array_56.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     4432 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array_56_10_9.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     4193 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array_56_bomb.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     3458 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array_56_v2.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     4039 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array_64.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     6558 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array_84_10_9.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     6248 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/array_84_bomb_v3.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     1341 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/calib_vw_ring32.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     1831 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/gfai_ring32.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     1153 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/minidsp_uma16.xml
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     4424 2020-02-28 09:28:17.000000 acoular-22.3/acoular/xml/tub_vogel64.xml
-drwxrwxr-x   0 sarradj   (1000) sarradj   (1000)        0 2022-03-28 17:49:59.878727 acoular-22.3/acoular.egg-info/
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     2050 2022-03-28 17:49:59.000000 acoular-22.3/acoular.egg-info/PKG-INFO
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     1856 2022-03-28 17:49:59.000000 acoular-22.3/acoular.egg-info/SOURCES.txt
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)        1 2022-03-28 17:49:59.000000 acoular-22.3/acoular.egg-info/dependency_links.txt
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)        1 2019-11-06 19:00:53.000000 acoular-22.3/acoular.egg-info/not-zip-safe
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)       80 2022-03-28 17:49:59.000000 acoular-22.3/acoular.egg-info/requires.txt
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)        8 2022-03-28 17:49:59.000000 acoular-22.3/acoular.egg-info/top_level.txt
-drwxrwxr-x   0 sarradj   (1000) sarradj   (1000)        0 2022-03-28 17:49:59.882727 acoular-22.3/examples/
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     2557 2022-03-28 14:49:27.000000 acoular-22.3/examples/acoular_demo.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     1207 2022-03-28 14:49:27.000000 acoular-22.3/examples/basic_beamformer_example.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     4818 2020-09-07 14:07:30.000000 acoular-22.3/examples/example_3D_beamforming.py
--rwxrwxr-x   0 sarradj   (1000) sarradj   (1000)      459 2020-09-07 14:07:30.000000 acoular-22.3/examples/example_GenericSignal.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     4791 2022-03-28 14:49:27.000000 acoular-22.3/examples/example_SampleSplitter_bufferhandling.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     3528 2022-03-28 14:49:27.000000 acoular-22.3/examples/example_SampleSplitter_multithreading.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     9149 2020-09-07 14:07:30.000000 acoular-22.3/examples/example_airfoil_in_open_jet_beamforming.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     4688 2022-03-08 16:09:50.000000 acoular-22.3/examples/example_airfoil_in_open_jet_cmf.py
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)     5543 2019-08-14 16:53:02.000000 acoular-22.3/examples/example_airfoil_in_open_jet_steering_vectors.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     4773 2022-03-28 14:49:27.000000 acoular-22.3/examples/example_airfoil_in_open_jet_time_beamforming.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     8778 2020-09-07 14:07:30.000000 acoular-22.3/examples/example_rotating_point_source.py
--rwxrwxr-x   0 sarradj   (1000) sarradj   (1000)     4507 2022-03-28 14:49:27.000000 acoular-22.3/examples/example_sectors_and_intergration.py
--rwxrwxr-x   0 sarradj   (1000) sarradj   (1000)     1926 2022-03-28 14:49:27.000000 acoular-22.3/examples/example_tools.py
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     1629 2022-03-28 14:49:27.000000 acoular-22.3/examples/three_sources.py
--rw-r--r--   0 sarradj   (1000) sarradj   (1000)       73 2022-03-28 17:49:59.882727 acoular-22.3/setup.cfg
--rw-rw-r--   0 sarradj   (1000) sarradj   (1000)     2007 2022-03-28 17:32:39.000000 acoular-22.3/setup.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 acoular-23.6/.gitlab-ci.yml
+-rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 acoular-23.6/.travis.yml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 acoular-23.6/MANIFEST.in
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 acoular-23.6/README.rst
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 acoular-23.6/build_conda.sh
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 acoular-23.6/noxfile.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 acoular-23.6/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 acoular-23.6/acoular/__init__.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 acoular-23.6/acoular/calib.py
+-rw-r--r--   0        0        0     5653 2020-02-02 00:00:00.000000 acoular-23.6/acoular/configuration.py
+-rw-r--r--   0        0        0    22189 2020-02-02 00:00:00.000000 acoular-23.6/acoular/environments.py
+-rw-r--r--   0        0        0    64561 2020-02-02 00:00:00.000000 acoular-23.6/acoular/fastFuncs.py
+-rw-r--r--   0        0        0   114180 2020-02-02 00:00:00.000000 acoular-23.6/acoular/fbeamform.py
+-rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 acoular-23.6/acoular/fileimport.py
+-rw-r--r--   0        0        0    45353 2020-02-02 00:00:00.000000 acoular-23.6/acoular/grids.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 acoular-23.6/acoular/h5cache.py
+-rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 acoular-23.6/acoular/h5files.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 acoular-23.6/acoular/internal.py
+-rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 acoular-23.6/acoular/microphones.py
+-rw-r--r--   0        0        0    10702 2020-02-02 00:00:00.000000 acoular-23.6/acoular/nidaqimport.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 acoular-23.6/acoular/sdinput.py
+-rw-r--r--   0        0        0    11865 2020-02-02 00:00:00.000000 acoular-23.6/acoular/signals.py
+-rw-r--r--   0        0        0    48492 2020-02-02 00:00:00.000000 acoular-23.6/acoular/sources.py
+-rw-r--r--   0        0        0    28975 2020-02-02 00:00:00.000000 acoular-23.6/acoular/spectra.py
+-rw-r--r--   0        0        0    30903 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tbeamform.py
+-rw-r--r--   0        0        0     7499 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tfastfuncs.py
+-rwxr-xr-x   0        0        0     9256 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tools.py
+-rw-r--r--   0        0        0    90970 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tprocess.py
+-rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 acoular-23.6/acoular/traitsviews.py
+-rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 acoular-23.6/acoular/trajectory.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 acoular-23.6/acoular/version.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 acoular-23.6/acoular/demo/__init__.py
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 acoular-23.6/acoular/demo/acoular_demo.py
+-rwxr-xr-x   0        0        0      288 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/run_tests.sh
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/run_tests_osx.sh
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test.npy
+-rw-r--r--   0        0        0     9054 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_beamformer_results.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_classes.py
+-rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_digest.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_environments.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_example1.py
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_signals.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_sources.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_spectra.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_timecache.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_tprocess.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/test_traj_beamformer_results.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerBase.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerCMF.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerCapon.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerClean.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerCleansc.npy
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerCleant.npy
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerCleantSq.npy
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerCleantSqTraj.npy
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerCleantTraj.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerDamas.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerDamasPlus.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerEig.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerFunctional.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerGIB.npy
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerGridlessOrth.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerMusic.npy
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerOrth.npy
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerTime.npy
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerTimeSq.npy
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerTimeSqTraj.npy
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/BeamformerTimeTraj.npy
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/Environment.npy
+-rw-r--r--   0        0        0     9688 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/Example1_numerical_values_testsum.h5
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/GeneralFlowEnvironment.npy
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/OpenJet.npy
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/PointSource.npy
+-rw-r--r--   0        0        0    46784 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/PowerSpectra_csm.npy
+-rw-r--r--   0        0        0    46784 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/PowerSpectra_ev.npy
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/RotatingFlow.npy
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/SlotJet.npy
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/UniformFlowEnvironment.npy
+-rw-r--r--   0        0        0    69960 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/reference_data/beamformer_traj_time_data.h5
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/functionalBeamformer.py
+-rw-r--r--   0        0        0     6266 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/precisionTest.py
+-rw-r--r--   0        0        0    13815 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/validationOfBeamformerFuncsPOSTAcoularIntegration.py
+-rw-r--r--   0        0        0    31698 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/validationOfBeamformerFuncsPREeAcoularIntegration.py
+-rw-r--r--   0        0        0   131252 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/OvernightTestcasesBeamformer_nMics32_nGridPoints100_nFreqs4_nTrials10.png
+-rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/cythonBeamformer.pyx
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/mainForCython.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/mainForParallelJit.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/setupCythonOpenMP.py
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/sharedFunctions.py
+-rw-r--r--   0        0        0   172747 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/timeOverNMics_AllImportantMethods.png
+-rw-r--r--   0        0        0   131665 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/timeOverNMics_faverage.png
+-rw-r--r--   0        0        0    10020 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/vglOptimierungFAverage.py
+-rw-r--r--   0        0        0     9712 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/vglOptimierungGaussSeidel.py
+-rwxr-xr-x   0        0        0    40111 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/vglOptimierungR_BEAMFULL_INVERSE.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/vglOptimierungR_BEAM_OS.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 acoular-23.6/acoular/tests/unsupported/SpeedComparison/whatsFastestWayFor_absASquared.py
+-rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/HW90D240_f10.xml
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/W90_D105_f10.xml
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/acousticam_2c.xml
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/acousticam_4c.xml
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array38.xml
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array92x.xml
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array_56.xml
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array_56_10_9.xml
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array_56_bomb.xml
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array_56_v2.xml
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array_64.xml
+-rw-r--r--   0        0        0     6558 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array_84_10_9.xml
+-rw-r--r--   0        0        0     6248 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/array_84_bomb_v3.xml
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/calib_vw_ring32.xml
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/gfai_ring32.xml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/minidsp_uma16.xml
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 acoular-23.6/acoular/xml/tub_vogel64.xml
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 acoular-23.6/docs/Makefile
+-rw-r--r--   0        0        0     7523 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/conf.py
+-rw-r--r--   0        0        0    39963 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/gen_rst.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/index.rst
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/requirements.txt
+-rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_static/Acoular_logo.png
+-rw-r--r--   0        0        0   248866 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_static/Airfoil_selfnoise_3d.png
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_static/acoular_logo.ico
+-rw-r--r--   0        0        0    37466 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_static/airfoil_leading_edge_noise.png
+-rw-r--r--   0        0        0     4315 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_static/no_image.png
+-rw-r--r--   0        0        0    60494 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_static/pantograph_noise_3d.png
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_themes/haikuac/layout.html
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_themes/haikuac/theme.conf
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_themes/haikuac/static/alert_info_32.png
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_themes/haikuac/static/alert_warning_32.png
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_themes/haikuac/static/bg-page.png
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_themes/haikuac/static/bullet_orange.png
+-rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/_themes/haikuac/static/haikuac.css_t
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/api_ref/index.rst
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_3D_beamforming.rst
+-rw-r--r--   0        0        0    78071 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_3D_beamforming_1.png
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_beamforming.rst
+-rw-r--r--   0        0        0    61537 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_beamforming_1.png
+-rw-r--r--   0        0        0    45784 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_beamforming_2.png
+-rw-r--r--   0        0        0    46411 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_beamforming_3.png
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_cmf.rst
+-rw-r--r--   0        0        0    36576 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_cmf_1.png
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_steering_vectors.rst
+-rw-r--r--   0        0        0    54480 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_steering_vectors_1.png
+-rw-r--r--   0        0        0    61898 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_airfoil_in_open_jet_steering_vectors_2.png
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_rotating_point_source.rst
+-rw-r--r--   0        0        0    65341 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_rotating_point_source_1.png
+-rw-r--r--   0        0        0    57493 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_rotating_point_source_2.png
+-rw-r--r--   0        0        0    31515 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/example_rotating_point_source_3.png
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/examples/index.rst
+-rw-r--r--   0        0        0    21039 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/get_started/array64.png
+-rw-r--r--   0        0        0    15250 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/get_started/array64_py3colormap.png
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/get_started/index.rst
+-rw-r--r--   0        0        0    64624 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/get_started/map_three_sources.png
+-rw-r--r--   0        0        0    34929 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/get_started/three_source_py3_colormap.png
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/install/index.rst
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/literature/index.rst
+-rw-r--r--   0        0        0     8628 2020-02-02 00:00:00.000000 acoular-23.6/docs/source/news/index.rst
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 acoular-23.6/examples/README.txt
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 acoular-23.6/examples/acoular_demo.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 acoular-23.6/examples/basic_beamformer_example.py
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_3D_beamforming.py
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_GenericSignal.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_SampleSplitter_bufferhandling.py
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_SampleSplitter_multithreading.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_airfoil_in_open_jet_beamforming.py
+-rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_airfoil_in_open_jet_cmf.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_airfoil_in_open_jet_steering_vectors.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_airfoil_in_open_jet_time_beamforming.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_calib.xml
+-rw-r--r--   0        0        0  5807392 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_data.h5
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_power_spectra_import.py
+-rw-r--r--   0        0        0     8778 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_rotating_point_source.py
+-rwxr-xr-x   0        0        0     4507 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_sectors_and_intergration.py
+-rwxr-xr-x   0        0        0     1926 2020-02-02 00:00:00.000000 acoular-23.6/examples/example_tools.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 acoular-23.6/examples/three_sources.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 acoular-23.6/recipe.local/meta.yaml
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 acoular-23.6/recipe.local/run_test.sh
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 acoular-23.6/scripts/plot_examples.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 acoular-23.6/.gitignore
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 acoular-23.6/AUTHORS.rst
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 acoular-23.6/LICENSE
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 acoular-23.6/README.md
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 acoular-23.6/pyproject.toml
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 acoular-23.6/PKG-INFO
```

### Comparing `acoular-22.3/LICENSE` & `acoular-23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `acoular-22.3/README.rst` & `acoular-23.6/README.rst`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/__init__.py` & `acoular-23.6/acoular/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,25 @@
 from .tprocess import SamplesGenerator, TimeInOut, MaskedTimeInOut, ChannelMixer, \
 Mixer, TimeAverage, TimeReverse, TimePower, FiltFiltOctave, FiltOctave, TimeCache, \
 WriteWAV, WriteH5, SpatialInterpolator, SpatialInterpolatorRotation, Trigger, \
 SampleSplitter, AngleTracker, SpatialInterpolatorConstantRotation, Filter, \
 TimeExpAverage, FiltFreqWeight, TimeCumAverage, FilterBank, OctaveFilterBank, TimeConvolve
 from .calib import Calib
 from .trajectory import Trajectory
-from .grids import Grid, RectGrid, RectGrid3D, Sector,RectSector,CircSector,\
+from .grids import Grid, RectGrid, RectGrid3D, Sector, RectSector, RectSector3D, CircSector,\
     PolySector, MultiSector, MergeGrid, LineGrid, ImportGrid, ConvexSector
 from .environments import cartToCyl, cylToCart, Environment, UniformFlowEnvironment, RotatingFlow, \
 FlowField, OpenJet, SlotJet, GeneralFlowEnvironment
 from .microphones import MicGeom
-from .spectra import PowerSpectra, PowerSpectra as EigSpectra, synthetic
+from .spectra import BaseSpectra, FFTSpectra, PowerSpectra, PowerSpectraImport, PowerSpectra as EigSpectra, synthetic
 
 from .fbeamform import BeamformerBase, BeamformerCapon, BeamformerEig, \
 BeamformerMusic, BeamformerDamas, BeamformerDamasPlus, BeamformerOrth,BeamformerCleansc, \
 BeamformerCMF,BeamformerSODIX, BeamformerClean, BeamformerFunctional, BeamformerGIB, L_p, integrate, \
-PointSpreadFunction, SteeringVector
+PointSpreadFunction, SteeringVector, BeamformerAdaptiveGrid, BeamformerGridlessOrth
 
 from .sources import PointSource, MovingPointSource, \
 TimeSamples, MaskedTimeSamples, PointSourceDipole, UncorrelatedNoiseSource, \
 SourceMixer, SphericalHarmonicSource, LineSource, MovingPointSourceDipole, \
 MovingLineSource
 from .signals import SineGenerator, WNoiseGenerator, SignalGenerator,\
 PNoiseGenerator, GenericSignalGenerator, FiltWNoiseGenerator
```

### Comparing `acoular-22.3/acoular/calib.py` & `acoular-23.6/acoular/calib.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/configuration.py` & `acoular-23.6/acoular/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # Copyright (c) Acoular Development Team.
 #------------------------------------------------------------------------------
 """Implements global configuration of Acoular.
 
 .. autosummary::
     :toctree: generated/
 
+    Config
     config
-
 """
 
 from os import path, mkdir
 from traits.api import Trait, Bool, Str, Property, HasStrictTraits
 
 class Config(HasStrictTraits):
     """
@@ -128,24 +128,24 @@
         self._td_dir = tddir
 
 config = Config()
 """
 This instance implements the global configuration of the Acoular package.
 
 General caching behaviour can be controlled by the :attr:`global_caching` attribute:
-  * 'individual': Acoular classes handle caching behavior individually.
-  * 'all': Acoular classes cache everything and read from cache if possible.
-  * 'none': Acoular classes do not cache results. Cachefiles are not created.
-  * 'readonly': Acoular classes do not actively cache, but read from cache if existing.
-  * 'overwrite': Acoular classes replace existing cachefile content with new data.
+* 'individual': Acoular classes handle caching behavior individually.
+* 'all': Acoular classes cache everything and read from cache if possible.
+* 'none': Acoular classes do not cache results. Cachefiles are not created.
+* 'readonly': Acoular classes do not actively cache, but read from cache if existing.
+* 'overwrite': Acoular classes replace existing cachefile content with new data.
 
 The package used to read and write .h5 files can be specified 
 by :attr:`h5library`:  
-  * 'pytables': Use 'tables' (or 'pytables', depending on python distribution).
-  * 'h5py': Use 'h5py'.
+* 'pytables': Use 'tables' (or 'pytables', depending on python distribution).
+* 'h5py': Use 'h5py'.
 
 Some Acoular classes support GUI elements for usage with tools from the TraitsUI package.
 If desired, this package has to be installed manually, as it is not a prerequisite for
 installing Acoular.
 To enable the functionality, the flag attribute :attr:`use_traitsui` has to be set to True (default: False).
 Note: this is independent from the GUI tools implemented in the spectAcoular package.
```

### Comparing `acoular-22.3/acoular/demo/acoular_demo.py` & `acoular-23.6/acoular/demo/acoular_demo.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/environments.py` & `acoular-23.6/acoular/environments.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 sqrt, arange, pi, exp, sin, cos, arccos, zeros_like, empty, dot, hstack, \
 vstack, identity, cross, sign, arctan2, matmul, sum, lexsort, stack, nonzero, append, outer, asarray
 from numpy.linalg.linalg import norm
 from scipy.integrate import ode
 from scipy.interpolate import LinearNDInterpolator
 from scipy.spatial import ConvexHull
 from traits.api import HasPrivateTraits, Float, Property, Int, \
-CArray, cached_property, Trait
+CArray, cached_property, Trait, Dict
 
-from .internal import digest
+from .internal import digest, ldigest
 
 f64ro = nb.types.Array(nb.types.float64,2,'A',readonly=True)
 f32ro = nb.types.Array(nb.types.float32,2,'A',readonly=True)
 
 @nb.njit([(f64ro, f64ro), (f64ro, f32ro), (f32ro, f64ro),(f32ro, f32ro)],
                 cache=True, fastmath=True)
 def dist_mat(gpos,mpos):
@@ -123,14 +123,17 @@
         depends_on=['c'], 
         )
 
     #: The speed of sound, defaults to 343 m/s
     c = Float(343., 
         desc="speed of sound")
 
+    #: The region of interest (ROI), not needed for most types of environment
+    roi = Trait(None,(None,CArray))
+
     def _get_digest( self ):
         return digest( self )
 
     def _r( self, gpos, mpos=0.0):
         """
         Calculates distances between grid point locations and microphone
         locations or the origin. Functionality may change in the future.
@@ -535,14 +538,17 @@
         desc="maximum solid angle")
 
     # internal identifier
     digest = Property(
         depends_on=['c', 'ff.digest', 'N', 'Om'], 
         )
 
+    # internal dictionary of interpolators
+    idict = Dict
+
     @cached_property
     def _get_digest( self ):
         return digest( self )
 
     def _r( self, gpos, mpos=0.0):
         """
         Calculates the virtual distances between grid point locations and
@@ -567,14 +573,53 @@
             then only a one-dimensional array is returned.
         """
         c = self.c
         
         if isscalar(mpos):
             mpos = array((0, 0, 0), dtype = float32)[:, newaxis]
 
+        gt = empty((gpos.shape[-1], mpos.shape[-1]))
+        for micnum, x0 in enumerate(mpos.T):
+            key = x0.tobytes() # make array hashable
+            #todo: the interpolator also depends the roi, so idict keys should also depend on roi
+            # OR the idict should be cleaned if roi changes
+            try:
+                li = self.idict[key] # fetch stored interpolator
+            except KeyError:
+                # if interpolator doesn't exist, construct it
+                roi = gpos
+                if self.roi is not None:
+                    roi = self.roi
+                li = self.get_interpolator(roi, x0)
+                self.idict[key] = li
+            # do the interpolation
+            gt[:, micnum] = li(gpos.T)
+        if gt.shape[1] == 1:
+            gt = gt[:, 0]
+        return c*gt #return distance along ray
+
+    def get_interpolator( self, roi, x0 ):
+        """
+        gets an LinearNDInterpolator object
+
+        Parameters
+        ----------
+        roi : array of floats of shape (3, N)
+            The locations of points in the region of interest in 3D cartesian
+            co-ordinates. Used to estimate the maximum distance and ROI
+            extension and center.
+        x0 : array of floats of shape (3)
+            The location of the microphone in 3D cartesian co-ordinates. 
+
+        Returns
+        -------
+        LinearNDInterpolator object
+        """
+        c = self.c
+
         # the DE system
         def f1(t, y, v):
             x = y[0:3]
             s = y[3:6]
             vv, dv = v(x)
             sa = sqrt(s[0]*s[0]+s[1]*s[1]+s[2]*s[2])
             x = empty(6)
@@ -595,41 +640,36 @@
             while oo.successful():
                 xyz.append(oo.y[0:3])
                 t.append(oo.t)
                 if norm(oo.y[0:3]-x0)>rmax:
                     break
                 oo.integrate(oo.t+dt)
 
-        gs2 = gpos.shape[-1]
-        gt = empty((gs2, mpos.shape[-1]))
+        gs2 = roi.shape[-1]
         vv = self.ff.v
         NN = int(sqrt(self.N))
-        for micnum, x0 in enumerate(mpos.T):
-            xe = gpos.mean(1) # center of grid
-            r = x0[:, newaxis]-gpos
-            rmax = sqrt((r*r).sum(0).max()) # maximum distance
-            nv = spiral_sphere(self.N, self.Om, b=xe-x0)
-            rstep = rmax/sqrt(self.N)
-            rmax += rstep
-            tstep = rstep/c
-            xyz = []
-            t = []
-            lastind = 0
-            for i, n0 in enumerate(nv.T):
-                fr(x0, n0, rmax, tstep, vv, xyz, t)
-                if i and i % NN == 0:
-                    if not lastind:
-                        dd = ConvexHull(vstack((gpos.T, xyz)), incremental=True)
-                    else:
-                        dd.add_points(xyz[lastind:], restart=True)
-                    lastind = len(xyz)
-                    # ConvexHull includes grid if no grid points on hull
-                    if dd.simplices.min()>=gs2:
-                        break
-            xyz = array(xyz)
-            t = array(t)
-            li = LinearNDInterpolator(xyz, t)
-            gt[:, micnum] = li(gpos.T)
-        if gt.shape[1] == 1:
-            gt = gt[:, 0]
-        return c*gt #return distance along ray
+        xe = roi.mean(1) # center of grid
+        r = x0[:, newaxis]-roi
+        rmax = sqrt((r*r).sum(0).max()) # maximum distance
+        nv = spiral_sphere(self.N, self.Om, b=xe-x0)
+        rstep = rmax/sqrt(self.N)
+        rmax += rstep
+        tstep = rstep/c
+        xyz = []
+        t = []
+        lastind = 0
+        for i, n0 in enumerate(nv.T):
+            fr(x0, n0, rmax, tstep, vv, xyz, t)
+            if i and i % NN == 0:
+                if not lastind:
+                    dd = ConvexHull(vstack((roi.T, xyz)), incremental=True)
+                else:
+                    dd.add_points(xyz[lastind:], restart=True)
+                lastind = len(xyz)
+                # ConvexHull includes grid if no grid points on hull
+                if dd.simplices.min()>=gs2:
+                    break
+        xyz = array(xyz)
+        t = array(t)
+        return LinearNDInterpolator(xyz, t)
+
```

### Comparing `acoular-22.3/acoular/fastFuncs.py` & `acoular-23.6/acoular/fastFuncs.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/fbeamform.py` & `acoular-23.6/acoular/fbeamform.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,53 +20,55 @@
     BeamformerDamas
     BeamformerDamasPlus
     BeamformerOrth
     BeamformerCleansc
     BeamformerCMF
     BeamformerSODIX
     BeamformerGIB
+    BeamformerAdaptiveGrid
+    BeamformerGridlessOrth
 
     PointSpreadFunction
     L_p
     integrate
 
 """
 
 # imports from other packages
 from __future__ import print_function, division
 
 import warnings
 
-from numpy import array, ones, full, hanning, hamming, bartlett, blackman, \
-invert, dot, newaxis, zeros, empty, fft, float32, float64, complex64, linalg, \
-where, searchsorted, pi, multiply, sign, diag, arange, sqrt, exp, log10, int,\
+from numpy import array, ones, full, \
+invert, dot, newaxis, zeros, linalg, \
+searchsorted, pi, sign, diag, arange, sqrt, log10, \
 reshape, hstack, vstack, eye, tril, size, clip, tile, round, delete, \
-absolute, argsort, sort, sum, hsplit, fill_diagonal, zeros_like, isclose, \
-vdot, flatnonzero, einsum, ndarray, isscalar, inf, real
+absolute, argsort, sum, hsplit, fill_diagonal, zeros_like, \
+einsum, ndarray, isscalar, inf, real, unique
 
 from numpy.linalg import norm
 
 from sklearn.linear_model import LassoLars, LassoLarsCV, LassoLarsIC,\
-OrthogonalMatchingPursuit, ElasticNet, OrthogonalMatchingPursuitCV, Lasso
+OrthogonalMatchingPursuitCV
 
-from scipy.optimize import nnls, linprog, fmin_l_bfgs_b
+from scipy.optimize import nnls, linprog, fmin_l_bfgs_b, shgo
 from scipy.linalg import inv, eigh, eigvals, fractional_matrix_power
 from warnings import warn
 
 #pylops imports for CMF solvers
 try:
     from  pylops import Identity, MatrixMult
     from pylops.optimization.sparsity import SplitBregman,FISTA
     PYLOPS_TRUE = True
 except:
     PYLOPS_TRUE = False
 
-from traits.api import HasPrivateTraits, Float, Int, ListInt, ListFloat, \
+from traits.api import HasPrivateTraits, Float, Int, \
 CArray, Property, Instance, Trait, Bool, Range, Delegate, Enum, Any, \
-cached_property, on_trait_change, property_depends_on
+cached_property, on_trait_change, property_depends_on, List, Tuple, Dict
 from traits.trait_errors import TraitError
 
 from .fastFuncs import beamformerFreq, calcTransfer, calcPointSpreadFunction, \
 damasSolverGaussSeidel
 
 from .h5cache import H5cache
 from .h5files import H5CacheFileBase
@@ -391,41 +393,56 @@
         global/local caching behaviour. Returns (None, None) if no cachefile/data 
         exist and global caching mode is 'readonly'.
         """
 #        print("get cachefile:", self.freq_data.basename)
         H5cache.get_cache_file( self, self.freq_data.basename ) 
         if not self.h5f: 
 #            print("no cachefile:", self.freq_data.basename)
-            return (None, None)# only happens in case of global caching readonly
+            return (None, None, None)# only happens in case of global caching readonly
 
         nodename = self.__class__.__name__ + self.digest
 #        print("collect filecache for nodename:",nodename)
         if config.global_caching == 'overwrite' and self.h5f.is_cached(nodename):
 #            print("remove existing data for nodename",nodename)
             self.h5f.remove_data(nodename) # remove old data before writing in overwrite mode
         
         if not self.h5f.is_cached(nodename):
 #            print("no data existent for nodename:", nodename)
             if config.global_caching == 'readonly': 
-                return (None, None)
+                return (None, None, None)
             else:
 #                print("initialize data.")
                 numfreq = self.freq_data.fftfreq().shape[0]# block_size/2 + 1steer_obj
                 group = self.h5f.create_new_group(nodename)
-                self.h5f.create_compressible_array('result',
-                                      (numfreq, self.steer.grid.size),
-                                      self.precision,
-                                      group)
                 self.h5f.create_compressible_array('freqs',
                                       (numfreq, ),
                                       'int8',#'bool', 
                                       group)
+                if isinstance(self,BeamformerAdaptiveGrid):
+                    self.h5f.create_compressible_array('gpos',
+                                      (3, self.size),
+                                      'float64',
+                                      group)
+                    self.h5f.create_compressible_array('result',
+                                      (numfreq, self.size),
+                                      self.precision,
+                                      group)
+                else:
+                    self.h5f.create_compressible_array('result',
+                                      (numfreq, self.steer.grid.size),
+                                      self.precision,
+                                      group)
+
         ac = self.h5f.get_data_by_reference('result','/'+nodename)
         fr = self.h5f.get_data_by_reference('freqs','/'+nodename)
-        return (ac,fr)        
+        if isinstance(self,BeamformerAdaptiveGrid):
+            gpos = self.h5f.get_data_by_reference('gpos','/'+nodename)
+        else:
+            gpos = None
+        return (ac,fr,gpos)        
 
     def _assert_equal_channels(self):
         numchannels = self.freq_data.numchannels
         if  numchannels != self.steer.mics.num_mics or numchannels == 0:
             raise ValueError("%i channels do not fit %i mics" % (numchannels, self.steer.mics.num_mics))        
 
     @property_depends_on('ext_digest')
@@ -436,38 +453,40 @@
         """
         f = self.freq_data
         numfreq = f.fftfreq().shape[0]# block_size/2 + 1steer_obj
         _digest = ''
         while self.digest != _digest:
             _digest = self.digest
             self._assert_equal_channels()
+            ac, fr = (None, None)
             if not ( # if result caching is active
                     config.global_caching == 'none' or 
                     (config.global_caching == 'individual' and self.cached == False)
                 ):
 #                print("get filecache..")
-                (ac,fr) = self._get_filecache() 
-                if ac and fr: 
+                (ac,fr,gpos) = self._get_filecache() 
+                if gpos:
+                    self._gpos = gpos
+            if ac and fr: 
 #                    print("cached data existent")
-                    if not fr[f.ind_low:f.ind_high].all():
+                if not fr[f.ind_low:f.ind_high].all():
 #                        print("calculate missing results")                            
-                        if config.global_caching == 'readonly': 
-                            (ac, fr) = (ac[:], fr[:])
-                        self.calc(ac,fr)
-                        self.h5f.flush()
+                    if config.global_caching == 'readonly': 
+                        (ac, fr) = (ac[:], fr[:])
+                    self.calc(ac,fr)
+                    self.h5f.flush()
 #                    else:
 #                        print("cached results are complete! return.")
+            else:
+#                print("no caching or not activated, calculate result")
+                if isinstance(self,BeamformerAdaptiveGrid):
+                    self._gpos = zeros((3, self.size), dtype=self.precision)
+                    ac = zeros((numfreq, self.size), dtype=self.precision)
                 else:
-#                    print("no caching, calculate result")
                     ac = zeros((numfreq, self.steer.grid.size), dtype=self.precision)
-                    fr = zeros(numfreq, dtype='int8')
-                    self.calc(ac,fr)
-            else:
-#                print("no caching activated, calculate result")
-                ac = zeros((numfreq, self.steer.grid.size), dtype=self.precision)
                 fr = zeros(numfreq, dtype='int8')
                 self.calc(ac,fr)
         return ac
       
     def sig_loss_norm(self):
         """ 
         If the diagonal of the CSM is removed one has to handle the loss 
@@ -622,15 +641,18 @@
             else:
                 h = sum(res[ind1:ind2], 0)
                 if not ((ind1 in indices) and (ind2 in indices)):
                     warn('Beamforming result may not have been calculated '
                          'for all queried frequencies. Check '
                          'freq_data.ind_low and freq_data.ind_high!',
                           Warning, stacklevel = 2)
-        return h.reshape(self.steer.grid.shape)
+        if isinstance(self,BeamformerAdaptiveGrid):
+            return h
+        else:
+            return h.reshape(self.steer.grid.shape)
 
 
     def integrate(self, sector):
         """
         Integrates result map over a given sector.
         
         Parameters
@@ -1926,16 +1948,16 @@
     Schallabstrahlung von Turbofantriebwerken, 2017. and 
     Oertwig, Advancements in the source localization method SODIX and
     application to short cowl engine data, 2019
     
     Source directivity modeling in the cross-spectral matrix
     """
     #: Type of fit method to be used ('fmin_l_bfgs_b').
-    #: These methods is implemented in 
-    #: the `scipy module.
+    #: These methods are implemented in 
+    #: the scipy module.
     method = Trait('fmin_l_bfgs_b', desc="fit method used")
         
     #: Maximum number of iterations,
     #: tradeoff between speed and precision;
     #: defaults to 200
     max_iter = Int(200, 
         desc="maximum number of iterations")
@@ -2127,15 +2149,15 @@
         its :meth:`~BeamformerSODIX.synthetic` method.        
         
         Parameters
         ----------
         ac : array of floats
             This array of dimension ([number of frequencies]x[number of gridpoints]x[number of microphones])
             is used as call-by-reference parameter and contains the calculated
-          #/= unit   value after calling this method. 
+            value after calling this method. 
         fr : array of booleans
             The entries of this [number of frequencies]-sized array are either 
             'True' (if the result for this frequency has already been calculated)
             or 'False' (for the frequencies where the result has yet to be calculated).
             After the calculation at a certain frequency the value will be set
             to 'True'
         
@@ -2410,14 +2432,180 @@
                         warn('Eigenvalue %g <= 0 for frequency index %g. Will not be calculated!' % (s, i),Warning, stacklevel = 2)
                     #Generate source maps of all selected eigenmodes, and superpose source intensity for each source type.
                 temp = zeros(numpoints)
                 temp[locpoints] = sum(absolute(qi[:,locpoints])**2,axis=0)
                 ac[i] = temp
                 fr[i] = 1    
 
+class BeamformerAdaptiveGrid(BeamformerBase,Grid):
+    """
+    Base class for array methods without predefined grid
+    """
+    
+    # the grid positions live in a shadow trait
+    _gpos = Any
+
+    def _get_shape ( self ):
+        return (self.size,)
+
+    def _get_gpos( self ):
+        return self._gpos
+
+    def integrate(self, sector):
+        """
+        Integrates result map over a given sector.
+        
+        Parameters
+        ----------
+        sector: :class:`~acoular.grids.Sector` or derived
+            Gives the sector over which to integrate
+              
+        Returns
+        -------
+        array of floats
+            The spectrum (all calculated frequency bands) for the integrated sector.
+        """
+        ind = self.subdomain(sector)
+        r = self.result
+        h = zeros(r.shape[0])
+        for i in range(r.shape[0]):
+            h[i] = r[i][ind].sum()
+        return h
+
+class BeamformerGridlessOrth(BeamformerAdaptiveGrid):
+    """
+    Orthogonal beamforming without predefined grid
+    """
+
+    #: List of components to consider, use this to directly set the eigenvalues
+    #: used in the beamformer. Alternatively, set :attr:`n`.
+    eva_list = CArray(dtype=int,
+        desc="components")
+        
+    #: Number of components to consider, defaults to 1. If set, 
+    #: :attr:`eva_list` will contain
+    #: the indices of the n largest eigenvalues. Setting :attr:`eva_list` 
+    #: afterwards will override this value.
+    n = Int(1)
+
+    #: Geometrical bounds of the search domain to consider.
+    #: :attr:`bound` ist a list that contains exactly three tuple of 
+    #: (min,max) for each of the coordinates x, y, z. 
+    #: Defaults to [(-1.,1.),(-1.,1.),(0.01,1.)]
+    bounds = List( Tuple(Float,Float), minlen=3, maxlen=3,
+        value = [(-1.,1.),(-1.,1.),(0.01,1.)])
+
+    #: options dictionary for the SHGO solver, see 
+    #: `scipy docs <https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.shgo.html>`_.
+    #: Default is Sobol sampling Nelder-Mead local minimizer, 256 initial sampling points 
+    #: and 1 iteration
+    shgo = Dict
+
+    # internal identifier
+    digest = Property( 
+        depends_on = ['freq_data.digest', '_steer_obj.digest', 'r_diag', 
+            'eva_list','bounds','shgo'], 
+        )
+   
+    @cached_property
+    def _get_digest( self ):
+        return digest( self )
+
+    @on_trait_change('n')
+    def set_eva_list(self):
+        """ sets the list of eigenvalues to consider """
+        self.eva_list = arange(-1, -1-self.n, -1)
+
+    @on_trait_change('eva_list')
+    def set_n(self):
+        """ sets the list of eigenvalues to consider """
+        self.n = self.eva_list.shape[0]
+    
+    @property_depends_on('n')
+    def _get_size ( self ):
+        return self.n*self.freq_data.fftfreq().shape[0]
+
+    def calc(self, ac, fr):
+        """
+        Calculates the result for the frequencies defined by :attr:`freq_data`
+        
+        This is an internal helper function that is automatically called when 
+        accessing the beamformer's :attr:`~BeamformerBase.result` or calling
+        its :meth:`~BeamformerBase.synthetic` method.        
+        
+        Parameters
+        ----------
+        ac : array of floats
+            This array of dimension ([number of frequencies]x[number of gridpoints])
+            is used as call-by-reference parameter and contains the calculated
+            value after calling this method. 
+        fr : array of booleans
+            The entries of this [number of frequencies]-sized array are either 
+            'True' (if the result for this frequency has already been calculated)
+            or 'False' (for the frequencies where the result has yet to be calculated).
+            After the calculation at a certain frequency the value will be set
+            to 'True'
+        
+        Returns
+        -------
+        This method only returns values through the *ac* and *fr* parameters
+        """
+        f = self.freq_data.fftfreq()
+        numchannels = self.freq_data.numchannels
+        # eigenvalue number list in standard form from largest to smallest 
+        eva_list = unique(self.eva_list % self.steer.mics.num_mics)[::-1]
+        steer_type = self.steer.steer_type
+        if steer_type == 'custom':
+            raise NotImplementedError('custom steer_type is not implemented')
+        mpos = self.steer.mics.mpos
+        env = self.steer.env
+        shgo_opts = {'n':256,'iters':1,'sampling_method':'sobol',
+                        'options':{'local_iter':1},
+                        'minimizer_kwargs':{'method':'Nelder-Mead'}
+                        }
+        shgo_opts.update(self.shgo)
+        roi = []
+        for x in self.bounds[0]:
+            for y in self.bounds[1]:
+                for z in self.bounds[2]:
+                    roi.append((x,y,z))
+        self.steer.env.roi = array(roi).T
+        bmin = array(tuple(map(min,self.bounds)))
+        bmax = array(tuple(map(max,self.bounds)))
+        for i in self.freq_data.indices:
+            if not fr[i]:
+                eva = array(self.freq_data.eva[i], dtype='float64')
+                eve = array(self.freq_data.eve[i], dtype='complex128')
+                k = 2*pi*f[i]/env.c
+                for j,n in enumerate(eva_list):
+                    #print(f[i],n)
+
+                    def func(xy):
+                        # function to minimize globally
+                        xy = clip(xy,bmin,bmax)
+                        r0 = env._r(xy[:,newaxis])
+                        rm = env._r(xy[:,newaxis],mpos)
+                        return -beamformerFreq(steer_type,
+                                                self.r_diag,
+                                                1.0,
+                                                (r0, rm, k),
+                                                (ones(1), eve[:,n:n+1]))[0][0]
+
+                    # simplical global homotopy optimizer
+                    oR = shgo(func,self.bounds,**shgo_opts)
+                    # index in grid
+                    ind = i*self.n+j 
+                    # store result for position
+                    self._gpos[:,ind] = oR['x']
+                    # store result for level
+                    ac[i,ind] = eva[n]/numchannels
+                    #print(oR['x'],eva[n]/numchannels,oR)
+                fr[i] = 1
+
+
 def L_p ( x ):
     """
     Calculates the sound pressure level from the squared sound pressure.
     
     :math:`L_p = 10 \lg ( x / 4\cdot 10^{-10})`
     
     Parameters
@@ -2447,15 +2635,15 @@
     It can, however, also be used with the 
     :meth:`Beamformer.synthetic<acoular.fbeamform.BeamformerBase.synthetic>`
     output.
     
     Parameters
     ----------
     data: array of floats
-        Contains the calculated sound pressures in Pa.        
+        Contains the calculated squared sound pressure values in Pa**2.        
         If data has the same number of entries than the number of grid points
         only one value is returned.
         In case of a 2-D array with the second dimension identical 
         to the number of grid points an array containing as many entries as
         the first dimension is returned.
     grid: Grid object 
         Object of a :class:`~acoular.grids.Grid`-derived class
```

### Comparing `acoular-22.3/acoular/fileimport.py` & `acoular-23.6/acoular/fileimport.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/grids.py` & `acoular-23.6/acoular/grids.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     RectGrid
     RectGrid3D
     ImportGrid
     LineGrid
     MergeGrid
     Sector
     RectSector
+    RectSector3D
     CircSector
     PolySector
     ConvexSector
     MultiSector
 
 """
 
@@ -714,15 +715,15 @@
     @property_depends_on('basename')
     def _get_size ( self ):
         return self.gpos.shape[-1]
 
     # 'digest' is a placeholder for other properties in derived classes
     @property_depends_on('basename')
     def _get_shape ( self ):
-        return self.gpos.shape[-1]
+        return (self.gpos.shape[-1],)
 
     @property_depends_on('basename')
     def _get_gpos( self ):
         return self.gpos_file
 
 
     subgrids = CArray(
@@ -885,15 +886,15 @@
     # 'digest' is a placeholder for other properties in derived classes
     @property_depends_on('numpoints')
     def _get_shape ( self ):
         return self.gpos.shape[-1]
 
     @property_depends_on('numpoints,length,direction,loc')
     def _get_gpos( self ):
-        dist = self.length / self.numpoints 
+        dist = self.length / (self.numpoints - 1)
         loc = array(self.loc, dtype = float).reshape((3, 1)) 
         direc_n = self.direction/norm(self.direction)
         pos = zeros((self.numpoints,3))
         for s in range(self.numpoints):
             pos[s] = (loc.T+direc_n*dist*s)
         return pos.T
 
@@ -1064,14 +1065,83 @@
         
         # if none inside, take nearest
         if ~inds.any() and self.default_nearest:
             x = (xmin + xmax) / 2.0
             y = (ymin + ymax) / 2.0
             dr2 = (pos[0, :] - x)**2 + (pos[1, :] - y)**2
             inds[argmin(dr2)] = True
+        
+        return inds.astype(bool)
+
+
+class RectSector3D( RectSector ):
+    """
+    Class for defining a cuboid sector.
+    
+    Can be used for 3D Grids for definining a cuboid sector.
+    """
+    
+    #: The lower z position of the cuboid
+    z_min = Float(-1.0,
+                  desc="minimum z position of the cuboid")
+
+    #: The upper z position of the cuboid
+    z_max = Float(1.0,
+                  desc="maximum z position of the cuboid")
+
+    def contains ( self, pos ):
+        """
+        Queries whether the coordinates in a given array lie within the 
+        rectangular sector. 
+        If no coordinate is inside, the nearest one to the rectangle center
+        is returned if :attr:`~Sector.default_nearest` is True.
+        
+        Parameters
+        ----------
+        pos : array of floats
+            Array with the shape 3x[number of gridpoints] containing the
+            grid positions
+        
+        Returns
+        -------
+        array of bools with as many entries as columns in pos
+            Array indicating which of the given positions lie within the
+            given sector                
+        """
+        # make sure xmin is minimum etc
+        xmin = min(self.x_min,self.x_max)
+        xmax = max(self.x_min,self.x_max)
+        ymin = min(self.y_min,self.y_max)
+        ymax = max(self.y_min,self.y_max)
+        zmin = min(self.z_min,self.z_max)
+        zmax = max(self.z_min,self.z_max)
+        
+        abs_tol = self.abs_tol
+        # get pos indices inside rectangle (* == and)
+        if self.include_border:
+            inds = (pos[0, :] - xmin > -abs_tol) * \
+                   (pos[0, :] - xmax < abs_tol) * \
+                   (pos[1, :] - ymin > -abs_tol) * \
+                   (pos[1, :] - ymax < abs_tol) * \
+                   (pos[2, :] - zmin > -abs_tol) * \
+                   (pos[2, :] - zmax < abs_tol)
+        else:
+            inds = (pos[0, :] - xmin > abs_tol) * \
+                   (pos[0, :] - xmax < -abs_tol) * \
+                   (pos[1, :] - ymin > abs_tol) * \
+                   (pos[1, :] - ymax < -abs_tol) * \
+                   (pos[2, :] - zmin > abs_tol) * \
+                   (pos[2, :] - zmax < -abs_tol)
+        
+        # if none inside, take nearest
+        if ~inds.any() and self.default_nearest:
+            x = (xmin + xmax) / 2.0
+            y = (ymin + ymax) / 2.0
+            dr2 = (pos[0, :] - x)**2 + (pos[1, :] - y)**2
+            inds[argmin(dr2)] = True
         
         return inds.astype(bool)
 
 
 class CircSector( Sector ):
     """
     Class for defining a circular sector.
```

### Comparing `acoular-22.3/acoular/h5cache.py` & `acoular-23.6/acoular/h5cache.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/h5files.py` & `acoular-23.6/acoular/h5files.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/microphones.py` & `acoular-23.6/acoular/microphones.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     :toctree: generated/
 
     MicGeom
 
 """
 
 # imports from other packages
-from numpy import array, average
+from numpy import array, average 
+from scipy.spatial.distance import cdist
 from traits.api import HasPrivateTraits, Property, File, \
 CArray, cached_property, on_trait_change, ListInt , Bool
 from os import path, strerror
 import errno
 
 from .internal import digest
 
@@ -52,14 +53,18 @@
     num_mics = Property( depends_on = ['mpos', ],
         desc="number of microphones in the geometry")
 
     #: Center of the array (arithmetic mean of all used array positions); readonly.
     center = Property( depends_on = ['mpos', ],
         desc="array center")
 
+    #: Aperture of the array (greatest extent between two microphones); readonly.
+    aperture = Property( depends_on = ['mpos', ],
+        desc="array aperture")
+
     #: Positions as (3, :attr:`num_mics`) array of floats, may include also invalid
     #: microphones (if any). Set either automatically on change of the
     #: :attr:`from_file` argument or explicitely by assigning an array of floats.
     mpos_tot = CArray(dtype=float,
         desc="x, y, z position of all microphones")
 
     #: Positions as (3, :attr:`num_mics`) array of floats, without invalid
@@ -97,14 +102,19 @@
     def _get_center( self ):
         if self.mpos.any():
             center = average(self.mpos,axis=1)
             # set very small values to zero
             center[abs(center) < 1e-16] = 0.
             return center
 
+    @cached_property
+    def _get_aperture( self ):
+        if self.mpos.any():
+            return cdist(self.mpos.T,self.mpos.T).max()
+
     @on_trait_change('basename')
     def import_mpos( self ):
         """
         Import the microphone positions from .xml file.
         Called when :attr:`basename` changes.
         """
         if not path.isfile(self.from_file):
```

### Comparing `acoular-22.3/acoular/nidaqimport.py` & `acoular-23.6/acoular/nidaqimport.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/sdinput.py` & `acoular-23.6/acoular/sdinput.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/signals.py` & `acoular-23.6/acoular/signals.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/sources.py` & `acoular-23.6/acoular/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,23 @@
 
 from numpy.fft import ifft, fft
 from numpy.linalg import norm
 
 import numba as nb
 
 from traits.api import Float, Int, Property, Trait, Delegate, \
-cached_property, Tuple, CLong, File, Instance, Any, \
-on_trait_change, List, ListInt, CArray, Bool, Dict, Enum
+cached_property, Tuple, CLong, File, Instance, Any, Str, \
+on_trait_change, observe, List, ListInt, CArray, Bool, Dict, Enum
 from os import path
 from warnings import warn
 
 # acoular imports
 from .calib import Calib
 from .trajectory import Trajectory
-from .internal import digest
+from .internal import digest, ldigest
 from .microphones import MicGeom
 from .environments import Environment
 from .tprocess import SamplesGenerator
 from .signals import SignalGenerator
 from .h5files import H5FileBase, _get_h5file_class
 from .tools import get_modes
 
@@ -1246,39 +1246,36 @@
     """
 
     #: List of :class:`~acoular.tprocess.SamplesGenerator` objects
     #: to be mixed.
     sources = List( Instance(SamplesGenerator, ()) ) 
 
     #: Sampling frequency of the signal.
-    sample_freq = Property( depends_on=['ldigest'] )
+    sample_freq = Property( depends_on=['sdigest'] )
     
     #: Number of channels.
-    numchannels = Property( depends_on=['ldigest'] )
+    numchannels = Property( depends_on=['sdigest'] )
                
     #: Number of samples.
-    numsamples = Property( depends_on=['ldigest'] )
+    numsamples = Property( depends_on=['sdigest'] )
     
     #: Amplitude weight(s) for the sources as array. If not set, 
     #: all source signals are equally weighted.
     #: Must match the number of sources in :attr:`sources`.
     weights = CArray(desc="channel weights")
 
-    # internal identifier
-    ldigest = Property( depends_on = ['sources.digest', ])
+    # internal identifier    
+    sdigest = Str()
 
-    # internal identifier
-    digest = Property( depends_on = ['ldigest', 'weights', '__class__'])
+    @observe('sources.items.digest')
+    def _set_sources_digest( self, event ):
+        self.sdigest = ldigest(self.sources) 
 
-    @cached_property
-    def _get_ldigest( self ):
-        res = ''
-        for s in self.sources:
-            res += s.digest
-        return res
+    # internal identifier
+    digest = Property( depends_on = ['sdigest', 'weights'])
 
     @cached_property
     def _get_digest( self ):
         return digest(self)
 
     @cached_property
     def _get_sample_freq( self ):
@@ -1302,14 +1299,16 @@
             numsamples = self.sources[0].numsamples
         else:
             numsamples = 0
         return numsamples
 
     def validate_sources( self ):
         """ Validates if sources fit together. """
+        if len(self.sources) < 1:
+            raise ValueError("Number of sources in SourceMixer should be at least 1.")
         for s in self.sources[1:]:
             if self.sample_freq != s.sample_freq:
                 raise ValueError("Sample frequency of %s does not fit" % s)
             if self.numchannels != s.numchannels:
                 raise ValueError("Channel count of %s does not fit" % s)
             if self.numsamples != s.numsamples:
                 raise ValueError("Number of samples of %s does not fit" % s)
@@ -1326,15 +1325,17 @@
             (i.e. the number of samples per block).
         
         Returns
         -------
         Samples in blocks of shape (num, numchannels). 
             The last block may be shorter than num.
         """
+        # check whether all sources fit together
         self.validate_sources()
+
         gens = [i.result(num) for i in self.sources[1:]]
         weights = self.weights.copy()
         if weights.size == 0:
             weights = array([1. for j in range(len( self.sources))])
         assert weights.shape[0] == len(self.sources)
         for temp in self.sources[0].result(num):
             temp *= weights[0]
```

### Comparing `acoular-22.3/acoular/spectra.py` & `acoular-23.6/acoular/spectra.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,36 +5,155 @@
 # Copyright (c) Acoular Development Team.
 #------------------------------------------------------------------------------
 """Estimation of power spectra and related tools
 
 .. autosummary::
     :toctree: generated/
 
+    BaseSpectra
+    FFTSpectra    
     PowerSpectra
     synthetic
+    PowerSpectraImport
 """
 from warnings import warn
 
 from numpy import array, ones, hanning, hamming, bartlett, blackman, \
-dot, newaxis, zeros, empty, fft, linalg, \
-searchsorted, isscalar, fill_diagonal, arange, zeros_like, sum
+dot, newaxis, zeros, empty, fft, linalg, sqrt,real, imag,\
+searchsorted, isscalar, fill_diagonal, arange, zeros_like, sum, ndarray
 from traits.api import HasPrivateTraits, Int, Property, Instance, Trait, \
-Range, Bool, cached_property, property_depends_on, Delegate, Float
+Bool, cached_property, property_depends_on, Delegate, Float, Enum, \
+    CArray
 
 from .fastFuncs import calcCSM
 from .h5cache import H5cache
 from .h5files import H5CacheFileBase
 from .internal import digest
-from .tprocess import SamplesGenerator
+from .tprocess import SamplesGenerator, TimeInOut
 from .calib import Calib
 from .configuration import config
 
 
+class BaseSpectra( HasPrivateTraits ):
 
-class PowerSpectra( HasPrivateTraits ):
+    #: Data source; :class:`~acoular.sources.SamplesGenerator` or derived object.
+    source = Trait(SamplesGenerator)
+
+    #: Sampling frequency of output signal, as given by :attr:`source`.
+    sample_freq = Delegate('source')
+
+    #: Number of time data channels 
+    numchannels = Delegate('source')
+
+    #: Window function for FFT, one of:
+    #:   * 'Rectangular' (default)
+    #:   * 'Hanning'
+    #:   * 'Hamming'
+    #:   * 'Bartlett'
+    #:   * 'Blackman'
+    window = Trait('Rectangular', 
+        {'Rectangular':ones, 
+        'Hanning':hanning, 
+        'Hamming':hamming, 
+        'Bartlett':bartlett, 
+        'Blackman':blackman}, 
+        desc="type of window for FFT")
+
+    #: Overlap factor for averaging: 'None'(default), '50%', '75%', '87.5%'.
+    overlap = Trait('None', {'None':1, '50%':2, '75%':4, '87.5%':8}, 
+        desc="overlap of FFT blocks")
+    
+    #: FFT block size, one of: 128, 256, 512, 1024, 2048 ... 65536,
+    #: defaults to 1024.
+    block_size = Trait(1024, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768, 65536,
+        desc="number of samples per FFT block")
+
+    #: The floating-number-precision of entries of csm, eigenvalues and 
+    #: eigenvectors, corresponding to numpy dtypes. Default is 64 bit.
+    precision = Trait('complex128', 'complex64', 
+                      desc="precision of the fft")
+    
+    # internal identifier
+    digest = Property( depends_on = ['precision','block_size',
+                                    'window','overlap'])
+
+    @cached_property
+    def _get_digest( self ):
+        return digest(self)
+
+    def fftfreq ( self ):
+        """
+        Return the Discrete Fourier Transform sample frequencies.
+        
+        Returns
+        -------
+        f : ndarray
+            Array of length *block_size/2+1* containing the sample frequencies.
+        """
+        if self.source is not None:
+            return abs(fft.fftfreq(self.block_size, 1./self.source.sample_freq)\
+                        [:int(self.block_size/2+1)])
+        else:
+            return None
+
+    #generator that yields the time data blocks for every channel (with optional overlap)
+    def get_source_data(self):
+        bs = self.block_size
+        temp = empty((2*bs, self.numchannels))
+        pos = bs
+        posinc = bs/self.overlap_
+        for data_block in self.source.result(bs):
+            ns = data_block.shape[0]
+            temp[bs:bs+ns] = data_block # fill from right
+            while pos+bs <= bs+ns:
+                yield temp[int(pos):int(pos+bs)]
+                pos += posinc
+            else:
+                temp[0:bs] = temp[bs:] # copy to left
+                pos -= bs
+
+
+class FFTSpectra( BaseSpectra,TimeInOut ):
+    """Provides the spectra of multichannel time data. 
+    
+    Returns Spectra per block over a Generator.       
+    """
+    
+    # internal identifier
+    digest = Property( depends_on = ['source.digest','precision','block_size',
+                                    'window','overlap'])
+
+    @cached_property
+    def _get_digest( self ):
+        return digest(self)
+
+    #generator that yields the fft for every channel
+    def result(self):
+        """ 
+        Python generator that yields the output block-wise.
+        
+        Parameters
+        ----------
+        num : integer
+            This parameter defines the size of the blocks to be yielded
+            (i.e. the number of samples per block).
+        
+        Returns
+        -------
+        Samples in blocks of shape (numfreq, :attr:`numchannels`). 
+            The last block may be shorter than num.
+            """
+        wind = self.window_( self.block_size )
+        weight=sqrt(2)/self.block_size*sqrt(self.block_size/dot(wind,wind))*wind[:, newaxis]
+        for data in self.get_source_data():
+            ft = fft.rfft(data*weight, None, 0).astype(self.precision)
+            yield ft
+
+
+class PowerSpectra( BaseSpectra ):
     """Provides the cross spectral matrix of multichannel time data
      and its eigen-decomposition.
     
     This class includes the efficient calculation of the full cross spectral
     matrix using the Welch method with windows and overlap. It also contains 
     the CSM's eigenvalues and eigenvectors and additional properties. 
     
@@ -44,39 +163,38 @@
     again triggered when an attribute is read. The result may be 
     cached on disk in HDF5 files and need not to be recomputed during
     subsequent program runs with identical input data and parameters. The
     input data is taken to be identical if the source has identical parameters
     and the same file name in case of that the data is read from a file.
     """
 
-    #: The :class:`~acoular.tprocess.SamplesGenerator` object that provides the data.
-    time_data = Trait(SamplesGenerator, 
+    # Shadow trait, should not be set directly, for internal use.
+    _source = Trait(SamplesGenerator)
+
+    #: Data source; :class:`~acoular.sources.SamplesGenerator` or derived object. 
+    source = Property(_source,
         desc="time data object")
 
-    #: Number of samples 
-    numchannels = Delegate('time_data')
+    #: The :class:`~acoular.tprocess.SamplesGenerator` object that provides the data.
+    time_data = Property(_source, 
+        desc="deprecated attribute holding the time data object. Use PowerSpectra.source instead!")
 
     #: The :class:`~acoular.calib.Calib` object that provides the calibration data, 
     #: defaults to no calibration, i.e. the raw time data is used.
     #:
     #: **deprecated**:      use :attr:`~acoular.sources.TimeSamples.calib` property of 
     #: :class:`~acoular.sources.TimeSamples` objects
     calib = Instance(Calib)
 
-    #: FFT block size, one of: 128, 256, 512, 1024, 2048 ... 65536,
-    #: defaults to 1024.
-    block_size = Trait(1024, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768, 65536,
-        desc="number of samples per FFT block")
-
     # Shadow trait, should not be set directly, for internal use.
     _ind_low = Int(1,
         desc="index of lowest frequency line")
 
     # Shadow trait, should not be set directly, for internal use.
-    _ind_high = Int(-1,
+    _ind_high = Trait(-1,(Int,None),
         desc="index of highest frequency line")
 
     #: Index of lowest frequency line to compute, integer, defaults to 1,
     #: is used only by objects that fetch the csm, PowerSpectra computes every
     #: frequency line.
     ind_low = Property(_ind_low,
         desc="index of lowest frequency line")
@@ -86,39 +204,21 @@
     ind_high = Property(_ind_high,
         desc="index of lowest frequency line")
 
     # Stores the set lower frequency, for internal use, should not be set directly.
     _freqlc = Float(0)
 
     # Stores the set higher frequency, for internal use, should not be set directly.
-    _freqhc = Float(0)
+    _freqhc = Trait(0,(Float,None))
 
     # Saves whether the user set indices or frequencies last, for internal use only,
     # not to be set directly, if True (default), indices are used for setting
     # the freq_range interval.
     _index_set_last = Bool(True)
-
-    #: Window function for FFT, one of:
-    #:   * 'Rectangular' (default)
-    #:   * 'Hanning'
-    #:   * 'Hamming'
-    #:   * 'Bartlett'
-    #:   * 'Blackman'
-    window = Trait('Rectangular', 
-        {'Rectangular':ones, 
-        'Hanning':hanning, 
-        'Hamming':hamming, 
-        'Bartlett':bartlett, 
-        'Blackman':blackman}, 
-        desc="type of window for FFT")
-
-    #: Overlap factor for averaging: 'None'(default), '50%', '75%', '87.5%'.
-    overlap = Trait('None', {'None':1, '50%':2, '75%':4, '87.5%':8}, 
-        desc="overlap of FFT blocks")
-        
+      
     #: Flag, if true (default), the result is cached in h5 files and need not
     #: to be recomputed during subsequent program runs.
     cached = Bool(True, 
         desc="cached flag")   
 
     #: Number of FFT blocks to average, readonly
     #: (set from block_size and overlap).
@@ -138,108 +238,133 @@
         
     #: Array with a sequence of indices for all frequencies 
     #: between :attr:`ind_low` and :attr:`ind_high` within the result, readonly.
     indices = Property(
         desc = "index range" )
         
     #: Name of the cache file without extension, readonly.
-    basename = Property( depends_on = 'time_data.digest', 
+    basename = Property( depends_on = '_source.digest', 
         desc="basename for cache file")
 
     #: The cross spectral matrix, 
     #: (number of frequencies, numchannels, numchannels) array of complex;
     #: readonly.
     csm = Property( 
         desc="cross spectral matrix")
     
-    #: The floating-number-precision of entries of csm, eigenvalues and 
-    #: eigenvectors, corresponding to numpy dtypes. Default is 64 bit.
-    precision = Trait('complex128', 'complex64', 
-                      desc="precision csm, eva, eve")
-
     #: Eigenvalues of the cross spectral matrix as an
     #: (number of frequencies) array of floats, readonly.
     eva = Property( 
         desc="eigenvalues of cross spectral matrix")
 
     #: Eigenvectors of the cross spectral matrix as an
     #: (number of frequencies, numchannels, numchannels) array of floats,
     #: readonly.
     eve = Property( 
         desc="eigenvectors of cross spectral matrix")
 
     # internal identifier
     digest = Property( 
-        depends_on = ['time_data.digest', 'calib.digest', 'block_size', 
+        depends_on = ['_source.digest', 'calib.digest', 'block_size', 
             'window', 'overlap', 'precision'], 
         )
 
     # hdf5 cache file
     h5f = Instance( H5CacheFileBase, transient = True )
     
-    @property_depends_on('time_data.numsamples, block_size, overlap')
+    @property_depends_on('_source.numsamples, block_size, overlap')
     def _get_num_blocks ( self ):
-        return self.overlap_*self.time_data.numsamples/self.block_size-\
+        return self.overlap_*self._source.numsamples/self.block_size-\
         self.overlap_+1
 
-    @property_depends_on('time_data.sample_freq, block_size, ind_low, ind_high')
+    @property_depends_on('_source.sample_freq, block_size, ind_low, ind_high')
     def _get_freq_range ( self ):
-        try:
-            return self.fftfreq()[[ self.ind_low, self.ind_high ]]
-        except IndexError:
-            return array([0., 0])
+        fftfreq = self.fftfreq()
+        if fftfreq is not None:
+            if self._ind_high is None:
+                return array([fftfreq[self.ind_low],None])
+            else:
+                return fftfreq[[ self.ind_low, self.ind_high ]]
 
     def _set_freq_range( self, freq_range ):# by setting this the user sets _freqlc and _freqhc
         self._index_set_last = False
         self._freqlc = freq_range[0]
         self._freqhc = freq_range[1]
 
-    @property_depends_on( 'time_data.sample_freq, block_size, _ind_low, _freqlc' )
+    @property_depends_on( '_source.sample_freq, block_size, _ind_low, _freqlc' )
     def _get_ind_low( self ):
-        if self._index_set_last:
-            return min(self._ind_low, self.block_size//2)
-        else:
-            return searchsorted(self.fftfreq()[:-1], self._freqlc)
+        fftfreq = self.fftfreq()
+        if fftfreq is not None:
+            if self._index_set_last:
+                return min(self._ind_low, fftfreq.shape[0]-1)
+            else:
+                return searchsorted(fftfreq[:-1], self._freqlc)
 
-    @property_depends_on( 'time_data.sample_freq, block_size, _ind_high, _freqhc' )
+    @property_depends_on( '_source.sample_freq, block_size, _ind_high, _freqhc' )
     def _get_ind_high( self ):
-        if self._index_set_last:
-            return min(self._ind_high, self.block_size//2)
-        else:
-            return searchsorted(self.fftfreq()[:-1], self._freqhc)
+        fftfreq = self.fftfreq()
+        if fftfreq is not None:
+            if self._index_set_last:
+                if self._ind_high is None: 
+                    return None
+                else:
+                    return min(self._ind_high, fftfreq.shape[0]-1)
+            else:
+                if self._freqhc is None:
+                    return None
+                else:
+                    return searchsorted(fftfreq[:-1], self._freqhc)
 
     def _set_ind_high(self, ind_high):# by setting this the user sets the lower index
         self._index_set_last = True
         self._ind_high = ind_high
 
     def _set_ind_low( self, ind_low):# by setting this the user sets the higher index
         self._index_set_last = True
         self._ind_low = ind_low
 
+    def _set_time_data(self, time_data):
+        self._source = time_data
+
+    def _set_source(self, source):
+        self._source = source
+
+    def _get_time_data(self):
+        return self._source
+
+    def _get_source(self):
+        return self._source
+
     @property_depends_on( 'block_size, ind_low, ind_high' )
     def _get_indices ( self ):
-        try:
-            return arange(self.block_size/2+1,dtype=int)[ self.ind_low: self.ind_high ]
-        except IndexError:
-            return range(0)
+        fftfreq = self.fftfreq()
+        if fftfreq is not None:
+            try:
+                indices = arange(fftfreq.shape[0],dtype=int)
+                if self.ind_high is None:
+                    return indices[ self.ind_low:]
+                else:
+                    return indices[ self.ind_low: self.ind_high ]
+            except IndexError:
+                return range(0)
 
     @cached_property
     def _get_digest( self ):
         return digest( self )
 
     @cached_property
     def _get_basename( self ):
-        if 'basename' in self.time_data.all_trait_names():
-            return self.time_data.basename
+        if 'basename' in self._source.all_trait_names():
+            return self._source.basename
         else: 
-            return self.time_data.__class__.__name__ + self.time_data.digest
+            return self._source.__class__.__name__ + self._source.digest
 
     def calc_csm( self ):
         """ csm calculation """
-        t = self.time_data
+        t = self.source
         wind = self.window_( self.block_size )
         weight = dot( wind, wind )
         wind = wind[newaxis, :].swapaxes( 0, 1 )
         numfreq = int(self.block_size/2 + 1)
         csm_shape = (numfreq, t.numchannels, t.numchannels)
         csmUpper = zeros(csm_shape, dtype=self.precision)
         #print "num blocks", self.num_blocks
@@ -247,33 +372,22 @@
         if self.calib and self.calib.num_mics > 0:
             if self.calib.num_mics == t.numchannels:
                 wind = wind * self.calib.data[newaxis, :]
             else:
                 raise ValueError(
                         "Calibration data not compatible: %i, %i" % \
                         (self.calib.num_mics, t.numchannels))
-        bs = self.block_size
-        temp = empty((2*bs, t.numchannels))
-        pos = bs
-        posinc = bs/self.overlap_
-        for data in t.result(bs):
-            ns = data.shape[0]
-            temp[bs:bs+ns] = data
-            while pos+bs <= bs+ns:
-                ft = fft.rfft(temp[int(pos):int(pos+bs)]*wind, None, 0).astype(self.precision)
-                calcCSM(csmUpper, ft)  # only upper triangular part of matrix is calculated (for speed reasons)
-                pos += posinc
-            temp[0:bs] = temp[bs:]
-            pos -= bs
-        
+        # get time data blockwise
+        for data in self.get_source_data():
+            ft = fft.rfft(data*wind, None, 0).astype(self.precision)
+            calcCSM(csmUpper, ft)  # only upper triangular part of matrix is calculated (for speed reasons)
         # create the full csm matrix via transposing and complex conj.
         csmLower = csmUpper.conj().transpose(0,2,1)
         [fill_diagonal(csmLower[cntFreq, :, :], 0) for cntFreq in range(csmLower.shape[0])]
         csm = csmLower + csmUpper
-
         # onesided spectrum: multiplication by 2.0=sqrt(2)^2
         csm = csm*(2.0/self.block_size/weight/self.num_blocks)
         return csm
 
     def calc_ev ( self ):
         """ eigenvalues / eigenvectors calculation """
         if self.precision == 'complex128': eva_dtype = 'float64'
@@ -291,15 +405,15 @@
         return self.calc_ev()[0]
     
     def calc_eve( self ):
         """ calculates eigenvectors of csm """
         return self.calc_ev()[1]
                 
     def _handle_dual_calibration(self):
-        obj = self.time_data # start with time_data obj
+        obj = self.source # start with time_data obj
         while obj:
             if 'calib' in obj.all_trait_names(): # at original source?
                 if obj.calib and self.calib:
                     if obj.calib.digest == self.calib.digest:
                         self.calib = None # ignore it silently
                     else:
                         raise ValueError("Non-identical dual calibration for "\
@@ -315,15 +429,15 @@
         """
         function handles result caching of csm, eigenvectors and eigenvalues
         calculation depending on global/local caching behaviour.  
         """
         if traitname == 'csm':
             func = self.calc_csm
             numfreq = int(self.block_size/2 + 1)
-            shape = (numfreq, self.time_data.numchannels, self.time_data.numchannels)
+            shape = (numfreq, self._source.numchannels, self._source.numchannels)
             precision = self.precision
         elif traitname == 'eva':
             func = self.calc_eva
             shape = self.csm.shape[0:2]
             if self.precision == 'complex128': precision = 'float64'
             elif self.precision == 'complex64': precision = 'float32'
         elif traitname == 'eve':
@@ -359,43 +473,43 @@
         Main work is done here:
         Cross spectral matrix is either loaded from cache file or
         calculated and then additionally stored into cache.
         """
         self._handle_dual_calibration()
         if (
                 config.global_caching == 'none' or 
-                (config.global_caching == 'individual' and self.cached == False)
+                (config.global_caching == 'individual' and self.cached is False)
             ):
             return self.calc_csm()
         else:
             return self._get_filecache('csm')
                           
     @property_depends_on('digest')
     def _get_eva ( self ):
         """
         Eigenvalues of cross spectral matrix are either loaded from cache file or
         calculated and then additionally stored into cache.
         """
         if (
                 config.global_caching == 'none' or 
-                (config.global_caching == 'individual' and self.cached == False)
+                (config.global_caching == 'individual' and self.cached is False)
             ):
             return self.calc_eva()
         else:
             return self._get_filecache('eva')
 
     @property_depends_on('digest')
     def _get_eve ( self ):
         """
         Eigenvectors of cross spectral matrix are either loaded from cache file or
         calculated and then additionally stored into cache.
         """
         if (
                 config.global_caching == 'none' or 
-                (config.global_caching == 'individual' and self.cached == False)
+                (config.global_caching == 'individual' and self.cached is False)
             ):
             return self.calc_eve()
         else:
             return self._get_filecache('eve')
 
     def synthetic_ev( self, freq, num=0):
         """Return synthesized frequency band values of the eigenvalues.
@@ -432,29 +546,14 @@
             f2 = searchsorted(f, freq*2.**(0.5/num))
             if f1 == f2:
                 return self.eva[f1]
             else:
                 return sum(self.eva[f1:f2], 0)
 
 
-    def fftfreq ( self ):
-        """
-        Return the Discrete Fourier Transform sample frequencies.
-        
-        Returns
-        -------
-        f : ndarray
-            Array of length *block_size/2+1* containing the sample frequencies.
-        """
-        return abs(fft.fftfreq(self.block_size, 1./self.time_data.sample_freq)\
-                    [:int(self.block_size/2+1)])
-
-
-
-
 
 def synthetic (data, freqs, f, num=3):
     """
     Returns synthesized frequency band values of spectral data.
     
     If used with :meth:`Beamformer.result()<acoular.fbeamform.BeamformerBase.result>` 
     and only one frequency band, the output is identical to the result of the intrinsic 
@@ -462,15 +561,15 @@
     It can, however, also be used with the 
     :meth:`Beamformer.integrate<acoular.fbeamform.BeamformerBase.integrate>`
     output and more frequency bands.
     
     Parameters
     ----------
     data : array of floats
-        The spectral data (sound pressures in Pa) in an array with one value 
+        The spectral data (squared sound pressures in Pa^2) in an array with one value 
         per frequency line.
         The number of entries must be identical to the number of
         grid points.
     freq : array of floats
         The frequencies that correspon to the input *data* (as yielded by
         the :meth:`PowerSpectra.fftfreq<acoular.spectra.PowerSpectra.fftfreq>`
         method).
@@ -534,7 +633,146 @@
                      Warning, stacklevel = 2)
                 h = zeros_like(data[0])
             else:
                 h = sum(data[ind1:ind2], 0)
             res += [h]
     return array(res)
 
+
+class PowerSpectraImport( PowerSpectra ):
+    """Provides a dummy class for using pre-calculated cross-spectral
+    matrices. 
+
+    This class does not calculate the cross-spectral matrix. Instead, 
+    the user can inject one or multiple existing CSMs by setting the 
+    :attr:`csm` attribute. This can be useful when algorithms shall be
+    evaluated with existing CSM matrices.
+    The frequency or frequencies contained by the CSM must be set via the 
+    attr:`frequencies` attribute. The attr:`numchannels` attributes
+    is determined on the basis of the CSM shape. 
+    In contrast to the PowerSpectra object, the attributes 
+    :attr:`sample_freq`, :attr:`time_data`, :attr:`source`,
+    :attr:`block_size`, :attr:`calib`, :attr:`window`, 
+    :attr:`overlap`, :attr:`cached`, and :attr:`num_blocks`
+    have no functionality. 
+    """
+
+    #: The cross spectral matrix, 
+    #: (number of frequencies, numchannels, numchannels) array of complex;
+    #: readonly.
+    csm = Property( 
+        desc="cross spectral matrix")
+
+    #: frequencies included in the cross-spectral matrix in ascending order.
+    #: Compound trait that accepts arguments of type list, array, and float
+    frequencies = Trait(None,(CArray,Float),
+        desc="frequencies included in the cross-spectral matrix")
+
+    #: Number of time data channels 
+    numchannels = Property(depends_on=['digest'])
+
+    time_data = Enum(None, 
+        desc="PowerSpectraImport cannot consume time data")
+
+    source = Enum(None, 
+        desc="PowerSpectraImport cannot consume time data")
+
+    # Sampling frequency of the signal, defaults to None
+    sample_freq = Enum(None, 
+        desc="sampling frequency")
+
+    block_size = Enum(None, 
+        desc="PowerSpectraImport does not operate on blocks of time data")
+
+    calib = Enum(None,
+        desc="PowerSpectraImport cannot calibrate the time data")
+
+    window = Enum(None,
+            desc="PowerSpectraImport does not perform windowing")
+
+    overlap = Enum(None,
+            desc="PowerSpectraImport does not consume time data")
+
+    cached = Enum(False,
+            desc="PowerSpectraImport has no caching capabilities")
+
+    num_blocks = Enum(None,
+            desc="PowerSpectraImport cannot determine the number of blocks")
+
+    # Shadow trait, should not be set directly, for internal use.
+    _ind_low = Int(0,
+        desc="index of lowest frequency line")
+
+    # Shadow trait, should not be set directly, for internal use.
+    _ind_high = Trait(None,(Int,None),
+        desc="index of highest frequency line")
+
+    # internal identifier
+    digest = Property( 
+        depends_on = ['_csmsum', 
+            ], 
+        )
+
+    #: Name of the cache file without extension, readonly.
+    basename = Property( depends_on = 'digest', 
+        desc="basename for cache file")
+
+    # csm shadow trait, only for internal use.
+    _csm = CArray()
+        
+    # CSM checksum to trigger digest calculation, only for internal use.
+    _csmsum = Float() 
+
+    def _get_basename( self ):
+        return "csm_import_"+self.digest
+
+    @cached_property
+    def _get_digest( self ):
+        return digest( self )
+
+    def _get_numchannels( self ):
+        return self.csm.shape[1]
+
+    def _get_csm ( self ):
+        return self._csm
+
+    def _set_csm (self, csm):
+        if (len(csm.shape) != 3) or (csm.shape[1] != csm.shape[2]):
+            raise ValueError(
+                "The cross spectral matrix must have the following shape: (number of frequencies, numchannels, numchannels)!")
+        self._csmsum = real(self._csm).sum() + (imag(self._csm)**2).sum() # to trigger new digest creation
+        self._csm = csm
+
+    @property_depends_on('digest')
+    def _get_eva ( self ):
+        """
+        Eigenvalues of cross spectral matrix are either loaded from cache file or
+        calculated and then additionally stored into cache.
+        """
+        return self.calc_eva()
+
+    @property_depends_on('digest')
+    def _get_eve ( self ):
+        """
+        Eigenvectors of cross spectral matrix are either loaded from cache file or
+        calculated and then additionally stored into cache.
+        """
+        return self.calc_eve()
+
+    def fftfreq ( self ):
+        """
+        Return the Discrete Fourier Transform sample frequencies.
+        
+        Returns
+        -------
+        f : ndarray
+            Array containing the frequencies.
+        """
+        if isinstance(self.frequencies,float): 
+            return array([self.frequencies])
+        elif isinstance(self.frequencies,ndarray):
+            return self.frequencies
+        elif self.frequencies is None:
+            warn("No frequencies defined for PowerSpectraImport object!")
+            return self.frequencies
+        else:
+            return self.frequencies
```

### Comparing `acoular-22.3/acoular/tbeamform.py` & `acoular-23.6/acoular/tbeamform.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/tfastfuncs.py` & `acoular-23.6/acoular/tfastfuncs.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/tools.py` & `acoular-23.6/acoular/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,17 @@
     Returns azimuthal and elevation angles between the mics and the source 
     
     Parameters
     ----------
     direction : array of floats
         Spherical Harmonic orientation
     mpos : array of floats
-            x, y, z position of microphones
+        x, y, z position of microphones
     sourceposition : array of floats
-            position of the source
-            
-        ========================
+        position of the source        
         
     Returns
     -------
     azi, ele : array of floats
         the angle between the mics and the source 
     """
     #direction of the Spherical Harmonics
@@ -113,19 +111,17 @@
     Parameters
     ----------
     lOrder : int
         Maximal order of spherical harmonic
     direction : array of floats
         Spherical Harmonic orientation
     mpos : array of floats
-            x, y, z position of microphones
+        x, y, z position of microphones
     sourceposition : array of floats
-            position of the source
-            
-        ========================
+        position of the source
 
     Returns
     -------
     modes : array of floats
         the radiation values at each microphone for each mode
     """
     azi, ele = get_radiation_angles(direction,mpos,sourceposition) # angles between source and mics
```

### Comparing `acoular-22.3/acoular/tprocess.py` & `acoular-23.6/acoular/tprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,31 +45,32 @@
 from numpy.linalg import norm
 from numpy.matlib import repmat
 
 from scipy.spatial import Delaunay
 from scipy.interpolate import LinearNDInterpolator,splrep, splev, \
 CloughTocher2DInterpolator, CubicSpline, Rbf
 from traits.api import HasPrivateTraits, Float, Int, CLong, Bool, ListInt, \
-Constant, File, Property, Instance, Trait, Delegate, \
-cached_property, on_trait_change, List, CArray, Dict, PrefixMap, Callable
+Constant, File, Property, Instance, Trait, Delegate, Str, \
+cached_property, on_trait_change, List, CArray, Dict, PrefixMap, Callable,\
+observe
 
 from scipy.fft import rfft, irfft
 import numba as nb
 
 from datetime import datetime
 from os import path
 import wave
 from scipy.signal import butter, lfilter, filtfilt, bilinear
 from warnings import warn
 from collections import deque
 from inspect import currentframe
 import threading
 
 # acoular imports
-from .internal import digest
+from .internal import digest, ldigest
 from .h5cache import H5cache
 from .h5files import H5CacheFileBase, _get_h5file_class
 from .environments import cartToCyl,cylToCart
 from .microphones import MicGeom
 from .configuration import config
 
 
@@ -90,18 +91,18 @@
     #: Number of channels 
     numchannels = CLong
                
     #: Number of samples 
     numsamples = CLong
     
     # internal identifier
-    digest = Property
+    digest = Property(depends_on = ['sample_freq', 'numchannels', 'numsamples'])
     
     def _get_digest( self ): 
-        return '' 
+        return digest( self )
                
     def result(self, num):
         """
         Python generator that yields the output block-wise.
                 
         Parameters
         ----------
@@ -1241,32 +1242,28 @@
     
     #: Number of channels in output as given by :attr:`source`.
     numchannels = Delegate('source')
                
     #: Number of samples in output as given by :attr:`source`.
     numsamples = Delegate('source')
 
-    # internal identifier
-    ldigest = Property( depends_on = ['sources.digest', ])
+    # internal identifier    
+    sdigest = Str()
 
+    @observe('sources.items.digest')
+    def _set_sources_digest( self, event ):
+        self.sdigest = ldigest(self.sources) 
+    
     # internal identifier
-    digest = Property( depends_on = ['sources','source.digest', 'ldigest', '__class__'])
-
-    @cached_property
-    def _get_ldigest( self ):
-        res = ''
-        for s in self.sources:
-            res += s.digest
-        return res
+    digest = Property( depends_on = ['source.digest','sdigest'])
 
     @cached_property
     def _get_digest( self ):
         return digest(self)
 
-    @on_trait_change('sources,source')
     def validate_sources( self ):
         """ validates if sources fit together """
         if self.source:
             for s in self.sources:
                 if self.sample_freq != s.sample_freq:
                     raise ValueError("Sample frequency of %s does not fit" % s)
                 if self.numchannels != s.numchannels:
@@ -1285,14 +1282,18 @@
             (i.e. the number of samples per block).
         
         Returns
         -------
         Samples in blocks of shape (num, numchannels). 
             The last block may be shorter than num.
         """
+        
+        # check whether all sources fit together
+        self.validate_sources()
+        
         gens = [i.result(num) for i in self.sources]
         for temp in self.source.result(num):
             sh = temp.shape[0]
             for g in gens:
                 temp1 = next(g)
                 if temp.shape[0] > temp1.shape[0]:
                     temp = temp[:temp1.shape[0]]
```

### Comparing `acoular-22.3/acoular/traitsviews.py` & `acoular-23.6/acoular/traitsviews.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/trajectory.py` & `acoular-23.6/acoular/trajectory.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/HW90D240_f10.xml` & `acoular-23.6/acoular/xml/HW90D240_f10.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/W90_D105_f10.xml` & `acoular-23.6/acoular/xml/W90_D105_f10.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/acousticam_2c.xml` & `acoular-23.6/acoular/xml/acousticam_2c.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/acousticam_4c.xml` & `acoular-23.6/acoular/xml/acousticam_4c.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array38.xml` & `acoular-23.6/acoular/xml/array38.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array92x.xml` & `acoular-23.6/acoular/xml/array92x.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array_56.xml` & `acoular-23.6/acoular/xml/array_56.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array_56_10_9.xml` & `acoular-23.6/acoular/xml/array_56_10_9.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array_56_bomb.xml` & `acoular-23.6/acoular/xml/array_56_bomb.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array_56_v2.xml` & `acoular-23.6/acoular/xml/array_56_v2.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array_64.xml` & `acoular-23.6/acoular/xml/array_64.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array_84_10_9.xml` & `acoular-23.6/acoular/xml/array_84_10_9.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/array_84_bomb_v3.xml` & `acoular-23.6/acoular/xml/array_84_bomb_v3.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/calib_vw_ring32.xml` & `acoular-23.6/acoular/xml/calib_vw_ring32.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/gfai_ring32.xml` & `acoular-23.6/acoular/xml/gfai_ring32.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/minidsp_uma16.xml` & `acoular-23.6/acoular/xml/minidsp_uma16.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/acoular/xml/tub_vogel64.xml` & `acoular-23.6/acoular/xml/tub_vogel64.xml`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/acoular_demo.py` & `acoular-23.6/examples/acoular_demo.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/basic_beamformer_example.py` & `acoular-23.6/examples/basic_beamformer_example.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_3D_beamforming.py` & `acoular-23.6/examples/example_3D_beamforming.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_SampleSplitter_bufferhandling.py` & `acoular-23.6/examples/example_SampleSplitter_bufferhandling.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_SampleSplitter_multithreading.py` & `acoular-23.6/examples/example_SampleSplitter_multithreading.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_airfoil_in_open_jet_beamforming.py` & `acoular-23.6/examples/example_airfoil_in_open_jet_beamforming.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_airfoil_in_open_jet_cmf.py` & `acoular-23.6/examples/example_airfoil_in_open_jet_cmf.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_airfoil_in_open_jet_steering_vectors.py` & `acoular-23.6/examples/example_airfoil_in_open_jet_steering_vectors.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_airfoil_in_open_jet_time_beamforming.py` & `acoular-23.6/examples/example_airfoil_in_open_jet_time_beamforming.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_rotating_point_source.py` & `acoular-23.6/examples/example_rotating_point_source.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_sectors_and_intergration.py` & `acoular-23.6/examples/example_sectors_and_intergration.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/example_tools.py` & `acoular-23.6/examples/example_tools.py`

 * *Files identical despite different names*

### Comparing `acoular-22.3/examples/three_sources.py` & `acoular-23.6/examples/three_sources.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 1      (-0.1,-0.1,0.3) 1 Pa
 2      (0.15,0,0.3)    0.7 Pa 
 3      (0,0.1,0.3)     0.5 Pa
 ====== =============== ======
 """
 
 from os import path
-from acoular import __file__ as bpath, td_dir, MicGeom, WNoiseGenerator, PointSource, Mixer, WriteH5
+from acoular import __file__ as bpath, MicGeom, WNoiseGenerator, PointSource, Mixer, WriteH5
 
 sfreq = 51200
 duration = 1
 nsamples = duration*sfreq
 micgeofile = path.join(path.split(bpath)[0],'xml','array_64.xml')
 h5savefile = 'three_sources.h5'
 
 m = MicGeom(from_file=micgeofile)
 n1 = WNoiseGenerator(sample_freq=sfreq, numsamples=nsamples, seed=1)
 n2 = WNoiseGenerator(sample_freq=sfreq, numsamples=nsamples, seed=2, rms=0.7)
 n3 = WNoiseGenerator(sample_freq=sfreq, numsamples=nsamples, seed=3, rms=0.5)
-p1 = PointSource(signal=n1, mpos=m,  loc=(-0.1,-0.1,0.3))
-p2 = PointSource(signal=n2, mpos=m,  loc=(0.15,0,0.3))
-p3 = PointSource(signal=n3, mpos=m,  loc=(0,0.1,0.3))
+p1 = PointSource(signal=n1, mics=m,  loc=(-0.1,-0.1,0.3))
+p2 = PointSource(signal=n2, mics=m,  loc=(0.15,0,0.3))
+p3 = PointSource(signal=n3, mics=m,  loc=(0,0.1,0.3))
 p = Mixer(source=p1, sources=[p2,p3])
 wh5 = WriteH5(source=p, name=h5savefile)
 wh5.save()
```

