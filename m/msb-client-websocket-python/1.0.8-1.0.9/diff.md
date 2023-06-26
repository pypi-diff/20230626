# Comparing `tmp/msb-client-websocket-python-1.0.8.tar.gz` & `tmp/msb-client-websocket-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/msb-client-websocket-python-1.0.8.tar", last modified: Thu May 14 14:27:26 2020, max compression
+gzip compressed data, was "dist/msb-client-websocket-python-1.0.9.tar", last modified: Tue Nov 24 14:37:43 2020, max compression
```

## Comparing `msb-client-websocket-python-1.0.8.tar` & `msb-client-websocket-python-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    21358 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/msb_client/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3405 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/Event.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6935 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/event_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/DataType.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3092 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/Function.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/DataFormat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37665 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/MsbClient.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6935 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/function_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3680 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/ComplexDataFormat.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      520 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/msb_client/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16106 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21358 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      618 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       75 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      285 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 14:27:26.000000 msb-client-websocket-python-1.0.8/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)    22018 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/test/test_integration.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   101472 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/test/test_unit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2020-05-14 14:25:52.000000 msb-client-websocket-python-1.0.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21671 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/msb_client/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3405 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/Event.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6935 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/event_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/DataType.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3092 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/Function.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1135 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/DataFormat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37677 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/MsbClient.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6935 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/function_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3680 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/ComplexDataFormat.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      520 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/msb_client/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16411 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21671 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       11 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)      618 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       75 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      285 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-11-24 14:37:43.000000 msb-client-websocket-python-1.0.9/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22018 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/test/test_integration.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   101472 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/test/test_unit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1737 2020-11-24 14:35:58.000000 msb-client-websocket-python-1.0.9/setup.py
```

### Comparing `msb-client-websocket-python-1.0.8/PKG-INFO` & `msb-client-websocket-python-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msb-client-websocket-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: The Python client library to connect to the Websocket Interface of the VFK MSB
 Home-page: https://research.virtualfortknox.de/
 Author: Daniel Stock
 Author-email: daniel.stock@ipa.fraunhofer.de
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/research-virtualfortknox/msb-client-websocket-python.git
 Project-URL: Bug Tracker, https://github.com/research-virtualfortknox/msb-client-websocket-python/issues
