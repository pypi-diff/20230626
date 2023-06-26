# Comparing `tmp/decode-config-13.0.0.0.tar.gz` & `tmp/decode-config-2022.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decode-config-13.0.0.0.tar", last modified: Mon Jun 26 15:15:30 2023, max compression
+gzip compressed data, was "decode-config-2022.1.tar", last modified: Sun Jan  9 08:16:25 2022, max compression
```

## Comparing `decode-config-13.0.0.0.tar` & `decode-config-2022.1.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:30.399428 decode-config-13.0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-26 15:15:20.000000 decode-config-13.0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    68302 2023-06-26 15:15:30.399428 decode-config-13.0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    67681 2023-06-26 15:15:20.000000 decode-config-13.0.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)   412538 2023-06-26 15:15:20.000000 decode-config-13.0.0.0/decode-config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:15:30.399428 decode-config-13.0.0.0/decode_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    68302 2023-06-26 15:15:30.000000 decode-config-13.0.0.0/decode_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-26 15:15:30.000000 decode-config-13.0.0.0/decode_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:15:30.000000 decode-config-13.0.0.0/decode_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 15:15:30.000000 decode-config-13.0.0.0/decode_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 15:15:30.000000 decode-config-13.0.0.0/decode_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 15:15:30.399428 decode-config-13.0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-26 15:15:20.000000 decode-config-13.0.0.0/setup.py
+drwxrwxr-x   0 curzon    (1000) curzon    (1000)        0 2022-01-09 08:16:25.589192 decode-config-2022.1/
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)     7653 2019-12-08 10:13:57.000000 decode-config-2022.1/LICENSE
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)    59382 2022-01-09 08:16:25.589192 decode-config-2022.1/PKG-INFO
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)    58726 2022-01-08 08:58:35.000000 decode-config-2022.1/README.md
+drwxrwxr-x   0 curzon    (1000) curzon    (1000)        0 2022-01-09 08:16:25.589192 decode-config-2022.1/decode_config.egg-info/
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)    59382 2022-01-09 08:16:25.000000 decode-config-2022.1/decode_config.egg-info/PKG-INFO
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)      190 2022-01-09 08:16:25.000000 decode-config-2022.1/decode_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)        1 2022-01-09 08:16:25.000000 decode-config-2022.1/decode_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)        1 2022-01-09 08:16:25.000000 decode-config-2022.1/decode_config.egg-info/top_level.txt
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)       98 2022-01-09 08:15:44.000000 decode-config-2022.1/pyproject.toml
+-rw-rw-r--   0 curzon    (1000) curzon    (1000)      676 2022-01-09 08:16:25.589192 decode-config-2022.1/setup.cfg
```

### Comparing `decode-config-13.0.0.0/LICENSE` & `decode-config-2022.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decode-config-13.0.0.0/PKG-INFO` & `decode-config-2022.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: decode-config
-Version: 13.0.0.0
+Version: 2022.1
 Summary: Backup/restore and decode configuration tool for Tasmota
 Home-page: https://github.com/tasmota/decode-config
 Author: Norbert Richter
 Author-email: nr@prsolution.eu
