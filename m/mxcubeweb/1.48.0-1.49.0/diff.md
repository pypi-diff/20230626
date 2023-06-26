# Comparing `tmp/mxcubeweb-1.48.0.tar.gz` & `tmp/mxcubeweb-1.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxcubeweb-1.48.0.tar", max compression
+gzip compressed data, was "mxcubeweb-1.49.0.tar", max compression
```

## Comparing `mxcubeweb-1.48.0.tar` & `mxcubeweb-1.49.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     7652 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/LICENSE
--rw-r--r--   0        0        0     3638 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/README.md
--rw-r--r--   0        0        0     3688 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/__init__.py
--rw-r--r--   0        0        0    18485 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/app.py
--rw-r--r--   0        0        0     1409 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/config.py
--rw-r--r--   0        0        0        0 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/__init__.py
--rw-r--r--   0        0        0     2408 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/actuator_adapter.py
--rw-r--r--   0        0        0    13582 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/adapter_base.py
--rw-r--r--   0        0        0     1846 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/beam_adapter.py
--rw-r--r--   0        0        0     1642 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/beamline_action_adapter.py
--rw-r--r--   0        0        0     3063 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/beamline_adapter.py
--rw-r--r--   0        0        0     1586 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/data_publisher_adapter.py
--rw-r--r--   0        0        0      494 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/detector_adapter.py
--rw-r--r--   0        0        0      988 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/diffractometer_adapter.py
--rw-r--r--   0        0        0      591 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/energy_adapter.py
--rw-r--r--   0        0        0     1384 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/flux_adapter.py
--rw-r--r--   0        0        0     1992 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/machine_info_adapter.py
--rw-r--r--   0        0        0     2218 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/motor_adapter.py
--rw-r--r--   0        0        0     1763 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/nstate_adapter.py
--rw-r--r--   0        0        0     2905 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/adapter/wavelength_adapter.py
--rw-r--r--   0        0        0    12293 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/beamline.py
--rw-r--r--   0        0        0     1384 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/chat.py
--rw-r--r--   0        0        0      630 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/component_base.py
--rw-r--r--   0        0        0     1246 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/gphl_workflow.py
--rw-r--r--   0        0        0    16902 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/lims.py
--rw-r--r--   0        0        0    90191 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/queue.py
--rw-r--r--   0        0        0    18591 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/samplechanger.py
--rw-r--r--   0        0        0    22573 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/sampleview.py
--rw-r--r--   0        0        0     1896 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/user/database.py
--rw-r--r--   0        0        0      418 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/user/dummyusermanager.py
--rw-r--r--   0        0        0    15116 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/user/usermanager.py
--rw-r--r--   0        0        0     1986 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/components/workflow.py
--rw-r--r--   0        0        0     2344 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/models/adaptermodels.py
--rw-r--r--   0        0        0     3070 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/models/configmodels.py
--rw-r--r--   0        0        0      254 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/models/generic.py
--rw-r--r--   0        0        0     3359 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/models/usermodels.py
--rw-r--r--   0        0        0     2344 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/util/adapterutils.py
--rw-r--r--   0        0        0     1630 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/util/convertutils.py
--rw-r--r--   0        0        0      523 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/util/fsutils.py
--rw-r--r--   0        0        0     4507 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/core/util/networkutils.py
--rw-r--r--   0        0        0     1188 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/logging_handler.py
--rw-r--r--   0        0        0        0 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/__init__.py
--rw-r--r--   0        0        0     8128 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/beamline.py
--rw-r--r--   0        0        0      859 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/detector.py
--rw-r--r--   0        0        0     4033 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/diffractometer.py
--rw-r--r--   0        0        0      587 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/gphl_workflow.py
--rw-r--r--   0        0        0     5165 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/lims.py
--rw-r--r--   0        0        0     1223 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/log.py
--rw-r--r--   0        0        0     3307 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/login.py
--rw-r--r--   0        0        0     2613 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/main.py
--rw-r--r--   0        0        0     4291 2023-06-26 07:35:54.970174 mxcubeweb-1.48.0/mxcube3/routes/mockups.py
--rw-r--r--   0        0        0    10369 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/routes/queue.py
--rw-r--r--   0        0        0     6224 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/routes/ra.py
--rw-r--r--   0        0        0    13766 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/routes/samplecentring.py
--rw-r--r--   0        0        0     4671 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/routes/samplechanger.py
--rw-r--r--   0        0        0    20592 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/routes/signals.py
--rw-r--r--   0        0        0     1125 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/routes/workflow.py
--rw-r--r--   0        0        0     7600 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/server.py
--rw-r--r--   0        0        0     1396 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/state_storage.py
--rw-r--r--   0        0        0      771 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/templates/characterisation-results.js
--rw-r--r--   0        0        0     3610 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/templates/data-collection-results.html
--rw-r--r--   0        0        0   329138 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/templates/precompiled.templates.min.js
--rw-r--r--   0        0        0      721 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/templates/workflow-results.js
--rw-r--r--   0        0        0       22 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/version.py
--rw-r--r--   0        0        0        0 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/video/__init__.py
--rw-r--r--   0        0        0     2647 2023-06-26 07:35:54.974174 mxcubeweb-1.48.0/mxcube3/video/websocket-relay.js
--rw-r--r--   0        0        0     1785 2023-06-26 07:36:16.306312 mxcubeweb-1.48.0/pyproject.toml
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 mxcubeweb-1.48.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/LICENSE
+-rw-r--r--   0        0        0     3638 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/README.md
+-rw-r--r--   0        0        0     3688 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/__init__.py
+-rw-r--r--   0        0        0    18662 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/app.py
+-rw-r--r--   0        0        0     1409 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/config.py
+-rw-r--r--   0        0        0        0 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/__init__.py
+-rw-r--r--   0        0        0     2408 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/actuator_adapter.py
+-rw-r--r--   0        0        0    13582 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/adapter_base.py
+-rw-r--r--   0        0        0     1846 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/beam_adapter.py
+-rw-r--r--   0        0        0     1642 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/beamline_action_adapter.py
+-rw-r--r--   0        0        0     3063 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/beamline_adapter.py
+-rw-r--r--   0        0        0     1586 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/data_publisher_adapter.py
+-rw-r--r--   0        0        0      494 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/detector_adapter.py
+-rw-r--r--   0        0        0      988 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/diffractometer_adapter.py
+-rw-r--r--   0        0        0      591 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/energy_adapter.py
+-rw-r--r--   0        0        0     1384 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/flux_adapter.py
+-rw-r--r--   0        0        0     1992 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/machine_info_adapter.py
+-rw-r--r--   0        0        0     2218 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/motor_adapter.py
+-rw-r--r--   0        0        0     1763 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/nstate_adapter.py
+-rw-r--r--   0        0        0     2905 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/adapter/wavelength_adapter.py
+-rw-r--r--   0        0        0    12293 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/beamline.py
+-rw-r--r--   0        0        0     1384 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/chat.py
+-rw-r--r--   0        0        0      630 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/component_base.py
+-rw-r--r--   0        0        0     1246 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/gphl_workflow.py
+-rw-r--r--   0        0        0    16902 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/lims.py
+-rw-r--r--   0        0        0    90191 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/queue.py
+-rw-r--r--   0        0        0    18591 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/samplechanger.py
+-rw-r--r--   0        0        0    22573 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/sampleview.py
+-rw-r--r--   0        0        0     1896 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/user/database.py
+-rw-r--r--   0        0        0      418 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/user/dummyusermanager.py
+-rw-r--r--   0        0        0    15144 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/user/usermanager.py
+-rw-r--r--   0        0        0     1986 2023-06-26 08:37:14.562204 mxcubeweb-1.49.0/mxcube3/core/components/workflow.py
+-rw-r--r--   0        0        0     2344 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/core/models/adaptermodels.py
+-rw-r--r--   0        0        0     3070 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/core/models/configmodels.py
+-rw-r--r--   0        0        0      254 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/core/models/generic.py
+-rw-r--r--   0        0        0     3359 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/core/models/usermodels.py
+-rw-r--r--   0        0        0     2344 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/core/util/adapterutils.py
+-rw-r--r--   0        0        0     1630 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/core/util/convertutils.py
+-rw-r--r--   0        0        0      523 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/core/util/fsutils.py
+-rw-r--r--   0        0        0     4647 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/core/util/networkutils.py
+-rw-r--r--   0        0        0     1188 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/logging_handler.py
+-rw-r--r--   0        0        0        0 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/__init__.py
+-rw-r--r--   0        0        0     8128 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/beamline.py
+-rw-r--r--   0        0        0      859 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/detector.py
+-rw-r--r--   0        0        0     4033 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/diffractometer.py
+-rw-r--r--   0        0        0      587 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/gphl_workflow.py
+-rw-r--r--   0        0        0     5165 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/lims.py
+-rw-r--r--   0        0        0     1223 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/log.py
+-rw-r--r--   0        0        0     3307 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/login.py
+-rw-r--r--   0        0        0     2471 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/main.py
+-rw-r--r--   0        0        0     4291 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/mockups.py
+-rw-r--r--   0        0        0    10369 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/queue.py
+-rw-r--r--   0        0        0     6224 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/ra.py
+-rw-r--r--   0        0        0    13766 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/samplecentring.py
+-rw-r--r--   0        0        0     4671 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/samplechanger.py
+-rw-r--r--   0        0        0    20592 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/signals.py
+-rw-r--r--   0        0        0     1125 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/routes/workflow.py
+-rw-r--r--   0        0        0     7438 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/server.py
+-rw-r--r--   0        0        0     1396 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/state_storage.py
+-rw-r--r--   0        0        0      771 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/templates/characterisation-results.js
+-rw-r--r--   0        0        0     3610 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/templates/data-collection-results.html
+-rw-r--r--   0        0        0   329138 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/templates/precompiled.templates.min.js
+-rw-r--r--   0        0        0      721 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/templates/workflow-results.js
+-rw-r--r--   0        0        0       22 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/version.py
+-rw-r--r--   0        0        0        0 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/video/__init__.py
+-rw-r--r--   0        0        0     2647 2023-06-26 08:37:14.566204 mxcubeweb-1.49.0/mxcube3/video/websocket-relay.js
+-rw-r--r--   0        0        0     1785 2023-06-26 08:37:35.754387 mxcubeweb-1.49.0/pyproject.toml
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 mxcubeweb-1.49.0/PKG-INFO
```

### Comparing `mxcubeweb-1.48.0/LICENSE` & `mxcubeweb-1.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/README.md` & `mxcubeweb-1.49.0/README.md`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/__init__.py` & `mxcubeweb-1.49.0/mxcube3/__init__.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/app.py` & `mxcubeweb-1.49.0/mxcube3/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import os
 import sys
 import logging
 import traceback
 import atexit
 import json
+import time
 
 from pathlib import Path
 from urllib.parse import urlparse
 from logging import StreamHandler
 from logging.handlers import TimedRotatingFileHandler
 
 from mxcubecore import HardwareRepository as HWR
@@ -179,14 +180,15 @@
                     for item in MXCUBECore.adapter_dict.values()
                 ],
             )
         )
 
 
 class MXCUBEApplication:
+    t0 = time.time()
     # Below variables used for internal application state
 
     # SampleID and sample data of currently mounted sample, to handle samples
     # that are not mounted by sample changer.
     CURRENTLY_MOUNTED_SAMPLE = ""
 
     # Sample location of sample that are in process of being mounted
@@ -292,14 +294,16 @@
         MXCUBEApplication.init_signal_handlers()
         atexit.register(MXCUBEApplication.app_atexit)
 
         # Install server-side UI state storage
         MXCUBEApplication.init_state_storage()
 
         # MXCUBEApplication.load_settings()
+        msg = "MXCuBE 3 initialized, it took %.1f seconds" % (time.time() - MXCUBEApplication.t0)
+        logging.getLogger("MX3.HWR").info(msg)
 
     @staticmethod
     def init_sample_video(_format, port):
         """
         Initializes video streaming
         :return: None
         """
@@ -427,15 +431,15 @@
                     adapter = mxcore.get_adapter(component_data.attribute)
                     adapter_cls_name = type(adapter).__name__
                     value_type = adapter.adapter_type
                 except AttributeError:
                     msg = f"{component_data.attribute} not accessible via Beamline object. "
                     msg += f"Verify that beamline.{component_data.attribute} is valid and/or "
                     msg += f"{component_data.attribute} accessible via get_role "
-                    msg += "check ui.yaml configuration file. " 
+                    msg += "check ui.yaml configuration file. "
                     msg += "(attribute will NOT be avilable in UI)"
                     logging.getLogger("HWR").warning(msg)
                     adapter_cls_name = ""
                     value_type = ""
                 else:
                     adapter_cls_name = adapter_cls_name.replace("Adapter", "")
```

