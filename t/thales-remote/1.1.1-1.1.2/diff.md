# Comparing `tmp/thales_remote-1.1.1.tar.gz` & `tmp/thales_remote-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thales_remote-1.1.1.tar", last modified: Mon Apr  3 07:53:21 2023, max compression
+gzip compressed data, was "thales_remote-1.1.2.tar", last modified: Mon Jun 26 09:51:46 2023, max compression
```

## Comparing `thales_remote-1.1.1.tar` & `thales_remote-1.1.2.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.922275 thales_remote-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-03 07:53:11.000000 thales_remote-1.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.910275 thales_remote-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.910275 thales_remote-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-03 07:53:11.000000 thales_remote-1.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-03 07:53:11.000000 thales_remote-1.1.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.910275 thales_remote-1.1.1/Examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.910275 thales_remote-1.1.1/Examples/BCMuxInterface/
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/BCMuxInterface/BCMuxInterface.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/BCMuxInterface/BCMuxInterface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.910275 thales_remote-1.1.1/Examples/BasicIntroduction/
--rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/BasicIntroduction/BasicIntroduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/BasicIntroduction/BasicIntroduction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.914275 thales_remote-1.1.1/Examples/CVImportPlot/
--rw-r--r--   0 runner    (1001) docker     (123)    75349 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/CVImportPlot/CV.svg
--rw-r--r--   0 runner    (1001) docker     (123)   203489 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/CVImportPlot/CVImportPlot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/CVImportPlot/CVImportPlot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.914275 thales_remote-1.1.1/Examples/CurrentVoltageCurve/
--rw-r--r--   0 runner    (1001) docker     (123)    44828 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/CurrentVoltageCurve/CurrentVoltageCurve.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/CurrentVoltageCurve/CurrentVoltageCurve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.914275 thales_remote-1.1.1/Examples/CyclicVoltammetry/
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/CyclicVoltammetry/CyclicVoltammetry.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/CyclicVoltammetry/CyclicVoltammetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.914275 thales_remote-1.1.1/Examples/DCSequencer/
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/DCSequencer/DCSequencer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/DCSequencer/DCSequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.914275 thales_remote-1.1.1/Examples/DynamicDCSequenceEIS/
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/DynamicDCSequenceEIS/DynamicDCSequenceEIS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/DynamicDCSequenceEIS/DynamicDCSequenceEIS.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/DynamicDCSequenceEIS/ocp_constant_current_template.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.914275 thales_remote-1.1.1/Examples/EIS/
--rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EIS/EIS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EIS/EIS.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.914275 thales_remote-1.1.1/Examples/EISCVLaTeX/
--rw-r--r--   0 runner    (1001) docker     (123)   206372 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISCVLaTeX/C1234.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISCVLaTeX/CV.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISCVLaTeX/EIS.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISCVLaTeX/EIS.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   369746 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISCVLaTeX/EISCVLaTeX.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISCVLaTeX/EISCVLaTeX.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISCVLaTeX/report.tex
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISCVLaTeX/report_filled.tex
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/EISImportPlot/
--rw-r--r--   0 runner    (1001) docker     (123)   234455 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISImportPlot/EISImportPlot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISImportPlot/EISImportPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)    91808 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISImportPlot/bode.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33909 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISImportPlot/nyquist.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/EISPad4/
--rw-r--r--   0 runner    (1001) docker     (123)   112053 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISPad4/EISPad4.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISPad4/EISPad4.py
--rw-r--r--   0 runner    (1001) docker     (123)    49687 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISPad4/nyquist.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/EISvsParameter/
--rw-r--r--   0 runner    (1001) docker     (123)   120866 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISvsParameter/EISvsParameter.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISvsParameter/EISvsParameter.py
--rw-r--r--   0 runner    (1001) docker     (123)   332372 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISvsParameter/impedance_contour.svg
--rw-r--r--   0 runner    (1001) docker     (123)   176623 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/EISvsParameter/phase_contour.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/ExternalDeviceFRA/
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/ExternalDeviceFRA/ExternalDeviceFRA.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/ExternalDeviceFRA/ExternalDeviceFRA.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/FileExchangeEIS/
--rw-r--r--   0 runner    (1001) docker     (123)    72500 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/FileExchangeEIS/FileExchangeEIS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/FileExchangeEIS/FileExchangeEIS.py
--rw-r--r--   0 runner    (1001) docker     (123)   271847 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/FileExchangeEIS/thales_python.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/HeartBeat/
--rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/HeartBeat/HeartBeat.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/HeartBeat/HeartBeat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/HeartBeatLiveData/
--rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/HeartBeatLiveData/HeartBeatLiveData.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/HeartBeatLiveData/HeartBeatLiveData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/ImpedanceMultiCellCycle/
--rw-r--r--   0 runner    (1001) docker     (123)    23771 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/ImpedanceMultiCellCycle/ImpedanceMultiCellCycle.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/ImpedanceMultiCellCycle/ImpedanceMultiCellCycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.918275 thales_remote-1.1.1/Examples/ImpedanceRampHotSwap/
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/ImpedanceRampHotSwap/ImpedanceRampHotSwap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/ImpedanceRampHotSwap/ImpedanceRampHotSwap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/LICENSE_jupyterlab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.922275 thales_remote-1.1.1/Examples/LoadWithExternalSource/
--rw-r--r--   0 runner    (1001) docker     (123)   363197 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/LoadWithExternalSource/EL1002_Supply.png
--rw-r--r--   0 runner    (1001) docker     (123)    93499 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/LoadWithExternalSource/LoadWithExternalSource.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/LoadWithExternalSource/LoadWithExternalSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-03 07:53:11.000000 thales_remote-1.1.1/Examples/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-03 07:53:11.000000 thales_remote-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-03 07:53:21.922275 thales_remote-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-04-03 07:53:11.000000 thales_remote-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.922275 thales_remote-1.1.1/delta_remote/
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-04-03 07:53:11.000000 thales_remote-1.1.1/delta_remote/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-03 07:53:11.000000 thales_remote-1.1.1/delta_remote/original_delta_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-04-03 07:53:11.000000 thales_remote-1.1.1/delta_remote/script_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-03 07:53:11.000000 thales_remote-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 07:53:21.922275 thales_remote-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.922275 thales_remote-1.1.1/thales_remote/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-03 07:53:11.000000 thales_remote-1.1.1/thales_remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-04-03 07:53:11.000000 thales_remote-1.1.1/thales_remote/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-04-03 07:53:11.000000 thales_remote-1.1.1/thales_remote/epc_scpi_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-03 07:53:11.000000 thales_remote-1.1.1/thales_remote/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-04-03 07:53:11.000000 thales_remote-1.1.1/thales_remote/file_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    67075 2023-04-03 07:53:11.000000 thales_remote-1.1.1/thales_remote/script_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 07:53:21.922275 thales_remote-1.1.1/thales_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13810 2023-04-03 07:53:21.000000 thales_remote-1.1.1/thales_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-04-03 07:53:21.000000 thales_remote-1.1.1/thales_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 07:53:21.000000 thales_remote-1.1.1/thales_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-03 07:53:21.000000 thales_remote-1.1.1/thales_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-03 07:53:21.000000 thales_remote-1.1.1/thales_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.121754 thales_remote-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-26 09:51:35.000000 thales_remote-1.1.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.101754 thales_remote-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.105754 thales_remote-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 09:51:35.000000 thales_remote-1.1.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 09:51:35.000000 thales_remote-1.1.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.105754 thales_remote-1.1.2/Examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.105754 thales_remote-1.1.2/Examples/BCMuxInterface/
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/BCMuxInterface/BCMuxInterface.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/BCMuxInterface/BCMuxInterface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.105754 thales_remote-1.1.2/Examples/BasicIntroduction/
+-rw-r--r--   0 runner    (1001) docker     (123)    14081 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/BasicIntroduction/BasicIntroduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/BasicIntroduction/BasicIntroduction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.109754 thales_remote-1.1.2/Examples/CVImportPlot/
+-rw-r--r--   0 runner    (1001) docker     (123)    75349 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/CVImportPlot/CV.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   203489 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/CVImportPlot/CVImportPlot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/CVImportPlot/CVImportPlot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.109754 thales_remote-1.1.2/Examples/CurrentVoltageCurve/
+-rw-r--r--   0 runner    (1001) docker     (123)    44828 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/CurrentVoltageCurve/CurrentVoltageCurve.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/CurrentVoltageCurve/CurrentVoltageCurve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.109754 thales_remote-1.1.2/Examples/CyclicVoltammetry/
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/CyclicVoltammetry/CyclicVoltammetry.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/CyclicVoltammetry/CyclicVoltammetry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.109754 thales_remote-1.1.2/Examples/DCSequencer/
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/DCSequencer/DCSequencer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/DCSequencer/DCSequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.109754 thales_remote-1.1.2/Examples/DynamicDCSequenceEIS/
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/DynamicDCSequenceEIS/DynamicDCSequenceEIS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/DynamicDCSequenceEIS/DynamicDCSequenceEIS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/DynamicDCSequenceEIS/ocp_constant_current_template.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.109754 thales_remote-1.1.2/Examples/EIS/
+-rw-r--r--   0 runner    (1001) docker     (123)     8676 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EIS/EIS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EIS/EIS.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.109754 thales_remote-1.1.2/Examples/EISCVLaTeX/
+-rw-r--r--   0 runner    (1001) docker     (123)   206372 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISCVLaTeX/C1234.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISCVLaTeX/CV.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISCVLaTeX/EIS.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISCVLaTeX/EIS.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   369746 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISCVLaTeX/EISCVLaTeX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISCVLaTeX/EISCVLaTeX.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISCVLaTeX/report.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISCVLaTeX/report_filled.tex
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.113754 thales_remote-1.1.2/Examples/EISImportPlot/
+-rw-r--r--   0 runner    (1001) docker     (123)   234455 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISImportPlot/EISImportPlot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISImportPlot/EISImportPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91808 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISImportPlot/bode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33909 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISImportPlot/nyquist.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.113754 thales_remote-1.1.2/Examples/EISPad4/
+-rw-r--r--   0 runner    (1001) docker     (123)   112053 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISPad4/EISPad4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISPad4/EISPad4.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49687 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISPad4/nyquist.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.113754 thales_remote-1.1.2/Examples/EISvsParameter/
+-rw-r--r--   0 runner    (1001) docker     (123)   120866 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISvsParameter/EISvsParameter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISvsParameter/EISvsParameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   332372 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISvsParameter/impedance_contour.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   176623 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/EISvsParameter/phase_contour.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.113754 thales_remote-1.1.2/Examples/ExternalDeviceFRA/
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/ExternalDeviceFRA/ExternalDeviceFRA.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/ExternalDeviceFRA/ExternalDeviceFRA.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.113754 thales_remote-1.1.2/Examples/FileExchangeEIS/
+-rw-r--r--   0 runner    (1001) docker     (123)    72500 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/FileExchangeEIS/FileExchangeEIS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/FileExchangeEIS/FileExchangeEIS.py
+-rw-r--r--   0 runner    (1001) docker     (123)   271847 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/FileExchangeEIS/thales_python.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.117754 thales_remote-1.1.2/Examples/HeartBeat/
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/HeartBeat/HeartBeat.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/HeartBeat/HeartBeat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.117754 thales_remote-1.1.2/Examples/HeartBeatLiveData/
+-rw-r--r--   0 runner    (1001) docker     (123)    14924 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/HeartBeatLiveData/HeartBeatLiveData.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/HeartBeatLiveData/HeartBeatLiveData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.117754 thales_remote-1.1.2/Examples/ImpedanceMultiCellCycle/
+-rw-r--r--   0 runner    (1001) docker     (123)    23771 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/ImpedanceMultiCellCycle/ImpedanceMultiCellCycle.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/ImpedanceMultiCellCycle/ImpedanceMultiCellCycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.117754 thales_remote-1.1.2/Examples/ImpedanceRampHotSwap/
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/ImpedanceRampHotSwap/ImpedanceRampHotSwap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/ImpedanceRampHotSwap/ImpedanceRampHotSwap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/LICENSE_jupyterlab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.117754 thales_remote-1.1.2/Examples/LoadWithExternalSource/
+-rw-r--r--   0 runner    (1001) docker     (123)   363197 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/LoadWithExternalSource/EL1002_Supply.png
+-rw-r--r--   0 runner    (1001) docker     (123)    93499 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/LoadWithExternalSource/LoadWithExternalSource.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/LoadWithExternalSource/LoadWithExternalSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-26 09:51:35.000000 thales_remote-1.1.2/Examples/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-26 09:51:35.000000 thales_remote-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-06-26 09:51:46.121754 thales_remote-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11205 2023-06-26 09:51:35.000000 thales_remote-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.117754 thales_remote-1.1.2/delta_remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-06-26 09:51:35.000000 thales_remote-1.1.2/delta_remote/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-26 09:51:35.000000 thales_remote-1.1.2/delta_remote/original_delta_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-26 09:51:35.000000 thales_remote-1.1.2/delta_remote/script_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-26 09:51:35.000000 thales_remote-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:51:46.121754 thales_remote-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.117754 thales_remote-1.1.2/thales_remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 09:51:35.000000 thales_remote-1.1.2/thales_remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-06-26 09:51:35.000000 thales_remote-1.1.2/thales_remote/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13665 2023-06-26 09:51:35.000000 thales_remote-1.1.2/thales_remote/epc_scpi_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-26 09:51:35.000000 thales_remote-1.1.2/thales_remote/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14107 2023-06-26 09:51:35.000000 thales_remote-1.1.2/thales_remote/file_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68002 2023-06-26 09:51:35.000000 thales_remote-1.1.2/thales_remote/script_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:51:46.121754 thales_remote-1.1.2/thales_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-06-26 09:51:46.000000 thales_remote-1.1.2/thales_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-26 09:51:46.000000 thales_remote-1.1.2/thales_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:51:46.000000 thales_remote-1.1.2/thales_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-26 09:51:46.000000 thales_remote-1.1.2/thales_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 09:51:46.000000 thales_remote-1.1.2/thales_remote.egg-info/top_level.txt
```

### Comparing `thales_remote-1.1.1/Examples/BCMuxInterface/BCMuxInterface.ipynb` & `thales_remote-1.1.2/Examples/BCMuxInterface/BCMuxInterface.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/BCMuxInterface/BCMuxInterface.py` & `thales_remote-1.1.2/Examples/BCMuxInterface/BCMuxInterface.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/BasicIntroduction/BasicIntroduction.ipynb` & `thales_remote-1.1.2/Examples/BasicIntroduction/BasicIntroduction.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/BasicIntroduction/BasicIntroduction.py` & `thales_remote-1.1.2/Examples/BasicIntroduction/BasicIntroduction.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/CVImportPlot/CV.svg` & `thales_remote-1.1.2/Examples/CVImportPlot/CV.svg`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/CVImportPlot/CVImportPlot.ipynb` & `thales_remote-1.1.2/Examples/CVImportPlot/CVImportPlot.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/CVImportPlot/CVImportPlot.py` & `thales_remote-1.1.2/Examples/CVImportPlot/CVImportPlot.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/CurrentVoltageCurve/CurrentVoltageCurve.ipynb` & `thales_remote-1.1.2/Examples/CurrentVoltageCurve/CurrentVoltageCurve.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/CurrentVoltageCurve/CurrentVoltageCurve.py` & `thales_remote-1.1.2/Examples/CurrentVoltageCurve/CurrentVoltageCurve.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/CyclicVoltammetry/CyclicVoltammetry.ipynb` & `thales_remote-1.1.2/Examples/CyclicVoltammetry/CyclicVoltammetry.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/CyclicVoltammetry/CyclicVoltammetry.py` & `thales_remote-1.1.2/Examples/CyclicVoltammetry/CyclicVoltammetry.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/DCSequencer/DCSequencer.ipynb` & `thales_remote-1.1.2/Examples/DCSequencer/DCSequencer.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/DCSequencer/DCSequencer.py` & `thales_remote-1.1.2/Examples/DCSequencer/DCSequencer.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/DynamicDCSequenceEIS/DynamicDCSequenceEIS.ipynb` & `thales_remote-1.1.2/Examples/DynamicDCSequenceEIS/DynamicDCSequenceEIS.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/DynamicDCSequenceEIS/DynamicDCSequenceEIS.py` & `thales_remote-1.1.2/Examples/DynamicDCSequenceEIS/DynamicDCSequenceEIS.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EIS/EIS.ipynb` & `thales_remote-1.1.2/Examples/EIS/EIS.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EIS/EIS.py` & `thales_remote-1.1.2/Examples/EIS/EIS.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISCVLaTeX/C1234.pdf` & `thales_remote-1.1.2/Examples/EISCVLaTeX/C1234.pdf`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISCVLaTeX/CV.pdf` & `thales_remote-1.1.2/Examples/EISCVLaTeX/CV.pdf`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISCVLaTeX/EIS.csv` & `thales_remote-1.1.2/Examples/EISCVLaTeX/EIS.csv`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISCVLaTeX/EIS.pdf` & `thales_remote-1.1.2/Examples/EISCVLaTeX/EIS.pdf`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISCVLaTeX/EISCVLaTeX.ipynb` & `thales_remote-1.1.2/Examples/EISCVLaTeX/EISCVLaTeX.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISCVLaTeX/EISCVLaTeX.py` & `thales_remote-1.1.2/Examples/EISCVLaTeX/EISCVLaTeX.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISCVLaTeX/report.tex` & `thales_remote-1.1.2/Examples/EISCVLaTeX/report.tex`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISCVLaTeX/report_filled.tex` & `thales_remote-1.1.2/Examples/EISCVLaTeX/report_filled.tex`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISImportPlot/EISImportPlot.ipynb` & `thales_remote-1.1.2/Examples/EISImportPlot/EISImportPlot.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISImportPlot/EISImportPlot.py` & `thales_remote-1.1.2/Examples/EISImportPlot/EISImportPlot.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISImportPlot/bode.svg` & `thales_remote-1.1.2/Examples/EISImportPlot/bode.svg`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISImportPlot/nyquist.svg` & `thales_remote-1.1.2/Examples/EISImportPlot/nyquist.svg`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISPad4/EISPad4.ipynb` & `thales_remote-1.1.2/Examples/EISPad4/EISPad4.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISPad4/EISPad4.py` & `thales_remote-1.1.2/Examples/EISPad4/EISPad4.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISPad4/nyquist.svg` & `thales_remote-1.1.2/Examples/EISPad4/nyquist.svg`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISvsParameter/EISvsParameter.ipynb` & `thales_remote-1.1.2/Examples/EISvsParameter/EISvsParameter.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISvsParameter/EISvsParameter.py` & `thales_remote-1.1.2/Examples/EISvsParameter/EISvsParameter.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISvsParameter/impedance_contour.svg` & `thales_remote-1.1.2/Examples/EISvsParameter/impedance_contour.svg`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/EISvsParameter/phase_contour.svg` & `thales_remote-1.1.2/Examples/EISvsParameter/phase_contour.svg`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/ExternalDeviceFRA/ExternalDeviceFRA.ipynb` & `thales_remote-1.1.2/Examples/ExternalDeviceFRA/ExternalDeviceFRA.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/ExternalDeviceFRA/ExternalDeviceFRA.py` & `thales_remote-1.1.2/Examples/ExternalDeviceFRA/ExternalDeviceFRA.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/FileExchangeEIS/FileExchangeEIS.ipynb` & `thales_remote-1.1.2/Examples/FileExchangeEIS/FileExchangeEIS.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/FileExchangeEIS/FileExchangeEIS.py` & `thales_remote-1.1.2/Examples/FileExchangeEIS/FileExchangeEIS.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/FileExchangeEIS/thales_python.png` & `thales_remote-1.1.2/Examples/FileExchangeEIS/thales_python.png`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/HeartBeat/HeartBeat.ipynb` & `thales_remote-1.1.2/Examples/HeartBeat/HeartBeat.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/HeartBeat/HeartBeat.py` & `thales_remote-1.1.2/Examples/HeartBeat/HeartBeat.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/HeartBeatLiveData/HeartBeatLiveData.ipynb` & `thales_remote-1.1.2/Examples/HeartBeatLiveData/HeartBeatLiveData.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/HeartBeatLiveData/HeartBeatLiveData.py` & `thales_remote-1.1.2/Examples/HeartBeatLiveData/HeartBeatLiveData.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/ImpedanceMultiCellCycle/ImpedanceMultiCellCycle.ipynb` & `thales_remote-1.1.2/Examples/ImpedanceMultiCellCycle/ImpedanceMultiCellCycle.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/ImpedanceMultiCellCycle/ImpedanceMultiCellCycle.py` & `thales_remote-1.1.2/Examples/ImpedanceMultiCellCycle/ImpedanceMultiCellCycle.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/ImpedanceRampHotSwap/ImpedanceRampHotSwap.ipynb` & `thales_remote-1.1.2/Examples/ImpedanceRampHotSwap/ImpedanceRampHotSwap.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/ImpedanceRampHotSwap/ImpedanceRampHotSwap.py` & `thales_remote-1.1.2/Examples/ImpedanceRampHotSwap/ImpedanceRampHotSwap.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/LICENSE_jupyterlab` & `thales_remote-1.1.2/Examples/LICENSE_jupyterlab`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/LoadWithExternalSource/EL1002_Supply.png` & `thales_remote-1.1.2/Examples/LoadWithExternalSource/EL1002_Supply.png`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/LoadWithExternalSource/LoadWithExternalSource.ipynb` & `thales_remote-1.1.2/Examples/LoadWithExternalSource/LoadWithExternalSource.ipynb`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/LoadWithExternalSource/LoadWithExternalSource.py` & `thales_remote-1.1.2/Examples/LoadWithExternalSource/LoadWithExternalSource.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/Examples/jupyter_utils.py` & `thales_remote-1.1.2/Examples/jupyter_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,15 @@
                 notebookText += "\n"
 
     jupyterName = jupyterNotebookName.replace("ipynb", "py")
     with open(jupyterName, "wb") as f:
         f.write(notebookText.encode(encoding="UTF-8"))
 
     os.system(f"python -m black {jupyterName}")