@@ -14,14 +14,15 @@
           </a>
         </p>
         
         # MSB websocket client library for Python
         
         [![Build Status](https://travis-ci.org/research-virtualfortknox/msb-client-websocket-python.svg?branch=master)](https://travis-ci.org/research-virtualfortknox/msb-client-websocket-python)
         [![PyPI version](https://badge.fury.io/py/msb-client-websocket-python.svg)](https://badge.fury.io/py/msb-client-websocket-python)
+        [![Coverage Status](https://coveralls.io/repos/github/research-virtualfortknox/msb-client-websocket-python/badge.svg?branch=feature-coveralls)](https://coveralls.io/github/research-virtualfortknox/msb-client-websocket-python?branch=feature-coveralls)
         [![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-python.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-python?ref=badge_shield)
         
         **Compatibility Matrix**
         
         Client version compatibility to MSB versions:
         
         | | **1.5.x-RELEASE** |
@@ -40,15 +41,15 @@
         
         TODO: Link to general documentation about VFK MSB
         
         You can use this client to connect a python app to VFK MSB.
         
         ## Prerequisites
         
-        * Setup [Python](https://www.python.org/downloads/) **version 3.6.x**
+        * Setup [Python](https://www.python.org/downloads/) **version 3.6.x** (last client version supporting Python 2.7 is v1.0.8)
         * MSB client installed using PyPi
         * Optional: Use pipenv to run your python app in a virtual environment to avoid dependency isssues with other apps
         
         Install MSB client from PyPi
         
         ```sh
         pip install msb-client-websocket-python
```

#### html2text {}

```diff
@@ -1,160 +1,164 @@
-Metadata-Version: 2.1 Name: msb-client-websocket-python Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: msb-client-websocket-python Version: 1.0.9 Summary:
 The Python client library to connect to the Websocket Interface of the VFK MSB
 Home-page: https://research.virtualfortknox.de/ Author: Daniel Stock Author-
 email: daniel.stock@ipa.fraunhofer.de License: Apache-2.0 Project-URL: Source
 Code, https://github.com/research-virtualfortknox/msb-client-websocket-
 python.git Project-URL: Bug Tracker, https://github.com/research-
 virtualfortknox/msb-client-websocket-python/issues Description:
                               [VFK_Research_Logo]
 # MSB websocket client library for Python [![Build Status](https://travis-
 ci.org/research-virtualfortknox/msb-client-websocket-python.svg?branch=master)]
 (https://travis-ci.org/research-virtualfortknox/msb-client-websocket-python) [!
 [PyPI version](https://badge.fury.io/py/msb-client-websocket-python.svg)]
-(https://badge.fury.io/py/msb-client-websocket-python) [![FOSSA Status](https:/
-/app.fossa.io/api/projects/git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-
-client-websocket-python.svg?type=shield)](https://app.fossa.io/projects/
+(https://badge.fury.io/py/msb-client-websocket-python) [![Coverage Status]
+(https://coveralls.io/repos/github/research-virtualfortknox/msb-client-
+websocket-python/badge.svg?branch=feature-coveralls)](https://coveralls.io/
+github/research-virtualfortknox/msb-client-websocket-python?branch=feature-
+coveralls) [![FOSSA Status](https://app.fossa.io/api/projects/
+git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-
+python.svg?type=shield)](https://app.fossa.io/projects/
 git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-
 python?ref=badge_shield) **Compatibility Matrix** Client version compatibility
 to MSB versions: | | **1.5.x-RELEASE** | |---|:---:| | 1.0.x | x | ## Welcome
 If you want to contribute, please read the [Contribution Guidelines](.github/
 CONTRIBUTING.md). If you want to test this client by using its sources and a
 sample app, read the [App Sample](doc/app_sample.md). If you want to know how
 to use this client in your own project, read below. ## What is VFK MSB TODO:
 Link to general documentation about VFK MSB You can use this client to connect
 a python app to VFK MSB. ## Prerequisites * Setup [Python](https://
-www.python.org/downloads/) **version 3.6.x** * MSB client installed using PyPi
-* Optional: Use pipenv to run your python app in a virtual environment to avoid
-dependency isssues with other apps Install MSB client from PyPi ```sh pip
-install msb-client-websocket-python ``` Import to your applicaton ```python
-from msb_client.ComplexDataFormat import ComplexDataFormat from
-msb_client.DataType import DataType from msb_client.Event import Event from
-msb_client.Function import Function from msb_client.MsbClient import MsbClient
-``` ## Create self-description The figure below shows a minimal required `self-
-description model` of a smart object / application. Every smart object /
-application requires (must have) a uuid and a token. The uuid is competent for
-identification and the token is used to verify the smart object / application
-for its owner on the MSB side. ![Self Description](doc/images/self-
-description.png) TODO: Here you can find more information about the `self-
-description structure` and `supported data formats`. ### Alternative 1 - By
-application.properties Add the main description by adding an
-`application.poperties` file to the root of your project: Generate the uuid
-e.g. by a tool like https://www.uuidgenerator.net/ ```sh msb.uuid=76499d88-
-34cf-4836-8cc1-7e0d9c54dacx msb.name=YourSmartObjectName
-msb.description=YourSmartObjectDesc msb.token=5e0d9c54dacx msb.type=SmartObject
-``` When initializing your msb client instance, the `application.properties`
-file will be loaded. ```python myMsbClient = MsbClient() ``` You can also set a
-custom path to the `application.properties` file. ```python myMsbClient =
-MsbClient(applicationPropertiesCustomPath="./your/path/to/
-application.properties") ``` ### Alternative 2 - By constructor If you do not
-provide an application.properties file, use the constructor to define the basic
-self description. ```python SERVICE_TYPE = "SmartObject" SO_UUID = str
-(uuid.uuid1()) # you can type in an own uuid here instead of generating it
-SO_NAME = "YourSmartObjectName" SO_DESCRIPTION = "YourSmartObjectDesc" SO_TOKEN
-= SO_UUID[-6:] myMsbClient = MsbClient( SERVICE_TYPE, SO_UUID, SO_NAME,
-SO_DESCRIPTION, SO_TOKEN, ) ``` ## Add Events Add `events` to your smart object
-/ application which can be send to MSB. ### Alternative 1: Simple event
-creation sample (using method params): ```python event_id = "E1" event_name =
-"EVENT " + event_id event_description = "EVENT Description " + event_id
-event_dataformat = DataType.STRING event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2
-(HIGH) isArray = False # just one value or array of it? # add the event
-myMsbClient.addEvent( event_id, event_name, event_description,
-event_dataformat, event_priority, isArray, ) ``` ### Alternative 2: Complex
-event creation sample (using object): ```python event_id = "E2" event_name =
-"EVENT " + event_id event_description = "EVENT Description " + event_id
-event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2 (HIGH) isArray = False # just one
-value or array of it? # define a complex data format to be used in an event #
-init the complex data format myDevice = ComplexDataFormat("MyDevice") myModule
-= ComplexDataFormat("MyModule") # add the properties to the complex objects #
-(property_name, property_datatype, isArray) myModule.addProperty("moduleName",
-DataType.STRING, False) myDevice.addProperty("deviceName", DataType.STRING,
-False) myDevice.addProperty("deviceWeight", DataType.FLOAT, False)
-myDevice.addProperty("submodules", myModule, True) # add the event (with the
-root of the nested complex object) myMsbClient.addEvent( event_id, event_name,
-event_description, myDevice, event_priority, isArray, ) ``` ### Alternative 3:
-Complex event creation sample (using json object): ```python event_id = "E3"
-event_name = "EVENT " + event_id event_description = "EVENT Description " +
-event_id event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2 (HIGH) isArray = False #
-just one value or array of it? # add the event (with the MSB-ready json object)
-myMsbClient.addEvent( event_id, event_name, event_description, { "Team" :
-{ "type" : "object", "properties" : { "staff" : { "type" : "array", "items" :
-{ "$ref" : "#/definitions/Member" } } } }, "Member" : { "type" : "object",
-"properties" : { "name" : { "type" : "string" }, "status" : { "enum" :
-[ "present", "absent" ], "type" : "string" } } }, "dataObject" : { "$ref" : "#/
-definitions/Team" } }, event_priority, isArray, ) ``` See `app_sample.py` for
-more event creation examples. ## Add Functions Add `functions` and their
-implementations your smart object / application is able to handle. ###
-Alternative 1: Simple function creation sample (using method params): ```python
-function_id = "F1" function_name = "FUNC " + function_id function_description =
-"FUNC Description " + function_id function_dataformat = DataType.STRING isArray
-= False # handle array of values or just one value? responseEvents = None # you
-can link to response events here by a list of event is e.g. ["E1"] # define the
-function which will be passed to the function description # this function
-implementation will be called def printMsg(msg): print(str(msg["dataObject"]))
-# add the function myMsbClient.addFunction( function_id, function_name,
-function_description, function_dataformat, printMsg, isArray, responseEvents, )
-``` ### Alternative 2: Complex function creation sample (using object):
-```python function_id = "F2" function_name = "FUNC " + function_id
-function_description = "FUNC Description " + function_id isArray = False #
-handle array of values or just one value? responseEvents = None # you can link
-to response events here by a list of event is e.g. ["E1"] # define a complex
-data format to be used in an event # init the complex data format myCar =
-ComplexDataFormat("MyCar") # add the properties to the complex objects #
-(property_name, property_datatype, isArray) myCar.addProperty("carColor",
-DataType.STRING, False) myCar.addProperty("carNrOfSeats", DataType.INT32,
-False) myCar.addProperty("carWeight", DataType.FLOAT, False) # define the
-function which will be passed to the function description # this function
-implementation will be called def printMsg(msg): print(str(msg["dataObject"]))
-# add the function myMsbClient.addFunction( function_id, function_name,
-function_description, myCar, printMsg, isArray, responseEvents, ) ``` ###
-Alternative 3: Complex function creation sample (using json object): ```python
-function_id = "F3" function_name = "FUNC " + function_id function_description =
-"FUNC Description " + function_id isArray = False # handle array of values or
-just one value? responseEvents = None # you can link to response events here by
-a list of event is e.g. ["E1"] # define the function which will be passed to
+www.python.org/downloads/) **version 3.6.x** (last client version supporting
+Python 2.7 is v1.0.8) * MSB client installed using PyPi * Optional: Use pipenv
+to run your python app in a virtual environment to avoid dependency isssues
+with other apps Install MSB client from PyPi ```sh pip install msb-client-
+websocket-python ``` Import to your applicaton ```python from
+msb_client.ComplexDataFormat import ComplexDataFormat from msb_client.DataType
+import DataType from msb_client.Event import Event from msb_client.Function
+import Function from msb_client.MsbClient import MsbClient ``` ## Create self-
+description The figure below shows a minimal required `self-description model`
+of a smart object / application. Every smart object / application requires
+(must have) a uuid and a token. The uuid is competent for identification and
+the token is used to verify the smart object / application for its owner on the
+MSB side. ![Self Description](doc/images/self-description.png) TODO: Here you
+can find more information about the `self-description structure` and `supported
+data formats`. ### Alternative 1 - By application.properties Add the main
+description by adding an `application.poperties` file to the root of your
+project: Generate the uuid e.g. by a tool like https://www.uuidgenerator.net/
+```sh msb.uuid=76499d88-34cf-4836-8cc1-7e0d9c54dacx
+msb.name=YourSmartObjectName msb.description=YourSmartObjectDesc
+msb.token=5e0d9c54dacx msb.type=SmartObject ``` When initializing your msb
+client instance, the `application.properties` file will be loaded. ```python
+myMsbClient = MsbClient() ``` You can also set a custom path to the
+`application.properties` file. ```python myMsbClient = MsbClient
+(applicationPropertiesCustomPath="./your/path/to/application.properties") ```
+### Alternative 2 - By constructor If you do not provide an
+application.properties file, use the constructor to define the basic self
+description. ```python SERVICE_TYPE = "SmartObject" SO_UUID = str(uuid.uuid1())
+# you can type in an own uuid here instead of generating it SO_NAME =
+"YourSmartObjectName" SO_DESCRIPTION = "YourSmartObjectDesc" SO_TOKEN = SO_UUID
+[-6:] myMsbClient = MsbClient( SERVICE_TYPE, SO_UUID, SO_NAME, SO_DESCRIPTION,
+SO_TOKEN, ) ``` ## Add Events Add `events` to your smart object / application
+which can be send to MSB. ### Alternative 1: Simple event creation sample
+(using method params): ```python event_id = "E1" event_name = "EVENT " +
+event_id event_description = "EVENT Description " + event_id event_dataformat =
+DataType.STRING event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2 (HIGH) isArray =
+False # just one value or array of it? # add the event myMsbClient.addEvent
+( event_id, event_name, event_description, event_dataformat, event_priority,
+isArray, ) ``` ### Alternative 2: Complex event creation sample (using object):
+```python event_id = "E2" event_name = "EVENT " + event_id event_description =
+"EVENT Description " + event_id event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2
+(HIGH) isArray = False # just one value or array of it? # define a complex data
+format to be used in an event # init the complex data format myDevice =
+ComplexDataFormat("MyDevice") myModule = ComplexDataFormat("MyModule") # add
+the properties to the complex objects # (property_name, property_datatype,
+isArray) myModule.addProperty("moduleName", DataType.STRING, False)
+myDevice.addProperty("deviceName", DataType.STRING, False) myDevice.addProperty
+("deviceWeight", DataType.FLOAT, False) myDevice.addProperty("submodules",
+myModule, True) # add the event (with the root of the nested complex object)
+myMsbClient.addEvent( event_id, event_name, event_description, myDevice,
+event_priority, isArray, ) ``` ### Alternative 3: Complex event creation sample
+(using json object): ```python event_id = "E3" event_name = "EVENT " + event_id
+event_description = "EVENT Description " + event_id event_priority = 1 # 0
+(LOW), 1 (MEDIUM), 2 (HIGH) isArray = False # just one value or array of it? #
+add the event (with the MSB-ready json object) myMsbClient.addEvent( event_id,
+event_name, event_description, { "Team" : { "type" : "object", "properties" :
+{ "staff" : { "type" : "array", "items" : { "$ref" : "#/definitions/Member" } }
+} }, "Member" : { "type" : "object", "properties" : { "name" : { "type" :
+"string" }, "status" : { "enum" : [ "present", "absent" ], "type" : "string" }
+} }, "dataObject" : { "$ref" : "#/definitions/Team" } }, event_priority,
+isArray, ) ``` See `app_sample.py` for more event creation examples. ## Add
+Functions Add `functions` and their implementations your smart object /
+application is able to handle. ### Alternative 1: Simple function creation
+sample (using method params): ```python function_id = "F1" function_name =
+"FUNC " + function_id function_description = "FUNC Description " + function_id
+function_dataformat = DataType.STRING isArray = False # handle array of values
+or just one value? responseEvents = None # you can link to response events here
+by a list of event is e.g. ["E1"] # define the function which will be passed to
 the function description # this function implementation will be called def
 printMsg(msg): print(str(msg["dataObject"])) # add the function
 myMsbClient.addFunction( function_id, function_name, function_description,
-{ "MyCar" : { "type" : "object", "properties" : { "carColor" : { "type" :
-"string" }, "carNrOfSeats" : { "format": "int32", "type": "integer" },
-"carWeight" : { "format": "float", "type": "number" }, "wheels" : { "type" :
-"array", "items" : { "$ref" : "#/definitions/MyWheel" } } } }, "MyWheel" :
-{ "type" : "object", "properties" : { "position" : { "enum" : [ "br", "bl",
-"fr", "fl" ], "type" : "string" } } }, "dataObject" : { "$ref" : "#/
-definitions/MyCar" } }, printMsg, isArray, responseEvents, ) ``` See
-`app_sample.py` of the application template for more (and complex) examples. ##
-Connect and Register Client ```python msb_url = 'ws://127.0.0.1:8085'
-myMsbClient.connect(msb_url) myMsbClient.register() ``` You will get an
-`IO_CONNECTED` and `IO_REGISTERED` event from MSB, if successful. ## Event
-publishing For publishing an event to a websocket broker interface, only the
-`eventId` and `data` are required of the already specified event (see above).
-```python event_id = "E1" event_value = 'Hello World!' myMsbClient.publish
-( event_id, event_value ) ``` The MSB responds with an `IO_PUBLISHED` event, if
-successful. By default events are published with a low priority. It is also
-possible to `set the priority` of an event. There are three possible priorities
-for events like it is shown at the following table. | `Constant` | `Value` | |:
----:|:---:| | LOW | 0 | | MEDIUM| 1 | | HIGH| 2 | ```python event_id = "E1"
-event_value = 'Hello World!' event_priority = 2 myMsbClient.publish( event_id,
-event_value, event_priority ) ``` Another option is to publish an event as
-`cached event` by setting the cache parameter to true. And you can add a `post
-date`. This means that the event is not deleted if the connection is broken.
+function_dataformat, printMsg, isArray, responseEvents, ) ``` ### Alternative
+2: Complex function creation sample (using object): ```python function_id =
+"F2" function_name = "FUNC " + function_id function_description = "FUNC
+Description " + function_id isArray = False # handle array of values or just
+one value? responseEvents = None # you can link to response events here by a
+list of event is e.g. ["E1"] # define a complex data format to be used in an
+event # init the complex data format myCar = ComplexDataFormat("MyCar") # add
+the properties to the complex objects # (property_name, property_datatype,
+isArray) myCar.addProperty("carColor", DataType.STRING, False)
+myCar.addProperty("carNrOfSeats", DataType.INT32, False) myCar.addProperty
+("carWeight", DataType.FLOAT, False) # define the function which will be passed
+to the function description # this function implementation will be called def
+printMsg(msg): print(str(msg["dataObject"])) # add the function
+myMsbClient.addFunction( function_id, function_name, function_description,
+myCar, printMsg, isArray, responseEvents, ) ``` ### Alternative 3: Complex
+function creation sample (using json object): ```python function_id = "F3"
+function_name = "FUNC " + function_id function_description = "FUNC Description
+" + function_id isArray = False # handle array of values or just one value?
+responseEvents = None # you can link to response events here by a list of event
+is e.g. ["E1"] # define the function which will be passed to the function
+description # this function implementation will be called def printMsg(msg):
+print(str(msg["dataObject"])) # add the function myMsbClient.addFunction
+( function_id, function_name, function_description, { "MyCar" : { "type" :
+"object", "properties" : { "carColor" : { "type" : "string" }, "carNrOfSeats" :
+{ "format": "int32", "type": "integer" }, "carWeight" : { "format": "float",
+"type": "number" }, "wheels" : { "type" : "array", "items" : { "$ref" : "#/
+definitions/MyWheel" } } } }, "MyWheel" : { "type" : "object", "properties" :
+{ "position" : { "enum" : [ "br", "bl", "fr", "fl" ], "type" : "string" } } },
+"dataObject" : { "$ref" : "#/definitions/MyCar" } }, printMsg, isArray,
+responseEvents, ) ``` See `app_sample.py` of the application template for more
+(and complex) examples. ## Connect and Register Client ```python msb_url = 'ws:
+//127.0.0.1:8085' myMsbClient.connect(msb_url) myMsbClient.register() ``` You
+will get an `IO_CONNECTED` and `IO_REGISTERED` event from MSB, if successful.
+## Event publishing For publishing an event to a websocket broker interface,
+only the `eventId` and `data` are required of the already specified event (see
+above). ```python event_id = "E1" event_value = 'Hello World!'
+myMsbClient.publish( event_id, event_value ) ``` The MSB responds with an
+`IO_PUBLISHED` event, if successful. By default events are published with a low
+priority. It is also possible to `set the priority` of an event. There are
+three possible priorities for events like it is shown at the following table. |
+`Constant` | `Value` | |:---:|:---:| | LOW | 0 | | MEDIUM| 1 | | HIGH| 2 |
 ```python event_id = "E1" event_value = 'Hello World!' event_priority = 2
-event_isCached = True event_postDate = datetime.datetime.utcnow().isoformat()[:
--3] + "Z" myMsbClient.publish( event_id, event_value, event_priority,
-event_isCached, event_postDate ) ``` You cann also handle `correlation ids` to
-identify an event among flows. ```python event_id = "E1" event_value = 'Hello
+myMsbClient.publish( event_id, event_value, event_priority ) ``` Another option
+is to publish an event as `cached event` by setting the cache parameter to
+true. And you can add a `post date`. This means that the event is not deleted
+if the connection is broken. ```python event_id = "E1" event_value = 'Hello
 World!' event_priority = 2 event_isCached = True event_postDate =
-datetime.datetime.utcnow().isoformat()[:-3] + "Z" event_correlationId =
-"72047f33-a9ae-4aa5-b7ae-c1c4a2797cac" myMsbClient.publish( event_id,
-event_value, event_priority, event_isCached, event_postDate,
-event_correlationId ) ``` For values based on complex data formats it will look
-like this: ```python event_id = "E2" event_priority = 2 event_isCached = True
-event_postDate = datetime.datetime.utcnow().isoformat()[:-3] + "Z"
-event_correlationId = "72047f33-a9ae-4aa5-b7ae-c1c4a2797cac" # pepare the
-complex ovbject based on a complex data format # use it as event value
+datetime.datetime.utcnow().isoformat()[:-3] + "Z" myMsbClient.publish
+( event_id, event_value, event_priority, event_isCached, event_postDate ) ```
+You cann also handle `correlation ids` to identify an event among flows.
+```python event_id = "E1" event_value = 'Hello World!' event_priority = 2
+event_isCached = True event_postDate = datetime.datetime.utcnow().isoformat()[:
+-3] + "Z" event_correlationId = "72047f33-a9ae-4aa5-b7ae-c1c4a2797cac"
+myMsbClient.publish( event_id, event_value, event_priority, event_isCached,
+event_postDate, event_correlationId ) ``` For values based on complex data
+formats it will look like this: ```python event_id = "E2" event_priority = 2
+event_isCached = True event_postDate = datetime.datetime.utcnow().isoformat()[:
+-3] + "Z" event_correlationId = "72047f33-a9ae-4aa5-b7ae-c1c4a2797cac" # pepare
+the complex ovbject based on a complex data format # use it as event value
 myModuleObj = {} myModuleObj['moduleName'] = 'Module 1' myDeviceObj = {}
 myDeviceObj['deviceName'] = 'Device 1' myDeviceObj['deviceWeight'] = 1.3
 myDeviceObj['submodules'] = [myModuleObj] myMsbClient.publish( event_id,
 myDeviceObj, event_priority, event_isCached, event_postDate,
 event_correlationId ) ``` ## Function call handling As shown above the
 addFunction method includes a `function pointer` to point to the function
 implementation. ## Configuration parameters Configuration parameters are a
```

### Comparing `msb-client-websocket-python-1.0.8/msb_client/Event.py` & `msb-client-websocket-python-1.0.9/msb_client/Event.py`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/msb_client/event_schema.json` & `msb-client-websocket-python-1.0.9/msb_client/event_schema.json`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/msb_client/DataType.py` & `msb-client-websocket-python-1.0.9/msb_client/DataType.py`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/msb_client/Function.py` & `msb-client-websocket-python-1.0.9/msb_client/Function.py`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/msb_client/DataFormat.py` & `msb-client-websocket-python-1.0.9/msb_client/DataFormat.py`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/msb_client/MsbClient.py` & `msb-client-websocket-python-1.0.9/msb_client/MsbClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -786,24 +786,24 @@
         _ev = []
         e_props = ["@id", "id", "dataFormat", "description", "eventId", "name"]
         for event in self.events:
             current_e_props = []
             e = jsonpickle.decode(
                 jsonpickle.encode(self.events[event], unpicklable=False)
             )
-            for key in e.keys():
+            for key in list(e.keys()):
                 if key == "id":
                     e["@id"] = e["id"]
                     del e[key]
             del e["priority"]
             del e["df"]
             if e["dataFormat"] is None:
                 del e["dataFormat"]
             del e["isArray"]
-            for key in e.keys():
+            for key in list(e.keys()):
                 current_e_props.append(key)
             for key in current_e_props:
                 if key not in e_props:
                     # logging.warning(self, 'Remove key from event if invalid in self description: ' + key)
                     try:
                         del e[key]
                     except Exception:
```

### Comparing `msb-client-websocket-python-1.0.8/msb_client/function_schema.json` & `msb-client-websocket-python-1.0.9/msb_client/function_schema.json`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/msb_client/ComplexDataFormat.py` & `msb-client-websocket-python-1.0.9/msb_client/ComplexDataFormat.py`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/msb_client/__init__.py` & `msb-client-websocket-python-1.0.9/msb_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Copyright (c) 2019 Fraunhofer Institute for Manufacturing Engineering and Automation (IPA)
 Authors: Daniel Stock, Matthias Stoehr
 
 Licensed under the Apache License, Version 2.0
 See the file "LICENSE" for the full license governing this code.
 """
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 
 # from .ComplexDataFormat import ComplexDataFormat
 # from .DataFormat import DataFormat
 # from .DataType import convertDataType, getDataType, DataType
 # from .Event import Event
 # from .Function import Function
 # from .MsbClient import MsbClient
```

### Comparing `msb-client-websocket-python-1.0.8/README.md` & `msb-client-websocket-python-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   </a>
 </p>
 
 # MSB websocket client library for Python
 
 [![Build Status](https://travis-ci.org/research-virtualfortknox/msb-client-websocket-python.svg?branch=master)](https://travis-ci.org/research-virtualfortknox/msb-client-websocket-python)
 [![PyPI version](https://badge.fury.io/py/msb-client-websocket-python.svg)](https://badge.fury.io/py/msb-client-websocket-python)
+[![Coverage Status](https://coveralls.io/repos/github/research-virtualfortknox/msb-client-websocket-python/badge.svg?branch=feature-coveralls)](https://coveralls.io/github/research-virtualfortknox/msb-client-websocket-python?branch=feature-coveralls)
 [![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-python.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-python?ref=badge_shield)
 
 **Compatibility Matrix**
 
 Client version compatibility to MSB versions:
 
 | | **1.5.x-RELEASE** |
@@ -30,15 +31,15 @@
 
 TODO: Link to general documentation about VFK MSB
 
 You can use this client to connect a python app to VFK MSB.
 
 ## Prerequisites
 
-* Setup [Python](https://www.python.org/downloads/) **version 3.6.x**
+* Setup [Python](https://www.python.org/downloads/) **version 3.6.x** (last client version supporting Python 2.7 is v1.0.8)
 * MSB client installed using PyPi
 * Optional: Use pipenv to run your python app in a virtual environment to avoid dependency isssues with other apps
 
 Install MSB client from PyPi
 
 ```sh
 pip install msb-client-websocket-python
```

### Comparing `msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/PKG-INFO` & `msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msb-client-websocket-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: The Python client library to connect to the Websocket Interface of the VFK MSB
 Home-page: https://research.virtualfortknox.de/
 Author: Daniel Stock
 Author-email: daniel.stock@ipa.fraunhofer.de
 License: Apache-2.0
 Project-URL: Source Code, https://github.com/research-virtualfortknox/msb-client-websocket-python.git
 Project-URL: Bug Tracker, https://github.com/research-virtualfortknox/msb-client-websocket-python/issues
@@ -14,14 +14,15 @@
           </a>
         </p>
         
         # MSB websocket client library for Python
         
         [![Build Status](https://travis-ci.org/research-virtualfortknox/msb-client-websocket-python.svg?branch=master)](https://travis-ci.org/research-virtualfortknox/msb-client-websocket-python)
         [![PyPI version](https://badge.fury.io/py/msb-client-websocket-python.svg)](https://badge.fury.io/py/msb-client-websocket-python)
+        [![Coverage Status](https://coveralls.io/repos/github/research-virtualfortknox/msb-client-websocket-python/badge.svg?branch=feature-coveralls)](https://coveralls.io/github/research-virtualfortknox/msb-client-websocket-python?branch=feature-coveralls)
         [![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-python.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-python?ref=badge_shield)
         
         **Compatibility Matrix**
         
         Client version compatibility to MSB versions:
         
         | | **1.5.x-RELEASE** |
@@ -40,15 +41,15 @@
         
         TODO: Link to general documentation about VFK MSB
         
         You can use this client to connect a python app to VFK MSB.
         
         ## Prerequisites
         
-        * Setup [Python](https://www.python.org/downloads/) **version 3.6.x**
+        * Setup [Python](https://www.python.org/downloads/) **version 3.6.x** (last client version supporting Python 2.7 is v1.0.8)
         * MSB client installed using PyPi
         * Optional: Use pipenv to run your python app in a virtual environment to avoid dependency isssues with other apps
         
         Install MSB client from PyPi
         
         ```sh
         pip install msb-client-websocket-python
```

#### html2text {}

```diff
@@ -1,160 +1,164 @@
-Metadata-Version: 2.1 Name: msb-client-websocket-python Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: msb-client-websocket-python Version: 1.0.9 Summary:
 The Python client library to connect to the Websocket Interface of the VFK MSB
 Home-page: https://research.virtualfortknox.de/ Author: Daniel Stock Author-
 email: daniel.stock@ipa.fraunhofer.de License: Apache-2.0 Project-URL: Source
 Code, https://github.com/research-virtualfortknox/msb-client-websocket-
 python.git Project-URL: Bug Tracker, https://github.com/research-
 virtualfortknox/msb-client-websocket-python/issues Description:
                               [VFK_Research_Logo]
 # MSB websocket client library for Python [![Build Status](https://travis-
 ci.org/research-virtualfortknox/msb-client-websocket-python.svg?branch=master)]
 (https://travis-ci.org/research-virtualfortknox/msb-client-websocket-python) [!
 [PyPI version](https://badge.fury.io/py/msb-client-websocket-python.svg)]
-(https://badge.fury.io/py/msb-client-websocket-python) [![FOSSA Status](https:/
-/app.fossa.io/api/projects/git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-
-client-websocket-python.svg?type=shield)](https://app.fossa.io/projects/
+(https://badge.fury.io/py/msb-client-websocket-python) [![Coverage Status]
+(https://coveralls.io/repos/github/research-virtualfortknox/msb-client-
+websocket-python/badge.svg?branch=feature-coveralls)](https://coveralls.io/
+github/research-virtualfortknox/msb-client-websocket-python?branch=feature-
+coveralls) [![FOSSA Status](https://app.fossa.io/api/projects/
+git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-
+python.svg?type=shield)](https://app.fossa.io/projects/
 git%2Bgithub.com%2Fresearch-virtualfortknox%2Fmsb-client-websocket-
 python?ref=badge_shield) **Compatibility Matrix** Client version compatibility
 to MSB versions: | | **1.5.x-RELEASE** | |---|:---:| | 1.0.x | x | ## Welcome
 If you want to contribute, please read the [Contribution Guidelines](.github/
 CONTRIBUTING.md). If you want to test this client by using its sources and a
 sample app, read the [App Sample](doc/app_sample.md). If you want to know how
 to use this client in your own project, read below. ## What is VFK MSB TODO:
 Link to general documentation about VFK MSB You can use this client to connect
 a python app to VFK MSB. ## Prerequisites * Setup [Python](https://
-www.python.org/downloads/) **version 3.6.x** * MSB client installed using PyPi
-* Optional: Use pipenv to run your python app in a virtual environment to avoid
-dependency isssues with other apps Install MSB client from PyPi ```sh pip
-install msb-client-websocket-python ``` Import to your applicaton ```python
-from msb_client.ComplexDataFormat import ComplexDataFormat from
-msb_client.DataType import DataType from msb_client.Event import Event from
-msb_client.Function import Function from msb_client.MsbClient import MsbClient
-``` ## Create self-description The figure below shows a minimal required `self-
-description model` of a smart object / application. Every smart object /
-application requires (must have) a uuid and a token. The uuid is competent for
-identification and the token is used to verify the smart object / application
-for its owner on the MSB side. ![Self Description](doc/images/self-
-description.png) TODO: Here you can find more information about the `self-
-description structure` and `supported data formats`. ### Alternative 1 - By
-application.properties Add the main description by adding an
-`application.poperties` file to the root of your project: Generate the uuid
-e.g. by a tool like https://www.uuidgenerator.net/ ```sh msb.uuid=76499d88-
-34cf-4836-8cc1-7e0d9c54dacx msb.name=YourSmartObjectName
-msb.description=YourSmartObjectDesc msb.token=5e0d9c54dacx msb.type=SmartObject
-``` When initializing your msb client instance, the `application.properties`
-file will be loaded. ```python myMsbClient = MsbClient() ``` You can also set a
-custom path to the `application.properties` file. ```python myMsbClient =
-MsbClient(applicationPropertiesCustomPath="./your/path/to/
-application.properties") ``` ### Alternative 2 - By constructor If you do not
-provide an application.properties file, use the constructor to define the basic
-self description. ```python SERVICE_TYPE = "SmartObject" SO_UUID = str
-(uuid.uuid1()) # you can type in an own uuid here instead of generating it
-SO_NAME = "YourSmartObjectName" SO_DESCRIPTION = "YourSmartObjectDesc" SO_TOKEN
-= SO_UUID[-6:] myMsbClient = MsbClient( SERVICE_TYPE, SO_UUID, SO_NAME,
-SO_DESCRIPTION, SO_TOKEN, ) ``` ## Add Events Add `events` to your smart object
-/ application which can be send to MSB. ### Alternative 1: Simple event
-creation sample (using method params): ```python event_id = "E1" event_name =
-"EVENT " + event_id event_description = "EVENT Description " + event_id
-event_dataformat = DataType.STRING event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2
-(HIGH) isArray = False # just one value or array of it? # add the event
-myMsbClient.addEvent( event_id, event_name, event_description,
-event_dataformat, event_priority, isArray, ) ``` ### Alternative 2: Complex
-event creation sample (using object): ```python event_id = "E2" event_name =
-"EVENT " + event_id event_description = "EVENT Description " + event_id
-event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2 (HIGH) isArray = False # just one
-value or array of it? # define a complex data format to be used in an event #
-init the complex data format myDevice = ComplexDataFormat("MyDevice") myModule
-= ComplexDataFormat("MyModule") # add the properties to the complex objects #
-(property_name, property_datatype, isArray) myModule.addProperty("moduleName",
-DataType.STRING, False) myDevice.addProperty("deviceName", DataType.STRING,
-False) myDevice.addProperty("deviceWeight", DataType.FLOAT, False)
-myDevice.addProperty("submodules", myModule, True) # add the event (with the
-root of the nested complex object) myMsbClient.addEvent( event_id, event_name,
-event_description, myDevice, event_priority, isArray, ) ``` ### Alternative 3:
-Complex event creation sample (using json object): ```python event_id = "E3"
-event_name = "EVENT " + event_id event_description = "EVENT Description " +
-event_id event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2 (HIGH) isArray = False #
-just one value or array of it? # add the event (with the MSB-ready json object)
-myMsbClient.addEvent( event_id, event_name, event_description, { "Team" :
-{ "type" : "object", "properties" : { "staff" : { "type" : "array", "items" :
-{ "$ref" : "#/definitions/Member" } } } }, "Member" : { "type" : "object",
-"properties" : { "name" : { "type" : "string" }, "status" : { "enum" :
-[ "present", "absent" ], "type" : "string" } } }, "dataObject" : { "$ref" : "#/
-definitions/Team" } }, event_priority, isArray, ) ``` See `app_sample.py` for
-more event creation examples. ## Add Functions Add `functions` and their
-implementations your smart object / application is able to handle. ###
-Alternative 1: Simple function creation sample (using method params): ```python
-function_id = "F1" function_name = "FUNC " + function_id function_description =
-"FUNC Description " + function_id function_dataformat = DataType.STRING isArray
-= False # handle array of values or just one value? responseEvents = None # you
-can link to response events here by a list of event is e.g. ["E1"] # define the
-function which will be passed to the function description # this function
-implementation will be called def printMsg(msg): print(str(msg["dataObject"]))
-# add the function myMsbClient.addFunction( function_id, function_name,
-function_description, function_dataformat, printMsg, isArray, responseEvents, )
-``` ### Alternative 2: Complex function creation sample (using object):
-```python function_id = "F2" function_name = "FUNC " + function_id
-function_description = "FUNC Description " + function_id isArray = False #
-handle array of values or just one value? responseEvents = None # you can link
-to response events here by a list of event is e.g. ["E1"] # define a complex
-data format to be used in an event # init the complex data format myCar =
-ComplexDataFormat("MyCar") # add the properties to the complex objects #
-(property_name, property_datatype, isArray) myCar.addProperty("carColor",
-DataType.STRING, False) myCar.addProperty("carNrOfSeats", DataType.INT32,
-False) myCar.addProperty("carWeight", DataType.FLOAT, False) # define the
-function which will be passed to the function description # this function
-implementation will be called def printMsg(msg): print(str(msg["dataObject"]))
-# add the function myMsbClient.addFunction( function_id, function_name,
-function_description, myCar, printMsg, isArray, responseEvents, ) ``` ###
-Alternative 3: Complex function creation sample (using json object): ```python
-function_id = "F3" function_name = "FUNC " + function_id function_description =
-"FUNC Description " + function_id isArray = False # handle array of values or
-just one value? responseEvents = None # you can link to response events here by
-a list of event is e.g. ["E1"] # define the function which will be passed to
+www.python.org/downloads/) **version 3.6.x** (last client version supporting
+Python 2.7 is v1.0.8) * MSB client installed using PyPi * Optional: Use pipenv
+to run your python app in a virtual environment to avoid dependency isssues
+with other apps Install MSB client from PyPi ```sh pip install msb-client-
+websocket-python ``` Import to your applicaton ```python from
+msb_client.ComplexDataFormat import ComplexDataFormat from msb_client.DataType
+import DataType from msb_client.Event import Event from msb_client.Function
+import Function from msb_client.MsbClient import MsbClient ``` ## Create self-
+description The figure below shows a minimal required `self-description model`
+of a smart object / application. Every smart object / application requires
+(must have) a uuid and a token. The uuid is competent for identification and
+the token is used to verify the smart object / application for its owner on the
+MSB side. ![Self Description](doc/images/self-description.png) TODO: Here you
+can find more information about the `self-description structure` and `supported
+data formats`. ### Alternative 1 - By application.properties Add the main
+description by adding an `application.poperties` file to the root of your
+project: Generate the uuid e.g. by a tool like https://www.uuidgenerator.net/
+```sh msb.uuid=76499d88-34cf-4836-8cc1-7e0d9c54dacx
+msb.name=YourSmartObjectName msb.description=YourSmartObjectDesc
+msb.token=5e0d9c54dacx msb.type=SmartObject ``` When initializing your msb
+client instance, the `application.properties` file will be loaded. ```python
+myMsbClient = MsbClient() ``` You can also set a custom path to the
+`application.properties` file. ```python myMsbClient = MsbClient
+(applicationPropertiesCustomPath="./your/path/to/application.properties") ```
+### Alternative 2 - By constructor If you do not provide an
+application.properties file, use the constructor to define the basic self
+description. ```python SERVICE_TYPE = "SmartObject" SO_UUID = str(uuid.uuid1())
+# you can type in an own uuid here instead of generating it SO_NAME =
+"YourSmartObjectName" SO_DESCRIPTION = "YourSmartObjectDesc" SO_TOKEN = SO_UUID
+[-6:] myMsbClient = MsbClient( SERVICE_TYPE, SO_UUID, SO_NAME, SO_DESCRIPTION,
+SO_TOKEN, ) ``` ## Add Events Add `events` to your smart object / application
+which can be send to MSB. ### Alternative 1: Simple event creation sample
+(using method params): ```python event_id = "E1" event_name = "EVENT " +
+event_id event_description = "EVENT Description " + event_id event_dataformat =
+DataType.STRING event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2 (HIGH) isArray =
+False # just one value or array of it? # add the event myMsbClient.addEvent
+( event_id, event_name, event_description, event_dataformat, event_priority,
+isArray, ) ``` ### Alternative 2: Complex event creation sample (using object):
+```python event_id = "E2" event_name = "EVENT " + event_id event_description =
+"EVENT Description " + event_id event_priority = 1 # 0 (LOW), 1 (MEDIUM), 2
+(HIGH) isArray = False # just one value or array of it? # define a complex data
+format to be used in an event # init the complex data format myDevice =
+ComplexDataFormat("MyDevice") myModule = ComplexDataFormat("MyModule") # add
+the properties to the complex objects # (property_name, property_datatype,
+isArray) myModule.addProperty("moduleName", DataType.STRING, False)
+myDevice.addProperty("deviceName", DataType.STRING, False) myDevice.addProperty
+("deviceWeight", DataType.FLOAT, False) myDevice.addProperty("submodules",
+myModule, True) # add the event (with the root of the nested complex object)
+myMsbClient.addEvent( event_id, event_name, event_description, myDevice,
+event_priority, isArray, ) ``` ### Alternative 3: Complex event creation sample
+(using json object): ```python event_id = "E3" event_name = "EVENT " + event_id
+event_description = "EVENT Description " + event_id event_priority = 1 # 0
+(LOW), 1 (MEDIUM), 2 (HIGH) isArray = False # just one value or array of it? #
+add the event (with the MSB-ready json object) myMsbClient.addEvent( event_id,
+event_name, event_description, { "Team" : { "type" : "object", "properties" :
+{ "staff" : { "type" : "array", "items" : { "$ref" : "#/definitions/Member" } }
+} }, "Member" : { "type" : "object", "properties" : { "name" : { "type" :
+"string" }, "status" : { "enum" : [ "present", "absent" ], "type" : "string" }
+} }, "dataObject" : { "$ref" : "#/definitions/Team" } }, event_priority,
+isArray, ) ``` See `app_sample.py` for more event creation examples. ## Add
+Functions Add `functions` and their implementations your smart object /
+application is able to handle. ### Alternative 1: Simple function creation
+sample (using method params): ```python function_id = "F1" function_name =
+"FUNC " + function_id function_description = "FUNC Description " + function_id
+function_dataformat = DataType.STRING isArray = False # handle array of values
+or just one value? responseEvents = None # you can link to response events here
+by a list of event is e.g. ["E1"] # define the function which will be passed to
 the function description # this function implementation will be called def
 printMsg(msg): print(str(msg["dataObject"])) # add the function
 myMsbClient.addFunction( function_id, function_name, function_description,
-{ "MyCar" : { "type" : "object", "properties" : { "carColor" : { "type" :
-"string" }, "carNrOfSeats" : { "format": "int32", "type": "integer" },
-"carWeight" : { "format": "float", "type": "number" }, "wheels" : { "type" :
-"array", "items" : { "$ref" : "#/definitions/MyWheel" } } } }, "MyWheel" :
-{ "type" : "object", "properties" : { "position" : { "enum" : [ "br", "bl",
-"fr", "fl" ], "type" : "string" } } }, "dataObject" : { "$ref" : "#/
-definitions/MyCar" } }, printMsg, isArray, responseEvents, ) ``` See
-`app_sample.py` of the application template for more (and complex) examples. ##
-Connect and Register Client ```python msb_url = 'ws://127.0.0.1:8085'
-myMsbClient.connect(msb_url) myMsbClient.register() ``` You will get an
-`IO_CONNECTED` and `IO_REGISTERED` event from MSB, if successful. ## Event
-publishing For publishing an event to a websocket broker interface, only the
-`eventId` and `data` are required of the already specified event (see above).
-```python event_id = "E1" event_value = 'Hello World!' myMsbClient.publish
-( event_id, event_value ) ``` The MSB responds with an `IO_PUBLISHED` event, if
-successful. By default events are published with a low priority. It is also
-possible to `set the priority` of an event. There are three possible priorities
-for events like it is shown at the following table. | `Constant` | `Value` | |:
----:|:---:| | LOW | 0 | | MEDIUM| 1 | | HIGH| 2 | ```python event_id = "E1"
-event_value = 'Hello World!' event_priority = 2 myMsbClient.publish( event_id,
-event_value, event_priority ) ``` Another option is to publish an event as
-`cached event` by setting the cache parameter to true. And you can add a `post
-date`. This means that the event is not deleted if the connection is broken.
+function_dataformat, printMsg, isArray, responseEvents, ) ``` ### Alternative
+2: Complex function creation sample (using object): ```python function_id =
+"F2" function_name = "FUNC " + function_id function_description = "FUNC
+Description " + function_id isArray = False # handle array of values or just
+one value? responseEvents = None # you can link to response events here by a
+list of event is e.g. ["E1"] # define a complex data format to be used in an
+event # init the complex data format myCar = ComplexDataFormat("MyCar") # add
+the properties to the complex objects # (property_name, property_datatype,
+isArray) myCar.addProperty("carColor", DataType.STRING, False)
+myCar.addProperty("carNrOfSeats", DataType.INT32, False) myCar.addProperty
+("carWeight", DataType.FLOAT, False) # define the function which will be passed
+to the function description # this function implementation will be called def
+printMsg(msg): print(str(msg["dataObject"])) # add the function
+myMsbClient.addFunction( function_id, function_name, function_description,
+myCar, printMsg, isArray, responseEvents, ) ``` ### Alternative 3: Complex
+function creation sample (using json object): ```python function_id = "F3"
+function_name = "FUNC " + function_id function_description = "FUNC Description
+" + function_id isArray = False # handle array of values or just one value?
+responseEvents = None # you can link to response events here by a list of event
+is e.g. ["E1"] # define the function which will be passed to the function
+description # this function implementation will be called def printMsg(msg):
+print(str(msg["dataObject"])) # add the function myMsbClient.addFunction
+( function_id, function_name, function_description, { "MyCar" : { "type" :
+"object", "properties" : { "carColor" : { "type" : "string" }, "carNrOfSeats" :
+{ "format": "int32", "type": "integer" }, "carWeight" : { "format": "float",
+"type": "number" }, "wheels" : { "type" : "array", "items" : { "$ref" : "#/
+definitions/MyWheel" } } } }, "MyWheel" : { "type" : "object", "properties" :
+{ "position" : { "enum" : [ "br", "bl", "fr", "fl" ], "type" : "string" } } },
+"dataObject" : { "$ref" : "#/definitions/MyCar" } }, printMsg, isArray,
+responseEvents, ) ``` See `app_sample.py` of the application template for more
+(and complex) examples. ## Connect and Register Client ```python msb_url = 'ws:
+//127.0.0.1:8085' myMsbClient.connect(msb_url) myMsbClient.register() ``` You
+will get an `IO_CONNECTED` and `IO_REGISTERED` event from MSB, if successful.
+## Event publishing For publishing an event to a websocket broker interface,
+only the `eventId` and `data` are required of the already specified event (see
+above). ```python event_id = "E1" event_value = 'Hello World!'
+myMsbClient.publish( event_id, event_value ) ``` The MSB responds with an
+`IO_PUBLISHED` event, if successful. By default events are published with a low
+priority. It is also possible to `set the priority` of an event. There are
+three possible priorities for events like it is shown at the following table. |
+`Constant` | `Value` | |:---:|:---:| | LOW | 0 | | MEDIUM| 1 | | HIGH| 2 |
 ```python event_id = "E1" event_value = 'Hello World!' event_priority = 2
-event_isCached = True event_postDate = datetime.datetime.utcnow().isoformat()[:
--3] + "Z" myMsbClient.publish( event_id, event_value, event_priority,
-event_isCached, event_postDate ) ``` You cann also handle `correlation ids` to
-identify an event among flows. ```python event_id = "E1" event_value = 'Hello
+myMsbClient.publish( event_id, event_value, event_priority ) ``` Another option
+is to publish an event as `cached event` by setting the cache parameter to
+true. And you can add a `post date`. This means that the event is not deleted
+if the connection is broken. ```python event_id = "E1" event_value = 'Hello
 World!' event_priority = 2 event_isCached = True event_postDate =
-datetime.datetime.utcnow().isoformat()[:-3] + "Z" event_correlationId =
-"72047f33-a9ae-4aa5-b7ae-c1c4a2797cac" myMsbClient.publish( event_id,
-event_value, event_priority, event_isCached, event_postDate,
-event_correlationId ) ``` For values based on complex data formats it will look
-like this: ```python event_id = "E2" event_priority = 2 event_isCached = True
-event_postDate = datetime.datetime.utcnow().isoformat()[:-3] + "Z"
-event_correlationId = "72047f33-a9ae-4aa5-b7ae-c1c4a2797cac" # pepare the
-complex ovbject based on a complex data format # use it as event value
+datetime.datetime.utcnow().isoformat()[:-3] + "Z" myMsbClient.publish
+( event_id, event_value, event_priority, event_isCached, event_postDate ) ```
+You cann also handle `correlation ids` to identify an event among flows.
+```python event_id = "E1" event_value = 'Hello World!' event_priority = 2
+event_isCached = True event_postDate = datetime.datetime.utcnow().isoformat()[:
+-3] + "Z" event_correlationId = "72047f33-a9ae-4aa5-b7ae-c1c4a2797cac"
+myMsbClient.publish( event_id, event_value, event_priority, event_isCached,
+event_postDate, event_correlationId ) ``` For values based on complex data
+formats it will look like this: ```python event_id = "E2" event_priority = 2
+event_isCached = True event_postDate = datetime.datetime.utcnow().isoformat()[:
+-3] + "Z" event_correlationId = "72047f33-a9ae-4aa5-b7ae-c1c4a2797cac" # pepare
+the complex ovbject based on a complex data format # use it as event value
 myModuleObj = {} myModuleObj['moduleName'] = 'Module 1' myDeviceObj = {}
 myDeviceObj['deviceName'] = 'Device 1' myDeviceObj['deviceWeight'] = 1.3
 myDeviceObj['submodules'] = [myModuleObj] myMsbClient.publish( event_id,
 myDeviceObj, event_priority, event_isCached, event_postDate,
 event_correlationId ) ``` ## Function call handling As shown above the
 addFunction method includes a `function pointer` to point to the function
 implementation. ## Configuration parameters Configuration parameters are a
```

### Comparing `msb-client-websocket-python-1.0.8/msb_client_websocket_python.egg-info/SOURCES.txt` & `msb-client-websocket-python-1.0.9/msb_client_websocket_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/test/test_integration.py` & `msb-client-websocket-python-1.0.9/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/test/test_unit.py` & `msb-client-websocket-python-1.0.9/test/test_unit.py`

 * *Files identical despite different names*

### Comparing `msb-client-websocket-python-1.0.8/setup.py` & `msb-client-websocket-python-1.0.9/setup.py`

 * *Files identical despite different names*