### Comparing `mxcubeweb-1.48.0/mxcube3/config.py` & `mxcubeweb-1.49.0/mxcube3/config.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/actuator_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/actuator_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/adapter_base.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/adapter_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/beam_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/beam_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/beamline_action_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/beamline_action_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/beamline_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/beamline_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/data_publisher_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/data_publisher_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/diffractometer_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/diffractometer_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/energy_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/energy_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/flux_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/flux_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/machine_info_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/machine_info_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/motor_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/motor_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/nstate_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/nstate_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/adapter/wavelength_adapter.py` & `mxcubeweb-1.49.0/mxcube3/core/adapter/wavelength_adapter.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/beamline.py` & `mxcubeweb-1.49.0/mxcube3/core/components/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/chat.py` & `mxcubeweb-1.49.0/mxcube3/core/components/chat.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/component_base.py` & `mxcubeweb-1.49.0/mxcube3/core/components/component_base.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/gphl_workflow.py` & `mxcubeweb-1.49.0/mxcube3/core/components/gphl_workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/lims.py` & `mxcubeweb-1.49.0/mxcube3/core/components/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/queue.py` & `mxcubeweb-1.49.0/mxcube3/core/components/queue.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/samplechanger.py` & `mxcubeweb-1.49.0/mxcube3/core/components/samplechanger.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/sampleview.py` & `mxcubeweb-1.49.0/mxcube3/core/components/sampleview.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/user/database.py` & `mxcubeweb-1.49.0/mxcube3/core/components/user/database.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/user/usermanager.py` & `mxcubeweb-1.49.0/mxcube3/core/components/user/usermanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,20 +221,22 @@
 
     def is_authenticated(self):
         return current_user.is_authenticated()
 
     def force_signout_user(self, username):
         user = self.get_user(username)
 