+    os.system(f"python -m black {jupyterNotebookName}")
     return
 
 
 def executionInNotebook():
     """Check if the code is executed in jupyter enviroment.
 
     This function checks if the execution of the code is done in python or in jupyter.
```

### Comparing `thales_remote-1.1.1/LICENSE` & `thales_remote-1.1.2/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Zahner-elektrik
+Copyright (c) 2023 Zahner-Elektrik
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `thales_remote-1.1.1/PKG-INFO` & `thales_remote-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: thales_remote
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library to control Zahner Zennium potentiostats
 Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
 License: MIT License
         
-        Copyright (c) 2023 Zahner-elektrik
+        Copyright (c) 2023 Zahner-Elektrik
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -233,15 +233,15 @@
 * Operation of the power potentiostats standalone without thales with the Python package [zahner_potentiostat](https://github.com/Zahner-elektrik/zahner_potentiostat)
 
 ## [BCMuxInterface.ipynb](Examples/BCMuxInterface/BCMuxInterface.ipynb)
 
 * Remote control of the BC-MUX
 * Class which realizes the remote control
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send a [mail](mailto:support@zahner.de?subject=Thales-Remote-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with an appropriate title and description in the [Thales-Remote-Python repository issue tracker](https://github.com/Zahner-elektrik/Thales-Remote-Python/issues). Or send a [mail](mailto:support@zahner.de?subject=Thales-Remote-Python%20Question&body=Your%20Message) to our support team.  
 If you have already found a solution to your issue or feature, **we would be happy to review your pull request**!
```

### Comparing `thales_remote-1.1.1/README.md` & `thales_remote-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 * Operation of the power potentiostats standalone without thales with the Python package [zahner_potentiostat](https://github.com/Zahner-elektrik/zahner_potentiostat)
 
 ## [BCMuxInterface.ipynb](Examples/BCMuxInterface/BCMuxInterface.ipynb)
 
 * Remote control of the BC-MUX
 * Class which realizes the remote control
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send a [mail](mailto:support@zahner.de?subject=Thales-Remote-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with an appropriate title and description in the [Thales-Remote-Python repository issue tracker](https://github.com/Zahner-elektrik/Thales-Remote-Python/issues). Or send a [mail](mailto:support@zahner.de?subject=Thales-Remote-Python%20Question&body=Your%20Message) to our support team.  
 If you have already found a solution to your issue or feature, **we would be happy to review your pull request**!
```

### Comparing `thales_remote-1.1.1/delta_remote/connection.py` & `thales_remote-1.1.2/delta_remote/connection.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/delta_remote/original_delta_example.py` & `thales_remote-1.1.2/delta_remote/original_delta_example.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/delta_remote/script_wrapper.py` & `thales_remote-1.1.2/delta_remote/script_wrapper.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/pyproject.toml` & `thales_remote-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/thales_remote/connection.py` & `thales_remote-1.1.2/thales_remote/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
         time.sleep(0.4)
 
         self._connectionName = connection_name
         payload_length = len(connection_name)
 
         registration_packet = bytearray()
-        registration_packet += bytearray(struct.pack("<H", payload_length))
+        registration_packet += bytearray(struct.pack(">H", payload_length))
         registration_packet += bytearray([0x12, 0xD0, 0xFF, 0xFF, 0xFF, 0xFF])
         registration_packet += bytearray(connection_name, "ASCII")
 
         # print("\n" + str(datetime.now().time()) + " send:")
         # print(f"payload_length: {payload_length}")
         # print(f"registration_packet: {registration_packet}")
         # print("complete packet:" + str(registration_packet))
```

### Comparing `thales_remote-1.1.1/thales_remote/epc_scpi_handler.py` & `thales_remote-1.1.2/thales_remote/epc_scpi_handler.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/thales_remote/error.py` & `thales_remote-1.1.2/thales_remote/error.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/thales_remote/file_interface.py` & `thales_remote-1.1.2/thales_remote/file_interface.py`

 * *Files identical despite different names*

### Comparing `thales_remote-1.1.1/thales_remote/script_wrapper.py` & `thales_remote-1.1.2/thales_remote/script_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,22 @@
 
         :returns: the measured potential value
         """
         return self._requestValueAndParseUsingRegexp(
             "POTENTIAL", "potential=\s*(.*?)V?[\r\n]{0,2}$"
         )
 