-Classifier: Development Status :: 5 - Production/Stable
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # decode-config
 
 Convert, backup and restore configuration data of devices flashed with [Tasmota firmware](https://github.com/arendst/Tasmota).
 
 <!-- markdownlint-disable MD033 -->
-<img src="https://github.com/tasmota/decode-config/blob/master/media/pic/decode-config.png" alt="Overview" title="decode-config Overview" width="600">
+<img src="https://github.com/curzon01/media/blob/master/pics/decode-config_overview.png" alt="Overview" title="decode-config Overview" width="600">
 
 <!-- markdownlint-disable MD033 -->
-[![master](https://img.shields.io/badge/master-v13.0.0.0-blue.svg)](https://github.com/tasmota/decode-config/tree/master)
+[![development](https://img.shields.io/badge/development-v2022.01.2-blue.svg)](https://github.com/tasmota/decode-config/tree/development)
 [![GitHub download](https://img.shields.io/github/downloads/tasmota/decode-config/total.svg)](https://github.com/tasmota/decode-config/releases/latest)
-[![PyPI version](https://badge.fury.io/py/decode-config.svg)](https://badge.fury.io/py/decode-config)
-![PyPI downloads](https://img.shields.io/pypi/dm/decode-config?label=pypi%20downloads)
 [![License](https://img.shields.io/github/license/tasmota/decode-config.svg)](LICENSE)
 
 If you like **decode-config** give it a star or fork it and contribute:
 
 [![GitHub stars](https://img.shields.io/github/stars/tasmota/decode-config.svg?style=social&label=Star)](https://github.com/tasmota/decode-config/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/tasmota/decode-config.svg?style=social&label=Fork)](https://github.com/tasmota/decode-config/network)
 [![donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://paypal.me/NorbertRichterDE)
@@ -49,229 +49,205 @@
 |:------------------------|:-----------------------:|:------------------:|
 | encrypted               |           No            |         Yes        |
 | readable                |           Yes           |         No         |
 | editable                |           Yes           |         No         |
 | batch processing        |           Yes           |         No         |
 | Backup/Restore subsets  |           Yes           |         No         |
 
-**decode-config** is compatible with all [Tasmota](https://github.com/arendst/Tasmota) versions, starting from Tasmota v5.10.0 up to the current one.
-
-## Development
+**decode-config** is compatible with [Tasmota](https://github.com/arendst/Tasmota) starting from v5.10.0 up to now.
 
-Using the latest development version of decode-config is only necessary if you also use the latest development version of Tasmota.
+## Content
 
-<!-- markdownlint-disable MD033 -->
-[![development version](https://img.shields.io/badge/development-v13.0.0.0-blue.svg)](https://github.com/tasmota/decode-config/tree/development)
+**This is the developer branch which contains decode-config matching the latest Tasmota developer version.**
 
-## Table of contents
+This branch does not contain any binaries. If you want to use a precompiled **decode-config** binary
+you can use binaries from latest [Release](https://github.com/tasmota/decode-config/releases).
 
-* [Development](#development)
-* [Table of contents](#table-of-contents)
-* [Running the program](#running-the-program)
-  * [Installation](#installation)
-* [Usage](#usage)
-  * [Basics](#basics)
-  * [Tasmota source](#tasmota-source)
-  * [Format JSON output](#format-json-output)
-  * [Parameter file](#parameter-file)
-  * [Save backup](#save-backup)
-  * [Restore backup](#restore-backup)
-  * [Auto file extensions](#auto-file-extensions)
-  * [Test your parameter](#test-your-parameter)
-  * [Console outputs](#console-outputs)
-  * [Filter by groups](#filter-by-groups)
-* [Usage examples](#usage-examples)
-  * [Using Tasmota binary configuration files](#using-tasmota-binary-configuration-files)
-  * [Using JSON editable file](#using-json-editable-file)
-  * [Use batch processing](#use-batch-processing)
-* [File Formats](#file-formats)
-  * [.dmp format](#dmp-format)
-  * [.json format](#json-format-1)
-  * [.bin format](#bin-format)
-* [Program parameter list](#program-parameter-list)
-  * [--full-help](#--full-help)
-  * [Parameter notes](#parameter-notes)
-  * [Obsolete parameters](#obsolete-parameters)
-* [Generated Tasmota commands](#generated-tasmota-commands)
-* [Program return codes](#program-return-codes)
+> **Note**  
+If you want to run the development **decode-config.py** from this branch, you need an
+installed [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) environment.
+See [Running as Python script](#running-as-python-script) for more details.
+
+### Files
+
+| File                     | Description |
+|:-------------------------|:------------------------------------------------------------------------|
+| `build`                  | contains files to build executables                                     |
+| `decode-config.py`       | Python source file running under your local Python environment          |
+| `README.md`              | This content                                                            |
+
+### Table of contents
+
+* [decode-config](#decode-config)
+  * [Content](#content)
+    * [Files](#files)
+    * [Table of contents](#table-of-contents)
+  * [Running the program](#running-the-program)
+    * [Prerequisite](#prerequisite)
+  * [Usage](#usage)
+    * [Basics](#basics)
+    * [Format JSON output](#format-json-output)
+    * [Parameter file](#parameter-file)
+    * [Save backup](#save-backup)
+    * [Restore backup](#restore-backup)
+    * [Auto file extensions](#auto-file-extensions)
+    * [Test your parameter](#test-your-parameter)
+    * [Console outputs](#console-outputs)
+    * [Filter by groups](#filter-by-groups)
+    * [Usage examples](#usage-examples)
+  * [File Formats](#file-formats)
+    * [.dmp format](#dmp-format)
+    * [.json format](#json-format)
+    * [.bin format](#bin-format)
+  * [Program parameter list](#program-parameter-list)
+    * [--full-help](#--full-help)
+    * [Parameter notes](#parameter-notes)
+    * [Obsolete parameters](#obsolete-parameters)
+  * [Generated Tasmota commands](#generated-tasmota-commands)
+  * [Program return codes](#program-return-codes)
 
 ## Running the program
 
-To use **decode-config.py** you can install it using Python environment and following the [Installation](#installation) section below.
-
-Alternatively you can download a ready-made binary from [Releases](https://github.com/tasmota/decode-config/releases) to use it without installing Python.
-
-### Installation
-
-**decode-config.py** needs an installed [Python](https://en.wikipedia.org/wiki/Python_%28programming_language%29) environment - (see [Prerequisite](#prerequisite)).
-
-After you have installed your Python environment, there are two ways to install deocde-config:
-
-#### Installation using PyPi
-
-```shell
-pip install decode-config
-```
+The program does not have a graphical user interface (GUI), you have to run it from your OS command line using [program arguments](#usage).
 
-The program does not have a graphical user interface (GUI), you have to run it from your OS command line using [program arguments](#usage) - see [Usage](#usage) for more details.
+### Prerequisite
 
-#### Manual installation
+#### Tasmota WebServer
 
-This is only necessary if you want to run **decode-config.py** from [development branch](https://github.com/tasmota/decode-config/tree/development). First install the required modules manually
+[Tasmota](https://github.com/arendst/Tasmota) provides its configuration data by http request only. To receive and send configuration data from Tasmota devices directly the http WebServer in Tasmota must be enabled:
 
-```shell
-python -m pip install -r requirements.txt
-```
+* enable web-server admin mode (Tasmota web command [WebServer 2](https://tasmota.github.io/docs/Commands/#webserver))
+* for self-compiled firmware enable web-server with (`#define USE_WEBSERVER` and `#define WEB_SERVER 2`).
 
-After that you can use the Phython script **decode-config.py** as normal program:
+> **Note**  
+Using MQTT for exchanging Tasmota configuration data is supported by Tasmota since v9.4.0.3; **decode-config** will be able using MQTT in future supporting configuration data exchange this way too.
 
-```shell
-decode-config.py
-```
+#### Python
 
-#### Prerequisite
+**decode-config.py** needs an installed [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) environment.
 
-Since **decode-config.py** is a Python program, it requires an installed [Python](https://en.wikipedia.org/wiki/Python_%28programming_language%29) environment.
+> **Note**  
+Due to the [Python 2.7 EOL](https://github.com/python/devguide/pull/344) in Jan 2020 Python 2.x is no longer supported.
 
 ##### Linux
 
-Install [Python 3.x](https://www.python.org/downloads/) and Pip:
+Install [Python 3.x](https://www.python.org/downloads/), Pip and follow [library installation for all OS](#all-os) below.
 
 ```bash
 sudo apt-get install python3 python3-pip
 ```
 
-##### Windows
+##### Windows 10
 
-Install [Python 3.x](https://www.python.org/downloads/windows/) as described
+Install [Python 3.x](https://www.python.org/downloads/windows/) as described and follow [library installation for all OS](#all-os) below.
 
 ##### MacOS
 
-Install [Python 3.x](https://www.python.org/downloads/mac-osx/) as described
+Install [Python 3.x](https://www.python.org/downloads/mac-osx/) as described and follow [library installation for all OS](#all-os) below.
+
+##### All OS
+
+After python and pip is installed, install dependencies:
+
+```shell
+python -m pip install requests configargparse
+```
 
 ## Usage
 
 For an overview start the program without any parameter and you will get a short help:
 
 <!-- markdownlint-capture -->
 <!-- markdownlint-disable MD031 -->
 ```bash
-decode-config.py
+decode-config
 ```
+> **Note**  
+Replace `decode-config` by the program name your are using:  
+`decode-config.py` when running as Python executable.
+<!-- markdownlint-restore -->
 
 This prints a short help:
 
 ```help
-usage: decode-config.py [-s <filename|host|url>] [-p <password>]
-                        [--fulltopic <topic>] [--cafile <file>]
-                        [--certfile <file>] [--keyfile <file>] [--insecure]
-                        [--keepalive <sec>] [-i <restorefile>]
+usage: decode-config.py [-s <filename|host|url>] [-i <restorefile>]
                         [-o <backupfile>] [-t json|bin|dmp] [-E] [-e] [-F]
                         [--json-indent <indent>] [--json-compact]
                         [--json-show-pw] [--cmnd-indent <indent>]
-                        [--cmnd-groups] [--cmnd-sort]
-                        [--cmnd-use-rule-concat] [--cmnd-use-backlog]
-                        [-c <configfile>] [-S] [-T json|cmnd|command]
+                        [--cmnd-groups] [--cmnd-sort] [--cmnd-use-rule-concat]
+                        [--cmnd-use-backlog] [-c <configfile>] [-S]
+                        [-T json|cmnd|command]
                         [-g <groupname> [<groupname> ...]] [-w] [--dry-run]
                         [-h] [-H] [-v] [-V]
 ```
 
 For advanced help run **decode-config** with parameter `--full--help` or `-H`. This will print a [Program parameter list](#program-parameter-list).
 
 > **Note**  
-If you're missing older parameters, don't worry, they're still there (see [Obsolete parameters](#obsolete-parameters)).
+If you miss parameters here that are already in use, don't worry, they are still there.  
+For details see [Obsolete parameters](#obsolete-parameters)
 
 ### Basics
 
-To get a program result, pass at least a [Tasmota source](#tasmota-source) from which you want to read the configuration data.
-
-### Tasmota source
-
-The Tasmota source determines where the configuration data should be loaded from and saved to.
-A source can be an offline file or an online Tasmota device accessed via HTTP or indirectly via MQTT.
-
-Use `--source` parameter to determine the configuration data source:
+To get a result, at least pass a Tasmota source where you want to read the configuration from.
 
-#### Binary (*.dmp) file (Offline)
+Source can be either
 
-Source is a Tasmota configuration file (having extension `.dmp`).
+* a device hostname, IP or [http-url](https://en.wikipedia.org/wiki/URL) available and online within your network:  
+use `--source <host|url>` or `-s <host|url>` parameter
+* a Tasmota configuration file (having extension `.dmp`):  
+use `--source <filename>` or `-s <filename>` parameter
 
-Pass the filename direclty or encoded as a [file-URL](https://en.wikipedia.org/wiki/URL):
+The [http-url](https://en.wikipedia.org/wiki/URL) variant also allows `<user>`, `<password>` and `<port>` number to be specified:
 
-```bash
-decode-config --source tasmota-4281.dmp
-decode-config -s file://path/to/tasmota-4281.dmp
-```
+* `--source http://admin:myPaszxwo!z@tasmota-4281`
+* `--source http://tasmota-4281:80`
+* `--source http://admin:myPaszxwo!z@tasmota-4281:80`
 
-#### HTTP connection (Online)
+#### Basic example
 
-Source is an online HTTP connection to a running Tasmota device. To use this source, **decode-config** must have access to the network on which Tasmota is running, [Tasmota Webserver](https://tasmota.github.io/docs/Commands/#webserver) running in admin mode (`WebServer 2`) is mandatory.
-
-Specify the hostname, IP o or [http-url](https://en.wikipedia.org/wiki/URL) of the Tasmota device.
-
-An optionally required HTTP password, username and different HTTP port of the device can be specified via [URL](https://en.wikipedia.org/wiki/URL) or separately via `--username`, `--password` and `--port`
+##### Access an online device
 
 ```bash
 decode-config --source tasmota-4281
 decode-config -s 192.168.10.92
-decode-config --source http://tasmota-4281 --password myPaszxwo!z
-decode-config --source http://admin:myPaszxwo!z@tasmota-4281:8000
-decode-config --source http://admin:myPaszxwo!z@tasmota-4281/cs?
+decode-config --source http://tasmota-4281
+decode-config --source http://admin:myPaszxwo!z@tasmota-4281
 ```
 
-An appended HTTP path (here "`/cs?`") is ignored.
-
-#### MQTT transission (Online)
+##### Access a config file
 
-Source is a MQTT server and topic where an online Tasmota device is connected to. To use this source, **decode-config** does not need to have access to the same network that Tasmota is running on, it just needs access to the MQTT server that Tasmota also uses.
+```bash
+decode-config --source tasmota-4281.dmp
+decode-config -s tasmota-4281.dmp
+```
 
-##### MQTT connection parameter
+will output a readable configuration in [JSON](http://www.json.org/)-format, e.g.:
 
-Specify the hostname or IP of the MQTT server (possibly also specify username and password for the MQTT server) and the Tasmota MQTT topic. The **decode-config** connection to MQTT server also allows SSL/TLS connection.
+```json
+{"altitude": 112, "baudrate": 115200, "blinkcount": 10, "blinktime": 10,...
+"ws_width": [1, 3, 5]}
+```
 
-The MQTT username and password must be encoded within the URL (the parameter `--password` can not be used for that, it has a different function here).  
-If the username/password combination for the **decode-config** MQTT connection is different from the one used by Tasmota itself (Tasmota command `MQTTPassword`), the Tasmota MQTT password must be specified via the `--password` parameter.
+> **Note**  
+The json names (like `"altitude"` or `"blinktime"` are internal names from Tasmotas [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/settings.h) STRUCT `Settings` and are not the same as known from Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/). However, since most variable names are self-describing, the functional meaning should be given in most cases.
 
-The Tasmota topic can be specfied either within the [URL path](https://en.wikipedia.org/wiki/URL#Syntax) component or using optional `--fulltopic` parameter.  
-The topic must be the full topic of the Tasmota device without any trailing command or result part. You can use any of the prefixed topic (*cmnd*, *stat* or *tele* topic) or use the placeholder *%prefix%* for it, example  
-`%prefix%/tasmota-4281` or `tele/tasmota-4281` are valid topics  
-`cmnd/tasmota-4281/POWER` or `tele/tasmota-4281/STATE` are invalid topics due to the trailing part.
+#### Password protected device
 
-For SSL/TLS connection to MQTT server use `mqtts://` [URL scheme](https://en.wikipedia.org/wiki/URL#Syntax).
+If you try to access data from a device and you get an error like `ERROR 401: Error on http GET request for http://.../dl - Unauthorized` you need to pass your WebPassword for this device:
 
 ```bash
-decode-config --source mqtts://mybroker.example.com/%prefx%/tasmota-4281
-decode-config --source mqtts://mybroker.example.com:8883/tele/tasmota-4281
-decode-config --source mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com  --fulltopic tele/tasmota-4281
-decode-config --source mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota-4281 --password myTasmotaMQTTPaszxwo!z
+decode-config --source tasmota-4281 --password "myPaszxwo!z"
 ```
 
-For own certifications use the parameters `--cafile`, `--certfile` and `--keyfile`. To suppress certification verification use `--insecure`.
-
-For none SSL/TLS connection to MQTT server use `mqtt://` [URL scheme](https://en.wikipedia.org/wiki/URL#Syntax).
-
-```bash
-decode-config --source mqtt://mybroker.example.com/%prefx%/tasmota-4281
-decode-config --source mqtt://mybroker.example.com:1883/tele/tasmota-4281
-decode-config --source mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com  --fulltopic tele/tasmota-4281
-decode-config --source mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota-4281 --password myTasmotaMQTTPaszxwo!z
-```
+> **Hint**  
+*decode-config* username default is `admin`. For self-compiled binaries using a non-standard web username, use `-u <user>` or `--username <user>`.
 
 ### Format JSON output
 
-All basic examples above will output a readable configuration in [JSON](http://www.json.org/)-format, e.g.:
-
-```json
-{"altitude": 112, "baudrate": 115200, "blinkcount": 10, "blinktime": 10,...
-"ws_width": [1, 3, 5]}
-```
-
-> **Note**  
-The json names (like `"altitude"` or `"blinktime"` are internal names from Tasmotas [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/include/tasmota_types.h) STRUCT `Settings` and are not the same as known from Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/). However, since most variable names are self-describing, the functional meaning should be given in most cases.
-
 The default JSON output can be formatted for better reading using the `--json-indent <n>` parameter:
 
 ```bash
 decode-config --source tasmota-4281 --password "myPaszxwo!z" --json-indent 2
 ```
 
 This will print a pretty better readable format and the example above becomes:
@@ -329,56 +305,52 @@
 
 ### Save backup
 
 To save data from a device or [*.dmp](#dmp-format) file into a backup file, use `--backup-file <filename>`.
 
 #### Backup filename macros
 
-You can use the following placeholders within filenames:
+You can use the following placeholders within backup/restore filenames:
 
-* **@v** is replaced by *Tasmota Version* (backup & restore filenames)
-* **@d** is replaced by *Devicename* (backup & restore filenames)
-* **@f** is replaced by first *Friendlyname1* (backup & restore filenames)
-* **@h** is replaced by the *Hostname* from configuration data (backup & restore filenames)  
-Note: This is the static hostname which is configured by the command *Hostname*, for real hostname from a device use macro the **@H**)
-* **@H** is replaced by the live device hostname  (only for http sources, backup & restore filenames)  
-Note: This can be different to the configured hostname as this can contain also macros).source
-* **@F** is replaced by the filename of MQTT request (only for MQTT sources, backup filenames only).  
-This is usually the filename that Tasmota uses when saving the configuration in the WebUI.
+* **@v** is replaced by _Tasmota Version_
+* **@d** is replaced by _Devicename_
+* **@f** is replaced by first _Friendlyname1_
+* **@h** is replaced by the __Hostname__ from configuration data (note: this is the static hostname which is configured by the command __Hostname__, for real hostname from a device use macro the **@H**)
+* **@H** is replaced by the live device hostname note: this can be different to the configured hostname as this can contain also macros). Only valid when using real devices as source
 
 Example:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 --backup-file Config_@d_@v
 ```
 
-This will create a file like `Config_Tasmota_13.0.json` (the part `Tasmota` and `13.0` will choosen related to your device configuration).
+This will create a file like `Config_Tasmota_10.1.0.json` (the part `Tasmota` and `10.1.0` will choosen related to your device configuration).
 
 #### Save multiple backup at once
 
-The `--backup-file` parameter can be specified multiple times to create different backup with different names and/or different formats at once:
+Since **decode-config** v8.2.0.5 the `--backup-file` parameter can be specified multiple times. With that it's easy to create different backup with different names and/or different formats at once:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 -o Config_@d_@v -o Backup_@H.json -o Backup_@H.dmp
 ```
 
 creates three backup files:
 
-* `Config_Tasmota_13.0.json` using JSON format
+* `Config_Tasmota_10.1.0.json` using JSON format
 * `Backup_tasmota-4281.json` using JSON format
 * `Backup_tasmota-4281.dmp` using Tasmota configuration file format
 
 ### Restore backup
 
 Reading back a previously saved backup file, use the `--restore-file <filename>` parameter.
 
-To restore the previously save backup file `Config_Tasmota_13.0.json` to device `tasmota-4281` use:
+To restore the previously save backup file `Config_Tasmota_10.1.0.json` to device `tasmota-4281` use:
 
 ```bash
-decode-config -c my.conf -s tasmota-4281 --restore-file Config_Tasmota_13.0
+decode-config -c my.conf -s tasmota-4281 --restore-file Config_Tasmota_10.1.0
 ```
 
 Restore operation also allows placeholders **@v**, **@d**, **@f**, **@h** or **@H** like in backup filenames so we can use the same naming as for the backup process:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 --restore-file Config_@d_@v
 ```
@@ -456,17 +428,17 @@
 ### Console outputs
 
 Output to the console screen is the default when calling the program without any backup or restore parameter.  
 Screen output is suppressed when using backup or restore parameter. In that case you can force screen output with `--output`.
 
 The console screen output supports two formats:
 
-* [JSON](#json-format):<br>
+* [JSON](#console-json-format):<br>
 This is identical with the backup/restore [json file Format](#json-format) but printed on screen standard output.
-* [Tasmota command](#tasmota-web-command-format):<br>
+* [Tasmota command](#console-tasmota-command-format):<br>
 This outputs the most (but not all!) configuration data as Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/).
 
 #### JSON format
 
 The default console output format is [JSON](#json-format) (optional you can force JSON backup format using `--output-format json`).
 
 Example:
@@ -615,76 +587,39 @@
 
 ```bash
 decode-config -s tasmota-4281 -c my.conf --output-format cmnd --group Main MQTT Management Wifi
 ```
 
 Filtering by groups affects the entire output, regardless of whether screen output or backup file.
 
-## Usage examples
-
-### Using Tasmota binary configuration files
-
-These examples use an online Tasmota device accessed over HTTP. The hostname of the Tasmota device is `tasmota-2f5d44-4281`
-
-#### Backup an online Tasmota device via HTTP into a Tasmota configuration file
-
-##### Use args to choice the file format
-
-```bash
-  decode-config -c my.conf -s tasmota-2f5d44-4281 --backup-type dmp --backup-file Config_@d_@v
-```
-
-##### Use file extension to choice the file format
-
-```bash
-decode-config -c my.conf -s tasmota-2f5d44-4281 --backup-file Config_@d_@v.dmp
-```
-
-#### Restore a Tasmota configuration file to an online Tasmota device via HTTP
-
-```bash
-decode-config -c my.conf -s http://tasmota-2f5d44-4281 --restore-file Config_@d_@v.dmp
-```
-
-### Using JSON editable file
-
-These examples use an online Tasmota device that is accessed indirectly via MQTT.
-
-In these examples, the MQTT server parameters are the same as those used by Tasmota itself:
+### Usage examples
 
-* MQTT Server: `mybroker.example.com`
-* MQTT Username: `mqttuser`
-* MQTT Password: `myBrokerPaszxwo!z`
-* Tasmota topic: `tele/tasmota_2F5D44`
+#### Using Tasmota binary configuration files
 
-#### Backup an online Tasmota device via MQTT into a JSON file
+1. Restore a Tasmota configuration file
 
-##### Use an unencrypted MQTT connection
-
-MQTT server uses a non default port 42110
-
-```bash
-decode-config -s mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com:42110/tele/tasmota_2F5D44 --backup-file Config_2f5d44-4281.json
-```
+  ```bash
+  decode-config -c my.conf -s tasmota --restore-file Config_Tasmota_6.2.1.dmp
+  ```
 
-##### Use SSL/TLS MQTT connection
+1. Backup device using Tasmota configuration compatible format
 
-Limit the configuration data to the groups `Control`, `Management` and `SetOption`
+   a) use file extension to choice the file format
 
-```bash
-decode-config -s mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com --fulltopic tele/tasmota_2F5D44 --backup-file Config_2f5d44-4281.json -g Control Management SetOption
-```
+  ```bash
+  decode-config -c my.conf -s tasmota --backup-file Config_@d_@v.dmp
+  ```
 
-#### Restore a JSON file to an online Tasmota device via MQTT
+   b) use args to choice the file format
 
-```bash
-decode-config -s mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota_2F5D44 --restore-file Config_2f5d44-4281.json
-```
+  ```bash
+    decode-config -c my.conf -s tasmota --backup-type dmp --backup-file Config_@d_@v
+  ```
 
-### Use batch processing
+#### Use batch processing
 
 Linux
 
 ```bash
 for device in tasmota1 tasmota2 tasmota3; do ./decode-config -c my.conf -s $device -o Config_@d_@v
 ```
 
@@ -708,18 +643,18 @@
 
 ### .json format
 
 This format uses the [JSON](http://www.json.org/) notation and contains the complete configuration data in plain text, human readable and editable.
 
 The .json format can be created by **decode-config** using the backup function (`--backup-file <filename>`) (for better identification you can append the optional parameter `--backup-type json`, but that's optional as json is the default backup format).
 
-In contrast to the other two binary formats [.dmp](#dmp-format) and [.bin](#bin-format), this type of format also allows the [partial modification](#restore-subset-of-data) of configurations.
+In contrast to the other two binary formats [.dmp](#dmp-format) and [.bin](#bin-format), this type of format also allows the [partial modification](#restore-a-subset-of-backup-data) of configurations.
 
 > **Note**  
-The keys used within the JSON file are based on the variable names of Tasmota source code in [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/include/tasmota_types.h) so they do not have the same naming as known for Tasmota web commands. However, since the variable names are self-explanatory, there should be no difficulties in assigning the functionality of the variables.
+The keys used within the JSON file are based on the variable names of Tasmota source code in [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/settings.h) so they do not have the same naming as known for Tasmota web commands. However, since the variable names are self-explanatory, there should be no difficulties in assigning the functionality of the variables.
 
 ### .bin format
 
 This format is binary with the same structure as the [.dmp](#dmp-format) format. The differences to .dmp are:
 
 * .bin is decrypted
 * .bin has 4 additional bytes at the end of the file
@@ -737,84 +672,58 @@
 A short list of possible program args is displayed using `-h` or `--help`.
 
 ### --full-help
 
 For advanced help use parameter `-H` or `--full-help`:
 
 ```help
-usage: decode-config.py [-s <filename|host|url>] [-p <password>]
-                        [--fulltopic <topic>] [--cafile <file>]
-                        [--certfile <file>] [--keyfile <file>] [--insecure]
-                        [--keepalive <sec>] [-i <restorefile>]
+usage: decode-config.py [-s <filename|host|url>] [-i <restorefile>]
                         [-o <backupfile>] [-t json|bin|dmp] [-E] [-e] [-F]
                         [--json-indent <indent>] [--json-compact]
                         [--json-show-pw] [--cmnd-indent <indent>]
-                        [--cmnd-groups] [--cmnd-sort]
-                        [--cmnd-use-rule-concat] [--cmnd-use-backlog]
-                        [-c <configfile>] [-S] [-T json|cmnd|command]
+                        [--cmnd-groups] [--cmnd-sort] [--cmnd-use-rule-concat]
+                        [--cmnd-use-backlog] [-c <configfile>] [-S]
+                        [-T json|cmnd|command]
                         [-g <groupname> [<groupname> ...]] [-w] [--dry-run]
                         [-h] [-H] [-v] [-V]
 
-Backup/Restore Tasmota configuration data. Args that start with '--' (eg.
--s) can also be set in a config file (specified via -c). Config file syntax
+Backup/Restore Tasmota configuration data. Args that start with '--' (eg. -s)
+can also be set in a config file (specified via -c). Config file syntax
 allows: key=value, flag=true, stuff=[a,b,c] (for details, see syntax at
 https://goo.gl/R74nmi). If an arg is specified in more than one place, then
 commandline values override config file values which override defaults.
 
 Source:
   Read/Write Tasmota configuration from/to
 
   -s, --source <filename|host|url>
                         source used for the Tasmota configuration (default:
-                        None). Specify source type, path, file, user,
-                        password, hostname, port and topic at once as an
-                        URL. The URL must be in the form 'scheme://[username
-                        [:password]@]host[:port][/topic]|pathfile'where
-                        scheme is 'file' for a tasmota binary config file,
-                        'http' for a Tasmota HTTP web connection and
-                        'mqtt(s)' for Tasmota MQTT transport ('mqtts' uses a
-                        TLS connection to MQTT server)
-  -p, --password <password>
-                        Web server password on HTTP source (set by Tasmota
-                        'WebPassword' command), MQTT server password in MQTT
-                        source (set by Tasmota 'MqttPassword' command)
-                        (default: None)
-
-MQTT:
-  MQTT transport settings
-
-  --fulltopic <topic>   Optional MQTT transport fulltopic used for accessing
-                        Tasmota device (default: )
-  --cafile <file>       Enables SSL/TLS connection: path to a or filename of
-                        the Certificate Authority certificate files that are
-                        to be treated as trusted by this client (default
-                        None)
-  --certfile <file>     Enables SSL/TLS connection: filename of a PEM
-                        encoded client certificate file (default None)
-  --keyfile <file>      Enables SSL/TLS connection: filename of a PEM
-                        encoded client private key file (default None)
-  --insecure            suppress verification of the MQTT server hostname in
-                        the server certificate (default False)
-  --keepalive <sec>     keepalive timeout for the client (default 60)
+                        None). The argument can be a <filename> containing
+                        Tasmota .dmp configuation data or a <hostname>,
+                        <ip>-address, <url> which means an online tasmota
+                        device is used. A url can also contain web login and
+                        port data in the format
+                        http://<user>:<password>@tasmota:<port>, e. g,
+                        http://admin:mypw@mytasmota:8090
 
 Backup/Restore:
   Backup & restore specification
 
   -i, --restore-file <restorefile>
                         file to restore configuration from (default: None).
                         Replacements: @v=firmware version from config,
                         @d=devicename, @f=friendlyname1, @h=hostname from
-                        config, @H=device hostname (http source only)
+                        config, @H=device hostname (invalid if using a file as
+                        source)
   -o, --backup-file <backupfile>
                         file to backup configuration to, can be specified
                         multiple times (default: None). Replacements:
                         @v=firmware version from config, @d=devicename,
                         @f=friendlyname1, @h=hostname from config, @H=device
-                        hostname (http source only), @F=configuration
-                        filename from MQTT request (mqtt source only)
+                        hostname (invalid if using a file as source)
   -t, --backup-type json|bin|dmp
                         backup filetype (default: 'json')
   -E, --extension       append filetype extension for -i and -o filename
                         (default)
   -e, --no-extension    do not append filetype extension, use -i and -o
                         filename as passed
   -F, --force-restore   force restore even configuration is identical
@@ -830,23 +739,22 @@
   --json-show-pw        unhide passwords (default)
 
 Tasmota command output:
   Tasmota command output format specification. To revert an option, insert
   "dont" or "no" after "cmnd", e.g. --cmnd-no-indent, --cmnd-dont-sort
 
   --cmnd-indent <indent>
-                        Tasmota command grouping indent level (default:
-                        '2'). 0 disables indent
+                        Tasmota command grouping indent level (default: '2').
+                        0 disables indent
   --cmnd-groups         group Tasmota commands (default)
   --cmnd-sort           sort Tasmota commands (default)
   --cmnd-use-rule-concat
                         use rule concatenation with + for Tasmota 'Rule'
                         command
-  --cmnd-use-backlog    use 'Backlog' for Tasmota commands as much as
-                        possible
+  --cmnd-use-backlog    use 'Backlog' for Tasmota commands as much as possible
 
 Common:
   Optional arguments
 
   -c, --config <configfile>
                         program config file - can be used to set default
                         command parameters (default: None)
@@ -854,16 +762,16 @@
                         (default do not output on backup or restore usage)
   -T, --output-format json|cmnd|command
                         display output format (default: 'json')
   -g, --group <groupname>
                         limit data processing to command groups (default no
                         filter)
   -w, --ignore-warnings
-                        do not exit on warnings. Not recommended, used by
-                        your own responsibility!
+                        do not exit on warnings. Not recommended, used by your
+                        own responsibility!
   --dry-run             test program without changing configuration data on
                         device or file
 
 Info:
   Extra information
 
   -h, --help            show usage help message and exit
@@ -879,15 +787,15 @@
 For details see [Obsolete parameters](#obsolete-parameters)
 
 ### Parameter notes
 
 * Filename replacement macros **@h** and **@H**:
   * **@h**
 The **@h** replacement macro uses the hostname configured with the Tasomta Wifi `Hostname <host>` command (defaults to `%s-%04d`). It will not use the network hostname of your device because this is not available when working with files only (e.g. `--source <filename>` as source).
-To prevent having an useless % in your filename, **@h** will not replaced by hostname if this contains '%' characters.
+To prevent having a useless % in your filename, **@h** will not replaced by hostname if this contains '%' characters.
   * **@H**
 If you want to use the network hostname within your filename, use the **@H** replacement macro instead - but be aware this will only replaced if you are using a network device as source (`<hostname>`, `<ip>`, `<url>`); it will not work when using a file as source (`<filename>`)
 
 ### Obsolete parameters
 
 The parameters listed here continue to work and are supported, but are no longer listed in the parameter list:
 
@@ -899,14 +807,16 @@
 file used for the Tasmota configuration (default: None)'
 * `-d`, `--device`, `--host` `<host|url>`  
 hostname, IP-address or url used for the Tasmota configuration (default: None)
 * `-P`, `--port` `<port>`  
 TCP/IP port number to use for the host connection (default: 80)
 * `-u`, `--username` `<username>`  
 host HTTP access username (default: admin)
+* `-p`, `--password` `<password>`  
+host HTTP access password (default: None)
 
 #### Obsolete JSON formating parameters
 
 * `--json-unhide-pw` same as `--json-show-pw`
 * `--json-hide-pw` same as `--json-dont-show-pw`
 * `--json-sort` sorts JSON output (this is the default)
 * `--json-unsort` prevents JSON sorting
@@ -938,94 +848,64 @@
 |                | LedState                    |                        |             |
 |                | Power<x\>                   |                        |             |
 |                | PowerOnState                |                        |             |
 |                | PulseTime<x\>               |                        |             |
 |                | SwitchDebounce              |                        |             |
 |                | SwitchMode<x\>              |                        |             |
 |                | Webbutton<x\>               |                        |             |
-|                | WCAEC<sup>2</sup>           |                        |             |
-|                | WCAECDSP<sup>2</sup>        |                        |             |
-|                | WCAECValue<sup>2</sup>      |                        |             |
-|                | WCAELevel<sup>2</sup>       |                        |             |
-|                | WCAGCGain<sup>2</sup>       |                        |             |
-|                | WCAWB<sup>2</sup>           |                        |             |
-|                | WCAWBGain<sup>2</sup>       |                        |             |
-|                | WCBPC<sup>2</sup>           |                        |             |
-|                | WCBrightness<sup>2</sup>    |                        |             |
-|                | WCClock<sup>2</sup>         |                        |             |
-|                | WCColorbar<sup>2</sup>      |                        |             |
-|                | WCContrast<sup>2</sup>      |                        |             |
-|                | WCDCW<sup>2</sup>           |                        |             |
-|                | WCFeature<sup>2</sup>       |                        |             |
-|                | WCFlip<sup>2</sup>          |                        |             |
-|                | WCGainCeiling<sup>2</sup>   |                        |             |
-|                | WCGammaCorrect<sup>2</sup>  |                        |             |
-|                | WCLensCorrect<sup>2</sup>   |                        |             |
+|                | WCStream<sup>2</sup>        |                        |             |
 |                | WCMirror<sup>2</sup>        |                        |             |
-|                | WCResolution<sup>2</sup>    |                        |             |
+|                | WCFlip<sup>2</sup>          |                        |             |
 |                | WCRtsp<sup>2</sup>          |                        |             |
-|                | WCSAuth<sup>2</sup>         |                        |             |
+|                | WCBrightness<sup>2</sup>    |                        |             |
+|                | WCContrast<sup>2</sup>      |                        |             |
 |                | WCSaturation<sup>2</sup>    |                        |             |
-|                | WCSpecialEffect<sup>2</sup> |                        |             |
-|                | WCStream<sup>2</sup>        |                        |             |
-|                | WCWBMode<sup>2</sup>        |                        |             |
-|                | WCWPC<sup>2</sup>           |                        |             |
+|                | WCResolution<sup>2</sup>    |                        |             |
 | **Management** | DeepSleepTime               | *Delay*                |             |
 |                | DeviceName                  | *Gpios*                |             |
 |                | Emulation                   | *I2Cscan*              |             |
 |                | FriendlyName<x\>            | *Modules*              |             |
 |                | Gpio<x\>                    | *Reset*                |             |
 |                | I2CDriver<x\>               | *Restart*              |             |
 |                | Ifx                         | *State*                |             |
 |                | IfxBucket                   | *Status*               |             |
 |                | IfxHost                     | *Upgrade*              |             |
 |                | IfxPassword                 | *Upload*               |             |
 |                | IfxPort                     | *SSPMLog<sup>2</sup>*  |             |
 |                | IfxUser                     | *SSPEnergy<sup>2</sup>*|             |
-|                | IfxRP                       | *SSPHistory<sup>2</sup>*|            |
-|                | IfxPeriod                   | *SSPScan<sup>2</sup>*  |             |
-|                | IfxSensor                   | *SSPIamHere<sup>2</sup>*|            |
-|                | L1MusicSync                 |                        |             |
-|                | LogHost                     |                        |             |
+|                | IfxPeriod                   | *SSPHistory<sup>2</sup>*|            |
+|                | L1MusicSync                 | *SSPScan<sup>2</sup>*  |             |
+|                | LogHost                     | *SSPIamHere<sup>2</sup>*|            |
 |                | LogPort                     |                        |             |
 |                | Module                      |                        |             |
 |                | Module2                     |                        |             |
 |                | MqttLog                     |                        |             |
 |                | NtpServer<x\>               |                        |             |
 |                | OtaUrl                      |                        |             |
 |                | Pwm<x\>                     |                        |             |
 |                | PwmFrequency                |                        |             |
 |                | PwmRange                    |                        |             |
-|                | RtcNtpserver                |                        |             |
 |                | SaveData                    |                        |             |
 |                | SerialLog                   |                        |             |
 |                | Sleep                       |                        |             |
 |                | SSPMDisplay<sup>2</sup>     |                        |             |
 |                | SysLog                      |                        |             |
 |                | Template                    |                        |             |
 |                | Time                        |                        |             |
 |                | TimeSTD                     |                        |             |
 |                | TimeDST                     |                        |             |
 |                | Timezone                    |                        |             |
-|                | TouchThres<sup>2</sup>      |                        |             |
 |                | TuyaMCU                     |                        |             |
 |                | TuyaTempSetRes              |                        |             |
 |                | WebLog                      |                        |             |
-|                | WebTime                     |                        |             |
 | **WiFi**       | CORS                        | *AP*                   |             |
-|                | DnsTimeout                  | *Ping<x\>*             |             |
-|                | Ethernet<sup>2</sup>        | *WebSend*              |             |
-|                | EthAddress<sup>2</sup>      | *Publish*              |             |
-|                | EthClockMode<sup>2</sup>    | *Publish2*             |             |
-|                | EthType<sup>2</sup>         |                        |             |
-|                | EthIPAddress<sup>2</sup>    |                        |             |
-|                | EthSubnetmask<sup>2</sup>   |                        |             |
-|                | EthGateway<sup>2</sup>      |                        |             |
-|                | EthDNSServer<sup>2</sup>    |                        |             |
-|                | EthDNSServer2<sup>2</sup>   |                        |             |
+|                | Ethernet<sup>2</sup>        | *Ping<x\>*             |             |
+|                | EthAddress<sup>2</sup>      | *WebSend*              |             |
+|                | EthClockMode<sup>2</sup>    | *Publish*              |             |
+|                | EthType<sup>2</sup>         | *Publish2*             |             |
 |                | Hostname                    |                        |             |
 |                | IPAddress<x\>               |                        |             |
 |                | Password<x\>                |                        |             |
 |                | RgxAddress                  |                        |             |
 |                | RgxNAPT                     |                        |             |
 |                | RgxPassword                 |                        |             |
 |                | RgxSsid                     |                        |             |
@@ -1056,15 +936,14 @@
 |                | MqttTimeout                 |                        |             |
 |                | MqttWifiTimeout             |                        |             |
 |                | PowerRetain                 |                        |             |
 |                | Prefix<x\>                  |                        |             |
 |                | SensorRetain                |                        |             |
 |                | StateRetain                 |                        |             |
 |                | StateText<x\>               |                        |             |
-|                | StatusRetain                |                        |             |
 |                | SwitchRetain                |                        |             |
 |                | SwitchTopic                 |                        |             |
 |                | TelePeriod                  |                        |             |
 |                | Topic                       |                        |             |
 | **Rules**      | CalcRes                     | *Add<x\>*              |             |
 |                | Mem<x\>                     | *Event*                |             |
 |                | Rule<x\>                    | *Mult<x\>*             |             |
@@ -1102,28 +981,25 @@
 |                | OT_TWater                   |                        |             |
 |                | Sensor13                    |                        |             |
 |                | Sensor15                    |                        |             |
 |                | Sensor18                    |                        |             |
 |                | Sensor20                    |                        |             |
 |                | Sensor29                    |                        |             |
 |                | Sensor34                    |                        |             |
-|                | Sensor40                    |                        |             |
 |                | Sensor54                    |                        |             |
 |                | Sensor68                    |                        |             |
-|                | Sensor96                    |                        |             |
 |                | Shift595DeviceCount         |                        |             |
 |                | SpeedUnit                   |                        |             |
 |                | TempRes                     |                        |             |
 |                | TempOffset                  |                        |             |
 |                | VoltRes                     |                        |             |
 |                | WattRes                     |                        |             |
 |                | WeightRes                   |                        |             |
-|                | Wiper<x\>                   |                        |             |
 | **Power**      | AmpRes                      | *CurrentSet*           |             |
-|                | CurrentCal                  | *FrequencySet*         |             |
+|                | CurrentCal                  | *FrequencySet*         |`EnergyReset`|
 |                | CurrentHigh                 | *ModuleAddress*        |             |
 |                | CurrentLow                  | *PowerSet*             |             |
 |                | EnergyRes                   | *Status8*              |             |
 |                | EnergyToday                 | *Status9*              |             |
 |                | EnergyTotal                 | *VoltageSet*           |             |
 |                | EnergyYesterday             |                        |             |
 |                | FreqRes                     |                        |             |
@@ -1153,30 +1029,27 @@
 |                | ShdWarmupBrightness         |                        |             |
 |                | ShdWarmupTime               |                        |             |
 |                | Speed                       |                        |             |
 |                | StepPixels                  |                        |             |
 |                | Wakeup                      |                        |             |
 |                | WakeupDuration              |                        |             |
 | **RF**         | RfProtocol                  | *RfRaw*                | `RfCode`    |
-|                | RfTimeOut                   |                        | `RfHigh`    |
+|                |                             |                        | `RfHigh`    |
 |                |                             |                        | `RfHost`    |
 |                |                             |                        | `RfKey<x>`  |
 |                |                             |                        | `RfLow`     |
 |                |                             |                        | `RfSync`    |
 | **IR**         |                             | *IRsend<x\>*           |             |
 |                |                             | *IRhvac*               |             |
 | **SetOption**  | SetOption<x\>               |                        |             |
 | **Serial**     | Baudrate                    | *SerialSend<x\>*       |             |
-|                | ModbusBaudrate              | *SSerialSend<x\>*      |             |
-|                | ModbusSerialConfig          | *TCPStart*             |             |
-|                | SBaudrate                   | *TuyaSend<x\>*         |             |
-|                | SerialConfig                |                        |             |
-|                | SerialDelimiter             |                        |             |
+|                | SBaudrate                   | *SSerialSend<x\>*      |             |
+|                | SerialConfig                | *TCPStart*             |             |
+|                | SerialDelimiter             | *TuyaSend<x\>*         |             |
 |                | SSerialConfig               |                        |             |
-|                | SSerialSend9                |                        |             |
 |                | TCPBaudrate                 |                        |             |
 |                | TCPConfig                   |                        |             |
 | **Domoticz**   | DomoticzIdx<x\>             |                        |             |
 |                | DomoticzKeyIdx<x\>          |                        |             |
 |                | DomoticzSensorIdx<x\>       |                        |             |
 |                | DomoticzSwitchIdx<x\>       |                        |             |
 |                | DomoticzUpdateTimer         |                        |             |
@@ -1203,18 +1076,17 @@
 |                | ShutterCloseDuration<x\>    | *ShutterOpen<x\>*      |             |
 |                | ShutterEnableEndStopTime<x\>| *ShutterSetClose<x\>*  |             |
 |                | ShutterInvert<x\>           | *ShutterStop<x\>*      |             |
 |                | ShutterInvertWebButtons<x\> | *ShutterStopClose<x\>* |             |
 |                | ShutterLock<x\>             | *ShutterStopOpen<x\>*  |             |
 |                | ShutterMode<x\>             | *ShutterStopPosition<x\>*|           |
 |                | ShutterMotorDelay<x\>       | *ShutterStopToggle<x\>*|             |
-|                | ShutterMotorStop            | *ShutterStopToggleDir<x\>*|          |
-|                | ShutterOpenDuration<x\>     | *ShutterToggle<x\>*    |             |
-|                | ShutterPosition<x\>         | *ShutterToggleDir<x\>* |             |
-|                | ShutterPWMRange<x\>         |                        |             |
+|                | ShutterOpenDuration<x\>     | *ShutterStopToggleDir<x\>*|          |
+|                | ShutterPosition<x\>         | *ShutterToggle<x\>*    |             |
+|                | ShutterPWMRange<x\>         | *ShutterToggleDir<x\>* |             |
 |                | ShutterRelay<x\>            |                        |             |
 |                | ShutterSetHalfway<x\>       |                        |             |
 |                | ShutterTiltConfig<x\>       |                        |             |
 | **Telegram**   | TmChatId                    | *TmPoll*               |             |
 |                | TmState                     | *TmSend*               |             |
 |                | TmToken                     |                        |             |
 | **Zigbee**     | ZbConfig                    | *ZbBind*               |             |
@@ -1281,14 +1153,13 @@
 
 * **21** = internal error:  
 An unexpected internal error occured  
 
 * **22** = HTTP connection error:  
 Source device HTTP connection lost or unavailable  
 
-* **23** = MQTT connection error:  
-MQTT server connection error  
-
-* **24...** = python library exit code:  
+* **23...** = python library exit code:  
 An unexpected internal library error occured  
 
 * **4xx**/**5xx** = HTTP errors  
+
+
```

### Comparing `decode-config-13.0.0.0/README.md` & `decode-config-2022.1/decode_config.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,36 @@
+Metadata-Version: 2.1
+Name: decode-config
+Version: 2022.1
+Summary: Backup/restore and decode configuration tool for Tasmota
+Home-page: https://github.com/tasmota/decode-config
+Author: Norbert Richter
+Author-email: nr@prsolution.eu
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Utilities
+Classifier: Environment :: Console
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # decode-config
 
 Convert, backup and restore configuration data of devices flashed with [Tasmota firmware](https://github.com/arendst/Tasmota).
 
 <!-- markdownlint-disable MD033 -->
-<img src="https://github.com/tasmota/decode-config/blob/master/media/pic/decode-config.png" alt="Overview" title="decode-config Overview" width="600">
+<img src="https://github.com/curzon01/media/blob/master/pics/decode-config_overview.png" alt="Overview" title="decode-config Overview" width="600">
 
 <!-- markdownlint-disable MD033 -->
-[![master](https://img.shields.io/badge/master-v13.0.0.0-blue.svg)](https://github.com/tasmota/decode-config/tree/master)
+[![development](https://img.shields.io/badge/development-v2022.01.2-blue.svg)](https://github.com/tasmota/decode-config/tree/development)
 [![GitHub download](https://img.shields.io/github/downloads/tasmota/decode-config/total.svg)](https://github.com/tasmota/decode-config/releases/latest)
-[![PyPI version](https://badge.fury.io/py/decode-config.svg)](https://badge.fury.io/py/decode-config)
-![PyPI downloads](https://img.shields.io/pypi/dm/decode-config?label=pypi%20downloads)
 [![License](https://img.shields.io/github/license/tasmota/decode-config.svg)](LICENSE)
 
 If you like **decode-config** give it a star or fork it and contribute:
 
 [![GitHub stars](https://img.shields.io/github/stars/tasmota/decode-config.svg?style=social&label=Star)](https://github.com/tasmota/decode-config/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/tasmota/decode-config.svg?style=social&label=Fork)](https://github.com/tasmota/decode-config/network)
 [![donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://paypal.me/NorbertRichterDE)
@@ -32,229 +49,205 @@
 |:------------------------|:-----------------------:|:------------------:|
 | encrypted               |           No            |         Yes        |
 | readable                |           Yes           |         No         |
 | editable                |           Yes           |         No         |
 | batch processing        |           Yes           |         No         |
 | Backup/Restore subsets  |           Yes           |         No         |
 
-**decode-config** is compatible with all [Tasmota](https://github.com/arendst/Tasmota) versions, starting from Tasmota v5.10.0 up to the current one.
-
-## Development
+**decode-config** is compatible with [Tasmota](https://github.com/arendst/Tasmota) starting from v5.10.0 up to now.
 
-Using the latest development version of decode-config is only necessary if you also use the latest development version of Tasmota.
+## Content
 
-<!-- markdownlint-disable MD033 -->
-[![development version](https://img.shields.io/badge/development-v13.0.0.0-blue.svg)](https://github.com/tasmota/decode-config/tree/development)
+**This is the developer branch which contains decode-config matching the latest Tasmota developer version.**
 
-## Table of contents
+This branch does not contain any binaries. If you want to use a precompiled **decode-config** binary
+you can use binaries from latest [Release](https://github.com/tasmota/decode-config/releases).
 
-* [Development](#development)
-* [Table of contents](#table-of-contents)
-* [Running the program](#running-the-program)
-  * [Installation](#installation)
-* [Usage](#usage)
-  * [Basics](#basics)
-  * [Tasmota source](#tasmota-source)
-  * [Format JSON output](#format-json-output)
-  * [Parameter file](#parameter-file)
-  * [Save backup](#save-backup)
-  * [Restore backup](#restore-backup)
-  * [Auto file extensions](#auto-file-extensions)
-  * [Test your parameter](#test-your-parameter)
-  * [Console outputs](#console-outputs)
-  * [Filter by groups](#filter-by-groups)
-* [Usage examples](#usage-examples)
-  * [Using Tasmota binary configuration files](#using-tasmota-binary-configuration-files)
-  * [Using JSON editable file](#using-json-editable-file)
-  * [Use batch processing](#use-batch-processing)
-* [File Formats](#file-formats)
-  * [.dmp format](#dmp-format)
-  * [.json format](#json-format-1)
-  * [.bin format](#bin-format)
-* [Program parameter list](#program-parameter-list)
-  * [--full-help](#--full-help)
-  * [Parameter notes](#parameter-notes)
-  * [Obsolete parameters](#obsolete-parameters)
-* [Generated Tasmota commands](#generated-tasmota-commands)
-* [Program return codes](#program-return-codes)
+> **Note**  
+If you want to run the development **decode-config.py** from this branch, you need an
+installed [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) environment.
+See [Running as Python script](#running-as-python-script) for more details.
+
+### Files
+
+| File                     | Description |
+|:-------------------------|:------------------------------------------------------------------------|
+| `build`                  | contains files to build executables                                     |
+| `decode-config.py`       | Python source file running under your local Python environment          |
+| `README.md`              | This content                                                            |
+
+### Table of contents
+
+* [decode-config](#decode-config)
+  * [Content](#content)
+    * [Files](#files)
+    * [Table of contents](#table-of-contents)
+  * [Running the program](#running-the-program)
+    * [Prerequisite](#prerequisite)
+  * [Usage](#usage)
+    * [Basics](#basics)
+    * [Format JSON output](#format-json-output)
+    * [Parameter file](#parameter-file)
+    * [Save backup](#save-backup)
+    * [Restore backup](#restore-backup)
+    * [Auto file extensions](#auto-file-extensions)
+    * [Test your parameter](#test-your-parameter)
+    * [Console outputs](#console-outputs)
+    * [Filter by groups](#filter-by-groups)
+    * [Usage examples](#usage-examples)
+  * [File Formats](#file-formats)
+    * [.dmp format](#dmp-format)
+    * [.json format](#json-format)
+    * [.bin format](#bin-format)
+  * [Program parameter list](#program-parameter-list)
+    * [--full-help](#--full-help)
+    * [Parameter notes](#parameter-notes)
+    * [Obsolete parameters](#obsolete-parameters)
+  * [Generated Tasmota commands](#generated-tasmota-commands)
+  * [Program return codes](#program-return-codes)
 
 ## Running the program
 
-To use **decode-config.py** you can install it using Python environment and following the [Installation](#installation) section below.
-
-Alternatively you can download a ready-made binary from [Releases](https://github.com/tasmota/decode-config/releases) to use it without installing Python.
-
-### Installation
-
-**decode-config.py** needs an installed [Python](https://en.wikipedia.org/wiki/Python_%28programming_language%29) environment - (see [Prerequisite](#prerequisite)).
-
-After you have installed your Python environment, there are two ways to install deocde-config:
-
-#### Installation using PyPi
-
-```shell
-pip install decode-config
-```
+The program does not have a graphical user interface (GUI), you have to run it from your OS command line using [program arguments](#usage).
 
-The program does not have a graphical user interface (GUI), you have to run it from your OS command line using [program arguments](#usage) - see [Usage](#usage) for more details.
+### Prerequisite
 
-#### Manual installation
+#### Tasmota WebServer
 
-This is only necessary if you want to run **decode-config.py** from [development branch](https://github.com/tasmota/decode-config/tree/development). First install the required modules manually
+[Tasmota](https://github.com/arendst/Tasmota) provides its configuration data by http request only. To receive and send configuration data from Tasmota devices directly the http WebServer in Tasmota must be enabled:
 
-```shell
-python -m pip install -r requirements.txt
-```
+* enable web-server admin mode (Tasmota web command [WebServer 2](https://tasmota.github.io/docs/Commands/#webserver))
+* for self-compiled firmware enable web-server with (`#define USE_WEBSERVER` and `#define WEB_SERVER 2`).
 
-After that you can use the Phython script **decode-config.py** as normal program:
+> **Note**  
+Using MQTT for exchanging Tasmota configuration data is supported by Tasmota since v9.4.0.3; **decode-config** will be able using MQTT in future supporting configuration data exchange this way too.
 
-```shell
-decode-config.py
-```
+#### Python
 
-#### Prerequisite
+**decode-config.py** needs an installed [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) environment.
 
-Since **decode-config.py** is a Python program, it requires an installed [Python](https://en.wikipedia.org/wiki/Python_%28programming_language%29) environment.
+> **Note**  
+Due to the [Python 2.7 EOL](https://github.com/python/devguide/pull/344) in Jan 2020 Python 2.x is no longer supported.
 
 ##### Linux
 
-Install [Python 3.x](https://www.python.org/downloads/) and Pip:
+Install [Python 3.x](https://www.python.org/downloads/), Pip and follow [library installation for all OS](#all-os) below.
 
 ```bash
 sudo apt-get install python3 python3-pip
 ```
 
-##### Windows
+##### Windows 10
 
-Install [Python 3.x](https://www.python.org/downloads/windows/) as described
+Install [Python 3.x](https://www.python.org/downloads/windows/) as described and follow [library installation for all OS](#all-os) below.
 
 ##### MacOS
 
-Install [Python 3.x](https://www.python.org/downloads/mac-osx/) as described
+Install [Python 3.x](https://www.python.org/downloads/mac-osx/) as described and follow [library installation for all OS](#all-os) below.
+
+##### All OS
+
+After python and pip is installed, install dependencies:
+
+```shell
+python -m pip install requests configargparse
+```
 
 ## Usage
 
 For an overview start the program without any parameter and you will get a short help:
 
 <!-- markdownlint-capture -->
 <!-- markdownlint-disable MD031 -->
 ```bash
-decode-config.py
+decode-config
 ```
+> **Note**  
+Replace `decode-config` by the program name your are using:  
+`decode-config.py` when running as Python executable.
+<!-- markdownlint-restore -->
 
 This prints a short help:
 
 ```help
-usage: decode-config.py [-s <filename|host|url>] [-p <password>]
-                        [--fulltopic <topic>] [--cafile <file>]
-                        [--certfile <file>] [--keyfile <file>] [--insecure]
-                        [--keepalive <sec>] [-i <restorefile>]
+usage: decode-config.py [-s <filename|host|url>] [-i <restorefile>]
                         [-o <backupfile>] [-t json|bin|dmp] [-E] [-e] [-F]
                         [--json-indent <indent>] [--json-compact]
                         [--json-show-pw] [--cmnd-indent <indent>]
-                        [--cmnd-groups] [--cmnd-sort]
-                        [--cmnd-use-rule-concat] [--cmnd-use-backlog]
-                        [-c <configfile>] [-S] [-T json|cmnd|command]
+                        [--cmnd-groups] [--cmnd-sort] [--cmnd-use-rule-concat]
+                        [--cmnd-use-backlog] [-c <configfile>] [-S]
+                        [-T json|cmnd|command]
                         [-g <groupname> [<groupname> ...]] [-w] [--dry-run]
                         [-h] [-H] [-v] [-V]
 ```
 
 For advanced help run **decode-config** with parameter `--full--help` or `-H`. This will print a [Program parameter list](#program-parameter-list).
 
 > **Note**  
-If you're missing older parameters, don't worry, they're still there (see [Obsolete parameters](#obsolete-parameters)).
+If you miss parameters here that are already in use, don't worry, they are still there.  
+For details see [Obsolete parameters](#obsolete-parameters)
 
 ### Basics
 
-To get a program result, pass at least a [Tasmota source](#tasmota-source) from which you want to read the configuration data.
-
-### Tasmota source
-
-The Tasmota source determines where the configuration data should be loaded from and saved to.
-A source can be an offline file or an online Tasmota device accessed via HTTP or indirectly via MQTT.
-
-Use `--source` parameter to determine the configuration data source:
-
-#### Binary (*.dmp) file (Offline)
+To get a result, at least pass a Tasmota source where you want to read the configuration from.
 
-Source is a Tasmota configuration file (having extension `.dmp`).
+Source can be either
 
-Pass the filename direclty or encoded as a [file-URL](https://en.wikipedia.org/wiki/URL):
+* a device hostname, IP or [http-url](https://en.wikipedia.org/wiki/URL) available and online within your network:  
+use `--source <host|url>` or `-s <host|url>` parameter
+* a Tasmota configuration file (having extension `.dmp`):  
+use `--source <filename>` or `-s <filename>` parameter
 
-```bash
-decode-config --source tasmota-4281.dmp
-decode-config -s file://path/to/tasmota-4281.dmp
-```
+The [http-url](https://en.wikipedia.org/wiki/URL) variant also allows `<user>`, `<password>` and `<port>` number to be specified:
 
-#### HTTP connection (Online)
+* `--source http://admin:myPaszxwo!z@tasmota-4281`
+* `--source http://tasmota-4281:80`
+* `--source http://admin:myPaszxwo!z@tasmota-4281:80`
 
-Source is an online HTTP connection to a running Tasmota device. To use this source, **decode-config** must have access to the network on which Tasmota is running, [Tasmota Webserver](https://tasmota.github.io/docs/Commands/#webserver) running in admin mode (`WebServer 2`) is mandatory.
+#### Basic example
 
-Specify the hostname, IP o or [http-url](https://en.wikipedia.org/wiki/URL) of the Tasmota device.
-
-An optionally required HTTP password, username and different HTTP port of the device can be specified via [URL](https://en.wikipedia.org/wiki/URL) or separately via `--username`, `--password` and `--port`
+##### Access an online device
 
 ```bash
 decode-config --source tasmota-4281
 decode-config -s 192.168.10.92
-decode-config --source http://tasmota-4281 --password myPaszxwo!z
-decode-config --source http://admin:myPaszxwo!z@tasmota-4281:8000
-decode-config --source http://admin:myPaszxwo!z@tasmota-4281/cs?
+decode-config --source http://tasmota-4281
+decode-config --source http://admin:myPaszxwo!z@tasmota-4281
 ```
 
-An appended HTTP path (here "`/cs?`") is ignored.
-
-#### MQTT transission (Online)
+##### Access a config file
 
-Source is a MQTT server and topic where an online Tasmota device is connected to. To use this source, **decode-config** does not need to have access to the same network that Tasmota is running on, it just needs access to the MQTT server that Tasmota also uses.
+```bash
+decode-config --source tasmota-4281.dmp
+decode-config -s tasmota-4281.dmp
+```
 
-##### MQTT connection parameter
+will output a readable configuration in [JSON](http://www.json.org/)-format, e.g.:
 
-Specify the hostname or IP of the MQTT server (possibly also specify username and password for the MQTT server) and the Tasmota MQTT topic. The **decode-config** connection to MQTT server also allows SSL/TLS connection.
+```json
+{"altitude": 112, "baudrate": 115200, "blinkcount": 10, "blinktime": 10,...
+"ws_width": [1, 3, 5]}
+```
 
-The MQTT username and password must be encoded within the URL (the parameter `--password` can not be used for that, it has a different function here).  
-If the username/password combination for the **decode-config** MQTT connection is different from the one used by Tasmota itself (Tasmota command `MQTTPassword`), the Tasmota MQTT password must be specified via the `--password` parameter.
+> **Note**  
+The json names (like `"altitude"` or `"blinktime"` are internal names from Tasmotas [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/settings.h) STRUCT `Settings` and are not the same as known from Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/). However, since most variable names are self-describing, the functional meaning should be given in most cases.
 
-The Tasmota topic can be specfied either within the [URL path](https://en.wikipedia.org/wiki/URL#Syntax) component or using optional `--fulltopic` parameter.  
-The topic must be the full topic of the Tasmota device without any trailing command or result part. You can use any of the prefixed topic (*cmnd*, *stat* or *tele* topic) or use the placeholder *%prefix%* for it, example  
-`%prefix%/tasmota-4281` or `tele/tasmota-4281` are valid topics  
-`cmnd/tasmota-4281/POWER` or `tele/tasmota-4281/STATE` are invalid topics due to the trailing part.
+#### Password protected device
 
-For SSL/TLS connection to MQTT server use `mqtts://` [URL scheme](https://en.wikipedia.org/wiki/URL#Syntax).
+If you try to access data from a device and you get an error like `ERROR 401: Error on http GET request for http://.../dl - Unauthorized` you need to pass your WebPassword for this device:
 
 ```bash
-decode-config --source mqtts://mybroker.example.com/%prefx%/tasmota-4281
-decode-config --source mqtts://mybroker.example.com:8883/tele/tasmota-4281
-decode-config --source mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com  --fulltopic tele/tasmota-4281
-decode-config --source mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota-4281 --password myTasmotaMQTTPaszxwo!z
+decode-config --source tasmota-4281 --password "myPaszxwo!z"
 ```
 
-For own certifications use the parameters `--cafile`, `--certfile` and `--keyfile`. To suppress certification verification use `--insecure`.
-
-For none SSL/TLS connection to MQTT server use `mqtt://` [URL scheme](https://en.wikipedia.org/wiki/URL#Syntax).
-
-```bash
-decode-config --source mqtt://mybroker.example.com/%prefx%/tasmota-4281
-decode-config --source mqtt://mybroker.example.com:1883/tele/tasmota-4281
-decode-config --source mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com  --fulltopic tele/tasmota-4281
-decode-config --source mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota-4281 --password myTasmotaMQTTPaszxwo!z
-```
+> **Hint**  
+*decode-config* username default is `admin`. For self-compiled binaries using a non-standard web username, use `-u <user>` or `--username <user>`.
 
 ### Format JSON output
 
-All basic examples above will output a readable configuration in [JSON](http://www.json.org/)-format, e.g.:
-
-```json
-{"altitude": 112, "baudrate": 115200, "blinkcount": 10, "blinktime": 10,...
-"ws_width": [1, 3, 5]}
-```
-
-> **Note**  
-The json names (like `"altitude"` or `"blinktime"` are internal names from Tasmotas [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/include/tasmota_types.h) STRUCT `Settings` and are not the same as known from Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/). However, since most variable names are self-describing, the functional meaning should be given in most cases.
-
 The default JSON output can be formatted for better reading using the `--json-indent <n>` parameter:
 
 ```bash
 decode-config --source tasmota-4281 --password "myPaszxwo!z" --json-indent 2
 ```
 
 This will print a pretty better readable format and the example above becomes:
@@ -312,56 +305,52 @@
 
 ### Save backup
 
 To save data from a device or [*.dmp](#dmp-format) file into a backup file, use `--backup-file <filename>`.
 
 #### Backup filename macros
 
-You can use the following placeholders within filenames:
+You can use the following placeholders within backup/restore filenames:
 
-* **@v** is replaced by *Tasmota Version* (backup & restore filenames)
-* **@d** is replaced by *Devicename* (backup & restore filenames)
-* **@f** is replaced by first *Friendlyname1* (backup & restore filenames)
-* **@h** is replaced by the *Hostname* from configuration data (backup & restore filenames)  
-Note: This is the static hostname which is configured by the command *Hostname*, for real hostname from a device use macro the **@H**)
-* **@H** is replaced by the live device hostname  (only for http sources, backup & restore filenames)  
-Note: This can be different to the configured hostname as this can contain also macros).source
-* **@F** is replaced by the filename of MQTT request (only for MQTT sources, backup filenames only).  
-This is usually the filename that Tasmota uses when saving the configuration in the WebUI.
+* **@v** is replaced by _Tasmota Version_
+* **@d** is replaced by _Devicename_
+* **@f** is replaced by first _Friendlyname1_
+* **@h** is replaced by the __Hostname__ from configuration data (note: this is the static hostname which is configured by the command __Hostname__, for real hostname from a device use macro the **@H**)
+* **@H** is replaced by the live device hostname note: this can be different to the configured hostname as this can contain also macros). Only valid when using real devices as source
 
 Example:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 --backup-file Config_@d_@v
 ```
 
-This will create a file like `Config_Tasmota_13.0.json` (the part `Tasmota` and `13.0` will choosen related to your device configuration).
+This will create a file like `Config_Tasmota_10.1.0.json` (the part `Tasmota` and `10.1.0` will choosen related to your device configuration).
 
 #### Save multiple backup at once
 
-The `--backup-file` parameter can be specified multiple times to create different backup with different names and/or different formats at once:
+Since **decode-config** v8.2.0.5 the `--backup-file` parameter can be specified multiple times. With that it's easy to create different backup with different names and/or different formats at once:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 -o Config_@d_@v -o Backup_@H.json -o Backup_@H.dmp
 ```
 
 creates three backup files:
 
-* `Config_Tasmota_13.0.json` using JSON format
+* `Config_Tasmota_10.1.0.json` using JSON format
 * `Backup_tasmota-4281.json` using JSON format
 * `Backup_tasmota-4281.dmp` using Tasmota configuration file format
 
 ### Restore backup
 
 Reading back a previously saved backup file, use the `--restore-file <filename>` parameter.
 
-To restore the previously save backup file `Config_Tasmota_13.0.json` to device `tasmota-4281` use:
+To restore the previously save backup file `Config_Tasmota_10.1.0.json` to device `tasmota-4281` use:
 
 ```bash
-decode-config -c my.conf -s tasmota-4281 --restore-file Config_Tasmota_13.0
+decode-config -c my.conf -s tasmota-4281 --restore-file Config_Tasmota_10.1.0
 ```
 
 Restore operation also allows placeholders **@v**, **@d**, **@f**, **@h** or **@H** like in backup filenames so we can use the same naming as for the backup process:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 --restore-file Config_@d_@v
 ```
@@ -439,17 +428,17 @@
 ### Console outputs
 
 Output to the console screen is the default when calling the program without any backup or restore parameter.  
 Screen output is suppressed when using backup or restore parameter. In that case you can force screen output with `--output`.
 
 The console screen output supports two formats:
 
-* [JSON](#json-format):<br>
+* [JSON](#console-json-format):<br>
 This is identical with the backup/restore [json file Format](#json-format) but printed on screen standard output.
-* [Tasmota command](#tasmota-web-command-format):<br>
+* [Tasmota command](#console-tasmota-command-format):<br>
 This outputs the most (but not all!) configuration data as Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/).
 
 #### JSON format
 
 The default console output format is [JSON](#json-format) (optional you can force JSON backup format using `--output-format json`).
 
 Example:
@@ -598,76 +587,39 @@
 
 ```bash
 decode-config -s tasmota-4281 -c my.conf --output-format cmnd --group Main MQTT Management Wifi
 ```
 
 Filtering by groups affects the entire output, regardless of whether screen output or backup file.
 
-## Usage examples
-
-### Using Tasmota binary configuration files
-
-These examples use an online Tasmota device accessed over HTTP. The hostname of the Tasmota device is `tasmota-2f5d44-4281`
-
-#### Backup an online Tasmota device via HTTP into a Tasmota configuration file
-
-##### Use args to choice the file format
+### Usage examples
 
-```bash
-  decode-config -c my.conf -s tasmota-2f5d44-4281 --backup-type dmp --backup-file Config_@d_@v
-```
-
-##### Use file extension to choice the file format
-
-```bash
-decode-config -c my.conf -s tasmota-2f5d44-4281 --backup-file Config_@d_@v.dmp
-```
+#### Using Tasmota binary configuration files
 
-#### Restore a Tasmota configuration file to an online Tasmota device via HTTP
+1. Restore a Tasmota configuration file
 
-```bash
-decode-config -c my.conf -s http://tasmota-2f5d44-4281 --restore-file Config_@d_@v.dmp
-```
-
-### Using JSON editable file
+  ```bash
+  decode-config -c my.conf -s tasmota --restore-file Config_Tasmota_6.2.1.dmp
+  ```
 
-These examples use an online Tasmota device that is accessed indirectly via MQTT.
+1. Backup device using Tasmota configuration compatible format
 
-In these examples, the MQTT server parameters are the same as those used by Tasmota itself:
+   a) use file extension to choice the file format
 
-* MQTT Server: `mybroker.example.com`
-* MQTT Username: `mqttuser`
-* MQTT Password: `myBrokerPaszxwo!z`
-* Tasmota topic: `tele/tasmota_2F5D44`
+  ```bash
+  decode-config -c my.conf -s tasmota --backup-file Config_@d_@v.dmp
+  ```
 
-#### Backup an online Tasmota device via MQTT into a JSON file
+   b) use args to choice the file format
 
-##### Use an unencrypted MQTT connection
+  ```bash
+    decode-config -c my.conf -s tasmota --backup-type dmp --backup-file Config_@d_@v
+  ```
 
-MQTT server uses a non default port 42110
-
-```bash
-decode-config -s mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com:42110/tele/tasmota_2F5D44 --backup-file Config_2f5d44-4281.json
-```
-
-##### Use SSL/TLS MQTT connection
-
-Limit the configuration data to the groups `Control`, `Management` and `SetOption`
-
-```bash
-decode-config -s mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com --fulltopic tele/tasmota_2F5D44 --backup-file Config_2f5d44-4281.json -g Control Management SetOption
-```
-
-#### Restore a JSON file to an online Tasmota device via MQTT
-
-```bash
-decode-config -s mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota_2F5D44 --restore-file Config_2f5d44-4281.json
-```
-
-### Use batch processing
+#### Use batch processing
 
 Linux
 
 ```bash
 for device in tasmota1 tasmota2 tasmota3; do ./decode-config -c my.conf -s $device -o Config_@d_@v
 ```
 
@@ -691,18 +643,18 @@
 
 ### .json format
 
 This format uses the [JSON](http://www.json.org/) notation and contains the complete configuration data in plain text, human readable and editable.
 
 The .json format can be created by **decode-config** using the backup function (`--backup-file <filename>`) (for better identification you can append the optional parameter `--backup-type json`, but that's optional as json is the default backup format).
 
-In contrast to the other two binary formats [.dmp](#dmp-format) and [.bin](#bin-format), this type of format also allows the [partial modification](#restore-subset-of-data) of configurations.
+In contrast to the other two binary formats [.dmp](#dmp-format) and [.bin](#bin-format), this type of format also allows the [partial modification](#restore-a-subset-of-backup-data) of configurations.
 
 > **Note**  
-The keys used within the JSON file are based on the variable names of Tasmota source code in [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/include/tasmota_types.h) so they do not have the same naming as known for Tasmota web commands. However, since the variable names are self-explanatory, there should be no difficulties in assigning the functionality of the variables.
+The keys used within the JSON file are based on the variable names of Tasmota source code in [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/settings.h) so they do not have the same naming as known for Tasmota web commands. However, since the variable names are self-explanatory, there should be no difficulties in assigning the functionality of the variables.
 
 ### .bin format
 
 This format is binary with the same structure as the [.dmp](#dmp-format) format. The differences to .dmp are:
 
 * .bin is decrypted
 * .bin has 4 additional bytes at the end of the file
@@ -720,84 +672,58 @@
 A short list of possible program args is displayed using `-h` or `--help`.
 
 ### --full-help
 
 For advanced help use parameter `-H` or `--full-help`:
 
 ```help
-usage: decode-config.py [-s <filename|host|url>] [-p <password>]
-                        [--fulltopic <topic>] [--cafile <file>]
-                        [--certfile <file>] [--keyfile <file>] [--insecure]
-                        [--keepalive <sec>] [-i <restorefile>]
+usage: decode-config.py [-s <filename|host|url>] [-i <restorefile>]
                         [-o <backupfile>] [-t json|bin|dmp] [-E] [-e] [-F]
                         [--json-indent <indent>] [--json-compact]
                         [--json-show-pw] [--cmnd-indent <indent>]
-                        [--cmnd-groups] [--cmnd-sort]
-                        [--cmnd-use-rule-concat] [--cmnd-use-backlog]
-                        [-c <configfile>] [-S] [-T json|cmnd|command]
+                        [--cmnd-groups] [--cmnd-sort] [--cmnd-use-rule-concat]
+                        [--cmnd-use-backlog] [-c <configfile>] [-S]
+                        [-T json|cmnd|command]
                         [-g <groupname> [<groupname> ...]] [-w] [--dry-run]
                         [-h] [-H] [-v] [-V]
 
-Backup/Restore Tasmota configuration data. Args that start with '--' (eg.
--s) can also be set in a config file (specified via -c). Config file syntax
+Backup/Restore Tasmota configuration data. Args that start with '--' (eg. -s)
+can also be set in a config file (specified via -c). Config file syntax
 allows: key=value, flag=true, stuff=[a,b,c] (for details, see syntax at
 https://goo.gl/R74nmi). If an arg is specified in more than one place, then
 commandline values override config file values which override defaults.
 
 Source:
   Read/Write Tasmota configuration from/to
 
   -s, --source <filename|host|url>
                         source used for the Tasmota configuration (default:
-                        None). Specify source type, path, file, user,
-                        password, hostname, port and topic at once as an
-                        URL. The URL must be in the form 'scheme://[username
-                        [:password]@]host[:port][/topic]|pathfile'where
-                        scheme is 'file' for a tasmota binary config file,
-                        'http' for a Tasmota HTTP web connection and
-                        'mqtt(s)' for Tasmota MQTT transport ('mqtts' uses a
-                        TLS connection to MQTT server)
-  -p, --password <password>
-                        Web server password on HTTP source (set by Tasmota
-                        'WebPassword' command), MQTT server password in MQTT
-                        source (set by Tasmota 'MqttPassword' command)
-                        (default: None)
-
-MQTT:
-  MQTT transport settings
-
-  --fulltopic <topic>   Optional MQTT transport fulltopic used for accessing
-                        Tasmota device (default: )
-  --cafile <file>       Enables SSL/TLS connection: path to a or filename of
-                        the Certificate Authority certificate files that are
-                        to be treated as trusted by this client (default
-                        None)
-  --certfile <file>     Enables SSL/TLS connection: filename of a PEM
-                        encoded client certificate file (default None)
-  --keyfile <file>      Enables SSL/TLS connection: filename of a PEM
-                        encoded client private key file (default None)
-  --insecure            suppress verification of the MQTT server hostname in
-                        the server certificate (default False)
-  --keepalive <sec>     keepalive timeout for the client (default 60)
+                        None). The argument can be a <filename> containing
+                        Tasmota .dmp configuation data or a <hostname>,
+                        <ip>-address, <url> which means an online tasmota
+                        device is used. A url can also contain web login and
+                        port data in the format
+                        http://<user>:<password>@tasmota:<port>, e. g,
+                        http://admin:mypw@mytasmota:8090
 
 Backup/Restore:
   Backup & restore specification
 
   -i, --restore-file <restorefile>
                         file to restore configuration from (default: None).
                         Replacements: @v=firmware version from config,
                         @d=devicename, @f=friendlyname1, @h=hostname from
-                        config, @H=device hostname (http source only)
+                        config, @H=device hostname (invalid if using a file as
+                        source)
   -o, --backup-file <backupfile>
                         file to backup configuration to, can be specified
                         multiple times (default: None). Replacements:
                         @v=firmware version from config, @d=devicename,
                         @f=friendlyname1, @h=hostname from config, @H=device
-                        hostname (http source only), @F=configuration
-                        filename from MQTT request (mqtt source only)
+                        hostname (invalid if using a file as source)
   -t, --backup-type json|bin|dmp
                         backup filetype (default: 'json')
   -E, --extension       append filetype extension for -i and -o filename
                         (default)
   -e, --no-extension    do not append filetype extension, use -i and -o
                         filename as passed
   -F, --force-restore   force restore even configuration is identical
@@ -813,23 +739,22 @@
   --json-show-pw        unhide passwords (default)
 
 Tasmota command output:
   Tasmota command output format specification. To revert an option, insert
   "dont" or "no" after "cmnd", e.g. --cmnd-no-indent, --cmnd-dont-sort
 
   --cmnd-indent <indent>
-                        Tasmota command grouping indent level (default:
-                        '2'). 0 disables indent
+                        Tasmota command grouping indent level (default: '2').
+                        0 disables indent
   --cmnd-groups         group Tasmota commands (default)
   --cmnd-sort           sort Tasmota commands (default)
   --cmnd-use-rule-concat
                         use rule concatenation with + for Tasmota 'Rule'
                         command
-  --cmnd-use-backlog    use 'Backlog' for Tasmota commands as much as
-                        possible
+  --cmnd-use-backlog    use 'Backlog' for Tasmota commands as much as possible
 
 Common:
   Optional arguments
 
   -c, --config <configfile>
                         program config file - can be used to set default
                         command parameters (default: None)
@@ -837,16 +762,16 @@
                         (default do not output on backup or restore usage)
   -T, --output-format json|cmnd|command
                         display output format (default: 'json')
   -g, --group <groupname>
                         limit data processing to command groups (default no
                         filter)
   -w, --ignore-warnings
-                        do not exit on warnings. Not recommended, used by
-                        your own responsibility!
+                        do not exit on warnings. Not recommended, used by your
+                        own responsibility!
   --dry-run             test program without changing configuration data on
                         device or file
 
 Info:
   Extra information
 
   -h, --help            show usage help message and exit
@@ -862,15 +787,15 @@
 For details see [Obsolete parameters](#obsolete-parameters)
 
 ### Parameter notes
 
 * Filename replacement macros **@h** and **@H**:
   * **@h**
 The **@h** replacement macro uses the hostname configured with the Tasomta Wifi `Hostname <host>` command (defaults to `%s-%04d`). It will not use the network hostname of your device because this is not available when working with files only (e.g. `--source <filename>` as source).
-To prevent having an useless % in your filename, **@h** will not replaced by hostname if this contains '%' characters.
+To prevent having a useless % in your filename, **@h** will not replaced by hostname if this contains '%' characters.
   * **@H**
 If you want to use the network hostname within your filename, use the **@H** replacement macro instead - but be aware this will only replaced if you are using a network device as source (`<hostname>`, `<ip>`, `<url>`); it will not work when using a file as source (`<filename>`)
 
 ### Obsolete parameters
 
 The parameters listed here continue to work and are supported, but are no longer listed in the parameter list:
 
@@ -882,14 +807,16 @@
 file used for the Tasmota configuration (default: None)'
 * `-d`, `--device`, `--host` `<host|url>`  
 hostname, IP-address or url used for the Tasmota configuration (default: None)
 * `-P`, `--port` `<port>`  
 TCP/IP port number to use for the host connection (default: 80)
 * `-u`, `--username` `<username>`  
 host HTTP access username (default: admin)
+* `-p`, `--password` `<password>`  
+host HTTP access password (default: None)
 
 #### Obsolete JSON formating parameters
 
 * `--json-unhide-pw` same as `--json-show-pw`
 * `--json-hide-pw` same as `--json-dont-show-pw`
 * `--json-sort` sorts JSON output (this is the default)
 * `--json-unsort` prevents JSON sorting
@@ -921,94 +848,64 @@
 |                | LedState                    |                        |             |
 |                | Power<x\>                   |                        |             |
 |                | PowerOnState                |                        |             |
 |                | PulseTime<x\>               |                        |             |
 |                | SwitchDebounce              |                        |             |
 |                | SwitchMode<x\>              |                        |             |
 |                | Webbutton<x\>               |                        |             |
-|                | WCAEC<sup>2</sup>           |                        |             |
-|                | WCAECDSP<sup>2</sup>        |                        |             |
-|                | WCAECValue<sup>2</sup>      |                        |             |
-|                | WCAELevel<sup>2</sup>       |                        |             |
-|                | WCAGCGain<sup>2</sup>       |                        |             |
-|                | WCAWB<sup>2</sup>           |                        |             |
-|                | WCAWBGain<sup>2</sup>       |                        |             |
-|                | WCBPC<sup>2</sup>           |                        |             |
-|                | WCBrightness<sup>2</sup>    |                        |             |
-|                | WCClock<sup>2</sup>         |                        |             |
-|                | WCColorbar<sup>2</sup>      |                        |             |
-|                | WCContrast<sup>2</sup>      |                        |             |
-|                | WCDCW<sup>2</sup>           |                        |             |
-|                | WCFeature<sup>2</sup>       |                        |             |
-|                | WCFlip<sup>2</sup>          |                        |             |
-|                | WCGainCeiling<sup>2</sup>   |                        |             |
-|                | WCGammaCorrect<sup>2</sup>  |                        |             |
-|                | WCLensCorrect<sup>2</sup>   |                        |             |
+|                | WCStream<sup>2</sup>        |                        |             |
 |                | WCMirror<sup>2</sup>        |                        |             |
-|                | WCResolution<sup>2</sup>    |                        |             |
+|                | WCFlip<sup>2</sup>          |                        |             |
 |                | WCRtsp<sup>2</sup>          |                        |             |
-|                | WCSAuth<sup>2</sup>         |                        |             |
+|                | WCBrightness<sup>2</sup>    |                        |             |
+|                | WCContrast<sup>2</sup>      |                        |             |
 |                | WCSaturation<sup>2</sup>    |                        |             |
-|                | WCSpecialEffect<sup>2</sup> |                        |             |
-|                | WCStream<sup>2</sup>        |                        |             |
-|                | WCWBMode<sup>2</sup>        |                        |             |
-|                | WCWPC<sup>2</sup>           |                        |             |
+|                | WCResolution<sup>2</sup>    |                        |             |
 | **Management** | DeepSleepTime               | *Delay*                |             |
 |                | DeviceName                  | *Gpios*                |             |
 |                | Emulation                   | *I2Cscan*              |             |
 |                | FriendlyName<x\>            | *Modules*              |             |
 |                | Gpio<x\>                    | *Reset*                |             |
 |                | I2CDriver<x\>               | *Restart*              |             |
 |                | Ifx                         | *State*                |             |
 |                | IfxBucket                   | *Status*               |             |
 |                | IfxHost                     | *Upgrade*              |             |
 |                | IfxPassword                 | *Upload*               |             |
 |                | IfxPort                     | *SSPMLog<sup>2</sup>*  |             |
 |                | IfxUser                     | *SSPEnergy<sup>2</sup>*|             |
-|                | IfxRP                       | *SSPHistory<sup>2</sup>*|            |
-|                | IfxPeriod                   | *SSPScan<sup>2</sup>*  |             |
-|                | IfxSensor                   | *SSPIamHere<sup>2</sup>*|            |
-|                | L1MusicSync                 |                        |             |
-|                | LogHost                     |                        |             |
+|                | IfxPeriod                   | *SSPHistory<sup>2</sup>*|            |
+|                | L1MusicSync                 | *SSPScan<sup>2</sup>*  |             |
+|                | LogHost                     | *SSPIamHere<sup>2</sup>*|            |
 |                | LogPort                     |                        |             |
 |                | Module                      |                        |             |
 |                | Module2                     |                        |             |
 |                | MqttLog                     |                        |             |
 |                | NtpServer<x\>               |                        |             |
 |                | OtaUrl                      |                        |             |
 |                | Pwm<x\>                     |                        |             |
 |                | PwmFrequency                |                        |             |
 |                | PwmRange                    |                        |             |
-|                | RtcNtpserver                |                        |             |
 |                | SaveData                    |                        |             |
 |                | SerialLog                   |                        |             |
 |                | Sleep                       |                        |             |
 |                | SSPMDisplay<sup>2</sup>     |                        |             |
 |                | SysLog                      |                        |             |
 |                | Template                    |                        |             |
 |                | Time                        |                        |             |
 |                | TimeSTD                     |                        |             |
 |                | TimeDST                     |                        |             |
 |                | Timezone                    |                        |             |
-|                | TouchThres<sup>2</sup>      |                        |             |
 |                | TuyaMCU                     |                        |             |
 |                | TuyaTempSetRes              |                        |             |
 |                | WebLog                      |                        |             |
-|                | WebTime                     |                        |             |
 | **WiFi**       | CORS                        | *AP*                   |             |
-|                | DnsTimeout                  | *Ping<x\>*             |             |
-|                | Ethernet<sup>2</sup>        | *WebSend*              |             |
-|                | EthAddress<sup>2</sup>      | *Publish*              |             |
-|                | EthClockMode<sup>2</sup>    | *Publish2*             |             |
-|                | EthType<sup>2</sup>         |                        |             |
-|                | EthIPAddress<sup>2</sup>    |                        |             |
-|                | EthSubnetmask<sup>2</sup>   |                        |             |
-|                | EthGateway<sup>2</sup>      |                        |             |
-|                | EthDNSServer<sup>2</sup>    |                        |             |
-|                | EthDNSServer2<sup>2</sup>   |                        |             |
+|                | Ethernet<sup>2</sup>        | *Ping<x\>*             |             |
+|                | EthAddress<sup>2</sup>      | *WebSend*              |             |
+|                | EthClockMode<sup>2</sup>    | *Publish*              |             |
+|                | EthType<sup>2</sup>         | *Publish2*             |             |
 |                | Hostname                    |                        |             |
 |                | IPAddress<x\>               |                        |             |
 |                | Password<x\>                |                        |             |
 |                | RgxAddress                  |                        |             |
 |                | RgxNAPT                     |                        |             |
 |                | RgxPassword                 |                        |             |
 |                | RgxSsid                     |                        |             |
@@ -1039,15 +936,14 @@
 |                | MqttTimeout                 |                        |             |
 |                | MqttWifiTimeout             |                        |             |
 |                | PowerRetain                 |                        |             |
 |                | Prefix<x\>                  |                        |             |
 |                | SensorRetain                |                        |             |
 |                | StateRetain                 |                        |             |
 |                | StateText<x\>               |                        |             |
-|                | StatusRetain                |                        |             |
 |                | SwitchRetain                |                        |             |
 |                | SwitchTopic                 |                        |             |
 |                | TelePeriod                  |                        |             |
 |                | Topic                       |                        |             |
 | **Rules**      | CalcRes                     | *Add<x\>*              |             |
 |                | Mem<x\>                     | *Event*                |             |
 |                | Rule<x\>                    | *Mult<x\>*             |             |
@@ -1085,28 +981,25 @@
 |                | OT_TWater                   |                        |             |
 |                | Sensor13                    |                        |             |
 |                | Sensor15                    |                        |             |
 |                | Sensor18                    |                        |             |
 |                | Sensor20                    |                        |             |
 |                | Sensor29                    |                        |             |
 |                | Sensor34                    |                        |             |
-|                | Sensor40                    |                        |             |
 |                | Sensor54                    |                        |             |
 |                | Sensor68                    |                        |             |
-|                | Sensor96                    |                        |             |
 |                | Shift595DeviceCount         |                        |             |
 |                | SpeedUnit                   |                        |             |
 |                | TempRes                     |                        |             |
 |                | TempOffset                  |                        |             |
 |                | VoltRes                     |                        |             |
 |                | WattRes                     |                        |             |
 |                | WeightRes                   |                        |             |
-|                | Wiper<x\>                   |                        |             |
 | **Power**      | AmpRes                      | *CurrentSet*           |             |
-|                | CurrentCal                  | *FrequencySet*         |             |
+|                | CurrentCal                  | *FrequencySet*         |`EnergyReset`|
 |                | CurrentHigh                 | *ModuleAddress*        |             |
 |                | CurrentLow                  | *PowerSet*             |             |
 |                | EnergyRes                   | *Status8*              |             |
 |                | EnergyToday                 | *Status9*              |             |
 |                | EnergyTotal                 | *VoltageSet*           |             |
 |                | EnergyYesterday             |                        |             |
 |                | FreqRes                     |                        |             |
@@ -1136,30 +1029,27 @@
 |                | ShdWarmupBrightness         |                        |             |
 |                | ShdWarmupTime               |                        |             |
 |                | Speed                       |                        |             |
 |                | StepPixels                  |                        |             |
 |                | Wakeup                      |                        |             |
 |                | WakeupDuration              |                        |             |
 | **RF**         | RfProtocol                  | *RfRaw*                | `RfCode`    |
-|                | RfTimeOut                   |                        | `RfHigh`    |
+|                |                             |                        | `RfHigh`    |
 |                |                             |                        | `RfHost`    |
 |                |                             |                        | `RfKey<x>`  |
 |                |                             |                        | `RfLow`     |
 |                |                             |                        | `RfSync`    |
 | **IR**         |                             | *IRsend<x\>*           |             |
 |                |                             | *IRhvac*               |             |
 | **SetOption**  | SetOption<x\>               |                        |             |
 | **Serial**     | Baudrate                    | *SerialSend<x\>*       |             |
-|                | ModbusBaudrate              | *SSerialSend<x\>*      |             |
-|                | ModbusSerialConfig          | *TCPStart*             |             |
-|                | SBaudrate                   | *TuyaSend<x\>*         |             |
-|                | SerialConfig                |                        |             |
-|                | SerialDelimiter             |                        |             |
+|                | SBaudrate                   | *SSerialSend<x\>*      |             |
+|                | SerialConfig                | *TCPStart*             |             |
+|                | SerialDelimiter             | *TuyaSend<x\>*         |             |
 |                | SSerialConfig               |                        |             |
-|                | SSerialSend9                |                        |             |
 |                | TCPBaudrate                 |                        |             |
 |                | TCPConfig                   |                        |             |
 | **Domoticz**   | DomoticzIdx<x\>             |                        |             |
 |                | DomoticzKeyIdx<x\>          |                        |             |
 |                | DomoticzSensorIdx<x\>       |                        |             |
 |                | DomoticzSwitchIdx<x\>       |                        |             |
 |                | DomoticzUpdateTimer         |                        |             |
@@ -1186,18 +1076,17 @@
 |                | ShutterCloseDuration<x\>    | *ShutterOpen<x\>*      |             |
 |                | ShutterEnableEndStopTime<x\>| *ShutterSetClose<x\>*  |             |
 |                | ShutterInvert<x\>           | *ShutterStop<x\>*      |             |
 |                | ShutterInvertWebButtons<x\> | *ShutterStopClose<x\>* |             |
 |                | ShutterLock<x\>             | *ShutterStopOpen<x\>*  |             |
 |                | ShutterMode<x\>             | *ShutterStopPosition<x\>*|           |
 |                | ShutterMotorDelay<x\>       | *ShutterStopToggle<x\>*|             |
-|                | ShutterMotorStop            | *ShutterStopToggleDir<x\>*|          |
-|                | ShutterOpenDuration<x\>     | *ShutterToggle<x\>*    |             |
-|                | ShutterPosition<x\>         | *ShutterToggleDir<x\>* |             |
-|                | ShutterPWMRange<x\>         |                        |             |
+|                | ShutterOpenDuration<x\>     | *ShutterStopToggleDir<x\>*|          |
+|                | ShutterPosition<x\>         | *ShutterToggle<x\>*    |             |
+|                | ShutterPWMRange<x\>         | *ShutterToggleDir<x\>* |             |
 |                | ShutterRelay<x\>            |                        |             |
 |                | ShutterSetHalfway<x\>       |                        |             |
 |                | ShutterTiltConfig<x\>       |                        |             |
 | **Telegram**   | TmChatId                    | *TmPoll*               |             |
 |                | TmState                     | *TmSend*               |             |
 |                | TmToken                     |                        |             |
 | **Zigbee**     | ZbConfig                    | *ZbBind*               |             |
@@ -1264,14 +1153,13 @@
 
 * **21** = internal error:  
 An unexpected internal error occured  
 
 * **22** = HTTP connection error:  
 Source device HTTP connection lost or unavailable  
 
-* **23** = MQTT connection error:  
-MQTT server connection error  
-
-* **24...** = python library exit code:  
+* **23...** = python library exit code:  
 An unexpected internal library error occured  
 
 * **4xx**/**5xx** = HTTP errors  
+
+
```

### Comparing `decode-config-13.0.0.0/decode_config.egg-info/PKG-INFO` & `decode-config-2022.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,17 @@
-Metadata-Version: 2.1
-Name: decode-config
-Version: 13.0.0.0
-Summary: Backup/restore and decode configuration tool for Tasmota
-Home-page: https://github.com/tasmota/decode-config
-Author: Norbert Richter
-Author-email: nr@prsolution.eu
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Utilities
-Classifier: Environment :: Console
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # decode-config
 
 Convert, backup and restore configuration data of devices flashed with [Tasmota firmware](https://github.com/arendst/Tasmota).
 
 <!-- markdownlint-disable MD033 -->
-<img src="https://github.com/tasmota/decode-config/blob/master/media/pic/decode-config.png" alt="Overview" title="decode-config Overview" width="600">
+<img src="https://github.com/curzon01/media/blob/master/pics/decode-config_overview.png" alt="Overview" title="decode-config Overview" width="600">
 
 <!-- markdownlint-disable MD033 -->
-[![master](https://img.shields.io/badge/master-v13.0.0.0-blue.svg)](https://github.com/tasmota/decode-config/tree/master)
+[![development](https://img.shields.io/badge/development-v2022.01.2-blue.svg)](https://github.com/tasmota/decode-config/tree/development)
 [![GitHub download](https://img.shields.io/github/downloads/tasmota/decode-config/total.svg)](https://github.com/tasmota/decode-config/releases/latest)
-[![PyPI version](https://badge.fury.io/py/decode-config.svg)](https://badge.fury.io/py/decode-config)
-![PyPI downloads](https://img.shields.io/pypi/dm/decode-config?label=pypi%20downloads)
 [![License](https://img.shields.io/github/license/tasmota/decode-config.svg)](LICENSE)
 
 If you like **decode-config** give it a star or fork it and contribute:
 
 [![GitHub stars](https://img.shields.io/github/stars/tasmota/decode-config.svg?style=social&label=Star)](https://github.com/tasmota/decode-config/stargazers)
 [![GitHub forks](https://img.shields.io/github/forks/tasmota/decode-config.svg?style=social&label=Fork)](https://github.com/tasmota/decode-config/network)
 [![donate](https://img.shields.io/badge/donate-PayPal-blue.svg)](https://paypal.me/NorbertRichterDE)
@@ -49,229 +30,205 @@
 |:------------------------|:-----------------------:|:------------------:|
 | encrypted               |           No            |         Yes        |
 | readable                |           Yes           |         No         |
 | editable                |           Yes           |         No         |
 | batch processing        |           Yes           |         No         |
 | Backup/Restore subsets  |           Yes           |         No         |
 
-**decode-config** is compatible with all [Tasmota](https://github.com/arendst/Tasmota) versions, starting from Tasmota v5.10.0 up to the current one.
-
-## Development
+**decode-config** is compatible with [Tasmota](https://github.com/arendst/Tasmota) starting from v5.10.0 up to now.
 
-Using the latest development version of decode-config is only necessary if you also use the latest development version of Tasmota.
+## Content
 
-<!-- markdownlint-disable MD033 -->
-[![development version](https://img.shields.io/badge/development-v13.0.0.0-blue.svg)](https://github.com/tasmota/decode-config/tree/development)
+**This is the developer branch which contains decode-config matching the latest Tasmota developer version.**
 
-## Table of contents
+This branch does not contain any binaries. If you want to use a precompiled **decode-config** binary
+you can use binaries from latest [Release](https://github.com/tasmota/decode-config/releases).
 
-* [Development](#development)
-* [Table of contents](#table-of-contents)
-* [Running the program](#running-the-program)
-  * [Installation](#installation)
-* [Usage](#usage)
-  * [Basics](#basics)
-  * [Tasmota source](#tasmota-source)
-  * [Format JSON output](#format-json-output)
-  * [Parameter file](#parameter-file)
-  * [Save backup](#save-backup)
-  * [Restore backup](#restore-backup)
-  * [Auto file extensions](#auto-file-extensions)
-  * [Test your parameter](#test-your-parameter)
-  * [Console outputs](#console-outputs)
-  * [Filter by groups](#filter-by-groups)
-* [Usage examples](#usage-examples)
-  * [Using Tasmota binary configuration files](#using-tasmota-binary-configuration-files)
-  * [Using JSON editable file](#using-json-editable-file)
-  * [Use batch processing](#use-batch-processing)
-* [File Formats](#file-formats)
-  * [.dmp format](#dmp-format)
-  * [.json format](#json-format-1)
-  * [.bin format](#bin-format)
-* [Program parameter list](#program-parameter-list)
-  * [--full-help](#--full-help)
-  * [Parameter notes](#parameter-notes)
-  * [Obsolete parameters](#obsolete-parameters)
-* [Generated Tasmota commands](#generated-tasmota-commands)
-* [Program return codes](#program-return-codes)
+> **Note**  
+If you want to run the development **decode-config.py** from this branch, you need an
+installed [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) environment.
+See [Running as Python script](#running-as-python-script) for more details.
+
+### Files
+
+| File                     | Description |
+|:-------------------------|:------------------------------------------------------------------------|
+| `build`                  | contains files to build executables                                     |
+| `decode-config.py`       | Python source file running under your local Python environment          |
+| `README.md`              | This content                                                            |
+
+### Table of contents
+
+* [decode-config](#decode-config)
+  * [Content](#content)
+    * [Files](#files)
+    * [Table of contents](#table-of-contents)
+  * [Running the program](#running-the-program)
+    * [Prerequisite](#prerequisite)
+  * [Usage](#usage)
+    * [Basics](#basics)
+    * [Format JSON output](#format-json-output)
+    * [Parameter file](#parameter-file)
+    * [Save backup](#save-backup)
+    * [Restore backup](#restore-backup)
+    * [Auto file extensions](#auto-file-extensions)
+    * [Test your parameter](#test-your-parameter)
+    * [Console outputs](#console-outputs)
+    * [Filter by groups](#filter-by-groups)
+    * [Usage examples](#usage-examples)
+  * [File Formats](#file-formats)
+    * [.dmp format](#dmp-format)
+    * [.json format](#json-format)
+    * [.bin format](#bin-format)
+  * [Program parameter list](#program-parameter-list)
+    * [--full-help](#--full-help)
+    * [Parameter notes](#parameter-notes)
+    * [Obsolete parameters](#obsolete-parameters)
+  * [Generated Tasmota commands](#generated-tasmota-commands)
+  * [Program return codes](#program-return-codes)
 
 ## Running the program
 
-To use **decode-config.py** you can install it using Python environment and following the [Installation](#installation) section below.
-
-Alternatively you can download a ready-made binary from [Releases](https://github.com/tasmota/decode-config/releases) to use it without installing Python.
-
-### Installation
-
-**decode-config.py** needs an installed [Python](https://en.wikipedia.org/wiki/Python_%28programming_language%29) environment - (see [Prerequisite](#prerequisite)).
-
-After you have installed your Python environment, there are two ways to install deocde-config:
-
-#### Installation using PyPi
-
-```shell
-pip install decode-config
-```
+The program does not have a graphical user interface (GUI), you have to run it from your OS command line using [program arguments](#usage).
 
-The program does not have a graphical user interface (GUI), you have to run it from your OS command line using [program arguments](#usage) - see [Usage](#usage) for more details.
+### Prerequisite
 
-#### Manual installation
+#### Tasmota WebServer
 
-This is only necessary if you want to run **decode-config.py** from [development branch](https://github.com/tasmota/decode-config/tree/development). First install the required modules manually
+[Tasmota](https://github.com/arendst/Tasmota) provides its configuration data by http request only. To receive and send configuration data from Tasmota devices directly the http WebServer in Tasmota must be enabled:
 
-```shell
-python -m pip install -r requirements.txt
-```
+* enable web-server admin mode (Tasmota web command [WebServer 2](https://tasmota.github.io/docs/Commands/#webserver))
+* for self-compiled firmware enable web-server with (`#define USE_WEBSERVER` and `#define WEB_SERVER 2`).
 
-After that you can use the Phython script **decode-config.py** as normal program:
+> **Note**  
+Using MQTT for exchanging Tasmota configuration data is supported by Tasmota since v9.4.0.3; **decode-config** will be able using MQTT in future supporting configuration data exchange this way too.
 
-```shell
-decode-config.py
-```
+#### Python
 
-#### Prerequisite
+**decode-config.py** needs an installed [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) environment.
 
-Since **decode-config.py** is a Python program, it requires an installed [Python](https://en.wikipedia.org/wiki/Python_%28programming_language%29) environment.
+> **Note**  
+Due to the [Python 2.7 EOL](https://github.com/python/devguide/pull/344) in Jan 2020 Python 2.x is no longer supported.
 
 ##### Linux
 
-Install [Python 3.x](https://www.python.org/downloads/) and Pip:
+Install [Python 3.x](https://www.python.org/downloads/), Pip and follow [library installation for all OS](#all-os) below.
 
 ```bash
 sudo apt-get install python3 python3-pip
 ```
 
-##### Windows
+##### Windows 10
 
-Install [Python 3.x](https://www.python.org/downloads/windows/) as described
+Install [Python 3.x](https://www.python.org/downloads/windows/) as described and follow [library installation for all OS](#all-os) below.
 
 ##### MacOS
 
-Install [Python 3.x](https://www.python.org/downloads/mac-osx/) as described
+Install [Python 3.x](https://www.python.org/downloads/mac-osx/) as described and follow [library installation for all OS](#all-os) below.
+
+##### All OS
+
+After python and pip is installed, install dependencies:
+
+```shell
+python -m pip install requests configargparse
+```
 
 ## Usage
 
 For an overview start the program without any parameter and you will get a short help:
 
 <!-- markdownlint-capture -->
 <!-- markdownlint-disable MD031 -->
 ```bash
-decode-config.py
+decode-config
 ```
+> **Note**  
+Replace `decode-config` by the program name your are using:  
+`decode-config.py` when running as Python executable.
+<!-- markdownlint-restore -->
 
 This prints a short help:
 
 ```help
-usage: decode-config.py [-s <filename|host|url>] [-p <password>]
-                        [--fulltopic <topic>] [--cafile <file>]
-                        [--certfile <file>] [--keyfile <file>] [--insecure]
-                        [--keepalive <sec>] [-i <restorefile>]
+usage: decode-config.py [-s <filename|host|url>] [-i <restorefile>]
                         [-o <backupfile>] [-t json|bin|dmp] [-E] [-e] [-F]
                         [--json-indent <indent>] [--json-compact]
                         [--json-show-pw] [--cmnd-indent <indent>]
-                        [--cmnd-groups] [--cmnd-sort]
-                        [--cmnd-use-rule-concat] [--cmnd-use-backlog]
-                        [-c <configfile>] [-S] [-T json|cmnd|command]
+                        [--cmnd-groups] [--cmnd-sort] [--cmnd-use-rule-concat]
+                        [--cmnd-use-backlog] [-c <configfile>] [-S]
+                        [-T json|cmnd|command]
                         [-g <groupname> [<groupname> ...]] [-w] [--dry-run]
                         [-h] [-H] [-v] [-V]
 ```
 
 For advanced help run **decode-config** with parameter `--full--help` or `-H`. This will print a [Program parameter list](#program-parameter-list).
 
 > **Note**  
-If you're missing older parameters, don't worry, they're still there (see [Obsolete parameters](#obsolete-parameters)).
+If you miss parameters here that are already in use, don't worry, they are still there.  
+For details see [Obsolete parameters](#obsolete-parameters)
 
 ### Basics
 
-To get a program result, pass at least a [Tasmota source](#tasmota-source) from which you want to read the configuration data.
-
-### Tasmota source
-
-The Tasmota source determines where the configuration data should be loaded from and saved to.
-A source can be an offline file or an online Tasmota device accessed via HTTP or indirectly via MQTT.
-
-Use `--source` parameter to determine the configuration data source:
-
-#### Binary (*.dmp) file (Offline)
+To get a result, at least pass a Tasmota source where you want to read the configuration from.
 
-Source is a Tasmota configuration file (having extension `.dmp`).
+Source can be either
 
-Pass the filename direclty or encoded as a [file-URL](https://en.wikipedia.org/wiki/URL):
+* a device hostname, IP or [http-url](https://en.wikipedia.org/wiki/URL) available and online within your network:  
+use `--source <host|url>` or `-s <host|url>` parameter
+* a Tasmota configuration file (having extension `.dmp`):  
+use `--source <filename>` or `-s <filename>` parameter
 
-```bash
-decode-config --source tasmota-4281.dmp
-decode-config -s file://path/to/tasmota-4281.dmp
-```
+The [http-url](https://en.wikipedia.org/wiki/URL) variant also allows `<user>`, `<password>` and `<port>` number to be specified:
 
-#### HTTP connection (Online)
+* `--source http://admin:myPaszxwo!z@tasmota-4281`
+* `--source http://tasmota-4281:80`
+* `--source http://admin:myPaszxwo!z@tasmota-4281:80`
 
-Source is an online HTTP connection to a running Tasmota device. To use this source, **decode-config** must have access to the network on which Tasmota is running, [Tasmota Webserver](https://tasmota.github.io/docs/Commands/#webserver) running in admin mode (`WebServer 2`) is mandatory.
+#### Basic example
 
-Specify the hostname, IP o or [http-url](https://en.wikipedia.org/wiki/URL) of the Tasmota device.
-
-An optionally required HTTP password, username and different HTTP port of the device can be specified via [URL](https://en.wikipedia.org/wiki/URL) or separately via `--username`, `--password` and `--port`
+##### Access an online device
 
 ```bash
 decode-config --source tasmota-4281
 decode-config -s 192.168.10.92
-decode-config --source http://tasmota-4281 --password myPaszxwo!z
-decode-config --source http://admin:myPaszxwo!z@tasmota-4281:8000
-decode-config --source http://admin:myPaszxwo!z@tasmota-4281/cs?
+decode-config --source http://tasmota-4281
+decode-config --source http://admin:myPaszxwo!z@tasmota-4281
 ```
 
-An appended HTTP path (here "`/cs?`") is ignored.
-
-#### MQTT transission (Online)
+##### Access a config file
 
-Source is a MQTT server and topic where an online Tasmota device is connected to. To use this source, **decode-config** does not need to have access to the same network that Tasmota is running on, it just needs access to the MQTT server that Tasmota also uses.
+```bash
+decode-config --source tasmota-4281.dmp
+decode-config -s tasmota-4281.dmp
+```
 
-##### MQTT connection parameter
+will output a readable configuration in [JSON](http://www.json.org/)-format, e.g.:
 
-Specify the hostname or IP of the MQTT server (possibly also specify username and password for the MQTT server) and the Tasmota MQTT topic. The **decode-config** connection to MQTT server also allows SSL/TLS connection.
+```json
+{"altitude": 112, "baudrate": 115200, "blinkcount": 10, "blinktime": 10,...
+"ws_width": [1, 3, 5]}
+```
 
-The MQTT username and password must be encoded within the URL (the parameter `--password` can not be used for that, it has a different function here).  
-If the username/password combination for the **decode-config** MQTT connection is different from the one used by Tasmota itself (Tasmota command `MQTTPassword`), the Tasmota MQTT password must be specified via the `--password` parameter.
+> **Note**  
+The json names (like `"altitude"` or `"blinktime"` are internal names from Tasmotas [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/settings.h) STRUCT `Settings` and are not the same as known from Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/). However, since most variable names are self-describing, the functional meaning should be given in most cases.
 
-The Tasmota topic can be specfied either within the [URL path](https://en.wikipedia.org/wiki/URL#Syntax) component or using optional `--fulltopic` parameter.  
-The topic must be the full topic of the Tasmota device without any trailing command or result part. You can use any of the prefixed topic (*cmnd*, *stat* or *tele* topic) or use the placeholder *%prefix%* for it, example  
-`%prefix%/tasmota-4281` or `tele/tasmota-4281` are valid topics  
-`cmnd/tasmota-4281/POWER` or `tele/tasmota-4281/STATE` are invalid topics due to the trailing part.
+#### Password protected device
 
-For SSL/TLS connection to MQTT server use `mqtts://` [URL scheme](https://en.wikipedia.org/wiki/URL#Syntax).
+If you try to access data from a device and you get an error like `ERROR 401: Error on http GET request for http://.../dl - Unauthorized` you need to pass your WebPassword for this device:
 
 ```bash
-decode-config --source mqtts://mybroker.example.com/%prefx%/tasmota-4281
-decode-config --source mqtts://mybroker.example.com:8883/tele/tasmota-4281
-decode-config --source mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com  --fulltopic tele/tasmota-4281
-decode-config --source mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota-4281 --password myTasmotaMQTTPaszxwo!z
+decode-config --source tasmota-4281 --password "myPaszxwo!z"
 ```
 
-For own certifications use the parameters `--cafile`, `--certfile` and `--keyfile`. To suppress certification verification use `--insecure`.
-
-For none SSL/TLS connection to MQTT server use `mqtt://` [URL scheme](https://en.wikipedia.org/wiki/URL#Syntax).
-
-```bash
-decode-config --source mqtt://mybroker.example.com/%prefx%/tasmota-4281
-decode-config --source mqtt://mybroker.example.com:1883/tele/tasmota-4281
-decode-config --source mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com  --fulltopic tele/tasmota-4281
-decode-config --source mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota-4281 --password myTasmotaMQTTPaszxwo!z
-```
+> **Hint**  
+*decode-config* username default is `admin`. For self-compiled binaries using a non-standard web username, use `-u <user>` or `--username <user>`.
 
 ### Format JSON output
 
-All basic examples above will output a readable configuration in [JSON](http://www.json.org/)-format, e.g.:
-
-```json
-{"altitude": 112, "baudrate": 115200, "blinkcount": 10, "blinktime": 10,...
-"ws_width": [1, 3, 5]}
-```
-
-> **Note**  
-The json names (like `"altitude"` or `"blinktime"` are internal names from Tasmotas [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/include/tasmota_types.h) STRUCT `Settings` and are not the same as known from Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/). However, since most variable names are self-describing, the functional meaning should be given in most cases.
-
 The default JSON output can be formatted for better reading using the `--json-indent <n>` parameter:
 
 ```bash
 decode-config --source tasmota-4281 --password "myPaszxwo!z" --json-indent 2
 ```
 
 This will print a pretty better readable format and the example above becomes:
@@ -329,56 +286,52 @@
 
 ### Save backup
 
 To save data from a device or [*.dmp](#dmp-format) file into a backup file, use `--backup-file <filename>`.
 
 #### Backup filename macros
 
-You can use the following placeholders within filenames:
+You can use the following placeholders within backup/restore filenames:
 
-* **@v** is replaced by *Tasmota Version* (backup & restore filenames)
-* **@d** is replaced by *Devicename* (backup & restore filenames)
-* **@f** is replaced by first *Friendlyname1* (backup & restore filenames)
-* **@h** is replaced by the *Hostname* from configuration data (backup & restore filenames)  
-Note: This is the static hostname which is configured by the command *Hostname*, for real hostname from a device use macro the **@H**)
-* **@H** is replaced by the live device hostname  (only for http sources, backup & restore filenames)  
-Note: This can be different to the configured hostname as this can contain also macros).source
-* **@F** is replaced by the filename of MQTT request (only for MQTT sources, backup filenames only).  
-This is usually the filename that Tasmota uses when saving the configuration in the WebUI.
+* **@v** is replaced by _Tasmota Version_
+* **@d** is replaced by _Devicename_
+* **@f** is replaced by first _Friendlyname1_
+* **@h** is replaced by the __Hostname__ from configuration data (note: this is the static hostname which is configured by the command __Hostname__, for real hostname from a device use macro the **@H**)
+* **@H** is replaced by the live device hostname note: this can be different to the configured hostname as this can contain also macros). Only valid when using real devices as source
 
 Example:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 --backup-file Config_@d_@v
 ```
 
-This will create a file like `Config_Tasmota_13.0.json` (the part `Tasmota` and `13.0` will choosen related to your device configuration).
+This will create a file like `Config_Tasmota_10.1.0.json` (the part `Tasmota` and `10.1.0` will choosen related to your device configuration).
 
 #### Save multiple backup at once
 
-The `--backup-file` parameter can be specified multiple times to create different backup with different names and/or different formats at once:
+Since **decode-config** v8.2.0.5 the `--backup-file` parameter can be specified multiple times. With that it's easy to create different backup with different names and/or different formats at once:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 -o Config_@d_@v -o Backup_@H.json -o Backup_@H.dmp
 ```
 
 creates three backup files:
 
-* `Config_Tasmota_13.0.json` using JSON format
+* `Config_Tasmota_10.1.0.json` using JSON format
 * `Backup_tasmota-4281.json` using JSON format
 * `Backup_tasmota-4281.dmp` using Tasmota configuration file format
 
 ### Restore backup
 
 Reading back a previously saved backup file, use the `--restore-file <filename>` parameter.
 
-To restore the previously save backup file `Config_Tasmota_13.0.json` to device `tasmota-4281` use:
+To restore the previously save backup file `Config_Tasmota_10.1.0.json` to device `tasmota-4281` use:
 
 ```bash
-decode-config -c my.conf -s tasmota-4281 --restore-file Config_Tasmota_13.0
+decode-config -c my.conf -s tasmota-4281 --restore-file Config_Tasmota_10.1.0
 ```
 
 Restore operation also allows placeholders **@v**, **@d**, **@f**, **@h** or **@H** like in backup filenames so we can use the same naming as for the backup process:
 
 ```bash
 decode-config -c my.conf -s tasmota-4281 --restore-file Config_@d_@v
 ```
@@ -456,17 +409,17 @@
 ### Console outputs
 
 Output to the console screen is the default when calling the program without any backup or restore parameter.  
 Screen output is suppressed when using backup or restore parameter. In that case you can force screen output with `--output`.
 
 The console screen output supports two formats:
 
-* [JSON](#json-format):<br>
+* [JSON](#console-json-format):<br>
 This is identical with the backup/restore [json file Format](#json-format) but printed on screen standard output.
-* [Tasmota command](#tasmota-web-command-format):<br>
+* [Tasmota command](#console-tasmota-command-format):<br>
 This outputs the most (but not all!) configuration data as Tasmota [web-console commands](https://tasmota.github.io/docs/Commands/).
 
 #### JSON format
 
 The default console output format is [JSON](#json-format) (optional you can force JSON backup format using `--output-format json`).
 
 Example:
@@ -615,76 +568,39 @@
 
 ```bash
 decode-config -s tasmota-4281 -c my.conf --output-format cmnd --group Main MQTT Management Wifi
 ```
 
 Filtering by groups affects the entire output, regardless of whether screen output or backup file.
 
-## Usage examples
-
-### Using Tasmota binary configuration files
-
-These examples use an online Tasmota device accessed over HTTP. The hostname of the Tasmota device is `tasmota-2f5d44-4281`
-
-#### Backup an online Tasmota device via HTTP into a Tasmota configuration file
-
-##### Use args to choice the file format
-
-```bash
-  decode-config -c my.conf -s tasmota-2f5d44-4281 --backup-type dmp --backup-file Config_@d_@v
-```
-
-##### Use file extension to choice the file format
-
-```bash
-decode-config -c my.conf -s tasmota-2f5d44-4281 --backup-file Config_@d_@v.dmp
-```
-
-#### Restore a Tasmota configuration file to an online Tasmota device via HTTP
-
-```bash
-decode-config -c my.conf -s http://tasmota-2f5d44-4281 --restore-file Config_@d_@v.dmp
-```
-
-### Using JSON editable file
-
-These examples use an online Tasmota device that is accessed indirectly via MQTT.
-
-In these examples, the MQTT server parameters are the same as those used by Tasmota itself:
-
-* MQTT Server: `mybroker.example.com`
-* MQTT Username: `mqttuser`
-* MQTT Password: `myBrokerPaszxwo!z`
-* Tasmota topic: `tele/tasmota_2F5D44`
-
-#### Backup an online Tasmota device via MQTT into a JSON file
+### Usage examples
 
-##### Use an unencrypted MQTT connection
+#### Using Tasmota binary configuration files
 
-MQTT server uses a non default port 42110
+1. Restore a Tasmota configuration file
 
-```bash
-decode-config -s mqtt://mqttuser:myBrokerPaszxwo!z@mybroker.example.com:42110/tele/tasmota_2F5D44 --backup-file Config_2f5d44-4281.json
-```
+  ```bash
+  decode-config -c my.conf -s tasmota --restore-file Config_Tasmota_6.2.1.dmp
+  ```
 
-##### Use SSL/TLS MQTT connection
+1. Backup device using Tasmota configuration compatible format
 
-Limit the configuration data to the groups `Control`, `Management` and `SetOption`
+   a) use file extension to choice the file format
 
-```bash
-decode-config -s mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com --fulltopic tele/tasmota_2F5D44 --backup-file Config_2f5d44-4281.json -g Control Management SetOption
-```
+  ```bash
+  decode-config -c my.conf -s tasmota --backup-file Config_@d_@v.dmp
+  ```
 
-#### Restore a JSON file to an online Tasmota device via MQTT
+   b) use args to choice the file format
 
-```bash
-decode-config -s mqtts://mqttuser:myBrokerPaszxwo!z@mybroker.example.com/tele/tasmota_2F5D44 --restore-file Config_2f5d44-4281.json
-```
+  ```bash
+    decode-config -c my.conf -s tasmota --backup-type dmp --backup-file Config_@d_@v
+  ```
 
-### Use batch processing
+#### Use batch processing
 
 Linux
 
 ```bash
 for device in tasmota1 tasmota2 tasmota3; do ./decode-config -c my.conf -s $device -o Config_@d_@v
 ```
 
@@ -708,18 +624,18 @@
 
 ### .json format
 
 This format uses the [JSON](http://www.json.org/) notation and contains the complete configuration data in plain text, human readable and editable.
 
 The .json format can be created by **decode-config** using the backup function (`--backup-file <filename>`) (for better identification you can append the optional parameter `--backup-type json`, but that's optional as json is the default backup format).
 
-In contrast to the other two binary formats [.dmp](#dmp-format) and [.bin](#bin-format), this type of format also allows the [partial modification](#restore-subset-of-data) of configurations.
+In contrast to the other two binary formats [.dmp](#dmp-format) and [.bin](#bin-format), this type of format also allows the [partial modification](#restore-a-subset-of-backup-data) of configurations.
 
 > **Note**  
-The keys used within the JSON file are based on the variable names of Tasmota source code in [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/include/tasmota_types.h) so they do not have the same naming as known for Tasmota web commands. However, since the variable names are self-explanatory, there should be no difficulties in assigning the functionality of the variables.
+The keys used within the JSON file are based on the variable names of Tasmota source code in [settings.h](https://github.com/arendst/Tasmota/blob/master/tasmota/settings.h) so they do not have the same naming as known for Tasmota web commands. However, since the variable names are self-explanatory, there should be no difficulties in assigning the functionality of the variables.
 
 ### .bin format
 
 This format is binary with the same structure as the [.dmp](#dmp-format) format. The differences to .dmp are:
 
 * .bin is decrypted
 * .bin has 4 additional bytes at the end of the file
@@ -737,84 +653,58 @@
 A short list of possible program args is displayed using `-h` or `--help`.
 
 ### --full-help
 
 For advanced help use parameter `-H` or `--full-help`:
 
 ```help
-usage: decode-config.py [-s <filename|host|url>] [-p <password>]
-                        [--fulltopic <topic>] [--cafile <file>]
-                        [--certfile <file>] [--keyfile <file>] [--insecure]
-                        [--keepalive <sec>] [-i <restorefile>]
+usage: decode-config.py [-s <filename|host|url>] [-i <restorefile>]
                         [-o <backupfile>] [-t json|bin|dmp] [-E] [-e] [-F]
                         [--json-indent <indent>] [--json-compact]
                         [--json-show-pw] [--cmnd-indent <indent>]
-                        [--cmnd-groups] [--cmnd-sort]
-                        [--cmnd-use-rule-concat] [--cmnd-use-backlog]
-                        [-c <configfile>] [-S] [-T json|cmnd|command]
+                        [--cmnd-groups] [--cmnd-sort] [--cmnd-use-rule-concat]
+                        [--cmnd-use-backlog] [-c <configfile>] [-S]
+                        [-T json|cmnd|command]
                         [-g <groupname> [<groupname> ...]] [-w] [--dry-run]
                         [-h] [-H] [-v] [-V]
 
-Backup/Restore Tasmota configuration data. Args that start with '--' (eg.
--s) can also be set in a config file (specified via -c). Config file syntax
+Backup/Restore Tasmota configuration data. Args that start with '--' (eg. -s)
+can also be set in a config file (specified via -c). Config file syntax
 allows: key=value, flag=true, stuff=[a,b,c] (for details, see syntax at
 https://goo.gl/R74nmi). If an arg is specified in more than one place, then
 commandline values override config file values which override defaults.
 
 Source:
   Read/Write Tasmota configuration from/to
 
   -s, --source <filename|host|url>
                         source used for the Tasmota configuration (default:
-                        None). Specify source type, path, file, user,
-                        password, hostname, port and topic at once as an
-                        URL. The URL must be in the form 'scheme://[username
-                        [:password]@]host[:port][/topic]|pathfile'where
-                        scheme is 'file' for a tasmota binary config file,
-                        'http' for a Tasmota HTTP web connection and
-                        'mqtt(s)' for Tasmota MQTT transport ('mqtts' uses a
-                        TLS connection to MQTT server)
-  -p, --password <password>
-                        Web server password on HTTP source (set by Tasmota
-                        'WebPassword' command), MQTT server password in MQTT
-                        source (set by Tasmota 'MqttPassword' command)
-                        (default: None)
-
-MQTT:
-  MQTT transport settings
-
-  --fulltopic <topic>   Optional MQTT transport fulltopic used for accessing
-                        Tasmota device (default: )
-  --cafile <file>       Enables SSL/TLS connection: path to a or filename of
-                        the Certificate Authority certificate files that are
-                        to be treated as trusted by this client (default
-                        None)
-  --certfile <file>     Enables SSL/TLS connection: filename of a PEM
-                        encoded client certificate file (default None)
-  --keyfile <file>      Enables SSL/TLS connection: filename of a PEM
-                        encoded client private key file (default None)
-  --insecure            suppress verification of the MQTT server hostname in
-                        the server certificate (default False)
-  --keepalive <sec>     keepalive timeout for the client (default 60)
+                        None). The argument can be a <filename> containing
+                        Tasmota .dmp configuation data or a <hostname>,
+                        <ip>-address, <url> which means an online tasmota
+                        device is used. A url can also contain web login and
+                        port data in the format
+                        http://<user>:<password>@tasmota:<port>, e. g,
+                        http://admin:mypw@mytasmota:8090
 
 Backup/Restore:
   Backup & restore specification
 
   -i, --restore-file <restorefile>
                         file to restore configuration from (default: None).
                         Replacements: @v=firmware version from config,
                         @d=devicename, @f=friendlyname1, @h=hostname from
-                        config, @H=device hostname (http source only)
+                        config, @H=device hostname (invalid if using a file as
+                        source)
   -o, --backup-file <backupfile>
                         file to backup configuration to, can be specified
                         multiple times (default: None). Replacements:
                         @v=firmware version from config, @d=devicename,
                         @f=friendlyname1, @h=hostname from config, @H=device
-                        hostname (http source only), @F=configuration
-                        filename from MQTT request (mqtt source only)
+                        hostname (invalid if using a file as source)
   -t, --backup-type json|bin|dmp
                         backup filetype (default: 'json')
   -E, --extension       append filetype extension for -i and -o filename
                         (default)
   -e, --no-extension    do not append filetype extension, use -i and -o
                         filename as passed
   -F, --force-restore   force restore even configuration is identical
@@ -830,23 +720,22 @@
   --json-show-pw        unhide passwords (default)
 
 Tasmota command output:
   Tasmota command output format specification. To revert an option, insert
   "dont" or "no" after "cmnd", e.g. --cmnd-no-indent, --cmnd-dont-sort
 
   --cmnd-indent <indent>
-                        Tasmota command grouping indent level (default:
-                        '2'). 0 disables indent
+                        Tasmota command grouping indent level (default: '2').
+                        0 disables indent
   --cmnd-groups         group Tasmota commands (default)
   --cmnd-sort           sort Tasmota commands (default)
   --cmnd-use-rule-concat
                         use rule concatenation with + for Tasmota 'Rule'
                         command
-  --cmnd-use-backlog    use 'Backlog' for Tasmota commands as much as
-                        possible
+  --cmnd-use-backlog    use 'Backlog' for Tasmota commands as much as possible
 
 Common:
   Optional arguments
 
   -c, --config <configfile>
                         program config file - can be used to set default
                         command parameters (default: None)
@@ -854,16 +743,16 @@
                         (default do not output on backup or restore usage)
   -T, --output-format json|cmnd|command
                         display output format (default: 'json')
   -g, --group <groupname>
                         limit data processing to command groups (default no
                         filter)
   -w, --ignore-warnings
-                        do not exit on warnings. Not recommended, used by
-                        your own responsibility!
+                        do not exit on warnings. Not recommended, used by your
+                        own responsibility!
   --dry-run             test program without changing configuration data on
                         device or file
 
 Info:
   Extra information
 
   -h, --help            show usage help message and exit
@@ -879,15 +768,15 @@
 For details see [Obsolete parameters](#obsolete-parameters)
 
 ### Parameter notes
 
 * Filename replacement macros **@h** and **@H**:
   * **@h**
 The **@h** replacement macro uses the hostname configured with the Tasomta Wifi `Hostname <host>` command (defaults to `%s-%04d`). It will not use the network hostname of your device because this is not available when working with files only (e.g. `--source <filename>` as source).
-To prevent having an useless % in your filename, **@h** will not replaced by hostname if this contains '%' characters.
+To prevent having a useless % in your filename, **@h** will not replaced by hostname if this contains '%' characters.
   * **@H**
 If you want to use the network hostname within your filename, use the **@H** replacement macro instead - but be aware this will only replaced if you are using a network device as source (`<hostname>`, `<ip>`, `<url>`); it will not work when using a file as source (`<filename>`)
 
 ### Obsolete parameters
 
 The parameters listed here continue to work and are supported, but are no longer listed in the parameter list:
 
@@ -899,14 +788,16 @@
 file used for the Tasmota configuration (default: None)'
 * `-d`, `--device`, `--host` `<host|url>`  
 hostname, IP-address or url used for the Tasmota configuration (default: None)
 * `-P`, `--port` `<port>`  
 TCP/IP port number to use for the host connection (default: 80)
 * `-u`, `--username` `<username>`  
 host HTTP access username (default: admin)
+* `-p`, `--password` `<password>`  
+host HTTP access password (default: None)
 
 #### Obsolete JSON formating parameters
 
 * `--json-unhide-pw` same as `--json-show-pw`
 * `--json-hide-pw` same as `--json-dont-show-pw`
 * `--json-sort` sorts JSON output (this is the default)
 * `--json-unsort` prevents JSON sorting
@@ -938,94 +829,64 @@
 |                | LedState                    |                        |             |
 |                | Power<x\>                   |                        |             |
 |                | PowerOnState                |                        |             |
 |                | PulseTime<x\>               |                        |             |
 |                | SwitchDebounce              |                        |             |
 |                | SwitchMode<x\>              |                        |             |
 |                | Webbutton<x\>               |                        |             |
-|                | WCAEC<sup>2</sup>           |                        |             |
-|                | WCAECDSP<sup>2</sup>        |                        |             |
-|                | WCAECValue<sup>2</sup>      |                        |             |
-|                | WCAELevel<sup>2</sup>       |                        |             |
-|                | WCAGCGain<sup>2</sup>       |                        |             |
-|                | WCAWB<sup>2</sup>           |                        |             |
-|                | WCAWBGain<sup>2</sup>       |                        |             |
-|                | WCBPC<sup>2</sup>           |                        |             |
-|                | WCBrightness<sup>2</sup>    |                        |             |
-|                | WCClock<sup>2</sup>         |                        |             |
-|                | WCColorbar<sup>2</sup>      |                        |             |
-|                | WCContrast<sup>2</sup>      |                        |             |
-|                | WCDCW<sup>2</sup>           |                        |             |
-|                | WCFeature<sup>2</sup>       |                        |             |
-|                | WCFlip<sup>2</sup>          |                        |             |
-|                | WCGainCeiling<sup>2</sup>   |                        |             |
-|                | WCGammaCorrect<sup>2</sup>  |                        |             |
-|                | WCLensCorrect<sup>2</sup>   |                        |             |
+|                | WCStream<sup>2</sup>        |                        |             |
 |                | WCMirror<sup>2</sup>        |                        |             |
-|                | WCResolution<sup>2</sup>    |                        |             |
+|                | WCFlip<sup>2</sup>          |                        |             |
 |                | WCRtsp<sup>2</sup>          |                        |             |
-|                | WCSAuth<sup>2</sup>         |                        |             |
+|                | WCBrightness<sup>2</sup>    |                        |             |
+|                | WCContrast<sup>2</sup>      |                        |             |
 |                | WCSaturation<sup>2</sup>    |                        |             |
-|                | WCSpecialEffect<sup>2</sup> |                        |             |
-|                | WCStream<sup>2</sup>        |                        |             |
-|                | WCWBMode<sup>2</sup>        |                        |             |
-|                | WCWPC<sup>2</sup>           |                        |             |
+|                | WCResolution<sup>2</sup>    |                        |             |
 | **Management** | DeepSleepTime               | *Delay*                |             |
 |                | DeviceName                  | *Gpios*                |             |
 |                | Emulation                   | *I2Cscan*              |             |
 |                | FriendlyName<x\>            | *Modules*              |             |
 |                | Gpio<x\>                    | *Reset*                |             |
 |                | I2CDriver<x\>               | *Restart*              |             |
 |                | Ifx                         | *State*                |             |
 |                | IfxBucket                   | *Status*               |             |
 |                | IfxHost                     | *Upgrade*              |             |
 |                | IfxPassword                 | *Upload*               |             |
 |                | IfxPort                     | *SSPMLog<sup>2</sup>*  |             |
 |                | IfxUser                     | *SSPEnergy<sup>2</sup>*|             |
-|                | IfxRP                       | *SSPHistory<sup>2</sup>*|            |
-|                | IfxPeriod                   | *SSPScan<sup>2</sup>*  |             |
-|                | IfxSensor                   | *SSPIamHere<sup>2</sup>*|            |
-|                | L1MusicSync                 |                        |             |
-|                | LogHost                     |                        |             |
+|                | IfxPeriod                   | *SSPHistory<sup>2</sup>*|            |
+|                | L1MusicSync                 | *SSPScan<sup>2</sup>*  |             |
+|                | LogHost                     | *SSPIamHere<sup>2</sup>*|            |
 |                | LogPort                     |                        |             |
 |                | Module                      |                        |             |
 |                | Module2                     |                        |             |
 |                | MqttLog                     |                        |             |
 |                | NtpServer<x\>               |                        |             |
 |                | OtaUrl                      |                        |             |
 |                | Pwm<x\>                     |                        |             |
 |                | PwmFrequency                |                        |             |
 |                | PwmRange                    |                        |             |
-|                | RtcNtpserver                |                        |             |
 |                | SaveData                    |                        |             |
 |                | SerialLog                   |                        |             |
 |                | Sleep                       |                        |             |
 |                | SSPMDisplay<sup>2</sup>     |                        |             |
 |                | SysLog                      |                        |             |
 |                | Template                    |                        |             |
 |                | Time                        |                        |             |
 |                | TimeSTD                     |                        |             |
 |                | TimeDST                     |                        |             |
 |                | Timezone                    |                        |             |
-|                | TouchThres<sup>2</sup>      |                        |             |
 |                | TuyaMCU                     |                        |             |
 |                | TuyaTempSetRes              |                        |             |
 |                | WebLog                      |                        |             |
-|                | WebTime                     |                        |             |
 | **WiFi**       | CORS                        | *AP*                   |             |
-|                | DnsTimeout                  | *Ping<x\>*             |             |
-|                | Ethernet<sup>2</sup>        | *WebSend*              |             |
-|                | EthAddress<sup>2</sup>      | *Publish*              |             |
-|                | EthClockMode<sup>2</sup>    | *Publish2*             |             |
-|                | EthType<sup>2</sup>         |                        |             |
-|                | EthIPAddress<sup>2</sup>    |                        |             |
-|                | EthSubnetmask<sup>2</sup>   |                        |             |
-|                | EthGateway<sup>2</sup>      |                        |             |
-|                | EthDNSServer<sup>2</sup>    |                        |             |
-|                | EthDNSServer2<sup>2</sup>   |                        |             |
+|                | Ethernet<sup>2</sup>        | *Ping<x\>*             |             |
+|                | EthAddress<sup>2</sup>      | *WebSend*              |             |
+|                | EthClockMode<sup>2</sup>    | *Publish*              |             |
+|                | EthType<sup>2</sup>         | *Publish2*             |             |
 |                | Hostname                    |                        |             |
 |                | IPAddress<x\>               |                        |             |
 |                | Password<x\>                |                        |             |
 |                | RgxAddress                  |                        |             |
 |                | RgxNAPT                     |                        |             |
 |                | RgxPassword                 |                        |             |
 |                | RgxSsid                     |                        |             |
@@ -1056,15 +917,14 @@
 |                | MqttTimeout                 |                        |             |
 |                | MqttWifiTimeout             |                        |             |
 |                | PowerRetain                 |                        |             |
 |                | Prefix<x\>                  |                        |             |
 |                | SensorRetain                |                        |             |
 |                | StateRetain                 |                        |             |
 |                | StateText<x\>               |                        |             |
-|                | StatusRetain                |                        |             |
 |                | SwitchRetain                |                        |             |
 |                | SwitchTopic                 |                        |             |
 |                | TelePeriod                  |                        |             |
 |                | Topic                       |                        |             |
 | **Rules**      | CalcRes                     | *Add<x\>*              |             |
 |                | Mem<x\>                     | *Event*                |             |
 |                | Rule<x\>                    | *Mult<x\>*             |             |
@@ -1102,28 +962,25 @@
 |                | OT_TWater                   |                        |             |
 |                | Sensor13                    |                        |             |
 |                | Sensor15                    |                        |             |
 |                | Sensor18                    |                        |             |
 |                | Sensor20                    |                        |             |
 |                | Sensor29                    |                        |             |
 |                | Sensor34                    |                        |             |
-|                | Sensor40                    |                        |             |
 |                | Sensor54                    |                        |             |
 |                | Sensor68                    |                        |             |
-|                | Sensor96                    |                        |             |
 |                | Shift595DeviceCount         |                        |             |
 |                | SpeedUnit                   |                        |             |
 |                | TempRes                     |                        |             |
 |                | TempOffset                  |                        |             |
 |                | VoltRes                     |                        |             |
 |                | WattRes                     |                        |             |
 |                | WeightRes                   |                        |             |
-|                | Wiper<x\>                   |                        |             |
 | **Power**      | AmpRes                      | *CurrentSet*           |             |
-|                | CurrentCal                  | *FrequencySet*         |             |
+|                | CurrentCal                  | *FrequencySet*         |`EnergyReset`|
 |                | CurrentHigh                 | *ModuleAddress*        |             |
 |                | CurrentLow                  | *PowerSet*             |             |
 |                | EnergyRes                   | *Status8*              |             |
 |                | EnergyToday                 | *Status9*              |             |
 |                | EnergyTotal                 | *VoltageSet*           |             |
 |                | EnergyYesterday             |                        |             |
 |                | FreqRes                     |                        |             |
@@ -1153,30 +1010,27 @@
 |                | ShdWarmupBrightness         |                        |             |
 |                | ShdWarmupTime               |                        |             |
 |                | Speed                       |                        |             |
 |                | StepPixels                  |                        |             |
 |                | Wakeup                      |                        |             |
 |                | WakeupDuration              |                        |             |
 | **RF**         | RfProtocol                  | *RfRaw*                | `RfCode`    |
-|                | RfTimeOut                   |                        | `RfHigh`    |
+|                |                             |                        | `RfHigh`    |
 |                |                             |                        | `RfHost`    |
 |                |                             |                        | `RfKey<x>`  |
 |                |                             |                        | `RfLow`     |
 |                |                             |                        | `RfSync`    |
 | **IR**         |                             | *IRsend<x\>*           |             |
 |                |                             | *IRhvac*               |             |
 | **SetOption**  | SetOption<x\>               |                        |             |
 | **Serial**     | Baudrate                    | *SerialSend<x\>*       |             |
-|                | ModbusBaudrate              | *SSerialSend<x\>*      |             |
-|                | ModbusSerialConfig          | *TCPStart*             |             |
-|                | SBaudrate                   | *TuyaSend<x\>*         |             |
-|                | SerialConfig                |                        |             |
-|                | SerialDelimiter             |                        |             |
+|                | SBaudrate                   | *SSerialSend<x\>*      |             |
+|                | SerialConfig                | *TCPStart*             |             |
+|                | SerialDelimiter             | *TuyaSend<x\>*         |             |
 |                | SSerialConfig               |                        |             |
-|                | SSerialSend9                |                        |             |
 |                | TCPBaudrate                 |                        |             |
 |                | TCPConfig                   |                        |             |
 | **Domoticz**   | DomoticzIdx<x\>             |                        |             |
 |                | DomoticzKeyIdx<x\>          |                        |             |
 |                | DomoticzSensorIdx<x\>       |                        |             |
 |                | DomoticzSwitchIdx<x\>       |                        |             |
 |                | DomoticzUpdateTimer         |                        |             |
@@ -1203,18 +1057,17 @@
 |                | ShutterCloseDuration<x\>    | *ShutterOpen<x\>*      |             |
 |                | ShutterEnableEndStopTime<x\>| *ShutterSetClose<x\>*  |             |
 |                | ShutterInvert<x\>           | *ShutterStop<x\>*      |             |
 |                | ShutterInvertWebButtons<x\> | *ShutterStopClose<x\>* |             |
 |                | ShutterLock<x\>             | *ShutterStopOpen<x\>*  |             |
 |                | ShutterMode<x\>             | *ShutterStopPosition<x\>*|           |
 |                | ShutterMotorDelay<x\>       | *ShutterStopToggle<x\>*|             |
-|                | ShutterMotorStop            | *ShutterStopToggleDir<x\>*|          |
-|                | ShutterOpenDuration<x\>     | *ShutterToggle<x\>*    |             |
-|                | ShutterPosition<x\>         | *ShutterToggleDir<x\>* |             |
-|                | ShutterPWMRange<x\>         |                        |             |
+|                | ShutterOpenDuration<x\>     | *ShutterStopToggleDir<x\>*|          |
+|                | ShutterPosition<x\>         | *ShutterToggle<x\>*    |             |
+|                | ShutterPWMRange<x\>         | *ShutterToggleDir<x\>* |             |
 |                | ShutterRelay<x\>            |                        |             |
 |                | ShutterSetHalfway<x\>       |                        |             |
 |                | ShutterTiltConfig<x\>       |                        |             |
 | **Telegram**   | TmChatId                    | *TmPoll*               |             |
 |                | TmState                     | *TmSend*               |             |
 |                | TmToken                     |                        |             |
 | **Zigbee**     | ZbConfig                    | *ZbBind*               |             |
@@ -1281,14 +1134,11 @@
 
 * **21** = internal error:  
 An unexpected internal error occured  
 
 * **22** = HTTP connection error:  
 Source device HTTP connection lost or unavailable  
 
-* **23** = MQTT connection error:  
-MQTT server connection error  
-
-* **24...** = python library exit code:  
+* **23...** = python library exit code:  
 An unexpected internal library error occured  
 
 * **4xx**/**5xx** = HTTP errors
```