-        if not user.in_control:
+        if not user.in_control or current_user.is_anonymous:
+            socketio_sid = user.socketio_session_id
+            self.app.server.user_datastore.delete_user(user)
+            self.app.server.user_datastore.commit()
             self.app.server.emit(
-                "forceSignoutObservers", room=user.socketio_session_id, namespace="/hwr"
+                "forceSignout", room=socketio_sid, namespace="/hwr"
             )
 
-            self.app.server.user_datastore.deactivate_user(user)
 
     def login_info(self):
         res = {
             "synchrotronName": HWR.beamline.session.synchrotron_name,
             "beamlineName": HWR.beamline.session.beamline_name,
             "loggedIn": False,
             "loginType": HWR.beamline.lims.loginType.title(),
@@ -376,17 +378,15 @@
             "inhouse": inhouse,
         }
 
         active_users = self.active_logged_in_users()
 
         if login_id in active_users:
             if current_user.is_anonymous:
-                raise Exception(
-                    "Login rejected, you are already logged in somewhere else"
-                )
+                self.force_signout_user(login_id)
             else:
                 if current_user.username == login_id:
                     raise Exception("You are already logged in here")
                 else:
                     raise Exception(
                         "Login rejected, you are already logged in somewhere else\nand Another user is already logged in here"
                     )