+    def getVoltage(self) -> float:
+        """
+        fead the measured potential from the device
+
+        :returns: the measured potential value
+        """
+        return self.getPotential()
+
     def setCurrent(self, current: float) -> str:
         """
         set the output current
 
         :param current: the output current to set
         :returns: response string from the device
         """
@@ -364,14 +372,35 @@
 
         :returns: the device name
         """
         reply = self.executeRemoteCommand("ALLNUM")
         match = re.search("(.*);(.*);([a-zA-Z]*)", reply)
         return match.group(3)
 
+    def readSetup(self) -> str:
+        """
+        read the currently set parameters
+
+        A string containing the configuration is returned.
+        For Example:
+
+        .. code-block::
+
+            OK;SETUP;Pset=1.0000e-05;Cset=1.0000e-06;Frq=1.0000e+03;Ampl=0.0000e+00;Nw=1;Pot=0;Gal=0;GAL=0;Cmin=-3.0000e+00;Cmax=3.0000e+00;Pmin=-5.2377e+00;Pmax=5.2377e+00;DEV=0;EPC=0;MAXDEV=4;ENDSETUP
+
+        :returns: reponse string from the device
+        """
+        reply = self.executeRemoteCommand("SENDSETUP")
+        if reply.find("ERROR") >= 0:
+            raise ThalesRemoteError(
+                reply.rstrip("\r")
+                + ThalesRemoteScriptWrapper.undefindedStandardErrorString
+            )
+        return reply
+
     def calibrateOffsets(self) -> str:
         """
         perform offset calibration on the device
 
         When the instrument has warmed up for about 30 minutes,
         this command can be used to perform the offset calibration again.
```

### Comparing `thales_remote-1.1.1/thales_remote.egg-info/PKG-INFO` & `thales_remote-1.1.2/thales_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: thales-remote
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library to control Zahner Zennium potentiostats
 Author-email: Maximilian Krapp <maximilian.krapp@zahner.de>
 License: MIT License
         
-        Copyright (c) 2023 Zahner-elektrik
+        Copyright (c) 2023 Zahner-Elektrik
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -233,15 +233,15 @@
 * Operation of the power potentiostats standalone without thales with the Python package [zahner_potentiostat](https://github.com/Zahner-elektrik/zahner_potentiostat)
 
 ## [BCMuxInterface.ipynb](Examples/BCMuxInterface/BCMuxInterface.ipynb)
 
 * Remote control of the BC-MUX
 * Class which realizes the remote control
 
-# 📧 Haveing a question?
+# 📧 Having a question?
 
 Send a [mail](mailto:support@zahner.de?subject=Thales-Remote-Python%20Question&body=Your%20Message) to our support team.
 
 # ⁉️ Found a bug or missing a specific feature?
 
 Feel free to **create a new issue** with an appropriate title and description in the [Thales-Remote-Python repository issue tracker](https://github.com/Zahner-elektrik/Thales-Remote-Python/issues). Or send a [mail](mailto:support@zahner.de?subject=Thales-Remote-Python%20Question&body=Your%20Message) to our support team.  
 If you have already found a solution to your issue or feature, **we would be happy to review your pull request**!
```

### Comparing `thales_remote-1.1.1/thales_remote.egg-info/SOURCES.txt` & `thales_remote-1.1.2/thales_remote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