```

### Comparing `mxcubeweb-1.48.0/mxcube3/core/components/workflow.py` & `mxcubeweb-1.49.0/mxcube3/core/components/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/models/adaptermodels.py` & `mxcubeweb-1.49.0/mxcube3/core/models/adaptermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/models/configmodels.py` & `mxcubeweb-1.49.0/mxcube3/core/models/configmodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/models/usermodels.py` & `mxcubeweb-1.49.0/mxcube3/core/models/usermodels.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/util/adapterutils.py` & `mxcubeweb-1.49.0/mxcube3/core/util/adapterutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/util/convertutils.py` & `mxcubeweb-1.49.0/mxcube3/core/util/convertutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/util/fsutils.py` & `mxcubeweb-1.49.0/mxcube3/core/util/fsutils.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/core/util/networkutils.py` & `mxcubeweb-1.49.0/mxcube3/core/util/networkutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,28 @@
 
 from flask_login import current_user, login_required
 from mxcubecore import HardwareRepository as HWR
 
 
 def RateLimited(maxPerSecond):
     minInterval = 1.0 / float(maxPerSecond)
-
+    lastTimeCalled = {}
     def decorate(func):
-        lastTimeCalled = [0.0]
-
         def rateLimitedFunction(*args, **kargs):
-            elapsed = time.time() - lastTimeCalled[0]
+            if type(args[0]) is dict:
+                key = args[0].get('Signal')
+            else:
+                key = args[0]
+            elapsed = time.time() - lastTimeCalled.get(key, 0)
             leftToWait = minInterval - elapsed
             if leftToWait > 0:
                 # ignore update
                 return
             ret = func(*args, **kargs)
-            lastTimeCalled[0] = time.time()
+            lastTimeCalled.update({key: time.time()})
             return ret
 
         return rateLimitedFunction
 
     return decorate
```

### Comparing `mxcubeweb-1.48.0/mxcube3/logging_handler.py` & `mxcubeweb-1.49.0/mxcube3/logging_handler.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/beamline.py` & `mxcubeweb-1.49.0/mxcube3/routes/beamline.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/detector.py` & `mxcubeweb-1.49.0/mxcube3/routes/detector.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/diffractometer.py` & `mxcubeweb-1.49.0/mxcube3/routes/diffractometer.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/gphl_workflow.py` & `mxcubeweb-1.49.0/mxcube3/routes/gphl_workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/lims.py` & `mxcubeweb-1.49.0/mxcube3/routes/lims.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/log.py` & `mxcubeweb-1.49.0/mxcube3/routes/log.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/login.py` & `mxcubeweb-1.49.0/mxcube3/routes/login.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/main.py` & `mxcubeweb-1.49.0/mxcube3/routes/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,25 +35,19 @@
 
     @bp.route("/uiproperties")
     @server.restrict
     @server.validate(resp=Response(HTTP_200=UIPropertiesListModel))
     def get_ui_properties():
         return app.get_ui_properties()
 
-    @bp.route("/version")
-    @server.restrict
-    @server.validate(resp=Response(HTTP_200=VersionModel))
-    def mxcube_version():
-        return jsonify({"version": version.__version__})
-
-    @bp.route("/mode")
+    @bp.route("/application_settings")
     @server.restrict
     @server.validate(resp=Response(HTTP_200=ModeEnumModel))
     def mxcube_mode():
-        return jsonify({"mode": app.CONFIG.app.mode})
+        return jsonify({"mode": app.CONFIG.app.mode, "version": version.__version__})
 
     @server.flask.before_request
     def before_request():
         logging.getLogger("MX3.HWR").debug('Remote Addr: %s', request.remote_addr)
         logging.getLogger("MX3.HWR").debug('Path: %s', request.full_path)
         logging.getLogger("MX3.HWR").debug('scheme: %s', request.scheme)
         logging.getLogger("MX3.HWR").debug('Headers: %s', request.headers)
```

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/mockups.py` & `mxcubeweb-1.49.0/mxcube3/routes/mockups.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/queue.py` & `mxcubeweb-1.49.0/mxcube3/routes/queue.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/ra.py` & `mxcubeweb-1.49.0/mxcube3/routes/ra.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/samplecentring.py` & `mxcubeweb-1.49.0/mxcube3/routes/samplecentring.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/samplechanger.py` & `mxcubeweb-1.49.0/mxcube3/routes/samplechanger.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/signals.py` & `mxcubeweb-1.49.0/mxcube3/routes/signals.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/routes/workflow.py` & `mxcubeweb-1.49.0/mxcube3/routes/workflow.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/server.py` & `mxcubeweb-1.49.0/mxcube3/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,14 @@
                 f.write("")
 
             for pid in pid_list:
                 os.kill(int(pid), signal.SIGKILL)
 
     @staticmethod
     def init(cmdline_options, cfg, mxcube):
-        t0 = time.time()
-
         template_dir = os.path.join(os.path.dirname(__file__), "templates")
 
         Server.flask = Flask(
             __name__,
             static_folder=cmdline_options.static_folder,
             static_url_path="",
             template_folder=template_dir,
@@ -101,17 +99,14 @@
 
             # Make the valid_login_only decorator available on server object
             Server.restrict = staticmethod(networkutils.login_required)
             Server.require_control = staticmethod(networkutils.require_control)
             Server.ws_restrict = staticmethod(networkutils.ws_valid_login_only)
             Server.route = staticmethod(Server.flask.route)
 
-            msg = "MXCuBE 3 initialized, it took %.1f seconds" % (time.time() - t0)
-            logging.getLogger("MX3.HWR").info(msg)
-
     def _register_route(init_blueprint_fn, app, url_prefix, tag=None):
         tag = url_prefix if tag is None else tag
         bp = init_blueprint_fn(app, Server, url_prefix)
 
         Server.flask.register_blueprint(bp)
 
         for key, function in Server.flask.view_functions.items():
```

### Comparing `mxcubeweb-1.48.0/mxcube3/state_storage.py` & `mxcubeweb-1.49.0/mxcube3/state_storage.py`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/templates/characterisation-results.js` & `mxcubeweb-1.49.0/mxcube3/templates/characterisation-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/templates/data-collection-results.html` & `mxcubeweb-1.49.0/mxcube3/templates/data-collection-results.html`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/templates/precompiled.templates.min.js` & `mxcubeweb-1.49.0/mxcube3/templates/precompiled.templates.min.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/templates/workflow-results.js` & `mxcubeweb-1.49.0/mxcube3/templates/workflow-results.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/mxcube3/video/websocket-relay.js` & `mxcubeweb-1.49.0/mxcube3/video/websocket-relay.js`

 * *Files identical despite different names*

### Comparing `mxcubeweb-1.48.0/pyproject.toml` & `mxcubeweb-1.49.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mxcubeweb"
-version = "1.48.0"
+version = "1.49.0"
 license = "LGPL-3.0-or-later"
 description = "MXCuBE Web user interface"
 authors = ["The MXCuBE collaboration <mxcube@esrf.fr>"]
 maintainers = [
     "MXCuBE collaboration <mxcube@esrf.fr>",
 ]
 readme = "README.md"
```

### Comparing `mxcubeweb-1.48.0/PKG-INFO` & `mxcubeweb-1.49.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxcubeweb
-Version: 1.48.0
+Version: 1.49.0
 Summary: MXCuBE Web user interface
 Home-page: http://github.com/mxcube/mxcubeweb
 License: LGPL-3.0-or-later
 Keywords: mxcube,mxcube3,mxcubeweb
 Author: The MXCuBE collaboration
 Author-email: mxcube@esrf.fr
 Maintainer: MXCuBE collaboration
```

