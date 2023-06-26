# Comparing `tmp/datapusher-plus-0.8.0.tar.gz` & `tmp/datapusher-plus-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapusher-plus-0.8.0.tar", last modified: Wed Jan 18 02:16:38 2023, max compression
+gzip compressed data, was "datapusher-plus-0.9.0.tar", last modified: Mon Jan 30 14:03:53 2023, max compression
```

## Comparing `datapusher-plus-0.8.0.tar` & `datapusher-plus-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jqnatividad  (1000) jqnatividad  (1000)        0 2023-01-18 02:16:38.104739 datapusher-plus-0.8.0/
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)    34499 2022-11-07 13:29:53.000000 datapusher-plus-0.8.0/LICENSE
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)       24 2022-11-07 13:29:53.000000 datapusher-plus-0.8.0/MANIFEST.in
--rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)    18016 2023-01-18 02:16:38.104739 datapusher-plus-0.8.0/PKG-INFO
--rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)    17314 2023-01-17 12:53:05.000000 datapusher-plus-0.8.0/README.md
-drwxrwxr-x   0 jqnatividad  (1000) jqnatividad  (1000)        0 2023-01-18 02:16:38.104739 datapusher-plus-0.8.0/datapusher/
--rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)     4210 2023-01-17 12:17:32.000000 datapusher-plus-0.8.0/datapusher/config.py
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)     3817 2022-12-10 16:19:40.000000 datapusher-plus-0.8.0/datapusher/config_local.py
--rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)    50806 2023-01-18 02:09:22.000000 datapusher-plus-0.8.0/datapusher/jobs.py
--rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)     1324 2023-01-15 14:08:27.000000 datapusher-plus-0.8.0/datapusher/main.py
--rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)      626 2022-12-09 13:55:11.000000 datapusher-plus-0.8.0/datapusher/settings_local.py
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)      268 2022-12-07 10:50:35.000000 datapusher-plus-0.8.0/datapusher/wsgi.py
-drwxrwxr-x   0 jqnatividad  (1000) jqnatividad  (1000)        0 2023-01-18 02:16:38.104739 datapusher-plus-0.8.0/datapusher_plus.egg-info/
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)    18016 2023-01-18 02:16:38.000000 datapusher-plus-0.8.0/datapusher_plus.egg-info/PKG-INFO
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)      408 2023-01-18 02:16:38.000000 datapusher-plus-0.8.0/datapusher_plus.egg-info/SOURCES.txt
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)        1 2023-01-18 02:16:38.000000 datapusher-plus-0.8.0/datapusher_plus.egg-info/dependency_links.txt
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)       95 2023-01-18 02:16:38.000000 datapusher-plus-0.8.0/datapusher_plus.egg-info/entry_points.txt
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)       85 2023-01-18 02:16:38.000000 datapusher-plus-0.8.0/datapusher_plus.egg-info/requires.txt
--rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)        1 2023-01-18 02:16:38.000000 datapusher-plus-0.8.0/datapusher_plus.egg-info/top_level.txt
--rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)       38 2023-01-18 02:16:38.104739 datapusher-plus-0.8.0/setup.cfg
--rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)     3463 2023-01-18 02:15:32.000000 datapusher-plus-0.8.0/setup.py
+drwxrwxr-x   0 jqnatividad  (1000) jqnatividad  (1000)        0 2023-01-30 14:03:53.654481 datapusher-plus-0.9.0/
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)    34499 2022-11-07 13:29:53.000000 datapusher-plus-0.9.0/LICENSE
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)       24 2022-11-07 13:29:53.000000 datapusher-plus-0.9.0/MANIFEST.in
+-rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)    15875 2023-01-30 14:03:53.654481 datapusher-plus-0.9.0/PKG-INFO
+-rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)    15173 2023-01-30 12:55:29.000000 datapusher-plus-0.9.0/README.md
+drwxrwxr-x   0 jqnatividad  (1000) jqnatividad  (1000)        0 2023-01-30 14:03:53.650480 datapusher-plus-0.9.0/datapusher/
+-rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)     4472 2023-01-23 10:56:47.000000 datapusher-plus-0.9.0/datapusher/config.py
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)     3817 2022-12-10 16:19:40.000000 datapusher-plus-0.9.0/datapusher/config_local.py
+-rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)    66199 2023-01-30 13:56:28.000000 datapusher-plus-0.9.0/datapusher/jobs.py
+-rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)     1324 2023-01-15 14:08:27.000000 datapusher-plus-0.9.0/datapusher/main.py
+-rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)      626 2022-12-09 13:55:11.000000 datapusher-plus-0.9.0/datapusher/settings_local.py
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)      268 2022-12-07 10:50:35.000000 datapusher-plus-0.9.0/datapusher/wsgi.py
+drwxrwxr-x   0 jqnatividad  (1000) jqnatividad  (1000)        0 2023-01-30 14:03:53.654481 datapusher-plus-0.9.0/datapusher_plus.egg-info/
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)    15875 2023-01-30 14:03:53.000000 datapusher-plus-0.9.0/datapusher_plus.egg-info/PKG-INFO
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)      408 2023-01-30 14:03:53.000000 datapusher-plus-0.9.0/datapusher_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)        1 2023-01-30 14:03:53.000000 datapusher-plus-0.9.0/datapusher_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)       95 2023-01-30 14:03:53.000000 datapusher-plus-0.9.0/datapusher_plus.egg-info/entry_points.txt
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)       92 2023-01-30 14:03:53.000000 datapusher-plus-0.9.0/datapusher_plus.egg-info/requires.txt
+-rw-r--r--   0 jqnatividad  (1000) jqnatividad  (1000)        1 2023-01-30 14:03:53.000000 datapusher-plus-0.9.0/datapusher_plus.egg-info/top_level.txt
+-rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)       38 2023-01-30 14:03:53.654481 datapusher-plus-0.9.0/setup.cfg
+-rw-rw-r--   0 jqnatividad  (1000) jqnatividad  (1000)     3481 2023-01-30 14:03:27.000000 datapusher-plus-0.9.0/setup.py
```

### Comparing `datapusher-plus-0.8.0/LICENSE` & `datapusher-plus-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datapusher-plus-0.8.0/PKG-INFO` & `datapusher-plus-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapusher-plus
-Version: 0.8.0
+Version: 0.9.0
 Summary: A standalone web service that parses the contents of a CKAN site's data files (CSV, TSV, Excel and ODS) and pushes them into its DataStore. Accelerated by qsv.
 Home-page: https://github.com/dathere/datapusher-plus
 License: AGPL
 Keywords: ckan csv tsv xls ods excel qsv
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
@@ -23,14 +23,16 @@
 [ckanext-xloader](https://github.com/ckan/ckanext-xloader) with the data type guessing of Datapusher.
 
 Datapusher+ is built using [CKAN Service Provider][], with [Messytables] replaced by [qsv].
 
 [TNRIS](https://tnris.org)/[TWDB](https://www.twdb.texas.gov/) provided the use cases that informed and supported the development
 of Datapusher+, specifically, to support a [Resource-first upload workflow](docs/RESOURCE_FIRST_WORKFLOW.md#Resource-first-Upload-Workflow).
 
+For a more detailed overview, see the [CKAN Monthly Live Jan 2023 presentation](https://docs.google.com/presentation/d/e/2PACX-1vT0BfmrrtaEINRGg4UI_m7B02_X6HlFr4yN_DXmgX9goVtgu2DNmZjl-SowL9ZA2ibQhDjScRRJh95q/pub?start=false&loop=false&delayms=3000).
+
 It features:
 
 * **"Bullet-proof", ultra-fast data type inferencing with qsv**
 
   Unlike [Messytables][] which scans only the the first few rows to guess the type of
   a column, [qsv][] scans the entire table so its data type inferences are guaranteed[^1].
 
@@ -123,17 +125,17 @@
     pip install -e .
 
 Install qsv:
 
 [Download the appropriate precompiled binaries](https://github.com/jqnatividad/qsv/releases/latest) for your platform and copy
 it to the appropriate directory, e.g. for Linux:
 
-    wget https://github.com/jqnatividad/qsv/releases/download/0.84.0/qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    unzip qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    rm qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    wget https://github.com/jqnatividad/qsv/releases/download/0.87.0/qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    unzip qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    rm qsv-0.87.0-x86_64-unknown-linux-gnu.zip
     sudo mv qsv* /usr/local/bin
 
 Alternatively, if you want to install qsv from source, follow
 the instructions [here](https://github.com/jqnatividad/qsv#installation). Note that when compiling from source,
 you may want to look into the [Performance Tuning](https://github.com/jqnatividad/qsv#performance-tuning)
 section to squeeze even more performance from qsv.
 
@@ -145,23 +147,23 @@
     qsvdp --update
 
 
 > ℹ️ **NOTE:** qsv is a general purpose CSV data-wrangling toolkit that gets regular updates. To update to the latest version, just run
 qsv with the `--update` option and it will check for the latest version and update as required.
 
 
-Copy `datapusher/config.py` to a new file like `config_local.py` and modify your configuration as required.
+Copy the `datapusher/dot-env.template` to file `datapusher/.env` and modify your configuration as required.
 Make sure to create the `datapusher` PostgreSQL user and the `datapusher_jobs` database (see [DataPusher+ Database Setup](#DataPusher+_Database_Setup)).
 
     cd datapusher
-    cp config.py config_local.py
+    cp dot-env.template .env
     # configure your installation as required
-    nano config_local.py
+    nano .env
 
-    python3 datapusher/main.py datapusher/config_local.py
+    python3 datapusher/main.py datapusher/config.py
 
 By default, DataPusher+ should be running at the following port:
 
     http://localhost:8800/
 
 ## Production deployment
 
@@ -177,41 +179,45 @@
 can be easily adapted to other WSGI servers like Gunicorn. You'll probably need
 to set up Nginx as a reverse proxy in front of it and something like Supervisor
 to keep the process up.
 
 
     # Install requirements for DataPusher+. Be sure to have at least Python 3.8
     sudo apt install python3-venv python3-dev build-essential libxslt1-dev libxml2-dev libffi-dev
-
+     
     cd /usr/lib/ckan
 
     # Create a virtualenv for DataPusher+. DP+ requires at least python 3.8.
     sudo python3.8 -m venv /usr/lib/ckan/dpplus_venv
 
     # Install qsv binary, if required
-    wget https://github.com/jqnatividad/qsv/releases/download/0.84.0/qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    unzip qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    wget https://github.com/jqnatividad/qsv/releases/download/0.87.0/qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    unzip qsv-0.87.0-x86_64-unknown-linux-gnu.zip
     sudo mv qsv* /usr/local/bin
-    rm qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    rm qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    
+    # Set Locales
+    export LC_ALL="en_US.UTF-8"
+    export LC_CTYPE="en_US.UTF-8"
+    sudo dpkg-reconfigure locales
 
     # if qsv is already installed, be sure to update it to the latest release
     sudo qsvdp --update
 
-    # ensure datapusher-plus and uwsgi are installed in the virtual environment
+    # install datapusher-plus in the virtual environment
     . /usr/lib/ckan/dpplus_venv/bin/activate
     pip3 install datapusher-plus
 
-    # generate a settings file and tune it, as well as a uwsgi ini file
+    # create an .env file and tune DP+ settings. Tune the uwsgi.ini file as well
     sudo mkdir -p /etc/ckan/datapusher-plus
-    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/settings.py -o /etc/ckan/datapusher-plus/settings.py
-    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/.env -o /etc/ckan/datapusher-plus/.env
+    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/dot-env.template -o /etc/ckan/datapusher-plus/.env
     sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/deployment/datapusher-uwsgi.ini -o /etc/ckan/datapusher-plus/uwsgi.ini
 
     # Be sure to initialize the database if required. (See Database Setup section below)
-    # Be sure to the .env and settings.py files have the right connect strings!
+    # Be sure to the .env file have the right connect strings!
 
     # Create a user to run the web service (if necessary)
     sudo addgroup www-data
     sudo adduser -G www-data www-data
 
 At this point you can run DataPusher+ with the following command:
 
@@ -262,43 +268,20 @@
 >```
 > ["TAB", "Tab Separated Values File", "text/tab-separated-values", []],
 >```
 
 
 ### DataPusher+ Configuration
 
-The DataPusher+ instance is configured in the `config_local.py`
-file. The location of this file can be adjusted using the `JOB_CONFIG`
-environment variable which should provide an absolute path to a python-formatted
-config file.
-
-Here's a summary of the options available.
-
-| Name | Default | Description |
-| -- | -- | -- |
-| HOST | '0.0.0.0' | Web server host |
-| PORT | 8800 | Web server port |
-| SQLALCHEMY_DATABASE_URI | 'postgresql://datapusher_jobs:<br/>YOURPASSWORD<br/>@localhost/datapusher_jobs' | SQLAlchemy Database URL. See note below about setting up the `datapusher_jobs` db beforehand. |
-| MAX_CONTENT_LENGTH | '1024000' | Max size of files to process in bytes |
-| CHUNK_SIZE | '16384' | Chunk size when processing the data file |
-| DOWNLOAD_TIMEOUT | '30' | Download timeout for requesting the file |
-| SSL_VERIFY | False | Do not validate SSL certificates when requesting the data file (*Warning*: Do not use this setting in production) |
-| TYPES | 'String', 'Float', 'Integer', 'DateTime', 'Date', 'NULL' | These are the types that qsv can infer. |
-| TYPE_MAPPING | {'String': 'text', 'Integer': 'numeric', 'Float': 'numeric', 'DateTime': 'timestamp', 'Date': 'timestamp', 'NULL': 'text'} | Internal qsv type mapping to PostgreSQL types |
-| LOG_FILE | `/tmp/ckan_service.log` | Where to write the logs. Use an empty string to disable |
-| STDERR | `True` | Log to stderr? |
-| QSV_BIN | /usr/local/bin/qsvdp | The location of the qsv binary to use. qsvdp is the DP+ optimized version of qsv. It only has the commands used by DP+, has the self-update engine removed, and is 6x smaller than qsv and 3x smaller than qsvlite. You may also want to look into using `qsvdp_nightly`, for even more performance. |
-| PREVIEW_ROWS | 1000 | The number of rows to insert to the data store. Set to 0 to insert all rows |
-| QSV_DEDUP | `True` | Automatically deduplicate rows? |
-| DEFAULT_EXCEL_SHEET | 0 | The zero-based index of the Excel sheet to export to CSV and insert into the Datastore. Negative values are accepted, i.e. -1 is the last sheet, -2 is 2nd to the last, etc. |
-| AUTO_ALIAS | `True` | Automatically create a resource alias - RESOURCE_NAME-PACKAGE_NAME-OWNER_ORG, that's easier to use in API calls and with the scheming datastore_choices helper |
-| WRITE_ENGINE_URL | | The Postgres connection string to use to write to the Datastore using Postgres COPY. This should be **similar** to your `ckan.datastore.write_url`, except you'll need to use the `datapusher` user |
+The DataPusher+ instance is configured in the `.env` file located in the working directory of DP+
+(`/etc/ckan/datapusher-plus` when running a production deployment. The root of the datapusher-plus
+source directory when running a development installation.)
+
+See [dot-env.template](datapusher/dot-env.template) for a summary of configuration options available.
 
-All of the configuration options above can be also provided as environment
-variables, which can be set by setting key-value pairs in a `.env` file. For variables with boolean values you must use `1` or `0`.
 
 ### DataPusher+ Database Setup
 
 DP+ requires a dedicated PostgreSQL account named `datapusher` to connect to the CKAN Datastore.
 
 To create the `datapusher` user and give it the required privileges to the `datastore_default` database:
```

### Comparing `datapusher-plus-0.8.0/README.md` & `datapusher-plus-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 [ckanext-xloader](https://github.com/ckan/ckanext-xloader) with the data type guessing of Datapusher.
 
 Datapusher+ is built using [CKAN Service Provider][], with [Messytables] replaced by [qsv].
 
 [TNRIS](https://tnris.org)/[TWDB](https://www.twdb.texas.gov/) provided the use cases that informed and supported the development
 of Datapusher+, specifically, to support a [Resource-first upload workflow](docs/RESOURCE_FIRST_WORKFLOW.md#Resource-first-Upload-Workflow).
 
+For a more detailed overview, see the [CKAN Monthly Live Jan 2023 presentation](https://docs.google.com/presentation/d/e/2PACX-1vT0BfmrrtaEINRGg4UI_m7B02_X6HlFr4yN_DXmgX9goVtgu2DNmZjl-SowL9ZA2ibQhDjScRRJh95q/pub?start=false&loop=false&delayms=3000).
+
 It features:
 
 * **"Bullet-proof", ultra-fast data type inferencing with qsv**
 
   Unlike [Messytables][] which scans only the the first few rows to guess the type of
   a column, [qsv][] scans the entire table so its data type inferences are guaranteed[^1].
 
@@ -108,17 +110,17 @@
     pip install -e .
 
 Install qsv:
 
 [Download the appropriate precompiled binaries](https://github.com/jqnatividad/qsv/releases/latest) for your platform and copy
 it to the appropriate directory, e.g. for Linux:
 
-    wget https://github.com/jqnatividad/qsv/releases/download/0.84.0/qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    unzip qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    rm qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    wget https://github.com/jqnatividad/qsv/releases/download/0.87.0/qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    unzip qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    rm qsv-0.87.0-x86_64-unknown-linux-gnu.zip
     sudo mv qsv* /usr/local/bin
 
 Alternatively, if you want to install qsv from source, follow
 the instructions [here](https://github.com/jqnatividad/qsv#installation). Note that when compiling from source,
 you may want to look into the [Performance Tuning](https://github.com/jqnatividad/qsv#performance-tuning)
 section to squeeze even more performance from qsv.
 
@@ -130,23 +132,23 @@
     qsvdp --update
 
 
 > ℹ️ **NOTE:** qsv is a general purpose CSV data-wrangling toolkit that gets regular updates. To update to the latest version, just run
 qsv with the `--update` option and it will check for the latest version and update as required.
 
 
-Copy `datapusher/config.py` to a new file like `config_local.py` and modify your configuration as required.
+Copy the `datapusher/dot-env.template` to file `datapusher/.env` and modify your configuration as required.
 Make sure to create the `datapusher` PostgreSQL user and the `datapusher_jobs` database (see [DataPusher+ Database Setup](#DataPusher+_Database_Setup)).
 
     cd datapusher
-    cp config.py config_local.py
+    cp dot-env.template .env
     # configure your installation as required
-    nano config_local.py
+    nano .env
 
-    python3 datapusher/main.py datapusher/config_local.py
+    python3 datapusher/main.py datapusher/config.py
 
 By default, DataPusher+ should be running at the following port:
 
     http://localhost:8800/
 
 ## Production deployment
 
@@ -162,41 +164,45 @@
 can be easily adapted to other WSGI servers like Gunicorn. You'll probably need
 to set up Nginx as a reverse proxy in front of it and something like Supervisor
 to keep the process up.
 
 
     # Install requirements for DataPusher+. Be sure to have at least Python 3.8
     sudo apt install python3-venv python3-dev build-essential libxslt1-dev libxml2-dev libffi-dev
-
+     
     cd /usr/lib/ckan
 
     # Create a virtualenv for DataPusher+. DP+ requires at least python 3.8.
     sudo python3.8 -m venv /usr/lib/ckan/dpplus_venv
 
     # Install qsv binary, if required
-    wget https://github.com/jqnatividad/qsv/releases/download/0.84.0/qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    unzip qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    wget https://github.com/jqnatividad/qsv/releases/download/0.87.0/qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    unzip qsv-0.87.0-x86_64-unknown-linux-gnu.zip
     sudo mv qsv* /usr/local/bin
-    rm qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    rm qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    
+    # Set Locales
+    export LC_ALL="en_US.UTF-8"
+    export LC_CTYPE="en_US.UTF-8"
+    sudo dpkg-reconfigure locales
 
     # if qsv is already installed, be sure to update it to the latest release
     sudo qsvdp --update
 
-    # ensure datapusher-plus and uwsgi are installed in the virtual environment
+    # install datapusher-plus in the virtual environment
     . /usr/lib/ckan/dpplus_venv/bin/activate
     pip3 install datapusher-plus
 
-    # generate a settings file and tune it, as well as a uwsgi ini file
+    # create an .env file and tune DP+ settings. Tune the uwsgi.ini file as well
     sudo mkdir -p /etc/ckan/datapusher-plus
-    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/settings.py -o /etc/ckan/datapusher-plus/settings.py
-    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/.env -o /etc/ckan/datapusher-plus/.env
+    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/dot-env.template -o /etc/ckan/datapusher-plus/.env
     sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/deployment/datapusher-uwsgi.ini -o /etc/ckan/datapusher-plus/uwsgi.ini
 
     # Be sure to initialize the database if required. (See Database Setup section below)
-    # Be sure to the .env and settings.py files have the right connect strings!
+    # Be sure to the .env file have the right connect strings!
 
     # Create a user to run the web service (if necessary)
     sudo addgroup www-data
     sudo adduser -G www-data www-data
 
 At this point you can run DataPusher+ with the following command:
 
@@ -247,43 +253,20 @@
 >```
 > ["TAB", "Tab Separated Values File", "text/tab-separated-values", []],
 >```
 
 
 ### DataPusher+ Configuration
 
-The DataPusher+ instance is configured in the `config_local.py`
-file. The location of this file can be adjusted using the `JOB_CONFIG`
-environment variable which should provide an absolute path to a python-formatted
-config file.
-
-Here's a summary of the options available.
-
-| Name | Default | Description |
-| -- | -- | -- |
-| HOST | '0.0.0.0' | Web server host |
-| PORT | 8800 | Web server port |
-| SQLALCHEMY_DATABASE_URI | 'postgresql://datapusher_jobs:<br/>YOURPASSWORD<br/>@localhost/datapusher_jobs' | SQLAlchemy Database URL. See note below about setting up the `datapusher_jobs` db beforehand. |
-| MAX_CONTENT_LENGTH | '1024000' | Max size of files to process in bytes |
-| CHUNK_SIZE | '16384' | Chunk size when processing the data file |
-| DOWNLOAD_TIMEOUT | '30' | Download timeout for requesting the file |
-| SSL_VERIFY | False | Do not validate SSL certificates when requesting the data file (*Warning*: Do not use this setting in production) |
-| TYPES | 'String', 'Float', 'Integer', 'DateTime', 'Date', 'NULL' | These are the types that qsv can infer. |
-| TYPE_MAPPING | {'String': 'text', 'Integer': 'numeric', 'Float': 'numeric', 'DateTime': 'timestamp', 'Date': 'timestamp', 'NULL': 'text'} | Internal qsv type mapping to PostgreSQL types |
-| LOG_FILE | `/tmp/ckan_service.log` | Where to write the logs. Use an empty string to disable |
-| STDERR | `True` | Log to stderr? |
-| QSV_BIN | /usr/local/bin/qsvdp | The location of the qsv binary to use. qsvdp is the DP+ optimized version of qsv. It only has the commands used by DP+, has the self-update engine removed, and is 6x smaller than qsv and 3x smaller than qsvlite. You may also want to look into using `qsvdp_nightly`, for even more performance. |
-| PREVIEW_ROWS | 1000 | The number of rows to insert to the data store. Set to 0 to insert all rows |
-| QSV_DEDUP | `True` | Automatically deduplicate rows? |
-| DEFAULT_EXCEL_SHEET | 0 | The zero-based index of the Excel sheet to export to CSV and insert into the Datastore. Negative values are accepted, i.e. -1 is the last sheet, -2 is 2nd to the last, etc. |
-| AUTO_ALIAS | `True` | Automatically create a resource alias - RESOURCE_NAME-PACKAGE_NAME-OWNER_ORG, that's easier to use in API calls and with the scheming datastore_choices helper |
-| WRITE_ENGINE_URL | | The Postgres connection string to use to write to the Datastore using Postgres COPY. This should be **similar** to your `ckan.datastore.write_url`, except you'll need to use the `datapusher` user |
+The DataPusher+ instance is configured in the `.env` file located in the working directory of DP+
+(`/etc/ckan/datapusher-plus` when running a production deployment. The root of the datapusher-plus
+source directory when running a development installation.)
+
+See [dot-env.template](datapusher/dot-env.template) for a summary of configuration options available.
 
-All of the configuration options above can be also provided as environment
-variables, which can be set by setting key-value pairs in a `.env` file. For variables with boolean values you must use `1` or `0`.
 
 ### DataPusher+ Database Setup
 
 DP+ requires a dedicated PostgreSQL account named `datapusher` to connect to the CKAN Datastore.
 
 To create the `datapusher` user and give it the required privileges to the `datastore_default` database:
```

### Comparing `datapusher-plus-0.8.0/datapusher/config.py` & `datapusher-plus-0.9.0/datapusher/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,26 +44,33 @@
     MAX_CONTENT_LENGTH: str = "25600000"
     IGNORE_FILE_HASH: bool = True
     CHUNK_SIZE: str = "16384"
     DOWNLOAD_TIMEOUT: int = 30
     SSL_VERIFY: bool = False
     TYPES: tuple = _TYPES
     TYPE_MAPPING: dict = _TYPE_MAPPING
+    PII_SCREENING: bool = True
+    PII_QUICK_SCREEN: bool = True
+    PII_FOUND_ABORT: bool = True
+    PII_SHOW_CANDIDATES: bool = True
+    PII_REGEX_RESOURCE_ID_OR_ALIAS: str = ""
     LOG_FILE: str = "/etc/ckan/datapusher-plus/ckan_service.log"
     STDERR: bool = True
     QSV_BIN: str = "/usr/local/bin/qsvdp"
     FILE_BIN: str = "/usr/bin/file"
     PREFER_DMY: bool = False
     PREVIEW_ROWS: int = 1000
     DOWNLOAD_PREVIEW_ONLY: bool = False
     AUTO_INDEX_THRESHOLD: int = 3
     AUTO_INDEX_DATES: bool = True
+    SORT_AND_DUPE_CHECK: bool = True
     DEDUP: bool = False
     DEFAULT_EXCEL_SHEET: int = 0
     ADD_SUMMARY_STATS_RESOURCE: bool = True
+    SUMMARY_STATS_WITH_PREVIEW: bool = False
     SUMMARY_STATS_OPTIONS: str = "--everything"
     AUTO_ALIAS: bool = True
     AUTO_ALIAS_UNIQUE: bool = False
     WRITE_ENGINE_URL: str = _WRITE_ENGINE_URL
     DOWNLOAD_PROXY: str = ""
 
     """
```

### Comparing `datapusher-plus-0.8.0/datapusher/config_local.py` & `datapusher-plus-0.9.0/datapusher/config_local.py`

 * *Files identical despite different names*

### Comparing `datapusher-plus-0.8.0/datapusher/jobs.py` & `datapusher-plus-0.9.0/datapusher/jobs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,3176 +1,4138 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
 00000010: 662d 3820 2d2a 2d0a 0a69 6d70 6f72 7420  f-8 -*-..import 
 00000020: 6a73 6f6e 0a69 6d70 6f72 7420 7265 7175  json.import requ
-00000030: 6573 7473 0a0a 7472 793a 0a20 2020 2066  ests..try:.    f
-00000040: 726f 6d20 7572 6c6c 6962 2e70 6172 7365  rom urllib.parse
-00000050: 2069 6d70 6f72 7420 7572 6c73 706c 6974   import urlsplit
-00000060: 0a65 7863 6570 7420 496d 706f 7274 4572  .except ImportEr
-00000070: 726f 723a 0a20 2020 2066 726f 6d20 7572  ror:.    from ur
-00000080: 6c70 6172 7365 2069 6d70 6f72 7420 7572  lparse import ur
-00000090: 6c73 706c 6974 0a0a 696d 706f 7274 2069  lsplit..import i
-000000a0: 7465 7274 6f6f 6c73 0a69 6d70 6f72 7420  tertools.import 
-000000b0: 6461 7465 7469 6d65 0a69 6d70 6f72 7420  datetime.import 
-000000c0: 6c6f 6361 6c65 0a69 6d70 6f72 7420 6c6f  locale.import lo
-000000d0: 6767 696e 670a 696d 706f 7274 2064 6563  gging.import dec
-000000e0: 696d 616c 0a69 6d70 6f72 7420 6861 7368  imal.import hash
-000000f0: 6c69 620a 696d 706f 7274 2074 696d 650a  lib.import time.
-00000100: 696d 706f 7274 2074 656d 7066 696c 650a  import tempfile.
-00000110: 696d 706f 7274 2073 7562 7072 6f63 6573  import subproces
-00000120: 730a 696d 706f 7274 2063 7376 0a69 6d70  s.import csv.imp
-00000130: 6f72 7420 6f73 0a69 6d70 6f72 7420 7073  ort os.import ps
-00000140: 7963 6f70 6732 0a66 726f 6d20 7061 7468  ycopg2.from path
-00000150: 6c69 6220 696d 706f 7274 2050 6174 680a  lib import Path.
-00000160: 6672 6f6d 2064 6174 6173 697a 6520 696d  from datasize im
-00000170: 706f 7274 2044 6174 6153 697a 650a 6672  port DataSize.fr
-00000180: 6f6d 2070 7379 636f 7067 3220 696d 706f  om psycopg2 impo
-00000190: 7274 2073 716c 0a0a 696d 706f 7274 2063  rt sql..import c
-000001a0: 6b61 6e73 6572 7669 6365 7072 6f76 6964  kanserviceprovid
-000001b0: 6572 2e6a 6f62 2061 7320 6a6f 620a 696d  er.job as job.im
-000001c0: 706f 7274 2063 6b61 6e73 6572 7669 6365  port ckanservice
-000001d0: 7072 6f76 6964 6572 2e75 7469 6c20 6173  provider.util as
-000001e0: 2075 7469 6c0a 6672 6f6d 2063 6b61 6e73   util.from ckans
-000001f0: 6572 7669 6365 7072 6f76 6964 6572 2069  erviceprovider i
-00000200: 6d70 6f72 7420 7765 620a 6672 6f6d 2064  mport web.from d
-00000210: 6174 6170 7573 6865 722e 636f 6e66 6967  atapusher.config
-00000220: 2069 6d70 6f72 7420 636f 6e66 6967 0a0a   import config..
-00000230: 0a69 6620 6c6f 6361 6c65 2e67 6574 6465  .if locale.getde
-00000240: 6661 756c 746c 6f63 616c 6528 295b 305d  faultlocale()[0]
-00000250: 3a0a 2020 2020 6c61 6e67 2c20 656e 636f  :.    lang, enco
-00000260: 6469 6e67 203d 206c 6f63 616c 652e 6765  ding = locale.ge
-00000270: 7464 6566 6175 6c74 6c6f 6361 6c65 2829  tdefaultlocale()
+00000030: 6573 7473 0a0a 6672 6f6d 2075 726c 6c69  ests..from urlli
+00000040: 622e 7061 7273 6520 696d 706f 7274 2075  b.parse import u
+00000050: 726c 7370 6c69 740a 696d 706f 7274 2064  rlsplit.import d
+00000060: 6174 6574 696d 650a 696d 706f 7274 206c  atetime.import l
+00000070: 6f63 616c 650a 696d 706f 7274 206c 6f67  ocale.import log
+00000080: 6769 6e67 0a69 6d70 6f72 7420 6465 6369  ging.import deci
+00000090: 6d61 6c0a 696d 706f 7274 2068 6173 686c  mal.import hashl
+000000a0: 6962 0a69 6d70 6f72 7420 7469 6d65 0a69  ib.import time.i
+000000b0: 6d70 6f72 7420 7465 6d70 6669 6c65 0a69  mport tempfile.i
+000000c0: 6d70 6f72 7420 7375 6270 726f 6365 7373  mport subprocess
+000000d0: 0a69 6d70 6f72 7420 6373 760a 696d 706f  .import csv.impo
+000000e0: 7274 206f 730a 696d 706f 7274 2070 7379  rt os.import psy
+000000f0: 636f 7067 320a 696d 706f 7274 2073 656d  copg2.import sem
+00000100: 7665 720a 6672 6f6d 2070 6174 686c 6962  ver.from pathlib
+00000110: 2069 6d70 6f72 7420 5061 7468 0a66 726f   import Path.fro
+00000120: 6d20 6461 7461 7369 7a65 2069 6d70 6f72  m datasize impor
+00000130: 7420 4461 7461 5369 7a65 0a66 726f 6d20  t DataSize.from 
+00000140: 7073 7963 6f70 6732 2069 6d70 6f72 7420  psycopg2 import 
+00000150: 7371 6c0a 0a69 6d70 6f72 7420 636b 616e  sql..import ckan
+00000160: 7365 7276 6963 6570 726f 7669 6465 722e  serviceprovider.
+00000170: 6a6f 6220 6173 206a 6f62 0a69 6d70 6f72  job as job.impor
+00000180: 7420 636b 616e 7365 7276 6963 6570 726f  t ckanservicepro
+00000190: 7669 6465 722e 7574 696c 2061 7320 7574  vider.util as ut
+000001a0: 696c 0a66 726f 6d20 636b 616e 7365 7276  il.from ckanserv
+000001b0: 6963 6570 726f 7669 6465 7220 696d 706f  iceprovider impo
+000001c0: 7274 2077 6562 0a66 726f 6d20 6461 7461  rt web.from data
+000001d0: 7075 7368 6572 2e63 6f6e 6669 6720 696d  pusher.config im
+000001e0: 706f 7274 2063 6f6e 6669 670a 0a0a 6966  port config...if
+000001f0: 206c 6f63 616c 652e 6765 7464 6566 6175   locale.getdefau
+00000200: 6c74 6c6f 6361 6c65 2829 5b30 5d3a 0a20  ltlocale()[0]:. 
+00000210: 2020 206c 616e 672c 2065 6e63 6f64 696e     lang, encodin
+00000220: 6720 3d20 6c6f 6361 6c65 2e67 6574 6465  g = locale.getde
+00000230: 6661 756c 746c 6f63 616c 6528 290a 2020  faultlocale().  
+00000240: 2020 6c6f 6361 6c65 2e73 6574 6c6f 6361    locale.setloca
+00000250: 6c65 286c 6f63 616c 652e 4c43 5f41 4c4c  le(locale.LC_ALL
+00000260: 2c20 6c6f 6361 6c65 3d28 6c61 6e67 2c20  , locale=(lang, 
+00000270: 656e 636f 6469 6e67 2929 0a65 6c73 653a  encoding)).else:
 00000280: 0a20 2020 206c 6f63 616c 652e 7365 746c  .    locale.setl
 00000290: 6f63 616c 6528 6c6f 6361 6c65 2e4c 435f  ocale(locale.LC_
-000002a0: 414c 4c2c 206c 6f63 616c 653d 286c 616e  ALL, locale=(lan
-000002b0: 672c 2065 6e63 6f64 696e 6729 290a 656c  g, encoding)).el
-000002c0: 7365 3a0a 2020 2020 6c6f 6361 6c65 2e73  se:.    locale.s
-000002d0: 6574 6c6f 6361 6c65 286c 6f63 616c 652e  etlocale(locale.
-000002e0: 4c43 5f41 4c4c 2c20 2222 290a 0a55 5345  LC_ALL, "")..USE
-000002f0: 5f50 524f 5859 203d 2022 444f 574e 4c4f  _PROXY = "DOWNLO
-00000300: 4144 5f50 524f 5859 2220 696e 2063 6f6e  AD_PROXY" in con
-00000310: 6669 670a 6966 2055 5345 5f50 524f 5859  fig.if USE_PROXY
-00000320: 3a0a 2020 2020 444f 574e 4c4f 4144 5f50  :.    DOWNLOAD_P
-00000330: 524f 5859 203d 2063 6f6e 6669 672e 6765  ROXY = config.ge
-00000340: 7428 2244 4f57 4e4c 4f41 445f 5052 4f58  t("DOWNLOAD_PROX
-00000350: 5922 290a 0a69 6620 6e6f 7420 636f 6e66  Y")..if not conf
-00000360: 6967 2e67 6574 2822 5353 4c5f 5645 5249  ig.get("SSL_VERI
-00000370: 4659 2229 3a0a 2020 2020 7265 7175 6573  FY"):.    reques
-00000380: 7473 2e70 6163 6b61 6765 732e 7572 6c6c  ts.packages.urll
-00000390: 6962 332e 6469 7361 626c 655f 7761 726e  ib3.disable_warn
-000003a0: 696e 6773 2829 0a0a 504f 5354 4752 4553  ings()..POSTGRES
-000003b0: 5f49 4e54 5f4d 4158 203d 2032 3134 3734  _INT_MAX = 21474
-000003c0: 3833 3634 370a 504f 5354 4752 4553 5f49  83647.POSTGRES_I
-000003d0: 4e54 5f4d 494e 203d 202d 3231 3437 3438  NT_MIN = -214748
-000003e0: 3336 3438 0a50 4f53 5447 5245 535f 4249  3648.POSTGRES_BI
-000003f0: 4749 4e54 5f4d 4158 203d 2039 3232 3333  GINT_MAX = 92233
-00000400: 3732 3033 3638 3534 3737 3538 3037 0a50  72036854775807.P
-00000410: 4f53 5447 5245 535f 4249 4749 4e54 5f4d  OSTGRES_BIGINT_M
-00000420: 494e 203d 202d 3932 3233 3337 3230 3336  IN = -9223372036
-00000430: 3835 3437 3735 3830 380a 0a44 4154 4153  854775808..DATAS
-00000440: 544f 5245 5f55 524c 5320 3d20 7b0a 2020  TORE_URLS = {.  
-00000450: 2020 2264 6174 6173 746f 7265 5f64 656c    "datastore_del
-00000460: 6574 6522 3a20 227b 636b 616e 5f75 726c  ete": "{ckan_url
-00000470: 7d2f 6170 692f 6163 7469 6f6e 2f64 6174  }/api/action/dat
-00000480: 6173 746f 7265 5f64 656c 6574 6522 2c0a  astore_delete",.
-00000490: 2020 2020 2272 6573 6f75 7263 655f 7570      "resource_up
-000004a0: 6461 7465 223a 2022 7b63 6b61 6e5f 7572  date": "{ckan_ur
-000004b0: 6c7d 2f61 7069 2f61 6374 696f 6e2f 7265  l}/api/action/re
-000004c0: 736f 7572 6365 5f75 7064 6174 6522 2c0a  source_update",.
-000004d0: 7d0a 0a0a 636c 6173 7320 4854 5450 4572  }...class HTTPEr
-000004e0: 726f 7228 7574 696c 2e4a 6f62 4572 726f  ror(util.JobErro
-000004f0: 7229 3a0a 2020 2020 2222 2245 7863 6570  r):.    """Excep
-00000500: 7469 6f6e 2074 6861 7427 7320 7261 6973  tion that's rais
-00000510: 6564 2069 6620 6120 6a6f 6220 6661 696c  ed if a job fail
-00000520: 7320 6475 6520 746f 2061 6e20 4854 5450  s due to an HTTP
-00000530: 2070 726f 626c 656d 2e22 2222 0a0a 2020   problem."""..  
-00000540: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00000550: 656c 662c 206d 6573 7361 6765 2c20 7374  elf, message, st
-00000560: 6174 7573 5f63 6f64 652c 2072 6571 7565  atus_code, reque
-00000570: 7374 5f75 726c 2c20 7265 7370 6f6e 7365  st_url, response
-00000580: 293a 0a20 2020 2020 2020 2022 2222 496e  ):.        """In
-00000590: 6974 6961 6c69 7365 2061 206e 6577 2048  itialise a new H
-000005a0: 5454 5045 7272 6f72 2e0a 0a20 2020 2020  TTPError...     
-000005b0: 2020 203a 7061 7261 6d20 6d65 7373 6167     :param messag
-000005c0: 653a 2041 2068 756d 616e 2d72 6561 6461  e: A human-reada
-000005d0: 626c 6520 6572 726f 7220 6d65 7373 6167  ble error messag
-000005e0: 650a 2020 2020 2020 2020 3a74 7970 6520  e.        :type 
-000005f0: 6d65 7373 6167 653a 2073 7472 696e 670a  message: string.
-00000600: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000610: 7374 6174 7573 5f63 6f64 653a 2054 6865  status_code: The
-00000620: 2073 7461 7475 7320 636f 6465 206f 6620   status code of 
-00000630: 7468 6520 6572 726f 7265 6420 4854 5450  the errored HTTP
-00000640: 2072 6573 706f 6e73 652c 0a20 2020 2020   response,.     
-00000650: 2020 2020 2020 2065 2e67 2e20 3530 300a         e.g. 500.
-00000660: 2020 2020 2020 2020 3a74 7970 6520 7374          :type st
-00000670: 6174 7573 5f63 6f64 653a 2069 6e74 0a0a  atus_code: int..
-00000680: 2020 2020 2020 2020 3a70 6172 616d 2072          :param r
-00000690: 6571 7565 7374 5f75 726c 3a20 5468 6520  equest_url: The 
-000006a0: 5552 4c20 7468 6174 2077 6173 2072 6571  URL that was req
-000006b0: 7565 7374 6564 0a20 2020 2020 2020 203a  uested.        :
-000006c0: 7479 7065 2072 6571 7565 7374 5f75 726c  type request_url
-000006d0: 3a20 7374 7269 6e67 0a0a 2020 2020 2020  : string..      
-000006e0: 2020 3a70 6172 616d 2072 6573 706f 6e73    :param respons
-000006f0: 653a 2054 6865 2062 6f64 7920 6f66 2074  e: The body of t
-00000700: 6865 2065 7272 6f72 6564 2048 5454 5020  he errored HTTP 
-00000710: 7265 7370 6f6e 7365 2061 7320 756e 6963  response as unic
-00000720: 6f64 650a 2020 2020 2020 2020 2020 2020  ode.            
-00000730: 2869 6620 796f 7520 6861 7665 2061 2072  (if you have a r
-00000740: 6571 7565 7374 732e 5265 7370 6f6e 7365  equests.Response
-00000750: 206f 626a 6563 7420 7468 656e 2072 6573   object then res
-00000760: 706f 6e73 652e 7465 7874 2077 696c 6c0a  ponse.text will.
-00000770: 2020 2020 2020 2020 2020 2020 6769 7665              give
-00000780: 2079 6f75 2074 6869 7329 0a20 2020 2020   you this).     
-00000790: 2020 203a 7479 7065 2072 6573 706f 6e73     :type respons
-000007a0: 653a 2075 6e69 636f 6465 0a0a 2020 2020  e: unicode..    
-000007b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000007c0: 7375 7065 7228 4854 5450 4572 726f 722c  super(HTTPError,
-000007d0: 2073 656c 6629 2e5f 5f69 6e69 745f 5f28   self).__init__(
-000007e0: 6d65 7373 6167 6529 0a20 2020 2020 2020  message).       
-000007f0: 2073 656c 662e 7374 6174 7573 5f63 6f64   self.status_cod
-00000800: 6520 3d20 7374 6174 7573 5f63 6f64 650a  e = status_code.
-00000810: 2020 2020 2020 2020 7365 6c66 2e72 6571          self.req
-00000820: 7565 7374 5f75 726c 203d 2072 6571 7565  uest_url = reque
-00000830: 7374 5f75 726c 0a20 2020 2020 2020 2073  st_url.        s
-00000840: 656c 662e 7265 7370 6f6e 7365 203d 2072  elf.response = r
-00000850: 6573 706f 6e73 650a 0a20 2020 2064 6566  esponse..    def
-00000860: 2061 735f 6469 6374 2873 656c 6629 3a0a   as_dict(self):.
-00000870: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
-00000880: 6e20 6120 4a53 4f4e 2d73 6572 6961 6c69  n a JSON-seriali
-00000890: 7a61 626c 6520 6469 6374 696f 6e61 7279  zable dictionary
-000008a0: 2072 6570 7265 7365 6e74 6174 696f 6e20   representation 
-000008b0: 6f66 2074 6869 7320 6572 726f 722e 0a0a  of this error...
-000008c0: 2020 2020 2020 2020 5375 6974 6162 6c65          Suitable
-000008d0: 2066 6f72 2063 6b61 6e73 6572 7669 6365   for ckanservice
-000008e0: 7072 6f76 6964 6572 2074 6f20 7265 7475  provider to retu
-000008f0: 726e 2074 6f20 7468 6520 636c 6965 6e74  rn to the client
-00000900: 2073 6974 6520 6173 2074 6865 0a20 2020   site as the.   
-00000910: 2020 2020 2076 616c 7565 2066 6f72 2074       value for t
-00000920: 6865 2022 6572 726f 7222 206b 6579 2069  he "error" key i
-00000930: 6e20 7468 6520 6a6f 6220 6469 6374 2e0a  n the job dict..
-00000940: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00000950: 2020 2020 2069 6620 7365 6c66 2e72 6573       if self.res
-00000960: 706f 6e73 6520 616e 6420 6c65 6e28 7365  ponse and len(se
-00000970: 6c66 2e72 6573 706f 6e73 6529 203e 2032  lf.response) > 2
-00000980: 3030 3a0a 2020 2020 2020 2020 2020 2020  00:.            
-00000990: 7265 7370 6f6e 7365 203d 2073 656c 662e  response = self.
-000009a0: 7265 7370 6f6e 7365 5b3a 3230 305d 0a20  response[:200]. 
-000009b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000009c0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-000009d0: 6520 3d20 7365 6c66 2e72 6573 706f 6e73  e = self.respons
-000009e0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-000009f0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00000a00: 6d65 7373 6167 6522 3a20 7365 6c66 2e6d  message": self.m
-00000a10: 6573 7361 6765 2c0a 2020 2020 2020 2020  essage,.        
-00000a20: 2020 2020 2248 5454 5020 7374 6174 7573      "HTTP status
-00000a30: 2063 6f64 6522 3a20 7365 6c66 2e73 7461   code": self.sta
-00000a40: 7475 735f 636f 6465 2c0a 2020 2020 2020  tus_code,.      
-00000a50: 2020 2020 2020 2252 6571 7565 7374 6564        "Requested
-00000a60: 2055 524c 223a 2073 656c 662e 7265 7175   URL": self.requ
-00000a70: 6573 745f 7572 6c2c 0a20 2020 2020 2020  est_url,.       
-00000a80: 2020 2020 2022 5265 7370 6f6e 7365 223a       "Response":
-00000a90: 2072 6573 706f 6e73 652c 0a20 2020 2020   response,.     
-00000aa0: 2020 207d 0a0a 2020 2020 6465 6620 5f5f     }..    def __
-00000ab0: 7374 725f 5f28 7365 6c66 293a 0a20 2020  str__(self):.   
-00000ac0: 2020 2020 2072 6574 7572 6e20 227b 7d20       return "{} 
-00000ad0: 7374 6174 7573 3d7b 7d20 7572 6c3d 7b7d  status={} url={}
-00000ae0: 2072 6573 706f 6e73 653d 7b7d 222e 666f   response={}".fo
-00000af0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00000b00: 2020 7365 6c66 2e6d 6573 7361 6765 2c20    self.message, 
-00000b10: 7365 6c66 2e73 7461 7475 735f 636f 6465  self.status_code
-00000b20: 2c20 7365 6c66 2e72 6571 7565 7374 5f75  , self.request_u
-00000b30: 726c 2c20 7365 6c66 2e72 6573 706f 6e73  rl, self.respons
-00000b40: 650a 2020 2020 2020 2020 292e 656e 636f  e.        ).enco
-00000b50: 6465 2822 6173 6369 6922 2c20 2272 6570  de("ascii", "rep
-00000b60: 6c61 6365 2229 0a0a 0a64 6566 2067 6574  lace")...def get
-00000b70: 5f75 726c 2861 6374 696f 6e2c 2063 6b61  _url(action, cka
-00000b80: 6e5f 7572 6c29 3a0a 2020 2020 2222 220a  n_url):.    """.
-00000b90: 2020 2020 4765 7420 7572 6c20 666f 7220      Get url for 
-00000ba0: 636b 616e 2061 6374 696f 6e0a 2020 2020  ckan action.    
-00000bb0: 2222 220a 2020 2020 6966 206e 6f74 2075  """.    if not u
-00000bc0: 726c 7370 6c69 7428 636b 616e 5f75 726c  rlsplit(ckan_url
-00000bd0: 292e 7363 6865 6d65 3a0a 2020 2020 2020  ).scheme:.      
-00000be0: 2020 636b 616e 5f75 726c 203d 2022 6874    ckan_url = "ht
-00000bf0: 7470 3a2f 2f22 202b 2063 6b61 6e5f 7572  tp://" + ckan_ur
-00000c00: 6c2e 6c73 7472 6970 2822 2f22 2920 2023  l.lstrip("/")  #
-00000c10: 2044 6576 536b 696d 3a20 6967 6e6f 7265   DevSkim: ignore
-00000c20: 2044 5331 3337 3133 380a 2020 2020 636b   DS137138.    ck
-00000c30: 616e 5f75 726c 203d 2063 6b61 6e5f 7572  an_url = ckan_ur
-00000c40: 6c2e 7273 7472 6970 2822 2f22 290a 2020  l.rstrip("/").  
-00000c50: 2020 7265 7475 726e 2022 7b63 6b61 6e5f    return "{ckan_
-00000c60: 7572 6c7d 2f61 7069 2f33 2f61 6374 696f  url}/api/3/actio
-00000c70: 6e2f 7b61 6374 696f 6e7d 222e 666f 726d  n/{action}".form
-00000c80: 6174 2863 6b61 6e5f 7572 6c3d 636b 616e  at(ckan_url=ckan
-00000c90: 5f75 726c 2c20 6163 7469 6f6e 3d61 6374  _url, action=act
-00000ca0: 696f 6e29 0a0a 0a64 6566 2063 6865 636b  ion)...def check
-00000cb0: 5f72 6573 706f 6e73 6528 0a20 2020 2072  _response(.    r
-00000cc0: 6573 706f 6e73 652c 2072 6571 7565 7374  esponse, request
-00000cd0: 5f75 726c 2c20 7768 6f2c 2067 6f6f 645f  _url, who, good_
-00000ce0: 7374 6174 7573 3d28 3230 312c 2032 3030  status=(201, 200
-00000cf0: 292c 2069 676e 6f72 655f 6e6f 5f73 7563  ), ignore_no_suc
-00000d00: 6365 7373 3d46 616c 7365 0a29 3a0a 2020  cess=False.):.  
-00000d10: 2020 2222 220a 2020 2020 4368 6563 6b73    """.    Checks
-00000d20: 2074 6865 2072 6573 706f 6e73 6520 616e   the response an
-00000d30: 6420 7261 6973 6573 2065 7863 6570 7469  d raises excepti
-00000d40: 6f6e 7320 6966 2073 6f6d 6574 6869 6e67  ons if something
-00000d50: 2077 656e 7420 7465 7272 6962 6c79 2077   went terribly w
-00000d60: 726f 6e67 0a0a 2020 2020 3a70 6172 616d  rong..    :param
-00000d70: 2077 686f 3a20 4120 7368 6f72 7420 6e61   who: A short na
-00000d80: 6d65 2074 6861 7420 696e 6469 6361 7465  me that indicate
-00000d90: 6420 7768 6572 6520 7468 6520 6572 726f  d where the erro
-00000da0: 7220 6f63 6375 7272 6564 0a20 2020 2020  r occurred.     
-00000db0: 2020 2020 2020 2020 2020 2028 666f 7220             (for 
-00000dc0: 6578 616d 706c 6520 2243 4b41 4e22 290a  example "CKAN").
-00000dd0: 2020 2020 3a70 6172 616d 2067 6f6f 645f      :param good_
-00000de0: 7374 6174 7573 3a20 5374 6174 7573 2063  status: Status c
-00000df0: 6f64 6573 2074 6861 7420 7368 6f75 6c64  odes that should
-00000e00: 206e 6f74 2072 6169 7365 2061 6e20 6578   not raise an ex
-00000e10: 6365 7074 696f 6e0a 0a20 2020 2022 2222  ception..    """
-00000e20: 0a20 2020 2069 6620 6e6f 7420 7265 7370  .    if not resp
-00000e30: 6f6e 7365 2e73 7461 7475 735f 636f 6465  onse.status_code
-00000e40: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00000e50: 4854 5450 4572 726f 7228 0a20 2020 2020  HTTPError(.     
-00000e60: 2020 2020 2020 2022 4461 7461 5075 7368         "DataPush
-00000e70: 6572 2072 6563 6569 7665 6420 616e 2048  er received an H
-00000e80: 5454 5020 7265 7370 6f6e 7365 2077 6974  TTP response wit
-00000e90: 6820 6e6f 2073 7461 7475 7320 636f 6465  h no status code
-00000ea0: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
-00000eb0: 7461 7475 735f 636f 6465 3d4e 6f6e 652c  tatus_code=None,
-00000ec0: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00000ed0: 7565 7374 5f75 726c 3d72 6571 7565 7374  uest_url=request
-00000ee0: 5f75 726c 2c0a 2020 2020 2020 2020 2020  _url,.          
-00000ef0: 2020 7265 7370 6f6e 7365 3d72 6573 706f    response=respo
-00000f00: 6e73 652e 7465 7874 2c0a 2020 2020 2020  nse.text,.      
-00000f10: 2020 290a 0a20 2020 206d 6573 7361 6765    )..    message
-00000f20: 203d 2022 7b77 686f 7d20 6261 6420 7265   = "{who} bad re
-00000f30: 7370 6f6e 7365 2e20 5374 6174 7573 2063  sponse. Status c
-00000f40: 6f64 653a 207b 636f 6465 7d20 7b72 6561  ode: {code} {rea
-00000f50: 736f 6e7d 2e20 4174 3a20 7b75 726c 7d2e  son}. At: {url}.
-00000f60: 220a 2020 2020 7472 793a 0a20 2020 2020  ".    try:.     
-00000f70: 2020 2069 6620 7265 7370 6f6e 7365 2e73     if response.s
-00000f80: 7461 7475 735f 636f 6465 206e 6f74 2069  tatus_code not i
-00000f90: 6e20 676f 6f64 5f73 7461 7475 733a 0a20  n good_status:. 
-00000fa0: 2020 2020 2020 2020 2020 206a 736f 6e5f             json_
-00000fb0: 7265 7370 6f6e 7365 203d 2072 6573 706f  response = respo
-00000fc0: 6e73 652e 6a73 6f6e 2829 0a20 2020 2020  nse.json().     
-00000fd0: 2020 2020 2020 2069 6620 6e6f 7420 6967         if not ig
-00000fe0: 6e6f 7265 5f6e 6f5f 7375 6363 6573 7320  nore_no_success 
-00000ff0: 6f72 206a 736f 6e5f 7265 7370 6f6e 7365  or json_response
-00001000: 2e67 6574 2822 7375 6363 6573 7322 293a  .get("success"):
-00001010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001020: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00001030: 2020 2020 2020 2020 2020 6d65 7373 6167            messag
-00001040: 6520 3d20 6a73 6f6e 5f72 6573 706f 6e73  e = json_respons
-00001050: 655b 2265 7272 6f72 225d 5b22 6d65 7373  e["error"]["mess
-00001060: 6167 6522 5d0a 2020 2020 2020 2020 2020  age"].          
-00001070: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00001080: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
-00001090: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-000010a0: 6167 6520 3d20 6d65 7373 6167 652e 666f  age = message.fo
-000010b0: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-000010c0: 2020 2020 2020 2020 2020 2020 2020 7768                wh
-000010d0: 6f3d 7768 6f2c 0a20 2020 2020 2020 2020  o=who,.         
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000010f0: 6f64 653d 7265 7370 6f6e 7365 2e73 7461  ode=response.sta
-00001100: 7475 735f 636f 6465 2c0a 2020 2020 2020  tus_code,.      
-00001110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001120: 2020 7265 6173 6f6e 3d72 6573 706f 6e73    reason=respons
-00001130: 652e 7265 6173 6f6e 2c0a 2020 2020 2020  e.reason,.      
-00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001150: 2020 7572 6c3d 7265 7175 6573 745f 7572    url=request_ur
-00001160: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-00001170: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00001180: 2020 2020 2020 2020 2072 6169 7365 2048           raise H
-00001190: 5454 5045 7272 6f72 280a 2020 2020 2020  TTPError(.      
-000011a0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-000011b0: 7373 6167 652c 0a20 2020 2020 2020 2020  ssage,.         
-000011c0: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-000011d0: 735f 636f 6465 3d72 6573 706f 6e73 652e  s_code=response.
-000011e0: 7374 6174 7573 5f63 6f64 652c 0a20 2020  status_code,.   
-000011f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001200: 2072 6571 7565 7374 5f75 726c 3d72 6571   request_url=req
-00001210: 7565 7374 5f75 726c 2c0a 2020 2020 2020  uest_url,.      
-00001220: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001230: 7370 6f6e 7365 3d72 6573 706f 6e73 652e  sponse=response.
-00001240: 7465 7874 2c0a 2020 2020 2020 2020 2020  text,.          
-00001250: 2020 2020 2020 290a 2020 2020 6578 6365        ).    exce
-00001260: 7074 2056 616c 7565 4572 726f 723a 0a20  pt ValueError:. 
-00001270: 2020 2020 2020 206d 6573 7361 6765 203d         message =
-00001280: 206d 6573 7361 6765 2e66 6f72 6d61 7428   message.format(
-00001290: 0a20 2020 2020 2020 2020 2020 2077 686f  .            who
-000012a0: 3d77 686f 2c0a 2020 2020 2020 2020 2020  =who,.          
-000012b0: 2020 636f 6465 3d72 6573 706f 6e73 652e    code=response.
-000012c0: 7374 6174 7573 5f63 6f64 652c 0a20 2020  status_code,.   
-000012d0: 2020 2020 2020 2020 2072 6561 736f 6e3d           reason=
-000012e0: 7265 7370 6f6e 7365 2e72 6561 736f 6e2c  response.reason,
-000012f0: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
-00001300: 3d72 6571 7565 7374 5f75 726c 2c0a 2020  =request_url,.  
-00001310: 2020 2020 2020 2020 2020 7265 7370 3d72            resp=r
-00001320: 6573 706f 6e73 652e 7465 7874 5b3a 3230  esponse.text[:20
-00001330: 305d 2c0a 2020 2020 2020 2020 290a 2020  0],.        ).  
-00001340: 2020 2020 2020 7261 6973 6520 4854 5450        raise HTTP
-00001350: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00001360: 2020 206d 6573 7361 6765 2c0a 2020 2020     message,.    
-00001370: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
-00001380: 6f64 653d 7265 7370 6f6e 7365 2e73 7461  ode=response.sta
-00001390: 7475 735f 636f 6465 2c0a 2020 2020 2020  tus_code,.      
-000013a0: 2020 2020 2020 7265 7175 6573 745f 7572        request_ur
-000013b0: 6c3d 7265 7175 6573 745f 7572 6c2c 0a20  l=request_url,. 
-000013c0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
-000013d0: 6e73 653d 7265 7370 6f6e 7365 2e74 6578  nse=response.tex
-000013e0: 742c 0a20 2020 2020 2020 2029 0a0a 0a63  t,.        )...c
-000013f0: 6c61 7373 2044 6174 6173 746f 7265 456e  lass DatastoreEn
-00001400: 636f 6465 7228 6a73 6f6e 2e4a 534f 4e45  coder(json.JSONE
-00001410: 6e63 6f64 6572 293a 0a20 2020 2023 2043  ncoder):.    # C
-00001420: 7573 746f 6d20 4a53 4f4e 2065 6e63 6f64  ustom JSON encod
-00001430: 6572 0a20 2020 2064 6566 2064 6566 6175  er.    def defau
-00001440: 6c74 2873 656c 662c 206f 626a 293a 0a20  lt(self, obj):. 
-00001450: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00001460: 616e 6365 286f 626a 2c20 6461 7465 7469  ance(obj, dateti
-00001470: 6d65 2e64 6174 6574 696d 6529 3a0a 2020  me.datetime):.  
-00001480: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00001490: 206f 626a 2e69 736f 666f 726d 6174 2829   obj.isoformat()
-000014a0: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-000014b0: 7374 616e 6365 286f 626a 2c20 6465 6369  stance(obj, deci
-000014c0: 6d61 6c2e 4465 6369 6d61 6c29 3a0a 2020  mal.Decimal):.  
-000014d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000014e0: 2073 7472 286f 626a 290a 0a20 2020 2020   str(obj)..     
-000014f0: 2020 2072 6574 7572 6e20 6a73 6f6e 2e4a     return json.J
-00001500: 534f 4e45 6e63 6f64 6572 2e64 6566 6175  SONEncoder.defau
-00001510: 6c74 2873 656c 662c 206f 626a 290a 0a0a  lt(self, obj)...
-00001520: 6465 6620 6465 6c65 7465 5f64 6174 6173  def delete_datas
-00001530: 746f 7265 5f72 6573 6f75 7263 6528 7265  tore_resource(re
-00001540: 736f 7572 6365 5f69 642c 2061 7069 5f6b  source_id, api_k
-00001550: 6579 2c20 636b 616e 5f75 726c 293a 0a20  ey, ckan_url):. 
-00001560: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00001570: 6465 6c65 7465 5f75 726c 203d 2067 6574  delete_url = get
-00001580: 5f75 726c 2822 6461 7461 7374 6f72 655f  _url("datastore_
-00001590: 6465 6c65 7465 222c 2063 6b61 6e5f 7572  delete", ckan_ur
-000015a0: 6c29 0a20 2020 2020 2020 2072 6573 706f  l).        respo
-000015b0: 6e73 6520 3d20 7265 7175 6573 7473 2e70  nse = requests.p
-000015c0: 6f73 7428 0a20 2020 2020 2020 2020 2020  ost(.           
-000015d0: 2064 656c 6574 655f 7572 6c2c 0a20 2020   delete_url,.   
-000015e0: 2020 2020 2020 2020 2076 6572 6966 793d           verify=
-000015f0: 636f 6e66 6967 2e67 6574 2822 5353 4c5f  config.get("SSL_
-00001600: 5645 5249 4659 2229 2c0a 2020 2020 2020  VERIFY"),.      
-00001610: 2020 2020 2020 6461 7461 3d6a 736f 6e2e        data=json.
-00001620: 6475 6d70 7328 7b22 6964 223a 2072 6573  dumps({"id": res
-00001630: 6f75 7263 655f 6964 2c20 2266 6f72 6365  ource_id, "force
-00001640: 223a 2054 7275 657d 292c 0a20 2020 2020  ": True}),.     
-00001650: 2020 2020 2020 2068 6561 6465 7273 3d7b         headers={
-00001660: 2243 6f6e 7465 6e74 2d54 7970 6522 3a20  "Content-Type": 
-00001670: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
-00001680: 6e22 2c20 2241 7574 686f 7269 7a61 7469  n", "Authorizati
-00001690: 6f6e 223a 2061 7069 5f6b 6579 7d2c 0a20  on": api_key},. 
-000016a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000016b0: 2063 6865 636b 5f72 6573 706f 6e73 6528   check_response(
-000016c0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000016d0: 706f 6e73 652c 0a20 2020 2020 2020 2020  ponse,.         
-000016e0: 2020 2064 656c 6574 655f 7572 6c2c 0a20     delete_url,. 
-000016f0: 2020 2020 2020 2020 2020 2022 434b 414e             "CKAN
-00001700: 222c 0a20 2020 2020 2020 2020 2020 2067  ",.            g
-00001710: 6f6f 645f 7374 6174 7573 3d28 3230 312c  ood_status=(201,
-00001720: 2032 3030 2c20 3430 3429 2c0a 2020 2020   200, 404),.    
-00001730: 2020 2020 2020 2020 6967 6e6f 7265 5f6e          ignore_n
-00001740: 6f5f 7375 6363 6573 733d 5472 7565 2c0a  o_success=True,.
-00001750: 2020 2020 2020 2020 290a 2020 2020 6578          ).    ex
-00001760: 6365 7074 2072 6571 7565 7374 732e 6578  cept requests.ex
-00001770: 6365 7074 696f 6e73 2e52 6571 7565 7374  ceptions.Request
-00001780: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
-00001790: 2020 2072 6169 7365 2075 7469 6c2e 4a6f     raise util.Jo
-000017a0: 6245 7272 6f72 2822 4465 6c65 7469 6e67  bError("Deleting
-000017b0: 2065 7869 7374 696e 6720 6461 7461 7374   existing datast
-000017c0: 6f72 6520 6661 696c 6564 2e22 290a 0a0a  ore failed.")...
-000017d0: 6465 6620 6465 6c65 7465 5f72 6573 6f75  def delete_resou
-000017e0: 7263 6528 7265 736f 7572 6365 5f69 642c  rce(resource_id,
-000017f0: 2061 7069 5f6b 6579 2c20 636b 616e 5f75   api_key, ckan_u
-00001800: 726c 293a 0a20 2020 2074 7279 3a0a 2020  rl):.    try:.  
-00001810: 2020 2020 2020 6465 6c65 7465 5f75 726c        delete_url
-00001820: 203d 2067 6574 5f75 726c 2822 7265 736f   = get_url("reso
-00001830: 7572 6365 5f64 656c 6574 6522 2c20 636b  urce_delete", ck
-00001840: 616e 5f75 726c 290a 2020 2020 2020 2020  an_url).        
-00001850: 7265 7370 6f6e 7365 203d 2072 6571 7565  response = reque
-00001860: 7374 732e 706f 7374 280a 2020 2020 2020  sts.post(.      
-00001870: 2020 2020 2020 6465 6c65 7465 5f75 726c        delete_url
-00001880: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
-00001890: 7269 6679 3d63 6f6e 6669 672e 6765 7428  rify=config.get(
-000018a0: 2253 534c 5f56 4552 4946 5922 292c 0a20  "SSL_VERIFY"),. 
-000018b0: 2020 2020 2020 2020 2020 2064 6174 613d             data=
-000018c0: 6a73 6f6e 2e64 756d 7073 287b 2269 6422  json.dumps({"id"
-000018d0: 3a20 7265 736f 7572 6365 5f69 642c 2022  : resource_id, "
-000018e0: 666f 7263 6522 3a20 5472 7565 7d29 2c0a  force": True}),.
-000018f0: 2020 2020 2020 2020 2020 2020 6865 6164              head
-00001900: 6572 733d 7b22 436f 6e74 656e 742d 5479  ers={"Content-Ty
-00001910: 7065 223a 2022 6170 706c 6963 6174 696f  pe": "applicatio
-00001920: 6e2f 6a73 6f6e 222c 2022 4175 7468 6f72  n/json", "Author
-00001930: 697a 6174 696f 6e22 3a20 6170 695f 6b65  ization": api_ke
-00001940: 797d 2c0a 2020 2020 2020 2020 290a 2020  y},.        ).  
-00001950: 2020 2020 2020 6368 6563 6b5f 7265 7370        check_resp
-00001960: 6f6e 7365 280a 2020 2020 2020 2020 2020  onse(.          
-00001970: 2020 7265 7370 6f6e 7365 2c0a 2020 2020    response,.    
-00001980: 2020 2020 2020 2020 6465 6c65 7465 5f75          delete_u
-00001990: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
-000019a0: 2243 4b41 4e22 2c0a 2020 2020 2020 2020  "CKAN",.        
-000019b0: 2020 2020 676f 6f64 5f73 7461 7475 733d      good_status=
-000019c0: 2832 3031 2c20 3230 302c 2034 3034 292c  (201, 200, 404),
-000019d0: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
-000019e0: 6f72 655f 6e6f 5f73 7563 6365 7373 3d54  ore_no_success=T
-000019f0: 7275 652c 0a20 2020 2020 2020 2029 0a20  rue,.        ). 
-00001a00: 2020 2065 7863 6570 7420 7265 7175 6573     except reques
-00001a10: 7473 2e65 7863 6570 7469 6f6e 732e 5265  ts.exceptions.Re
-00001a20: 7175 6573 7445 7863 6570 7469 6f6e 3a0a  questException:.
-00001a30: 2020 2020 2020 2020 7261 6973 6520 7574          raise ut
-00001a40: 696c 2e4a 6f62 4572 726f 7228 2244 656c  il.JobError("Del
-00001a50: 6574 696e 6720 6578 6973 7469 6e67 2072  eting existing r
-00001a60: 6573 6f75 7263 6520 6661 696c 6564 2e22  esource failed."
-00001a70: 290a 0a0a 6465 6620 6461 7461 7374 6f72  )...def datastor
-00001a80: 655f 7265 736f 7572 6365 5f65 7869 7374  e_resource_exist
-00001a90: 7328 7265 736f 7572 6365 5f69 642c 2061  s(resource_id, a
-00001aa0: 7069 5f6b 6579 2c20 636b 616e 5f75 726c  pi_key, ckan_url
-00001ab0: 293a 0a20 2020 2074 7279 3a0a 2020 2020  ):.    try:.    
-00001ac0: 2020 2020 7365 6172 6368 5f75 726c 203d      search_url =
-00001ad0: 2067 6574 5f75 726c 2822 6461 7461 7374   get_url("datast
-00001ae0: 6f72 655f 7365 6172 6368 222c 2063 6b61  ore_search", cka
-00001af0: 6e5f 7572 6c29 0a20 2020 2020 2020 2072  n_url).        r
-00001b00: 6573 706f 6e73 6520 3d20 7265 7175 6573  esponse = reques
-00001b10: 7473 2e70 6f73 7428 0a20 2020 2020 2020  ts.post(.       
-00001b20: 2020 2020 2073 6561 7263 685f 7572 6c2c       search_url,
-00001b30: 0a20 2020 2020 2020 2020 2020 2076 6572  .            ver
-00001b40: 6966 793d 636f 6e66 6967 2e67 6574 2822  ify=config.get("
-00001b50: 5353 4c5f 5645 5249 4659 2229 2c0a 2020  SSL_VERIFY"),.  
-00001b60: 2020 2020 2020 2020 2020 6461 7461 3d6a            data=j
-00001b70: 736f 6e2e 6475 6d70 7328 7b22 6964 223a  son.dumps({"id":
-00001b80: 2072 6573 6f75 7263 655f 6964 2c20 226c   resource_id, "l
-00001b90: 696d 6974 223a 2030 7d29 2c0a 2020 2020  imit": 0}),.    
-00001ba0: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
-00001bb0: 7b22 436f 6e74 656e 742d 5479 7065 223a  {"Content-Type":
-00001bc0: 2022 6170 706c 6963 6174 696f 6e2f 6a73   "application/js
-00001bd0: 6f6e 222c 2022 4175 7468 6f72 697a 6174  on", "Authorizat
-00001be0: 696f 6e22 3a20 6170 695f 6b65 797d 2c0a  ion": api_key},.
-00001bf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00001c00: 2020 6966 2072 6573 706f 6e73 652e 7374    if response.st
-00001c10: 6174 7573 5f63 6f64 6520 3d3d 2034 3034  atus_code == 404
+000002a0: 414c 4c2c 2022 2229 0a0a 5553 455f 5052  ALL, "")..USE_PR
+000002b0: 4f58 5920 3d20 2244 4f57 4e4c 4f41 445f  OXY = "DOWNLOAD_
+000002c0: 5052 4f58 5922 2069 6e20 636f 6e66 6967  PROXY" in config
+000002d0: 0a69 6620 5553 455f 5052 4f58 593a 0a20  .if USE_PROXY:. 
+000002e0: 2020 2044 4f57 4e4c 4f41 445f 5052 4f58     DOWNLOAD_PROX
+000002f0: 5920 3d20 636f 6e66 6967 2e67 6574 2822  Y = config.get("
+00000300: 444f 574e 4c4f 4144 5f50 524f 5859 2229  DOWNLOAD_PROXY")
+00000310: 0a0a 6966 206e 6f74 2063 6f6e 6669 672e  ..if not config.
+00000320: 6765 7428 2253 534c 5f56 4552 4946 5922  get("SSL_VERIFY"
+00000330: 293a 0a20 2020 2072 6571 7565 7374 732e  ):.    requests.
+00000340: 7061 636b 6167 6573 2e75 726c 6c69 6233  packages.urllib3
+00000350: 2e64 6973 6162 6c65 5f77 6172 6e69 6e67  .disable_warning
+00000360: 7328 290a 0a50 4f53 5447 5245 535f 494e  s()..POSTGRES_IN
+00000370: 545f 4d41 5820 3d20 3231 3437 3438 3336  T_MAX = 21474836
+00000380: 3437 0a50 4f53 5447 5245 535f 494e 545f  47.POSTGRES_INT_
+00000390: 4d49 4e20 3d20 2d32 3134 3734 3833 3634  MIN = -214748364
+000003a0: 380a 504f 5354 4752 4553 5f42 4947 494e  8.POSTGRES_BIGIN
+000003b0: 545f 4d41 5820 3d20 3932 3233 3337 3230  T_MAX = 92233720
+000003c0: 3336 3835 3437 3735 3830 370a 504f 5354  36854775807.POST
+000003d0: 4752 4553 5f42 4947 494e 545f 4d49 4e20  GRES_BIGINT_MIN 
+000003e0: 3d20 2d39 3232 3333 3732 3033 3638 3534  = -9223372036854
+000003f0: 3737 3538 3038 0a0a 4441 5441 5354 4f52  775808..DATASTOR
+00000400: 455f 5552 4c53 203d 207b 0a20 2020 2022  E_URLS = {.    "
+00000410: 6461 7461 7374 6f72 655f 6465 6c65 7465  datastore_delete
+00000420: 223a 2022 7b63 6b61 6e5f 7572 6c7d 2f61  ": "{ckan_url}/a
+00000430: 7069 2f61 6374 696f 6e2f 6461 7461 7374  pi/action/datast
+00000440: 6f72 655f 6465 6c65 7465 222c 0a20 2020  ore_delete",.   
+00000450: 2022 7265 736f 7572 6365 5f75 7064 6174   "resource_updat
+00000460: 6522 3a20 227b 636b 616e 5f75 726c 7d2f  e": "{ckan_url}/
+00000470: 6170 692f 6163 7469 6f6e 2f72 6573 6f75  api/action/resou
+00000480: 7263 655f 7570 6461 7465 222c 0a7d 0a0a  rce_update",.}..
+00000490: 0a63 6c61 7373 2048 5454 5045 7272 6f72  .class HTTPError
+000004a0: 2875 7469 6c2e 4a6f 6245 7272 6f72 293a  (util.JobError):
+000004b0: 0a20 2020 2022 2222 4578 6365 7074 696f  .    """Exceptio
+000004c0: 6e20 7468 6174 2773 2072 6169 7365 6420  n that's raised 
+000004d0: 6966 2061 206a 6f62 2066 6169 6c73 2064  if a job fails d
+000004e0: 7565 2074 6f20 616e 2048 5454 5020 7072  ue to an HTTP pr
+000004f0: 6f62 6c65 6d2e 2222 220a 0a20 2020 2064  oblem."""..    d
+00000500: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00000510: 2c20 6d65 7373 6167 652c 2073 7461 7475  , message, statu
+00000520: 735f 636f 6465 2c20 7265 7175 6573 745f  s_code, request_
+00000530: 7572 6c2c 2072 6573 706f 6e73 6529 3a0a  url, response):.
+00000540: 2020 2020 2020 2020 2222 2249 6e69 7469          """Initi
+00000550: 616c 6973 6520 6120 6e65 7720 4854 5450  alise a new HTTP
+00000560: 4572 726f 722e 0a0a 2020 2020 2020 2020  Error...        
+00000570: 3a70 6172 616d 206d 6573 7361 6765 3a20  :param message: 
+00000580: 4120 6875 6d61 6e2d 7265 6164 6162 6c65  A human-readable
+00000590: 2065 7272 6f72 206d 6573 7361 6765 0a20   error message. 
+000005a0: 2020 2020 2020 203a 7479 7065 206d 6573         :type mes
+000005b0: 7361 6765 3a20 7374 7269 6e67 0a0a 2020  sage: string..  
+000005c0: 2020 2020 2020 3a70 6172 616d 2073 7461        :param sta
+000005d0: 7475 735f 636f 6465 3a20 5468 6520 7374  tus_code: The st
+000005e0: 6174 7573 2063 6f64 6520 6f66 2074 6865  atus code of the
+000005f0: 2065 7272 6f72 6564 2048 5454 5020 7265   errored HTTP re
+00000600: 7370 6f6e 7365 2c0a 2020 2020 2020 2020  sponse,.        
+00000610: 2020 2020 652e 672e 2035 3030 0a20 2020      e.g. 500.   
+00000620: 2020 2020 203a 7479 7065 2073 7461 7475       :type statu
+00000630: 735f 636f 6465 3a20 696e 740a 0a20 2020  s_code: int..   
+00000640: 2020 2020 203a 7061 7261 6d20 7265 7175       :param requ
+00000650: 6573 745f 7572 6c3a 2054 6865 2055 524c  est_url: The URL
+00000660: 2074 6861 7420 7761 7320 7265 7175 6573   that was reques
+00000670: 7465 640a 2020 2020 2020 2020 3a74 7970  ted.        :typ
+00000680: 6520 7265 7175 6573 745f 7572 6c3a 2073  e request_url: s
+00000690: 7472 696e 670a 0a20 2020 2020 2020 203a  tring..        :
+000006a0: 7061 7261 6d20 7265 7370 6f6e 7365 3a20  param response: 
+000006b0: 5468 6520 626f 6479 206f 6620 7468 6520  The body of the 
+000006c0: 6572 726f 7265 6420 4854 5450 2072 6573  errored HTTP res
+000006d0: 706f 6e73 6520 6173 2075 6e69 636f 6465  ponse as unicode
+000006e0: 0a20 2020 2020 2020 2020 2020 2028 6966  .            (if
+000006f0: 2079 6f75 2068 6176 6520 6120 7265 7175   you have a requ
+00000700: 6573 7473 2e52 6573 706f 6e73 6520 6f62  ests.Response ob
+00000710: 6a65 6374 2074 6865 6e20 7265 7370 6f6e  ject then respon
+00000720: 7365 2e74 6578 7420 7769 6c6c 0a20 2020  se.text will.   
+00000730: 2020 2020 2020 2020 2067 6976 6520 796f           give yo
+00000740: 7520 7468 6973 290a 2020 2020 2020 2020  u this).        
+00000750: 3a74 7970 6520 7265 7370 6f6e 7365 3a20  :type response: 
+00000760: 756e 6963 6f64 650a 0a20 2020 2020 2020  unicode..       
+00000770: 2022 2222 0a20 2020 2020 2020 2073 7570   """.        sup
+00000780: 6572 2848 5454 5045 7272 6f72 2c20 7365  er(HTTPError, se
+00000790: 6c66 292e 5f5f 696e 6974 5f5f 286d 6573  lf).__init__(mes
+000007a0: 7361 6765 290a 2020 2020 2020 2020 7365  sage).        se
+000007b0: 6c66 2e73 7461 7475 735f 636f 6465 203d  lf.status_code =
+000007c0: 2073 7461 7475 735f 636f 6465 0a20 2020   status_code.   
+000007d0: 2020 2020 2073 656c 662e 7265 7175 6573       self.reques
+000007e0: 745f 7572 6c20 3d20 7265 7175 6573 745f  t_url = request_
+000007f0: 7572 6c0a 2020 2020 2020 2020 7365 6c66  url.        self
+00000800: 2e72 6573 706f 6e73 6520 3d20 7265 7370  .response = resp
+00000810: 6f6e 7365 0a0a 2020 2020 6465 6620 6173  onse..    def as
+00000820: 5f64 6963 7428 7365 6c66 293a 0a20 2020  _dict(self):.   
+00000830: 2020 2020 2022 2222 5265 7475 726e 2061       """Return a
+00000840: 204a 534f 4e2d 7365 7269 616c 697a 6162   JSON-serializab
+00000850: 6c65 2064 6963 7469 6f6e 6172 7920 7265  le dictionary re
+00000860: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
+00000870: 7468 6973 2065 7272 6f72 2e0a 0a20 2020  this error...   
+00000880: 2020 2020 2053 7569 7461 626c 6520 666f       Suitable fo
+00000890: 7220 636b 616e 7365 7276 6963 6570 726f  r ckanservicepro
+000008a0: 7669 6465 7220 746f 2072 6574 7572 6e20  vider to return 
+000008b0: 746f 2074 6865 2063 6c69 656e 7420 7369  to the client si
+000008c0: 7465 2061 7320 7468 650a 2020 2020 2020  te as the.      
+000008d0: 2020 7661 6c75 6520 666f 7220 7468 6520    value for the 
+000008e0: 2265 7272 6f72 2220 6b65 7920 696e 2074  "error" key in t
+000008f0: 6865 206a 6f62 2064 6963 742e 0a0a 2020  he job dict...  
+00000900: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00000910: 2020 6966 2073 656c 662e 7265 7370 6f6e    if self.respon
+00000920: 7365 2061 6e64 206c 656e 2873 656c 662e  se and len(self.
+00000930: 7265 7370 6f6e 7365 2920 3e20 3230 303a  response) > 200:
+00000940: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00000950: 706f 6e73 6520 3d20 7365 6c66 2e72 6573  ponse = self.res
+00000960: 706f 6e73 655b 3a32 3030 5d0a 2020 2020  ponse[:200].    
+00000970: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00000980: 2020 2020 2020 7265 7370 6f6e 7365 203d        response =
+00000990: 2073 656c 662e 7265 7370 6f6e 7365 0a20   self.response. 
+000009a0: 2020 2020 2020 2072 6574 7572 6e20 7b0a         return {.
+000009b0: 2020 2020 2020 2020 2020 2020 226d 6573              "mes
+000009c0: 7361 6765 223a 2073 656c 662e 6d65 7373  sage": self.mess
+000009d0: 6167 652c 0a20 2020 2020 2020 2020 2020  age,.           
+000009e0: 2022 4854 5450 2073 7461 7475 7320 636f   "HTTP status co
+000009f0: 6465 223a 2073 656c 662e 7374 6174 7573  de": self.status
+00000a00: 5f63 6f64 652c 0a20 2020 2020 2020 2020  _code,.         
+00000a10: 2020 2022 5265 7175 6573 7465 6420 5552     "Requested UR
+00000a20: 4c22 3a20 7365 6c66 2e72 6571 7565 7374  L": self.request
+00000a30: 5f75 726c 2c0a 2020 2020 2020 2020 2020  _url,.          
+00000a40: 2020 2252 6573 706f 6e73 6522 3a20 7265    "Response": re
+00000a50: 7370 6f6e 7365 2c0a 2020 2020 2020 2020  sponse,.        
+00000a60: 7d0a 0a20 2020 2064 6566 205f 5f73 7472  }..    def __str
+00000a70: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00000a80: 2020 7265 7475 726e 2022 7b7d 2073 7461    return "{} sta
+00000a90: 7475 733d 7b7d 2075 726c 3d7b 7d20 7265  tus={} url={} re
+00000aa0: 7370 6f6e 7365 3d7b 7d22 2e66 6f72 6d61  sponse={}".forma
+00000ab0: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
+00000ac0: 656c 662e 6d65 7373 6167 652c 2073 656c  elf.message, sel
+00000ad0: 662e 7374 6174 7573 5f63 6f64 652c 2073  f.status_code, s
+00000ae0: 656c 662e 7265 7175 6573 745f 7572 6c2c  elf.request_url,
+00000af0: 2073 656c 662e 7265 7370 6f6e 7365 0a20   self.response. 
+00000b00: 2020 2020 2020 2029 2e65 6e63 6f64 6528         ).encode(
+00000b10: 2261 7363 6969 222c 2022 7265 706c 6163  "ascii", "replac
+00000b20: 6522 290a 0a0a 6465 6620 6765 745f 7572  e")...def get_ur
+00000b30: 6c28 6163 7469 6f6e 2c20 636b 616e 5f75  l(action, ckan_u
+00000b40: 726c 293a 0a20 2020 2022 2222 0a20 2020  rl):.    """.   
+00000b50: 2047 6574 2075 726c 2066 6f72 2063 6b61   Get url for cka
+00000b60: 6e20 6163 7469 6f6e 0a20 2020 2022 2222  n action.    """
+00000b70: 0a20 2020 2069 6620 6e6f 7420 7572 6c73  .    if not urls
+00000b80: 706c 6974 2863 6b61 6e5f 7572 6c29 2e73  plit(ckan_url).s
+00000b90: 6368 656d 653a 0a20 2020 2020 2020 2063  cheme:.        c
+00000ba0: 6b61 6e5f 7572 6c20 3d20 2268 7474 703a  kan_url = "http:
+00000bb0: 2f2f 2220 2b20 636b 616e 5f75 726c 2e6c  //" + ckan_url.l
+00000bc0: 7374 7269 7028 222f 2229 2020 2320 4465  strip("/")  # De
+00000bd0: 7653 6b69 6d3a 2069 676e 6f72 6520 4453  vSkim: ignore DS
+00000be0: 3133 3731 3338 0a20 2020 2063 6b61 6e5f  137138.    ckan_
+00000bf0: 7572 6c20 3d20 636b 616e 5f75 726c 2e72  url = ckan_url.r
+00000c00: 7374 7269 7028 222f 2229 0a20 2020 2072  strip("/").    r
+00000c10: 6574 7572 6e20 227b 636b 616e 5f75 726c  eturn "{ckan_url
+00000c20: 7d2f 6170 692f 332f 6163 7469 6f6e 2f7b  }/api/3/action/{
+00000c30: 6163 7469 6f6e 7d22 2e66 6f72 6d61 7428  action}".format(
+00000c40: 636b 616e 5f75 726c 3d63 6b61 6e5f 7572  ckan_url=ckan_ur
+00000c50: 6c2c 2061 6374 696f 6e3d 6163 7469 6f6e  l, action=action
+00000c60: 290a 0a0a 6465 6620 6368 6563 6b5f 7265  )...def check_re
+00000c70: 7370 6f6e 7365 280a 2020 2020 7265 7370  sponse(.    resp
+00000c80: 6f6e 7365 2c20 7265 7175 6573 745f 7572  onse, request_ur
+00000c90: 6c2c 2077 686f 2c20 676f 6f64 5f73 7461  l, who, good_sta
+00000ca0: 7475 733d 2832 3031 2c20 3230 3029 2c20  tus=(201, 200), 
+00000cb0: 6967 6e6f 7265 5f6e 6f5f 7375 6363 6573  ignore_no_succes
+00000cc0: 733d 4661 6c73 650a 293a 0a20 2020 2022  s=False.):.    "
+00000cd0: 2222 0a20 2020 2043 6865 636b 7320 7468  "".    Checks th
+00000ce0: 6520 7265 7370 6f6e 7365 2061 6e64 2072  e response and r
+00000cf0: 6169 7365 7320 6578 6365 7074 696f 6e73  aises exceptions
+00000d00: 2069 6620 736f 6d65 7468 696e 6720 7765   if something we
+00000d10: 6e74 2074 6572 7269 626c 7920 7772 6f6e  nt terribly wron
+00000d20: 670a 0a20 2020 203a 7061 7261 6d20 7768  g..    :param wh
+00000d30: 6f3a 2041 2073 686f 7274 206e 616d 6520  o: A short name 
+00000d40: 7468 6174 2069 6e64 6963 6174 6564 2077  that indicated w
+00000d50: 6865 7265 2074 6865 2065 7272 6f72 206f  here the error o
+00000d60: 6363 7572 7265 640a 2020 2020 2020 2020  ccurred.        
+00000d70: 2020 2020 2020 2020 2866 6f72 2065 7861          (for exa
+00000d80: 6d70 6c65 2022 434b 414e 2229 0a20 2020  mple "CKAN").   
+00000d90: 203a 7061 7261 6d20 676f 6f64 5f73 7461   :param good_sta
+00000da0: 7475 733a 2053 7461 7475 7320 636f 6465  tus: Status code
+00000db0: 7320 7468 6174 2073 686f 756c 6420 6e6f  s that should no
+00000dc0: 7420 7261 6973 6520 616e 2065 7863 6570  t raise an excep
+00000dd0: 7469 6f6e 0a0a 2020 2020 2222 220a 2020  tion..    """.  
+00000de0: 2020 6966 206e 6f74 2072 6573 706f 6e73    if not respons
+00000df0: 652e 7374 6174 7573 5f63 6f64 653a 0a20  e.status_code:. 
+00000e00: 2020 2020 2020 2072 6169 7365 2048 5454         raise HTT
+00000e10: 5045 7272 6f72 280a 2020 2020 2020 2020  PError(.        
+00000e20: 2020 2020 2244 6174 6150 7573 6865 7220      "DataPusher 
+00000e30: 7265 6365 6976 6564 2061 6e20 4854 5450  received an HTTP
+00000e40: 2072 6573 706f 6e73 6520 7769 7468 206e   response with n
+00000e50: 6f20 7374 6174 7573 2063 6f64 6522 2c0a  o status code",.
+00000e60: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00000e70: 7573 5f63 6f64 653d 4e6f 6e65 2c0a 2020  us_code=None,.  
+00000e80: 2020 2020 2020 2020 2020 7265 7175 6573            reques
+00000e90: 745f 7572 6c3d 7265 7175 6573 745f 7572  t_url=request_ur
+00000ea0: 6c2c 0a20 2020 2020 2020 2020 2020 2072  l,.            r
+00000eb0: 6573 706f 6e73 653d 7265 7370 6f6e 7365  esponse=response
+00000ec0: 2e74 6578 742c 0a20 2020 2020 2020 2029  .text,.        )
+00000ed0: 0a0a 2020 2020 6d65 7373 6167 6520 3d20  ..    message = 
+00000ee0: 227b 7768 6f7d 2062 6164 2072 6573 706f  "{who} bad respo
+00000ef0: 6e73 652e 2053 7461 7475 7320 636f 6465  nse. Status code
+00000f00: 3a20 7b63 6f64 657d 207b 7265 6173 6f6e  : {code} {reason
+00000f10: 7d2e 2041 743a 207b 7572 6c7d 2e22 0a20  }. At: {url}.". 
+00000f20: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00000f30: 6966 2072 6573 706f 6e73 652e 7374 6174  if response.stat
+00000f40: 7573 5f63 6f64 6520 6e6f 7420 696e 2067  us_code not in g
+00000f50: 6f6f 645f 7374 6174 7573 3a0a 2020 2020  ood_status:.    
+00000f60: 2020 2020 2020 2020 6a73 6f6e 5f72 6573          json_res
+00000f70: 706f 6e73 6520 3d20 7265 7370 6f6e 7365  ponse = response
+00000f80: 2e6a 736f 6e28 290a 2020 2020 2020 2020  .json().        
+00000f90: 2020 2020 6966 206e 6f74 2069 676e 6f72      if not ignor
+00000fa0: 655f 6e6f 5f73 7563 6365 7373 206f 7220  e_no_success or 
+00000fb0: 6a73 6f6e 5f72 6573 706f 6e73 652e 6765  json_response.ge
+00000fc0: 7428 2273 7563 6365 7373 2229 3a0a 2020  t("success"):.  
+00000fd0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00000fe0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00000ff0: 2020 2020 2020 206d 6573 7361 6765 203d         message =
+00001000: 206a 736f 6e5f 7265 7370 6f6e 7365 5b22   json_response["
+00001010: 6572 726f 7222 5d5b 226d 6573 7361 6765  error"]["message
+00001020: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00001030: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00001040: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00001050: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00001060: 203d 206d 6573 7361 6765 2e66 6f72 6d61   = message.forma
+00001070: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00001080: 2020 2020 2020 2020 2020 2077 686f 3d77             who=w
+00001090: 686f 2c0a 2020 2020 2020 2020 2020 2020  ho,.            
+000010a0: 2020 2020 2020 2020 2020 2020 636f 6465              code
+000010b0: 3d72 6573 706f 6e73 652e 7374 6174 7573  =response.status
+000010c0: 5f63 6f64 652c 0a20 2020 2020 2020 2020  _code,.         
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000010e0: 6561 736f 6e3d 7265 7370 6f6e 7365 2e72  eason=response.r
+000010f0: 6561 736f 6e2c 0a20 2020 2020 2020 2020  eason,.         
+00001100: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00001110: 726c 3d72 6571 7565 7374 5f75 726c 2c0a  rl=request_url,.
+00001120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001130: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00001140: 2020 2020 2020 7261 6973 6520 4854 5450        raise HTTP
+00001150: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
+00001160: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00001170: 6765 2c0a 2020 2020 2020 2020 2020 2020  ge,.            
+00001180: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+00001190: 6f64 653d 7265 7370 6f6e 7365 2e73 7461  ode=response.sta
+000011a0: 7475 735f 636f 6465 2c0a 2020 2020 2020  tus_code,.      
+000011b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000011c0: 7175 6573 745f 7572 6c3d 7265 7175 6573  quest_url=reques
+000011d0: 745f 7572 6c2c 0a20 2020 2020 2020 2020  t_url,.         
+000011e0: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+000011f0: 6e73 653d 7265 7370 6f6e 7365 2e74 6578  nse=response.tex
+00001200: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00001210: 2020 2029 0a20 2020 2065 7863 6570 7420     ).    except 
+00001220: 5661 6c75 6545 7272 6f72 3a0a 2020 2020  ValueError:.    
+00001230: 2020 2020 6d65 7373 6167 6520 3d20 6d65      message = me
+00001240: 7373 6167 652e 666f 726d 6174 280a 2020  ssage.format(.  
+00001250: 2020 2020 2020 2020 2020 7768 6f3d 7768            who=wh
+00001260: 6f2c 0a20 2020 2020 2020 2020 2020 2063  o,.            c
+00001270: 6f64 653d 7265 7370 6f6e 7365 2e73 7461  ode=response.sta
+00001280: 7475 735f 636f 6465 2c0a 2020 2020 2020  tus_code,.      
+00001290: 2020 2020 2020 7265 6173 6f6e 3d72 6573        reason=res
+000012a0: 706f 6e73 652e 7265 6173 6f6e 2c0a 2020  ponse.reason,.  
+000012b0: 2020 2020 2020 2020 2020 7572 6c3d 7265            url=re
+000012c0: 7175 6573 745f 7572 6c2c 0a20 2020 2020  quest_url,.     
+000012d0: 2020 2020 2020 2072 6573 703d 7265 7370         resp=resp
+000012e0: 6f6e 7365 2e74 6578 745b 3a32 3030 5d2c  onse.text[:200],
+000012f0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00001300: 2020 2072 6169 7365 2048 5454 5045 7272     raise HTTPErr
+00001310: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00001320: 6d65 7373 6167 652c 0a20 2020 2020 2020  message,.       
+00001330: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
+00001340: 3d72 6573 706f 6e73 652e 7374 6174 7573  =response.status
+00001350: 5f63 6f64 652c 0a20 2020 2020 2020 2020  _code,.         
+00001360: 2020 2072 6571 7565 7374 5f75 726c 3d72     request_url=r
+00001370: 6571 7565 7374 5f75 726c 2c0a 2020 2020  equest_url,.    
+00001380: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00001390: 3d72 6573 706f 6e73 652e 7465 7874 2c0a  =response.text,.
+000013a0: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+000013b0: 7320 4461 7461 7374 6f72 6545 6e63 6f64  s DatastoreEncod
+000013c0: 6572 286a 736f 6e2e 4a53 4f4e 456e 636f  er(json.JSONEnco
+000013d0: 6465 7229 3a0a 2020 2020 2320 4375 7374  der):.    # Cust
+000013e0: 6f6d 204a 534f 4e20 656e 636f 6465 720a  om JSON encoder.
+000013f0: 2020 2020 6465 6620 6465 6661 756c 7428      def default(
+00001400: 7365 6c66 2c20 6f62 6a29 3a0a 2020 2020  self, obj):.    
+00001410: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00001420: 6528 6f62 6a2c 2064 6174 6574 696d 652e  e(obj, datetime.
+00001430: 6461 7465 7469 6d65 293a 0a20 2020 2020  datetime):.     
+00001440: 2020 2020 2020 2072 6574 7572 6e20 6f62         return ob
+00001450: 6a2e 6973 6f66 6f72 6d61 7428 290a 2020  j.isoformat().  
+00001460: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00001470: 6e63 6528 6f62 6a2c 2064 6563 696d 616c  nce(obj, decimal
+00001480: 2e44 6563 696d 616c 293a 0a20 2020 2020  .Decimal):.     
+00001490: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+000014a0: 7228 6f62 6a29 0a0a 2020 2020 2020 2020  r(obj)..        
+000014b0: 7265 7475 726e 206a 736f 6e2e 4a53 4f4e  return json.JSON
+000014c0: 456e 636f 6465 722e 6465 6661 756c 7428  Encoder.default(
+000014d0: 7365 6c66 2c20 6f62 6a29 0a0a 0a64 6566  self, obj)...def
+000014e0: 2064 656c 6574 655f 6461 7461 7374 6f72   delete_datastor
+000014f0: 655f 7265 736f 7572 6365 2872 6573 6f75  e_resource(resou
+00001500: 7263 655f 6964 2c20 6170 695f 6b65 792c  rce_id, api_key,
+00001510: 2063 6b61 6e5f 7572 6c29 3a0a 2020 2020   ckan_url):.    
+00001520: 7472 793a 0a20 2020 2020 2020 2064 656c  try:.        del
+00001530: 6574 655f 7572 6c20 3d20 6765 745f 7572  ete_url = get_ur
+00001540: 6c28 2264 6174 6173 746f 7265 5f64 656c  l("datastore_del
+00001550: 6574 6522 2c20 636b 616e 5f75 726c 290a  ete", ckan_url).
+00001560: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00001570: 203d 2072 6571 7565 7374 732e 706f 7374   = requests.post
+00001580: 280a 2020 2020 2020 2020 2020 2020 6465  (.            de
+00001590: 6c65 7465 5f75 726c 2c0a 2020 2020 2020  lete_url,.      
+000015a0: 2020 2020 2020 7665 7269 6679 3d63 6f6e        verify=con
+000015b0: 6669 672e 6765 7428 2253 534c 5f56 4552  fig.get("SSL_VER
+000015c0: 4946 5922 292c 0a20 2020 2020 2020 2020  IFY"),.         
+000015d0: 2020 2064 6174 613d 6a73 6f6e 2e64 756d     data=json.dum
+000015e0: 7073 287b 2269 6422 3a20 7265 736f 7572  ps({"id": resour
+000015f0: 6365 5f69 642c 2022 666f 7263 6522 3a20  ce_id, "force": 
+00001600: 5472 7565 7d29 2c0a 2020 2020 2020 2020  True}),.        
+00001610: 2020 2020 6865 6164 6572 733d 7b22 436f      headers={"Co
+00001620: 6e74 656e 742d 5479 7065 223a 2022 6170  ntent-Type": "ap
+00001630: 706c 6963 6174 696f 6e2f 6a73 6f6e 222c  plication/json",
+00001640: 2022 4175 7468 6f72 697a 6174 696f 6e22   "Authorization"
+00001650: 3a20 6170 695f 6b65 797d 2c0a 2020 2020  : api_key},.    
+00001660: 2020 2020 290a 2020 2020 2020 2020 6368      ).        ch
+00001670: 6563 6b5f 7265 7370 6f6e 7365 280a 2020  eck_response(.  
+00001680: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+00001690: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+000016a0: 6465 6c65 7465 5f75 726c 2c0a 2020 2020  delete_url,.    
+000016b0: 2020 2020 2020 2020 2243 4b41 4e22 2c0a          "CKAN",.
+000016c0: 2020 2020 2020 2020 2020 2020 676f 6f64              good
+000016d0: 5f73 7461 7475 733d 2832 3031 2c20 3230  _status=(201, 20
+000016e0: 302c 2034 3034 292c 0a20 2020 2020 2020  0, 404),.       
+000016f0: 2020 2020 2069 676e 6f72 655f 6e6f 5f73       ignore_no_s
+00001700: 7563 6365 7373 3d54 7275 652c 0a20 2020  uccess=True,.   
+00001710: 2020 2020 2029 0a20 2020 2065 7863 6570       ).    excep
+00001720: 7420 7265 7175 6573 7473 2e65 7863 6570  t requests.excep
+00001730: 7469 6f6e 732e 5265 7175 6573 7445 7863  tions.RequestExc
+00001740: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
+00001750: 7261 6973 6520 7574 696c 2e4a 6f62 4572  raise util.JobEr
+00001760: 726f 7228 2244 656c 6574 696e 6720 6578  ror("Deleting ex
+00001770: 6973 7469 6e67 2064 6174 6173 746f 7265  isting datastore
+00001780: 2066 6169 6c65 642e 2229 0a0a 0a64 6566   failed.")...def
+00001790: 2064 656c 6574 655f 7265 736f 7572 6365   delete_resource
+000017a0: 2872 6573 6f75 7263 655f 6964 2c20 6170  (resource_id, ap
+000017b0: 695f 6b65 792c 2063 6b61 6e5f 7572 6c29  i_key, ckan_url)
+000017c0: 3a0a 2020 2020 7472 793a 0a20 2020 2020  :.    try:.     
+000017d0: 2020 2064 656c 6574 655f 7572 6c20 3d20     delete_url = 
+000017e0: 6765 745f 7572 6c28 2272 6573 6f75 7263  get_url("resourc
+000017f0: 655f 6465 6c65 7465 222c 2063 6b61 6e5f  e_delete", ckan_
+00001800: 7572 6c29 0a20 2020 2020 2020 2072 6573  url).        res
+00001810: 706f 6e73 6520 3d20 7265 7175 6573 7473  ponse = requests
+00001820: 2e70 6f73 7428 0a20 2020 2020 2020 2020  .post(.         
+00001830: 2020 2064 656c 6574 655f 7572 6c2c 0a20     delete_url,. 
+00001840: 2020 2020 2020 2020 2020 2076 6572 6966             verif
+00001850: 793d 636f 6e66 6967 2e67 6574 2822 5353  y=config.get("SS
+00001860: 4c5f 5645 5249 4659 2229 2c0a 2020 2020  L_VERIFY"),.    
+00001870: 2020 2020 2020 2020 6461 7461 3d6a 736f          data=jso
+00001880: 6e2e 6475 6d70 7328 7b22 6964 223a 2072  n.dumps({"id": r
+00001890: 6573 6f75 7263 655f 6964 2c20 2266 6f72  esource_id, "for
+000018a0: 6365 223a 2054 7275 657d 292c 0a20 2020  ce": True}),.   
+000018b0: 2020 2020 2020 2020 2068 6561 6465 7273           headers
+000018c0: 3d7b 2243 6f6e 7465 6e74 2d54 7970 6522  ={"Content-Type"
+000018d0: 3a20 2261 7070 6c69 6361 7469 6f6e 2f6a  : "application/j
+000018e0: 736f 6e22 2c20 2241 7574 686f 7269 7a61  son", "Authoriza
+000018f0: 7469 6f6e 223a 2061 7069 5f6b 6579 7d2c  tion": api_key},
+00001900: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00001910: 2020 2063 6865 636b 5f72 6573 706f 6e73     check_respons
+00001920: 6528 0a20 2020 2020 2020 2020 2020 2072  e(.            r
+00001930: 6573 706f 6e73 652c 0a20 2020 2020 2020  esponse,.       
+00001940: 2020 2020 2064 656c 6574 655f 7572 6c2c       delete_url,
+00001950: 0a20 2020 2020 2020 2020 2020 2022 434b  .            "CK
+00001960: 414e 222c 0a20 2020 2020 2020 2020 2020  AN",.           
+00001970: 2067 6f6f 645f 7374 6174 7573 3d28 3230   good_status=(20
+00001980: 312c 2032 3030 2c20 3430 3429 2c0a 2020  1, 200, 404),.  
+00001990: 2020 2020 2020 2020 2020 6967 6e6f 7265            ignore
+000019a0: 5f6e 6f5f 7375 6363 6573 733d 5472 7565  _no_success=True
+000019b0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+000019c0: 6578 6365 7074 2072 6571 7565 7374 732e  except requests.
+000019d0: 6578 6365 7074 696f 6e73 2e52 6571 7565  exceptions.Reque
+000019e0: 7374 4578 6365 7074 696f 6e3a 0a20 2020  stException:.   
+000019f0: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
+00001a00: 4a6f 6245 7272 6f72 2822 4465 6c65 7469  JobError("Deleti
+00001a10: 6e67 2065 7869 7374 696e 6720 7265 736f  ng existing reso
+00001a20: 7572 6365 2066 6169 6c65 642e 2229 0a0a  urce failed.")..
+00001a30: 0a64 6566 2064 6174 6173 746f 7265 5f72  .def datastore_r
+00001a40: 6573 6f75 7263 655f 6578 6973 7473 2872  esource_exists(r
+00001a50: 6573 6f75 7263 655f 6964 2c20 6170 695f  esource_id, api_
+00001a60: 6b65 792c 2063 6b61 6e5f 7572 6c29 3a0a  key, ckan_url):.
+00001a70: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00001a80: 2073 6561 7263 685f 7572 6c20 3d20 6765   search_url = ge
+00001a90: 745f 7572 6c28 2264 6174 6173 746f 7265  t_url("datastore
+00001aa0: 5f73 6561 7263 6822 2c20 636b 616e 5f75  _search", ckan_u
+00001ab0: 726c 290a 2020 2020 2020 2020 7265 7370  rl).        resp
+00001ac0: 6f6e 7365 203d 2072 6571 7565 7374 732e  onse = requests.
+00001ad0: 706f 7374 280a 2020 2020 2020 2020 2020  post(.          
+00001ae0: 2020 7365 6172 6368 5f75 726c 2c0a 2020    search_url,.  
+00001af0: 2020 2020 2020 2020 2020 7665 7269 6679            verify
+00001b00: 3d63 6f6e 6669 672e 6765 7428 2253 534c  =config.get("SSL
+00001b10: 5f56 4552 4946 5922 292c 0a20 2020 2020  _VERIFY"),.     
+00001b20: 2020 2020 2020 2064 6174 613d 6a73 6f6e         data=json
+00001b30: 2e64 756d 7073 287b 2269 6422 3a20 7265  .dumps({"id": re
+00001b40: 736f 7572 6365 5f69 642c 2022 6c69 6d69  source_id, "limi
+00001b50: 7422 3a20 307d 292c 0a20 2020 2020 2020  t": 0}),.       
+00001b60: 2020 2020 2068 6561 6465 7273 3d7b 2243       headers={"C
+00001b70: 6f6e 7465 6e74 2d54 7970 6522 3a20 2261  ontent-Type": "a
+00001b80: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e22  pplication/json"
+00001b90: 2c20 2241 7574 686f 7269 7a61 7469 6f6e  , "Authorization
+00001ba0: 223a 2061 7069 5f6b 6579 7d2c 0a20 2020  ": api_key},.   
+00001bb0: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00001bc0: 6620 7265 7370 6f6e 7365 2e73 7461 7475  f response.statu
+00001bd0: 735f 636f 6465 203d 3d20 3430 343a 0a20  s_code == 404:. 
+00001be0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001bf0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00001c00: 656c 6966 2072 6573 706f 6e73 652e 7374  elif response.st
+00001c10: 6174 7573 5f63 6f64 6520 3d3d 2032 3030  atus_code == 200
 00001c20: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00001c30: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
-00001c40: 2020 2065 6c69 6620 7265 7370 6f6e 7365     elif response
-00001c50: 2e73 7461 7475 735f 636f 6465 203d 3d20  .status_code == 
-00001c60: 3230 303a 0a20 2020 2020 2020 2020 2020  200:.           
-00001c70: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00001c80: 2e6a 736f 6e28 292e 6765 7428 2272 6573  .json().get("res
-00001c90: 756c 7422 2c20 7b22 6669 656c 6473 223a  ult", {"fields":
-00001ca0: 205b 5d7d 290a 2020 2020 2020 2020 656c   []}).        el
-00001cb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00001cc0: 7261 6973 6520 4854 5450 4572 726f 7228  raise HTTPError(
-00001cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ce0: 2022 4572 726f 7220 6765 7474 696e 6720   "Error getting 
-00001cf0: 6461 7461 7374 6f72 6520 7265 736f 7572  datastore resour
-00001d00: 6365 2e22 2c0a 2020 2020 2020 2020 2020  ce.",.          
-00001d10: 2020 2020 2020 7265 7370 6f6e 7365 2e73        response.s
-00001d20: 7461 7475 735f 636f 6465 2c0a 2020 2020  tatus_code,.    
-00001d30: 2020 2020 2020 2020 2020 2020 7365 6172              sear
-00001d40: 6368 5f75 726c 2c0a 2020 2020 2020 2020  ch_url,.        
-00001d50: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00001d60: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-00001d70: 2020 2020 6578 6365 7074 2072 6571 7565      except reque
-00001d80: 7374 732e 6578 6365 7074 696f 6e73 2e52  sts.exceptions.R
-00001d90: 6571 7565 7374 4578 6365 7074 696f 6e20  equestException 
-00001da0: 6173 2065 3a0a 2020 2020 2020 2020 7261  as e:.        ra
-00001db0: 6973 6520 7574 696c 2e4a 6f62 4572 726f  ise util.JobErro
-00001dc0: 7228 2245 7272 6f72 2067 6574 7469 6e67  r("Error getting
-00001dd0: 2064 6174 6173 746f 7265 2072 6573 6f75   datastore resou
-00001de0: 7263 6520 287b 2173 7d29 2e22 2e66 6f72  rce ({!s}).".for
-00001df0: 6d61 7428 6529 290a 0a0a 6465 6620 7365  mat(e))...def se
-00001e00: 6e64 5f72 6573 6f75 7263 655f 746f 5f64  nd_resource_to_d
-00001e10: 6174 6173 746f 7265 280a 2020 2020 7265  atastore(.    re
-00001e20: 736f 7572 6365 2c0a 2020 2020 7265 736f  source,.    reso
-00001e30: 7572 6365 5f69 642c 0a20 2020 2068 6561  urce_id,.    hea
-00001e40: 6465 7273 2c0a 2020 2020 6170 695f 6b65  ders,.    api_ke
-00001e50: 792c 0a20 2020 2063 6b61 6e5f 7572 6c2c  y,.    ckan_url,
-00001e60: 0a20 2020 2072 6563 6f72 6473 2c0a 2020  .    records,.  
-00001e70: 2020 616c 6961 7365 732c 0a20 2020 2063    aliases,.    c
-00001e80: 616c 6375 6c61 7465 5f72 6563 6f72 645f  alculate_record_
-00001e90: 636f 756e 742c 0a29 3a0a 2020 2020 2222  count,.):.    ""
-00001ea0: 220a 2020 2020 5374 6f72 6573 2072 6563  ".    Stores rec
-00001eb0: 6f72 6473 2069 6e20 434b 414e 2064 6174  ords in CKAN dat
-00001ec0: 6173 746f 7265 0a20 2020 2022 2222 0a0a  astore.    """..
-00001ed0: 2020 2020 6966 2072 6573 6f75 7263 655f      if resource_
-00001ee0: 6964 3a0a 2020 2020 2020 2020 2320 7573  id:.        # us
-00001ef0: 6564 2074 6f20 6372 6561 7465 2074 6865  ed to create the
-00001f00: 2022 6d61 696e 2220 7265 736f 7572 6365   "main" resource
-00001f10: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-00001f20: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-00001f30: 2022 7265 736f 7572 6365 5f69 6422 3a20   "resource_id": 
-00001f40: 7265 736f 7572 6365 5f69 642c 0a20 2020  resource_id,.   
-00001f50: 2020 2020 2020 2020 2022 6669 656c 6473           "fields
-00001f60: 223a 2068 6561 6465 7273 2c0a 2020 2020  ": headers,.    
-00001f70: 2020 2020 2020 2020 2266 6f72 6365 223a          "force":
-00001f80: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-00001f90: 2020 2022 7265 636f 7264 7322 3a20 7265     "records": re
-00001fa0: 636f 7264 732c 0a20 2020 2020 2020 2020  cords,.         
-00001fb0: 2020 2022 616c 6961 7365 7322 3a20 616c     "aliases": al
-00001fc0: 6961 7365 732c 0a20 2020 2020 2020 2020  iases,.         
-00001fd0: 2020 2022 6361 6c63 756c 6174 655f 7265     "calculate_re
-00001fe0: 636f 7264 5f63 6f75 6e74 223a 2063 616c  cord_count": cal
-00001ff0: 6375 6c61 7465 5f72 6563 6f72 645f 636f  culate_record_co
-00002000: 756e 742c 0a20 2020 2020 2020 207d 0a20  unt,.        }. 
-00002010: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00002020: 2023 2075 7365 6420 746f 2063 7265 6174   # used to creat
-00002030: 6520 7468 6520 2273 7461 7473 2220 7265  e the "stats" re
-00002040: 736f 7572 6365 0a20 2020 2020 2020 2072  source.        r
-00002050: 6571 7565 7374 203d 207b 0a20 2020 2020  equest = {.     
-00002060: 2020 2020 2020 2022 7265 736f 7572 6365         "resource
-00002070: 223a 2072 6573 6f75 7263 652c 0a20 2020  ": resource,.   
-00002080: 2020 2020 2020 2020 2022 6669 656c 6473           "fields
-00002090: 223a 2068 6561 6465 7273 2c0a 2020 2020  ": headers,.    
-000020a0: 2020 2020 2020 2020 2266 6f72 6365 223a          "force":
-000020b0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-000020c0: 2020 2022 616c 6961 7365 7322 3a20 616c     "aliases": al
-000020d0: 6961 7365 732c 0a20 2020 2020 2020 2020  iases,.         
-000020e0: 2020 2022 6361 6c63 756c 6174 655f 7265     "calculate_re
-000020f0: 636f 7264 5f63 6f75 6e74 223a 2063 616c  cord_count": cal
-00002100: 6375 6c61 7465 5f72 6563 6f72 645f 636f  culate_record_co
-00002110: 756e 742c 0a20 2020 2020 2020 207d 0a0a  unt,.        }..
-00002120: 2020 2020 7572 6c20 3d20 6765 745f 7572      url = get_ur
-00002130: 6c28 2264 6174 6173 746f 7265 5f63 7265  l("datastore_cre
-00002140: 6174 6522 2c20 636b 616e 5f75 726c 290a  ate", ckan_url).
-00002150: 2020 2020 7220 3d20 7265 7175 6573 7473      r = requests
-00002160: 2e70 6f73 7428 0a20 2020 2020 2020 2075  .post(.        u
-00002170: 726c 2c0a 2020 2020 2020 2020 7665 7269  rl,.        veri
-00002180: 6679 3d63 6f6e 6669 672e 6765 7428 2253  fy=config.get("S
-00002190: 534c 5f56 4552 4946 5922 292c 0a20 2020  SL_VERIFY"),.   
-000021a0: 2020 2020 2064 6174 613d 6a73 6f6e 2e64       data=json.d
-000021b0: 756d 7073 2872 6571 7565 7374 2c20 636c  umps(request, cl
-000021c0: 733d 4461 7461 7374 6f72 6545 6e63 6f64  s=DatastoreEncod
-000021d0: 6572 292c 0a20 2020 2020 2020 2068 6561  er),.        hea
-000021e0: 6465 7273 3d7b 2243 6f6e 7465 6e74 2d54  ders={"Content-T
-000021f0: 7970 6522 3a20 2261 7070 6c69 6361 7469  ype": "applicati
-00002200: 6f6e 2f6a 736f 6e22 2c20 2241 7574 686f  on/json", "Autho
-00002210: 7269 7a61 7469 6f6e 223a 2061 7069 5f6b  rization": api_k
-00002220: 6579 7d2c 0a20 2020 2029 0a20 2020 2063  ey},.    ).    c
-00002230: 6865 636b 5f72 6573 706f 6e73 6528 722c  heck_response(r,
-00002240: 2075 726c 2c20 2243 4b41 4e20 4461 7461   url, "CKAN Data
-00002250: 5374 6f72 6522 290a 2020 2020 7265 7475  Store").    retu
-00002260: 726e 2072 2e6a 736f 6e28 290a 0a0a 6465  rn r.json()...de
-00002270: 6620 7570 6461 7465 5f72 6573 6f75 7263  f update_resourc
-00002280: 6528 7265 736f 7572 6365 2c20 6170 695f  e(resource, api_
-00002290: 6b65 792c 2063 6b61 6e5f 7572 6c29 3a0a  key, ckan_url):.
-000022a0: 2020 2020 2222 220a 2020 2020 5570 6461      """.    Upda
-000022b0: 7465 2077 6562 7374 6f72 655f 7572 6c20  te webstore_url 
-000022c0: 616e 6420 7765 6273 746f 7265 5f6c 6173  and webstore_las
-000022d0: 745f 7570 6461 7465 6420 696e 2043 4b41  t_updated in CKA
-000022e0: 4e0a 2020 2020 2222 220a 0a20 2020 2075  N.    """..    u
-000022f0: 726c 203d 2067 6574 5f75 726c 2822 7265  rl = get_url("re
-00002300: 736f 7572 6365 5f75 7064 6174 6522 2c20  source_update", 
-00002310: 636b 616e 5f75 726c 290a 2020 2020 7220  ckan_url).    r 
-00002320: 3d20 7265 7175 6573 7473 2e70 6f73 7428  = requests.post(
-00002330: 0a20 2020 2020 2020 2075 726c 2c0a 2020  .        url,.  
-00002340: 2020 2020 2020 7665 7269 6679 3d63 6f6e        verify=con
-00002350: 6669 672e 6765 7428 2253 534c 5f56 4552  fig.get("SSL_VER
-00002360: 4946 5922 292c 0a20 2020 2020 2020 2064  IFY"),.        d
-00002370: 6174 613d 6a73 6f6e 2e64 756d 7073 2872  ata=json.dumps(r
-00002380: 6573 6f75 7263 6529 2c0a 2020 2020 2020  esource),.      
-00002390: 2020 6865 6164 6572 733d 7b22 436f 6e74    headers={"Cont
-000023a0: 656e 742d 5479 7065 223a 2022 6170 706c  ent-Type": "appl
-000023b0: 6963 6174 696f 6e2f 6a73 6f6e 222c 2022  ication/json", "
-000023c0: 4175 7468 6f72 697a 6174 696f 6e22 3a20  Authorization": 
-000023d0: 6170 695f 6b65 797d 2c0a 2020 2020 290a  api_key},.    ).
-000023e0: 0a20 2020 2063 6865 636b 5f72 6573 706f  .    check_respo
-000023f0: 6e73 6528 722c 2075 726c 2c20 2243 4b41  nse(r, url, "CKA
-00002400: 4e22 290a 0a0a 6465 6620 6765 745f 7265  N")...def get_re
-00002410: 736f 7572 6365 2872 6573 6f75 7263 655f  source(resource_
-00002420: 6964 2c20 636b 616e 5f75 726c 2c20 6170  id, ckan_url, ap
-00002430: 695f 6b65 7929 3a0a 2020 2020 2222 220a  i_key):.    """.
-00002440: 2020 2020 4765 7473 2061 7661 696c 6162      Gets availab
-00002450: 6c65 2069 6e66 6f72 6d61 7469 6f6e 2061  le information a
-00002460: 626f 7574 2074 6865 2072 6573 6f75 7263  bout the resourc
-00002470: 6520 6672 6f6d 2043 4b41 4e0a 2020 2020  e from CKAN.    
-00002480: 2222 220a 2020 2020 7572 6c20 3d20 6765  """.    url = ge
-00002490: 745f 7572 6c28 2272 6573 6f75 7263 655f  t_url("resource_
-000024a0: 7368 6f77 222c 2063 6b61 6e5f 7572 6c29  show", ckan_url)
-000024b0: 0a20 2020 2072 203d 2072 6571 7565 7374  .    r = request
-000024c0: 732e 706f 7374 280a 2020 2020 2020 2020  s.post(.        
-000024d0: 7572 6c2c 0a20 2020 2020 2020 2076 6572  url,.        ver
-000024e0: 6966 793d 636f 6e66 6967 2e67 6574 2822  ify=config.get("
-000024f0: 5353 4c5f 5645 5249 4659 2229 2c0a 2020  SSL_VERIFY"),.  
-00002500: 2020 2020 2020 6461 7461 3d6a 736f 6e2e        data=json.
-00002510: 6475 6d70 7328 7b22 6964 223a 2072 6573  dumps({"id": res
-00002520: 6f75 7263 655f 6964 7d29 2c0a 2020 2020  ource_id}),.    
-00002530: 2020 2020 6865 6164 6572 733d 7b22 436f      headers={"Co
-00002540: 6e74 656e 742d 5479 7065 223a 2022 6170  ntent-Type": "ap
-00002550: 706c 6963 6174 696f 6e2f 6a73 6f6e 222c  plication/json",
-00002560: 2022 4175 7468 6f72 697a 6174 696f 6e22   "Authorization"
-00002570: 3a20 6170 695f 6b65 797d 2c0a 2020 2020  : api_key},.    
-00002580: 290a 2020 2020 6368 6563 6b5f 7265 7370  ).    check_resp
-00002590: 6f6e 7365 2872 2c20 7572 6c2c 2022 434b  onse(r, url, "CK
-000025a0: 414e 2229 0a0a 2020 2020 7265 7475 726e  AN")..    return
-000025b0: 2072 2e6a 736f 6e28 295b 2272 6573 756c   r.json()["resul
-000025c0: 7422 5d0a 0a0a 6465 6620 6765 745f 7061  t"]...def get_pa
-000025d0: 636b 6167 6528 7061 636b 6167 655f 6964  ckage(package_id
-000025e0: 2c20 636b 616e 5f75 726c 2c20 6170 695f  , ckan_url, api_
-000025f0: 6b65 7929 3a0a 2020 2020 2222 220a 2020  key):.    """.  
-00002600: 2020 4765 7473 2061 7661 696c 6162 6c65    Gets available
-00002610: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-00002620: 7574 2061 2070 6163 6b61 6765 2066 726f  ut a package fro
-00002630: 6d20 434b 414e 0a20 2020 2022 2222 0a20  m CKAN.    """. 
-00002640: 2020 2075 726c 203d 2067 6574 5f75 726c     url = get_url
-00002650: 2822 7061 636b 6167 655f 7368 6f77 222c  ("package_show",
-00002660: 2063 6b61 6e5f 7572 6c29 0a20 2020 2072   ckan_url).    r
-00002670: 203d 2072 6571 7565 7374 732e 706f 7374   = requests.post
-00002680: 280a 2020 2020 2020 2020 7572 6c2c 0a20  (.        url,. 
-00002690: 2020 2020 2020 2076 6572 6966 793d 636f         verify=co
-000026a0: 6e66 6967 2e67 6574 2822 5353 4c5f 5645  nfig.get("SSL_VE
-000026b0: 5249 4659 2229 2c0a 2020 2020 2020 2020  RIFY"),.        
-000026c0: 6461 7461 3d6a 736f 6e2e 6475 6d70 7328  data=json.dumps(
-000026d0: 7b22 6964 223a 2070 6163 6b61 6765 5f69  {"id": package_i
-000026e0: 647d 292c 0a20 2020 2020 2020 2068 6561  d}),.        hea
-000026f0: 6465 7273 3d7b 2243 6f6e 7465 6e74 2d54  ders={"Content-T
-00002700: 7970 6522 3a20 2261 7070 6c69 6361 7469  ype": "applicati
-00002710: 6f6e 2f6a 736f 6e22 2c20 2241 7574 686f  on/json", "Autho
-00002720: 7269 7a61 7469 6f6e 223a 2061 7069 5f6b  rization": api_k
-00002730: 6579 7d2c 0a20 2020 2029 0a20 2020 2063  ey},.    ).    c
-00002740: 6865 636b 5f72 6573 706f 6e73 6528 722c  heck_response(r,
-00002750: 2075 726c 2c20 2243 4b41 4e22 290a 0a20   url, "CKAN").. 
-00002760: 2020 2072 6574 7572 6e20 722e 6a73 6f6e     return r.json
-00002770: 2829 5b22 7265 7375 6c74 225d 0a0a 0a64  ()["result"]...d
-00002780: 6566 2076 616c 6964 6174 655f 696e 7075  ef validate_inpu
-00002790: 7428 696e 7075 7429 3a0a 2020 2020 2320  t(input):.    # 
-000027a0: 4573 7065 6369 616c 6c79 2076 616c 6964  Especially valid
-000027b0: 6174 6520 6d65 7461 6461 7461 2077 6869  ate metadata whi
-000027c0: 6368 2069 7320 7072 6f76 6964 6564 2062  ch is provided b
-000027d0: 7920 7468 6520 7573 6572 0a20 2020 2069  y the user.    i
-000027e0: 6620 226d 6574 6164 6174 6122 206e 6f74  f "metadata" not
-000027f0: 2069 6e20 696e 7075 743a 0a20 2020 2020   in input:.     
-00002800: 2020 2072 6169 7365 2075 7469 6c2e 4a6f     raise util.Jo
-00002810: 6245 7272 6f72 2822 4d65 7461 6461 7461  bError("Metadata
-00002820: 206d 6973 7369 6e67 2229 0a0a 2020 2020   missing")..    
-00002830: 6461 7461 203d 2069 6e70 7574 5b22 6d65  data = input["me
-00002840: 7461 6461 7461 225d 0a0a 2020 2020 6966  tadata"]..    if
-00002850: 2022 7265 736f 7572 6365 5f69 6422 206e   "resource_id" n
-00002860: 6f74 2069 6e20 6461 7461 3a0a 2020 2020  ot in data:.    
-00002870: 2020 2020 7261 6973 6520 7574 696c 2e4a      raise util.J
-00002880: 6f62 4572 726f 7228 224e 6f20 6964 2070  obError("No id p
-00002890: 726f 7669 6465 642e 2229 0a20 2020 2069  rovided.").    i
-000028a0: 6620 2263 6b61 6e5f 7572 6c22 206e 6f74  f "ckan_url" not
-000028b0: 2069 6e20 6461 7461 3a0a 2020 2020 2020   in data:.      
-000028c0: 2020 7261 6973 6520 7574 696c 2e4a 6f62    raise util.Job
-000028d0: 4572 726f 7228 224e 6f20 636b 616e 5f75  Error("No ckan_u
-000028e0: 726c 2070 726f 7669 6465 642e 2229 0a20  rl provided."). 
-000028f0: 2020 2069 6620 6e6f 7420 696e 7075 742e     if not input.
-00002900: 6765 7428 2261 7069 5f6b 6579 2229 3a0a  get("api_key"):.
-00002910: 2020 2020 2020 2020 7261 6973 6520 7574          raise ut
-00002920: 696c 2e4a 6f62 4572 726f 7228 224e 6f20  il.JobError("No 
-00002930: 434b 414e 2041 5049 206b 6579 2070 726f  CKAN API key pro
-00002940: 7669 6465 6422 290a 0a0a 406a 6f62 2e61  vided")...@job.a
-00002950: 7379 6e63 6872 6f6e 6f75 730a 6465 6620  synchronous.def 
-00002960: 7075 7368 5f74 6f5f 6461 7461 7374 6f72  push_to_datastor
-00002970: 6528 7461 736b 5f69 642c 2069 6e70 7574  e(task_id, input
-00002980: 2c20 6472 795f 7275 6e3d 4661 6c73 6529  , dry_run=False)
-00002990: 3a0a 2020 2020 2222 2244 6f77 6e6c 6f61  :.    """Downloa
-000029a0: 6420 616e 6420 7061 7273 6520 6120 7265  d and parse a re
-000029b0: 736f 7572 6365 2070 7573 6820 6974 7320  source push its 
-000029c0: 6461 7461 2069 6e74 6f20 434b 414e 2773  data into CKAN's
-000029d0: 2044 6174 6153 746f 7265 2e0a 0a20 2020   DataStore...   
-000029e0: 2041 6e20 6173 796e 6368 726f 6e6f 7573   An asynchronous
-000029f0: 206a 6f62 2074 6861 7420 6765 7473 2061   job that gets a
-00002a00: 2072 6573 6f75 7263 6520 6672 6f6d 2043   resource from C
-00002a10: 4b41 4e2c 2064 6f77 6e6c 6f61 6473 2074  KAN, downloads t
-00002a20: 6865 0a20 2020 2072 6573 6f75 7263 6527  he.    resource'
-00002a30: 7320 6461 7461 2066 696c 6520 616e 642c  s data file and,
-00002a40: 2069 6620 7468 6520 6461 7461 2066 696c   if the data fil
-00002a50: 6520 6861 7320 6368 616e 6765 6420 7369  e has changed si
-00002a60: 6e63 6520 6c61 7374 2074 696d 652c 0a20  nce last time,. 
-00002a70: 2020 2070 6172 7365 7320 7468 6520 6461     parses the da
-00002a80: 7461 2061 6e64 2070 6f73 7473 2069 7420  ta and posts it 
-00002a90: 696e 746f 2043 4b41 4e27 7320 4461 7461  into CKAN's Data
-00002aa0: 5374 6f72 652e 0a0a 2020 2020 3a70 6172  Store...    :par
-00002ab0: 616d 2064 7279 5f72 756e 3a20 4665 7463  am dry_run: Fetc
-00002ac0: 6820 616e 6420 7061 7273 6520 7468 6520  h and parse the 
-00002ad0: 6461 7461 2066 696c 6520 6275 7420 646f  data file but do
-00002ae0: 6e27 7420 6163 7475 616c 6c79 2070 6f73  n't actually pos
-00002af0: 7420 7468 650a 2020 2020 2020 2020 6461  t the.        da
-00002b00: 7461 2074 6f20 7468 6520 4461 7461 5374  ta to the DataSt
-00002b10: 6f72 652c 2069 6e73 7465 6164 2072 6574  ore, instead ret
-00002b20: 7572 6e20 7468 6520 6461 7461 2068 6561  urn the data hea
-00002b30: 6465 7273 2061 6e64 2072 6f77 7320 7468  ders and rows th
-00002b40: 6174 0a20 2020 2020 2020 2077 6f75 6c64  at.        would
-00002b50: 2068 6176 6520 6265 656e 2070 6f73 7465   have been poste
-00002b60: 642e 0a20 2020 203a 7479 7065 2064 7279  d..    :type dry
-00002b70: 5f72 756e 3a20 626f 6f6c 6561 6e0a 0a20  _run: boolean.. 
-00002b80: 2020 2022 2222 0a20 2020 2068 616e 646c     """.    handl
-00002b90: 6572 203d 2075 7469 6c2e 5374 6f72 696e  er = util.Storin
-00002ba0: 6748 616e 646c 6572 2874 6173 6b5f 6964  gHandler(task_id
-00002bb0: 2c20 696e 7075 7429 0a20 2020 206c 6f67  , input).    log
-00002bc0: 6765 7220 3d20 6c6f 6767 696e 672e 6765  ger = logging.ge
-00002bd0: 744c 6f67 6765 7228 7461 736b 5f69 6429  tLogger(task_id)
-00002be0: 0a20 2020 206c 6f67 6765 722e 6164 6448  .    logger.addH
-00002bf0: 616e 646c 6572 2868 616e 646c 6572 290a  andler(handler).
-00002c00: 2020 2020 6c6f 6767 6572 2e73 6574 4c65      logger.setLe
-00002c10: 7665 6c28 6c6f 6767 696e 672e 4445 4255  vel(logging.DEBU
-00002c20: 4729 0a0a 2020 2020 2320 6368 6563 6b20  G)..    # check 
-00002c30: 6966 2051 5356 5f42 494e 2065 7869 7374  if QSV_BIN exist
-00002c40: 730a 2020 2020 7173 765f 6269 6e20 3d20  s.    qsv_bin = 
-00002c50: 636f 6e66 6967 2e67 6574 2822 5153 565f  config.get("QSV_
-00002c60: 4249 4e22 290a 2020 2020 7173 765f 7061  BIN").    qsv_pa
-00002c70: 7468 203d 2050 6174 6828 7173 765f 6269  th = Path(qsv_bi
-00002c80: 6e29 0a20 2020 2069 6620 6e6f 7420 7173  n).    if not qs
-00002c90: 765f 7061 7468 2e69 735f 6669 6c65 2829  v_path.is_file()
-00002ca0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00002cb0: 7574 696c 2e4a 6f62 4572 726f 7228 227b  util.JobError("{
-00002cc0: 7d20 6e6f 7420 666f 756e 642e 222e 666f  } not found.".fo
-00002cd0: 726d 6174 2863 6f6e 6669 672e 6765 7428  rmat(config.get(
-00002ce0: 2251 5356 5f42 494e 2229 2929 0a0a 2020  "QSV_BIN")))..  
-00002cf0: 2020 7661 6c69 6461 7465 5f69 6e70 7574    validate_input
-00002d00: 2869 6e70 7574 290a 0a20 2020 2064 6174  (input)..    dat
-00002d10: 6120 3d20 696e 7075 745b 226d 6574 6164  a = input["metad
-00002d20: 6174 6122 5d0a 0a20 2020 2063 6b61 6e5f  ata"]..    ckan_
-00002d30: 7572 6c20 3d20 6461 7461 5b22 636b 616e  url = data["ckan
-00002d40: 5f75 726c 225d 0a20 2020 2072 6573 6f75  _url"].    resou
-00002d50: 7263 655f 6964 203d 2064 6174 615b 2272  rce_id = data["r
-00002d60: 6573 6f75 7263 655f 6964 225d 0a20 2020  esource_id"].   
-00002d70: 2061 7069 5f6b 6579 203d 2069 6e70 7574   api_key = input
-00002d80: 2e67 6574 2822 6170 695f 6b65 7922 290a  .get("api_key").
-00002d90: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
-00002da0: 2020 7265 736f 7572 6365 203d 2067 6574    resource = get
-00002db0: 5f72 6573 6f75 7263 6528 7265 736f 7572  _resource(resour
-00002dc0: 6365 5f69 642c 2063 6b61 6e5f 7572 6c2c  ce_id, ckan_url,
-00002dd0: 2061 7069 5f6b 6579 290a 2020 2020 6578   api_key).    ex
-00002de0: 6365 7074 2075 7469 6c2e 4a6f 6245 7272  cept util.JobErr
-00002df0: 6f72 3a0a 2020 2020 2020 2020 2320 7472  or:.        # tr
-00002e00: 7920 6167 6169 6e20 696e 2035 2073 6563  y again in 5 sec
-00002e10: 6f6e 6473 206a 7573 7420 696e 6361 7365  onds just incase
-00002e20: 2043 4b41 4e20 6973 2073 6c6f 7720 6174   CKAN is slow at
-00002e30: 2061 6464 696e 6720 7265 736f 7572 6365   adding resource
-00002e40: 0a20 2020 2020 2020 2074 696d 652e 736c  .        time.sl
-00002e50: 6565 7028 3529 0a20 2020 2020 2020 2072  eep(5).        r
-00002e60: 6573 6f75 7263 6520 3d20 6765 745f 7265  esource = get_re
-00002e70: 736f 7572 6365 2872 6573 6f75 7263 655f  source(resource_
-00002e80: 6964 2c20 636b 616e 5f75 726c 2c20 6170  id, ckan_url, ap
-00002e90: 695f 6b65 7929 0a0a 2020 2020 2320 6368  i_key)..    # ch
-00002ea0: 6563 6b20 6966 2074 6865 2072 6573 6f75  eck if the resou
-00002eb0: 7263 6520 7572 6c5f 7479 7065 2069 7320  rce url_type is 
-00002ec0: 6120 6461 7461 7374 6f72 650a 2020 2020  a datastore.    
-00002ed0: 6966 2072 6573 6f75 7263 652e 6765 7428  if resource.get(
-00002ee0: 2275 726c 5f74 7970 6522 2920 3d3d 2022  "url_type") == "
-00002ef0: 6461 7461 7374 6f72 6522 3a0a 2020 2020  datastore":.    
-00002f00: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00002f10: 2244 756d 7020 6669 6c65 7320 6172 6520  "Dump files are 
-00002f20: 6d61 6e61 6765 6420 7769 7468 2074 6865  managed with the
-00002f30: 2044 6174 6173 746f 7265 2041 5049 2229   Datastore API")
-00002f40: 0a20 2020 2020 2020 2072 6574 7572 6e0a  .        return.
-00002f50: 0a20 2020 2023 2063 6865 636b 2073 6368  .    # check sch
-00002f60: 656d 650a 2020 2020 7572 6c20 3d20 7265  eme.    url = re
-00002f70: 736f 7572 6365 2e67 6574 2822 7572 6c22  source.get("url"
-00002f80: 290a 2020 2020 7363 6865 6d65 203d 2075  ).    scheme = u
-00002f90: 726c 7370 6c69 7428 7572 6c29 2e73 6368  rlsplit(url).sch
-00002fa0: 656d 650a 2020 2020 6966 2073 6368 656d  eme.    if schem
-00002fb0: 6520 6e6f 7420 696e 2028 2268 7474 7022  e not in ("http"
-00002fc0: 2c20 2268 7474 7073 222c 2022 6674 7022  , "https", "ftp"
-00002fd0: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00002fe0: 2075 7469 6c2e 4a6f 6245 7272 6f72 2822   util.JobError("
-00002ff0: 4f6e 6c79 2068 7474 702c 2068 7474 7073  Only http, https
-00003000: 2c20 616e 6420 6674 7020 7265 736f 7572  , and ftp resour
-00003010: 6365 7320 6d61 7920 6265 2066 6574 6368  ces may be fetch
-00003020: 6564 2e22 290a 0a20 2020 2074 696d 6572  ed.")..    timer
-00003030: 5f73 7461 7274 203d 2074 696d 652e 7065  _start = time.pe
-00003040: 7266 5f63 6f75 6e74 6572 2829 0a0a 2020  rf_counter()..  
-00003050: 2020 2320 6665 7463 6820 7468 6520 7265    # fetch the re
-00003060: 736f 7572 6365 2064 6174 610a 2020 2020  source data.    
-00003070: 6c6f 6767 6572 2e69 6e66 6f28 2246 6574  logger.info("Fet
-00003080: 6368 696e 6720 6672 6f6d 3a20 7b30 7d2e  ching from: {0}.
-00003090: 2e2e 222e 666f 726d 6174 2875 726c 2929  ..".format(url))
-000030a0: 0a20 2020 2068 6561 6465 7273 203d 207b  .    headers = {
-000030b0: 7d0a 2020 2020 7072 6576 6965 775f 726f  }.    preview_ro
-000030c0: 7773 203d 2069 6e74 2863 6f6e 6669 672e  ws = int(config.
-000030d0: 6765 7428 2250 5245 5649 4557 5f52 4f57  get("PREVIEW_ROW
-000030e0: 5322 2929 0a20 2020 2064 6f77 6e6c 6f61  S")).    downloa
-000030f0: 645f 7072 6576 6965 775f 6f6e 6c79 203d  d_preview_only =
-00003100: 2063 6f6e 6669 672e 6765 7428 2244 4f57   config.get("DOW
-00003110: 4e4c 4f41 445f 5052 4556 4945 575f 4f4e  NLOAD_PREVIEW_ON
-00003120: 4c59 2229 0a20 2020 2069 6620 7265 736f  LY").    if reso
-00003130: 7572 6365 2e67 6574 2822 7572 6c5f 7479  urce.get("url_ty
-00003140: 7065 2229 203d 3d20 2275 706c 6f61 6422  pe") == "upload"
-00003150: 3a0a 2020 2020 2020 2020 2320 4966 2074  :.        # If t
-00003160: 6869 7320 6973 2061 6e20 7570 6c6f 6164  his is an upload
-00003170: 6564 2066 696c 6520 746f 2043 4b41 4e2c  ed file to CKAN,
-00003180: 2061 7574 6865 6e74 6963 6174 6520 7468   authenticate th
-00003190: 6520 7265 7175 6573 742c 0a20 2020 2020  e request,.     
-000031a0: 2020 2023 206f 7468 6572 7769 7365 2077     # otherwise w
-000031b0: 6520 776f 6e27 7420 6765 7420 6669 6c65  e won't get file
-000031c0: 2066 726f 6d20 7072 6976 6174 6520 7265   from private re
-000031d0: 736f 7572 6365 730a 2020 2020 2020 2020  sources.        
-000031e0: 6865 6164 6572 735b 2241 7574 686f 7269  headers["Authori
-000031f0: 7a61 7469 6f6e 225d 203d 2061 7069 5f6b  zation"] = api_k
-00003200: 6579 0a20 2020 2074 7279 3a0a 2020 2020  ey.    try:.    
-00003210: 2020 2020 6b77 6172 6773 203d 207b 0a20      kwargs = {. 
-00003220: 2020 2020 2020 2020 2020 2022 6865 6164             "head
-00003230: 6572 7322 3a20 6865 6164 6572 732c 0a20  ers": headers,. 
-00003240: 2020 2020 2020 2020 2020 2022 7469 6d65             "time
-00003250: 6f75 7422 3a20 636f 6e66 6967 2e67 6574  out": config.get
-00003260: 2822 444f 574e 4c4f 4144 5f54 494d 454f  ("DOWNLOAD_TIMEO
-00003270: 5554 2229 2c0a 2020 2020 2020 2020 2020  UT"),.          
-00003280: 2020 2276 6572 6966 7922 3a20 636f 6e66    "verify": conf
-00003290: 6967 2e67 6574 2822 5353 4c5f 5645 5249  ig.get("SSL_VERI
-000032a0: 4659 2229 2c0a 2020 2020 2020 2020 2020  FY"),.          
-000032b0: 2020 2273 7472 6561 6d22 3a20 5472 7565    "stream": True
-000032c0: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
-000032d0: 2020 2020 6966 2055 5345 5f50 524f 5859      if USE_PROXY
-000032e0: 3a0a 2020 2020 2020 2020 2020 2020 6b77  :.            kw
-000032f0: 6172 6773 5b22 7072 6f78 6965 7322 5d20  args["proxies"] 
-00003300: 3d20 7b22 6874 7470 223a 2044 4f57 4e4c  = {"http": DOWNL
-00003310: 4f41 445f 5052 4f58 592c 2022 6874 7470  OAD_PROXY, "http
-00003320: 7322 3a20 444f 574e 4c4f 4144 5f50 524f  s": DOWNLOAD_PRO
-00003330: 5859 7d0a 2020 2020 2020 2020 7265 7370  XY}.        resp
-00003340: 6f6e 7365 203d 2072 6571 7565 7374 732e  onse = requests.
-00003350: 6765 7428 7572 6c2c 202a 2a6b 7761 7267  get(url, **kwarg
-00003360: 7329 0a20 2020 2020 2020 2072 6573 706f  s).        respo
-00003370: 6e73 652e 7261 6973 655f 666f 725f 7374  nse.raise_for_st
-00003380: 6174 7573 2829 0a0a 2020 2020 2020 2020  atus()..        
-00003390: 636c 203d 2072 6573 706f 6e73 652e 6865  cl = response.he
-000033a0: 6164 6572 732e 6765 7428 2263 6f6e 7465  aders.get("conte
-000033b0: 6e74 2d6c 656e 6774 6822 290a 2020 2020  nt-length").    
-000033c0: 2020 2020 6d61 785f 636f 6e74 656e 745f      max_content_
-000033d0: 6c65 6e67 7468 203d 2069 6e74 2863 6f6e  length = int(con
-000033e0: 6669 672e 6765 7428 224d 4158 5f43 4f4e  fig.get("MAX_CON
-000033f0: 5445 4e54 5f4c 454e 4754 4822 2929 0a20  TENT_LENGTH")). 
-00003400: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00003410: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
-00003420: 2020 2020 2020 2020 2020 2020 2063 6c0a               cl.
-00003430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003440: 616e 6420 696e 7428 636c 2920 3e20 6d61  and int(cl) > ma
-00003450: 785f 636f 6e74 656e 745f 6c65 6e67 7468  x_content_length
-00003460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003470: 2061 6e64 2028 7072 6576 6965 775f 726f   and (preview_ro
-00003480: 7773 203e 2030 2061 6e64 206e 6f74 2064  ws > 0 and not d
-00003490: 6f77 6e6c 6f61 645f 7072 6576 6965 775f  ownload_preview_
-000034a0: 6f6e 6c79 290a 2020 2020 2020 2020 2020  only).          
-000034b0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
-000034c0: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
-000034d0: 4a6f 6245 7272 6f72 280a 2020 2020 2020  JobError(.      
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2252                "R
-000034f0: 6573 6f75 7263 6520 746f 6f20 6c61 7267  esource too larg
-00003500: 6520 746f 2064 6f77 6e6c 6f61 643a 207b  e to download: {
-00003510: 636c 3a2e 324d 427d 203e 206d 6178 2028  cl:.2MB} > max (
-00003520: 7b6d 6178 5f63 6c3a 2e32 4d42 7d29 2e22  {max_cl:.2MB})."
-00003530: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003550: 2063 6c3d 4461 7461 5369 7a65 2869 6e74   cl=DataSize(int
-00003560: 2863 6c29 292c 206d 6178 5f63 6c3d 4461  (cl)), max_cl=Da
-00003570: 7461 5369 7a65 2869 6e74 286d 6178 5f63  taSize(int(max_c
-00003580: 6f6e 7465 6e74 5f6c 656e 6774 6829 290a  ontent_length)).
-00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035a0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000035b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000035c0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-000035d0: 723a 0a20 2020 2020 2020 2020 2020 2070  r:.            p
-000035e0: 6173 730a 0a20 2020 2020 2020 2074 6d70  ass..        tmp
-000035f0: 203d 2074 656d 7066 696c 652e 4e61 6d65   = tempfile.Name
-00003600: 6454 656d 706f 7261 7279 4669 6c65 2873  dTemporaryFile(s
-00003610: 7566 6669 783d 222e 2220 2b20 7265 736f  uffix="." + reso
-00003620: 7572 6365 2e67 6574 2822 666f 726d 6174  urce.get("format
-00003630: 2229 2e6c 6f77 6572 2829 290a 2020 2020  ").lower()).    
-00003640: 2020 2020 6c65 6e67 7468 203d 2030 0a20      length = 0. 
-00003650: 2020 2020 2020 206d 203d 2068 6173 686c         m = hashl
-00003660: 6962 2e6d 6435 2829 0a0a 2020 2020 2020  ib.md5()..      
-00003670: 2020 6966 2064 6f77 6e6c 6f61 645f 7072    if download_pr
-00003680: 6576 6965 775f 6f6e 6c79 2061 6e64 2070  eview_only and p
-00003690: 7265 7669 6577 5f72 6f77 7320 3e20 303a  review_rows > 0:
-000036a0: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
-000036b0: 6620 646f 776e 6c6f 6164 5f70 7265 7669  f download_previ
-000036c0: 6577 5f6f 6e6c 7920 616e 6420 7072 6576  ew_only and prev
-000036d0: 6965 775f 726f 7773 2069 7320 6772 6561  iew_rows is grea
-000036e0: 7465 7220 7468 616e 207a 6572 6f0a 2020  ter than zero.  
-000036f0: 2020 2020 2020 2020 2020 2320 7765 2772            # we'r
-00003700: 6520 646f 776e 6c6f 6164 696e 6720 7468  e downloading th
-00003710: 6520 7072 6576 6965 7720 726f 7773 206f  e preview rows o
-00003720: 6e6c 792c 206e 6f74 2074 6865 2077 686f  nly, not the who
-00003730: 6c65 2066 696c 650a 2020 2020 2020 2020  le file.        
-00003740: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-00003750: 2244 6f77 6e6c 6f61 6469 6e67 207b 3a2c  "Downloading {:,
-00003760: 7d2d 726f 7720 7072 6576 6965 772e 2e2e  }-row preview...
-00003770: 222e 666f 726d 6174 2870 7265 7669 6577  ".format(preview
-00003780: 5f72 6f77 7329 290a 0a20 2020 2020 2020  _rows))..       
-00003790: 2020 2020 2063 7572 725f 6c69 6e65 203d       curr_line =
-000037a0: 2030 0a20 2020 2020 2020 2020 2020 2066   0.            f
-000037b0: 6f72 206c 696e 6520 696e 2072 6573 706f  or line in respo
-000037c0: 6e73 652e 6974 6572 5f6c 696e 6573 2869  nse.iter_lines(i
-000037d0: 6e74 2863 6f6e 6669 672e 6765 7428 2243  nt(config.get("C
-000037e0: 4855 4e4b 5f53 495a 4522 2929 293a 0a20  HUNK_SIZE"))):. 
-000037f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003800: 7572 725f 6c69 6e65 202b 3d20 310a 2020  urr_line += 1.  
-00003810: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00003820: 6164 6420 6261 636b 2074 6865 206c 696e  add back the lin
-00003830: 6566 6565 6420 6173 2069 7465 725f 6c69  efeed as iter_li
-00003840: 6e65 7320 7265 6d6f 7665 7320 6974 0a20  nes removes it. 
-00003850: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00003860: 696e 6520 3d20 6c69 6e65 202b 2022 5c6e  ine = line + "\n
-00003870: 222e 656e 636f 6465 2822 6173 6369 6922  ".encode("ascii"
-00003880: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003890: 2020 6c65 6e67 7468 202b 3d20 6c65 6e28    length += len(
-000038a0: 6c69 6e65 290a 0a20 2020 2020 2020 2020  line)..         
-000038b0: 2020 2020 2020 2074 6d70 2e77 7269 7465         tmp.write
-000038c0: 286c 696e 6529 0a20 2020 2020 2020 2020  (line).         
-000038d0: 2020 2020 2020 206d 2e75 7064 6174 6528         m.update(
-000038e0: 6c69 6e65 290a 2020 2020 2020 2020 2020  line).          
-000038f0: 2020 2020 2020 6966 2063 7572 725f 6c69        if curr_li
-00003900: 6e65 203e 2070 7265 7669 6577 5f72 6f77  ne > preview_row
-00003910: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00003920: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00003930: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00003940: 2020 2020 2020 2023 2064 6f77 6e6c 6f61         # downloa
-00003950: 6420 7468 6520 656e 7469 7265 2066 696c  d the entire fil
-00003960: 6520 6f74 6865 7277 6973 650a 2020 2020  e otherwise.    
-00003970: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-00003980: 6861 6e64 6c65 2077 6865 6e20 7072 6576  handle when prev
-00003990: 6965 775f 726f 7773 2069 7320 6e65 6761  iew_rows is nega
-000039a0: 7469 7665 2028 6765 7420 7468 6520 7072  tive (get the pr
-000039b0: 6576 6965 7720 6672 6f6d 2074 6865 0a20  eview from the. 
-000039c0: 2020 2020 2020 2020 2020 2023 2065 6e64             # end
-000039d0: 206f 6620 7468 6520 6669 6c65 2920 736f   of the file) so
-000039e0: 2077 6520 7573 6520 6874 7470 2072 616e   we use http ran
-000039f0: 6765 2072 6571 7565 7374 2074 6f20 6765  ge request to ge
-00003a00: 7420 7468 6520 7072 6576 6965 7720 6672  t the preview fr
-00003a10: 6f6d 0a20 2020 2020 2020 2020 2020 2023  om.            #
-00003a20: 2074 6865 2065 6e64 2077 6974 686f 7574   the end without
-00003a30: 2064 6f77 6e6c 6f61 6469 6e67 2074 6865   downloading the
-00003a40: 2065 6e74 6972 6520 6669 6c65 0a20 2020   entire file.   
-00003a50: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00003a60: 696e 666f 2822 446f 776e 6c6f 6164 696e  info("Downloadin
-00003a70: 6720 7b3a 2e32 4d42 7d20 6669 6c65 2e2e  g {:.2MB} file..
-00003a80: 2e22 2e66 6f72 6d61 7428 4461 7461 5369  .".format(DataSi
-00003a90: 7a65 2869 6e74 2863 6c29 2929 290a 0a20  ze(int(cl)))).. 
-00003aa0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00003ab0: 6875 6e6b 2069 6e20 7265 7370 6f6e 7365  hunk in response
-00003ac0: 2e69 7465 725f 636f 6e74 656e 7428 696e  .iter_content(in
-00003ad0: 7428 636f 6e66 6967 2e67 6574 2822 4348  t(config.get("CH
-00003ae0: 554e 4b5f 5349 5a45 2229 2929 3a0a 2020  UNK_SIZE"))):.  
-00003af0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00003b00: 6e67 7468 202b 3d20 6c65 6e28 6368 756e  ngth += len(chun
-00003b10: 6b29 0a20 2020 2020 2020 2020 2020 2020  k).             
-00003b20: 2020 2069 6620 6c65 6e67 7468 203e 206d     if length > m
-00003b30: 6178 5f63 6f6e 7465 6e74 5f6c 656e 6774  ax_content_lengt
-00003b40: 6820 616e 6420 6e6f 7420 7072 6576 6965  h and not previe
-00003b50: 775f 726f 7773 3a0a 2020 2020 2020 2020  w_rows:.        
-00003b60: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00003b70: 6520 7574 696c 2e4a 6f62 4572 726f 7228  e util.JobError(
-00003b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003b90: 2020 2020 2020 2020 2022 5265 736f 7572           "Resour
-00003ba0: 6365 2074 6f6f 206c 6172 6765 2074 6f20  ce too large to 
-00003bb0: 7072 6f63 6573 733a 207b 636c 7d20 3e20  process: {cl} > 
-00003bc0: 6d61 7820 287b 6d61 785f 636c 7d29 2e22  max ({max_cl})."
-00003bd0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bf0: 2020 2020 2063 6c3d 6c65 6e67 7468 2c20       cl=length, 
-00003c00: 6d61 785f 636c 3d6d 6178 5f63 6f6e 7465  max_cl=max_conte
-00003c10: 6e74 5f6c 656e 6774 680a 2020 2020 2020  nt_length.      
-00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c30: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00003c40: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00003c50: 2020 2020 2020 2020 2020 746d 702e 7772            tmp.wr
-00003c60: 6974 6528 6368 756e 6b29 0a20 2020 2020  ite(chunk).     
-00003c70: 2020 2020 2020 2020 2020 206d 2e75 7064             m.upd
-00003c80: 6174 6528 6368 756e 6b29 0a0a 2020 2020  ate(chunk)..    
-00003c90: 2020 2020 6374 203d 2072 6573 706f 6e73      ct = respons
-00003ca0: 652e 6865 6164 6572 732e 6765 7428 2263  e.headers.get("c
-00003cb0: 6f6e 7465 6e74 2d74 7970 6522 2c20 2222  ontent-type", ""
-00003cc0: 292e 7370 6c69 7428 223b 222c 2031 295b  ).split(";", 1)[
-00003cd0: 305d 0a20 2020 2065 7863 6570 7420 7265  0].    except re
-00003ce0: 7175 6573 7473 2e48 5454 5045 7272 6f72  quests.HTTPError
-00003cf0: 2061 7320 653a 0a20 2020 2020 2020 2072   as e:.        r
-00003d00: 6169 7365 2048 5454 5045 7272 6f72 280a  aise HTTPError(.
-00003d10: 2020 2020 2020 2020 2020 2020 2244 6174              "Dat
-00003d20: 6150 7573 6865 722b 2072 6563 6569 7665  aPusher+ receive
-00003d30: 6420 6120 6261 6420 4854 5450 2072 6573  d a bad HTTP res
-00003d40: 706f 6e73 6520 7768 656e 2074 7279 696e  ponse when tryin
-00003d50: 6720 746f 2064 6f77 6e6c 6f61 6420 220a  g to download ".
-00003d60: 2020 2020 2020 2020 2020 2020 2274 6865              "the
-00003d70: 2064 6174 6120 6669 6c65 222c 0a20 2020   data file",.   
-00003d80: 2020 2020 2020 2020 2073 7461 7475 735f           status_
-00003d90: 636f 6465 3d65 2e72 6573 706f 6e73 652e  code=e.response.
-00003da0: 7374 6174 7573 5f63 6f64 652c 0a20 2020  status_code,.   
-00003db0: 2020 2020 2020 2020 2072 6571 7565 7374           request
-00003dc0: 5f75 726c 3d75 726c 2c0a 2020 2020 2020  _url=url,.      
-00003dd0: 2020 2020 2020 7265 7370 6f6e 7365 3d65        response=e
-00003de0: 2e72 6573 706f 6e73 652e 636f 6e74 656e  .response.conten
-00003df0: 742c 0a20 2020 2020 2020 2029 0a20 2020  t,.        ).   
-00003e00: 2065 7863 6570 7420 7265 7175 6573 7473   except requests
-00003e10: 2e52 6571 7565 7374 4578 6365 7074 696f  .RequestExceptio
-00003e20: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
-00003e30: 7261 6973 6520 4854 5450 4572 726f 7228  raise HTTPError(
-00003e40: 0a20 2020 2020 2020 2020 2020 206d 6573  .            mes
-00003e50: 7361 6765 3d73 7472 2865 292c 2073 7461  sage=str(e), sta
-00003e60: 7475 735f 636f 6465 3d4e 6f6e 652c 2072  tus_code=None, r
-00003e70: 6571 7565 7374 5f75 726c 3d75 726c 2c20  equest_url=url, 
-00003e80: 7265 7370 6f6e 7365 3d4e 6f6e 650a 2020  response=None.  
-00003e90: 2020 2020 2020 290a 0a20 2020 2066 696c        )..    fil
-00003ea0: 655f 6861 7368 203d 206d 2e68 6578 6469  e_hash = m.hexdi
-00003eb0: 6765 7374 2829 0a20 2020 2074 6d70 2e73  gest().    tmp.s
-00003ec0: 6565 6b28 3029 0a0a 2020 2020 6966 2028  eek(0)..    if (
-00003ed0: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
-00003ee0: 652e 6765 7428 2268 6173 6822 2920 3d3d  e.get("hash") ==
-00003ef0: 2066 696c 655f 6861 7368 0a20 2020 2020   file_hash.     
-00003f00: 2020 2061 6e64 206e 6f74 2064 6174 612e     and not data.
-00003f10: 6765 7428 2269 676e 6f72 655f 6861 7368  get("ignore_hash
-00003f20: 2229 0a20 2020 2020 2020 2061 6e64 206e  ").        and n
-00003f30: 6f74 2063 6f6e 6669 672e 6765 7428 2249  ot config.get("I
-00003f40: 474e 4f52 455f 4649 4c45 5f48 4153 4822  GNORE_FILE_HASH"
-00003f50: 290a 2020 2020 293a 0a20 2020 2020 2020  ).    ):.       
-00003f60: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-00003f70: 0a20 2020 2020 2020 2020 2020 2022 5570  .            "Up
-00003f80: 6c6f 6164 2073 6b69 7070 6564 2061 7320  load skipped as 
-00003f90: 7468 6520 6669 6c65 2068 6173 6820 6861  the file hash ha
-00003fa0: 736e 2774 2063 6861 6e67 6564 3a20 7b68  sn't changed: {h
-00003fb0: 6173 687d 2e22 2e66 6f72 6d61 7428 0a20  ash}.".format(. 
-00003fc0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
-00003fd0: 6173 683d 6669 6c65 5f68 6173 680a 2020  ash=file_hash.  
-00003fe0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00003ff0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-00004000: 7475 726e 0a0a 2020 2020 7265 736f 7572  turn..    resour
-00004010: 6365 5b22 6861 7368 225d 203d 2066 696c  ce["hash"] = fil
-00004020: 655f 6861 7368 0a0a 2020 2020 6465 6620  e_hash..    def 
-00004030: 636c 6561 6e75 705f 7465 6d70 6669 6c65  cleanup_tempfile
-00004040: 7328 293a 0a20 2020 2020 2020 2023 2063  s():.        # c
-00004050: 6c65 616e 7570 2074 656d 706f 7261 7279  leanup temporary
-00004060: 2066 696c 6573 0a20 2020 2020 2020 2069   files.        i
-00004070: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
-00004080: 2874 6d70 2e6e 616d 6520 2b20 222e 6964  (tmp.name + ".id
-00004090: 7822 293a 0a20 2020 2020 2020 2020 2020  x"):.           
-000040a0: 206f 732e 7265 6d6f 7665 2874 6d70 2e6e   os.remove(tmp.n
-000040b0: 616d 6520 2b20 222e 6964 7822 290a 2020  ame + ".idx").  
-000040c0: 2020 2020 2020 746d 702e 636c 6f73 6528        tmp.close(
-000040d0: 290a 2020 2020 2020 2020 6966 2022 7173  ).        if "qs
-000040e0: 765f 736c 6963 655f 6373 7622 2069 6e20  v_slice_csv" in 
-000040f0: 676c 6f62 616c 7328 293a 0a20 2020 2020  globals():.     
-00004100: 2020 2020 2020 2071 7376 5f73 6c69 6365         qsv_slice
-00004110: 5f63 7376 2e63 6c6f 7365 2829 0a20 2020  _csv.close().   
-00004120: 2020 2020 2069 6620 2271 7376 5f65 7863       if "qsv_exc
-00004130: 656c 5f63 7376 2220 696e 2067 6c6f 6261  el_csv" in globa
-00004140: 6c73 2829 3a0a 2020 2020 2020 2020 2020  ls():.          
-00004150: 2020 7173 765f 6578 6365 6c5f 6373 762e    qsv_excel_csv.
-00004160: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-00004170: 6966 2022 7173 765f 696e 7075 745f 6373  if "qsv_input_cs
-00004180: 7622 2069 6e20 676c 6f62 616c 7328 293a  v" in globals():
-00004190: 0a20 2020 2020 2020 2020 2020 2071 7376  .            qsv
-000041a0: 5f69 6e70 7574 5f63 7376 2e63 6c6f 7365  _input_csv.close
-000041b0: 2829 0a20 2020 2020 2020 2069 6620 2271  ().        if "q
-000041c0: 7376 5f64 6564 7570 5f63 7376 2220 696e  sv_dedup_csv" in
-000041d0: 2067 6c6f 6261 6c73 2829 3a0a 2020 2020   globals():.    
-000041e0: 2020 2020 2020 2020 7173 765f 6465 6475          qsv_dedu
-000041f0: 705f 6373 762e 636c 6f73 6528 290a 2020  p_csv.close().  
-00004200: 2020 2020 2020 6966 2022 7173 765f 6865        if "qsv_he
-00004210: 6164 6572 7322 2069 6e20 676c 6f62 616c  aders" in global
-00004220: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
-00004230: 2071 7376 5f68 6561 6465 7273 2e63 6c6f   qsv_headers.clo
-00004240: 7365 2829 0a20 2020 2020 2020 2069 6620  se().        if 
-00004250: 2271 7376 5f73 6166 656e 616d 6573 5f63  "qsv_safenames_c
-00004260: 7376 2220 696e 2067 6c6f 6261 6c73 2829  sv" in globals()
-00004270: 3a0a 2020 2020 2020 2020 2020 2020 7173  :.            qs
-00004280: 765f 7361 6665 6e61 6d65 735f 6373 762e  v_safenames_csv.
-00004290: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-000042a0: 6966 2022 7173 765f 6170 706c 7964 705f  if "qsv_applydp_
-000042b0: 6373 7622 2069 6e20 676c 6f62 616c 7328  csv" in globals(
-000042c0: 293a 0a20 2020 2020 2020 2020 2020 2071  ):.            q
-000042d0: 7376 5f61 7070 6c79 6470 5f63 7376 2e63  sv_applydp_csv.c
-000042e0: 6c6f 7365 2829 0a20 2020 2020 2020 2069  lose().        i
-000042f0: 6620 2271 7376 5f73 7461 7473 5f63 7376  f "qsv_stats_csv
-00004300: 2220 696e 2067 6c6f 6261 6c73 2829 3a0a  " in globals():.
-00004310: 2020 2020 2020 2020 2020 2020 6966 2022              if "
-00004320: 7173 765f 696e 6465 785f 6669 6c65 2220  qsv_index_file" 
-00004330: 696e 2067 6c6f 6261 6c73 2829 3a0a 2020  in globals():.  
-00004340: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-00004350: 6561 6e75 705f 6964 7866 696c 6528 7173  eanup_idxfile(qs
-00004360: 765f 696e 6465 785f 6669 6c65 290a 2020  v_index_file).  
-00004370: 2020 2020 2020 2020 2020 7173 765f 7374            qsv_st
-00004380: 6174 735f 6373 762e 636c 6f73 6528 290a  ats_csv.close().
-00004390: 0a20 2020 2064 6566 2063 6c65 616e 7570  .    def cleanup
-000043a0: 5f69 6478 6669 6c65 2869 6478 6669 6c65  _idxfile(idxfile
-000043b0: 293a 0a20 2020 2020 2020 2069 6620 6f73  ):.        if os
-000043c0: 2e70 6174 682e 6578 6973 7473 2869 6478  .path.exists(idx
-000043d0: 6669 6c65 293a 0a20 2020 2020 2020 2020  file):.         
-000043e0: 2020 206f 732e 7265 6d6f 7665 2869 6478     os.remove(idx
-000043f0: 6669 6c65 290a 0a20 2020 2022 2222 0a20  file)..    """. 
-00004400: 2020 2053 7461 7274 2041 6e61 6c79 7369     Start Analysi
-00004410: 7320 7573 696e 6720 7173 7620 696e 7374  s using qsv inst
-00004420: 6561 6420 6f66 206d 6573 7379 7461 626c  ead of messytabl
-00004430: 6573 2c20 6173 2031 2920 6974 7320 7479  es, as 1) its ty
-00004440: 7065 2069 6e66 6572 656e 6365 7320 6172  pe inferences ar
-00004450: 6520 6275 6c6c 6574 2d70 726f 6f66 0a20  e bullet-proof. 
-00004460: 2020 206e 6f74 2067 7565 7373 6573 2061     not guesses a
-00004470: 7320 6974 2073 6361 6e73 2074 6865 2065  s it scans the e
-00004480: 6e74 6972 6520 6669 6c65 2c20 3229 2069  ntire file, 2) i
-00004490: 7473 2073 7570 6572 2d66 6173 742c 2061  ts super-fast, a
-000044a0: 6e64 2033 2920 6974 2068 6173 0a20 2020  nd 3) it has.   
-000044b0: 2061 6464 6c20 6461 7461 2d77 7261 6e67   addl data-wrang
-000044c0: 6c69 6e67 2063 6170 6162 696c 6974 6965  ling capabilitie
-000044d0: 7320 7765 2075 7365 2069 6e20 6461 7461  s we use in data
-000044e0: 7075 7368 6572 2b20 2d20 736c 6963 652c  pusher+ - slice,
-000044f0: 2069 6e70 7574 2c20 636f 756e 742c 2068   input, count, h
-00004500: 6561 6465 7273 2c20 6574 632e 0a20 2020  eaders, etc..   
-00004510: 2022 2222 0a20 2020 2066 6574 6368 5f65   """.    fetch_e
-00004520: 6c61 7073 6564 203d 2074 696d 652e 7065  lapsed = time.pe
-00004530: 7266 5f63 6f75 6e74 6572 2829 202d 2074  rf_counter() - t
-00004540: 696d 6572 5f73 7461 7274 0a20 2020 206c  imer_start.    l
-00004550: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
-00004560: 2020 2020 2246 6574 6368 6564 207b 3a2e      "Fetched {:.
-00004570: 324d 427d 2066 696c 6520 696e 207b 3a2c  2MB} file in {:,
-00004580: 2e32 667d 2073 6563 6f6e 6473 2e22 2e66  .2f} seconds.".f
-00004590: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-000045a0: 2020 2044 6174 6153 697a 6528 6c65 6e67     DataSize(leng
-000045b0: 7468 292c 2066 6574 6368 5f65 6c61 7073  th), fetch_elaps
-000045c0: 6564 0a20 2020 2020 2020 2029 0a20 2020  ed.        ).   
-000045d0: 2029 0a20 2020 2061 6e61 6c79 7369 735f   ).    analysis_
-000045e0: 7374 6172 7420 3d20 7469 6d65 2e70 6572  start = time.per
-000045f0: 665f 636f 756e 7465 7228 290a 2020 2020  f_counter().    
-00004600: 6c6f 6767 6572 2e69 6e66 6f28 2241 4e41  logger.info("ANA
-00004610: 4c59 5a49 4e47 2057 4954 4820 5153 562e  LYZING WITH QSV.
-00004620: 2e22 290a 0a20 2020 2023 2063 6865 636b  .")..    # check
-00004630: 2063 6f6e 7465 6e74 2074 7970 6520 6f72   content type or
-00004640: 2066 696c 6520 6578 7465 6e73 696f 6e20   file extension 
-00004650: 6966 2069 7473 2061 2073 7072 6561 6473  if its a spreads
-00004660: 6865 6574 0a20 2020 2073 7072 6561 6473  heet.    spreads
-00004670: 6865 6574 5f65 7874 656e 7369 6f6e 7320  heet_extensions 
-00004680: 3d20 5b22 584c 5322 2c20 2258 4c53 5822  = ["XLS", "XLSX"
-00004690: 2c20 224f 4453 222c 2022 584c 534d 222c  , "ODS", "XLSM",
-000046a0: 2022 584c 5342 225d 0a20 2020 2066 6f72   "XLSB"].    for
-000046b0: 6d61 7420 3d20 7265 736f 7572 6365 2e67  mat = resource.g
-000046c0: 6574 2822 666f 726d 6174 2229 2e75 7070  et("format").upp
-000046d0: 6572 2829 0a20 2020 2069 6620 666f 726d  er().    if form
-000046e0: 6174 2069 6e20 7370 7265 6164 7368 6565  at in spreadshee
-000046f0: 745f 6578 7465 6e73 696f 6e73 3a0a 2020  t_extensions:.  
-00004700: 2020 2020 2020 2320 6966 2073 6f2c 2065        # if so, e
-00004710: 7870 6f72 7420 6974 2061 7320 6120 6373  xport it as a cs
-00004720: 7620 6669 6c65 0a20 2020 2020 2020 206c  v file.        l
-00004730: 6f67 6765 722e 696e 666f 2822 436f 6e76  ogger.info("Conv
-00004740: 6572 7469 6e67 207b 7d20 746f 2043 5356  erting {} to CSV
-00004750: 2e2e 2e22 2e66 6f72 6d61 7428 666f 726d  ...".format(form
-00004760: 6174 2929 0a20 2020 2020 2020 2022 2222  at)).        """
-00004770: 0a20 2020 2020 2020 2066 6972 7374 2c20  .        first, 
-00004780: 7765 206e 6565 6420 6120 7465 6d70 6f72  we need a tempor
-00004790: 6172 7920 7370 7265 6164 7368 6565 7420  ary spreadsheet 
-000047a0: 6669 6c65 6e61 6d65 2077 6974 6820 7468  filename with th
-000047b0: 6520 7269 6768 7420 6669 6c65 2065 7874  e right file ext
-000047c0: 656e 7369 6f6e 0a20 2020 2020 2020 2077  ension.        w
-000047d0: 6520 6f6e 6c79 206e 6565 6420 7468 6520  e only need the 
-000047e0: 6669 6c65 6e61 6d65 2074 686f 7567 682c  filename though,
-000047f0: 2074 6861 7427 7320 7768 7920 7765 2072   that's why we r
-00004800: 656d 6f76 6520 6974 0a20 2020 2020 2020  emove it.       
-00004810: 2061 6e64 2063 7265 6174 6520 6120 6861   and create a ha
-00004820: 7264 6c69 6e6b 2074 6f20 7468 6520 6669  rdlink to the fi
-00004830: 6c65 2077 6520 676f 7420 6672 6f6d 2043  le we got from C
-00004840: 4b41 4e0a 2020 2020 2020 2020 2222 220a  KAN.        """.
-00004850: 2020 2020 2020 2020 7173 765f 7370 7265          qsv_spre
-00004860: 6164 7368 6565 7420 3d20 7465 6d70 6669  adsheet = tempfi
-00004870: 6c65 2e4e 616d 6564 5465 6d70 6f72 6172  le.NamedTemporar
-00004880: 7946 696c 6528 7375 6666 6978 3d22 2e22  yFile(suffix="."
-00004890: 202b 2066 6f72 6d61 7429 0a20 2020 2020   + format).     
-000048a0: 2020 206f 732e 7265 6d6f 7665 2871 7376     os.remove(qsv
-000048b0: 5f73 7072 6561 6473 6865 6574 2e6e 616d  _spreadsheet.nam
-000048c0: 6529 0a20 2020 2020 2020 206f 732e 6c69  e).        os.li
-000048d0: 6e6b 2874 6d70 2e6e 616d 652c 2071 7376  nk(tmp.name, qsv
-000048e0: 5f73 7072 6561 6473 6865 6574 2e6e 616d  _spreadsheet.nam
-000048f0: 6529 0a0a 2020 2020 2020 2020 2320 7275  e)..        # ru
-00004900: 6e20 6071 7376 2065 7863 656c 6020 616e  n `qsv excel` an
-00004910: 6420 6578 706f 7274 2069 7420 746f 2061  d export it to a
-00004920: 2043 5356 0a20 2020 2020 2020 2023 2075   CSV.        # u
-00004930: 7365 202d 2d74 7269 6d20 6f70 7469 6f6e  se --trim option
-00004940: 2074 6f20 7472 696d 2063 6f6c 756d 6e20   to trim column 
-00004950: 6e61 6d65 7320 616e 6420 7468 6520 6461  names and the da
-00004960: 7461 0a20 2020 2020 2020 2071 7376 5f65  ta.        qsv_e
-00004970: 7863 656c 5f63 7376 203d 2074 656d 7066  xcel_csv = tempf
-00004980: 696c 652e 4e61 6d65 6454 656d 706f 7261  ile.NamedTempora
-00004990: 7279 4669 6c65 2873 7566 6669 783d 222e  ryFile(suffix=".
-000049a0: 6373 7622 290a 2020 2020 2020 2020 6465  csv").        de
-000049b0: 6661 756c 745f 6578 6365 6c5f 7368 6565  fault_excel_shee
-000049c0: 7420 3d20 636f 6e66 6967 2e67 6574 2822  t = config.get("
-000049d0: 4445 4641 554c 545f 4558 4345 4c5f 5348  DEFAULT_EXCEL_SH
-000049e0: 4545 5422 290a 2020 2020 2020 2020 7472  EET").        tr
-000049f0: 793a 0a20 2020 2020 2020 2020 2020 2071  y:.            q
-00004a00: 7376 5f65 7863 656c 203d 2073 7562 7072  sv_excel = subpr
-00004a10: 6f63 6573 732e 7275 6e28 0a20 2020 2020  ocess.run(.     
-00004a20: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2071 7376 5f62 696e 2c0a 2020 2020 2020   qsv_bin,.      
-00004a50: 2020 2020 2020 2020 2020 2020 2020 2265                "e
-00004a60: 7863 656c 222c 0a20 2020 2020 2020 2020  xcel",.         
-00004a70: 2020 2020 2020 2020 2020 2071 7376 5f73             qsv_s
-00004a80: 7072 6561 6473 6865 6574 2e6e 616d 652c  preadsheet.name,
-00004a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004aa0: 2020 2020 2022 2d2d 7368 6565 7422 2c0a       "--sheet",.
-00004ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ac0: 2020 2020 7374 7228 6465 6661 756c 745f      str(default_
-00004ad0: 6578 6365 6c5f 7368 6565 7429 2c0a 2020  excel_sheet),.  
-00004ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004af0: 2020 222d 2d74 7269 6d22 2c0a 2020 2020    "--trim",.    
-00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b10: 222d 2d6f 7574 7075 7422 2c0a 2020 2020  "--output",.    
-00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b30: 7173 765f 6578 6365 6c5f 6373 762e 6e61  qsv_excel_csv.na
-00004b40: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00004b50: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00004b60: 2020 2020 2020 2063 6865 636b 3d54 7275         check=Tru
-00004b70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00004b80: 2020 2063 6170 7475 7265 5f6f 7574 7075     capture_outpu
-00004b90: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
-00004ba0: 2020 2020 2020 2020 7465 7874 3d54 7275          text=Tru
-00004bb0: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
-00004bc0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00004bd0: 7375 6270 726f 6365 7373 2e43 616c 6c65  subprocess.Calle
-00004be0: 6450 726f 6365 7373 4572 726f 7220 6173  dProcessError as
-00004bf0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-00004c00: 6c6f 6767 6572 2e65 7272 6f72 280a 2020  logger.error(.  
-00004c10: 2020 2020 2020 2020 2020 2020 2020 2255                "U
-00004c20: 706c 6f61 6420 6162 6f72 7465 642e 2043  pload aborted. C
-00004c30: 616e 6e6f 7420 6578 706f 7274 2073 7072  annot export spr
-00004c40: 6561 6473 6865 6574 283f 2920 746f 2043  eadsheet(?) to C
-00004c50: 5356 3a20 7b7d 222e 666f 726d 6174 2865  SV: {}".format(e
-00004c60: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
-00004c70: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00004c80: 655f 6269 6e20 3d20 636f 6e66 6967 2e67  e_bin = config.g
-00004c90: 6574 2822 4649 4c45 5f42 494e 2229 0a20  et("FILE_BIN"). 
-00004ca0: 2020 2020 2020 2020 2020 2023 2067 6574             # get
-00004cb0: 2073 6f6d 6520 6669 6c65 2069 6e66 6f20   some file info 
-00004cc0: 616e 6420 6c6f 6720 6974 2062 7920 7275  and log it by ru
-00004cd0: 6e6e 696e 6720 6066 696c 6560 0a20 2020  nning `file`.   
-00004ce0: 2020 2020 2020 2020 2023 206a 7573 7420           # just 
-00004cf0: 696e 2063 6173 6520 7468 6520 6669 6c65  in case the file
-00004d00: 2069 7320 6e6f 7420 6163 7475 616c 6c79   is not actually
-00004d10: 2061 2073 7072 6561 6473 6865 6574 206f   a spreadsheet o
-00004d20: 7220 6973 2065 6e63 7279 7074 6564 0a20  r is encrypted. 
-00004d30: 2020 2020 2020 2020 2020 2066 696c 655f             file_
-00004d40: 666f 726d 6174 203d 2073 7562 7072 6f63  format = subproc
-00004d50: 6573 732e 7275 6e28 0a20 2020 2020 2020  ess.run(.       
-00004d60: 2020 2020 2020 2020 205b 6669 6c65 5f62           [file_b
-00004d70: 696e 2c20 7173 765f 7370 7265 6164 7368  in, qsv_spreadsh
-00004d80: 6565 742e 6e61 6d65 5d2c 0a20 2020 2020  eet.name],.     
-00004d90: 2020 2020 2020 2020 2020 2063 6865 636b             check
-00004da0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-00004db0: 2020 2020 2020 2063 6170 7475 7265 5f6f         capture_o
-00004dc0: 7574 7075 743d 5472 7565 2c0a 2020 2020  utput=True,.    
-00004dd0: 2020 2020 2020 2020 2020 2020 7465 7874              text
-00004de0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-00004df0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00004e00: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
-00004e10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00004e20: 2020 2249 7320 7468 6520 6669 6c65 2065    "Is the file e
-00004e30: 6e63 7279 7074 6564 206f 7220 6973 206e  ncrypted or is n
-00004e40: 6f74 2061 2073 7072 6561 6473 6865 6574  ot a spreadsheet
-00004e50: 3f5c 6e46 494c 4520 4154 5452 4942 5554  ?\nFILE ATTRIBUT
-00004e60: 4553 3a20 7b7d 222e 666f 726d 6174 280a  ES: {}".format(.
-00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e80: 2020 2020 6669 6c65 5f66 6f72 6d61 742e      file_format.
-00004e90: 7374 646f 7574 0a20 2020 2020 2020 2020  stdout.         
-00004ea0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004eb0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00004ec0: 2020 2020 636c 6561 6e75 705f 7465 6d70      cleanup_temp
-00004ed0: 6669 6c65 7328 290a 2020 2020 2020 2020  files().        
-00004ee0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00004ef0: 2020 2071 7376 5f73 7072 6561 6473 6865     qsv_spreadshe
-00004f00: 6574 2e63 6c6f 7365 2829 0a20 2020 2020  et.close().     
-00004f10: 2020 2065 7863 656c 5f65 7870 6f72 745f     excel_export_
-00004f20: 6d73 6720 3d20 7173 765f 6578 6365 6c2e  msg = qsv_excel.
-00004f30: 7374 6465 7272 0a20 2020 2020 2020 206c  stderr.        l
-00004f40: 6f67 6765 722e 696e 666f 2822 7b7d 2e2e  ogger.info("{}..
-00004f50: 2e22 2e66 6f72 6d61 7428 6578 6365 6c5f  .".format(excel_
-00004f60: 6578 706f 7274 5f6d 7367 2929 0a20 2020  export_msg)).   
-00004f70: 2020 2020 2074 6d70 203d 2071 7376 5f65       tmp = qsv_e
-00004f80: 7863 656c 5f63 7376 0a20 2020 2065 6c73  xcel_csv.    els
-00004f90: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
-00004fa0: 2020 2020 2020 2069 7473 2061 2043 5356         its a CSV
-00004fb0: 2f54 5356 2f54 4142 2066 696c 652c 206e  /TSV/TAB file, n
-00004fc0: 6f74 2061 2073 7072 6561 6473 6865 6574  ot a spreadsheet
-00004fd0: 2e0a 2020 2020 2020 2020 4e6f 726d 616c  ..        Normal
-00004fe0: 697a 6520 2620 7472 616e 7363 6f64 6520  ize & transcode 
-00004ff0: 746f 2055 5446 2d38 2075 7369 6e67 2060  to UTF-8 using `
-00005000: 7173 7620 696e 7075 7460 2e20 5765 206e  qsv input`. We n
-00005010: 6565 6420 746f 206e 6f72 6d61 6c69 7a65  eed to normalize
-00005020: 2061 7320 6974 2063 6f75 6c64 2062 650a   as it could be.
-00005030: 2020 2020 2020 2020 6120 4353 562f 5453          a CSV/TS
-00005040: 562f 5441 4220 6469 616c 6563 7420 7769  V/TAB dialect wi
-00005050: 7468 2064 6966 6665 7269 6e67 2064 656c  th differing del
-00005060: 696d 6974 6572 732c 2071 756f 7469 6e67  imiters, quoting
-00005070: 2c20 6574 632e 0a20 2020 2020 2020 2055  , etc..        U
-00005080: 7369 6e67 2071 7376 2069 6e70 7574 2773  sing qsv input's
-00005090: 202d 2d6f 7574 7075 7420 6f70 7469 6f6e   --output option
-000050a0: 2061 6c73 6f20 6175 746f 2d74 7261 6e73   also auto-trans
-000050b0: 636f 6465 7320 746f 2055 5446 2d38 2e0a  codes to UTF-8..
-000050c0: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
-000050d0: 6174 2077 6520 6f6e 6c79 2063 6861 6e67  at we only chang
-000050e0: 6520 7468 6520 776f 726b 6669 6c65 2c20  e the workfile, 
-000050f0: 7468 6520 7265 736f 7572 6365 2066 696c  the resource fil
-00005100: 6520 6974 7365 6c66 2069 7320 756e 6368  e itself is unch
-00005110: 616e 6765 642e 0a20 2020 2020 2020 2022  anged..        "
-00005120: 2222 0a0a 2020 2020 2020 2020 2320 6e6f  ""..        # no
-00005130: 726d 616c 697a 6520 746f 2043 5356 2c20  rmalize to CSV, 
-00005140: 616e 6420 7472 616e 7363 6f64 6520 746f  and transcode to
-00005150: 2055 5446 2d38 2069 6620 7265 7175 6972   UTF-8 if requir
-00005160: 6564 0a20 2020 2020 2020 2071 7376 5f69  ed.        qsv_i
-00005170: 6e70 7574 5f63 7376 203d 2074 656d 7066  nput_csv = tempf
-00005180: 696c 652e 4e61 6d65 6454 656d 706f 7261  ile.NamedTempora
-00005190: 7279 4669 6c65 2873 7566 6669 783d 222e  ryFile(suffix=".
-000051a0: 6373 7622 290a 2020 2020 2020 2020 6966  csv").        if
-000051b0: 2066 6f72 6d61 742e 7570 7065 7228 2920   format.upper() 
-000051c0: 3d3d 2022 4353 5622 3a0a 2020 2020 2020  == "CSV":.      
-000051d0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-000051e0: 6f28 224e 6f72 6d61 6c69 7a69 6e67 2f55  o("Normalizing/U
-000051f0: 5446 2d38 2074 7261 6e73 636f 6469 6e67  TF-8 transcoding
-00005200: 207b 7d2e 2e2e 222e 666f 726d 6174 2866   {}...".format(f
-00005210: 6f72 6d61 7429 290a 2020 2020 2020 2020  ormat)).        
-00005220: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00005230: 2020 6c6f 6767 6572 2e69 6e66 6f28 224e    logger.info("N
-00005240: 6f72 6d61 6c69 7a69 6e67 2f55 5446 2d38  ormalizing/UTF-8
-00005250: 2074 7261 6e73 636f 6469 6e67 207b 7d20   transcoding {} 
-00005260: 746f 2043 5356 2e2e 2e22 2e66 6f72 6d61  to CSV...".forma
-00005270: 7428 666f 726d 6174 2929 0a20 2020 2020  t(format)).     
-00005280: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00005290: 2020 2020 7173 765f 696e 7075 7420 3d20      qsv_input = 
-000052a0: 7375 6270 726f 6365 7373 2e72 756e 280a  subprocess.run(.
-000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052c0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-000052d0: 2020 2020 2020 7173 765f 6269 6e2c 0a20        qsv_bin,. 
-000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052f0: 2020 2022 696e 7075 7422 2c0a 2020 2020     "input",.    
-00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005310: 746d 702e 6e61 6d65 2c0a 2020 2020 2020  tmp.name,.      
-00005320: 2020 2020 2020 2020 2020 2020 2020 222d                "-
-00005330: 2d74 7269 6d2d 6865 6164 6572 7322 2c0a  -trim-headers",.
-00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005350: 2020 2020 222d 2d6f 7574 7075 7422 2c0a      "--output",.
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005370: 2020 2020 7173 765f 696e 7075 745f 6373      qsv_input_cs
-00005380: 762e 6e61 6d65 2c0a 2020 2020 2020 2020  v.name,.        
-00005390: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
-000053a0: 2020 2020 2020 2020 2020 2063 6865 636b             check
-000053b0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-000053c0: 2020 2029 0a20 2020 2020 2020 2065 7863     ).        exc
-000053d0: 6570 7420 7375 6270 726f 6365 7373 2e43  ept subprocess.C
-000053e0: 616c 6c65 6450 726f 6365 7373 4572 726f  alledProcessErro
-000053f0: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
-00005400: 2020 2020 2320 7265 7475 726e 2061 7320      # return as 
-00005410: 7765 2063 616e 2774 2070 7573 6820 616e  we can't push an
-00005420: 2069 6e76 616c 6964 2043 5356 2066 696c   invalid CSV fil
-00005430: 650a 2020 2020 2020 2020 2020 2020 636c  e.            cl
-00005440: 6561 6e75 705f 7465 6d70 6669 6c65 7328  eanup_tempfiles(
-00005450: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
-00005460: 6767 6572 2e65 7272 6f72 280a 2020 2020  gger.error(.    
-00005470: 2020 2020 2020 2020 2020 2020 224a 6f62              "Job
-00005480: 2061 626f 7274 6564 2061 7320 7468 6520   aborted as the 
-00005490: 6669 6c65 2063 616e 6e6f 7420 6265 206e  file cannot be n
-000054a0: 6f72 6d61 6c69 7a65 642f 7472 616e 7363  ormalized/transc
-000054b0: 6f64 6564 3a20 7b7d 2e22 2e66 6f72 6d61  oded: {}.".forma
-000054c0: 7428 6529 0a20 2020 2020 2020 2020 2020  t(e).           
-000054d0: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-000054e0: 6574 7572 6e0a 2020 2020 2020 2020 746d  eturn.        tm
-000054f0: 7020 3d20 7173 765f 696e 7075 745f 6373  p = qsv_input_cs
-00005500: 760a 2020 2020 2020 2020 6c6f 6767 6572  v.        logger
-00005510: 2e69 6e66 6f28 224e 6f72 6d61 6c69 7a65  .info("Normalize
-00005520: 6420 2620 7472 616e 7363 6f64 6564 2e2e  d & transcoded..
-00005530: 2e22 290a 0a20 2020 2023 2076 616c 6964  .")..    # valid
-00005540: 6174 696f 6e20 7068 6173 650a 2020 2020  ation phase.    
-00005550: 2320 5275 6e20 616e 2052 4643 3431 3830  # Run an RFC4180
-00005560: 2063 6865 636b 2077 6974 6820 6071 7376   check with `qsv
-00005570: 2076 616c 6964 6174 6560 2061 6761 696e   validate` again
-00005580: 7374 2074 6865 206e 6f72 6d61 6c69 7a65  st the normalize
-00005590: 642c 2055 5446 2d38 2065 6e63 6f64 6564  d, UTF-8 encoded
-000055a0: 2043 5356 2066 696c 652e 0a20 2020 2023   CSV file..    #
-000055b0: 2045 7665 6e20 6578 6365 6c20 6578 706f   Even excel expo
-000055c0: 7274 6564 2043 5356 7320 6361 6e20 6265  rted CSVs can be
-000055d0: 2070 6f74 656e 7469 616c 6c79 2069 6e76   potentially inv
-000055e0: 616c 6964 2c20 6173 2069 7420 616c 6c6f  alid, as it allo
-000055f0: 7773 2074 6865 2065 7870 6f72 7420 6f66  ws the export of
-00005600: 2022 666c 6578 6962 6c65 220a 2020 2020   "flexible".    
-00005610: 2320 4353 5673 202d 2069 2e65 2e20 726f  # CSVs - i.e. ro
-00005620: 7773 206d 6179 2068 6176 6520 6469 6666  ws may have diff
-00005630: 6572 656e 7420 636f 6c75 6d6e 2063 6f75  erent column cou
-00005640: 6e74 732e 0a20 2020 2023 2049 6620 6974  nts..    # If it
-00005650: 2070 6173 7365 7320 7661 6c69 6461 7469   passes validati
-00005660: 6f6e 2c20 7765 2063 616e 206e 6f77 2068  on, we can now h
-00005670: 616e 646c 6520 6974 2077 6974 6820 636f  andle it with co
-00005680: 6e66 6964 656e 6365 2064 6f77 6e73 7472  nfidence downstr
-00005690: 6561 6d20 6173 2061 2022 6e6f 726d 616c  eam as a "normal
-000056a0: 2220 4353 562e 0a20 2020 206c 6f67 6765  " CSV..    logge
-000056b0: 722e 696e 666f 2822 5661 6c69 6461 7469  r.info("Validati
-000056c0: 6e67 2043 5356 2e2e 2e22 290a 2020 2020  ng CSV...").    
-000056d0: 7472 793a 0a20 2020 2020 2020 2071 7376  try:.        qsv
-000056e0: 5f76 616c 6964 6174 6520 3d20 7375 6270  _validate = subp
-000056f0: 726f 6365 7373 2e72 756e 280a 2020 2020  rocess.run(.    
-00005700: 2020 2020 2020 2020 5b71 7376 5f62 696e          [qsv_bin
-00005710: 2c20 2276 616c 6964 6174 6522 2c20 746d  , "validate", tm
-00005720: 702e 6e61 6d65 5d2c 2063 6865 636b 3d54  p.name], check=T
-00005730: 7275 652c 2063 6170 7475 7265 5f6f 7574  rue, capture_out
-00005740: 7075 743d 5472 7565 2c20 7465 7874 3d54  put=True, text=T
-00005750: 7275 650a 2020 2020 2020 2020 290a 2020  rue.        ).  
-00005760: 2020 6578 6365 7074 2073 7562 7072 6f63    except subproc
-00005770: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
-00005780: 7345 7272 6f72 2061 7320 653a 0a20 2020  sError as e:.   
-00005790: 2020 2020 2023 2072 6574 7572 6e20 6173       # return as
-000057a0: 2077 6520 6361 6e27 7420 7075 7368 2061   we can't push a
-000057b0: 6e20 696e 7661 6c69 6420 4353 5620 6669  n invalid CSV fi
-000057c0: 6c65 0a20 2020 2020 2020 2063 6c65 616e  le.        clean
-000057d0: 7570 5f74 656d 7066 696c 6573 2829 0a20  up_tempfiles(). 
-000057e0: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
-000057f0: 6572 726f 725f 6d73 6720 3d20 7173 765f  error_msg = qsv_
-00005800: 7661 6c69 6461 7465 2e73 7464 6572 720a  validate.stderr.
-00005810: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-00005820: 7272 6f72 2822 496e 7661 6c69 6420 6669  rror("Invalid fi
-00005830: 6c65 2120 4a6f 6220 6162 6f72 7465 643a  le! Job aborted:
-00005840: 207b 7d2e 222e 666f 726d 6174 2876 616c   {}.".format(val
-00005850: 6964 6174 655f 6572 726f 725f 6d73 6729  idate_error_msg)
-00005860: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00005870: 0a20 2020 206c 6f67 6765 722e 696e 666f  .    logger.info
-00005880: 2822 5765 6c6c 2d66 6f72 6d65 642c 2076  ("Well-formed, v
-00005890: 616c 6964 2043 5356 2066 696c 6520 636f  alid CSV file co
-000058a0: 6e66 6972 6d65 642e 2e2e 2229 0a0a 2020  nfirmed...")..  
-000058b0: 2020 2320 646f 2077 6520 6e65 6564 2074    # do we need t
-000058c0: 6f20 6465 6475 703f 0a20 2020 2023 206e  o dedup?.    # n
-000058d0: 6f74 6520 7468 6174 2064 6564 7570 696e  ote that dedupin
-000058e0: 6720 616c 736f 2065 6e64 7320 7570 2063  g also ends up c
-000058f0: 7265 6174 696e 6720 6120 736f 7274 6564  reating a sorted
-00005900: 2043 5356 0a20 2020 2064 6564 7570 203d   CSV.    dedup =
-00005910: 2063 6f6e 6669 672e 6765 7428 2244 4544   config.get("DED
-00005920: 5550 2229 0a20 2020 2069 6620 6465 6475  UP").    if dedu
-00005930: 703a 0a20 2020 2020 2020 2071 7376 5f64  p:.        qsv_d
-00005940: 6564 7570 5f63 7376 203d 2074 656d 7066  edup_csv = tempf
-00005950: 696c 652e 4e61 6d65 6454 656d 706f 7261  ile.NamedTempora
-00005960: 7279 4669 6c65 2873 7566 6669 783d 222e  ryFile(suffix=".
-00005970: 6373 7622 290a 2020 2020 2020 2020 6c6f  csv").        lo
-00005980: 6767 6572 2e69 6e66 6f28 2243 6865 636b  gger.info("Check
-00005990: 696e 6720 666f 7220 6475 706c 6963 6174  ing for duplicat
-000059a0: 6520 726f 7773 2e2e 2e22 290a 2020 2020  e rows...").    
-000059b0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000059c0: 2020 2020 2071 7376 5f64 6564 7570 203d       qsv_dedup =
-000059d0: 2073 7562 7072 6f63 6573 732e 7275 6e28   subprocess.run(
-000059e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059f0: 205b 7173 765f 6269 6e2c 2022 6465 6475   [qsv_bin, "dedu
-00005a00: 7022 2c20 746d 702e 6e61 6d65 2c20 222d  p", tmp.name, "-
-00005a10: 2d6f 7574 7075 7422 2c20 7173 765f 6465  -output", qsv_de
-00005a20: 6475 705f 6373 762e 6e61 6d65 5d2c 0a20  dup_csv.name],. 
-00005a30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00005a40: 6170 7475 7265 5f6f 7574 7075 743d 5472  apture_output=Tr
-00005a50: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00005a60: 2020 2020 7465 7874 3d54 7275 652c 0a20      text=True,. 
-00005a70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00005a80: 2020 2020 2065 7863 6570 7420 7375 6270       except subp
-00005a90: 726f 6365 7373 2e43 616c 6c65 6450 726f  rocess.CalledPro
-00005aa0: 6365 7373 4572 726f 7220 6173 2065 3a0a  cessError as e:.
-00005ab0: 2020 2020 2020 2020 2020 2020 636c 6561              clea
-00005ac0: 6e75 705f 7465 6d70 6669 6c65 7328 290a  nup_tempfiles().
-00005ad0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00005ae0: 6520 7574 696c 2e4a 6f62 4572 726f 7228  e util.JobError(
-00005af0: 2243 6865 636b 2066 6f72 2064 7570 6c69  "Check for dupli
-00005b00: 6361 7465 7320 6572 726f 723a 207b 7d22  cates error: {}"
-00005b10: 2e66 6f72 6d61 7428 6529 290a 2020 2020  .format(e)).    
-00005b20: 2020 2020 6475 7065 5f63 6f75 6e74 203d      dupe_count =
-00005b30: 2069 6e74 2873 7472 2871 7376 5f64 6564   int(str(qsv_ded
-00005b40: 7570 2e73 7464 6572 7229 2e73 7472 6970  up.stderr).strip
-00005b50: 2829 290a 2020 2020 2020 2020 6966 2064  ()).        if d
-00005b60: 7570 655f 636f 756e 7420 3e20 303a 0a20  upe_count > 0:. 
-00005b70: 2020 2020 2020 2020 2020 2074 6d70 203d             tmp =
-00005b80: 2071 7376 5f64 6564 7570 5f63 7376 0a20   qsv_dedup_csv. 
-00005b90: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00005ba0: 722e 7761 726e 696e 6728 227b 3a2c 7d20  r.warning("{:,} 
-00005bb0: 6475 706c 6963 6174 6573 2066 6f75 6e64  duplicates found
-00005bc0: 2061 6e64 2072 656d 6f76 6564 2e2e 2e22   and removed..."
-00005bd0: 2e66 6f72 6d61 7428 6475 7065 5f63 6f75  .format(dupe_cou
-00005be0: 6e74 2929 0a20 2020 2020 2020 2065 6c73  nt)).        els
-00005bf0: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
-00005c00: 6f67 6765 722e 696e 666f 2822 4e6f 2064  ogger.info("No d
-00005c10: 7570 6c69 6361 7465 7320 666f 756e 642e  uplicates found.
-00005c20: 2e2e 2229 0a0a 2020 2020 2320 6765 7420  ..")..    # get 
-00005c30: 6578 6973 7469 6e67 2068 6561 6465 7220  existing header 
-00005c40: 6e61 6d65 732c 2073 6f20 7765 2063 616e  names, so we can
-00005c50: 2075 7365 2074 6865 6d20 666f 7220 6461   use them for da
-00005c60: 7461 2064 6963 7469 6f6e 6172 7920 6c61  ta dictionary la
-00005c70: 6265 6c73 0a20 2020 2023 2073 686f 756c  bels.    # shoul
-00005c80: 6420 7765 206e 6565 6420 746f 2063 6861  d we need to cha
-00005c90: 6e67 6520 7468 6520 636f 6c75 6d6e 206e  nge the column n
-00005ca0: 616d 6520 746f 206d 616b 6520 6974 2022  ame to make it "
-00005cb0: 6462 2d73 6166 6522 0a20 2020 2074 7279  db-safe".    try
-00005cc0: 3a0a 2020 2020 2020 2020 7173 765f 6865  :.        qsv_he
-00005cd0: 6164 6572 7320 3d20 7375 6270 726f 6365  aders = subproce
-00005ce0: 7373 2e72 756e 280a 2020 2020 2020 2020  ss.run(.        
-00005cf0: 2020 2020 5b71 7376 5f62 696e 2c20 2268      [qsv_bin, "h
-00005d00: 6561 6465 7273 222c 2022 2d2d 6a75 7374  eaders", "--just
-00005d10: 2d6e 616d 6573 222c 2074 6d70 2e6e 616d  -names", tmp.nam
-00005d20: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
-00005d30: 6361 7074 7572 655f 6f75 7470 7574 3d54  capture_output=T
-00005d40: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00005d50: 2063 6865 636b 3d54 7275 652c 0a20 2020   check=True,.   
-00005d60: 2020 2020 2020 2020 2074 6578 743d 5472           text=Tr
-00005d70: 7565 2c0a 2020 2020 2020 2020 290a 2020  ue,.        ).  
-00005d80: 2020 6578 6365 7074 2073 7562 7072 6f63    except subproc
-00005d90: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
-00005da0: 7345 7272 6f72 2061 7320 653a 0a20 2020  sError as e:.   
-00005db0: 2020 2020 2063 6c65 616e 7570 5f74 656d       cleanup_tem
-00005dc0: 7066 696c 6573 2829 0a20 2020 2020 2020  pfiles().       
-00005dd0: 2072 6169 7365 2075 7469 6c2e 4a6f 6245   raise util.JobE
-00005de0: 7272 6f72 2822 4361 6e6e 6f74 2073 6361  rror("Cannot sca
-00005df0: 6e20 4353 5620 6865 6164 6572 733a 207b  n CSV headers: {
-00005e00: 7d22 2e66 6f72 6d61 7428 6529 290a 2020  }".format(e)).  
-00005e10: 2020 6f72 6967 696e 616c 5f68 6561 6465    original_heade
-00005e20: 7273 203d 2073 7472 2871 7376 5f68 6561  rs = str(qsv_hea
-00005e30: 6465 7273 2e73 7464 6f75 7429 2e73 7472  ders.stdout).str
-00005e40: 6970 2829 0a20 2020 206f 7269 6769 6e61  ip().    origina
-00005e50: 6c5f 6865 6164 6572 5f64 6963 7420 3d20  l_header_dict = 
-00005e60: 7b0a 2020 2020 2020 2020 6964 783a 2065  {.        idx: e
-00005e70: 6c65 2066 6f72 2069 6478 2c20 656c 6520  le for idx, ele 
-00005e80: 696e 2065 6e75 6d65 7261 7465 286f 7269  in enumerate(ori
-00005e90: 6769 6e61 6c5f 6865 6164 6572 732e 7370  ginal_headers.sp
-00005ea0: 6c69 746c 696e 6573 2829 290a 2020 2020  litlines()).    
-00005eb0: 7d0a 0a20 2020 2023 206e 6f77 2c20 656e  }..    # now, en
-00005ec0: 7375 7265 206f 7572 2063 6f6c 756d 6e2f  sure our column/
-00005ed0: 6865 6164 6572 206e 616d 6573 2069 6465  header names ide
-00005ee0: 6e74 6966 6965 7273 2061 7265 2022 7361  ntifiers are "sa
-00005ef0: 6665 206e 616d 6573 220a 2020 2020 2320  fe names".    # 
-00005f00: 692e 652e 2076 616c 6964 2070 6f73 7467  i.e. valid postg
-00005f10: 7265 7320 6964 656e 7469 6669 6572 730a  res identifiers.
-00005f20: 2020 2020 7173 765f 7361 6665 6e61 6d65      qsv_safename
-00005f30: 735f 6373 7620 3d20 7465 6d70 6669 6c65  s_csv = tempfile
-00005f40: 2e4e 616d 6564 5465 6d70 6f72 6172 7946  .NamedTemporaryF
-00005f50: 696c 6528 7375 6666 6978 3d22 2e63 7376  ile(suffix=".csv
-00005f60: 2229 0a20 2020 206c 6f67 6765 722e 696e  ").    logger.in
-00005f70: 666f 2827 4368 6563 6b69 6e67 2066 6f72  fo('Checking for
-00005f80: 2022 6461 7461 6261 7365 2d73 6166 6522   "database-safe"
-00005f90: 2068 6561 6465 7220 6e61 6d65 732e 2e2e   header names...
-00005fa0: 2729 0a20 2020 2074 7279 3a0a 2020 2020  ').    try:.    
-00005fb0: 2020 2020 7173 765f 7361 6665 6e61 6d65      qsv_safename
-00005fc0: 7320 3d20 7375 6270 726f 6365 7373 2e72  s = subprocess.r
-00005fd0: 756e 280a 2020 2020 2020 2020 2020 2020  un(.            
-00005fe0: 5b71 7376 5f62 696e 2c20 2273 6166 656e  [qsv_bin, "safen
-00005ff0: 616d 6573 222c 2074 6d70 2e6e 616d 652c  ames", tmp.name,
-00006000: 2022 2d2d 6d6f 6465 222c 2022 6a73 6f6e   "--mode", "json
-00006010: 222c 5d2c 0a20 2020 2020 2020 2020 2020  ",],.           
-00006020: 2063 6170 7475 7265 5f6f 7574 7075 743d   capture_output=
-00006030: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00006040: 2020 7465 7874 3d54 7275 652c 0a20 2020    text=True,.   
-00006050: 2020 2020 2029 0a20 2020 2065 7863 6570       ).    excep
-00006060: 7420 7375 6270 726f 6365 7373 2e43 616c  t subprocess.Cal
-00006070: 6c65 6450 726f 6365 7373 4572 726f 7220  ledProcessError 
-00006080: 6173 2065 3a0a 2020 2020 2020 2020 636c  as e:.        cl
-00006090: 6561 6e75 705f 7465 6d70 6669 6c65 7328  eanup_tempfiles(
-000060a0: 290a 2020 2020 2020 2020 7261 6973 6520  ).        raise 
-000060b0: 7574 696c 2e4a 6f62 4572 726f 7228 2253  util.JobError("S
-000060c0: 6166 656e 616d 6573 2065 7272 6f72 3a20  afenames error: 
-000060d0: 7b7d 222e 666f 726d 6174 2865 2929 0a0a  {}".format(e))..
-000060e0: 2020 2020 756e 7361 6665 5f6a 736f 6e20      unsafe_json 
-000060f0: 3d20 6a73 6f6e 2e6c 6f61 6473 2873 7472  = json.loads(str
-00006100: 2871 7376 5f73 6166 656e 616d 6573 2e73  (qsv_safenames.s
-00006110: 7464 6f75 7429 290a 2020 2020 756e 7361  tdout)).    unsa
-00006120: 6665 5f68 6561 6465 7273 203d 2075 6e73  fe_headers = uns
-00006130: 6166 655f 6a73 6f6e 5b22 756e 7361 6665  afe_json["unsafe
-00006140: 5f68 6561 6465 7273 225d 0a0a 2020 2020  _headers"]..    
-00006150: 6966 2075 6e73 6166 655f 6865 6164 6572  if unsafe_header
-00006160: 733a 0a20 2020 2020 2020 206c 6f67 6765  s:.        logge
-00006170: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
-00006180: 2020 2020 2722 7b7d 2075 6e73 6166 6522      '"{} unsafe"
-00006190: 2068 6561 6465 7220 6e61 6d65 7320 666f   header names fo
-000061a0: 756e 6420 287b 7d29 2e20 5361 6e69 7469  und ({}). Saniti
-000061b0: 7a69 6e67 2e2e 2e22 272e 666f 726d 6174  zing..."'.format
-000061c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000061d0: 2020 6c65 6e28 756e 7361 6665 5f68 6561    len(unsafe_hea
-000061e0: 6465 7273 292c 2075 6e73 6166 655f 6865  ders), unsafe_he
-000061f0: 6164 6572 730a 2020 2020 2020 2020 2020  aders.          
-00006200: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
-00006210: 2020 2020 2020 7173 765f 7361 6665 6e61        qsv_safena
-00006220: 6d65 7320 3d20 7375 6270 726f 6365 7373  mes = subprocess
-00006230: 2e72 756e 280a 2020 2020 2020 2020 2020  .run(.          
-00006240: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-00006250: 2020 2020 7173 765f 6269 6e2c 0a20 2020      qsv_bin,.   
-00006260: 2020 2020 2020 2020 2020 2020 2022 7361               "sa
-00006270: 6665 6e61 6d65 7322 2c0a 2020 2020 2020  fenames",.      
-00006280: 2020 2020 2020 2020 2020 746d 702e 6e61            tmp.na
-00006290: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-000062a0: 2020 2020 222d 2d6d 6f64 6522 2c0a 2020      "--mode",.  
-000062b0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-000062c0: 6f6e 6469 7469 6f6e 616c 222c 0a20 2020  onditional",.   
-000062d0: 2020 2020 2020 2020 2020 2020 2022 2d2d               "--
-000062e0: 6f75 7470 7574 222c 0a20 2020 2020 2020  output",.       
-000062f0: 2020 2020 2020 2020 2071 7376 5f73 6166           qsv_saf
-00006300: 656e 616d 6573 5f63 7376 2e6e 616d 652c  enames_csv.name,
-00006310: 0a20 2020 2020 2020 2020 2020 205d 2c0a  .            ],.
-00006320: 2020 2020 2020 2020 2020 2020 6361 7074              capt
-00006330: 7572 655f 6f75 7470 7574 3d54 7275 652c  ure_output=True,
-00006340: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
-00006350: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
-00006360: 290a 2020 2020 2020 2020 746d 7020 3d20  ).        tmp = 
-00006370: 7173 765f 7361 6665 6e61 6d65 735f 6373  qsv_safenames_cs
-00006380: 760a 2020 2020 656c 7365 3a0a 2020 2020  v.    else:.    
-00006390: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-000063a0: 224e 6f20 756e 7361 6665 2068 6561 6465  "No unsafe heade
-000063b0: 7220 6e61 6d65 7320 666f 756e 642e 2e2e  r names found...
-000063c0: 2229 0a0a 2020 2020 2320 6174 2074 6869  ")..    # at thi
-000063d0: 7320 7374 6167 652c 2077 6520 6861 7665  s stage, we have
-000063e0: 2061 2022 636c 6561 6e22 2043 5356 2072   a "clean" CSV r
-000063f0: 6561 6479 2066 6f72 2074 7970 6520 696e  eady for type in
-00006400: 6665 7265 6e63 696e 670a 0a20 2020 2023  ferencing..    #
-00006410: 2066 6972 7374 2c20 696e 6465 7820 6373   first, index cs
-00006420: 7620 666f 7220 7370 6565 6420 2d20 636f  v for speed - co
-00006430: 756e 742c 2073 7461 7473 2061 6e64 2073  unt, stats and s
-00006440: 6c69 6365 0a20 2020 2023 2061 7265 2061  lice.    # are a
-00006450: 6c6c 2061 6363 656c 6572 6174 6564 2f6d  ll accelerated/m
-00006460: 756c 7469 7468 7265 6164 6564 2077 6865  ultithreaded whe
-00006470: 6e20 616e 2069 6e64 6578 2069 7320 7072  n an index is pr
-00006480: 6573 656e 740a 2020 2020 7472 793a 0a20  esent.    try:. 
-00006490: 2020 2020 2020 2071 7376 5f69 6e64 6578         qsv_index
-000064a0: 5f66 696c 6520 3d20 746d 702e 6e61 6d65  _file = tmp.name
-000064b0: 202b 2022 2e69 6478 220a 2020 2020 2020   + ".idx".      
-000064c0: 2020 7375 6270 726f 6365 7373 2e72 756e    subprocess.run
-000064d0: 285b 7173 765f 6269 6e2c 2022 696e 6465  ([qsv_bin, "inde
-000064e0: 7822 2c20 746d 702e 6e61 6d65 5d2c 2063  x", tmp.name], c
-000064f0: 6865 636b 3d54 7275 6529 0a20 2020 2065  heck=True).    e
-00006500: 7863 6570 7420 7375 6270 726f 6365 7373  xcept subprocess
-00006510: 2e43 616c 6c65 6450 726f 6365 7373 4572  .CalledProcessEr
-00006520: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
-00006530: 2020 636c 6561 6e75 705f 7465 6d70 6669    cleanup_tempfi
-00006540: 6c65 730a 2020 2020 2020 2020 7261 6973  les.        rais
-00006550: 6520 7574 696c 2e4a 6f62 4572 726f 7228  e util.JobError(
-00006560: 2243 616e 6e6f 7420 696e 6465 7820 4353  "Cannot index CS
-00006570: 563a 207b 7d22 2e66 6f72 6d61 7428 6529  V: {}".format(e)
-00006580: 290a 0a20 2020 2023 2067 6574 2072 6563  )..    # get rec
-00006590: 6f72 6420 636f 756e 742c 2074 6869 7320  ord count, this 
-000065a0: 6973 2069 6e73 7461 6e74 616e 656f 7573  is instantaneous
-000065b0: 2077 6974 6820 616e 2069 6e64 6578 0a20   with an index. 
-000065c0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000065d0: 7173 765f 636f 756e 7420 3d20 7375 6270  qsv_count = subp
-000065e0: 726f 6365 7373 2e72 756e 280a 2020 2020  rocess.run(.    
-000065f0: 2020 2020 2020 2020 5b71 7376 5f62 696e          [qsv_bin
-00006600: 2c20 2263 6f75 6e74 222c 2074 6d70 2e6e  , "count", tmp.n
-00006610: 616d 655d 2c20 6361 7074 7572 655f 6f75  ame], capture_ou
-00006620: 7470 7574 3d54 7275 652c 2063 6865 636b  tput=True, check
-00006630: 3d54 7275 652c 2074 6578 743d 5472 7565  =True, text=True
-00006640: 0a20 2020 2020 2020 2029 0a20 2020 2065  .        ).    e
-00006650: 7863 6570 7420 7375 6270 726f 6365 7373  xcept subprocess
-00006660: 2e43 616c 6c65 6450 726f 6365 7373 4572  .CalledProcessEr
-00006670: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
-00006680: 2020 636c 6561 6e75 705f 7465 6d70 6669    cleanup_tempfi
-00006690: 6c65 7328 290a 2020 2020 2020 2020 7261  les().        ra
-000066a0: 6973 6520 7574 696c 2e4a 6f62 4572 726f  ise util.JobErro
-000066b0: 7228 2243 616e 6e6f 7420 636f 756e 7420  r("Cannot count 
-000066c0: 7265 636f 7264 7320 696e 2043 5356 3a20  records in CSV: 
-000066d0: 7b7d 222e 666f 726d 6174 2865 2929 0a20  {}".format(e)). 
-000066e0: 2020 2072 6563 6f72 645f 636f 756e 7420     record_count 
-000066f0: 3d20 696e 7428 7374 7228 7173 765f 636f  = int(str(qsv_co
-00006700: 756e 742e 7374 646f 7574 292e 7374 7269  unt.stdout).stri
-00006710: 7028 2929 0a0a 2020 2020 2320 6974 7320  p())..    # its 
-00006720: 656d 7074 792c 206e 6f74 6869 6e67 2074  empty, nothing t
-00006730: 6f20 646f 0a20 2020 2069 6620 7265 636f  o do.    if reco
-00006740: 7264 5f63 6f75 6e74 203d 3d20 303a 0a20  rd_count == 0:. 
-00006750: 2020 2020 2020 2063 6c65 616e 7570 5f74         cleanup_t
-00006760: 656d 7066 696c 6573 2829 0a20 2020 2020  empfiles().     
-00006770: 2020 206c 6f67 6765 722e 7761 726e 696e     logger.warnin
-00006780: 6728 2255 706c 6f61 6420 736b 6970 7065  g("Upload skippe
-00006790: 6420 6173 2074 6865 7265 2061 7265 207a  d as there are z
-000067a0: 6572 6f20 7265 636f 7264 732e 2229 0a20  ero records."). 
-000067b0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-000067c0: 2020 2023 206c 6f67 2068 6f77 206d 616e     # log how man
-000067d0: 7920 7265 636f 7264 7320 7765 2064 6574  y records we det
-000067e0: 6563 7465 640a 2020 2020 756e 6971 7565  ected.    unique
-000067f0: 5f71 7561 6c69 6669 6572 203d 2022 220a  _qualifier = "".
-00006800: 2020 2020 6966 2064 6564 7570 3a0a 2020      if dedup:.  
-00006810: 2020 2020 2020 756e 6971 7565 5f71 7561        unique_qua
-00006820: 6c69 6669 6572 203d 2022 756e 6971 7565  lifier = "unique
-00006830: 220a 2020 2020 6c6f 6767 6572 2e69 6e66  ".    logger.inf
-00006840: 6f28 227b 3a2c 7d20 7b7d 2072 6563 6f72  o("{:,} {} recor
-00006850: 6473 2064 6574 6563 7465 642e 2e2e 222e  ds detected...".
-00006860: 666f 726d 6174 2872 6563 6f72 645f 636f  format(record_co
-00006870: 756e 742c 2075 6e69 7175 655f 7175 616c  unt, unique_qual
-00006880: 6966 6965 7229 290a 0a20 2020 2023 2072  ifier))..    # r
-00006890: 756e 2071 7376 2073 7461 7473 2074 6f20  un qsv stats to 
-000068a0: 6765 7420 6461 7461 2074 7970 6573 2061  get data types a
-000068b0: 6e64 2073 756d 6d61 7279 2073 7461 7469  nd summary stati
-000068c0: 7374 6963 730a 2020 2020 6c6f 6767 6572  stics.    logger
-000068d0: 2e69 6e66 6f28 2249 6e66 6572 7269 6e67  .info("Inferring
-000068e0: 2064 6174 6120 7479 7065 7320 616e 6420   data types and 
-000068f0: 636f 6d70 696c 696e 6720 7374 6174 6973  compiling statis
-00006900: 7469 6373 2e2e 2e22 290a 2020 2020 6865  tics...").    he
-00006910: 6164 6572 7320 3d20 5b5d 0a20 2020 2074  aders = [].    t
-00006920: 7970 6573 203d 205b 5d0a 2020 2020 6865  ypes = [].    he
-00006930: 6164 6572 735f 6d69 6e20 3d20 5b5d 0a20  aders_min = []. 
-00006940: 2020 2068 6561 6465 7273 5f6d 6178 203d     headers_max =
-00006950: 205b 5d0a 2020 2020 6865 6164 6572 735f   [].    headers_
-00006960: 6361 7264 696e 616c 6974 7920 3d20 5b5d  cardinality = []
-00006970: 0a20 2020 2071 7376 5f73 7461 7473 5f63  .    qsv_stats_c
-00006980: 7376 203d 2074 656d 7066 696c 652e 4e61  sv = tempfile.Na
-00006990: 6d65 6454 656d 706f 7261 7279 4669 6c65  medTemporaryFile
-000069a0: 2873 7566 6669 783d 222e 6373 7622 290a  (suffix=".csv").
-000069b0: 2020 2020 7173 765f 7374 6174 735f 636d      qsv_stats_cm
-000069c0: 6420 3d20 5b0a 2020 2020 2020 2020 7173  d = [.        qs
-000069d0: 765f 6269 6e2c 0a20 2020 2020 2020 2022  v_bin,.        "
-000069e0: 7374 6174 7322 2c0a 2020 2020 2020 2020  stats",.        
-000069f0: 746d 702e 6e61 6d65 2c0a 2020 2020 2020  tmp.name,.      
-00006a00: 2020 222d 2d69 6e66 6572 2d64 6174 6573    "--infer-dates
-00006a10: 222c 0a20 2020 2020 2020 2022 2d2d 6461  ",.        "--da
-00006a20: 7465 732d 7768 6974 656c 6973 7422 2c0a  tes-whitelist",.
-00006a30: 2020 2020 2020 2020 2261 6c6c 222c 0a20          "all",. 
-00006a40: 2020 2020 2020 2022 2d2d 6f75 7470 7574         "--output
-00006a50: 222c 0a20 2020 2020 2020 2071 7376 5f73  ",.        qsv_s
-00006a60: 7461 7473 5f63 7376 2e6e 616d 652c 0a20  tats_csv.name,. 
-00006a70: 2020 205d 0a20 2020 2070 7265 6665 725f     ].    prefer_
-00006a80: 646d 7920 3d20 636f 6e66 6967 2e67 6574  dmy = config.get
-00006a90: 2822 5052 4546 4552 5f44 4d59 2229 0a20  ("PREFER_DMY"). 
-00006aa0: 2020 2069 6620 7072 6566 6572 5f64 6d79     if prefer_dmy
-00006ab0: 3a0a 2020 2020 2020 2020 7173 765f 7374  :.        qsv_st
-00006ac0: 6174 735f 636d 642e 6170 7065 6e64 2822  ats_cmd.append("
-00006ad0: 2d2d 7072 6566 6572 5f64 6d79 2229 0a20  --prefer_dmy"). 
-00006ae0: 2020 2061 7574 6f5f 696e 6465 785f 7468     auto_index_th
-00006af0: 7265 7368 6f6c 6420 3d20 636f 6e66 6967  reshold = config
-00006b00: 2e67 6574 2822 4155 544f 5f49 4e44 4558  .get("AUTO_INDEX
-00006b10: 5f54 4852 4553 484f 4c44 2229 0a20 2020  _THRESHOLD").   
-00006b20: 2069 6620 6175 746f 5f69 6e64 6578 5f74   if auto_index_t
-00006b30: 6872 6573 686f 6c64 3a0a 2020 2020 2020  hreshold:.      
-00006b40: 2020 7173 765f 7374 6174 735f 636d 642e    qsv_stats_cmd.
-00006b50: 6170 7065 6e64 2822 2d2d 6361 7264 696e  append("--cardin
-00006b60: 616c 6974 7922 290a 2020 2020 7375 6d6d  ality").    summ
-00006b70: 6172 795f 7374 6174 735f 6f70 7469 6f6e  ary_stats_option
-00006b80: 7320 3d20 636f 6e66 6967 2e67 6574 2822  s = config.get("
-00006b90: 5355 4d4d 4152 595f 5354 4154 535f 4f50  SUMMARY_STATS_OP
-00006ba0: 5449 4f4e 5322 290a 2020 2020 6966 2073  TIONS").    if s
-00006bb0: 756d 6d61 7279 5f73 7461 7473 5f6f 7074  ummary_stats_opt
-00006bc0: 696f 6e73 3a0a 2020 2020 2020 2020 7173  ions:.        qs
-00006bd0: 765f 7374 6174 735f 636d 642e 6170 7065  v_stats_cmd.appe
-00006be0: 6e64 2873 756d 6d61 7279 5f73 7461 7473  nd(summary_stats
-00006bf0: 5f6f 7074 696f 6e73 290a 0a20 2020 2074  _options)..    t
-00006c00: 7279 3a0a 2020 2020 2020 2020 7173 765f  ry:.        qsv_
-00006c10: 7374 6174 7320 3d20 7375 6270 726f 6365  stats = subproce
-00006c20: 7373 2e72 756e 2871 7376 5f73 7461 7473  ss.run(qsv_stats
-00006c30: 5f63 6d64 2c20 6368 6563 6b3d 5472 7565  _cmd, check=True
-00006c40: 290a 2020 2020 6578 6365 7074 2073 7562  ).    except sub
-00006c50: 7072 6f63 6573 732e 4361 6c6c 6564 5072  process.CalledPr
-00006c60: 6f63 6573 7345 7272 6f72 2061 7320 653a  ocessError as e:
-00006c70: 0a20 2020 2020 2020 2063 6c65 616e 7570  .        cleanup
-00006c80: 5f74 656d 7066 696c 6573 2829 0a20 2020  _tempfiles().   
-00006c90: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
-00006ca0: 4a6f 6245 7272 6f72 280a 2020 2020 2020  JobError(.      
-00006cb0: 2020 2020 2020 2243 616e 6e6f 7420 696e        "Cannot in
-00006cc0: 6665 7220 6461 7461 2074 7970 6573 2061  fer data types a
-00006cd0: 6e64 2063 6f6d 7069 6c65 2073 7461 7469  nd compile stati
-00006ce0: 7374 6963 733a 207b 7d22 2e66 6f72 6d61  stics: {}".forma
-00006cf0: 7428 6529 0a20 2020 2020 2020 2029 0a0a  t(e).        )..
-00006d00: 2020 2020 7769 7468 206f 7065 6e28 7173      with open(qs
-00006d10: 765f 7374 6174 735f 6373 762e 6e61 6d65  v_stats_csv.name
-00006d20: 2c20 6d6f 6465 3d22 7222 2920 6173 2069  , mode="r") as i
-00006d30: 6e70 3a0a 2020 2020 2020 2020 7265 6164  np:.        read
-00006d40: 6572 203d 2063 7376 2e44 6963 7452 6561  er = csv.DictRea
-00006d50: 6465 7228 696e 7029 0a20 2020 2020 2020  der(inp).       
-00006d60: 2066 6f72 2072 6f77 2069 6e20 7265 6164   for row in read
-00006d70: 6572 3a0a 2020 2020 2020 2020 2020 2020  er:.            
-00006d80: 6865 6164 6572 732e 6170 7065 6e64 2872  headers.append(r
-00006d90: 6f77 5b22 6669 656c 6422 5d29 0a20 2020  ow["field"]).   
-00006da0: 2020 2020 2020 2020 2074 7970 6573 2e61           types.a
-00006db0: 7070 656e 6428 726f 775b 2274 7970 6522  ppend(row["type"
-00006dc0: 5d29 0a20 2020 2020 2020 2020 2020 2068  ]).            h
-00006dd0: 6561 6465 7273 5f6d 696e 2e61 7070 656e  eaders_min.appen
-00006de0: 6428 726f 775b 226d 696e 225d 290a 2020  d(row["min"]).  
-00006df0: 2020 2020 2020 2020 2020 6865 6164 6572            header
-00006e00: 735f 6d61 782e 6170 7065 6e64 2872 6f77  s_max.append(row
-00006e10: 5b22 6d61 7822 5d29 0a20 2020 2020 2020  ["max"]).       
-00006e20: 2020 2020 2069 6620 6175 746f 5f69 6e64       if auto_ind
-00006e30: 6578 5f74 6872 6573 686f 6c64 3a0a 2020  ex_threshold:.  
-00006e40: 2020 2020 2020 2020 2020 2020 2020 6865                he
-00006e50: 6164 6572 735f 6361 7264 696e 616c 6974  aders_cardinalit
-00006e60: 792e 6170 7065 6e64 2869 6e74 2872 6f77  y.append(int(row
-00006e70: 5b22 6361 7264 696e 616c 6974 7922 5d29  ["cardinality"])
-00006e80: 290a 0a20 2020 2065 7869 7374 696e 6720  )..    existing 
-00006e90: 3d20 6461 7461 7374 6f72 655f 7265 736f  = datastore_reso
-00006ea0: 7572 6365 5f65 7869 7374 7328 7265 736f  urce_exists(reso
-00006eb0: 7572 6365 5f69 642c 2061 7069 5f6b 6579  urce_id, api_key
-00006ec0: 2c20 636b 616e 5f75 726c 290a 2020 2020  , ckan_url).    
-00006ed0: 6578 6973 7469 6e67 5f69 6e66 6f20 3d20  existing_info = 
-00006ee0: 4e6f 6e65 0a20 2020 2069 6620 6578 6973  None.    if exis
-00006ef0: 7469 6e67 3a0a 2020 2020 2020 2020 6578  ting:.        ex
-00006f00: 6973 7469 6e67 5f69 6e66 6f20 3d20 6469  isting_info = di
-00006f10: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-00006f20: 2866 5b22 6964 225d 2c20 665b 2269 6e66  (f["id"], f["inf
-00006f30: 6f22 5d29 2066 6f72 2066 2069 6e20 6578  o"]) for f in ex
-00006f40: 6973 7469 6e67 2e67 6574 2822 6669 656c  isting.get("fiel
-00006f50: 6473 222c 205b 5d29 2069 6620 2269 6e66  ds", []) if "inf
-00006f60: 6f22 2069 6e20 660a 2020 2020 2020 2020  o" in f.        
-00006f70: 290a 0a20 2020 2023 2069 6620 7468 6973  )..    # if this
-00006f80: 2069 7320 616e 2065 7869 7374 696e 6720   is an existing 
-00006f90: 7265 736f 7572 6365 0a20 2020 2023 206f  resource.    # o
-00006fa0: 7665 7272 6964 6520 7769 7468 2074 7970  verride with typ
-00006fb0: 6573 2075 7365 7220 7265 7175 6573 7465  es user requeste
-00006fc0: 6420 696e 2044 6174 6120 4469 6374 696f  d in Data Dictio
-00006fd0: 6e61 7279 0a20 2020 2069 6620 6578 6973  nary.    if exis
-00006fe0: 7469 6e67 5f69 6e66 6f3a 0a20 2020 2020  ting_info:.     
-00006ff0: 2020 2074 7970 6573 203d 205b 0a20 2020     types = [.   
-00007000: 2020 2020 2020 2020 207b 2274 6578 7422           {"text"
-00007010: 3a20 2253 7472 696e 6722 2c20 226e 756d  : "String", "num
-00007020: 6572 6963 223a 2022 466c 6f61 7422 2c20  eric": "Float", 
-00007030: 2274 696d 6573 7461 6d70 223a 2022 4461  "timestamp": "Da
-00007040: 7465 5469 6d65 222c 7d2e 6765 7428 0a20  teTime",}.get(. 
-00007050: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00007060: 7869 7374 696e 675f 696e 666f 2e67 6574  xisting_info.get
-00007070: 2868 2c20 7b7d 292e 6765 7428 2274 7970  (h, {}).get("typ
-00007080: 655f 6f76 6572 7269 6465 2229 2c20 740a  e_override"), t.
-00007090: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000070a0: 2020 2020 2020 2020 2020 666f 7220 742c            for t,
-000070b0: 2068 2069 6e20 7a69 7028 7479 7065 732c   h in zip(types,
-000070c0: 2068 6561 6465 7273 290a 2020 2020 2020   headers).      
-000070d0: 2020 5d0a 0a20 2020 2023 2044 656c 6574    ]..    # Delet
-000070e0: 6520 6578 6973 7469 6e67 2064 6174 6173  e existing datas
-000070f0: 746f 7265 2072 6573 6f75 7263 6520 6265  tore resource be
-00007100: 666f 7265 2070 726f 6365 6564 696e 672e  fore proceeding.
-00007110: 0a20 2020 2069 6620 6578 6973 7469 6e67  .    if existing
-00007120: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
-00007130: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-00007140: 2020 2027 4465 6c65 7469 6e67 2065 7869     'Deleting exi
-00007150: 7374 696e 6720 7265 736f 7572 6365 2022  sting resource "
-00007160: 7b72 6573 5f69 647d 2220 6672 6f6d 2064  {res_id}" from d
-00007170: 6174 6173 746f 7265 2e27 2e66 6f72 6d61  atastore.'.forma
-00007180: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00007190: 2020 2072 6573 5f69 643d 7265 736f 7572     res_id=resour
-000071a0: 6365 5f69 640a 2020 2020 2020 2020 2020  ce_id.          
-000071b0: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
-000071c0: 2020 2020 2020 6465 6c65 7465 5f64 6174        delete_dat
-000071d0: 6173 746f 7265 5f72 6573 6f75 7263 6528  astore_resource(
-000071e0: 7265 736f 7572 6365 5f69 642c 2061 7069  resource_id, api
-000071f0: 5f6b 6579 2c20 636b 616e 5f75 726c 290a  _key, ckan_url).
-00007200: 0a20 2020 2023 2031 7374 2070 6173 7320  .    # 1st pass 
-00007210: 6f66 2062 7569 6c64 696e 6720 6865 6164  of building head
-00007220: 6572 735f 6469 6374 0a20 2020 2023 2068  ers_dict.    # h
-00007230: 6572 6520 7765 206d 6170 2069 6e66 6572  ere we map infer
-00007240: 7265 6420 7479 7065 7320 746f 2070 6f73  red types to pos
-00007250: 7467 7265 7371 6c20 6461 7461 2074 7970  tgresql data typ
-00007260: 6573 0a20 2020 2074 7970 655f 6d61 7070  es.    type_mapp
-00007270: 696e 6720 3d20 636f 6e66 6967 2e67 6574  ing = config.get
-00007280: 2822 5459 5045 5f4d 4150 5049 4e47 2229  ("TYPE_MAPPING")
-00007290: 0a20 2020 2074 656d 705f 6865 6164 6572  .    temp_header
-000072a0: 735f 6469 6374 7320 3d20 5b0a 2020 2020  s_dicts = [.    
-000072b0: 2020 2020 6469 6374 2869 643d 6669 656c      dict(id=fiel
-000072c0: 645b 305d 2c20 7479 7065 3d74 7970 655f  d[0], type=type_
-000072d0: 6d61 7070 696e 675b 7374 7228 6669 656c  mapping[str(fiel
-000072e0: 645b 315d 295d 290a 2020 2020 2020 2020  d[1])]).        
-000072f0: 666f 7220 6669 656c 6420 696e 207a 6970  for field in zip
-00007300: 2868 6561 6465 7273 2c20 7479 7065 7329  (headers, types)
-00007310: 0a20 2020 205d 0a0a 2020 2020 2320 326e  .    ]..    # 2n
-00007320: 6420 7061 7373 2068 6561 6465 725f 6469  d pass header_di
-00007330: 6374 732c 2063 6865 636b 696e 6720 666f  cts, checking fo
-00007340: 7220 736d 6172 7469 6e74 2074 7970 6573  r smartint types
-00007350: 2e0a 2020 2020 2320 2273 6d61 7274 696e  ..    # "smartin
-00007360: 7422 2077 696c 6c20 6175 746f 6d61 7469  t" will automati
-00007370: 6361 6c6c 7920 7365 6c65 6374 2074 6865  cally select the
-00007380: 2062 6573 7420 696e 7465 6765 7220 6461   best integer da
-00007390: 7461 2074 7970 6520 6261 7365 6420 6f6e  ta type based on
-000073a0: 2074 6865 0a20 2020 2023 206d 696e 2f6d   the.    # min/m
-000073b0: 6178 2076 616c 7565 7320 6f66 2074 6865  ax values of the
-000073c0: 2063 6f6c 756d 6e20 7765 2067 6f74 2066   column we got f
-000073d0: 726f 6d20 7173 7620 7374 6174 730a 2020  rom qsv stats.  
-000073e0: 2020 2320 616e 6420 7365 7420 6c61 6265    # and set labe
-000073f0: 6c73 2074 6f20 6f72 6967 696e 616c 2063  ls to original c
-00007400: 6f6c 756d 6e20 6e61 6d65 7320 696e 2063  olumn names in c
-00007410: 6173 6520 7765 206d 6164 6520 7468 6520  ase we made the 
-00007420: 6e61 6d65 7320 2264 622d 7361 6665 220a  names "db-safe".
-00007430: 2020 2020 2320 6173 2074 6865 206c 6162      # as the lab
-00007440: 656c 7320 6172 6520 7573 6564 2062 7920  els are used by 
-00007450: 4461 7461 5461 626c 6573 5f76 6965 7720  DataTables_view 
-00007460: 746f 206c 6162 656c 2063 6f6c 756d 6e73  to label columns
-00007470: 0a20 2020 2023 2077 6520 616c 736f 2074  .    # we also t
-00007480: 616b 6520 6e6f 7465 206f 6620 6461 7465  ake note of date
-00007490: 7469 6d65 2f74 696d 6573 7461 6d70 2066  time/timestamp f
-000074a0: 6965 6c64 732c 2073 6f20 7765 2063 616e  ields, so we can
-000074b0: 206e 6f72 6d61 6c69 7a65 2074 6865 6d0a   normalize them.
-000074c0: 2020 2020 2320 746f 2052 4643 3333 3339      # to RFC3339
-000074d0: 2066 6f72 6d61 740a 2020 2020 6461 7465   format.    date
-000074e0: 7469 6d65 636f 6c73 5f6c 6973 7420 3d20  timecols_list = 
-000074f0: 5b5d 0a20 2020 2068 6561 6465 7273 5f64  [].    headers_d
-00007500: 6963 7473 203d 205b 5d0a 2020 2020 666f  icts = [].    fo
-00007510: 7220 6964 782c 2068 6561 6465 7220 696e  r idx, header in
-00007520: 2065 6e75 6d65 7261 7465 2874 656d 705f   enumerate(temp_
-00007530: 6865 6164 6572 735f 6469 6374 7329 3a0a  headers_dicts):.
-00007540: 2020 2020 2020 2020 6966 2068 6561 6465          if heade
-00007550: 725b 2274 7970 6522 5d20 3d3d 2022 736d  r["type"] == "sm
-00007560: 6172 7469 6e74 223a 0a20 2020 2020 2020  artint":.       
-00007570: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00007580: 2020 2020 2020 2020 2020 696e 7428 6865            int(he
-00007590: 6164 6572 735f 6d61 785b 6964 785d 2920  aders_max[idx]) 
-000075a0: 3c3d 2050 4f53 5447 5245 535f 494e 545f  <= POSTGRES_INT_
-000075b0: 4d41 580a 2020 2020 2020 2020 2020 2020  MAX.            
-000075c0: 2020 2020 616e 6420 696e 7428 6865 6164      and int(head
-000075d0: 6572 735f 6d69 6e5b 6964 785d 2920 3e3d  ers_min[idx]) >=
-000075e0: 2050 4f53 5447 5245 535f 494e 545f 4d49   POSTGRES_INT_MI
-000075f0: 4e0a 2020 2020 2020 2020 2020 2020 293a  N.            ):
-00007600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007610: 2068 6561 6465 725f 7479 7065 203d 2022   header_type = "
-00007620: 696e 7465 6765 7222 0a20 2020 2020 2020  integer".       
-00007630: 2020 2020 2065 6c69 6620 280a 2020 2020       elif (.    
-00007640: 2020 2020 2020 2020 2020 2020 696e 7428              int(
-00007650: 6865 6164 6572 735f 6d61 785b 6964 785d  headers_max[idx]
-00007660: 2920 3c3d 2050 4f53 5447 5245 535f 4249  ) <= POSTGRES_BI
-00007670: 4749 4e54 5f4d 4158 0a20 2020 2020 2020  GINT_MAX.       
-00007680: 2020 2020 2020 2020 2061 6e64 2069 6e74           and int
-00007690: 2868 6561 6465 7273 5f6d 696e 5b69 6478  (headers_min[idx
-000076a0: 5d29 203e 3d20 504f 5354 4752 4553 5f42  ]) >= POSTGRES_B
-000076b0: 4947 494e 545f 4d49 4e0a 2020 2020 2020  IGINT_MIN.      
-000076c0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
-000076d0: 2020 2020 2020 2020 2068 6561 6465 725f           header_
-000076e0: 7479 7065 203d 2022 6269 6769 6e74 220a  type = "bigint".
-000076f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00007700: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007710: 2020 6865 6164 6572 5f74 7970 6520 3d20    header_type = 
-00007720: 226e 756d 6572 6963 220a 2020 2020 2020  "numeric".      
-00007730: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007740: 2020 2020 6865 6164 6572 5f74 7970 6520      header_type 
-00007750: 3d20 6865 6164 6572 5b22 7479 7065 225d  = header["type"]
-00007760: 0a20 2020 2020 2020 2069 6620 6865 6164  .        if head
-00007770: 6572 5f74 7970 6520 3d3d 2022 7469 6d65  er_type == "time
-00007780: 7374 616d 7022 3a0a 2020 2020 2020 2020  stamp":.        
-00007790: 2020 2020 6461 7465 7469 6d65 636f 6c73      datetimecols
-000077a0: 5f6c 6973 742e 6170 7065 6e64 2868 6561  _list.append(hea
-000077b0: 6465 725b 2269 6422 5d29 0a20 2020 2020  der["id"]).     
-000077c0: 2020 2069 6e66 6f5f 6469 6374 203d 2064     info_dict = d
-000077d0: 6963 7428 6c61 6265 6c3d 6f72 6967 696e  ict(label=origin
-000077e0: 616c 5f68 6561 6465 725f 6469 6374 5b69  al_header_dict[i
-000077f0: 6478 5d29 0a20 2020 2020 2020 2068 6561  dx]).        hea
-00007800: 6465 7273 5f64 6963 7473 2e61 7070 656e  ders_dicts.appen
-00007810: 6428 6469 6374 2869 643d 6865 6164 6572  d(dict(id=header
-00007820: 5b22 6964 225d 2c20 7479 7065 3d68 6561  ["id"], type=hea
-00007830: 6465 725f 7479 7065 2c20 696e 666f 3d69  der_type, info=i
-00007840: 6e66 6f5f 6469 6374 2929 0a0a 2020 2020  nfo_dict))..    
-00007850: 2320 4d61 696e 7461 696e 2064 6174 6120  # Maintain data 
-00007860: 6469 6374 696f 6e61 7269 6573 2066 726f  dictionaries fro
-00007870: 6d20 6d61 7463 6869 6e67 2063 6f6c 756d  m matching colum
-00007880: 6e20 6e61 6d65 730a 2020 2020 6966 2065  n names.    if e
-00007890: 7869 7374 696e 675f 696e 666f 3a0a 2020  xisting_info:.  
-000078a0: 2020 2020 2020 666f 7220 6820 696e 2068        for h in h
-000078b0: 6561 6465 7273 5f64 6963 7473 3a0a 2020  eaders_dicts:.  
-000078c0: 2020 2020 2020 2020 2020 6966 2068 5b22            if h["
-000078d0: 6964 225d 2069 6e20 6578 6973 7469 6e67  id"] in existing
-000078e0: 5f69 6e66 6f3a 0a20 2020 2020 2020 2020  _info:.         
-000078f0: 2020 2020 2020 2068 5b22 696e 666f 225d         h["info"]
-00007900: 203d 2065 7869 7374 696e 675f 696e 666f   = existing_info
-00007910: 5b68 5b22 6964 225d 5d0a 2020 2020 2020  [h["id"]].      
-00007920: 2020 2020 2020 2020 2020 2320 6372 6561            # crea
-00007930: 7465 2063 6f6c 756d 6e73 2077 6974 6820  te columns with 
-00007940: 7479 7065 7320 7573 6572 2072 6571 7565  types user reque
-00007950: 7374 6564 0a20 2020 2020 2020 2020 2020  sted.           
-00007960: 2020 2020 2074 7970 655f 6f76 6572 7269       type_overri
-00007970: 6465 203d 2065 7869 7374 696e 675f 696e  de = existing_in
-00007980: 666f 5b68 5b22 6964 225d 5d2e 6765 7428  fo[h["id"]].get(
-00007990: 2274 7970 655f 6f76 6572 7269 6465 2229  "type_override")
-000079a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000079b0: 2069 6620 7479 7065 5f6f 7665 7272 6964   if type_overrid
-000079c0: 6520 696e 206c 6973 7428 7479 7065 5f6d  e in list(type_m
-000079d0: 6170 7069 6e67 2e76 616c 7565 7328 2929  apping.values())
-000079e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000079f0: 2020 2020 2020 685b 2274 7970 6522 5d20        h["type"] 
-00007a00: 3d20 7479 7065 5f6f 7665 7272 6964 650a  = type_override.
-00007a10: 0a20 2020 206c 6f67 6765 722e 696e 666f  .    logger.info
-00007a20: 280a 2020 2020 2020 2020 2244 6574 6572  (.        "Deter
-00007a30: 6d69 6e65 6420 6865 6164 6572 7320 616e  mined headers an
-00007a40: 6420 7479 7065 733a 207b 6865 6164 6572  d types: {header
-00007a50: 737d 2e2e 2e22 2e66 6f72 6d61 7428 6865  s}...".format(he
-00007a60: 6164 6572 733d 6865 6164 6572 735f 6469  aders=headers_di
-00007a70: 6374 7329 0a20 2020 2029 0a0a 2020 2020  cts).    )..    
-00007a80: 2320 6966 2050 5245 5649 4557 5f52 4f57  # if PREVIEW_ROW
-00007a90: 5320 6973 206e 6f74 207a 6572 6f2c 2063  S is not zero, c
-00007aa0: 7265 6174 6520 6120 7072 6576 6965 7720  reate a preview 
-00007ab0: 7573 696e 6720 7173 7620 736c 6963 650a  using qsv slice.
-00007ac0: 2020 2020 726f 7773 5f74 6f5f 636f 7079      rows_to_copy
-00007ad0: 203d 2072 6563 6f72 645f 636f 756e 740a   = record_count.
-00007ae0: 2020 2020 6966 2070 7265 7669 6577 5f72      if preview_r
-00007af0: 6f77 7320 616e 6420 7265 636f 7264 5f63  ows and record_c
-00007b00: 6f75 6e74 203e 2070 7265 7669 6577 5f72  ount > preview_r
-00007b10: 6f77 733a 0a20 2020 2020 2020 2069 6620  ows:.        if 
-00007b20: 7072 6576 6965 775f 726f 7773 203e 2030  preview_rows > 0
-00007b30: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00007b40: 5052 4556 4945 575f 524f 5753 2069 7320  PREVIEW_ROWS is 
-00007b50: 706f 7369 7469 7665 2c20 736c 6963 6520  positive, slice 
-00007b60: 6672 6f6d 2074 6865 2062 6567 696e 6e69  from the beginni
-00007b70: 6e67 0a20 2020 2020 2020 2020 2020 206c  ng.            l
-00007b80: 6f67 6765 722e 696e 666f 2822 5072 6570  ogger.info("Prep
-00007b90: 6172 696e 6720 7b3a 2c7d 2d72 6f77 2070  aring {:,}-row p
-00007ba0: 7265 7669 6577 2e2e 2e22 2e66 6f72 6d61  review...".forma
-00007bb0: 7428 7072 6576 6965 775f 726f 7773 2929  t(preview_rows))
-00007bc0: 0a20 2020 2020 2020 2020 2020 2071 7376  .            qsv
-00007bd0: 5f73 6c69 6365 5f63 7376 203d 2074 656d  _slice_csv = tem
-00007be0: 7066 696c 652e 4e61 6d65 6454 656d 706f  pfile.NamedTempo
-00007bf0: 7261 7279 4669 6c65 2873 7566 6669 783d  raryFile(suffix=
-00007c00: 222e 6373 7622 290a 2020 2020 2020 2020  ".csv").        
-00007c10: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00007c20: 2020 2020 2020 2020 2071 7376 5f73 6c69           qsv_sli
-00007c30: 6365 203d 2073 7562 7072 6f63 6573 732e  ce = subprocess.
-00007c40: 7275 6e28 0a20 2020 2020 2020 2020 2020  run(.           
-00007c50: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c70: 2020 2071 7376 5f62 696e 2c0a 2020 2020     qsv_bin,.    
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 2273 6c69 6365 222c 0a20 2020      "slice",.   
-00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cb0: 2020 2020 2022 2d2d 6c65 6e22 2c0a 2020       "--len",.  
-00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 2020 2020 7374 7228 7072 6576 6965        str(previe
-00007ce0: 775f 726f 7773 292c 0a20 2020 2020 2020  w_rows),.       
-00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2074 6d70 2e6e 616d 652c 0a20 2020 2020   tmp.name,.     
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2022 2d2d 6f75 7470 7574 222c 0a20     "--output",. 
-00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d40: 2020 2020 2020 2071 7376 5f73 6c69 6365         qsv_slice
-00007d50: 5f63 7376 2e6e 616d 652c 0a20 2020 2020  _csv.name,.     
-00007d60: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00007d70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007d80: 2020 2020 2020 6368 6563 6b3d 5472 7565        check=True
-00007d90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007da0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00007db0: 6578 6365 7074 2073 7562 7072 6f63 6573  except subproces
-00007dc0: 732e 4361 6c6c 6564 5072 6f63 6573 7345  s.CalledProcessE
-00007dd0: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
-00007de0: 2020 2020 2020 2020 2020 2063 6c65 616e             clean
-00007df0: 7570 5f74 656d 7066 696c 6573 2829 0a20  up_tempfiles(). 
-00007e00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00007e10: 6169 7365 2075 7469 6c2e 4a6f 6245 7272  aise util.JobErr
-00007e20: 6f72 2822 4361 6e6e 6f74 2063 7265 6174  or("Cannot creat
-00007e30: 6520 6120 7072 6576 6965 7720 736c 6963  e a preview slic
-00007e40: 653a 207b 7d22 2e66 6f72 6d61 7428 6529  e: {}".format(e)
-00007e50: 290a 2020 2020 2020 2020 2020 2020 726f  ).            ro
-00007e60: 7773 5f74 6f5f 636f 7079 203d 2070 7265  ws_to_copy = pre
-00007e70: 7669 6577 5f72 6f77 730a 2020 2020 2020  view_rows.      
-00007e80: 2020 2020 2020 746d 7020 3d20 7173 765f        tmp = qsv_
-00007e90: 736c 6963 655f 6373 760a 2020 2020 2020  slice_csv.      
-00007ea0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00007eb0: 2020 2020 2320 5052 4556 4945 575f 524f      # PREVIEW_RO
-00007ec0: 5753 2069 7320 6e65 6761 7469 7665 2c20  WS is negative, 
-00007ed0: 736c 6963 6520 6672 6f6d 2074 6865 2065  slice from the e
-00007ee0: 6e64 0a20 2020 2020 2020 2020 2020 2073  nd.            s
-00007ef0: 6c69 6365 5f6c 656e 203d 2061 6273 2870  lice_len = abs(p
-00007f00: 7265 7669 6577 5f72 6f77 7329 0a20 2020  review_rows).   
-00007f10: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00007f20: 696e 666f 2822 5072 6570 6172 696e 6720  info("Preparing 
-00007f30: 7b3a 2c7d 2d72 6f77 2070 7265 7669 6577  {:,}-row preview
-00007f40: 2066 726f 6d20 7468 6520 656e 642e 2e2e   from the end...
-00007f50: 222e 666f 726d 6174 2873 6c69 6365 5f6c  ".format(slice_l
-00007f60: 656e 2929 0a20 2020 2020 2020 2020 2020  en)).           
-00007f70: 2071 7376 5f73 6c69 6365 5f63 7376 203d   qsv_slice_csv =
-00007f80: 2074 656d 7066 696c 652e 4e61 6d65 6454   tempfile.NamedT
-00007f90: 656d 706f 7261 7279 4669 6c65 2873 7566  emporaryFile(suf
-00007fa0: 6669 783d 222e 6373 7622 290a 2020 2020  fix=".csv").    
-00007fb0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00007fc0: 2020 2020 2020 2020 2020 2020 2071 7376               qsv
-00007fd0: 5f73 6c69 6365 203d 2073 7562 7072 6f63  _slice = subproc
-00007fe0: 6573 732e 7275 6e28 0a20 2020 2020 2020  ess.run(.       
-00007ff0: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
-00008000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008010: 2020 2020 2020 2071 7376 5f62 696e 2c0a         qsv_bin,.
-00008020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008030: 2020 2020 2020 2020 2273 6c69 6365 222c          "slice",
-00008040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008050: 2020 2020 2020 2020 2022 2d2d 7374 6172           "--star
-00008060: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00008070: 2020 2020 2020 2020 2020 2020 222d 3122              "-1"
-00008080: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008090: 2020 2020 2020 2020 2020 222d 2d6c 656e            "--len
-000080a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000080b0: 2020 2020 2020 2020 2020 2073 7472 2873             str(s
-000080c0: 6c69 6365 5f6c 656e 292c 0a20 2020 2020  lice_len),.     
-000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080e0: 2020 2074 6d70 2e6e 616d 652c 0a20 2020     tmp.name,.   
-000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008100: 2020 2020 2022 2d2d 6f75 7470 7574 222c       "--output",
-00008110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008120: 2020 2020 2020 2020 2071 7376 5f73 6c69           qsv_sli
-00008130: 6365 5f63 7376 2e6e 616d 652c 0a20 2020  ce_csv.name,.   
-00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008150: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00008160: 2020 2020 2020 2020 6368 6563 6b3d 5472          check=Tr
-00008170: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00008180: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00008190: 2020 6578 6365 7074 2073 7562 7072 6f63    except subproc
-000081a0: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
-000081b0: 7345 7272 6f72 2061 7320 653a 0a20 2020  sError as e:.   
-000081c0: 2020 2020 2020 2020 2020 2020 2063 6c65               cle
-000081d0: 616e 7570 5f74 656d 7066 696c 6573 2829  anup_tempfiles()
-000081e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000081f0: 2072 6169 7365 2075 7469 6c2e 4a6f 6245   raise util.JobE
-00008200: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00008210: 2020 2020 2020 2020 2020 2243 616e 6e6f            "Canno
-00008220: 7420 6372 6561 7465 2061 2070 7265 7669  t create a previ
-00008230: 6577 2073 6c69 6365 2066 726f 6d20 7468  ew slice from th
-00008240: 6520 656e 643a 207b 7d22 2e66 6f72 6d61  e end: {}".forma
-00008250: 7428 6529 0a20 2020 2020 2020 2020 2020  t(e).           
-00008260: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00008270: 2020 2072 6f77 735f 746f 5f63 6f70 7920     rows_to_copy 
-00008280: 3d20 736c 6963 655f 6c65 6e0a 2020 2020  = slice_len.    
-00008290: 2020 2020 2020 2020 746d 7020 3d20 7173          tmp = qs
-000082a0: 765f 736c 6963 655f 6373 760a 0a20 2020  v_slice_csv..   
-000082b0: 2023 2069 6620 7468 6572 6520 6172 6520   # if there are 
-000082c0: 616e 7920 6461 7465 7469 6d65 2066 6965  any datetime fie
-000082d0: 6c64 732c 206e 6f72 6d61 6c69 7a65 2074  lds, normalize t
-000082e0: 6865 6d20 746f 2052 4643 3333 3339 2066  hem to RFC3339 f
-000082f0: 6f72 6d61 740a 2020 2020 2320 736f 2077  ormat.    # so w
-00008300: 6520 6361 6e20 7265 6164 696c 7920 696e  e can readily in
-00008310: 7365 7274 2074 6865 6d20 6173 2074 696d  sert them as tim
-00008320: 6573 7461 6d70 7320 696e 746f 2070 6f73  estamps into pos
-00008330: 7467 7265 7371 6c20 7769 7468 2043 4f50  tgresql with COP
-00008340: 590a 2020 2020 6966 2064 6174 6574 696d  Y.    if datetim
-00008350: 6563 6f6c 735f 6c69 7374 3a0a 2020 2020  ecols_list:.    
-00008360: 2020 2020 7173 765f 6170 706c 7964 705f      qsv_applydp_
-00008370: 6373 7620 3d20 7465 6d70 6669 6c65 2e4e  csv = tempfile.N
-00008380: 616d 6564 5465 6d70 6f72 6172 7946 696c  amedTemporaryFil
-00008390: 6528 7375 6666 6978 3d22 2e63 7376 2229  e(suffix=".csv")
-000083a0: 0a20 2020 2020 2020 2064 6174 6563 6f6c  .        datecol
-000083b0: 7320 3d20 222c 222e 6a6f 696e 2864 6174  s = ",".join(dat
-000083c0: 6574 696d 6563 6f6c 735f 6c69 7374 290a  etimecols_list).
-000083d0: 0a20 2020 2020 2020 2071 7376 5f61 7070  .        qsv_app
-000083e0: 6c79 6470 5f63 6d64 203d 205b 0a20 2020  lydp_cmd = [.   
-000083f0: 2020 2020 2020 2020 2071 7376 5f62 696e           qsv_bin
-00008400: 2c0a 2020 2020 2020 2020 2020 2020 2261  ,.            "a
-00008410: 7070 6c79 6470 222c 0a20 2020 2020 2020  pplydp",.       
-00008420: 2020 2020 2022 6461 7465 666d 7422 2c0a       "datefmt",.
-00008430: 2020 2020 2020 2020 2020 2020 6461 7465              date
-00008440: 636f 6c73 2c0a 2020 2020 2020 2020 2020  cols,.          
-00008450: 2020 746d 702e 6e61 6d65 2c0a 2020 2020    tmp.name,.    
-00008460: 2020 2020 2020 2020 222d 2d6f 7574 7075          "--outpu
-00008470: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00008480: 7173 765f 6170 706c 7964 705f 6373 762e  qsv_applydp_csv.
-00008490: 6e61 6d65 2c0a 2020 2020 2020 2020 5d0a  name,.        ].
-000084a0: 2020 2020 2020 2020 6966 2070 7265 6665          if prefe
-000084b0: 725f 646d 793a 0a20 2020 2020 2020 2020  r_dmy:.         
-000084c0: 2020 2071 7376 5f61 7070 6c79 6470 5f63     qsv_applydp_c
-000084d0: 6d64 2e61 7070 656e 6428 222d 2d70 7265  md.append("--pre
-000084e0: 6665 725f 646d 7922 290a 2020 2020 2020  fer_dmy").      
-000084f0: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
-00008500: 2020 2020 2020 2020 2020 2027 466f 726d             'Form
-00008510: 6174 7469 6e67 2064 6174 6573 2022 7b7d  atting dates "{}
-00008520: 2220 746f 2049 534f 2038 3630 312f 5246  " to ISO 8601/RF
-00008530: 4320 3333 3339 2066 6f72 6d61 7420 7769  C 3339 format wi
-00008540: 7468 2050 5245 4645 525f 444d 593a 207b  th PREFER_DMY: {
-00008550: 7d2e 2e2e 272e 666f 726d 6174 280a 2020  }...'.format(.  
-00008560: 2020 2020 2020 2020 2020 2020 2020 6461                da
-00008570: 7465 636f 6c73 2c20 7072 6566 6572 5f64  tecols, prefer_d
-00008580: 6d79 0a20 2020 2020 2020 2020 2020 2029  my.            )
-00008590: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000085a0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-000085b0: 2020 2020 7173 765f 6170 706c 7964 7020      qsv_applydp 
-000085c0: 3d20 7375 6270 726f 6365 7373 2e72 756e  = subprocess.run
-000085d0: 2871 7376 5f61 7070 6c79 6470 5f63 6d64  (qsv_applydp_cmd
-000085e0: 2c20 6368 6563 6b3d 5472 7565 290a 2020  , check=True).  
-000085f0: 2020 2020 2020 6578 6365 7074 2073 7562        except sub
-00008600: 7072 6f63 6573 732e 4361 6c6c 6564 5072  process.CalledPr
-00008610: 6f63 6573 7345 7272 6f72 2061 7320 653a  ocessError as e:
-00008620: 0a20 2020 2020 2020 2020 2020 2063 6c65  .            cle
-00008630: 616e 7570 5f74 656d 7066 696c 6573 2829  anup_tempfiles()
-00008640: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00008650: 7365 2075 7469 6c2e 4a6f 6245 7272 6f72  se util.JobError
-00008660: 2822 4170 706c 7964 7020 6572 726f 723a  ("Applydp error:
-00008670: 207b 7d22 2e66 6f72 6d61 7428 6529 290a   {}".format(e)).
-00008680: 2020 2020 2020 2020 746d 7020 3d20 7173          tmp = qs
-00008690: 765f 6170 706c 7964 705f 6373 760a 0a20  v_applydp_csv.. 
-000086a0: 2020 2061 6e61 6c79 7369 735f 656c 6170     analysis_elap
-000086b0: 7365 6420 3d20 7469 6d65 2e70 6572 665f  sed = time.perf_
-000086c0: 636f 756e 7465 7228 2920 2d20 616e 616c  counter() - anal
-000086d0: 7973 6973 5f73 7461 7274 0a20 2020 206c  ysis_start.    l
-000086e0: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
-000086f0: 2020 2020 2241 4e41 4c59 5349 5320 444f      "ANALYSIS DO
-00008700: 4e45 2120 416e 616c 797a 6564 2061 6e64  NE! Analyzed and
-00008710: 2070 7265 7070 6564 2069 6e20 7b3a 2c2e   prepped in {:,.
-00008720: 3266 7d20 7365 636f 6e64 732e 222e 666f  2f} seconds.".fo
-00008730: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
-00008740: 2020 616e 616c 7973 6973 5f65 6c61 7073    analysis_elaps
-00008750: 6564 0a20 2020 2020 2020 2029 0a20 2020  ed.        ).   
-00008760: 2029 0a0a 2020 2020 2320 6174 2074 6869   )..    # at thi
-00008770: 7320 7374 6167 652c 2074 6865 2072 6573  s stage, the res
-00008780: 6f75 7263 6520 6973 2072 6561 6479 2066  ource is ready f
-00008790: 6f72 2043 4f50 5969 6e67 2074 6f20 7468  or COPYing to th
-000087a0: 6520 4461 7461 7374 6f72 650a 0a20 2020  e Datastore..   
-000087b0: 2069 6620 6472 795f 7275 6e3a 0a20 2020   if dry_run:.   
-000087c0: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
-000087d0: 696e 6728 2244 7279 2072 756e 206f 6e6c  ing("Dry run onl
-000087e0: 792e 2052 6574 7572 6e69 6e67 2077 6974  y. Returning wit
-000087f0: 686f 7574 2063 6f70 7969 6e67 2074 6f20  hout copying to 
-00008800: 7468 6520 4461 7461 7374 6f72 652e 2e2e  the Datastore...
-00008810: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00008820: 6e20 6865 6164 6572 735f 6469 6374 730a  n headers_dicts.
-00008830: 0a20 2020 206c 6f67 6765 722e 696e 666f  .    logger.info
-00008840: 2822 434f 5059 494e 4720 7b3a 2c7d 2072  ("COPYING {:,} r
-00008850: 6f77 7320 746f 2044 6174 6173 746f 7265  ows to Datastore
-00008860: 2e2e 2e22 2e66 6f72 6d61 7428 726f 7773  ...".format(rows
-00008870: 5f74 6f5f 636f 7079 2929 0a20 2020 2063  _to_copy)).    c
-00008880: 6f70 795f 7374 6172 7420 3d20 7469 6d65  opy_start = time
-00008890: 2e70 6572 665f 636f 756e 7465 7228 290a  .perf_counter().
-000088a0: 0a20 2020 2023 2066 6972 7374 2c20 6c65  .    # first, le
-000088b0: 7427 7320 6372 6561 7465 2061 6e20 656d  t's create an em
-000088c0: 7074 7920 6461 7461 7374 6f72 6520 7461  pty datastore ta
-000088d0: 626c 6520 772f 2067 7565 7373 6564 2074  ble w/ guessed t
-000088e0: 7970 6573 0a20 2020 2073 656e 645f 7265  ypes.    send_re
-000088f0: 736f 7572 6365 5f74 6f5f 6461 7461 7374  source_to_datast
-00008900: 6f72 6528 0a20 2020 2020 2020 2072 6573  ore(.        res
-00008910: 6f75 7263 653d 4e6f 6e65 2c0a 2020 2020  ource=None,.    
-00008920: 2020 2020 7265 736f 7572 6365 5f69 643d      resource_id=
-00008930: 7265 736f 7572 6365 5b22 6964 225d 2c0a  resource["id"],.
-00008940: 2020 2020 2020 2020 6865 6164 6572 733d          headers=
-00008950: 6865 6164 6572 735f 6469 6374 732c 0a20  headers_dicts,. 
-00008960: 2020 2020 2020 2061 7069 5f6b 6579 3d61         api_key=a
-00008970: 7069 5f6b 6579 2c0a 2020 2020 2020 2020  pi_key,.        
-00008980: 636b 616e 5f75 726c 3d63 6b61 6e5f 7572  ckan_url=ckan_ur
-00008990: 6c2c 0a20 2020 2020 2020 2072 6563 6f72  l,.        recor
-000089a0: 6473 3d4e 6f6e 652c 0a20 2020 2020 2020  ds=None,.       
-000089b0: 2061 6c69 6173 6573 3d4e 6f6e 652c 0a20   aliases=None,. 
-000089c0: 2020 2020 2020 2063 616c 6375 6c61 7465         calculate
-000089d0: 5f72 6563 6f72 645f 636f 756e 743d 4661  _record_count=Fa
-000089e0: 6c73 652c 0a20 2020 2029 0a0a 2020 2020  lse,.    )..    
-000089f0: 636f 7069 6564 5f63 6f75 6e74 203d 2030  copied_count = 0
-00008a00: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
-00008a10: 2020 7261 775f 636f 6e6e 6563 7469 6f6e    raw_connection
-00008a20: 203d 2070 7379 636f 7067 322e 636f 6e6e   = psycopg2.conn
-00008a30: 6563 7428 636f 6e66 6967 2e67 6574 2822  ect(config.get("
-00008a40: 5752 4954 455f 454e 4749 4e45 5f55 524c  WRITE_ENGINE_URL
-00008a50: 2229 290a 2020 2020 6578 6365 7074 2070  ")).    except p
-00008a60: 7379 636f 7067 322e 4572 726f 7220 6173  sycopg2.Error as
-00008a70: 2065 3a0a 2020 2020 2020 2020 636c 6561   e:.        clea
-00008a80: 6e75 705f 7465 6d70 6669 6c65 7328 290a  nup_tempfiles().
-00008a90: 2020 2020 2020 2020 7261 6973 6520 7574          raise ut
-00008aa0: 696c 2e4a 6f62 4572 726f 7228 2243 6f75  il.JobError("Cou
-00008ab0: 6c64 206e 6f74 2063 6f6e 6e65 6374 2074  ld not connect t
-00008ac0: 6f20 7468 6520 4461 7461 7374 6f72 653a  o the Datastore:
-00008ad0: 207b 7d22 2e66 6f72 6d61 7428 6529 290a   {}".format(e)).
-00008ae0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00008af0: 2020 6375 7220 3d20 7261 775f 636f 6e6e    cur = raw_conn
-00008b00: 6563 7469 6f6e 2e63 7572 736f 7228 290a  ection.cursor().
-00008b10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00008b20: 2020 2020 7472 756e 6361 7465 2074 6162      truncate tab
-00008b30: 6c65 2074 6f20 7573 6520 636f 7079 2066  le to use copy f
-00008b40: 7265 657a 6520 6f70 7469 6f6e 2061 6e64  reeze option and
-00008b50: 2066 7572 7468 6572 2069 6e63 7265 6173   further increas
-00008b60: 650a 2020 2020 2020 2020 7065 7266 6f72  e.        perfor
-00008b70: 6d61 6e63 6520 6173 2074 6865 7265 2069  mance as there i
-00008b80: 7320 6e6f 206e 6565 6420 666f 7220 5741  s no need for WA
-00008b90: 4c20 6c6f 6773 2074 6f20 6265 206d 6169  L logs to be mai
-00008ba0: 6e74 6169 6e65 640a 2020 2020 2020 2020  ntained.        
-00008bb0: 6874 7470 733a 2f2f 7777 772e 706f 7374  https://www.post
-00008bc0: 6772 6573 716c 2e6f 7267 2f64 6f63 732f  gresql.org/docs/
-00008bd0: 392e 312f 706f 7075 6c61 7465 2e68 746d  9.1/populate.htm
-00008be0: 6c23 504f 5055 4c41 5445 2d43 4f50 592d  l#POPULATE-COPY-
-00008bf0: 4652 4f4d 0a20 2020 2020 2020 2022 2222  FROM.        """
-00008c00: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00008c10: 2020 2020 2020 2020 2020 6375 722e 6578            cur.ex
-00008c20: 6563 7574 6528 0a20 2020 2020 2020 2020  ecute(.         
-00008c30: 2020 2020 2020 2073 716c 2e53 514c 2822         sql.SQL("
-00008c40: 5452 554e 4341 5445 2054 4142 4c45 207b  TRUNCATE TABLE {
-00008c50: 7d22 292e 666f 726d 6174 2873 716c 2e49  }").format(sql.I
-00008c60: 6465 6e74 6966 6965 7228 7265 736f 7572  dentifier(resour
-00008c70: 6365 5f69 6429 290a 2020 2020 2020 2020  ce_id)).        
-00008c80: 2020 2020 290a 0a20 2020 2020 2020 2065      )..        e
-00008c90: 7863 6570 7420 7073 7963 6f70 6732 2e45  xcept psycopg2.E
-00008ca0: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
-00008cb0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-00008cc0: 726e 696e 6728 2243 6f75 6c64 206e 6f74  rning("Could not
-00008cd0: 2054 5255 4e43 4154 453a 207b 7d22 2e66   TRUNCATE: {}".f
-00008ce0: 6f72 6d61 7428 6529 290a 0a20 2020 2020  ormat(e))..     
-00008cf0: 2020 2063 6f70 795f 7371 6c20 3d20 280a     copy_sql = (.
-00008d00: 2020 2020 2020 2020 2020 2020 2743 4f50              'COP
-00008d10: 5920 227b 7265 736f 7572 6365 5f69 647d  Y "{resource_id}
-00008d20: 2220 287b 636f 6c75 6d6e 5f6e 616d 6573  " ({column_names
-00008d30: 7d29 2046 524f 4d20 5354 4449 4e20 270a  }) FROM STDIN '.
-00008d40: 2020 2020 2020 2020 2020 2020 2257 4954              "WIT
-00008d50: 4820 2846 4f52 4d41 5420 4353 562c 2046  H (FORMAT CSV, F
-00008d60: 5245 455a 4520 312c 2022 0a20 2020 2020  REEZE 1, ".     
-00008d70: 2020 2020 2020 2022 4845 4144 4552 2031         "HEADER 1
-00008d80: 2c20 454e 434f 4449 4e47 2027 5554 4638  , ENCODING 'UTF8
-00008d90: 2729 3b22 0a20 2020 2020 2020 2029 2e66  ');".        ).f
-00008da0: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
-00008db0: 2020 2072 6573 6f75 7263 655f 6964 3d72     resource_id=r
-00008dc0: 6573 6f75 7263 655f 6964 2c0a 2020 2020  esource_id,.    
-00008dd0: 2020 2020 2020 2020 636f 6c75 6d6e 5f6e          column_n
-00008de0: 616d 6573 3d22 2c20 222e 6a6f 696e 285b  ames=", ".join([
-00008df0: 2722 7b7d 2227 2e66 6f72 6d61 7428 685b  '"{}"'.format(h[
-00008e00: 2269 6422 5d29 2066 6f72 2068 2069 6e20  "id"]) for h in 
-00008e10: 6865 6164 6572 735f 6469 6374 735d 292c  headers_dicts]),
-00008e20: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-00008e30: 2020 206c 6f67 6765 722e 696e 666f 2863     logger.info(c
-00008e40: 6f70 795f 7371 6c29 0a20 2020 2020 2020  opy_sql).       
-00008e50: 2077 6974 6820 6f70 656e 2874 6d70 2e6e   with open(tmp.n
-00008e60: 616d 652c 2022 7262 2229 2061 7320 663a  ame, "rb") as f:
-00008e70: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00008e80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008e90: 2020 6375 722e 636f 7079 5f65 7870 6572    cur.copy_exper
-00008ea0: 7428 636f 7079 5f73 716c 2c20 6629 0a20  t(copy_sql, f). 
-00008eb0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00008ec0: 7420 7073 7963 6f70 6732 2e45 7272 6f72  t psycopg2.Error
-00008ed0: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00008ee0: 2020 2020 2020 2063 6c65 616e 7570 5f74         cleanup_t
-00008ef0: 656d 7066 696c 6573 2829 0a20 2020 2020  empfiles().     
-00008f00: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00008f10: 2075 7469 6c2e 4a6f 6245 7272 6f72 2822   util.JobError("
-00008f20: 506f 7374 6772 6573 2043 4f50 5920 6661  Postgres COPY fa
-00008f30: 696c 6564 3a20 7b7d 222e 666f 726d 6174  iled: {}".format
-00008f40: 2865 2929 0a20 2020 2020 2020 2020 2020  (e)).           
-00008f50: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00008f60: 2020 2020 2020 2063 6f70 6965 645f 636f         copied_co
-00008f70: 756e 7420 3d20 6375 722e 726f 7763 6f75  unt = cur.rowcou
-00008f80: 6e74 0a0a 2020 2020 2020 2020 7261 775f  nt..        raw_
-00008f90: 636f 6e6e 6563 7469 6f6e 2e63 6f6d 6d69  connection.commi
-00008fa0: 7428 290a 2020 2020 2020 2020 2320 7468  t().        # th
-00008fb0: 6973 2069 7320 6e65 6564 6564 2074 6f20  is is needed to 
-00008fc0: 6973 7375 6520 6120 5641 4355 554d 2041  issue a VACUUM A
-00008fd0: 4e41 4c59 5a45 0a20 2020 2020 2020 2072  NALYZE.        r
-00008fe0: 6177 5f63 6f6e 6e65 6374 696f 6e2e 7365  aw_connection.se
-00008ff0: 745f 6973 6f6c 6174 696f 6e5f 6c65 7665  t_isolation_leve
-00009000: 6c28 0a20 2020 2020 2020 2020 2020 2070  l(.            p
-00009010: 7379 636f 7067 322e 6578 7465 6e73 696f  sycopg2.extensio
-00009020: 6e73 2e49 534f 4c41 5449 4f4e 5f4c 4556  ns.ISOLATION_LEV
-00009030: 454c 5f41 5554 4f43 4f4d 4d49 540a 2020  EL_AUTOCOMMIT.  
-00009040: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00009050: 616e 616c 797a 655f 6375 7220 3d20 7261  analyze_cur = ra
-00009060: 775f 636f 6e6e 6563 7469 6f6e 2e63 7572  w_connection.cur
-00009070: 736f 7228 290a 2020 2020 2020 2020 616e  sor().        an
-00009080: 616c 797a 655f 6375 722e 6578 6563 7574  alyze_cur.execut
-00009090: 6528 0a20 2020 2020 2020 2020 2020 2073  e(.            s
-000090a0: 716c 2e53 514c 2822 5641 4355 554d 2041  ql.SQL("VACUUM A
-000090b0: 4e41 4c59 5a45 207b 7d22 292e 666f 726d  NALYZE {}").form
-000090c0: 6174 2873 716c 2e49 6465 6e74 6966 6965  at(sql.Identifie
-000090d0: 7228 7265 736f 7572 6365 5f69 6429 290a  r(resource_id)).
-000090e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000090f0: 2020 616e 616c 797a 655f 6375 722e 636c    analyze_cur.cl
-00009100: 6f73 6528 290a 0a20 2020 2063 6f70 795f  ose()..    copy_
-00009110: 656c 6170 7365 6420 3d20 7469 6d65 2e70  elapsed = time.p
-00009120: 6572 665f 636f 756e 7465 7228 2920 2d20  erf_counter() - 
-00009130: 636f 7079 5f73 7461 7274 0a20 2020 206c  copy_start.    l
-00009140: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
-00009150: 2020 2020 272e 2e2e 636f 7079 696e 6720      '...copying 
-00009160: 646f 6e65 2e20 436f 7069 6564 207b 6e7d  done. Copied {n}
-00009170: 2072 6f77 7320 746f 2022 7b72 6573 5f69   rows to "{res_i
-00009180: 647d 2220 696e 207b 636f 7079 5f65 6c61  d}" in {copy_ela
-00009190: 7073 6564 7d20 7365 636f 6e64 732e 272e  psed} seconds.'.
-000091a0: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-000091b0: 2020 2020 6e3d 227b 3a2c 7d22 2e66 6f72      n="{:,}".for
-000091c0: 6d61 7428 636f 7069 6564 5f63 6f75 6e74  mat(copied_count
-000091d0: 292c 0a20 2020 2020 2020 2020 2020 2072  ),.            r
-000091e0: 6573 5f69 643d 7265 736f 7572 6365 5f69  es_id=resource_i
-000091f0: 642c 0a20 2020 2020 2020 2020 2020 2063  d,.            c
-00009200: 6f70 795f 656c 6170 7365 643d 227b 3a2c  opy_elapsed="{:,
-00009210: 2e32 667d 222e 666f 726d 6174 2863 6f70  .2f}".format(cop
-00009220: 795f 656c 6170 7365 6429 2c0a 2020 2020  y_elapsed),.    
-00009230: 2020 2020 290a 2020 2020 290a 0a20 2020      ).    )..   
-00009240: 2072 6573 6f75 7263 655b 2264 6174 6173   resource["datas
-00009250: 746f 7265 5f61 6374 6976 6522 5d20 3d20  tore_active"] = 
-00009260: 5472 7565 0a20 2020 2072 6573 6f75 7263  True.    resourc
-00009270: 655b 2274 6f74 616c 5f72 6563 6f72 645f  e["total_record_
-00009280: 636f 756e 7422 5d20 3d20 7265 636f 7264  count"] = record
-00009290: 5f63 6f75 6e74 0a20 2020 2069 6620 7072  _count.    if pr
-000092a0: 6576 6965 775f 726f 7773 203c 2072 6563  eview_rows < rec
-000092b0: 6f72 645f 636f 756e 7420 6f72 2028 7072  ord_count or (pr
-000092c0: 6576 6965 775f 726f 7773 203e 2030 2061  eview_rows > 0 a
-000092d0: 6e64 2064 6f77 6e6c 6f61 645f 7072 6576  nd download_prev
-000092e0: 6965 775f 6f6e 6c79 293a 0a20 2020 2020  iew_only):.     
-000092f0: 2020 2072 6573 6f75 7263 655b 2270 7265     resource["pre
-00009300: 7669 6577 225d 203d 2054 7275 650a 2020  view"] = True.  
-00009310: 2020 2020 2020 7265 736f 7572 6365 5b22        resource["
-00009320: 7072 6576 6965 775f 726f 7773 225d 203d  preview_rows"] =
-00009330: 2063 6f70 6965 645f 636f 756e 740a 2020   copied_count.  
-00009340: 2020 2020 2020 7265 736f 7572 6365 5b22        resource["
-00009350: 7061 7274 6961 6c5f 646f 776e 6c6f 6164  partial_download
-00009360: 225d 203d 2064 6f77 6e6c 6f61 645f 7072  "] = download_pr
-00009370: 6576 6965 775f 6f6e 6c79 0a20 2020 2075  eview_only.    u
-00009380: 7064 6174 655f 7265 736f 7572 6365 2872  pdate_resource(r
-00009390: 6573 6f75 7263 652c 2061 7069 5f6b 6579  esource, api_key
-000093a0: 2c20 636b 616e 5f75 726c 290a 0a20 2020  , ckan_url)..   
-000093b0: 2023 2061 6c69 6173 6573 2061 7265 2068   # aliases are h
-000093c0: 756d 616e 2d72 6561 6461 626c 652c 2061  uman-readable, a
-000093d0: 6e64 206d 616b 6520 6974 2065 6173 6965  nd make it easie
-000093e0: 7220 746f 2075 7365 2074 6861 6e20 7265  r to use than re
-000093f0: 736f 7572 6365 2069 6420 6861 7368 0a20  source id hash. 
-00009400: 2020 2023 2069 6e20 7573 696e 6720 7468     # in using th
-00009410: 6520 4461 7461 7374 6f72 6520 4150 4920  e Datastore API 
-00009420: 616e 6420 696e 2053 514c 2071 7565 7269  and in SQL queri
-00009430: 6573 0a20 2020 2061 7574 6f5f 616c 6961  es.    auto_alia
-00009440: 7320 3d20 636f 6e66 6967 2e67 6574 2822  s = config.get("
-00009450: 4155 544f 5f41 4c49 4153 2229 0a20 2020  AUTO_ALIAS").   
-00009460: 2061 7574 6f5f 616c 6961 735f 756e 6971   auto_alias_uniq
-00009470: 7565 203d 2063 6f6e 6669 672e 6765 7428  ue = config.get(
-00009480: 2241 5554 4f5f 414c 4941 535f 554e 4951  "AUTO_ALIAS_UNIQ
-00009490: 5545 2229 0a20 2020 2069 6620 6175 746f  UE").    if auto
-000094a0: 5f61 6c69 6173 3a0a 2020 2020 2020 2020  _alias:.        
-000094b0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
-000094c0: 2020 2020 2020 2020 2022 4155 544f 2d41           "AUTO-A
-000094d0: 4c49 4153 494e 472e 2041 7574 6f2d 616c  LIASING. Auto-al
-000094e0: 6961 732d 756e 6971 7565 3a20 7b7d 202e  ias-unique: {} .
-000094f0: 2e2e 222e 666f 726d 6174 2861 7574 6f5f  ..".format(auto_
-00009500: 616c 6961 735f 756e 6971 7565 290a 2020  alias_unique).  
-00009510: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00009520: 2320 6765 7420 7061 636b 6167 6520 696e  # get package in
-00009530: 666f 2c20 736f 2077 6520 6361 6e20 636f  fo, so we can co
-00009540: 6e73 7472 7563 7420 7468 6520 616c 6961  nstruct the alia
-00009550: 730a 2020 2020 2020 2020 7061 636b 6167  s.        packag
-00009560: 6520 3d20 6765 745f 7061 636b 6167 6528  e = get_package(
-00009570: 7265 736f 7572 6365 5b22 7061 636b 6167  resource["packag
-00009580: 655f 6964 225d 2c20 636b 616e 5f75 726c  e_id"], ckan_url
-00009590: 2c20 6170 695f 6b65 7929 0a0a 2020 2020  , api_key)..    
-000095a0: 2020 2020 7265 736f 7572 6365 5f6e 616d      resource_nam
-000095b0: 6520 3d20 7265 736f 7572 6365 2e67 6574  e = resource.get
-000095c0: 2822 6e61 6d65 2229 0a20 2020 2020 2020  ("name").       
-000095d0: 2070 6163 6b61 6765 5f6e 616d 6520 3d20   package_name = 
-000095e0: 7061 636b 6167 652e 6765 7428 226e 616d  package.get("nam
-000095f0: 6522 290a 2020 2020 2020 2020 6f77 6e65  e").        owne
-00009600: 725f 6f72 6720 3d20 7061 636b 6167 652e  r_org = package.
-00009610: 6765 7428 226f 7267 616e 697a 6174 696f  get("organizatio
-00009620: 6e22 290a 2020 2020 2020 2020 6f77 6e65  n").        owne
-00009630: 725f 6f72 675f 6e61 6d65 203d 2022 220a  r_org_name = "".
-00009640: 2020 2020 2020 2020 6966 206f 776e 6572          if owner
-00009650: 5f6f 7267 3a0a 2020 2020 2020 2020 2020  _org:.          
-00009660: 2020 6f77 6e65 725f 6f72 675f 6e61 6d65    owner_org_name
-00009670: 203d 206f 776e 6572 5f6f 7267 2e67 6574   = owner_org.get
-00009680: 2822 6e61 6d65 2229 0a20 2020 2020 2020  ("name").       
-00009690: 2069 6620 7265 736f 7572 6365 5f6e 616d   if resource_nam
-000096a0: 6520 616e 6420 7061 636b 6167 655f 6e61  e and package_na
-000096b0: 6d65 2061 6e64 206f 776e 6572 5f6f 7267  me and owner_org
-000096c0: 5f6e 616d 653a 0a20 2020 2020 2020 2020  _name:.         
-000096d0: 2020 2023 2077 6520 6c69 6d69 7420 6974     # we limit it
-000096e0: 2074 6f20 3535 2c20 736f 2077 6520 7374   to 55, so we st
-000096f0: 696c 6c20 6861 7665 2073 7061 6365 2066  ill have space f
-00009700: 6f72 2073 6571 7565 6e63 6520 2620 7374  or sequence & st
-00009710: 6174 7320 7375 6666 6978 0a20 2020 2020  ats suffix.     
-00009720: 2020 2020 2020 2023 2070 6f73 7467 7265         # postgre
-00009730: 7320 6d61 7820 6964 656e 7469 6669 6572  s max identifier
-00009740: 206c 656e 6774 6820 6973 2036 330a 2020   length is 63.  
-00009750: 2020 2020 2020 2020 2020 616c 6961 7320            alias 
-00009760: 3d20 6622 7b72 6573 6f75 7263 655f 6e61  = f"{resource_na
-00009770: 6d65 7d2d 7b70 6163 6b61 6765 5f6e 616d  me}-{package_nam
-00009780: 657d 2d7b 6f77 6e65 725f 6f72 675f 6e61  e}-{owner_org_na
-00009790: 6d65 7d22 5b3a 3535 5d0a 2020 2020 2020  me}"[:55].      
-000097a0: 2020 2020 2020 2320 6966 2041 5554 4f5f        # if AUTO_
-000097b0: 414c 4941 535f 554e 4951 5545 2069 7320  ALIAS_UNIQUE is 
-000097c0: 7472 7565 2c20 6368 6563 6b20 6966 2074  true, check if t
-000097d0: 6865 2061 6c69 6173 2061 6c72 6561 6479  he alias already
-000097e0: 2065 7869 7374 2c20 6966 2069 7420 646f   exist, if it do
-000097f0: 6573 0a20 2020 2020 2020 2020 2020 2023  es.            #
-00009800: 2061 6464 2061 2073 6571 7565 6e63 6520   add a sequence 
-00009810: 7375 6666 6978 2073 6f20 7468 6520 6e65  suffix so the ne
-00009820: 7720 616c 6961 7320 6361 6e20 6265 2063  w alias can be c
-00009830: 7265 6174 6564 0a20 2020 2020 2020 2020  reated.         
-00009840: 2020 2063 7572 2e65 7865 6375 7465 280a     cur.execute(.
-00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009860: 2253 454c 4543 5420 434f 554e 5428 2a29  "SELECT COUNT(*)
-00009870: 2c20 616c 6961 735f 6f66 2046 524f 4d20  , alias_of FROM 
-00009880: 5f74 6162 6c65 5f6d 6574 6164 6174 6120  _table_metadata 
-00009890: 7768 6572 6520 6e61 6d65 206c 696b 6520  where name like 
-000098a0: 2573 2067 726f 7570 2062 7920 616c 6961  %s group by alia
-000098b0: 735f 6f66 222c 0a20 2020 2020 2020 2020  s_of",.         
-000098c0: 2020 2020 2020 2028 616c 6961 7320 2b20         (alias + 
-000098d0: 2225 222c 292c 0a20 2020 2020 2020 2020  "%",),.         
-000098e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000098f0: 2061 6c69 6173 5f71 7565 7279 5f72 6573   alias_query_res
-00009900: 756c 7420 3d20 6375 722e 6665 7463 686f  ult = cur.fetcho
-00009910: 6e65 2829 0a20 2020 2020 2020 2020 2020  ne().           
-00009920: 2069 6620 616c 6961 735f 7175 6572 795f   if alias_query_
-00009930: 7265 7375 6c74 3a0a 2020 2020 2020 2020  result:.        
-00009940: 2020 2020 2020 2020 616c 6961 735f 636f          alias_co
-00009950: 756e 7420 3d20 616c 6961 735f 7175 6572  unt = alias_quer
-00009960: 795f 7265 7375 6c74 5b30 5d0a 2020 2020  y_result[0].    
-00009970: 2020 2020 2020 2020 2020 2020 6578 6973              exis
-00009980: 7469 6e67 5f61 6c69 6173 5f6f 6620 3d20  ting_alias_of = 
-00009990: 616c 6961 735f 7175 6572 795f 7265 7375  alias_query_resu
-000099a0: 6c74 5b31 5d0a 2020 2020 2020 2020 2020  lt[1].          
-000099b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000099c0: 2020 2020 2020 2020 616c 6961 735f 636f          alias_co
-000099d0: 756e 7420 3d20 300a 2020 2020 2020 2020  unt = 0.        
-000099e0: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
-000099f0: 5f61 6c69 6173 5f6f 6620 3d20 2222 0a20  _alias_of = "". 
-00009a00: 2020 2020 2020 2020 2020 2069 6620 6175             if au
-00009a10: 746f 5f61 6c69 6173 5f75 6e69 7175 6520  to_alias_unique 
-00009a20: 616e 6420 616c 6961 735f 636f 756e 7420  and alias_count 
-00009a30: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
-00009a40: 2020 2020 2061 6c69 6173 5f73 6571 7565       alias_seque
-00009a50: 6e63 6520 3d20 616c 6961 735f 636f 756e  nce = alias_coun
-00009a60: 7420 2b20 310a 2020 2020 2020 2020 2020  t + 1.          
-00009a70: 2020 2020 2020 7768 696c 6520 5472 7565        while True
-00009a80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009a90: 2020 2020 2020 2320 7765 2064 6f20 7468        # we do th
-00009aa0: 6973 2c20 736f 2077 6527 7265 2063 6572  is, so we're cer
-00009ab0: 7461 696e 2074 6865 206e 6577 2061 6c69  tain the new ali
-00009ac0: 6173 2064 6f65 7320 6e6f 7420 6578 6973  as does not exis
-00009ad0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00009ae0: 2020 2020 2020 2320 6a75 7374 2069 6e20        # just in 
-00009af0: 6361 7365 2074 6865 7920 6465 6c65 7465  case they delete
-00009b00: 6420 616e 206f 6c64 6572 2061 6c69 6173  d an older alias
-00009b10: 2077 6974 6820 6120 6c6f 7765 7220 7365   with a lower se
-00009b20: 7175 656e 6365 2023 0a20 2020 2020 2020  quence #.       
-00009b30: 2020 2020 2020 2020 2020 2020 2061 6c69               ali
-00009b40: 6173 203d 2066 227b 616c 6961 737d 2d7b  as = f"{alias}-{
-00009b50: 616c 6961 735f 7365 7175 656e 6365 3a30  alias_sequence:0
-00009b60: 337d 220a 2020 2020 2020 2020 2020 2020  3}".            
-00009b70: 2020 2020 2020 2020 6375 722e 6578 6563          cur.exec
-00009b80: 7574 6528 0a20 2020 2020 2020 2020 2020  ute(.           
-00009b90: 2020 2020 2020 2020 2020 2020 2022 5345               "SE
-00009ba0: 4c45 4354 2043 4f55 4e54 282a 292c 2061  LECT COUNT(*), a
-00009bb0: 6c69 6173 5f6f 6620 4652 4f4d 205f 7461  lias_of FROM _ta
-00009bc0: 626c 655f 6d65 7461 6461 7461 2077 6865  ble_metadata whe
-00009bd0: 7265 206e 616d 6520 6c69 6b65 2025 7320  re name like %s 
-00009be0: 6772 6f75 7020 6279 2061 6c69 6173 5f6f  group by alias_o
-00009bf0: 663b 222c 0a20 2020 2020 2020 2020 2020  f;",.           
-00009c00: 2020 2020 2020 2020 2020 2020 2028 616c               (al
-00009c10: 6961 7320 2b20 2225 222c 292c 0a20 2020  ias + "%",),.   
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00009c40: 2020 2020 2020 2061 6c69 6173 5f65 7869         alias_exi
-00009c50: 7374 7320 3d20 6375 722e 6665 7463 686f  sts = cur.fetcho
-00009c60: 6e65 2829 5b30 5d0a 2020 2020 2020 2020  ne()[0].        
-00009c70: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00009c80: 6f74 2061 6c69 6173 5f65 7869 7374 733a  ot alias_exists:
-00009c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009ca0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cc0: 2020 2061 6c69 6173 5f73 6571 7565 6e63     alias_sequenc
-00009cd0: 6520 2b3d 2031 0a20 2020 2020 2020 2020  e += 1.         
-00009ce0: 2020 2065 6c69 6620 616c 6961 735f 636f     elif alias_co
-00009cf0: 756e 7420 3d3d 2031 3a0a 2020 2020 2020  unt == 1:.      
-00009d00: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00009d10: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
-00009d20: 2020 2020 2020 2020 2020 2020 2020 2744                'D
-00009d30: 726f 7070 696e 6720 6578 6973 7469 6e67  ropping existing
-00009d40: 2061 6c69 6173 2022 7b7d 2220 666f 7220   alias "{}" for 
-00009d50: 7265 736f 7572 6365 2022 7b7d 222e 2e2e  resource "{}"...
-00009d60: 272e 666f 726d 6174 280a 2020 2020 2020  '.format(.      
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 616c 6961 732c 2065 7869 7374 696e    alias, existin
-00009d90: 675f 616c 6961 735f 6f66 0a20 2020 2020  g_alias_of.     
-00009da0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00009db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009dc0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00009dd0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00009de0: 2020 2020 2020 2020 2020 2020 6375 722e              cur.
-00009df0: 6578 6563 7574 6528 0a20 2020 2020 2020  execute(.       
-00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e10: 2073 716c 2e53 514c 2822 4452 4f50 2056   sql.SQL("DROP V
-00009e20: 4945 5720 4946 2045 5849 5354 5320 7b7d  IEW IF EXISTS {}
-00009e30: 2229 2e66 6f72 6d61 7428 7371 6c2e 4964  ").format(sql.Id
-00009e40: 656e 7469 6669 6572 2861 6c69 6173 2929  entifier(alias))
-00009e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e60: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00009e70: 2020 2020 2020 2065 7863 6570 7420 7073         except ps
-00009e80: 7963 6f70 6732 2e45 7272 6f72 2061 7320  ycopg2.Error as 
-00009e90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00009ea0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-00009eb0: 726e 696e 6728 2243 6f75 6c64 206e 6f74  rning("Could not
-00009ec0: 2064 726f 7020 616c 6961 732f 7669 6577   drop alias/view
-00009ed0: 3a20 7b7d 222e 666f 726d 6174 2865 2929  : {}".format(e))
-00009ee0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00009ef0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00009f00: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
-00009f10: 2020 2020 2020 2020 2020 2022 4361 6e6e             "Cann
-00009f20: 6f74 2063 7265 6174 6520 616c 6961 733a  ot create alias:
-00009f30: 207b 7d2d 7b7d 2d7b 7d22 2e66 6f72 6d61   {}-{}-{}".forma
-00009f40: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00009f50: 2020 2020 2020 2072 6573 6f75 7263 655f         resource_
-00009f60: 6e61 6d65 2c20 7061 636b 6167 655f 6e61  name, package_na
-00009f70: 6d65 2c20 6f77 6e65 725f 6f72 670a 2020  me, owner_org.  
-00009f80: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00009f90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00009fa0: 2020 2020 2020 2020 2020 616c 6961 7320            alias 
-00009fb0: 3d20 4e6f 6e65 0a0a 2020 2020 2320 7465  = None..    # te
-00009fc0: 6c6c 2043 4b41 4e20 746f 2063 616c 6375  ll CKAN to calcu
-00009fd0: 6c61 7465 5f72 6563 6f72 645f 636f 756e  late_record_coun
-00009fe0: 7420 616e 6420 7365 7420 616c 6961 7320  t and set alias 
-00009ff0: 6966 2073 6574 0a20 2020 2073 656e 645f  if set.    send_
-0000a000: 7265 736f 7572 6365 5f74 6f5f 6461 7461  resource_to_data
-0000a010: 7374 6f72 6528 0a20 2020 2020 2020 2072  store(.        r
-0000a020: 6573 6f75 7263 653d 4e6f 6e65 2c0a 2020  esource=None,.  
-0000a030: 2020 2020 2020 7265 736f 7572 6365 5f69        resource_i
-0000a040: 643d 7265 736f 7572 6365 5b22 6964 225d  d=resource["id"]
-0000a050: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
-0000a060: 733d 6865 6164 6572 735f 6469 6374 732c  s=headers_dicts,
-0000a070: 0a20 2020 2020 2020 2061 7069 5f6b 6579  .        api_key
-0000a080: 3d61 7069 5f6b 6579 2c0a 2020 2020 2020  =api_key,.      
-0000a090: 2020 636b 616e 5f75 726c 3d63 6b61 6e5f    ckan_url=ckan_
-0000a0a0: 7572 6c2c 0a20 2020 2020 2020 2072 6563  url,.        rec
-0000a0b0: 6f72 6473 3d4e 6f6e 652c 0a20 2020 2020  ords=None,.     
-0000a0c0: 2020 2061 6c69 6173 6573 3d61 6c69 6173     aliases=alias
-0000a0d0: 2c0a 2020 2020 2020 2020 6361 6c63 756c  ,.        calcul
-0000a0e0: 6174 655f 7265 636f 7264 5f63 6f75 6e74  ate_record_count
-0000a0f0: 3d54 7275 652c 0a20 2020 2029 0a0a 2020  =True,.    )..  
-0000a100: 2020 6966 2061 6c69 6173 3a0a 2020 2020    if alias:.    
-0000a110: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-0000a120: 2743 7265 6174 6564 2061 6c69 6173 2022  'Created alias "
-0000a130: 7b7d 2220 666f 7220 227b 7d22 2e2e 2e27  {}" for "{}"...'
-0000a140: 2e66 6f72 6d61 7428 616c 6961 732c 2072  .format(alias, r
-0000a150: 6573 6f75 7263 655f 6964 2929 0a0a 2020  esource_id))..  
-0000a160: 2020 6375 722e 636c 6f73 6528 290a 2020    cur.close().  
-0000a170: 2020 7261 775f 636f 6e6e 6563 7469 6f6e    raw_connection
-0000a180: 2e63 6f6d 6d69 7428 290a 0a20 2020 2023  .commit()..    #
-0000a190: 2020 7368 6f75 6c64 2077 6520 4144 445f    should we ADD_
-0000a1a0: 5355 4d4d 4152 595f 5354 4154 535f 5245  SUMMARY_STATS_RE
-0000a1b0: 534f 5552 4345 3f0a 2020 2020 6966 2063  SOURCE?.    if c
-0000a1c0: 6f6e 6669 672e 6765 7428 2241 4444 5f53  onfig.get("ADD_S
-0000a1d0: 554d 4d41 5259 5f53 5441 5453 5f52 4553  UMMARY_STATS_RES
-0000a1e0: 4f55 5243 4522 293a 0a0a 2020 2020 2020  OURCE"):..      
-0000a1f0: 2020 2320 6368 6563 6b20 6966 2074 6865    # check if the
-0000a200: 2073 7461 7473 2061 6c72 6561 6479 2065   stats already e
-0000a210: 7869 7374 0a20 2020 2020 2020 2069 6620  xist.        if 
-0000a220: 6175 746f 5f61 6c69 6173 3a0a 2020 2020  auto_alias:.    
-0000a230: 2020 2020 2020 2020 7374 6174 735f 7265          stats_re
-0000a240: 736f 7572 6365 5f69 6420 3d20 616c 6961  source_id = alia
-0000a250: 7320 2b20 222d 7374 6174 7322 0a20 2020  s + "-stats".   
-0000a260: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a270: 2020 2020 2020 2073 7461 7473 5f72 6573         stats_res
-0000a280: 6f75 7263 655f 6964 203d 2072 6573 6f75  ource_id = resou
-0000a290: 7263 655f 6964 202b 2022 2d73 7461 7473  rce_id + "-stats
-0000a2a0: 220a 2020 2020 2020 2020 6578 6973 7469  ".        existi
-0000a2b0: 6e67 5f73 7461 7473 203d 2064 6174 6173  ng_stats = datas
-0000a2c0: 746f 7265 5f72 6573 6f75 7263 655f 6578  tore_resource_ex
-0000a2d0: 6973 7473 2873 7461 7473 5f72 6573 6f75  ists(stats_resou
-0000a2e0: 7263 655f 6964 2c20 6170 695f 6b65 792c  rce_id, api_key,
-0000a2f0: 2063 6b61 6e5f 7572 6c29 0a0a 2020 2020   ckan_url)..    
-0000a300: 2020 2020 7374 6174 735f 6375 7220 3d20      stats_cur = 
-0000a310: 7261 775f 636f 6e6e 6563 7469 6f6e 2e63  raw_connection.c
-0000a320: 7572 736f 7228 290a 0a20 2020 2020 2020  ursor()..       
-0000a330: 2023 2044 656c 6574 6520 6578 6973 7469   # Delete existi
-0000a340: 6e67 2064 6174 6173 746f 7265 2072 6573  ng datastore res
-0000a350: 6f75 7263 652d 7374 6174 7320 6265 666f  ource-stats befo
-0000a360: 7265 2070 726f 6365 6564 696e 672e 0a20  re proceeding.. 
-0000a370: 2020 2020 2020 2069 6620 6578 6973 7469         if existi
-0000a380: 6e67 5f73 7461 7473 3a0a 2020 2020 2020  ng_stats:.      
-0000a390: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-0000a3a0: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
-0000a3b0: 2020 2027 4465 6c65 7469 6e67 2065 7869     'Deleting exi
-0000a3c0: 7374 696e 6720 7375 6d6d 6172 7920 7374  sting summary st
-0000a3d0: 6174 7320 227b 7265 735f 6964 7d22 2e27  ats "{res_id}".'
-0000a3e0: 2e66 6f72 6d61 7428 0a20 2020 2020 2020  .format(.       
-0000a3f0: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000a400: 5f69 643d 7374 6174 735f 7265 736f 7572  _id=stats_resour
-0000a410: 6365 5f69 640a 2020 2020 2020 2020 2020  ce_id.          
-0000a420: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000a430: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000a440: 2020 2073 7461 7473 5f63 7572 2e65 7865     stats_cur.exe
-0000a450: 6375 7465 280a 2020 2020 2020 2020 2020  cute(.          
-0000a460: 2020 2020 2020 2253 454c 4543 5420 616c        "SELECT al
-0000a470: 6961 735f 6f66 2046 524f 4d20 5f74 6162  ias_of FROM _tab
-0000a480: 6c65 5f6d 6574 6164 6174 6120 7768 6572  le_metadata wher
-0000a490: 6520 6e61 6d65 206c 696b 6520 2573 2067  e name like %s g
-0000a4a0: 726f 7570 2062 7920 616c 6961 735f 6f66  roup by alias_of
-0000a4b0: 3b22 2c0a 2020 2020 2020 2020 2020 2020  ;",.            
-0000a4c0: 2020 2020 2873 7461 7473 5f72 6573 6f75      (stats_resou
-0000a4d0: 7263 655f 6964 202b 2022 2522 2c29 2c0a  rce_id + "%",),.
-0000a4e0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000a4f0: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
-0000a500: 616c 6961 735f 7265 7375 6c74 203d 2073  alias_result = s
-0000a510: 7461 7473 5f63 7572 2e66 6574 6368 6f6e  tats_cur.fetchon
-0000a520: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
-0000a530: 6966 2073 7461 7473 5f61 6c69 6173 5f72  if stats_alias_r
-0000a540: 6573 756c 743a 0a20 2020 2020 2020 2020  esult:.         
-0000a550: 2020 2020 2020 2065 7869 7374 696e 675f         existing_
-0000a560: 7374 6174 735f 616c 6961 735f 6f66 203d  stats_alias_of =
-0000a570: 2073 7461 7473 5f61 6c69 6173 5f72 6573   stats_alias_res
-0000a580: 756c 745b 305d 0a0a 2020 2020 2020 2020  ult[0]..        
-0000a590: 2020 2020 2020 2020 6465 6c65 7465 5f64          delete_d
-0000a5a0: 6174 6173 746f 7265 5f72 6573 6f75 7263  atastore_resourc
-0000a5b0: 6528 6578 6973 7469 6e67 5f73 7461 7473  e(existing_stats
-0000a5c0: 5f61 6c69 6173 5f6f 662c 2061 7069 5f6b  _alias_of, api_k
-0000a5d0: 6579 2c20 636b 616e 5f75 726c 290a 2020  ey, ckan_url).  
-0000a5e0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-0000a5f0: 6c65 7465 5f72 6573 6f75 7263 6528 6578  lete_resource(ex
-0000a600: 6973 7469 6e67 5f73 7461 7473 5f61 6c69  isting_stats_ali
-0000a610: 6173 5f6f 662c 2061 7069 5f6b 6579 2c20  as_of, api_key, 
-0000a620: 636b 616e 5f75 726c 290a 0a20 2020 2020  ckan_url)..     
-0000a630: 2020 2073 7461 7473 5f61 6c69 6173 203d     stats_alias =
-0000a640: 204e 6f6e 650a 2020 2020 2020 2020 7374   None.        st
-0000a650: 6174 735f 616c 6961 735f 6e61 6d65 203d  ats_alias_name =
-0000a660: 2061 6c69 6173 202b 2022 2d73 7461 7473   alias + "-stats
-0000a670: 220a 2020 2020 2020 2020 6966 2061 7574  ".        if aut
-0000a680: 6f5f 616c 6961 733a 0a20 2020 2020 2020  o_alias:.       
-0000a690: 2020 2020 2073 7461 7473 5f61 6c69 6173       stats_alias
-0000a6a0: 203d 205b 7374 6174 735f 616c 6961 735f   = [stats_alias_
-0000a6b0: 6e61 6d65 5d0a 2020 2020 2020 2020 2020  name].          
-0000a6c0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000a6d0: 2020 2020 2020 2073 7461 7473 5f63 7572         stats_cur
-0000a6e0: 2e65 7865 6375 7465 280a 2020 2020 2020  .execute(.      
-0000a6f0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
-0000a700: 6c2e 5351 4c28 2244 524f 5020 5649 4557  l.SQL("DROP VIEW
-0000a710: 2049 4620 4558 4953 5453 207b 7d22 292e   IF EXISTS {}").
-0000a720: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
-0000a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a740: 7371 6c2e 4964 656e 7469 6669 6572 2873  sql.Identifier(s
-0000a750: 7461 7473 5f61 6c69 6173 5f6e 616d 6529  tats_alias_name)
-0000a760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a770: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000a780: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000a790: 2020 2020 2065 7863 6570 7420 7073 7963       except psyc
-0000a7a0: 6f70 6732 2e45 7272 6f72 2061 7320 653a  opg2.Error as e:
-0000a7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a7c0: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
-0000a7d0: 2243 6f75 6c64 206e 6f74 2064 726f 7020  "Could not drop 
-0000a7e0: 7374 6174 7320 616c 6961 732f 7669 6577  stats alias/view
-0000a7f0: 3a20 7b7d 222e 666f 726d 6174 2865 2929  : {}".format(e))
-0000a800: 0a0a 2020 2020 2020 2020 2320 7275 6e20  ..        # run 
-0000a810: 7374 6174 7320 6f6e 2073 7461 7473 2043  stats on stats C
-0000a820: 5356 2074 6f20 6765 7420 6865 6164 6572  SV to get header
-0000a830: 206e 616d 6573 2061 6e64 2069 6e66 6572   names and infer
-0000a840: 2064 6174 6120 7479 7065 730a 2020 2020   data types.    
-0000a850: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-0000a860: 2020 2020 2071 7376 5f73 7461 7473 5f73       qsv_stats_s
-0000a870: 7461 7473 203d 2073 7562 7072 6f63 6573  tats = subproces
-0000a880: 732e 7275 6e28 0a20 2020 2020 2020 2020  s.run(.         
-0000a890: 2020 2020 2020 205b 7173 765f 6269 6e2c         [qsv_bin,
-0000a8a0: 2022 7374 6174 7322 2c20 222d 2d74 7970   "stats", "--typ
-0000a8b0: 6573 6f6e 6c79 222c 2071 7376 5f73 7461  esonly", qsv_sta
-0000a8c0: 7473 5f63 7376 2e6e 616d 652c 5d2c 0a20  ts_csv.name,],. 
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000a8e0: 6170 7475 7265 5f6f 7574 7075 743d 5472  apture_output=Tr
-0000a8f0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-0000a900: 2020 2020 6368 6563 6b3d 5472 7565 2c0a      check=True,.
-0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a920: 7465 7874 3d54 7275 652c 0a20 2020 2020  text=True,.     
-0000a930: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000a940: 2065 7863 6570 7420 7375 6270 726f 6365   except subproce
-0000a950: 7373 2e43 616c 6c65 6450 726f 6365 7373  ss.CalledProcess
-0000a960: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-0000a970: 2020 2020 2020 2020 636c 6561 6e75 705f          cleanup_
-0000a980: 7465 6d70 6669 6c65 7328 290a 2020 2020  tempfiles().    
-0000a990: 2020 2020 2020 2020 7261 6973 6520 7574          raise ut
-0000a9a0: 696c 2e4a 6f62 4572 726f 7228 2243 616e  il.JobError("Can
-0000a9b0: 6e6f 7420 7275 6e20 7374 6174 7320 6f6e  not run stats on
-0000a9c0: 2043 5356 2073 7461 7473 3a20 7b7d 222e   CSV stats: {}".
-0000a9d0: 666f 726d 6174 2865 2929 0a0a 2020 2020  format(e))..    
-0000a9e0: 2020 2020 7374 6174 735f 7374 6174 7320      stats_stats 
-0000a9f0: 3d20 7374 7228 7173 765f 7374 6174 735f  = str(qsv_stats_
-0000aa00: 7374 6174 732e 7374 646f 7574 292e 7374  stats.stdout).st
-0000aa10: 7269 7028 290a 2020 2020 2020 2020 7374  rip().        st
-0000aa20: 6174 735f 7374 6174 735f 6469 6374 203d  ats_stats_dict =
-0000aa30: 205b 0a20 2020 2020 2020 2020 2020 2064   [.            d
-0000aa40: 6963 7428 6964 3d65 6c65 2e73 706c 6974  ict(id=ele.split
-0000aa50: 2822 2c22 295b 305d 2c20 7479 7065 3d74  (",")[0], type=t
-0000aa60: 7970 655f 6d61 7070 696e 675b 656c 652e  ype_mapping[ele.
-0000aa70: 7370 6c69 7428 222c 2229 5b31 5d5d 290a  split(",")[1]]).
-0000aa80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000aa90: 6964 782c 2065 6c65 2069 6e20 656e 756d  idx, ele in enum
-0000aaa0: 6572 6174 6528 7374 6174 735f 7374 6174  erate(stats_stat
-0000aab0: 732e 7370 6c69 746c 696e 6573 2829 5b31  s.splitlines()[1
-0000aac0: 3a5d 2c20 3129 0a20 2020 2020 2020 205d  :], 1).        ]
-0000aad0: 0a0a 2020 2020 2020 2020 2320 6c6f 6767  ..        # logg
-0000aae0: 6572 2e69 6e66 6f28 2244 4542 5547 3a20  er.info("DEBUG: 
-0000aaf0: 7374 6174 735f 7374 6174 735f 6469 6374  stats_stats_dict
-0000ab00: 3a20 7b7d 222e 666f 726d 6174 2873 7461  : {}".format(sta
-0000ab10: 7473 5f73 7461 7473 5f64 6963 7429 290a  ts_stats_dict)).
-0000ab20: 0a20 2020 2020 2020 2073 7461 7473 5f72  .        stats_r
-0000ab30: 6573 6f75 7263 6520 3d20 7b0a 2020 2020  esource = {.    
-0000ab40: 2020 2020 2020 2020 2270 6163 6b61 6765          "package
-0000ab50: 5f69 6422 3a20 7265 736f 7572 6365 5b22  _id": resource["
-0000ab60: 7061 636b 6167 655f 6964 225d 2c0a 2020  package_id"],.  
-0000ab70: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-0000ab80: 3a20 7265 736f 7572 6365 5f6e 616d 6520  : resource_name 
-0000ab90: 2b20 2220 2d20 5375 6d6d 6172 7920 5374  + " - Summary St
-0000aba0: 6174 6973 7469 6373 222c 0a20 2020 2020  atistics",.     
-0000abb0: 2020 2020 2020 2022 666f 726d 6174 223a         "format":
-0000abc0: 2022 4353 5622 2c0a 2020 2020 2020 2020   "CSV",.        
-0000abd0: 2020 2020 226d 696d 6574 7970 6522 3a20      "mimetype": 
-0000abe0: 2274 6578 742f 6373 7622 2c0a 2020 2020  "text/csv",.    
-0000abf0: 2020 2020 7d0a 2020 2020 2020 2020 7374      }.        st
-0000ac00: 6174 735f 7265 7370 6f6e 7365 203d 2073  ats_response = s
-0000ac10: 656e 645f 7265 736f 7572 6365 5f74 6f5f  end_resource_to_
-0000ac20: 6461 7461 7374 6f72 6528 0a20 2020 2020  datastore(.     
-0000ac30: 2020 2020 2020 2073 7461 7473 5f72 6573         stats_res
-0000ac40: 6f75 7263 652c 0a20 2020 2020 2020 2020  ource,.         
-0000ac50: 2020 2072 6573 6f75 7263 655f 6964 3d4e     resource_id=N
-0000ac60: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000ac70: 2068 6561 6465 7273 3d73 7461 7473 5f73   headers=stats_s
-0000ac80: 7461 7473 5f64 6963 742c 0a20 2020 2020  tats_dict,.     
-0000ac90: 2020 2020 2020 2061 7069 5f6b 6579 3d61         api_key=a
-0000aca0: 7069 5f6b 6579 2c0a 2020 2020 2020 2020  pi_key,.        
-0000acb0: 2020 2020 636b 616e 5f75 726c 3d63 6b61      ckan_url=cka
-0000acc0: 6e5f 7572 6c2c 0a20 2020 2020 2020 2020  n_url,.         
-0000acd0: 2020 2072 6563 6f72 6473 3d4e 6f6e 652c     records=None,
-0000ace0: 0a20 2020 2020 2020 2020 2020 2061 6c69  .            ali
-0000acf0: 6173 6573 3d73 7461 7473 5f61 6c69 6173  ases=stats_alias
-0000ad00: 2c0a 2020 2020 2020 2020 2020 2020 6361  ,.            ca
-0000ad10: 6c63 756c 6174 655f 7265 636f 7264 5f63  lculate_record_c
-0000ad20: 6f75 6e74 3d46 616c 7365 2c0a 2020 2020  ount=False,.    
-0000ad30: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
-0000ad40: 7461 7473 5f72 6573 6f75 7263 655f 6964  tats_resource_id
-0000ad50: 203d 2073 7461 7473 5f72 6573 706f 6e73   = stats_respons
-0000ad60: 655b 2272 6573 756c 7422 5d5b 2272 6573  e["result"]["res
-0000ad70: 6f75 7263 655f 6964 225d 0a0a 2020 2020  ource_id"]..    
-0000ad80: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-0000ad90: 0a20 2020 2020 2020 2020 2020 2027 4144  .            'AD
-0000ada0: 4449 4e47 2053 554d 4d41 5259 2053 5441  DING SUMMARY STA
-0000adb0: 5449 5354 4943 5320 227b 7d22 2066 6f72  TISTICS "{}" for
-0000adc0: 2022 7b7d 222e 2e2e 272e 666f 726d 6174   "{}"...'.format
-0000add0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ade0: 2020 7374 6174 735f 616c 6961 735f 6e61    stats_alias_na
-0000adf0: 6d65 2c20 7374 6174 735f 7265 736f 7572  me, stats_resour
-0000ae00: 6365 5f69 640a 2020 2020 2020 2020 2020  ce_id.          
-0000ae10: 2020 290a 2020 2020 2020 2020 290a 0a20    ).        ).. 
-0000ae20: 2020 2020 2020 2023 206e 6f77 2043 4f50         # now COP
-0000ae30: 5920 7468 6520 7374 6174 7320 746f 2074  Y the stats to t
-0000ae40: 6865 2064 6174 6173 746f 7265 0a20 2020  he datastore.   
-0000ae50: 2020 2020 2063 6f70 795f 7371 6c20 3d20       copy_sql = 
-0000ae60: 280a 2020 2020 2020 2020 2020 2020 2743  (.            'C
-0000ae70: 4f50 5920 227b 7265 736f 7572 6365 5f69  OPY "{resource_i
-0000ae80: 647d 2220 287b 636f 6c75 6d6e 5f6e 616d  d}" ({column_nam
-0000ae90: 6573 7d29 2046 524f 4d20 5354 4449 4e20  es}) FROM STDIN 
-0000aea0: 270a 2020 2020 2020 2020 2020 2020 2257  '.            "W
-0000aeb0: 4954 4820 2846 4f52 4d41 5420 4353 562c  ITH (FORMAT CSV,
-0000aec0: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
-0000aed0: 4845 4144 4552 2031 2c20 454e 434f 4449  HEADER 1, ENCODI
-0000aee0: 4e47 2027 5554 4638 2729 3b22 0a20 2020  NG 'UTF8');".   
-0000aef0: 2020 2020 2029 2e66 6f72 6d61 7428 0a20       ).format(. 
-0000af00: 2020 2020 2020 2020 2020 2072 6573 6f75             resou
-0000af10: 7263 655f 6964 3d73 7461 7473 5f72 6573  rce_id=stats_res
-0000af20: 6f75 7263 655f 6964 2c0a 2020 2020 2020  ource_id,.      
-0000af30: 2020 2020 2020 636f 6c75 6d6e 5f6e 616d        column_nam
-0000af40: 6573 3d22 2c20 222e 6a6f 696e 285b 2722  es=", ".join(['"
-0000af50: 7b7d 2227 2e66 6f72 6d61 7428 685b 2269  {}"'.format(h["i
-0000af60: 6422 5d29 2066 6f72 2068 2069 6e20 7374  d"]) for h in st
-0000af70: 6174 735f 7374 6174 735f 6469 6374 5d29  ats_stats_dict])
-0000af80: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-0000af90: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-0000afa0: 2863 6f70 795f 7371 6c29 0a20 2020 2020  (copy_sql).     
-0000afb0: 2020 2077 6974 6820 6f70 656e 2871 7376     with open(qsv
-0000afc0: 5f73 7461 7473 5f63 7376 2e6e 616d 652c  _stats_csv.name,
-0000afd0: 2022 7262 2229 2061 7320 663a 0a20 2020   "rb") as f:.   
-0000afe0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-0000aff0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-0000b000: 6174 735f 6375 722e 636f 7079 5f65 7870  ats_cur.copy_exp
-0000b010: 6572 7428 636f 7079 5f73 716c 2c20 6629  ert(copy_sql, f)
-0000b020: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-0000b030: 6570 7420 7073 7963 6f70 6732 2e45 7272  ept psycopg2.Err
-0000b040: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-0000b050: 2020 2020 2020 2020 2063 6c65 616e 7570           cleanup
-0000b060: 5f74 656d 7066 696c 6573 2829 0a20 2020  _tempfiles().   
-0000b070: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-0000b080: 7365 2075 7469 6c2e 4a6f 6245 7272 6f72  se util.JobError
-0000b090: 2822 506f 7374 6772 6573 2043 4f50 5920  ("Postgres COPY 
-0000b0a0: 6661 696c 6564 3a20 7b7d 222e 666f 726d  failed: {}".form
-0000b0b0: 6174 2865 2929 0a0a 2020 2020 2020 2020  at(e))..        
-0000b0c0: 7374 6174 735f 6375 722e 636c 6f73 6528  stats_cur.close(
-0000b0d0: 290a 2020 2020 2020 2020 7261 775f 636f  ).        raw_co
-0000b0e0: 6e6e 6563 7469 6f6e 2e63 6f6d 6d69 7428  nnection.commit(
-0000b0f0: 290a 0a20 2020 2020 2020 2073 7461 7473  )..        stats
-0000b100: 5f72 6573 6f75 7263 655b 2269 6422 5d20  _resource["id"] 
-0000b110: 3d20 7374 6174 735f 7265 736f 7572 6365  = stats_resource
-0000b120: 5f69 640a 2020 2020 2020 2020 7374 6174  _id.        stat
-0000b130: 735f 7265 736f 7572 6365 5b22 7375 6d6d  s_resource["summ
-0000b140: 6172 795f 7374 6174 6973 7469 6373 225d  ary_statistics"]
-0000b150: 203d 2054 7275 650a 2020 2020 2020 2020   = True.        
-0000b160: 7374 6174 735f 7265 736f 7572 6365 5b22  stats_resource["
-0000b170: 7375 6d6d 6172 795f 6f66 5f72 6573 6f75  summary_of_resou
-0000b180: 7263 6522 5d20 3d20 7265 736f 7572 6365  rce"] = resource
-0000b190: 5f69 640a 2020 2020 2020 2020 7570 6461  _id.        upda
-0000b1a0: 7465 5f72 6573 6f75 7263 6528 7374 6174  te_resource(stat
-0000b1b0: 735f 7265 736f 7572 6365 2c20 6170 695f  s_resource, api_
-0000b1c0: 6b65 792c 2063 6b61 6e5f 7572 6c29 0a0a  key, ckan_url)..
-0000b1d0: 2020 2020 7261 775f 636f 6e6e 6563 7469      raw_connecti
-0000b1e0: 6f6e 2e63 6c6f 7365 2829 0a0a 2020 2020  on.close()..    
-0000b1f0: 2320 6966 2041 5554 4f5f 494e 4445 585f  # if AUTO_INDEX_
-0000b200: 5448 5245 5348 4f4c 4420 3e20 3020 6f72  THRESHOLD > 0 or
-0000b210: 2041 5554 4f5f 494e 4445 585f 4441 5445   AUTO_INDEX_DATE
-0000b220: 5320 6973 2074 7275 650a 2020 2020 2320  S is true.    # 
-0000b230: 6372 6561 7465 2069 6e64 6963 6573 2061  create indices a
-0000b240: 7574 6f6d 6174 6963 616c 6c79 2062 6173  utomatically bas
-0000b250: 6564 206f 6e20 7375 6d6d 6172 7920 7374  ed on summary st
-0000b260: 6174 6973 7469 6373 0a20 2020 2023 2046  atistics.    # F
-0000b270: 6f72 2063 6f6c 756d 6e73 2077 2f20 6361  or columns w/ ca
-0000b280: 7264 696e 616c 6974 7920 3d20 7265 636f  rdinality = reco
-0000b290: 7264 5f63 6f75 6e74 2c20 6974 2773 2061  rd_count, it's a
-0000b2a0: 6c6c 2075 6e69 7175 6520 7661 6c75 6573  ll unique values
-0000b2b0: 2c20 6372 6561 7465 2061 2075 6e69 7175  , create a uniqu
-0000b2c0: 6520 696e 6465 780a 2020 2020 2320 4966  e index.    # If
-0000b2d0: 2041 5554 4f5f 494e 4445 585f 4441 5445   AUTO_INDEX_DATE
-0000b2e0: 5320 6973 2074 7275 652c 2069 6e64 6578  S is true, index
-0000b2f0: 2061 6c6c 2064 6174 6520 636f 6c75 6d6e   all date column
-0000b300: 730a 2020 2020 2320 6966 2061 2063 6f6c  s.    # if a col
-0000b310: 756d 6e27 7320 6361 7264 696e 616c 6974  umn's cardinalit
-0000b320: 7920 3c3d 2041 5554 4f5f 494e 4445 585f  y <= AUTO_INDEX_
-0000b330: 5448 5245 5348 4f4c 442c 2063 7265 6174  THRESHOLD, creat
-0000b340: 6520 616e 2069 6e64 6578 2066 6f72 2074  e an index for t
-0000b350: 6861 7420 636f 6c75 6d6e 0a20 2020 2061  hat column.    a
-0000b360: 7574 6f5f 696e 6465 785f 6461 7465 7320  uto_index_dates 
-0000b370: 3d20 636f 6e66 6967 2e67 6574 2822 4155  = config.get("AU
-0000b380: 544f 5f49 4e44 4558 5f44 4154 4553 2229  TO_INDEX_DATES")
-0000b390: 0a20 2020 2069 6620 6175 746f 5f69 6e64  .    if auto_ind
-0000b3a0: 6578 5f74 6872 6573 686f 6c64 206f 7220  ex_threshold or 
-0000b3b0: 2861 7574 6f5f 696e 6465 785f 6461 7465  (auto_index_date
-0000b3c0: 7320 616e 6420 6461 7465 7469 6d65 636f  s and datetimeco
-0000b3d0: 6c73 5f6c 6973 7429 3a0a 2020 2020 2020  ls_list):.      
-0000b3e0: 2020 696e 6465 785f 7374 6172 7420 3d20    index_start = 
-0000b3f0: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
-0000b400: 7228 290a 2020 2020 2020 2020 6c6f 6767  r().        logg
-0000b410: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
-0000b420: 2020 2020 2022 4155 544f 2d49 4e44 4558       "AUTO-INDEX
-0000b430: 494e 472e 2041 7574 6f2d 696e 6465 7820  ING. Auto-index 
-0000b440: 7468 7265 7368 6f6c 643a 207b 3a2c 7d20  threshold: {:,} 
-0000b450: 756e 6971 7565 2076 616c 7565 2f73 2e20  unique value/s. 
-0000b460: 4175 746f 2d69 6e64 6578 2064 6174 6573  Auto-index dates
-0000b470: 3a20 7b7d 202e 2e2e 222e 666f 726d 6174  : {} ...".format
-0000b480: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000b490: 2020 6175 746f 5f69 6e64 6578 5f74 6872    auto_index_thr
-0000b4a0: 6573 686f 6c64 2c20 6175 746f 5f69 6e64  eshold, auto_ind
-0000b4b0: 6578 5f64 6174 6573 0a20 2020 2020 2020  ex_dates.       
-0000b4c0: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
-0000b4d0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-0000b4e0: 2020 2020 2020 2020 2020 7261 775f 636f            raw_co
-0000b4f0: 6e6e 6563 7469 6f6e 203d 2070 7379 636f  nnection = psyco
-0000b500: 7067 322e 636f 6e6e 6563 7428 636f 6e66  pg2.connect(conf
-0000b510: 6967 2e67 6574 2822 5752 4954 455f 454e  ig.get("WRITE_EN
-0000b520: 4749 4e45 5f55 524c 2229 290a 2020 2020  GINE_URL")).    
-0000b530: 2020 2020 6578 6365 7074 2070 7379 636f      except psyco
-0000b540: 7067 322e 4572 726f 7220 6173 2065 3a0a  pg2.Error as e:.
-0000b550: 2020 2020 2020 2020 2020 2020 636c 6561              clea
-0000b560: 6e75 705f 7465 6d70 6669 6c65 7328 290a  nup_tempfiles().
-0000b570: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000b580: 6520 7574 696c 2e4a 6f62 4572 726f 7228  e util.JobError(
-0000b590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b5a0: 2022 436f 756c 6420 6e6f 7420 636f 6e6e   "Could not conn
-0000b5b0: 6563 7420 746f 2074 6865 2044 6174 6173  ect to the Datas
-0000b5c0: 746f 7265 2074 6f20 6372 6561 7465 2069  tore to create i
-0000b5d0: 6e64 6963 6573 3a20 7b7d 222e 666f 726d  ndices: {}".form
-0000b5e0: 6174 2865 290a 2020 2020 2020 2020 2020  at(e).          
-0000b5f0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
-0000b600: 3a0a 2020 2020 2020 2020 2020 2020 696e  :.            in
-0000b610: 6465 785f 6375 7220 3d20 7261 775f 636f  dex_cur = raw_co
-0000b620: 6e6e 6563 7469 6f6e 2e63 7572 736f 7228  nnection.cursor(
-0000b630: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-0000b640: 2069 6620 6175 746f 5f69 6e64 6578 5f74   if auto_index_t
-0000b650: 6872 6573 686f 6c64 203d 3d20 2d31 0a20  hreshold == -1. 
-0000b660: 2020 2020 2020 2020 2020 2023 2077 6520             # we 
-0000b670: 696e 6465 7820 616c 6c20 7468 6520 636f  index all the co
-0000b680: 6c75 6d6e 730a 2020 2020 2020 2020 2020  lumns.          
-0000b690: 2020 6966 2061 7574 6f5f 696e 6465 785f    if auto_index_
-0000b6a0: 7468 7265 7368 6f6c 6420 3d3d 202d 313a  threshold == -1:
-0000b6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b6c0: 2061 7574 6f5f 696e 6465 785f 7468 7265   auto_index_thre
-0000b6d0: 7368 6f6c 6420 3d20 7265 636f 7264 5f63  shold = record_c
-0000b6e0: 6f75 6e74 0a0a 2020 2020 2020 2020 2020  ount..          
-0000b6f0: 2020 696e 6465 785f 636f 756e 7420 3d20    index_count = 
-0000b700: 300a 2020 2020 2020 2020 2020 2020 666f  0.            fo
-0000b710: 7220 6964 782c 2063 6172 6469 6e61 6c69  r idx, cardinali
-0000b720: 7479 2069 6e20 656e 756d 6572 6174 6528  ty in enumerate(
-0000b730: 6865 6164 6572 735f 6361 7264 696e 616c  headers_cardinal
-0000b740: 6974 7929 3a0a 0a20 2020 2020 2020 2020  ity):..         
-0000b750: 2020 2020 2020 2063 7572 725f 636f 6c20         curr_col 
-0000b760: 3d20 6865 6164 6572 735b 6964 785d 0a20  = headers[idx]. 
-0000b770: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000b780: 6620 6175 746f 5f69 6e64 6578 5f74 6872  f auto_index_thr
-0000b790: 6573 686f 6c64 203e 2030 206f 7220 6175  eshold > 0 or au
-0000b7a0: 746f 5f69 6e64 6578 5f64 6174 6573 3a0a  to_index_dates:.
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7c0: 2020 2020 6966 2063 6172 6469 6e61 6c69      if cardinali
-0000b7d0: 7479 203d 3d20 7265 636f 7264 5f63 6f75  ty == record_cou
-0000b7e0: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
-0000b7f0: 2020 2020 2020 2020 2020 2020 2320 616c              # al
-0000b800: 6c20 7468 6520 7661 6c75 6573 2061 7265  l the values are
-0000b810: 2075 6e69 7175 6520 666f 7220 7468 6973   unique for this
-0000b820: 2063 6f6c 756d 6e2c 2063 7265 6174 6520   column, create 
-0000b830: 6120 756e 6971 7565 2069 6e64 6578 0a20  a unique index. 
-0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b850: 2020 2020 2020 2075 6e69 7175 655f 7661         unique_va
-0000b860: 6c75 655f 636f 756e 7420 3d20 6d69 6e28  lue_count = min(
-0000b870: 7072 6576 6965 775f 726f 7773 2c20 6361  preview_rows, ca
-0000b880: 7264 696e 616c 6974 7929 0a20 2020 2020  rdinality).     
-0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8a0: 2020 206c 6f67 6765 722e 696e 666f 280a     logger.info(.
-0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8c0: 2020 2020 2020 2020 2020 2020 2743 7265              'Cre
-0000b8d0: 6174 696e 6720 554e 4951 5545 2069 6e64  ating UNIQUE ind
-0000b8e0: 6578 206f 6e20 227b 7d22 2066 6f72 207b  ex on "{}" for {
-0000b8f0: 3a2c 7d20 756e 6971 7565 2076 616c 7565  :,} unique value
-0000b900: 732e 2e2e 272e 666f 726d 6174 280a 2020  s...'.format(.  
-0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b920: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-0000b930: 7272 5f63 6f6c 2c20 756e 6971 7565 5f76  rr_col, unique_v
-0000b940: 616c 7565 5f63 6f75 6e74 0a20 2020 2020  alue_count.     
-0000b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b960: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b980: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000b990: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9b0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-0000b9c0: 785f 6375 722e 6578 6563 7574 6528 0a20  x_cur.execute(. 
-0000b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000b9f0: 4352 4541 5445 2055 4e49 5155 4520 494e  CREATE UNIQUE IN
-0000ba00: 4445 5820 4f4e 2022 7b72 6573 6f75 7263  DEX ON "{resourc
-0000ba10: 655f 6964 7d22 2028 227b 636f 6c5f 6e61  e_id}" ("{col_na
-0000ba20: 6d65 7d22 293b 272e 666f 726d 6174 280a  me}");'.format(.
-0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba50: 2020 2020 7265 736f 7572 6365 5f69 643d      resource_id=
-0000ba60: 7265 736f 7572 6365 5f69 642c 2063 6f6c  resource_id, col
-0000ba70: 5f6e 616d 653d 6375 7272 5f63 6f6c 0a20  _name=curr_col. 
-0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba90: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000baa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bab0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bad0: 2020 2020 2020 2065 7863 6570 7420 7073         except ps
-0000bae0: 7963 6f70 6732 2e45 7272 6f72 2061 7320  ycopg2.Error as 
-0000baf0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000bb00: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000bb10: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
-0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000bb40: 436f 756c 6420 6e6f 7420 4352 4541 5445  Could not CREATE
-0000bb50: 2055 4e49 5155 4520 494e 4445 5820 6f6e   UNIQUE INDEX on
-0000bb60: 2022 7b7d 223a 207b 7d27 2e66 6f72 6d61   "{}": {}'.forma
-0000bb70: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb90: 2020 2020 2020 2063 7572 725f 636f 6c2c         curr_col,
-0000bba0: 2065 0a20 2020 2020 2020 2020 2020 2020   e.             
-0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbc0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bbe0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000bbf0: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-0000bc00: 5f63 6f75 6e74 202b 3d20 310a 2020 2020  _count += 1.    
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc20: 656c 6966 2063 6172 6469 6e61 6c69 7479  elif cardinality
-0000bc30: 203c 3d20 6175 746f 5f69 6e64 6578 5f74   <= auto_index_t
-0000bc40: 6872 6573 686f 6c64 206f 7220 280a 2020  hreshold or (.  
-0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc60: 2020 2020 2020 6175 746f 5f69 6e64 6578        auto_index
-0000bc70: 5f64 6174 6573 2061 6e64 2028 6375 7272  _dates and (curr
-0000bc80: 5f63 6f6c 2069 6e20 6461 7465 7469 6d65  _col in datetime
-0000bc90: 636f 6c73 5f6c 6973 7429 0a20 2020 2020  cols_list).     
-0000bca0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000bcb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bcc0: 2020 2020 2020 2020 2020 2320 6361 7264            # card
-0000bcd0: 696e 616c 6974 7920 3c3d 2061 7574 6f5f  inality <= auto_
-0000bce0: 696e 6465 785f 7468 7265 7368 6f6c 6420  index_threshold 
-0000bcf0: 6f72 2069 7473 2061 2064 6174 6520 616e  or its a date an
-0000bd00: 6420 6175 746f 5f69 6e64 6578 5f64 6174  d auto_index_dat
-0000bd10: 6520 6973 2074 7275 650a 2020 2020 2020  e is true.      
-0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2020 2320 6372 6561 7465 2061 6e20 696e    # create an in
-0000bd40: 6465 780a 2020 2020 2020 2020 2020 2020  dex.            
-0000bd50: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-0000bd60: 7572 725f 636f 6c20 696e 2064 6174 6574  urr_col in datet
-0000bd70: 696d 6563 6f6c 735f 6c69 7374 3a0a 2020  imecols_list:.  
-0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd90: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000bda0: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdc0: 2020 2020 2020 2027 4372 6561 7469 6e67         'Creating
-0000bdd0: 2069 6e64 6578 206f 6e20 227b 7d22 2064   index on "{}" d
-0000bde0: 6174 6520 636f 6c75 6d6e 2066 6f72 207b  ate column for {
-0000bdf0: 3a2c 7d20 756e 6971 7565 2076 616c 7565  :,} unique value
-0000be00: 2f73 2e2e 2e27 2e66 6f72 6d61 7428 0a20  /s...'.format(. 
-0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be30: 2020 2063 7572 725f 636f 6c2c 2063 6172     curr_col, car
-0000be40: 6469 6e61 6c69 7479 0a20 2020 2020 2020  dinality.       
-0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be60: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bea0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bec0: 2020 206c 6f67 6765 722e 696e 666f 280a     logger.info(.
-0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bef0: 2743 7265 6174 696e 6720 696e 6465 7820  'Creating index 
-0000bf00: 6f6e 2022 7b7d 2220 666f 7220 7b3a 2c7d  on "{}" for {:,}
-0000bf10: 2075 6e69 7175 6520 7661 6c75 652f 732e   unique value/s.
-0000bf20: 2e2e 272e 666f 726d 6174 280a 2020 2020  ..'.format(.    
-0000bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf50: 6375 7272 5f63 6f6c 2c20 6361 7264 696e  curr_col, cardin
-0000bf60: 616c 6974 790a 2020 2020 2020 2020 2020  ality.          
-0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf80: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000bf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfa0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000bfb0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-0000bfc0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000bfd0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000bfe0: 6e64 6578 5f63 7572 2e65 7865 6375 7465  ndex_cur.execute
-0000bff0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 2020 2743 5245 4154 4520 494e 4445 5820    'CREATE INDEX 
-0000c020: 4f4e 2022 7b72 6573 6f75 7263 655f 6964  ON "{resource_id
-0000c030: 7d22 2028 227b 636f 6c5f 6e61 6d65 7d22  }" ("{col_name}"
-0000c040: 293b 272e 666f 726d 6174 280a 2020 2020  );'.format(.    
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c070: 7265 736f 7572 6365 5f69 643d 7265 736f  resource_id=reso
-0000c080: 7572 6365 5f69 642c 2063 6f6c 5f6e 616d  urce_id, col_nam
-0000c090: 653d 6375 7272 5f63 6f6c 0a20 2020 2020  e=curr_col.     
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0f0: 2020 2065 7863 6570 7420 7073 7963 6f70     except psycop
-0000c100: 6732 2e45 7272 6f72 2061 7320 653a 0a20  g2.Error as e:. 
-0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c120: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000c130: 722e 7761 726e 696e 6728 0a20 2020 2020  r.warning(.     
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c150: 2020 2020 2020 2020 2020 2027 436f 756c             'Coul
-0000c160: 6420 6e6f 7420 4352 4541 5445 2049 4e44  d not CREATE IND
-0000c170: 4558 206f 6e20 227b 7d22 3a20 7b7d 272e  EX on "{}": {}'.
-0000c180: 666f 726d 6174 2863 7572 725f 636f 6c2c  format(curr_col,
-0000c190: 2065 290a 2020 2020 2020 2020 2020 2020   e).            
-0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c1c0: 2020 2020 2020 2020 2020 696e 6465 785f            index_
-0000c1d0: 636f 756e 7420 2b3d 2031 0a0a 2020 2020  count += 1..    
-0000c1e0: 2020 2020 2020 2020 696e 6465 785f 6375          index_cu
-0000c1f0: 722e 636c 6f73 6528 290a 2020 2020 2020  r.close().      
-0000c200: 2020 2020 2020 7261 775f 636f 6e6e 6563        raw_connec
-0000c210: 7469 6f6e 2e63 6f6d 6d69 7428 290a 0a20  tion.commit().. 
-0000c220: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000c230: 722e 696e 666f 2822 5661 6375 756d 2041  r.info("Vacuum A
-0000c240: 6e61 6c79 7a69 6e67 2074 6162 6c65 2074  nalyzing table t
-0000c250: 6f20 6f70 7469 6d69 7a65 2069 6e64 6963  o optimize indic
-0000c260: 6573 2e2e 2e22 290a 0a20 2020 2020 2020  es...")..       
-0000c270: 2020 2020 2023 2074 6869 7320 6973 206e       # this is n
-0000c280: 6565 6465 6420 746f 2069 7373 7565 2061  eeded to issue a
-0000c290: 2056 4143 5555 4d20 414e 414c 595a 450a   VACUUM ANALYZE.
-0000c2a0: 2020 2020 2020 2020 2020 2020 7261 775f              raw_
-0000c2b0: 636f 6e6e 6563 7469 6f6e 2e73 6574 5f69  connection.set_i
-0000c2c0: 736f 6c61 7469 6f6e 5f6c 6576 656c 280a  solation_level(.
-0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2e0: 7073 7963 6f70 6732 2e65 7874 656e 7369  psycopg2.extensi
-0000c2f0: 6f6e 732e 4953 4f4c 4154 494f 4e5f 4c45  ons.ISOLATION_LE
-0000c300: 5645 4c5f 4155 544f 434f 4d4d 4954 0a20  VEL_AUTOCOMMIT. 
-0000c310: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000c320: 2020 2020 2020 2020 2061 6e61 6c79 7a65           analyze
-0000c330: 5f63 7572 203d 2072 6177 5f63 6f6e 6e65  _cur = raw_conne
-0000c340: 6374 696f 6e2e 6375 7273 6f72 2829 0a20  ction.cursor(). 
-0000c350: 2020 2020 2020 2020 2020 2061 6e61 6c79             analy
-0000c360: 7a65 5f63 7572 2e65 7865 6375 7465 280a  ze_cur.execute(.
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 7371 6c2e 5351 4c28 2256 4143 5555 4d20  sql.SQL("VACUUM 
-0000c390: 414e 414c 595a 4520 7b7d 2229 2e66 6f72  ANALYZE {}").for
-0000c3a0: 6d61 7428 7371 6c2e 4964 656e 7469 6669  mat(sql.Identifi
-0000c3b0: 6572 2872 6573 6f75 7263 655f 6964 2929  er(resource_id))
-0000c3c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000c3d0: 2020 2020 2020 2020 2020 2061 6e61 6c79             analy
-0000c3e0: 7a65 5f63 7572 2e63 6c6f 7365 2829 0a0a  ze_cur.close()..
-0000c3f0: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-0000c400: 785f 656c 6170 7365 6420 3d20 7469 6d65  x_elapsed = time
-0000c410: 2e70 6572 665f 636f 756e 7465 7228 2920  .perf_counter() 
-0000c420: 2d20 696e 6465 785f 7374 6172 740a 2020  - index_start.  
-0000c430: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000c440: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
-0000c450: 2020 2020 2020 2027 2e2e 2e69 6e64 6578         '...index
-0000c460: 696e 672f 7661 6375 756d 2061 6e61 6c79  ing/vacuum analy
-0000c470: 7369 7320 646f 6e65 2e20 496e 6465 7865  sis done. Indexe
-0000c480: 6420 7b6e 7d20 636f 6c75 6d6e 7320 696e  d {n} columns in
-0000c490: 2022 7b72 6573 5f69 647d 2220 696e 207b   "{res_id}" in {
-0000c4a0: 696e 6465 785f 656c 6170 7365 647d 2073  index_elapsed} s
-0000c4b0: 6563 6f6e 6473 2e27 2e66 6f72 6d61 7428  econds.'.format(
-0000c4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c4d0: 2020 2020 206e 3d22 7b3a 2c7d 222e 666f       n="{:,}".fo
-0000c4e0: 726d 6174 2869 6e64 6578 5f63 6f75 6e74  rmat(index_count
-0000c4f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000c500: 2020 2020 2020 2072 6573 5f69 643d 7265         res_id=re
-0000c510: 736f 7572 6365 5f69 642c 0a20 2020 2020  source_id,.     
-0000c520: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000c530: 6e64 6578 5f65 6c61 7073 6564 3d22 7b3a  ndex_elapsed="{:
-0000c540: 2c2e 3266 7d22 2e66 6f72 6d61 7428 696e  ,.2f}".format(in
-0000c550: 6465 785f 656c 6170 7365 6429 2c0a 2020  dex_elapsed),.  
-0000c560: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000c570: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000c580: 2020 2020 2020 2072 6177 5f63 6f6e 6e65         raw_conne
-0000c590: 6374 696f 6e2e 636c 6f73 6528 290a 0a20  ction.close().. 
-0000c5a0: 2020 2063 6c65 616e 7570 5f74 656d 7066     cleanup_tempf
-0000c5b0: 696c 6573 2829 0a0a 2020 2020 746f 7461  iles()..    tota
-0000c5c0: 6c5f 656c 6170 7365 6420 3d20 7469 6d65  l_elapsed = time
-0000c5d0: 2e70 6572 665f 636f 756e 7465 7228 2920  .perf_counter() 
-0000c5e0: 2d20 7469 6d65 725f 7374 6172 740a 2020  - timer_start.  
-0000c5f0: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
-0000c600: 2020 2020 2020 2022 4441 5441 5055 5348         "DATAPUSH
-0000c610: 4552 2b20 4a4f 4220 444f 4e45 2120 546f  ER+ JOB DONE! To
-0000c620: 7461 6c20 656c 6170 7365 6420 7469 6d65  tal elapsed time
-0000c630: 3a20 7b3a 2c2e 3266 7d20 7365 636f 6e64  : {:,.2f} second
-0000c640: 732e 222e 666f 726d 6174 280a 2020 2020  s.".format(.    
-0000c650: 2020 2020 2020 2020 746f 7461 6c5f 656c          total_el
-0000c660: 6170 7365 640a 2020 2020 2020 2020 290a  apsed.        ).
-0000c670: 2020 2020 290a                               ).
+00001c30: 7475 726e 2072 6573 706f 6e73 652e 6a73  turn response.js
+00001c40: 6f6e 2829 2e67 6574 2822 7265 7375 6c74  on().get("result
+00001c50: 222c 207b 2266 6965 6c64 7322 3a20 5b5d  ", {"fields": []
+00001c60: 7d29 0a20 2020 2020 2020 2065 6c73 653a  }).        else:
+00001c70: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00001c80: 7365 2048 5454 5045 7272 6f72 280a 2020  se HTTPError(.  
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2245                "E
+00001ca0: 7272 6f72 2067 6574 7469 6e67 2064 6174  rror getting dat
+00001cb0: 6173 746f 7265 2072 6573 6f75 7263 652e  astore resource.
+00001cc0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00001cd0: 2020 2072 6573 706f 6e73 652e 7374 6174     response.stat
+00001ce0: 7573 5f63 6f64 652c 0a20 2020 2020 2020  us_code,.       
+00001cf0: 2020 2020 2020 2020 2073 6561 7263 685f           search_
+00001d00: 7572 6c2c 0a20 2020 2020 2020 2020 2020  url,.           
+00001d10: 2020 2020 2072 6573 706f 6e73 652c 0a20       response,. 
+00001d20: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00001d30: 2065 7863 6570 7420 7265 7175 6573 7473   except requests
+00001d40: 2e65 7863 6570 7469 6f6e 732e 5265 7175  .exceptions.Requ
+00001d50: 6573 7445 7863 6570 7469 6f6e 2061 7320  estException as 
+00001d60: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
+00001d70: 2075 7469 6c2e 4a6f 6245 7272 6f72 2822   util.JobError("
+00001d80: 4572 726f 7220 6765 7474 696e 6720 6461  Error getting da
+00001d90: 7461 7374 6f72 6520 7265 736f 7572 6365  tastore resource
+00001da0: 2028 7b21 737d 292e 222e 666f 726d 6174   ({!s}).".format
+00001db0: 2865 2929 0a0a 0a64 6566 2073 656e 645f  (e))...def send_
+00001dc0: 7265 736f 7572 6365 5f74 6f5f 6461 7461  resource_to_data
+00001dd0: 7374 6f72 6528 0a20 2020 2072 6573 6f75  store(.    resou
+00001de0: 7263 652c 0a20 2020 2072 6573 6f75 7263  rce,.    resourc
+00001df0: 655f 6964 2c0a 2020 2020 6865 6164 6572  e_id,.    header
+00001e00: 732c 0a20 2020 2061 7069 5f6b 6579 2c0a  s,.    api_key,.
+00001e10: 2020 2020 636b 616e 5f75 726c 2c0a 2020      ckan_url,.  
+00001e20: 2020 7265 636f 7264 732c 0a20 2020 2061    records,.    a
+00001e30: 6c69 6173 6573 2c0a 2020 2020 6361 6c63  liases,.    calc
+00001e40: 756c 6174 655f 7265 636f 7264 5f63 6f75  ulate_record_cou
+00001e50: 6e74 2c0a 293a 0a20 2020 2022 2222 0a20  nt,.):.    """. 
+00001e60: 2020 2053 746f 7265 7320 7265 636f 7264     Stores record
+00001e70: 7320 696e 2043 4b41 4e20 6461 7461 7374  s in CKAN datast
+00001e80: 6f72 650a 2020 2020 2222 220a 0a20 2020  ore.    """..   
+00001e90: 2069 6620 7265 736f 7572 6365 5f69 643a   if resource_id:
+00001ea0: 0a20 2020 2020 2020 2023 2075 7365 6420  .        # used 
+00001eb0: 746f 2063 7265 6174 6520 7468 6520 226d  to create the "m
+00001ec0: 6169 6e22 2072 6573 6f75 7263 650a 2020  ain" resource.  
+00001ed0: 2020 2020 2020 7265 7175 6573 7420 3d20        request = 
+00001ee0: 7b0a 2020 2020 2020 2020 2020 2020 2272  {.            "r
+00001ef0: 6573 6f75 7263 655f 6964 223a 2072 6573  esource_id": res
+00001f00: 6f75 7263 655f 6964 2c0a 2020 2020 2020  ource_id,.      
+00001f10: 2020 2020 2020 2266 6965 6c64 7322 3a20        "fields": 
+00001f20: 6865 6164 6572 732c 0a20 2020 2020 2020  headers,.       
+00001f30: 2020 2020 2022 666f 7263 6522 3a20 5472       "force": Tr
+00001f40: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00001f50: 2272 6563 6f72 6473 223a 2072 6563 6f72  "records": recor
+00001f60: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+00001f70: 2261 6c69 6173 6573 223a 2061 6c69 6173  "aliases": alias
+00001f80: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00001f90: 2263 616c 6375 6c61 7465 5f72 6563 6f72  "calculate_recor
+00001fa0: 645f 636f 756e 7422 3a20 6361 6c63 756c  d_count": calcul
+00001fb0: 6174 655f 7265 636f 7264 5f63 6f75 6e74  ate_record_count
+00001fc0: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
+00001fd0: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+00001fe0: 7573 6564 2074 6f20 6372 6561 7465 2074  used to create t
+00001ff0: 6865 2022 7374 6174 7322 2072 6573 6f75  he "stats" resou
+00002000: 7263 650a 2020 2020 2020 2020 7265 7175  rce.        requ
+00002010: 6573 7420 3d20 7b0a 2020 2020 2020 2020  est = {.        
+00002020: 2020 2020 2272 6573 6f75 7263 6522 3a20      "resource": 
+00002030: 7265 736f 7572 6365 2c0a 2020 2020 2020  resource,.      
+00002040: 2020 2020 2020 2266 6965 6c64 7322 3a20        "fields": 
+00002050: 6865 6164 6572 732c 0a20 2020 2020 2020  headers,.       
+00002060: 2020 2020 2022 666f 7263 6522 3a20 5472       "force": Tr
+00002070: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00002080: 2261 6c69 6173 6573 223a 2061 6c69 6173  "aliases": alias
+00002090: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+000020a0: 2263 616c 6375 6c61 7465 5f72 6563 6f72  "calculate_recor
+000020b0: 645f 636f 756e 7422 3a20 6361 6c63 756c  d_count": calcul
+000020c0: 6174 655f 7265 636f 7264 5f63 6f75 6e74  ate_record_count
+000020d0: 2c0a 2020 2020 2020 2020 7d0a 0a20 2020  ,.        }..   
+000020e0: 2075 726c 203d 2067 6574 5f75 726c 2822   url = get_url("
+000020f0: 6461 7461 7374 6f72 655f 6372 6561 7465  datastore_create
+00002100: 222c 2063 6b61 6e5f 7572 6c29 0a20 2020  ", ckan_url).   
+00002110: 2072 203d 2072 6571 7565 7374 732e 706f   r = requests.po
+00002120: 7374 280a 2020 2020 2020 2020 7572 6c2c  st(.        url,
+00002130: 0a20 2020 2020 2020 2076 6572 6966 793d  .        verify=
+00002140: 636f 6e66 6967 2e67 6574 2822 5353 4c5f  config.get("SSL_
+00002150: 5645 5249 4659 2229 2c0a 2020 2020 2020  VERIFY"),.      
+00002160: 2020 6461 7461 3d6a 736f 6e2e 6475 6d70    data=json.dump
+00002170: 7328 7265 7175 6573 742c 2063 6c73 3d44  s(request, cls=D
+00002180: 6174 6173 746f 7265 456e 636f 6465 7229  atastoreEncoder)
+00002190: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+000021a0: 733d 7b22 436f 6e74 656e 742d 5479 7065  s={"Content-Type
+000021b0: 223a 2022 6170 706c 6963 6174 696f 6e2f  ": "application/
+000021c0: 6a73 6f6e 222c 2022 4175 7468 6f72 697a  json", "Authoriz
+000021d0: 6174 696f 6e22 3a20 6170 695f 6b65 797d  ation": api_key}
+000021e0: 2c0a 2020 2020 290a 2020 2020 6368 6563  ,.    ).    chec
+000021f0: 6b5f 7265 7370 6f6e 7365 2872 2c20 7572  k_response(r, ur
+00002200: 6c2c 2022 434b 414e 2044 6174 6153 746f  l, "CKAN DataSto
+00002210: 7265 2229 0a20 2020 2072 6574 7572 6e20  re").    return 
+00002220: 722e 6a73 6f6e 2829 0a0a 0a64 6566 2075  r.json()...def u
+00002230: 7064 6174 655f 7265 736f 7572 6365 2872  pdate_resource(r
+00002240: 6573 6f75 7263 652c 2063 6b61 6e5f 7572  esource, ckan_ur
+00002250: 6c2c 2061 7069 5f6b 6579 293a 0a20 2020  l, api_key):.   
+00002260: 2075 726c 203d 2067 6574 5f75 726c 2822   url = get_url("
+00002270: 7265 736f 7572 6365 5f75 7064 6174 6522  resource_update"
+00002280: 2c20 636b 616e 5f75 726c 290a 2020 2020  , ckan_url).    
+00002290: 7220 3d20 7265 7175 6573 7473 2e70 6f73  r = requests.pos
+000022a0: 7428 0a20 2020 2020 2020 2075 726c 2c0a  t(.        url,.
+000022b0: 2020 2020 2020 2020 7665 7269 6679 3d63          verify=c
+000022c0: 6f6e 6669 672e 6765 7428 2253 534c 5f56  onfig.get("SSL_V
+000022d0: 4552 4946 5922 292c 0a20 2020 2020 2020  ERIFY"),.       
+000022e0: 2064 6174 613d 6a73 6f6e 2e64 756d 7073   data=json.dumps
+000022f0: 2872 6573 6f75 7263 6529 2c0a 2020 2020  (resource),.    
+00002300: 2020 2020 6865 6164 6572 733d 7b22 436f      headers={"Co
+00002310: 6e74 656e 742d 5479 7065 223a 2022 6170  ntent-Type": "ap
+00002320: 706c 6963 6174 696f 6e2f 6a73 6f6e 222c  plication/json",
+00002330: 2022 4175 7468 6f72 697a 6174 696f 6e22   "Authorization"
+00002340: 3a20 6170 695f 6b65 797d 2c0a 2020 2020  : api_key},.    
+00002350: 290a 0a20 2020 2063 6865 636b 5f72 6573  )..    check_res
+00002360: 706f 6e73 6528 722c 2075 726c 2c20 2243  ponse(r, url, "C
+00002370: 4b41 4e22 290a 0a0a 6465 6620 6765 745f  KAN")...def get_
+00002380: 7265 736f 7572 6365 2872 6573 6f75 7263  resource(resourc
+00002390: 655f 6964 2c20 636b 616e 5f75 726c 2c20  e_id, ckan_url, 
+000023a0: 6170 695f 6b65 7929 3a0a 2020 2020 2222  api_key):.    ""
+000023b0: 220a 2020 2020 4765 7473 2061 7661 696c  ".    Gets avail
+000023c0: 6162 6c65 2069 6e66 6f72 6d61 7469 6f6e  able information
+000023d0: 2061 626f 7574 2074 6865 2072 6573 6f75   about the resou
+000023e0: 7263 6520 6672 6f6d 2043 4b41 4e0a 2020  rce from CKAN.  
+000023f0: 2020 2222 220a 2020 2020 7572 6c20 3d20    """.    url = 
+00002400: 6765 745f 7572 6c28 2272 6573 6f75 7263  get_url("resourc
+00002410: 655f 7368 6f77 222c 2063 6b61 6e5f 7572  e_show", ckan_ur
+00002420: 6c29 0a20 2020 2072 203d 2072 6571 7565  l).    r = reque
+00002430: 7374 732e 706f 7374 280a 2020 2020 2020  sts.post(.      
+00002440: 2020 7572 6c2c 0a20 2020 2020 2020 2076    url,.        v
+00002450: 6572 6966 793d 636f 6e66 6967 2e67 6574  erify=config.get
+00002460: 2822 5353 4c5f 5645 5249 4659 2229 2c0a  ("SSL_VERIFY"),.
+00002470: 2020 2020 2020 2020 6461 7461 3d6a 736f          data=jso
+00002480: 6e2e 6475 6d70 7328 7b22 6964 223a 2072  n.dumps({"id": r
+00002490: 6573 6f75 7263 655f 6964 7d29 2c0a 2020  esource_id}),.  
+000024a0: 2020 2020 2020 6865 6164 6572 733d 7b22        headers={"
+000024b0: 436f 6e74 656e 742d 5479 7065 223a 2022  Content-Type": "
+000024c0: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+000024d0: 222c 2022 4175 7468 6f72 697a 6174 696f  ", "Authorizatio
+000024e0: 6e22 3a20 6170 695f 6b65 797d 2c0a 2020  n": api_key},.  
+000024f0: 2020 290a 2020 2020 6368 6563 6b5f 7265    ).    check_re
+00002500: 7370 6f6e 7365 2872 2c20 7572 6c2c 2022  sponse(r, url, "
+00002510: 434b 414e 2229 0a0a 2020 2020 7265 7475  CKAN")..    retu
+00002520: 726e 2072 2e6a 736f 6e28 295b 2272 6573  rn r.json()["res
+00002530: 756c 7422 5d0a 0a0a 6465 6620 6765 745f  ult"]...def get_
+00002540: 7061 636b 6167 6528 7061 636b 6167 655f  package(package_
+00002550: 6964 2c20 636b 616e 5f75 726c 2c20 6170  id, ckan_url, ap
+00002560: 695f 6b65 7929 3a0a 2020 2020 2222 220a  i_key):.    """.
+00002570: 2020 2020 4765 7473 2061 7661 696c 6162      Gets availab
+00002580: 6c65 2069 6e66 6f72 6d61 7469 6f6e 2061  le information a
+00002590: 626f 7574 2061 2070 6163 6b61 6765 2066  bout a package f
+000025a0: 726f 6d20 434b 414e 0a20 2020 2022 2222  rom CKAN.    """
+000025b0: 0a20 2020 2075 726c 203d 2067 6574 5f75  .    url = get_u
+000025c0: 726c 2822 7061 636b 6167 655f 7368 6f77  rl("package_show
+000025d0: 222c 2063 6b61 6e5f 7572 6c29 0a20 2020  ", ckan_url).   
+000025e0: 2072 203d 2072 6571 7565 7374 732e 706f   r = requests.po
+000025f0: 7374 280a 2020 2020 2020 2020 7572 6c2c  st(.        url,
+00002600: 0a20 2020 2020 2020 2076 6572 6966 793d  .        verify=
+00002610: 636f 6e66 6967 2e67 6574 2822 5353 4c5f  config.get("SSL_
+00002620: 5645 5249 4659 2229 2c0a 2020 2020 2020  VERIFY"),.      
+00002630: 2020 6461 7461 3d6a 736f 6e2e 6475 6d70    data=json.dump
+00002640: 7328 7b22 6964 223a 2070 6163 6b61 6765  s({"id": package
+00002650: 5f69 647d 292c 0a20 2020 2020 2020 2068  _id}),.        h
+00002660: 6561 6465 7273 3d7b 2243 6f6e 7465 6e74  eaders={"Content
+00002670: 2d54 7970 6522 3a20 2261 7070 6c69 6361  -Type": "applica
+00002680: 7469 6f6e 2f6a 736f 6e22 2c20 2241 7574  tion/json", "Aut
+00002690: 686f 7269 7a61 7469 6f6e 223a 2061 7069  horization": api
+000026a0: 5f6b 6579 7d2c 0a20 2020 2029 0a20 2020  _key},.    ).   
+000026b0: 2063 6865 636b 5f72 6573 706f 6e73 6528   check_response(
+000026c0: 722c 2075 726c 2c20 2243 4b41 4e22 290a  r, url, "CKAN").
+000026d0: 0a20 2020 2072 6574 7572 6e20 722e 6a73  .    return r.js
+000026e0: 6f6e 2829 5b22 7265 7375 6c74 225d 0a0a  on()["result"]..
+000026f0: 0a64 6566 2076 616c 6964 6174 655f 696e  .def validate_in
+00002700: 7075 7428 696e 7075 7429 3a0a 2020 2020  put(input):.    
+00002710: 2320 4573 7065 6369 616c 6c79 2076 616c  # Especially val
+00002720: 6964 6174 6520 6d65 7461 6461 7461 2077  idate metadata w
+00002730: 6869 6368 2069 7320 7072 6f76 6964 6564  hich is provided
+00002740: 2062 7920 7468 6520 7573 6572 0a20 2020   by the user.   
+00002750: 2069 6620 226d 6574 6164 6174 6122 206e   if "metadata" n
+00002760: 6f74 2069 6e20 696e 7075 743a 0a20 2020  ot in input:.   
+00002770: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
+00002780: 4a6f 6245 7272 6f72 2822 4d65 7461 6461  JobError("Metada
+00002790: 7461 206d 6973 7369 6e67 2229 0a0a 2020  ta missing")..  
+000027a0: 2020 6461 7461 203d 2069 6e70 7574 5b22    data = input["
+000027b0: 6d65 7461 6461 7461 225d 0a0a 2020 2020  metadata"]..    
+000027c0: 6966 2022 7265 736f 7572 6365 5f69 6422  if "resource_id"
+000027d0: 206e 6f74 2069 6e20 6461 7461 3a0a 2020   not in data:.  
+000027e0: 2020 2020 2020 7261 6973 6520 7574 696c        raise util
+000027f0: 2e4a 6f62 4572 726f 7228 224e 6f20 6964  .JobError("No id
+00002800: 2070 726f 7669 6465 642e 2229 0a20 2020   provided.").   
+00002810: 2069 6620 2263 6b61 6e5f 7572 6c22 206e   if "ckan_url" n
+00002820: 6f74 2069 6e20 6461 7461 3a0a 2020 2020  ot in data:.    
+00002830: 2020 2020 7261 6973 6520 7574 696c 2e4a      raise util.J
+00002840: 6f62 4572 726f 7228 224e 6f20 636b 616e  obError("No ckan
+00002850: 5f75 726c 2070 726f 7669 6465 642e 2229  _url provided.")
+00002860: 0a20 2020 2069 6620 6e6f 7420 696e 7075  .    if not inpu
+00002870: 742e 6765 7428 2261 7069 5f6b 6579 2229  t.get("api_key")
+00002880: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00002890: 7574 696c 2e4a 6f62 4572 726f 7228 224e  util.JobError("N
+000028a0: 6f20 434b 414e 2041 5049 206b 6579 2070  o CKAN API key p
+000028b0: 726f 7669 6465 6422 290a 0a0a 406a 6f62  rovided")...@job
+000028c0: 2e61 7379 6e63 6872 6f6e 6f75 730a 6465  .asynchronous.de
+000028d0: 6620 7075 7368 5f74 6f5f 6461 7461 7374  f push_to_datast
+000028e0: 6f72 6528 7461 736b 5f69 642c 2069 6e70  ore(task_id, inp
+000028f0: 7574 2c20 6472 795f 7275 6e3d 4661 6c73  ut, dry_run=Fals
+00002900: 6529 3a0a 2020 2020 2222 2244 6f77 6e6c  e):.    """Downl
+00002910: 6f61 6420 616e 6420 7061 7273 6520 6120  oad and parse a 
+00002920: 7265 736f 7572 6365 2070 7573 6820 6974  resource push it
+00002930: 7320 6461 7461 2069 6e74 6f20 434b 414e  s data into CKAN
+00002940: 2773 2044 6174 6153 746f 7265 2e0a 0a20  's DataStore... 
+00002950: 2020 2041 6e20 6173 796e 6368 726f 6e6f     An asynchrono
+00002960: 7573 206a 6f62 2074 6861 7420 6765 7473  us job that gets
+00002970: 2061 2072 6573 6f75 7263 6520 6672 6f6d   a resource from
+00002980: 2043 4b41 4e2c 2064 6f77 6e6c 6f61 6473   CKAN, downloads
+00002990: 2074 6865 0a20 2020 2072 6573 6f75 7263   the.    resourc
+000029a0: 6527 7320 6461 7461 2066 696c 6520 616e  e's data file an
+000029b0: 642c 2069 6620 7468 6520 6461 7461 2066  d, if the data f
+000029c0: 696c 6520 6861 7320 6368 616e 6765 6420  ile has changed 
+000029d0: 7369 6e63 6520 6c61 7374 2074 696d 652c  since last time,
+000029e0: 0a20 2020 2070 6172 7365 7320 7468 6520  .    parses the 
+000029f0: 6461 7461 2061 6e64 2070 6f73 7473 2069  data and posts i
+00002a00: 7420 696e 746f 2043 4b41 4e27 7320 4461  t into CKAN's Da
+00002a10: 7461 5374 6f72 652e 0a0a 2020 2020 3a70  taStore...    :p
+00002a20: 6172 616d 2064 7279 5f72 756e 3a20 4665  aram dry_run: Fe
+00002a30: 7463 6820 616e 6420 7061 7273 6520 7468  tch and parse th
+00002a40: 6520 6461 7461 2066 696c 6520 6275 7420  e data file but 
+00002a50: 646f 6e27 7420 6163 7475 616c 6c79 2070  don't actually p
+00002a60: 6f73 7420 7468 650a 2020 2020 2020 2020  ost the.        
+00002a70: 6461 7461 2074 6f20 7468 6520 4461 7461  data to the Data
+00002a80: 5374 6f72 652c 2069 6e73 7465 6164 2072  Store, instead r
+00002a90: 6574 7572 6e20 7468 6520 6461 7461 2068  eturn the data h
+00002aa0: 6561 6465 7273 2061 6e64 2072 6f77 7320  eaders and rows 
+00002ab0: 7468 6174 0a20 2020 2020 2020 2077 6f75  that.        wou
+00002ac0: 6c64 2068 6176 6520 6265 656e 2070 6f73  ld have been pos
+00002ad0: 7465 642e 0a20 2020 203a 7479 7065 2064  ted..    :type d
+00002ae0: 7279 5f72 756e 3a20 626f 6f6c 6561 6e0a  ry_run: boolean.
+00002af0: 0a20 2020 2022 2222 0a20 2020 2068 616e  .    """.    han
+00002b00: 646c 6572 203d 2075 7469 6c2e 5374 6f72  dler = util.Stor
+00002b10: 696e 6748 616e 646c 6572 2874 6173 6b5f  ingHandler(task_
+00002b20: 6964 2c20 696e 7075 7429 0a20 2020 206c  id, input).    l
+00002b30: 6f67 6765 7220 3d20 6c6f 6767 696e 672e  ogger = logging.
+00002b40: 6765 744c 6f67 6765 7228 7461 736b 5f69  getLogger(task_i
+00002b50: 6429 0a20 2020 206c 6f67 6765 722e 6164  d).    logger.ad
+00002b60: 6448 616e 646c 6572 2868 616e 646c 6572  dHandler(handler
+00002b70: 290a 2020 2020 6c6f 6767 6572 2e73 6574  ).    logger.set
+00002b80: 4c65 7665 6c28 6c6f 6767 696e 672e 4445  Level(logging.DE
+00002b90: 4255 4729 0a0a 2020 2020 2320 6368 6563  BUG)..    # chec
+00002ba0: 6b20 6966 2051 5356 5f42 494e 2061 6e64  k if QSV_BIN and
+00002bb0: 2046 494c 455f 4249 4e20 6578 6973 7473   FILE_BIN exists
+00002bc0: 0a20 2020 2071 7376 5f62 696e 203d 2063  .    qsv_bin = c
+00002bd0: 6f6e 6669 672e 6765 7428 2251 5356 5f42  onfig.get("QSV_B
+00002be0: 494e 2229 0a20 2020 2071 7376 5f70 6174  IN").    qsv_pat
+00002bf0: 6820 3d20 5061 7468 2871 7376 5f62 696e  h = Path(qsv_bin
+00002c00: 290a 2020 2020 6966 206e 6f74 2071 7376  ).    if not qsv
+00002c10: 5f70 6174 682e 6973 5f66 696c 6528 293a  _path.is_file():
+00002c20: 0a20 2020 2020 2020 2072 6169 7365 2075  .        raise u
+00002c30: 7469 6c2e 4a6f 6245 7272 6f72 2822 7b7d  til.JobError("{}
+00002c40: 206e 6f74 2066 6f75 6e64 2e22 2e66 6f72   not found.".for
+00002c50: 6d61 7428 7173 765f 6269 6e29 290a 2020  mat(qsv_bin)).  
+00002c60: 2020 6669 6c65 5f62 696e 203d 2063 6f6e    file_bin = con
+00002c70: 6669 672e 6765 7428 2246 494c 455f 4249  fig.get("FILE_BI
+00002c80: 4e22 290a 0a20 2020 2066 696c 655f 7061  N")..    file_pa
+00002c90: 7468 203d 2050 6174 6828 6669 6c65 5f62  th = Path(file_b
+00002ca0: 696e 290a 2020 2020 6966 206e 6f74 2066  in).    if not f
+00002cb0: 696c 655f 7061 7468 2e69 735f 6669 6c65  ile_path.is_file
+00002cc0: 2829 3a0a 2020 2020 2020 2020 7261 6973  ():.        rais
+00002cd0: 6520 7574 696c 2e4a 6f62 4572 726f 7228  e util.JobError(
+00002ce0: 227b 7d20 6e6f 7420 666f 756e 642e 222e  "{} not found.".
+00002cf0: 666f 726d 6174 2866 696c 655f 6269 6e29  format(file_bin)
+00002d00: 290a 0a20 2020 2023 206d 616b 6520 7375  )..    # make su
+00002d10: 7265 2071 7376 2062 696e 6172 7920 7661  re qsv binary va
+00002d20: 7269 616e 7420 6973 2075 702d 746f 2d64  riant is up-to-d
+00002d30: 6174 650a 2020 2020 7472 793a 0a20 2020  ate.    try:.   
+00002d40: 2020 2020 2071 7376 5f76 6572 7369 6f6e       qsv_version
+00002d50: 203d 2073 7562 7072 6f63 6573 732e 7275   = subprocess.ru
+00002d60: 6e28 0a20 2020 2020 2020 2020 2020 205b  n(.            [
+00002d70: 7173 765f 6269 6e2c 2022 2d2d 7665 7273  qsv_bin, "--vers
+00002d80: 696f 6e22 5d2c 0a20 2020 2020 2020 2020  ion"],.         
+00002d90: 2020 2063 6170 7475 7265 5f6f 7574 7075     capture_outpu
+00002da0: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
+00002db0: 2020 2020 7465 7874 3d54 7275 652c 0a20      text=True,. 
+00002dc0: 2020 2020 2020 2029 0a20 2020 2065 7863         ).    exc
+00002dd0: 6570 7420 7375 6270 726f 6365 7373 2e43  ept subprocess.C
+00002de0: 616c 6c65 6450 726f 6365 7373 4572 726f  alledProcessErro
+00002df0: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
+00002e00: 7261 6973 6520 7574 696c 2e4a 6f62 4572  raise util.JobEr
+00002e10: 726f 7228 2271 7376 2076 6572 7369 6f6e  ror("qsv version
+00002e20: 2063 6865 636b 2065 7272 6f72 3a20 7b7d   check error: {}
+00002e30: 222e 666f 726d 6174 2865 2929 0a20 2020  ".format(e)).   
+00002e40: 2071 7376 5f76 6572 7369 6f6e 5f69 6e66   qsv_version_inf
+00002e50: 6f20 3d20 7374 7228 7173 765f 7665 7273  o = str(qsv_vers
+00002e60: 696f 6e2e 7374 646f 7574 290a 2020 2020  ion.stdout).    
+00002e70: 7173 765f 7365 6d76 6572 203d 2071 7376  qsv_semver = qsv
+00002e80: 5f76 6572 7369 6f6e 5f69 6e66 6f5b 0a20  _version_info[. 
+00002e90: 2020 2020 2020 2071 7376 5f76 6572 7369         qsv_versi
+00002ea0: 6f6e 5f69 6e66 6f2e 6669 6e64 2822 2022  on_info.find(" "
+00002eb0: 2920 3a20 7173 765f 7665 7273 696f 6e5f  ) : qsv_version_
+00002ec0: 696e 666f 2e66 696e 6428 222d 2229 0a20  info.find("-"). 
+00002ed0: 2020 205d 2e6c 7374 7269 7028 290a 2020     ].lstrip().  
+00002ee0: 2020 7472 793a 0a20 2020 2020 2020 2069    try:.        i
+00002ef0: 6620 7365 6d76 6572 2e63 6f6d 7061 7265  f semver.compare
+00002f00: 2871 7376 5f73 656d 7665 722c 2022 302e  (qsv_semver, "0.
+00002f10: 3835 2e30 2229 203c 2030 3a0a 2020 2020  85.0") < 0:.    
+00002f20: 2020 2020 2020 2020 7261 6973 6520 7574          raise ut
+00002f30: 696c 2e4a 6f62 4572 726f 7228 0a20 2020  il.JobError(.   
+00002f40: 2020 2020 2020 2020 2020 2020 2022 4174               "At
+00002f50: 206c 6561 7374 2071 7376 2076 6572 7369   least qsv versi
+00002f60: 6f6e 2030 2e38 352e 3020 7265 7175 6972  on 0.85.0 requir
+00002f70: 6564 2e20 466f 756e 6420 7b7d 2e20 596f  ed. Found {}. Yo
+00002f80: 7520 6361 6e20 6765 7420 7468 6520 6c61  u can get the la
+00002f90: 7465 7374 2072 656c 6561 7365 2061 7420  test release at 
+00002fa0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00002fb0: 6f6d 2f6a 716e 6174 6976 6964 6164 2f71  om/jqnatividad/q
+00002fc0: 7376 2f72 656c 6561 7365 732f 6c61 7465  sv/releases/late
+00002fd0: 7374 222e 666f 726d 6174 280a 2020 2020  st".format(.    
+00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ff0: 7173 765f 7665 7273 696f 6e5f 696e 666f  qsv_version_info
+00003000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003010: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+00003020: 0a20 2020 2065 7863 6570 7420 5661 6c75  .    except Valu
+00003030: 6545 7272 6f72 2061 7320 653a 0a20 2020  eError as e:.   
+00003040: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
+00003050: 4a6f 6245 7272 6f72 2822 4361 6e6e 6f74  JobError("Cannot
+00003060: 2070 6172 7365 2071 7376 2076 6572 7369   parse qsv versi
+00003070: 6f6e 2069 6e66 6f3a 207b 7d22 2e66 6f72  on info: {}".for
+00003080: 6d61 7428 6529 290a 0a20 2020 2076 616c  mat(e))..    val
+00003090: 6964 6174 655f 696e 7075 7428 696e 7075  idate_input(inpu
+000030a0: 7429 0a0a 2020 2020 6461 7461 203d 2069  t)..    data = i
+000030b0: 6e70 7574 5b22 6d65 7461 6461 7461 225d  nput["metadata"]
+000030c0: 0a0a 2020 2020 636b 616e 5f75 726c 203d  ..    ckan_url =
+000030d0: 2064 6174 615b 2263 6b61 6e5f 7572 6c22   data["ckan_url"
+000030e0: 5d0a 2020 2020 7265 736f 7572 6365 5f69  ].    resource_i
+000030f0: 6420 3d20 6461 7461 5b22 7265 736f 7572  d = data["resour
+00003100: 6365 5f69 6422 5d0a 2020 2020 6170 695f  ce_id"].    api_
+00003110: 6b65 7920 3d20 696e 7075 742e 6765 7428  key = input.get(
+00003120: 2261 7069 5f6b 6579 2229 0a0a 2020 2020  "api_key")..    
+00003130: 7472 793a 0a20 2020 2020 2020 2072 6573  try:.        res
+00003140: 6f75 7263 6520 3d20 6765 745f 7265 736f  ource = get_reso
+00003150: 7572 6365 2872 6573 6f75 7263 655f 6964  urce(resource_id
+00003160: 2c20 636b 616e 5f75 726c 2c20 6170 695f  , ckan_url, api_
+00003170: 6b65 7929 0a20 2020 2065 7863 6570 7420  key).    except 
+00003180: 7574 696c 2e4a 6f62 4572 726f 723a 0a20  util.JobError:. 
+00003190: 2020 2020 2020 2023 2074 7279 2061 6761         # try aga
+000031a0: 696e 2069 6e20 3520 7365 636f 6e64 7320  in in 5 seconds 
+000031b0: 6a75 7374 2069 6e63 6173 6520 434b 414e  just incase CKAN
+000031c0: 2069 7320 736c 6f77 2061 7420 6164 6469   is slow at addi
+000031d0: 6e67 2072 6573 6f75 7263 650a 2020 2020  ng resource.    
+000031e0: 2020 2020 7469 6d65 2e73 6c65 6570 2835      time.sleep(5
+000031f0: 290a 2020 2020 2020 2020 7265 736f 7572  ).        resour
+00003200: 6365 203d 2067 6574 5f72 6573 6f75 7263  ce = get_resourc
+00003210: 6528 7265 736f 7572 6365 5f69 642c 2063  e(resource_id, c
+00003220: 6b61 6e5f 7572 6c2c 2061 7069 5f6b 6579  kan_url, api_key
+00003230: 290a 0a20 2020 2023 2063 6865 636b 2069  )..    # check i
+00003240: 6620 7468 6520 7265 736f 7572 6365 2075  f the resource u
+00003250: 726c 5f74 7970 6520 6973 2061 2064 6174  rl_type is a dat
+00003260: 6173 746f 7265 0a20 2020 2069 6620 7265  astore.    if re
+00003270: 736f 7572 6365 2e67 6574 2822 7572 6c5f  source.get("url_
+00003280: 7479 7065 2229 203d 3d20 2264 6174 6173  type") == "datas
+00003290: 746f 7265 223a 0a20 2020 2020 2020 206c  tore":.        l
+000032a0: 6f67 6765 722e 696e 666f 2822 4475 6d70  ogger.info("Dump
+000032b0: 2066 696c 6573 2061 7265 206d 616e 6167   files are manag
+000032c0: 6564 2077 6974 6820 7468 6520 4461 7461  ed with the Data
+000032d0: 7374 6f72 6520 4150 4922 290a 2020 2020  store API").    
+000032e0: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+000032f0: 2320 6368 6563 6b20 7363 6865 6d65 0a20  # check scheme. 
+00003300: 2020 2075 726c 203d 2072 6573 6f75 7263     url = resourc
+00003310: 652e 6765 7428 2275 726c 2229 0a20 2020  e.get("url").   
+00003320: 2073 6368 656d 6520 3d20 7572 6c73 706c   scheme = urlspl
+00003330: 6974 2875 726c 292e 7363 6865 6d65 0a20  it(url).scheme. 
+00003340: 2020 2069 6620 7363 6865 6d65 206e 6f74     if scheme not
+00003350: 2069 6e20 2822 6874 7470 222c 2022 6874   in ("http", "ht
+00003360: 7470 7322 2c20 2266 7470 2229 3a0a 2020  tps", "ftp"):.  
+00003370: 2020 2020 2020 7261 6973 6520 7574 696c        raise util
+00003380: 2e4a 6f62 4572 726f 7228 224f 6e6c 7920  .JobError("Only 
+00003390: 6874 7470 2c20 6874 7470 732c 2061 6e64  http, https, and
+000033a0: 2066 7470 2072 6573 6f75 7263 6573 206d   ftp resources m
+000033b0: 6179 2062 6520 6665 7463 6865 642e 2229  ay be fetched.")
+000033c0: 0a0a 2020 2020 2320 3d3d 3d3d 3d3d 3d3d  ..    # ========
+000033d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000033e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000033f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003400: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003410: 3d3d 0a20 2020 2023 2044 4f57 4e4c 4f41  ==.    # DOWNLOA
+00003420: 440a 2020 2020 2320 3d3d 3d3d 3d3d 3d3d  D.    # ========
+00003430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003450: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003470: 3d3d 0a20 2020 2074 696d 6572 5f73 7461  ==.    timer_sta
+00003480: 7274 203d 2074 696d 652e 7065 7266 5f63  rt = time.perf_c
+00003490: 6f75 6e74 6572 2829 0a0a 2020 2020 2320  ounter()..    # 
+000034a0: 6665 7463 6820 7468 6520 7265 736f 7572  fetch the resour
+000034b0: 6365 2064 6174 610a 2020 2020 6c6f 6767  ce data.    logg
+000034c0: 6572 2e69 6e66 6f28 2246 6574 6368 696e  er.info("Fetchin
+000034d0: 6720 6672 6f6d 3a20 7b30 7d2e 2e2e 222e  g from: {0}...".
+000034e0: 666f 726d 6174 2875 726c 2929 0a20 2020  format(url)).   
+000034f0: 2068 6561 6465 7273 203d 207b 7d0a 2020   headers = {}.  
+00003500: 2020 7072 6576 6965 775f 726f 7773 203d    preview_rows =
+00003510: 2069 6e74 2863 6f6e 6669 672e 6765 7428   int(config.get(
+00003520: 2250 5245 5649 4557 5f52 4f57 5322 2929  "PREVIEW_ROWS"))
+00003530: 0a20 2020 2064 6f77 6e6c 6f61 645f 7072  .    download_pr
+00003540: 6576 6965 775f 6f6e 6c79 203d 2063 6f6e  eview_only = con
+00003550: 6669 672e 6765 7428 2244 4f57 4e4c 4f41  fig.get("DOWNLOA
+00003560: 445f 5052 4556 4945 575f 4f4e 4c59 2229  D_PREVIEW_ONLY")
+00003570: 0a20 2020 2069 6620 7265 736f 7572 6365  .    if resource
+00003580: 2e67 6574 2822 7572 6c5f 7479 7065 2229  .get("url_type")
+00003590: 203d 3d20 2275 706c 6f61 6422 3a0a 2020   == "upload":.  
+000035a0: 2020 2020 2020 2320 4966 2074 6869 7320        # If this 
+000035b0: 6973 2061 6e20 7570 6c6f 6164 6564 2066  is an uploaded f
+000035c0: 696c 6520 746f 2043 4b41 4e2c 2061 7574  ile to CKAN, aut
+000035d0: 6865 6e74 6963 6174 6520 7468 6520 7265  henticate the re
+000035e0: 7175 6573 742c 0a20 2020 2020 2020 2023  quest,.        #
+000035f0: 206f 7468 6572 7769 7365 2077 6520 776f   otherwise we wo
+00003600: 6e27 7420 6765 7420 6669 6c65 2066 726f  n't get file fro
+00003610: 6d20 7072 6976 6174 6520 7265 736f 7572  m private resour
+00003620: 6365 730a 2020 2020 2020 2020 6865 6164  ces.        head
+00003630: 6572 735b 2241 7574 686f 7269 7a61 7469  ers["Authorizati
+00003640: 6f6e 225d 203d 2061 7069 5f6b 6579 0a20  on"] = api_key. 
+00003650: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00003660: 6b77 6172 6773 203d 207b 0a20 2020 2020  kwargs = {.     
+00003670: 2020 2020 2020 2022 6865 6164 6572 7322         "headers"
+00003680: 3a20 6865 6164 6572 732c 0a20 2020 2020  : headers,.     
+00003690: 2020 2020 2020 2022 7469 6d65 6f75 7422         "timeout"
+000036a0: 3a20 636f 6e66 6967 2e67 6574 2822 444f  : config.get("DO
+000036b0: 574e 4c4f 4144 5f54 494d 454f 5554 2229  WNLOAD_TIMEOUT")
+000036c0: 2c0a 2020 2020 2020 2020 2020 2020 2276  ,.            "v
+000036d0: 6572 6966 7922 3a20 636f 6e66 6967 2e67  erify": config.g
+000036e0: 6574 2822 5353 4c5f 5645 5249 4659 2229  et("SSL_VERIFY")
+000036f0: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
+00003700: 7472 6561 6d22 3a20 5472 7565 2c0a 2020  tream": True,.  
+00003710: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00003720: 6966 2055 5345 5f50 524f 5859 3a0a 2020  if USE_PROXY:.  
+00003730: 2020 2020 2020 2020 2020 6b77 6172 6773            kwargs
+00003740: 5b22 7072 6f78 6965 7322 5d20 3d20 7b22  ["proxies"] = {"
+00003750: 6874 7470 223a 2044 4f57 4e4c 4f41 445f  http": DOWNLOAD_
+00003760: 5052 4f58 592c 2022 6874 7470 7322 3a20  PROXY, "https": 
+00003770: 444f 574e 4c4f 4144 5f50 524f 5859 7d0a  DOWNLOAD_PROXY}.
+00003780: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00003790: 203d 2072 6571 7565 7374 732e 6765 7428   = requests.get(
+000037a0: 7572 6c2c 202a 2a6b 7761 7267 7329 0a20  url, **kwargs). 
+000037b0: 2020 2020 2020 2072 6573 706f 6e73 652e         response.
+000037c0: 7261 6973 655f 666f 725f 7374 6174 7573  raise_for_status
+000037d0: 2829 0a0a 2020 2020 2020 2020 636c 203d  ()..        cl =
+000037e0: 2072 6573 706f 6e73 652e 6865 6164 6572   response.header
+000037f0: 732e 6765 7428 2263 6f6e 7465 6e74 2d6c  s.get("content-l
+00003800: 656e 6774 6822 290a 2020 2020 2020 2020  ength").        
+00003810: 6d61 785f 636f 6e74 656e 745f 6c65 6e67  max_content_leng
+00003820: 7468 203d 2069 6e74 2863 6f6e 6669 672e  th = int(config.
+00003830: 6765 7428 224d 4158 5f43 4f4e 5445 4e54  get("MAX_CONTENT
+00003840: 5f4c 454e 4754 4822 2929 0a20 2020 2020  _LENGTH")).     
+00003850: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+00003860: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+00003870: 2020 2020 2020 2020 2063 6c0a 2020 2020           cl.    
+00003880: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00003890: 696e 7428 636c 2920 3e20 6d61 785f 636f  int(cl) > max_co
+000038a0: 6e74 656e 745f 6c65 6e67 7468 0a20 2020  ntent_length.   
+000038b0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+000038c0: 2028 7072 6576 6965 775f 726f 7773 203e   (preview_rows >
+000038d0: 2030 2061 6e64 206e 6f74 2064 6f77 6e6c   0 and not downl
+000038e0: 6f61 645f 7072 6576 6965 775f 6f6e 6c79  oad_preview_only
+000038f0: 290a 2020 2020 2020 2020 2020 2020 293a  ).            ):
+00003900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003910: 2072 6169 7365 2075 7469 6c2e 4a6f 6245   raise util.JobE
+00003920: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00003930: 2020 2020 2020 2020 2020 2252 6573 6f75            "Resou
+00003940: 7263 6520 746f 6f20 6c61 7267 6520 746f  rce too large to
+00003950: 2064 6f77 6e6c 6f61 643a 207b 636c 3a2e   download: {cl:.
+00003960: 324d 427d 203e 206d 6178 2028 7b6d 6178  2MB} > max ({max
+00003970: 5f63 6c3a 2e32 4d42 7d29 2e22 2e66 6f72  _cl:.2MB}).".for
+00003980: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+00003990: 2020 2020 2020 2020 2020 2020 2063 6c3d               cl=
+000039a0: 4461 7461 5369 7a65 2869 6e74 2863 6c29  DataSize(int(cl)
+000039b0: 292c 206d 6178 5f63 6c3d 4461 7461 5369  ), max_cl=DataSi
+000039c0: 7a65 2869 6e74 286d 6178 5f63 6f6e 7465  ze(int(max_conte
+000039d0: 6e74 5f6c 656e 6774 6829 290a 2020 2020  nt_length)).    
+000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003a00: 2020 290a 2020 2020 2020 2020 6578 6365    ).        exce
+00003a10: 7074 2056 616c 7565 4572 726f 723a 0a20  pt ValueError:. 
+00003a20: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
+00003a30: 0a20 2020 2020 2020 2074 6d70 203d 2074  .        tmp = t
+00003a40: 656d 7066 696c 652e 4e61 6d65 6454 656d  empfile.NamedTem
+00003a50: 706f 7261 7279 4669 6c65 2873 7566 6669  poraryFile(suffi
+00003a60: 783d 222e 2220 2b20 7265 736f 7572 6365  x="." + resource
+00003a70: 2e67 6574 2822 666f 726d 6174 2229 2e6c  .get("format").l
+00003a80: 6f77 6572 2829 290a 2020 2020 2020 2020  ower()).        
+00003a90: 6c65 6e67 7468 203d 2030 0a20 2020 2020  length = 0.     
+00003aa0: 2020 206d 203d 2068 6173 686c 6962 2e6d     m = hashlib.m
+00003ab0: 6435 2829 0a0a 2020 2020 2020 2020 6966  d5()..        if
+00003ac0: 2064 6f77 6e6c 6f61 645f 7072 6576 6965   download_previe
+00003ad0: 775f 6f6e 6c79 2061 6e64 2070 7265 7669  w_only and previ
+00003ae0: 6577 5f72 6f77 7320 3e20 303a 0a20 2020  ew_rows > 0:.   
+00003af0: 2020 2020 2020 2020 2023 2069 6620 646f           # if do
+00003b00: 776e 6c6f 6164 5f70 7265 7669 6577 5f6f  wnload_preview_o
+00003b10: 6e6c 7920 616e 6420 7072 6576 6965 775f  nly and preview_
+00003b20: 726f 7773 2069 7320 6772 6561 7465 7220  rows is greater 
+00003b30: 7468 616e 207a 6572 6f0a 2020 2020 2020  than zero.      
+00003b40: 2020 2020 2020 2320 7765 2772 6520 646f        # we're do
+00003b50: 776e 6c6f 6164 696e 6720 7468 6520 7072  wnloading the pr
+00003b60: 6576 6965 7720 726f 7773 206f 6e6c 792c  eview rows only,
+00003b70: 206e 6f74 2074 6865 2077 686f 6c65 2066   not the whole f
+00003b80: 696c 650a 2020 2020 2020 2020 2020 2020  ile.            
+00003b90: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+00003ba0: 2020 2020 2020 2020 2020 2020 2022 446f               "Do
+00003bb0: 776e 6c6f 6164 696e 6720 6f6e 6c79 2066  wnloading only f
+00003bc0: 6972 7374 207b 3a2c 7d20 726f 7720 7072  irst {:,} row pr
+00003bd0: 6576 6965 7720 6672 6f6d 207b 3a2e 324d  eview from {:.2M
+00003be0: 427d 2066 696c 652e 2e2e 222e 666f 726d  B} file...".form
+00003bf0: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00003c00: 2020 2020 2020 2020 7072 6576 6965 775f          preview_
+00003c10: 726f 7773 2c20 4461 7461 5369 7a65 2869  rows, DataSize(i
+00003c20: 6e74 2863 6c29 290a 2020 2020 2020 2020  nt(cl)).        
+00003c30: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00003c40: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00003c50: 2020 2020 2063 7572 725f 6c69 6e65 203d       curr_line =
+00003c60: 2030 0a20 2020 2020 2020 2020 2020 2066   0.            f
+00003c70: 6f72 206c 696e 6520 696e 2072 6573 706f  or line in respo
+00003c80: 6e73 652e 6974 6572 5f6c 696e 6573 2869  nse.iter_lines(i
+00003c90: 6e74 2863 6f6e 6669 672e 6765 7428 2243  nt(config.get("C
+00003ca0: 4855 4e4b 5f53 495a 4522 2929 293a 0a20  HUNK_SIZE"))):. 
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00003cc0: 7572 725f 6c69 6e65 202b 3d20 310a 2020  urr_line += 1.  
+00003cd0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003ce0: 6164 6420 6261 636b 2074 6865 206c 696e  add back the lin
+00003cf0: 6566 6565 6420 6173 2069 7465 725f 6c69  efeed as iter_li
+00003d00: 6e65 7320 7265 6d6f 7665 7320 6974 0a20  nes removes it. 
+00003d10: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00003d20: 696e 6520 3d20 6c69 6e65 202b 2022 5c6e  ine = line + "\n
+00003d30: 222e 656e 636f 6465 2822 6173 6369 6922  ".encode("ascii"
+00003d40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003d50: 2020 6c65 6e67 7468 202b 3d20 6c65 6e28    length += len(
+00003d60: 6c69 6e65 290a 0a20 2020 2020 2020 2020  line)..         
+00003d70: 2020 2020 2020 2074 6d70 2e77 7269 7465         tmp.write
+00003d80: 286c 696e 6529 0a20 2020 2020 2020 2020  (line).         
+00003d90: 2020 2020 2020 206d 2e75 7064 6174 6528         m.update(
+00003da0: 6c69 6e65 290a 2020 2020 2020 2020 2020  line).          
+00003db0: 2020 2020 2020 6966 2063 7572 725f 6c69        if curr_li
+00003dc0: 6e65 203e 2070 7265 7669 6577 5f72 6f77  ne > preview_row
+00003dd0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00003de0: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00003df0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00003e00: 2020 2020 2020 2023 2064 6f77 6e6c 6f61         # downloa
+00003e10: 6420 7468 6520 656e 7469 7265 2066 696c  d the entire fil
+00003e20: 6520 6f74 6865 7277 6973 650a 2020 2020  e otherwise.    
+00003e30: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
+00003e40: 6861 6e64 6c65 2077 6865 6e20 7072 6576  handle when prev
+00003e50: 6965 775f 726f 7773 2069 7320 6e65 6761  iew_rows is nega
+00003e60: 7469 7665 2028 6765 7420 7468 6520 7072  tive (get the pr
+00003e70: 6576 6965 7720 6672 6f6d 2074 6865 0a20  eview from the. 
+00003e80: 2020 2020 2020 2020 2020 2023 2065 6e64             # end
+00003e90: 206f 6620 7468 6520 6669 6c65 2920 736f   of the file) so
+00003ea0: 2077 6520 6361 6e20 7573 6520 6874 7470   we can use http
+00003eb0: 2072 616e 6765 2072 6571 7565 7374 2074   range request t
+00003ec0: 6f20 6765 7420 7468 6520 7072 6576 6965  o get the previe
+00003ed0: 7720 6672 6f6d 0a20 2020 2020 2020 2020  w from.         
+00003ee0: 2020 2023 2074 6865 2065 6e64 2077 6974     # the end wit
+00003ef0: 686f 7574 2064 6f77 6e6c 6f61 6469 6e67  hout downloading
+00003f00: 2074 6865 2065 6e74 6972 6520 6669 6c65   the entire file
+00003f10: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00003f20: 6765 722e 696e 666f 2822 446f 776e 6c6f  ger.info("Downlo
+00003f30: 6164 696e 6720 7b3a 2e32 4d42 7d20 6669  ading {:.2MB} fi
+00003f40: 6c65 2e2e 2e22 2e66 6f72 6d61 7428 4461  le...".format(Da
+00003f50: 7461 5369 7a65 2869 6e74 2863 6c29 2929  taSize(int(cl)))
+00003f60: 290a 0a20 2020 2020 2020 2020 2020 2066  )..            f
+00003f70: 6f72 2063 6875 6e6b 2069 6e20 7265 7370  or chunk in resp
+00003f80: 6f6e 7365 2e69 7465 725f 636f 6e74 656e  onse.iter_conten
+00003f90: 7428 696e 7428 636f 6e66 6967 2e67 6574  t(int(config.get
+00003fa0: 2822 4348 554e 4b5f 5349 5a45 2229 2929  ("CHUNK_SIZE")))
+00003fb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003fc0: 2020 6c65 6e67 7468 202b 3d20 6c65 6e28    length += len(
+00003fd0: 6368 756e 6b29 0a20 2020 2020 2020 2020  chunk).         
+00003fe0: 2020 2020 2020 2069 6620 6c65 6e67 7468         if length
+00003ff0: 203e 206d 6178 5f63 6f6e 7465 6e74 5f6c   > max_content_l
+00004000: 656e 6774 6820 616e 6420 6e6f 7420 7072  ength and not pr
+00004010: 6576 6965 775f 726f 7773 3a0a 2020 2020  eview_rows:.    
+00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004030: 7261 6973 6520 7574 696c 2e4a 6f62 4572  raise util.JobEr
+00004040: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00004050: 2020 2020 2020 2020 2020 2020 2022 5265               "Re
+00004060: 736f 7572 6365 2074 6f6f 206c 6172 6765  source too large
+00004070: 2074 6f20 7072 6f63 6573 733a 207b 636c   to process: {cl
+00004080: 7d20 3e20 6d61 7820 287b 6d61 785f 636c  } > max ({max_cl
+00004090: 7d29 2e22 2e66 6f72 6d61 7428 0a20 2020  }).".format(.   
+000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040b0: 2020 2020 2020 2020 2063 6c3d 6c65 6e67           cl=leng
+000040c0: 7468 2c20 6d61 785f 636c 3d6d 6178 5f63  th, max_cl=max_c
+000040d0: 6f6e 7465 6e74 5f6c 656e 6774 680a 2020  ontent_length.  
+000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004100: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00004110: 2020 2020 2020 2020 2020 2020 2020 746d                tm
+00004120: 702e 7772 6974 6528 6368 756e 6b29 0a20  p.write(chunk). 
+00004130: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00004140: 2e75 7064 6174 6528 6368 756e 6b29 0a0a  .update(chunk)..
+00004150: 2020 2020 2020 2020 6374 203d 2072 6573          ct = res
+00004160: 706f 6e73 652e 6865 6164 6572 732e 6765  ponse.headers.ge
+00004170: 7428 2263 6f6e 7465 6e74 2d74 7970 6522  t("content-type"
+00004180: 2c20 2222 292e 7370 6c69 7428 223b 222c  , "").split(";",
+00004190: 2031 295b 305d 0a20 2020 2065 7863 6570   1)[0].    excep
+000041a0: 7420 7265 7175 6573 7473 2e48 5454 5045  t requests.HTTPE
+000041b0: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
+000041c0: 2020 2072 6169 7365 2048 5454 5045 7272     raise HTTPErr
+000041d0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+000041e0: 2244 6174 6150 7573 6865 722b 2072 6563  "DataPusher+ rec
+000041f0: 6569 7665 6420 6120 6261 6420 4854 5450  eived a bad HTTP
+00004200: 2072 6573 706f 6e73 6520 7768 656e 2074   response when t
+00004210: 7279 696e 6720 746f 2064 6f77 6e6c 6f61  rying to downloa
+00004220: 6420 220a 2020 2020 2020 2020 2020 2020  d ".            
+00004230: 2274 6865 2064 6174 6120 6669 6c65 222c  "the data file",
+00004240: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00004250: 7475 735f 636f 6465 3d65 2e72 6573 706f  tus_code=e.respo
+00004260: 6e73 652e 7374 6174 7573 5f63 6f64 652c  nse.status_code,
+00004270: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
+00004280: 7565 7374 5f75 726c 3d75 726c 2c0a 2020  uest_url=url,.  
+00004290: 2020 2020 2020 2020 2020 7265 7370 6f6e            respon
+000042a0: 7365 3d65 2e72 6573 706f 6e73 652e 636f  se=e.response.co
+000042b0: 6e74 656e 742c 0a20 2020 2020 2020 2029  ntent,.        )
+000042c0: 0a20 2020 2065 7863 6570 7420 7265 7175  .    except requ
+000042d0: 6573 7473 2e52 6571 7565 7374 4578 6365  ests.RequestExce
+000042e0: 7074 696f 6e20 6173 2065 3a0a 2020 2020  ption as e:.    
+000042f0: 2020 2020 7261 6973 6520 4854 5450 4572      raise HTTPEr
+00004300: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00004310: 206d 6573 7361 6765 3d73 7472 2865 292c   message=str(e),
+00004320: 2073 7461 7475 735f 636f 6465 3d4e 6f6e   status_code=Non
+00004330: 652c 2072 6571 7565 7374 5f75 726c 3d75  e, request_url=u
+00004340: 726c 2c20 7265 7370 6f6e 7365 3d4e 6f6e  rl, response=Non
+00004350: 650a 2020 2020 2020 2020 290a 0a20 2020  e.        )..   
+00004360: 2066 696c 655f 6861 7368 203d 206d 2e68   file_hash = m.h
+00004370: 6578 6469 6765 7374 2829 0a20 2020 2074  exdigest().    t
+00004380: 6d70 2e73 6565 6b28 3029 0a0a 2020 2020  mp.seek(0)..    
+00004390: 6966 2028 0a20 2020 2020 2020 2072 6573  if (.        res
+000043a0: 6f75 7263 652e 6765 7428 2268 6173 6822  ource.get("hash"
+000043b0: 2920 3d3d 2066 696c 655f 6861 7368 0a20  ) == file_hash. 
+000043c0: 2020 2020 2020 2061 6e64 206e 6f74 2064         and not d
+000043d0: 6174 612e 6765 7428 2269 676e 6f72 655f  ata.get("ignore_
+000043e0: 6861 7368 2229 0a20 2020 2020 2020 2061  hash").        a
+000043f0: 6e64 206e 6f74 2063 6f6e 6669 672e 6765  nd not config.ge
+00004400: 7428 2249 474e 4f52 455f 4649 4c45 5f48  t("IGNORE_FILE_H
+00004410: 4153 4822 290a 2020 2020 293a 0a20 2020  ASH").    ):.   
+00004420: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
+00004430: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+00004440: 2022 5570 6c6f 6164 2073 6b69 7070 6564   "Upload skipped
+00004450: 2061 7320 7468 6520 6669 6c65 2068 6173   as the file has
+00004460: 6820 6861 736e 2774 2063 6861 6e67 6564  h hasn't changed
+00004470: 3a20 7b68 6173 687d 2e22 2e66 6f72 6d61  : {hash}.".forma
+00004480: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00004490: 2020 2068 6173 683d 6669 6c65 5f68 6173     hash=file_has
+000044a0: 680a 2020 2020 2020 2020 2020 2020 290a  h.            ).
+000044b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000044c0: 2020 7265 7475 726e 0a0a 2020 2020 7265    return..    re
+000044d0: 736f 7572 6365 5b22 6861 7368 225d 203d  source["hash"] =
+000044e0: 2066 696c 655f 6861 7368 0a0a 2020 2020   file_hash..    
+000044f0: 6665 7463 685f 656c 6170 7365 6420 3d20  fetch_elapsed = 
+00004500: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
+00004510: 7228 2920 2d20 7469 6d65 725f 7374 6172  r() - timer_star
+00004520: 740a 2020 2020 6c6f 6767 6572 2e69 6e66  t.    logger.inf
+00004530: 6f28 0a20 2020 2020 2020 2022 4665 7463  o(.        "Fetc
+00004540: 6865 6420 7b3a 2e32 4d42 7d20 6669 6c65  hed {:.2MB} file
+00004550: 2069 6e20 7b3a 2c2e 3266 7d20 7365 636f   in {:,.2f} seco
+00004560: 6e64 732e 222e 666f 726d 6174 280a 2020  nds.".format(.  
+00004570: 2020 2020 2020 2020 2020 4461 7461 5369            DataSi
+00004580: 7a65 286c 656e 6774 6829 2c20 6665 7463  ze(length), fetc
+00004590: 685f 656c 6170 7365 640a 2020 2020 2020  h_elapsed.      
+000045a0: 2020 290a 2020 2020 290a 0a20 2020 2023    ).    )..    #
+000045b0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+000045c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000045d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000045e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000045f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004600: 3d3d 3d3d 0a20 2020 2023 2041 4e41 4c59  ====.    # ANALY
+00004610: 5a45 2057 4954 4820 5153 560a 2020 2020  ZE WITH QSV.    
+00004620: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
+00004630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00004670: 3d3d 3d3d 3d0a 2020 2020 2320 5374 6172  =====.    # Star
+00004680: 7420 416e 616c 7973 6973 2075 7369 6e67  t Analysis using
+00004690: 2071 7376 2069 6e73 7465 6164 206f 6620   qsv instead of 
+000046a0: 6d65 7373 7974 6162 6c65 732c 2061 730a  messytables, as.
+000046b0: 2020 2020 2320 3129 2069 7473 2074 7970      # 1) its typ
+000046c0: 6520 696e 6665 7265 6e63 6573 2061 7265  e inferences are
+000046d0: 2062 756c 6c65 742d 7072 6f6f 6620 6e6f   bullet-proof no
+000046e0: 7420 6775 6573 7365 7320 6173 2069 7420  t guesses as it 
+000046f0: 7363 616e 7320 7468 6520 656e 7469 7265  scans the entire
+00004700: 2066 696c 652c 0a20 2020 2023 2032 2920   file,.    # 2) 
+00004710: 6974 7320 7375 7065 722d 6661 7374 2c20  its super-fast, 
+00004720: 616e 640a 2020 2020 2320 3329 2069 7420  and.    # 3) it 
+00004730: 6861 7320 6164 646c 2064 6174 612d 7772  has addl data-wr
+00004740: 616e 676c 696e 6720 6361 7061 6269 6c69  angling capabili
+00004750: 7469 6573 2077 6520 7573 6520 696e 2044  ties we use in D
+00004760: 502b 2028 652e 672e 2073 7461 7473 2c20  P+ (e.g. stats, 
+00004770: 6465 6475 702c 2065 7463 2e29 0a20 2020  dedup, etc.).   
+00004780: 2061 6e61 6c79 7369 735f 7374 6172 7420   analysis_start 
+00004790: 3d20 7469 6d65 2e70 6572 665f 636f 756e  = time.perf_coun
+000047a0: 7465 7228 290a 2020 2020 6c6f 6767 6572  ter().    logger
+000047b0: 2e69 6e66 6f28 2241 4e41 4c59 5a49 4e47  .info("ANALYZING
+000047c0: 2057 4954 4820 5153 562e 2e22 290a 0a20   WITH QSV..").. 
+000047d0: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
+000047e0: 2d2d 2d2d 2d2d 2069 7320 6974 2061 2073  ------ is it a s
+000047f0: 7072 6561 6473 6865 6574 3f20 2d2d 2d2d  preadsheet? ----
+00004800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00004810: 2320 6368 6563 6b20 636f 6e74 656e 7420  # check content 
+00004820: 7479 7065 206f 7220 6669 6c65 2065 7874  type or file ext
+00004830: 656e 7369 6f6e 2069 6620 6974 7320 6120  ension if its a 
+00004840: 7370 7265 6164 7368 6565 740a 2020 2020  spreadsheet.    
+00004850: 7370 7265 6164 7368 6565 745f 6578 7465  spreadsheet_exte
+00004860: 6e73 696f 6e73 203d 205b 2258 4c53 222c  nsions = ["XLS",
+00004870: 2022 584c 5358 222c 2022 4f44 5322 2c20   "XLSX", "ODS", 
+00004880: 2258 4c53 4d22 2c20 2258 4c53 4222 5d0a  "XLSM", "XLSB"].
+00004890: 2020 2020 666f 726d 6174 203d 2072 6573      format = res
+000048a0: 6f75 7263 652e 6765 7428 2266 6f72 6d61  ource.get("forma
+000048b0: 7422 292e 7570 7065 7228 290a 2020 2020  t").upper().    
+000048c0: 6966 2066 6f72 6d61 7420 696e 2073 7072  if format in spr
+000048d0: 6561 6473 6865 6574 5f65 7874 656e 7369  eadsheet_extensi
+000048e0: 6f6e 733a 0a20 2020 2020 2020 2023 2069  ons:.        # i
+000048f0: 6620 736f 2c20 6578 706f 7274 2073 7072  f so, export spr
+00004900: 6561 6473 6865 6574 2061 7320 6120 4353  eadsheet as a CS
+00004910: 5620 6669 6c65 0a20 2020 2020 2020 2064  V file.        d
+00004920: 6566 6175 6c74 5f65 7863 656c 5f73 6865  efault_excel_she
+00004930: 6574 203d 2063 6f6e 6669 672e 6765 7428  et = config.get(
+00004940: 2244 4546 4155 4c54 5f45 5843 454c 5f53  "DEFAULT_EXCEL_S
+00004950: 4845 4554 2229 0a20 2020 2020 2020 206c  HEET").        l
+00004960: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
+00004970: 2020 2020 2020 2020 2243 6f6e 7665 7274          "Convert
+00004980: 696e 6720 7b7d 2073 6865 6574 207b 7d20  ing {} sheet {} 
+00004990: 746f 2043 5356 2e2e 2e22 2e66 6f72 6d61  to CSV...".forma
+000049a0: 7428 666f 726d 6174 2c20 6465 6661 756c  t(format, defaul
+000049b0: 745f 6578 6365 6c5f 7368 6565 7429 0a20  t_excel_sheet). 
+000049c0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000049d0: 2023 2066 6972 7374 2c20 7765 206e 6565   # first, we nee
+000049e0: 6420 6120 7465 6d70 6f72 6172 7920 7370  d a temporary sp
+000049f0: 7265 6164 7368 6565 7420 6669 6c65 6e61  readsheet filena
+00004a00: 6d65 2077 6974 6820 7468 6520 7269 6768  me with the righ
+00004a10: 7420 6669 6c65 2065 7874 656e 7369 6f6e  t file extension
+00004a20: 0a20 2020 2020 2020 2023 2077 6520 6f6e  .        # we on
+00004a30: 6c79 206e 6565 6420 7468 6520 6669 6c65  ly need the file
+00004a40: 6e61 6d65 2074 686f 7567 682c 2074 6861  name though, tha
+00004a50: 7427 7320 7768 7920 7765 2072 656d 6f76  t's why we remov
+00004a60: 6520 6974 0a20 2020 2020 2020 2023 2061  e it.        # a
+00004a70: 6e64 2063 7265 6174 6520 6120 6861 7264  nd create a hard
+00004a80: 6c69 6e6b 2074 6f20 7468 6520 6669 6c65  link to the file
+00004a90: 2077 6520 676f 7420 6672 6f6d 2043 4b41   we got from CKA
+00004aa0: 4e0a 2020 2020 2020 2020 7173 765f 7370  N.        qsv_sp
+00004ab0: 7265 6164 7368 6565 7420 3d20 7465 6d70  readsheet = temp
+00004ac0: 6669 6c65 2e4e 616d 6564 5465 6d70 6f72  file.NamedTempor
+00004ad0: 6172 7946 696c 6528 7375 6666 6978 3d22  aryFile(suffix="
+00004ae0: 2e22 202b 2066 6f72 6d61 7429 0a20 2020  ." + format).   
+00004af0: 2020 2020 206f 732e 7265 6d6f 7665 2871       os.remove(q
+00004b00: 7376 5f73 7072 6561 6473 6865 6574 2e6e  sv_spreadsheet.n
+00004b10: 616d 6529 0a20 2020 2020 2020 206f 732e  ame).        os.
+00004b20: 6c69 6e6b 2874 6d70 2e6e 616d 652c 2071  link(tmp.name, q
+00004b30: 7376 5f73 7072 6561 6473 6865 6574 2e6e  sv_spreadsheet.n
+00004b40: 616d 6529 0a0a 2020 2020 2020 2020 2320  ame)..        # 
+00004b50: 7275 6e20 6071 7376 2065 7863 656c 6020  run `qsv excel` 
+00004b60: 616e 6420 6578 706f 7274 2069 7420 746f  and export it to
+00004b70: 2061 2043 5356 0a20 2020 2020 2020 2023   a CSV.        #
+00004b80: 2075 7365 202d 2d74 7269 6d20 6f70 7469   use --trim opti
+00004b90: 6f6e 2074 6f20 7472 696d 2063 6f6c 756d  on to trim colum
+00004ba0: 6e20 6e61 6d65 7320 616e 6420 7468 6520  n names and the 
+00004bb0: 6461 7461 0a20 2020 2020 2020 2071 7376  data.        qsv
+00004bc0: 5f65 7863 656c 5f63 7376 203d 2074 656d  _excel_csv = tem
+00004bd0: 7066 696c 652e 4e61 6d65 6454 656d 706f  pfile.NamedTempo
+00004be0: 7261 7279 4669 6c65 2873 7566 6669 783d  raryFile(suffix=
+00004bf0: 222e 6373 7622 290a 2020 2020 2020 2020  ".csv").        
+00004c00: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00004c10: 2071 7376 5f65 7863 656c 203d 2073 7562   qsv_excel = sub
+00004c20: 7072 6f63 6573 732e 7275 6e28 0a20 2020  process.run(.   
+00004c30: 2020 2020 2020 2020 2020 2020 205b 0a20               [. 
+00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c50: 2020 2071 7376 5f62 696e 2c0a 2020 2020     qsv_bin,.    
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2265 7863 656c 222c 0a20 2020 2020 2020  "excel",.       
+00004c80: 2020 2020 2020 2020 2020 2020 2071 7376               qsv
+00004c90: 5f73 7072 6561 6473 6865 6574 2e6e 616d  _spreadsheet.nam
+00004ca0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00004cb0: 2020 2020 2020 2022 2d2d 7368 6565 7422         "--sheet"
+00004cc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004cd0: 2020 2020 2020 7374 7228 6465 6661 756c        str(defaul
+00004ce0: 745f 6578 6365 6c5f 7368 6565 7429 2c0a  t_excel_sheet),.
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 2020 2020 222d 2d74 7269 6d22 2c0a 2020      "--trim",.  
+00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d20: 2020 222d 2d6f 7574 7075 7422 2c0a 2020    "--output",.  
+00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d40: 2020 7173 765f 6578 6365 6c5f 6373 762e    qsv_excel_csv.
+00004d50: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00004d60: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00004d70: 2020 2020 2020 2020 2063 6865 636b 3d54           check=T
+00004d80: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00004d90: 2020 2020 2063 6170 7475 7265 5f6f 7574       capture_out
+00004da0: 7075 743d 5472 7565 2c0a 2020 2020 2020  put=True,.      
+00004db0: 2020 2020 2020 2020 2020 7465 7874 3d54            text=T
+00004dc0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00004dd0: 2029 0a20 2020 2020 2020 2065 7863 6570   ).        excep
+00004de0: 7420 7375 6270 726f 6365 7373 2e43 616c  t subprocess.Cal
+00004df0: 6c65 6450 726f 6365 7373 4572 726f 7220  ledProcessError 
+00004e00: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00004e10: 2020 6c6f 6767 6572 2e65 7272 6f72 280a    logger.error(.
+00004e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e30: 2255 706c 6f61 6420 6162 6f72 7465 642e  "Upload aborted.
+00004e40: 2043 616e 6e6f 7420 6578 706f 7274 2073   Cannot export s
+00004e50: 7072 6561 6473 6865 6574 283f 2920 746f  preadsheet(?) to
+00004e60: 2043 5356 3a20 7b7d 222e 666f 726d 6174   CSV: {}".format
+00004e70: 2865 290a 2020 2020 2020 2020 2020 2020  (e).            
+00004e80: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00004e90: 2069 7420 6861 6420 6120 7370 7265 6164   it had a spread
+00004ea0: 7368 6565 7420 6578 7465 6e73 696f 6e20  sheet extension 
+00004eb0: 6275 7420 6071 7376 2065 7863 656c 6020  but `qsv excel` 
+00004ec0: 6661 696c 6564 2c0a 2020 2020 2020 2020  failed,.        
+00004ed0: 2020 2020 2320 6765 7420 736f 6d65 2066      # get some f
+00004ee0: 696c 6520 696e 666f 2061 6e64 206c 6f67  ile info and log
+00004ef0: 2069 7420 6279 2072 756e 6e69 6e67 2060   it by running `
+00004f00: 6669 6c65 600a 2020 2020 2020 2020 2020  file`.          
+00004f10: 2020 2320 6a75 7374 2069 6e20 6361 7365    # just in case
+00004f20: 2074 6865 2066 696c 6520 6973 206e 6f74   the file is not
+00004f30: 2061 6374 7561 6c6c 7920 6120 7370 7265   actually a spre
+00004f40: 6164 7368 6565 7420 6f72 2069 7320 656e  adsheet or is en
+00004f50: 6372 7970 7465 640a 2020 2020 2020 2020  crypted.        
+00004f60: 2020 2020 2320 736f 2074 6865 2075 7365      # so the use
+00004f70: 7220 6861 7320 736f 6d65 2061 6374 696f  r has some actio
+00004f80: 6e61 626c 6520 696e 666f 0a20 2020 2020  nable info.     
+00004f90: 2020 2020 2020 2066 696c 655f 666f 726d         file_form
+00004fa0: 6174 203d 2073 7562 7072 6f63 6573 732e  at = subprocess.
+00004fb0: 7275 6e28 0a20 2020 2020 2020 2020 2020  run(.           
+00004fc0: 2020 2020 205b 6669 6c65 5f62 696e 2c20       [file_bin, 
+00004fd0: 7173 765f 7370 7265 6164 7368 6565 742e  qsv_spreadsheet.
+00004fe0: 6e61 6d65 5d2c 0a20 2020 2020 2020 2020  name],.         
+00004ff0: 2020 2020 2020 2063 6865 636b 3d54 7275         check=Tru
+00005000: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00005010: 2020 2063 6170 7475 7265 5f6f 7574 7075     capture_outpu
+00005020: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
+00005030: 2020 2020 2020 2020 7465 7874 3d54 7275          text=Tru
+00005040: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+00005050: 0a0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00005060: 6767 6572 2e77 6172 6e69 6e67 280a 2020  gger.warning(.  
+00005070: 2020 2020 2020 2020 2020 2020 2020 2249                "I
+00005080: 7320 7468 6520 6669 6c65 2065 6e63 7279  s the file encry
+00005090: 7074 6564 206f 7220 6973 206e 6f74 2061  pted or is not a
+000050a0: 2073 7072 6561 6473 6865 6574 3f5c 6e46   spreadsheet?\nF
+000050b0: 494c 4520 4154 5452 4942 5554 4553 3a20  ILE ATTRIBUTES: 
+000050c0: 7b7d 222e 666f 726d 6174 280a 2020 2020  {}".format(.    
+000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050e0: 6669 6c65 5f66 6f72 6d61 742e 7374 646f  file_format.stdo
+000050f0: 7574 0a20 2020 2020 2020 2020 2020 2020  ut.             
+00005100: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00005110: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00005120: 7265 7475 726e 0a20 2020 2020 2020 2071  return.        q
+00005130: 7376 5f73 7072 6561 6473 6865 6574 2e63  sv_spreadsheet.c
+00005140: 6c6f 7365 2829 0a20 2020 2020 2020 2065  lose().        e
+00005150: 7863 656c 5f65 7870 6f72 745f 6d73 6720  xcel_export_msg 
+00005160: 3d20 7173 765f 6578 6365 6c2e 7374 6465  = qsv_excel.stde
+00005170: 7272 0a20 2020 2020 2020 206c 6f67 6765  rr.        logge
+00005180: 722e 696e 666f 2822 7b7d 2e2e 2e22 2e66  r.info("{}...".f
+00005190: 6f72 6d61 7428 6578 6365 6c5f 6578 706f  ormat(excel_expo
+000051a0: 7274 5f6d 7367 2929 0a20 2020 2020 2020  rt_msg)).       
+000051b0: 2074 6d70 203d 2071 7376 5f65 7863 656c   tmp = qsv_excel
+000051c0: 5f63 7376 0a20 2020 2065 6c73 653a 0a20  _csv.    else:. 
+000051d0: 2020 2020 2020 2023 202d 2d2d 2d2d 2d2d         # -------
+000051e0: 2d2d 2d2d 2d2d 2d20 6974 7320 6e6f 7420  ------- its not 
+000051f0: 6120 7370 7265 6164 7368 6565 742c 2069  a spreadsheet, i
+00005200: 7473 2061 2043 5356 2f54 5356 2f54 4142  ts a CSV/TSV/TAB
+00005210: 2066 696c 6520 2d2d 2d2d 2d2d 2d2d 2d2d   file ----------
+00005220: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2320  -----.        # 
+00005230: 4e6f 726d 616c 697a 6520 2620 7472 616e  Normalize & tran
+00005240: 7363 6f64 6520 746f 2055 5446 2d38 2075  scode to UTF-8 u
+00005250: 7369 6e67 2060 7173 7620 696e 7075 7460  sing `qsv input`
+00005260: 2e20 5765 206e 6565 6420 746f 206e 6f72  . We need to nor
+00005270: 6d61 6c69 7a65 2061 730a 2020 2020 2020  malize as.      
+00005280: 2020 2320 6974 2063 6f75 6c64 2062 6520    # it could be 
+00005290: 6120 4353 562f 5453 562f 5441 4220 6469  a CSV/TSV/TAB di
+000052a0: 616c 6563 7420 7769 7468 2064 6966 6665  alect with diffe
+000052b0: 7269 6e67 2064 656c 696d 6974 6572 732c  ring delimiters,
+000052c0: 2071 756f 7469 6e67 2c20 6574 632e 0a20   quoting, etc.. 
+000052d0: 2020 2020 2020 2023 2055 7369 6e67 2071         # Using q
+000052e0: 7376 2069 6e70 7574 2773 202d 2d6f 7574  sv input's --out
+000052f0: 7075 7420 6f70 7469 6f6e 2061 6c73 6f20  put option also 
+00005300: 6175 746f 2d74 7261 6e73 636f 6465 7320  auto-transcodes 
+00005310: 746f 2055 5446 2d38 2e0a 2020 2020 2020  to UTF-8..      
+00005320: 2020 2320 4e6f 7465 2074 6861 7420 7765    # Note that we
+00005330: 206f 6e6c 7920 6368 616e 6765 2074 6865   only change the
+00005340: 2077 6f72 6b66 696c 652c 2074 6865 2072   workfile, the r
+00005350: 6573 6f75 7263 6520 6669 6c65 2069 7473  esource file its
+00005360: 656c 6620 6973 2075 6e63 6861 6e67 6564  elf is unchanged
+00005370: 2e0a 0a20 2020 2020 2020 2023 202d 2d2d  ...        # ---
+00005380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005390: 204e 6f72 6d61 6c69 7a65 2074 6f20 4353   Normalize to CS
+000053a0: 5620 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  V --------------
+000053b0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000053c0: 7173 765f 696e 7075 745f 6373 7620 3d20  qsv_input_csv = 
+000053d0: 7465 6d70 6669 6c65 2e4e 616d 6564 5465  tempfile.NamedTe
+000053e0: 6d70 6f72 6172 7946 696c 6528 7375 6666  mporaryFile(suff
+000053f0: 6978 3d22 2e63 7376 2229 0a20 2020 2020  ix=".csv").     
+00005400: 2020 2069 6620 666f 726d 6174 2e75 7070     if format.upp
+00005410: 6572 2829 203d 3d20 2243 5356 223a 0a20  er() == "CSV":. 
+00005420: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00005430: 722e 696e 666f 2822 4e6f 726d 616c 697a  r.info("Normaliz
+00005440: 696e 672f 5554 462d 3820 7472 616e 7363  ing/UTF-8 transc
+00005450: 6f64 696e 6720 7b7d 2e2e 2e22 2e66 6f72  oding {}...".for
+00005460: 6d61 7428 666f 726d 6174 2929 0a20 2020  mat(format)).   
+00005470: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00005480: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00005490: 666f 2822 4e6f 726d 616c 697a 696e 672f  fo("Normalizing/
+000054a0: 5554 462d 3820 7472 616e 7363 6f64 696e  UTF-8 transcodin
+000054b0: 6720 7b7d 2074 6f20 4353 562e 2e2e 222e  g {} to CSV...".
+000054c0: 666f 726d 6174 2866 6f72 6d61 7429 290a  format(format)).
+000054d0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+000054e0: 2020 2020 2020 2020 2071 7376 5f69 6e70           qsv_inp
+000054f0: 7574 203d 2073 7562 7072 6f63 6573 732e  ut = subprocess.
+00005500: 7275 6e28 0a20 2020 2020 2020 2020 2020  run(.           
+00005510: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00005520: 2020 2020 2020 2020 2020 2071 7376 5f62             qsv_b
+00005530: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+00005540: 2020 2020 2020 2020 2269 6e70 7574 222c          "input",
+00005550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005560: 2020 2020 2074 6d70 2e6e 616d 652c 0a20       tmp.name,. 
+00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005580: 2020 2022 2d2d 7472 696d 2d68 6561 6465     "--trim-heade
+00005590: 7273 222c 0a20 2020 2020 2020 2020 2020  rs",.           
+000055a0: 2020 2020 2020 2020 2022 2d2d 6f75 7470           "--outp
+000055b0: 7574 222c 0a20 2020 2020 2020 2020 2020  ut",.           
+000055c0: 2020 2020 2020 2020 2071 7376 5f69 6e70           qsv_inp
+000055d0: 7574 5f63 7376 2e6e 616d 652c 0a20 2020  ut_csv.name,.   
+000055e0: 2020 2020 2020 2020 2020 2020 205d 2c0a               ],.
+000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005600: 6368 6563 6b3d 5472 7565 2c0a 2020 2020  check=True,.    
+00005610: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00005620: 2020 6578 6365 7074 2073 7562 7072 6f63    except subproc
+00005630: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
+00005640: 7345 7272 6f72 2061 7320 653a 0a20 2020  sError as e:.   
+00005650: 2020 2020 2020 2020 2023 2072 6574 7572           # retur
+00005660: 6e20 6173 2077 6520 6361 6e27 7420 7075  n as we can't pu
+00005670: 7368 2061 6e20 696e 7661 6c69 6420 4353  sh an invalid CS
+00005680: 5620 6669 6c65 0a20 2020 2020 2020 2020  V file.         
+00005690: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
+000056a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000056b0: 2022 4a6f 6220 6162 6f72 7465 6420 6173   "Job aborted as
+000056c0: 2074 6865 2066 696c 6520 6361 6e6e 6f74   the file cannot
+000056d0: 2062 6520 6e6f 726d 616c 697a 6564 2f74   be normalized/t
+000056e0: 7261 6e73 636f 6465 643a 207b 7d2e 222e  ranscoded: {}.".
+000056f0: 666f 726d 6174 2865 290a 2020 2020 2020  format(e).      
+00005700: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00005710: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00005720: 2020 2074 6d70 203d 2071 7376 5f69 6e70     tmp = qsv_inp
+00005730: 7574 5f63 7376 0a20 2020 2020 2020 206c  ut_csv.        l
+00005740: 6f67 6765 722e 696e 666f 2822 4e6f 726d  ogger.info("Norm
+00005750: 616c 697a 6564 2026 2074 7261 6e73 636f  alized & transco
+00005760: 6465 642e 2e2e 2229 0a0a 2020 2020 2320  ded...")..    # 
+00005770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005790: 2d2d 2d2d 2d20 5661 6c69 6461 7465 2043  ----- Validate C
+000057a0: 5356 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  SV -------------
+000057b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000057c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2320  ---------.    # 
+000057d0: 5275 6e20 616e 2052 4643 3431 3830 2063  Run an RFC4180 c
+000057e0: 6865 636b 2077 6974 6820 6071 7376 2076  heck with `qsv v
+000057f0: 616c 6964 6174 6560 2061 6761 696e 7374  alidate` against
+00005800: 2074 6865 206e 6f72 6d61 6c69 7a65 642c   the normalized,
+00005810: 2055 5446 2d38 2065 6e63 6f64 6564 2043   UTF-8 encoded C
+00005820: 5356 2066 696c 652e 0a20 2020 2023 2045  SV file..    # E
+00005830: 7665 6e20 6578 6365 6c20 6578 706f 7274  ven excel export
+00005840: 6564 2043 5356 7320 6361 6e20 6265 2070  ed CSVs can be p
+00005850: 6f74 656e 7469 616c 6c79 2069 6e76 616c  otentially inval
+00005860: 6964 2c20 6173 2069 7420 616c 6c6f 7773  id, as it allows
+00005870: 2074 6865 2065 7870 6f72 7420 6f66 2022   the export of "
+00005880: 666c 6578 6962 6c65 220a 2020 2020 2320  flexible".    # 
+00005890: 4353 5673 202d 2069 2e65 2e20 726f 7773  CSVs - i.e. rows
+000058a0: 206d 6179 2068 6176 6520 6469 6666 6572   may have differ
+000058b0: 656e 7420 636f 6c75 6d6e 2063 6f75 6e74  ent column count
+000058c0: 732e 0a20 2020 2023 2049 6620 6974 2070  s..    # If it p
+000058d0: 6173 7365 7320 7661 6c69 6461 7469 6f6e  asses validation
+000058e0: 2c20 7765 2063 616e 2068 616e 646c 6520  , we can handle 
+000058f0: 6974 2077 6974 6820 636f 6e66 6964 656e  it with confiden
+00005900: 6365 2064 6f77 6e73 7472 6561 6d20 6173  ce downstream as
+00005910: 2061 2022 6e6f 726d 616c 2220 4353 562e   a "normal" CSV.
+00005920: 0a20 2020 206c 6f67 6765 722e 696e 666f  .    logger.info
+00005930: 2822 5661 6c69 6461 7469 6e67 2043 5356  ("Validating CSV
+00005940: 2e2e 2e22 290a 2020 2020 7472 793a 0a20  ...").    try:. 
+00005950: 2020 2020 2020 2071 7376 5f76 616c 6964         qsv_valid
+00005960: 6174 6520 3d20 7375 6270 726f 6365 7373  ate = subprocess
+00005970: 2e72 756e 280a 2020 2020 2020 2020 2020  .run(.          
+00005980: 2020 5b71 7376 5f62 696e 2c20 2276 616c    [qsv_bin, "val
+00005990: 6964 6174 6522 2c20 746d 702e 6e61 6d65  idate", tmp.name
+000059a0: 5d2c 2063 6865 636b 3d54 7275 652c 2063  ], check=True, c
+000059b0: 6170 7475 7265 5f6f 7574 7075 743d 5472  apture_output=Tr
+000059c0: 7565 2c20 7465 7874 3d54 7275 650a 2020  ue, text=True.  
+000059d0: 2020 2020 2020 290a 2020 2020 6578 6365        ).    exce
+000059e0: 7074 2073 7562 7072 6f63 6573 732e 4361  pt subprocess.Ca
+000059f0: 6c6c 6564 5072 6f63 6573 7345 7272 6f72  lledProcessError
+00005a00: 2061 7320 653a 0a20 2020 2020 2020 2023   as e:.        #
+00005a10: 2072 6574 7572 6e20 6173 2077 6520 6361   return as we ca
+00005a20: 6e27 7420 7075 7368 2061 6e20 696e 7661  n't push an inva
+00005a30: 6c69 6420 4353 5620 6669 6c65 0a20 2020  lid CSV file.   
+00005a40: 2020 2020 2076 616c 6964 6174 655f 6572       validate_er
+00005a50: 726f 725f 6d73 6720 3d20 7173 765f 7661  ror_msg = qsv_va
+00005a60: 6c69 6461 7465 2e73 7464 6572 720a 2020  lidate.stderr.  
+00005a70: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
+00005a80: 6f72 2822 496e 7661 6c69 6420 4353 5621  or("Invalid CSV!
+00005a90: 204a 6f62 2061 626f 7274 6564 3a20 7b7d   Job aborted: {}
+00005aa0: 2e22 2e66 6f72 6d61 7428 7661 6c69 6461  .".format(valida
+00005ab0: 7465 5f65 7272 6f72 5f6d 7367 2929 0a20  te_error_msg)). 
+00005ac0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00005ad0: 2020 6c6f 6767 6572 2e69 6e66 6f28 2257    logger.info("W
+00005ae0: 656c 6c2d 666f 726d 6564 2c20 7661 6c69  ell-formed, vali
+00005af0: 6420 4353 5620 6669 6c65 2063 6f6e 6669  d CSV file confi
+00005b00: 726d 6564 2e2e 2e22 290a 0a20 2020 2023  rmed...")..    #
+00005b10: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00005b20: 2d2d 2d2d 2d2d 2053 6f72 7463 6865 636b  ------ Sortcheck
+00005b30: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00005b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00005b50: 2320 6966 2053 4f52 545f 414e 445f 4455  # if SORT_AND_DU
+00005b60: 5045 5f43 4845 434b 2069 7320 5472 7565  PE_CHECK is True
+00005b70: 206f 7220 4445 4455 5020 6973 2054 7275   or DEDUP is Tru
+00005b80: 650a 2020 2020 2320 6368 6563 6b20 6966  e.    # check if
+00005b90: 2074 6865 2066 696c 6520 6973 2073 6f72   the file is sor
+00005ba0: 7465 6420 616e 6420 6966 2069 7420 6861  ted and if it ha
+00005bb0: 7320 6475 706c 6963 6174 6573 0a20 2020  s duplicates.   
+00005bc0: 2023 2067 6574 2074 6865 2072 6563 6f72   # get the recor
+00005bd0: 6420 636f 756e 742c 2075 6e73 6f72 7465  d count, unsorte
+00005be0: 6420 6272 6561 6b73 2061 6e64 2064 7570  d breaks and dup
+00005bf0: 6c69 6361 7465 2063 6f75 6e74 2061 7320  licate count as 
+00005c00: 7765 6c6c 0a20 2020 2073 6f72 745f 616e  well.    sort_an
+00005c10: 645f 6475 7065 5f63 6865 636b 203d 2063  d_dupe_check = c
+00005c20: 6f6e 6669 672e 6765 7428 2253 4f52 545f  onfig.get("SORT_
+00005c30: 414e 445f 4455 5045 5f43 4845 434b 2229  AND_DUPE_CHECK")
+00005c40: 0a20 2020 2064 6564 7570 203d 2063 6f6e  .    dedup = con
+00005c50: 6669 672e 6765 7428 2244 4544 5550 2229  fig.get("DEDUP")
+00005c60: 0a0a 2020 2020 6966 2073 6f72 745f 616e  ..    if sort_an
+00005c70: 645f 6475 7065 5f63 6865 636b 206f 7220  d_dupe_check or 
+00005c80: 6465 6475 703a 0a20 2020 2020 2020 206c  dedup:.        l
+00005c90: 6f67 6765 722e 696e 666f 2822 4368 6563  ogger.info("Chec
+00005ca0: 6b69 6e67 2066 6f72 2064 7570 6c69 6361  king for duplica
+00005cb0: 7465 7320 616e 6420 6966 2074 6865 2043  tes and if the C
+00005cc0: 5356 2069 7320 736f 7274 6564 2e2e 2e22  SV is sorted..."
+00005cd0: 290a 2020 2020 2020 2020 7472 793a 0a20  ).        try:. 
+00005ce0: 2020 2020 2020 2020 2020 2071 7376 5f73             qsv_s
+00005cf0: 6f72 7463 6865 636b 203d 2073 7562 7072  ortcheck = subpr
+00005d00: 6f63 6573 732e 7275 6e28 0a20 2020 2020  ocess.run(.     
+00005d10: 2020 2020 2020 2020 2020 205b 7173 765f             [qsv_
+00005d20: 6269 6e2c 2022 736f 7274 6368 6563 6b22  bin, "sortcheck"
+00005d30: 2c20 746d 702e 6e61 6d65 2c20 222d 2d6a  , tmp.name, "--j
+00005d40: 736f 6e22 5d2c 0a20 2020 2020 2020 2020  son"],.         
+00005d50: 2020 2020 2020 2063 6170 7475 7265 5f6f         capture_o
+00005d60: 7574 7075 743d 5472 7565 2c0a 2020 2020  utput=True,.    
+00005d70: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00005d80: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00005d90: 2020 2029 0a20 2020 2020 2020 2065 7863     ).        exc
+00005da0: 6570 7420 7375 6270 726f 6365 7373 2e43  ept subprocess.C
+00005db0: 616c 6c65 6450 726f 6365 7373 4572 726f  alledProcessErro
+00005dc0: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
+00005dd0: 2020 2020 7261 6973 6520 7574 696c 2e4a      raise util.J
+00005de0: 6f62 4572 726f 7228 2253 6f72 7463 6865  obError("Sortche
+00005df0: 636b 2065 7272 6f72 3a20 7b7d 222e 666f  ck error: {}".fo
+00005e00: 726d 6174 2865 2929 0a20 2020 2020 2020  rmat(e)).       
+00005e10: 2073 6f72 7463 6865 636b 5f6a 736f 6e20   sortcheck_json 
+00005e20: 3d20 6a73 6f6e 2e6c 6f61 6473 2873 7472  = json.loads(str
+00005e30: 2871 7376 5f73 6f72 7463 6865 636b 2e73  (qsv_sortcheck.s
+00005e40: 7464 6f75 7429 290a 2020 2020 2020 2020  tdout)).        
+00005e50: 6973 5f73 6f72 7465 6420 3d20 736f 7274  is_sorted = sort
+00005e60: 6368 6563 6b5f 6a73 6f6e 5b22 736f 7274  check_json["sort
+00005e70: 6564 225d 0a20 2020 2020 2020 2072 6563  ed"].        rec
+00005e80: 6f72 645f 636f 756e 7420 3d20 696e 7428  ord_count = int(
+00005e90: 736f 7274 6368 6563 6b5f 6a73 6f6e 5b22  sortcheck_json["
+00005ea0: 7265 636f 7264 5f63 6f75 6e74 225d 290a  record_count"]).
+00005eb0: 2020 2020 2020 2020 756e 736f 7274 6564          unsorted
+00005ec0: 5f62 7265 616b 7320 3d20 696e 7428 736f  _breaks = int(so
+00005ed0: 7274 6368 6563 6b5f 6a73 6f6e 5b22 756e  rtcheck_json["un
+00005ee0: 736f 7274 6564 5f62 7265 616b 7322 5d29  sorted_breaks"])
+00005ef0: 0a20 2020 2020 2020 2064 7570 655f 636f  .        dupe_co
+00005f00: 756e 7420 3d20 696e 7428 736f 7274 6368  unt = int(sortch
+00005f10: 6563 6b5f 6a73 6f6e 5b22 6475 7065 5f63  eck_json["dupe_c
+00005f20: 6f75 6e74 225d 290a 2020 2020 2020 2020  ount"]).        
+00005f30: 736f 7274 6368 6563 6b5f 6d73 6720 3d20  sortcheck_msg = 
+00005f40: 2253 6f72 7465 643a 207b 7d3b 2055 6e73  "Sorted: {}; Uns
+00005f50: 6f72 7465 6420 6272 6561 6b73 3a20 7b3a  orted breaks: {:
+00005f60: 2c7d 222e 666f 726d 6174 280a 2020 2020  ,}".format(.    
+00005f70: 2020 2020 2020 2020 6973 5f73 6f72 7465          is_sorte
+00005f80: 642c 2075 6e73 6f72 7465 645f 6272 6561  d, unsorted_brea
+00005f90: 6b73 0a20 2020 2020 2020 2029 0a20 2020  ks.        ).   
+00005fa0: 2020 2020 2023 2064 7570 6520 636f 756e       # dupe coun
+00005fb0: 7420 6973 206f 6e6c 7920 7265 6c65 7661  t is only releva
+00005fc0: 6e74 2069 6620 7468 6520 6669 6c65 2069  nt if the file i
+00005fd0: 7320 736f 7274 6564 0a20 2020 2020 2020  s sorted.       
+00005fe0: 2069 6620 6973 5f73 6f72 7465 6420 616e   if is_sorted an
+00005ff0: 6420 6475 7065 5f63 6f75 6e74 203e 2030  d dupe_count > 0
+00006000: 3a0a 2020 2020 2020 2020 2020 2020 736f  :.            so
+00006010: 7274 6368 6563 6b5f 6d73 6720 3d20 736f  rtcheck_msg = so
+00006020: 7274 6368 6563 6b5f 6d73 6720 2b20 2220  rtcheck_msg + " 
+00006030: 4475 706c 6963 6174 6573 3a20 7b3a 2c7d  Duplicates: {:,}
+00006040: 222e 666f 726d 6174 2864 7570 655f 636f  ".format(dupe_co
+00006050: 756e 7429 0a20 2020 2020 2020 206c 6f67  unt).        log
+00006060: 6765 722e 696e 666f 2873 6f72 7463 6865  ger.info(sortche
+00006070: 636b 5f6d 7367 290a 0a20 2020 2023 202d  ck_msg)..    # -
+00006080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2044  -------------- D
+00006090: 6f20 7765 206e 6565 6420 746f 2064 6564  o we need to ded
+000060a0: 7570 3f20 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  up? ------------
+000060b0: 2d2d 2d2d 2d2d 0a20 2020 2023 206e 6f74  ------.    # not
+000060c0: 6520 7468 6174 2064 6564 7570 696e 6720  e that deduping 
+000060d0: 616c 736f 2065 6e64 7320 7570 2063 7265  also ends up cre
+000060e0: 6174 696e 6720 6120 736f 7274 6564 2043  ating a sorted C
+000060f0: 5356 0a20 2020 2069 6620 6465 6475 7020  SV.    if dedup 
+00006100: 616e 6420 6475 7065 5f63 6f75 6e74 203e  and dupe_count >
+00006110: 2030 3a0a 2020 2020 2020 2020 7173 765f   0:.        qsv_
+00006120: 6465 6475 705f 6373 7620 3d20 7465 6d70  dedup_csv = temp
+00006130: 6669 6c65 2e4e 616d 6564 5465 6d70 6f72  file.NamedTempor
+00006140: 6172 7946 696c 6528 7375 6666 6978 3d22  aryFile(suffix="
+00006150: 2e63 7376 2229 0a20 2020 2020 2020 206c  .csv").        l
+00006160: 6f67 6765 722e 696e 666f 2822 7b3a 2e7d  ogger.info("{:.}
+00006170: 2064 7570 6c69 6361 7465 2072 6f77 7320   duplicate rows 
+00006180: 666f 756e 642e 2044 6564 7570 696e 672e  found. Deduping.
+00006190: 2e2e 222e 666f 726d 6174 2864 7570 655f  ..".format(dupe_
+000061a0: 636f 756e 7429 290a 2020 2020 2020 2020  count)).        
+000061b0: 7173 765f 6465 6475 705f 636d 6420 3d20  qsv_dedup_cmd = 
+000061c0: 5b71 7376 5f62 696e 2c20 2264 6564 7570  [qsv_bin, "dedup
+000061d0: 222c 2074 6d70 2e6e 616d 652c 2022 2d2d  ", tmp.name, "--
+000061e0: 6f75 7470 7574 222c 2071 7376 5f64 6564  output", qsv_ded
+000061f0: 7570 5f63 7376 2e6e 616d 655d 0a0a 2020  up_csv.name]..  
+00006200: 2020 2020 2020 2320 6966 2074 6865 2066        # if the f
+00006210: 696c 6520 6973 2061 6c72 6561 6479 2073  ile is already s
+00006220: 6f72 7465 642c 0a20 2020 2020 2020 2023  orted,.        #
+00006230: 2077 6520 6361 6e20 7361 7665 2061 206c   we can save a l
+00006240: 6f74 206f 6620 7469 6d65 2062 7920 7061  ot of time by pa
+00006250: 7373 696e 6720 7468 6520 2d2d 736f 7274  ssing the --sort
+00006260: 6564 2066 6c61 670a 2020 2020 2020 2020  ed flag.        
+00006270: 2320 7765 2061 6c73 6f20 6765 7420 746f  # we also get to
+00006280: 2022 7374 7265 616d 2220 7468 6520 6669   "stream" the fi
+00006290: 6c65 2061 6e64 206e 6f74 206c 6f61 6420  le and not load 
+000062a0: 6974 2069 6e74 6f20 6d65 6d6f 7279 2c0a  it into memory,.
+000062b0: 2020 2020 2020 2020 2320 6173 2077 6520          # as we 
+000062c0: 646f 6e27 7420 6e65 6564 2074 6f20 736f  don't need to so
+000062d0: 7274 2069 7420 6669 7273 740a 2020 2020  rt it first.    
+000062e0: 2020 2020 6966 2069 735f 736f 7274 6564      if is_sorted
+000062f0: 3a0a 2020 2020 2020 2020 2020 2020 7173  :.            qs
+00006300: 765f 6465 6475 705f 636d 642e 6170 7065  v_dedup_cmd.appe
+00006310: 6e64 2822 2d2d 736f 7274 6564 2229 0a20  nd("--sorted"). 
+00006320: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00006330: 2020 2020 2020 2020 7173 765f 6465 6475          qsv_dedu
+00006340: 7020 3d20 7375 6270 726f 6365 7373 2e72  p = subprocess.r
+00006350: 756e 280a 2020 2020 2020 2020 2020 2020  un(.            
+00006360: 2020 2020 7173 765f 6465 6475 705f 636d      qsv_dedup_cm
+00006370: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00006380: 2020 2063 6170 7475 7265 5f6f 7574 7075     capture_outpu
+00006390: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
+000063a0: 2020 2020 2020 2020 7465 7874 3d54 7275          text=Tru
+000063b0: 652c 0a20 2020 2020 2020 2020 2020 2029  e,.            )
+000063c0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000063d0: 7375 6270 726f 6365 7373 2e43 616c 6c65  subprocess.Calle
+000063e0: 6450 726f 6365 7373 4572 726f 7220 6173  dProcessError as
+000063f0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00006400: 7261 6973 6520 7574 696c 2e4a 6f62 4572  raise util.JobEr
+00006410: 726f 7228 2243 6865 636b 2066 6f72 2064  ror("Check for d
+00006420: 7570 6c69 6361 7465 7320 6572 726f 723a  uplicates error:
+00006430: 207b 7d22 2e66 6f72 6d61 7428 6529 290a   {}".format(e)).
+00006440: 2020 2020 2020 2020 6475 7065 5f63 6f75          dupe_cou
+00006450: 6e74 203d 2069 6e74 2873 7472 2871 7376  nt = int(str(qsv
+00006460: 5f64 6564 7570 2e73 7464 6572 7229 2e73  _dedup.stderr).s
+00006470: 7472 6970 2829 290a 2020 2020 2020 2020  trip()).        
+00006480: 6966 2064 7570 655f 636f 756e 7420 3e20  if dupe_count > 
+00006490: 303a 0a20 2020 2020 2020 2020 2020 2074  0:.            t
+000064a0: 6d70 203d 2071 7376 5f64 6564 7570 5f63  mp = qsv_dedup_c
+000064b0: 7376 0a20 2020 2020 2020 2020 2020 206c  sv.            l
+000064c0: 6f67 6765 722e 7761 726e 696e 6728 0a20  ogger.warning(. 
+000064d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000064e0: 7b3a 2c7d 2064 7570 6c69 6361 7465 7320  {:,} duplicates 
+000064f0: 666f 756e 6420 616e 6420 7265 6d6f 7665  found and remove
+00006500: 642e 204e 6f74 6520 7468 6174 2064 6564  d. Note that ded
+00006510: 7570 696e 6720 7265 7375 6c74 7320 696e  uping results in
+00006520: 2061 2073 6f72 7465 6420 4353 562e 222e   a sorted CSV.".
+00006530: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+00006540: 2020 2020 2020 2020 2020 2020 6475 7065              dupe
+00006550: 5f63 6f75 6e74 0a20 2020 2020 2020 2020  _count.         
+00006560: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00006570: 2020 2020 2029 0a20 2020 2065 6c69 6620       ).    elif 
+00006580: 6475 7065 5f63 6f75 6e74 203e 2030 3a0a  dupe_count > 0:.
+00006590: 2020 2020 2020 2020 6c6f 6767 6572 2e77          logger.w
+000065a0: 6172 6e69 6e67 2822 7b3a 2c7d 2064 7570  arning("{:,} dup
+000065b0: 6c69 6361 7465 7320 666f 756e 6420 6275  licates found bu
+000065c0: 7420 6e6f 7420 6465 6475 7069 6e67 2e2e  t not deduping..
+000065d0: 2e22 2e66 6f72 6d61 7428 6475 7065 5f63  .".format(dupe_c
+000065e0: 6f75 6e74 2929 0a0a 2020 2020 2320 2d2d  ount))..    # --
+000065f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006600: 2d2d 2d2d 2d20 4865 6164 6572 7320 2620  ----- Headers & 
+00006610: 5361 6665 6e61 6d65 7320 2d2d 2d2d 2d2d  Safenames ------
+00006620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006630: 2d2d 2d2d 2d0a 2020 2020 2320 6765 7420  -----.    # get 
+00006640: 6578 6973 7469 6e67 2068 6561 6465 7220  existing header 
+00006650: 6e61 6d65 732c 2073 6f20 7765 2063 616e  names, so we can
+00006660: 2075 7365 2074 6865 6d20 666f 7220 6461   use them for da
+00006670: 7461 2064 6963 7469 6f6e 6172 7920 6c61  ta dictionary la
+00006680: 6265 6c73 0a20 2020 2023 2073 686f 756c  bels.    # shoul
+00006690: 6420 7765 206e 6565 6420 746f 2063 6861  d we need to cha
+000066a0: 6e67 6520 7468 6520 636f 6c75 6d6e 206e  nge the column n
+000066b0: 616d 6520 746f 206d 616b 6520 6974 2022  ame to make it "
+000066c0: 6462 2d73 6166 6522 0a20 2020 2074 7279  db-safe".    try
+000066d0: 3a0a 2020 2020 2020 2020 7173 765f 6865  :.        qsv_he
+000066e0: 6164 6572 7320 3d20 7375 6270 726f 6365  aders = subproce
+000066f0: 7373 2e72 756e 280a 2020 2020 2020 2020  ss.run(.        
+00006700: 2020 2020 5b71 7376 5f62 696e 2c20 2268      [qsv_bin, "h
+00006710: 6561 6465 7273 222c 2022 2d2d 6a75 7374  eaders", "--just
+00006720: 2d6e 616d 6573 222c 2074 6d70 2e6e 616d  -names", tmp.nam
+00006730: 655d 2c0a 2020 2020 2020 2020 2020 2020  e],.            
+00006740: 6361 7074 7572 655f 6f75 7470 7574 3d54  capture_output=T
+00006750: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+00006760: 2063 6865 636b 3d54 7275 652c 0a20 2020   check=True,.   
+00006770: 2020 2020 2020 2020 2074 6578 743d 5472           text=Tr
+00006780: 7565 2c0a 2020 2020 2020 2020 290a 2020  ue,.        ).  
+00006790: 2020 6578 6365 7074 2073 7562 7072 6f63    except subproc
+000067a0: 6573 732e 4361 6c6c 6564 5072 6f63 6573  ess.CalledProces
+000067b0: 7345 7272 6f72 2061 7320 653a 0a20 2020  sError as e:.   
+000067c0: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
+000067d0: 4a6f 6245 7272 6f72 2822 4361 6e6e 6f74  JobError("Cannot
+000067e0: 2073 6361 6e20 4353 5620 6865 6164 6572   scan CSV header
+000067f0: 733a 207b 7d22 2e66 6f72 6d61 7428 6529  s: {}".format(e)
+00006800: 290a 2020 2020 6f72 6967 696e 616c 5f68  ).    original_h
+00006810: 6561 6465 7273 203d 2073 7472 2871 7376  eaders = str(qsv
+00006820: 5f68 6561 6465 7273 2e73 7464 6f75 7429  _headers.stdout)
+00006830: 2e73 7472 6970 2829 0a20 2020 206f 7269  .strip().    ori
+00006840: 6769 6e61 6c5f 6865 6164 6572 5f64 6963  ginal_header_dic
+00006850: 7420 3d20 7b0a 2020 2020 2020 2020 6964  t = {.        id
+00006860: 783a 2065 6c65 2066 6f72 2069 6478 2c20  x: ele for idx, 
+00006870: 656c 6520 696e 2065 6e75 6d65 7261 7465  ele in enumerate
+00006880: 286f 7269 6769 6e61 6c5f 6865 6164 6572  (original_header
+00006890: 732e 7370 6c69 746c 696e 6573 2829 290a  s.splitlines()).
+000068a0: 2020 2020 7d0a 0a20 2020 2023 206e 6f77      }..    # now
+000068b0: 2c20 656e 7375 7265 206f 7572 2063 6f6c  , ensure our col
+000068c0: 756d 6e2f 6865 6164 6572 206e 616d 6573  umn/header names
+000068d0: 2069 6465 6e74 6966 6965 7273 2061 7265   identifiers are
+000068e0: 2022 7361 6665 206e 616d 6573 220a 2020   "safe names".  
+000068f0: 2020 2320 692e 652e 2076 616c 6964 2070    # i.e. valid p
+00006900: 6f73 7467 7265 732f 434b 414e 2044 6174  ostgres/CKAN Dat
+00006910: 6173 746f 7265 2069 6465 6e74 6966 6965  astore identifie
+00006920: 7273 0a20 2020 2071 7376 5f73 6166 656e  rs.    qsv_safen
+00006930: 616d 6573 5f63 7376 203d 2074 656d 7066  ames_csv = tempf
+00006940: 696c 652e 4e61 6d65 6454 656d 706f 7261  ile.NamedTempora
+00006950: 7279 4669 6c65 2873 7566 6669 783d 222e  ryFile(suffix=".
+00006960: 6373 7622 290a 2020 2020 6c6f 6767 6572  csv").    logger
+00006970: 2e69 6e66 6f28 2743 6865 636b 696e 6720  .info('Checking 
+00006980: 666f 7220 2264 6174 6162 6173 652d 7361  for "database-sa
+00006990: 6665 2220 6865 6164 6572 206e 616d 6573  fe" header names
+000069a0: 2e2e 2e27 290a 2020 2020 7472 793a 0a20  ...').    try:. 
+000069b0: 2020 2020 2020 2071 7376 5f73 6166 656e         qsv_safen
+000069c0: 616d 6573 203d 2073 7562 7072 6f63 6573  ames = subproces
+000069d0: 732e 7275 6e28 0a20 2020 2020 2020 2020  s.run(.         
+000069e0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+000069f0: 2020 2020 2071 7376 5f62 696e 2c0a 2020       qsv_bin,.  
+00006a00: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00006a10: 6166 656e 616d 6573 222c 0a20 2020 2020  afenames",.     
+00006a20: 2020 2020 2020 2020 2020 2074 6d70 2e6e             tmp.n
+00006a30: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00006a40: 2020 2020 2022 2d2d 6d6f 6465 222c 0a20       "--mode",. 
+00006a50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006a60: 6a73 6f6e 222c 0a20 2020 2020 2020 2020  json",.         
+00006a70: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
+00006a80: 2020 6361 7074 7572 655f 6f75 7470 7574    capture_output
+00006a90: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+00006aa0: 2020 2074 6578 743d 5472 7565 2c0a 2020     text=True,.  
+00006ab0: 2020 2020 2020 290a 2020 2020 6578 6365        ).    exce
+00006ac0: 7074 2073 7562 7072 6f63 6573 732e 4361  pt subprocess.Ca
+00006ad0: 6c6c 6564 5072 6f63 6573 7345 7272 6f72  lledProcessError
+00006ae0: 2061 7320 653a 0a20 2020 2020 2020 2072   as e:.        r
+00006af0: 6169 7365 2075 7469 6c2e 4a6f 6245 7272  aise util.JobErr
+00006b00: 6f72 2822 5361 6665 6e61 6d65 7320 6572  or("Safenames er
+00006b10: 726f 723a 207b 7d22 2e66 6f72 6d61 7428  ror: {}".format(
+00006b20: 6529 290a 0a20 2020 2075 6e73 6166 655f  e))..    unsafe_
+00006b30: 6a73 6f6e 203d 206a 736f 6e2e 6c6f 6164  json = json.load
+00006b40: 7328 7374 7228 7173 765f 7361 6665 6e61  s(str(qsv_safena
+00006b50: 6d65 732e 7374 646f 7574 2929 0a20 2020  mes.stdout)).   
+00006b60: 2075 6e73 6166 655f 6865 6164 6572 7320   unsafe_headers 
+00006b70: 3d20 756e 7361 6665 5f6a 736f 6e5b 2275  = unsafe_json["u
+00006b80: 6e73 6166 655f 6865 6164 6572 7322 5d0a  nsafe_headers"].
+00006b90: 0a20 2020 2069 6620 756e 7361 6665 5f68  .    if unsafe_h
+00006ba0: 6561 6465 7273 3a0a 2020 2020 2020 2020  eaders:.        
+00006bb0: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+00006bc0: 2020 2020 2020 2020 2027 227b 7d20 756e           '"{} un
+00006bd0: 7361 6665 2220 6865 6164 6572 206e 616d  safe" header nam
+00006be0: 6573 2066 6f75 6e64 2028 7b7d 292e 2053  es found ({}). S
+00006bf0: 616e 6974 697a 696e 672e 2e2e 2227 2e66  anitizing..."'.f
+00006c00: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00006c10: 2020 2020 2020 206c 656e 2875 6e73 6166         len(unsaf
+00006c20: 655f 6865 6164 6572 7329 2c20 756e 7361  e_headers), unsa
+00006c30: 6665 5f68 6561 6465 7273 0a20 2020 2020  fe_headers.     
+00006c40: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00006c50: 2029 0a20 2020 2020 2020 2071 7376 5f73   ).        qsv_s
+00006c60: 6166 656e 616d 6573 203d 2073 7562 7072  afenames = subpr
+00006c70: 6f63 6573 732e 7275 6e28 0a20 2020 2020  ocess.run(.     
+00006c80: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+00006c90: 2020 2020 2020 2020 2071 7376 5f62 696e           qsv_bin
+00006ca0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006cb0: 2020 2273 6166 656e 616d 6573 222c 0a20    "safenames",. 
+00006cc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00006cd0: 6d70 2e6e 616d 652c 0a20 2020 2020 2020  mp.name,.       
+00006ce0: 2020 2020 2020 2020 2022 2d2d 6d6f 6465           "--mode
+00006cf0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006d00: 2020 2022 636f 6e64 6974 696f 6e61 6c22     "conditional"
+00006d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006d20: 2020 222d 2d6f 7574 7075 7422 2c0a 2020    "--output",.  
+00006d30: 2020 2020 2020 2020 2020 2020 2020 7173                qs
+00006d40: 765f 7361 6665 6e61 6d65 735f 6373 762e  v_safenames_csv.
+00006d50: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
+00006d60: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+00006d70: 2063 6170 7475 7265 5f6f 7574 7075 743d   capture_output=
+00006d80: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00006d90: 2020 7465 7874 3d54 7275 652c 0a20 2020    text=True,.   
+00006da0: 2020 2020 2029 0a20 2020 2020 2020 2074       ).        t
+00006db0: 6d70 203d 2071 7376 5f73 6166 656e 616d  mp = qsv_safenam
+00006dc0: 6573 5f63 7376 0a20 2020 2065 6c73 653a  es_csv.    else:
+00006dd0: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00006de0: 696e 666f 2822 4e6f 2075 6e73 6166 6520  info("No unsafe 
+00006df0: 6865 6164 6572 206e 616d 6573 2066 6f75  header names fou
+00006e00: 6e64 2e2e 2e22 290a 0a20 2020 2023 202d  nd...")..    # -
+00006e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00006e20: 2d2d 2d2d 2d20 5479 7065 2049 6e66 6572  ----- Type Infer
+00006e30: 656e 6369 6e67 202d 2d2d 2d2d 2d2d 2d2d  encing ---------
+00006e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00006e50: 2020 2023 2061 7420 7468 6973 2073 7461     # at this sta
+00006e60: 6765 2c20 7765 2068 6176 6520 6120 2263  ge, we have a "c
+00006e70: 6c65 616e 2220 4353 5620 7265 6164 7920  lean" CSV ready 
+00006e80: 666f 7220 5479 7065 2049 6e66 6572 656e  for Type Inferen
+00006e90: 6369 6e67 0a0a 2020 2020 2320 6669 7273  cing..    # firs
+00006ea0: 742c 2069 6e64 6578 2063 7376 2066 6f72  t, index csv for
+00006eb0: 2073 7065 6564 202d 2063 6f75 6e74 2c20   speed - count, 
+00006ec0: 7374 6174 7320 616e 6420 736c 6963 650a  stats and slice.
+00006ed0: 2020 2020 2320 6172 6520 616c 6c20 6163      # are all ac
+00006ee0: 6365 6c65 7261 7465 642f 6d75 6c74 6974  celerated/multit
+00006ef0: 6872 6561 6465 6420 7768 656e 2061 6e20  hreaded when an 
+00006f00: 696e 6465 7820 6973 2070 7265 7365 6e74  index is present
+00006f10: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
+00006f20: 2020 7173 765f 696e 6465 785f 6669 6c65    qsv_index_file
+00006f30: 203d 2074 6d70 2e6e 616d 6520 2b20 222e   = tmp.name + ".
+00006f40: 6964 7822 0a20 2020 2020 2020 2073 7562  idx".        sub
+00006f50: 7072 6f63 6573 732e 7275 6e28 5b71 7376  process.run([qsv
+00006f60: 5f62 696e 2c20 2269 6e64 6578 222c 2074  _bin, "index", t
+00006f70: 6d70 2e6e 616d 655d 2c20 6368 6563 6b3d  mp.name], check=
+00006f80: 5472 7565 290a 2020 2020 6578 6365 7074  True).    except
+00006f90: 2073 7562 7072 6f63 6573 732e 4361 6c6c   subprocess.Call
+00006fa0: 6564 5072 6f63 6573 7345 7272 6f72 2061  edProcessError a
+00006fb0: 7320 653a 0a20 2020 2020 2020 2072 6169  s e:.        rai
+00006fc0: 7365 2075 7469 6c2e 4a6f 6245 7272 6f72  se util.JobError
+00006fd0: 2822 4361 6e6e 6f74 2069 6e64 6578 2043  ("Cannot index C
+00006fe0: 5356 3a20 7b7d 222e 666f 726d 6174 2865  SV: {}".format(e
+00006ff0: 2929 0a0a 2020 2020 2320 6966 2053 4f52  ))..    # if SOR
+00007000: 545f 414e 445f 4455 5045 5f43 4845 434b  T_AND_DUPE_CHECK
+00007010: 203d 2054 7275 652c 2077 6520 616c 7265   = True, we alre
+00007020: 6164 7920 6b6e 6f77 2074 6865 2072 6563  ady know the rec
+00007030: 6f72 6420 636f 756e 740a 2020 2020 2320  ord count.    # 
+00007040: 736f 2077 6520 6361 6e20 736b 6970 2071  so we can skip q
+00007050: 7376 2063 6f75 6e74 2e0a 2020 2020 6966  sv count..    if
+00007060: 206e 6f74 2073 6f72 745f 616e 645f 6475   not sort_and_du
+00007070: 7065 5f63 6865 636b 3a0a 2020 2020 2020  pe_check:.      
+00007080: 2020 2320 6765 7420 7265 636f 7264 2063    # get record c
+00007090: 6f75 6e74 2c20 7468 6973 2069 7320 696e  ount, this is in
+000070a0: 7374 616e 7461 6e65 6f75 7320 7769 7468  stantaneous with
+000070b0: 2061 6e20 696e 6465 780a 2020 2020 2020   an index.      
+000070c0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000070d0: 2020 2071 7376 5f63 6f75 6e74 203d 2073     qsv_count = s
+000070e0: 7562 7072 6f63 6573 732e 7275 6e28 0a20  ubprocess.run(. 
+000070f0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00007100: 7173 765f 6269 6e2c 2022 636f 756e 7422  qsv_bin, "count"
+00007110: 2c20 746d 702e 6e61 6d65 5d2c 2063 6170  , tmp.name], cap
+00007120: 7475 7265 5f6f 7574 7075 743d 5472 7565  ture_output=True
+00007130: 2c20 6368 6563 6b3d 5472 7565 2c20 7465  , check=True, te
+00007140: 7874 3d54 7275 650a 2020 2020 2020 2020  xt=True.        
+00007150: 2020 2020 290a 2020 2020 2020 2020 6578      ).        ex
+00007160: 6365 7074 2073 7562 7072 6f63 6573 732e  cept subprocess.
+00007170: 4361 6c6c 6564 5072 6f63 6573 7345 7272  CalledProcessErr
+00007180: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
+00007190: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
+000071a0: 4a6f 6245 7272 6f72 2822 4361 6e6e 6f74  JobError("Cannot
+000071b0: 2063 6f75 6e74 2072 6563 6f72 6473 2069   count records i
+000071c0: 6e20 4353 563a 207b 7d22 2e66 6f72 6d61  n CSV: {}".forma
+000071d0: 7428 6529 290a 2020 2020 2020 2020 7265  t(e)).        re
+000071e0: 636f 7264 5f63 6f75 6e74 203d 2069 6e74  cord_count = int
+000071f0: 2873 7472 2871 7376 5f63 6f75 6e74 2e73  (str(qsv_count.s
+00007200: 7464 6f75 7429 2e73 7472 6970 2829 290a  tdout).strip()).
+00007210: 0a20 2020 2023 2069 7473 2065 6d70 7479  .    # its empty
+00007220: 2c20 6e6f 7468 696e 6720 746f 2064 6f0a  , nothing to do.
+00007230: 2020 2020 6966 2072 6563 6f72 645f 636f      if record_co
+00007240: 756e 7420 3d3d 2030 3a0a 2020 2020 2020  unt == 0:.      
+00007250: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
+00007260: 2822 5570 6c6f 6164 2073 6b69 7070 6564  ("Upload skipped
+00007270: 2061 7320 7468 6572 6520 6172 6520 7a65   as there are ze
+00007280: 726f 2072 6563 6f72 6473 2e22 290a 2020  ro records.").  
+00007290: 2020 2020 2020 7265 7475 726e 0a0a 2020        return..  
+000072a0: 2020 2320 6c6f 6720 686f 7720 6d61 6e79    # log how many
+000072b0: 2072 6563 6f72 6473 2077 6520 6465 7465   records we dete
+000072c0: 6374 6564 0a20 2020 2075 6e69 7175 655f  cted.    unique_
+000072d0: 7175 616c 6966 6965 7220 3d20 2222 0a20  qualifier = "". 
+000072e0: 2020 2069 6620 6465 6475 703a 0a20 2020     if dedup:.   
+000072f0: 2020 2020 2075 6e69 7175 655f 7175 616c       unique_qual
+00007300: 6966 6965 7220 3d20 2275 6e69 7175 6522  ifier = "unique"
+00007310: 0a20 2020 206c 6f67 6765 722e 696e 666f  .    logger.info
+00007320: 2822 7b3a 2c7d 207b 7d20 7265 636f 7264  ("{:,} {} record
+00007330: 7320 6465 7465 6374 6564 2e2e 2e22 2e66  s detected...".f
+00007340: 6f72 6d61 7428 7265 636f 7264 5f63 6f75  ormat(record_cou
+00007350: 6e74 2c20 756e 6971 7565 5f71 7561 6c69  nt, unique_quali
+00007360: 6669 6572 2929 0a0a 2020 2020 2320 7275  fier))..    # ru
+00007370: 6e20 7173 7620 7374 6174 7320 746f 2067  n qsv stats to g
+00007380: 6574 2064 6174 6120 7479 7065 7320 616e  et data types an
+00007390: 6420 7375 6d6d 6172 7920 7374 6174 6973  d summary statis
+000073a0: 7469 6373 0a20 2020 206c 6f67 6765 722e  tics.    logger.
+000073b0: 696e 666f 2822 496e 6665 7272 696e 6720  info("Inferring 
+000073c0: 6461 7461 2074 7970 6573 2061 6e64 2063  data types and c
+000073d0: 6f6d 7069 6c69 6e67 2073 7461 7469 7374  ompiling statist
+000073e0: 6963 732e 2e2e 2229 0a20 2020 2068 6561  ics...").    hea
+000073f0: 6465 7273 203d 205b 5d0a 2020 2020 7479  ders = [].    ty
+00007400: 7065 7320 3d20 5b5d 0a20 2020 2068 6561  pes = [].    hea
+00007410: 6465 7273 5f6d 696e 203d 205b 5d0a 2020  ders_min = [].  
+00007420: 2020 6865 6164 6572 735f 6d61 7820 3d20    headers_max = 
+00007430: 5b5d 0a20 2020 2068 6561 6465 7273 5f63  [].    headers_c
+00007440: 6172 6469 6e61 6c69 7479 203d 205b 5d0a  ardinality = [].
+00007450: 2020 2020 7173 765f 7374 6174 735f 6373      qsv_stats_cs
+00007460: 7620 3d20 7465 6d70 6669 6c65 2e4e 616d  v = tempfile.Nam
+00007470: 6564 5465 6d70 6f72 6172 7946 696c 6528  edTemporaryFile(
+00007480: 7375 6666 6978 3d22 2e63 7376 2229 0a20  suffix=".csv"). 
+00007490: 2020 2071 7376 5f73 7461 7473 5f63 6d64     qsv_stats_cmd
+000074a0: 203d 205b 0a20 2020 2020 2020 2071 7376   = [.        qsv
+000074b0: 5f62 696e 2c0a 2020 2020 2020 2020 2273  _bin,.        "s
+000074c0: 7461 7473 222c 0a20 2020 2020 2020 2074  tats",.        t
+000074d0: 6d70 2e6e 616d 652c 0a20 2020 2020 2020  mp.name,.       
+000074e0: 2022 2d2d 696e 6665 722d 6461 7465 7322   "--infer-dates"
+000074f0: 2c0a 2020 2020 2020 2020 222d 2d64 6174  ,.        "--dat
+00007500: 6573 2d77 6869 7465 6c69 7374 222c 0a20  es-whitelist",. 
+00007510: 2020 2020 2020 2022 616c 6c22 2c0a 2020         "all",.  
+00007520: 2020 2020 2020 222d 2d6f 7574 7075 7422        "--output"
+00007530: 2c0a 2020 2020 2020 2020 7173 765f 7374  ,.        qsv_st
+00007540: 6174 735f 6373 762e 6e61 6d65 2c0a 2020  ats_csv.name,.  
+00007550: 2020 5d0a 2020 2020 7072 6566 6572 5f64    ].    prefer_d
+00007560: 6d79 203d 2063 6f6e 6669 672e 6765 7428  my = config.get(
+00007570: 2250 5245 4645 525f 444d 5922 290a 2020  "PREFER_DMY").  
+00007580: 2020 6966 2070 7265 6665 725f 646d 793a    if prefer_dmy:
+00007590: 0a20 2020 2020 2020 2071 7376 5f73 7461  .        qsv_sta
+000075a0: 7473 5f63 6d64 2e61 7070 656e 6428 222d  ts_cmd.append("-
+000075b0: 2d70 7265 6665 725f 646d 7922 290a 2020  -prefer_dmy").  
+000075c0: 2020 6175 746f 5f69 6e64 6578 5f74 6872    auto_index_thr
+000075d0: 6573 686f 6c64 203d 2063 6f6e 6669 672e  eshold = config.
+000075e0: 6765 7428 2241 5554 4f5f 494e 4445 585f  get("AUTO_INDEX_
+000075f0: 5448 5245 5348 4f4c 4422 290a 2020 2020  THRESHOLD").    
+00007600: 6966 2061 7574 6f5f 696e 6465 785f 7468  if auto_index_th
+00007610: 7265 7368 6f6c 643a 0a20 2020 2020 2020  reshold:.       
+00007620: 2071 7376 5f73 7461 7473 5f63 6d64 2e61   qsv_stats_cmd.a
+00007630: 7070 656e 6428 222d 2d63 6172 6469 6e61  ppend("--cardina
+00007640: 6c69 7479 2229 0a20 2020 2073 756d 6d61  lity").    summa
+00007650: 7279 5f73 7461 7473 5f6f 7074 696f 6e73  ry_stats_options
+00007660: 203d 2063 6f6e 6669 672e 6765 7428 2253   = config.get("S
+00007670: 554d 4d41 5259 5f53 5441 5453 5f4f 5054  UMMARY_STATS_OPT
+00007680: 494f 4e53 2229 0a20 2020 2069 6620 7375  IONS").    if su
+00007690: 6d6d 6172 795f 7374 6174 735f 6f70 7469  mmary_stats_opti
+000076a0: 6f6e 733a 0a20 2020 2020 2020 2071 7376  ons:.        qsv
+000076b0: 5f73 7461 7473 5f63 6d64 2e61 7070 656e  _stats_cmd.appen
+000076c0: 6428 7375 6d6d 6172 795f 7374 6174 735f  d(summary_stats_
+000076d0: 6f70 7469 6f6e 7329 0a0a 2020 2020 7472  options)..    tr
+000076e0: 793a 0a20 2020 2020 2020 2071 7376 5f73  y:.        qsv_s
+000076f0: 7461 7473 203d 2073 7562 7072 6f63 6573  tats = subproces
+00007700: 732e 7275 6e28 7173 765f 7374 6174 735f  s.run(qsv_stats_
+00007710: 636d 642c 2063 6865 636b 3d54 7275 6529  cmd, check=True)
+00007720: 0a20 2020 2065 7863 6570 7420 7375 6270  .    except subp
+00007730: 726f 6365 7373 2e43 616c 6c65 6450 726f  rocess.CalledPro
+00007740: 6365 7373 4572 726f 7220 6173 2065 3a0a  cessError as e:.
+00007750: 2020 2020 2020 2020 7261 6973 6520 7574          raise ut
+00007760: 696c 2e4a 6f62 4572 726f 7228 0a20 2020  il.JobError(.   
+00007770: 2020 2020 2020 2020 2022 4361 6e6e 6f74           "Cannot
+00007780: 2069 6e66 6572 2064 6174 6120 7479 7065   infer data type
+00007790: 7320 616e 6420 636f 6d70 696c 6520 7374  s and compile st
+000077a0: 6174 6973 7469 6373 3a20 7b7d 222e 666f  atistics: {}".fo
+000077b0: 726d 6174 2865 290a 2020 2020 2020 2020  rmat(e).        
+000077c0: 290a 0a20 2020 2077 6974 6820 6f70 656e  )..    with open
+000077d0: 2871 7376 5f73 7461 7473 5f63 7376 2e6e  (qsv_stats_csv.n
+000077e0: 616d 652c 206d 6f64 653d 2272 2229 2061  ame, mode="r") a
+000077f0: 7320 696e 703a 0a20 2020 2020 2020 2072  s inp:.        r
+00007800: 6561 6465 7220 3d20 6373 762e 4469 6374  eader = csv.Dict
+00007810: 5265 6164 6572 2869 6e70 290a 2020 2020  Reader(inp).    
+00007820: 2020 2020 666f 7220 726f 7720 696e 2072      for row in r
+00007830: 6561 6465 723a 0a20 2020 2020 2020 2020  eader:.         
+00007840: 2020 2068 6561 6465 7273 2e61 7070 656e     headers.appen
+00007850: 6428 726f 775b 2266 6965 6c64 225d 290a  d(row["field"]).
+00007860: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00007870: 732e 6170 7065 6e64 2872 6f77 5b22 7479  s.append(row["ty
+00007880: 7065 225d 290a 2020 2020 2020 2020 2020  pe"]).          
+00007890: 2020 6865 6164 6572 735f 6d69 6e2e 6170    headers_min.ap
+000078a0: 7065 6e64 2872 6f77 5b22 6d69 6e22 5d29  pend(row["min"])
+000078b0: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
+000078c0: 6465 7273 5f6d 6178 2e61 7070 656e 6428  ders_max.append(
+000078d0: 726f 775b 226d 6178 225d 290a 2020 2020  row["max"]).    
+000078e0: 2020 2020 2020 2020 6966 2061 7574 6f5f          if auto_
+000078f0: 696e 6465 785f 7468 7265 7368 6f6c 643a  index_threshold:
+00007900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007910: 2068 6561 6465 7273 5f63 6172 6469 6e61   headers_cardina
+00007920: 6c69 7479 2e61 7070 656e 6428 696e 7428  lity.append(int(
+00007930: 726f 775b 2263 6172 6469 6e61 6c69 7479  row["cardinality
+00007940: 225d 2929 0a0a 2020 2020 6578 6973 7469  "]))..    existi
+00007950: 6e67 203d 2064 6174 6173 746f 7265 5f72  ng = datastore_r
+00007960: 6573 6f75 7263 655f 6578 6973 7473 2872  esource_exists(r
+00007970: 6573 6f75 7263 655f 6964 2c20 6170 695f  esource_id, api_
+00007980: 6b65 792c 2063 6b61 6e5f 7572 6c29 0a20  key, ckan_url). 
+00007990: 2020 2065 7869 7374 696e 675f 696e 666f     existing_info
+000079a0: 203d 204e 6f6e 650a 2020 2020 6966 2065   = None.    if e
+000079b0: 7869 7374 696e 673a 0a20 2020 2020 2020  xisting:.       
+000079c0: 2065 7869 7374 696e 675f 696e 666f 203d   existing_info =
+000079d0: 2064 6963 7428 0a20 2020 2020 2020 2020   dict(.         
+000079e0: 2020 2028 665b 2269 6422 5d2c 2066 5b22     (f["id"], f["
+000079f0: 696e 666f 225d 2920 666f 7220 6620 696e  info"]) for f in
+00007a00: 2065 7869 7374 696e 672e 6765 7428 2266   existing.get("f
+00007a10: 6965 6c64 7322 2c20 5b5d 2920 6966 2022  ields", []) if "
+00007a20: 696e 666f 2220 696e 2066 0a20 2020 2020  info" in f.     
+00007a30: 2020 2029 0a0a 2020 2020 2320 6966 2074     )..    # if t
+00007a40: 6869 7320 6973 2061 6e20 6578 6973 7469  his is an existi
+00007a50: 6e67 2072 6573 6f75 7263 650a 2020 2020  ng resource.    
+00007a60: 2320 6f76 6572 7269 6465 2077 6974 6820  # override with 
+00007a70: 7479 7065 7320 7573 6572 2072 6571 7565  types user reque
+00007a80: 7374 6564 2069 6e20 4461 7461 2044 6963  sted in Data Dic
+00007a90: 7469 6f6e 6172 790a 2020 2020 6966 2065  tionary.    if e
+00007aa0: 7869 7374 696e 675f 696e 666f 3a0a 2020  xisting_info:.  
+00007ab0: 2020 2020 2020 7479 7065 7320 3d20 5b0a        types = [.
+00007ac0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00007ad0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00007ae0: 6578 7422 3a20 2253 7472 696e 6722 2c0a  ext": "String",.
+00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b00: 226e 756d 6572 6963 223a 2022 466c 6f61  "numeric": "Floa
+00007b10: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00007b20: 2020 2020 2274 696d 6573 7461 6d70 223a      "timestamp":
+00007b30: 2022 4461 7465 5469 6d65 222c 0a20 2020   "DateTime",.   
+00007b40: 2020 2020 2020 2020 207d 2e67 6574 2865           }.get(e
+00007b50: 7869 7374 696e 675f 696e 666f 2e67 6574  xisting_info.get
+00007b60: 2868 2c20 7b7d 292e 6765 7428 2274 7970  (h, {}).get("typ
+00007b70: 655f 6f76 6572 7269 6465 2229 2c20 7429  e_override"), t)
+00007b80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00007b90: 2074 2c20 6820 696e 207a 6970 2874 7970   t, h in zip(typ
+00007ba0: 6573 2c20 6865 6164 6572 7329 0a20 2020  es, headers).   
+00007bb0: 2020 2020 205d 0a0a 2020 2020 2320 4465       ]..    # De
+00007bc0: 6c65 7465 2065 7869 7374 696e 6720 6461  lete existing da
+00007bd0: 7461 7374 6f72 6520 7265 736f 7572 6365  tastore resource
+00007be0: 2062 6566 6f72 6520 7072 6f63 6565 6469   before proceedi
+00007bf0: 6e67 2e0a 2020 2020 6966 2065 7869 7374  ng..    if exist
+00007c00: 696e 673a 0a20 2020 2020 2020 206c 6f67  ing:.        log
+00007c10: 6765 722e 696e 666f 280a 2020 2020 2020  ger.info(.      
+00007c20: 2020 2020 2020 2744 656c 6574 696e 6720        'Deleting 
+00007c30: 6578 6973 7469 6e67 2072 6573 6f75 7263  existing resourc
+00007c40: 6520 227b 7265 735f 6964 7d22 2066 726f  e "{res_id}" fro
+00007c50: 6d20 6461 7461 7374 6f72 652e 272e 666f  m datastore.'.fo
+00007c60: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+00007c70: 2020 2020 2020 7265 735f 6964 3d72 6573        res_id=res
+00007c80: 6f75 7263 655f 6964 0a20 2020 2020 2020  ource_id.       
+00007c90: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+00007ca0: 0a20 2020 2020 2020 2064 656c 6574 655f  .        delete_
+00007cb0: 6461 7461 7374 6f72 655f 7265 736f 7572  datastore_resour
+00007cc0: 6365 2872 6573 6f75 7263 655f 6964 2c20  ce(resource_id, 
+00007cd0: 6170 695f 6b65 792c 2063 6b61 6e5f 7572  api_key, ckan_ur
+00007ce0: 6c29 0a0a 2020 2020 2320 3173 7420 7061  l)..    # 1st pa
+00007cf0: 7373 206f 6620 6275 696c 6469 6e67 2068  ss of building h
+00007d00: 6561 6465 7273 5f64 6963 740a 2020 2020  eaders_dict.    
+00007d10: 2320 6865 7265 2077 6520 6d61 7020 696e  # here we map in
+00007d20: 6665 7272 6564 2074 7970 6573 2074 6f20  ferred types to 
+00007d30: 706f 7374 6772 6573 716c 2064 6174 6120  postgresql data 
+00007d40: 7479 7065 730a 2020 2020 7479 7065 5f6d  types.    type_m
+00007d50: 6170 7069 6e67 203d 2063 6f6e 6669 672e  apping = config.
+00007d60: 6765 7428 2254 5950 455f 4d41 5050 494e  get("TYPE_MAPPIN
+00007d70: 4722 290a 2020 2020 7465 6d70 5f68 6561  G").    temp_hea
+00007d80: 6465 7273 5f64 6963 7473 203d 205b 0a20  ders_dicts = [. 
+00007d90: 2020 2020 2020 2064 6963 7428 6964 3d66         dict(id=f
+00007da0: 6965 6c64 5b30 5d2c 2074 7970 653d 7479  ield[0], type=ty
+00007db0: 7065 5f6d 6170 7069 6e67 5b73 7472 2866  pe_mapping[str(f
+00007dc0: 6965 6c64 5b31 5d29 5d29 0a20 2020 2020  ield[1])]).     
+00007dd0: 2020 2066 6f72 2066 6965 6c64 2069 6e20     for field in 
+00007de0: 7a69 7028 6865 6164 6572 732c 2074 7970  zip(headers, typ
+00007df0: 6573 290a 2020 2020 5d0a 0a20 2020 2023  es).    ]..    #
+00007e00: 2032 6e64 2070 6173 7320 6865 6164 6572   2nd pass header
+00007e10: 5f64 6963 7473 2c20 6368 6563 6b69 6e67  _dicts, checking
+00007e20: 2066 6f72 2073 6d61 7274 696e 7420 7479   for smartint ty
+00007e30: 7065 732e 0a20 2020 2023 2022 736d 6172  pes..    # "smar
+00007e40: 7469 6e74 2220 7769 6c6c 2061 7574 6f6d  tint" will autom
+00007e50: 6174 6963 616c 6c79 2073 656c 6563 7420  atically select 
+00007e60: 7468 6520 6265 7374 2069 6e74 6567 6572  the best integer
+00007e70: 2064 6174 6120 7479 7065 2062 6173 6564   data type based
+00007e80: 206f 6e20 7468 650a 2020 2020 2320 6d69   on the.    # mi
+00007e90: 6e2f 6d61 7820 7661 6c75 6573 206f 6620  n/max values of 
+00007ea0: 7468 6520 636f 6c75 6d6e 2077 6520 676f  the column we go
+00007eb0: 7420 6672 6f6d 2071 7376 2073 7461 7473  t from qsv stats
+00007ec0: 2e0a 2020 2020 2320 5765 2061 6c73 6f20  ..    # We also 
+00007ed0: 7365 7420 7468 6520 4461 7461 2044 6963  set the Data Dic
+00007ee0: 7469 6f6e 6172 7920 4c61 6265 6c20 746f  tionary Label to
+00007ef0: 206f 7269 6769 6e61 6c20 636f 6c75 6d6e   original column
+00007f00: 206e 616d 6573 2069 6e20 6361 7365 2077   names in case w
+00007f10: 6520 6d61 6465 0a20 2020 2023 2074 6865  e made.    # the
+00007f20: 206e 616d 6573 2022 6462 2d73 6166 6522   names "db-safe"
+00007f30: 2061 7320 7468 6520 6c61 6265 6c73 2061   as the labels a
+00007f40: 7265 2075 7365 6420 6279 2044 6174 6154  re used by DataT
+00007f50: 6162 6c65 735f 7669 6577 2074 6f20 6c61  ables_view to la
+00007f60: 6265 6c20 636f 6c75 6d6e 730a 2020 2020  bel columns.    
+00007f70: 2320 7765 2061 6c73 6f20 7461 6b65 206e  # we also take n
+00007f80: 6f74 6520 6f66 2064 6174 6574 696d 652f  ote of datetime/
+00007f90: 7469 6d65 7374 616d 7020 6669 656c 6473  timestamp fields
+00007fa0: 2c20 736f 2077 6520 6361 6e20 6e6f 726d  , so we can norm
+00007fb0: 616c 697a 6520 7468 656d 0a20 2020 2023  alize them.    #
+00007fc0: 2074 6f20 5246 4333 3333 3920 666f 726d   to RFC3339 form
+00007fd0: 6174 2c20 7768 6963 6820 6973 2050 6f73  at, which is Pos
+00007fe0: 7467 7265 7320 434f 5059 2072 6561 6479  tgres COPY ready
+00007ff0: 0a20 2020 2064 6174 6574 696d 6563 6f6c  .    datetimecol
+00008000: 735f 6c69 7374 203d 205b 5d0a 2020 2020  s_list = [].    
+00008010: 6865 6164 6572 735f 6469 6374 7320 3d20  headers_dicts = 
+00008020: 5b5d 0a20 2020 2066 6f72 2069 6478 2c20  [].    for idx, 
+00008030: 6865 6164 6572 2069 6e20 656e 756d 6572  header in enumer
+00008040: 6174 6528 7465 6d70 5f68 6561 6465 7273  ate(temp_headers
+00008050: 5f64 6963 7473 293a 0a20 2020 2020 2020  _dicts):.       
+00008060: 2069 6620 6865 6164 6572 5b22 7479 7065   if header["type
+00008070: 225d 203d 3d20 2273 6d61 7274 696e 7422  "] == "smartint"
+00008080: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00008090: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+000080a0: 2020 2069 6e74 2868 6561 6465 7273 5f6d     int(headers_m
+000080b0: 6178 5b69 6478 5d29 203c 3d20 504f 5354  ax[idx]) <= POST
+000080c0: 4752 4553 5f49 4e54 5f4d 4158 0a20 2020  GRES_INT_MAX.   
+000080d0: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+000080e0: 2069 6e74 2868 6561 6465 7273 5f6d 696e   int(headers_min
+000080f0: 5b69 6478 5d29 203e 3d20 504f 5354 4752  [idx]) >= POSTGR
+00008100: 4553 5f49 4e54 5f4d 494e 0a20 2020 2020  ES_INT_MIN.     
+00008110: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00008120: 2020 2020 2020 2020 2020 6865 6164 6572            header
+00008130: 5f74 7970 6520 3d20 2269 6e74 6567 6572  _type = "integer
+00008140: 220a 2020 2020 2020 2020 2020 2020 656c  ".            el
+00008150: 6966 2028 0a20 2020 2020 2020 2020 2020  if (.           
+00008160: 2020 2020 2069 6e74 2868 6561 6465 7273       int(headers
+00008170: 5f6d 6178 5b69 6478 5d29 203c 3d20 504f  _max[idx]) <= PO
+00008180: 5354 4752 4553 5f42 4947 494e 545f 4d41  STGRES_BIGINT_MA
+00008190: 580a 2020 2020 2020 2020 2020 2020 2020  X.              
+000081a0: 2020 616e 6420 696e 7428 6865 6164 6572    and int(header
+000081b0: 735f 6d69 6e5b 6964 785d 2920 3e3d 2050  s_min[idx]) >= P
+000081c0: 4f53 5447 5245 535f 4249 4749 4e54 5f4d  OSTGRES_BIGINT_M
+000081d0: 494e 0a20 2020 2020 2020 2020 2020 2029  IN.            )
+000081e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000081f0: 2020 6865 6164 6572 5f74 7970 6520 3d20    header_type = 
+00008200: 2262 6967 696e 7422 0a20 2020 2020 2020  "bigint".       
+00008210: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008220: 2020 2020 2020 2020 2020 2068 6561 6465             heade
+00008230: 725f 7479 7065 203d 2022 6e75 6d65 7269  r_type = "numeri
+00008240: 6322 0a20 2020 2020 2020 2065 6c73 653a  c".        else:
+00008250: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
+00008260: 6465 725f 7479 7065 203d 2068 6561 6465  der_type = heade
+00008270: 725b 2274 7970 6522 5d0a 2020 2020 2020  r["type"].      
+00008280: 2020 6966 2068 6561 6465 725f 7479 7065    if header_type
+00008290: 203d 3d20 2274 696d 6573 7461 6d70 223a   == "timestamp":
+000082a0: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+000082b0: 6574 696d 6563 6f6c 735f 6c69 7374 2e61  etimecols_list.a
+000082c0: 7070 656e 6428 6865 6164 6572 5b22 6964  ppend(header["id
+000082d0: 225d 290a 2020 2020 2020 2020 696e 666f  "]).        info
+000082e0: 5f64 6963 7420 3d20 6469 6374 286c 6162  _dict = dict(lab
+000082f0: 656c 3d6f 7269 6769 6e61 6c5f 6865 6164  el=original_head
+00008300: 6572 5f64 6963 745b 6964 785d 290a 2020  er_dict[idx]).  
+00008310: 2020 2020 2020 6865 6164 6572 735f 6469        headers_di
+00008320: 6374 732e 6170 7065 6e64 2864 6963 7428  cts.append(dict(
+00008330: 6964 3d68 6561 6465 725b 2269 6422 5d2c  id=header["id"],
+00008340: 2074 7970 653d 6865 6164 6572 5f74 7970   type=header_typ
+00008350: 652c 2069 6e66 6f3d 696e 666f 5f64 6963  e, info=info_dic
+00008360: 7429 290a 0a20 2020 2023 204d 6169 6e74  t))..    # Maint
+00008370: 6169 6e20 6461 7461 2064 6963 7469 6f6e  ain data diction
+00008380: 6172 6965 7320 6672 6f6d 206d 6174 6368  aries from match
+00008390: 696e 6720 636f 6c75 6d6e 206e 616d 6573  ing column names
+000083a0: 0a20 2020 2023 2069 6620 6461 7461 2064  .    # if data d
+000083b0: 6963 7469 6f6e 6172 7920 616c 7265 6164  ictionary alread
+000083c0: 7920 6578 6973 7473 2066 6f72 2074 6869  y exists for thi
+000083d0: 7320 7265 736f 7572 6365 2061 730a 2020  s resource as.  
+000083e0: 2020 2320 7765 2077 616e 7420 746f 2070    # we want to p
+000083f0: 7265 7365 7276 6520 7468 6520 7573 6572  reserve the user
+00008400: 2773 2064 6174 6120 6469 6374 696f 6e61  's data dictiona
+00008410: 7279 2063 7572 6174 696f 6e73 0a20 2020  ry curations.   
+00008420: 2069 6620 6578 6973 7469 6e67 5f69 6e66   if existing_inf
+00008430: 6f3a 0a20 2020 2020 2020 2066 6f72 2068  o:.        for h
+00008440: 2069 6e20 6865 6164 6572 735f 6469 6374   in headers_dict
+00008450: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00008460: 6620 685b 2269 6422 5d20 696e 2065 7869  f h["id"] in exi
+00008470: 7374 696e 675f 696e 666f 3a0a 2020 2020  sting_info:.    
+00008480: 2020 2020 2020 2020 2020 2020 685b 2269              h["i
+00008490: 6e66 6f22 5d20 3d20 6578 6973 7469 6e67  nfo"] = existing
+000084a0: 5f69 6e66 6f5b 685b 2269 6422 5d5d 0a20  _info[h["id"]]. 
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000084c0: 2063 7265 6174 6520 636f 6c75 6d6e 7320   create columns 
+000084d0: 7769 7468 2074 7970 6573 2075 7365 7220  with types user 
+000084e0: 7265 7175 6573 7465 640a 2020 2020 2020  requested.      
+000084f0: 2020 2020 2020 2020 2020 7479 7065 5f6f            type_o
+00008500: 7665 7272 6964 6520 3d20 6578 6973 7469  verride = existi
+00008510: 6e67 5f69 6e66 6f5b 685b 2269 6422 5d5d  ng_info[h["id"]]
+00008520: 2e67 6574 2822 7479 7065 5f6f 7665 7272  .get("type_overr
+00008530: 6964 6522 290a 2020 2020 2020 2020 2020  ide").          
+00008540: 2020 2020 2020 6966 2074 7970 655f 6f76        if type_ov
+00008550: 6572 7269 6465 2069 6e20 6c69 7374 2874  erride in list(t
+00008560: 7970 655f 6d61 7070 696e 672e 7661 6c75  ype_mapping.valu
+00008570: 6573 2829 293a 0a20 2020 2020 2020 2020  es()):.         
+00008580: 2020 2020 2020 2020 2020 2068 5b22 7479             h["ty
+00008590: 7065 225d 203d 2074 7970 655f 6f76 6572  pe"] = type_over
+000085a0: 7269 6465 0a0a 2020 2020 6c6f 6767 6572  ride..    logger
+000085b0: 2e69 6e66 6f28 0a20 2020 2020 2020 2022  .info(.        "
+000085c0: 4465 7465 726d 696e 6564 2068 6561 6465  Determined heade
+000085d0: 7273 2061 6e64 2074 7970 6573 3a20 7b68  rs and types: {h
+000085e0: 6561 6465 7273 7d2e 2e2e 222e 666f 726d  eaders}...".form
+000085f0: 6174 2868 6561 6465 7273 3d68 6561 6465  at(headers=heade
+00008600: 7273 5f64 6963 7473 290a 2020 2020 290a  rs_dicts).    ).
+00008610: 0a20 2020 2023 202d 2d2d 2d2d 2d2d 2d2d  .    # ---------
+00008620: 2d2d 2d2d 2d2d 2d2d 2d2d 2044 6f20 7765  ---------- Do we
+00008630: 206e 6565 6420 746f 2063 7265 6174 6520   need to create 
+00008640: 6120 5072 6576 6965 773f 2020 2d2d 2d2d  a Preview?  ----
+00008650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008660: 2d2d 2d0a 2020 2020 2320 6966 2050 5245  ---.    # if PRE
+00008670: 5649 4557 5f52 4f57 5320 6973 206e 6f74  VIEW_ROWS is not
+00008680: 207a 6572 6f2c 2063 7265 6174 6520 6120   zero, create a 
+00008690: 7072 6576 6965 7720 7573 696e 6720 7173  preview using qs
+000086a0: 7620 736c 6963 650a 2020 2020 2320 7765  v slice.    # we
+000086b0: 2064 6f20 7468 6520 726f 7773 5f74 6f5f   do the rows_to_
+000086c0: 636f 7079 203e 2070 7265 7669 6577 5f72  copy > preview_r
+000086d0: 6f77 7320 746f 2063 6865 636b 2069 6620  ows to check if 
+000086e0: 7765 2064 6f6e 2774 206e 6565 6420 746f  we don't need to
+000086f0: 2073 6c69 6365 0a20 2020 2023 2074 6865   slice.    # the
+00008700: 2043 5356 2061 6e79 6d6f 7265 2069 6620   CSV anymore if 
+00008710: 7765 206f 6e6c 7920 6469 6420 6120 7061  we only did a pa
+00008720: 7274 6961 6c20 646f 776e 6c6f 6164 206f  rtial download o
+00008730: 6620 4e20 7072 6576 6965 775f 726f 7773  f N preview_rows
+00008740: 2061 6c72 6561 6479 0a20 2020 2072 6f77   already.    row
+00008750: 735f 746f 5f63 6f70 7920 3d20 7265 636f  s_to_copy = reco
+00008760: 7264 5f63 6f75 6e74 0a20 2020 2069 6620  rd_count.    if 
+00008770: 7072 6576 6965 775f 726f 7773 2061 6e64  preview_rows and
+00008780: 2072 6563 6f72 645f 636f 756e 7420 3e20   record_count > 
+00008790: 7072 6576 6965 775f 726f 7773 3a0a 2020  preview_rows:.  
+000087a0: 2020 2020 2020 6966 2070 7265 7669 6577        if preview
+000087b0: 5f72 6f77 7320 3e20 303a 0a20 2020 2020  _rows > 0:.     
+000087c0: 2020 2020 2020 2023 2050 5245 5649 4557         # PREVIEW
+000087d0: 5f52 4f57 5320 6973 2070 6f73 6974 6976  _ROWS is positiv
+000087e0: 652c 2073 6c69 6365 2066 726f 6d20 7468  e, slice from th
+000087f0: 6520 6265 6769 6e6e 696e 670a 2020 2020  e beginning.    
+00008800: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00008810: 6e66 6f28 2250 7265 7061 7269 6e67 207b  nfo("Preparing {
+00008820: 3a2c 7d2d 726f 7720 7072 6576 6965 772e  :,}-row preview.
+00008830: 2e2e 222e 666f 726d 6174 2870 7265 7669  ..".format(previ
+00008840: 6577 5f72 6f77 7329 290a 2020 2020 2020  ew_rows)).      
+00008850: 2020 2020 2020 7173 765f 736c 6963 655f        qsv_slice_
+00008860: 6373 7620 3d20 7465 6d70 6669 6c65 2e4e  csv = tempfile.N
+00008870: 616d 6564 5465 6d70 6f72 6172 7946 696c  amedTemporaryFil
+00008880: 6528 7375 6666 6978 3d22 2e63 7376 2229  e(suffix=".csv")
+00008890: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+000088a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000088b0: 2020 7173 765f 736c 6963 6520 3d20 7375    qsv_slice = su
+000088c0: 6270 726f 6365 7373 2e72 756e 280a 2020  bprocess.run(.  
+000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088e0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+000088f0: 2020 2020 2020 2020 2020 2020 7173 765f              qsv_
+00008900: 6269 6e2c 0a20 2020 2020 2020 2020 2020  bin,.           
+00008910: 2020 2020 2020 2020 2020 2020 2022 736c               "sl
+00008920: 6963 6522 2c0a 2020 2020 2020 2020 2020  ice",.          
+00008930: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+00008940: 2d6c 656e 222c 0a20 2020 2020 2020 2020  -len",.         
+00008950: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008960: 7472 2870 7265 7669 6577 5f72 6f77 7329  tr(preview_rows)
+00008970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008980: 2020 2020 2020 2020 2020 746d 702e 6e61            tmp.na
+00008990: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000089a0: 2020 2020 2020 2020 2020 2020 222d 2d6f              "--o
+000089b0: 7574 7075 7422 2c0a 2020 2020 2020 2020  utput",.        
+000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089d0: 7173 765f 736c 6963 655f 6373 762e 6e61  qsv_slice_csv.na
+000089e0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000089f0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00008a00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00008a10: 6865 636b 3d54 7275 652c 0a20 2020 2020  heck=True,.     
+00008a20: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00008a30: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00008a40: 7375 6270 726f 6365 7373 2e43 616c 6c65  subprocess.Calle
+00008a50: 6450 726f 6365 7373 4572 726f 7220 6173  dProcessError as
+00008a60: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
+00008a70: 2020 2020 7261 6973 6520 7574 696c 2e4a      raise util.J
+00008a80: 6f62 4572 726f 7228 2243 616e 6e6f 7420  obError("Cannot 
+00008a90: 6372 6561 7465 2061 2070 7265 7669 6577  create a preview
+00008aa0: 2073 6c69 6365 3a20 7b7d 222e 666f 726d   slice: {}".form
+00008ab0: 6174 2865 2929 0a20 2020 2020 2020 2020  at(e)).         
+00008ac0: 2020 2072 6f77 735f 746f 5f63 6f70 7920     rows_to_copy 
+00008ad0: 3d20 7072 6576 6965 775f 726f 7773 0a20  = preview_rows. 
+00008ae0: 2020 2020 2020 2020 2020 2074 6d70 203d             tmp =
+00008af0: 2071 7376 5f73 6c69 6365 5f63 7376 0a20   qsv_slice_csv. 
+00008b00: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00008b10: 2020 2020 2020 2020 2023 2050 5245 5649           # PREVI
+00008b20: 4557 5f52 4f57 5320 6973 206e 6567 6174  EW_ROWS is negat
+00008b30: 6976 652c 2073 6c69 6365 2066 726f 6d20  ive, slice from 
+00008b40: 7468 6520 656e 640a 2020 2020 2020 2020  the end.        
+00008b50: 2020 2020 2320 544f 444f 3a20 646f 2068      # TODO: do h
+00008b60: 7474 7020 7261 6e67 6520 7265 7175 6573  ttp range reques
+00008b70: 7420 736f 2077 6520 646f 6e27 7420 6861  t so we don't ha
+00008b80: 7665 2074 6f20 646f 776e 6c6f 6164 2074  ve to download t
+00008b90: 6865 2077 686f 6c65 2066 696c 650a 2020  he whole file.  
+00008ba0: 2020 2020 2020 2020 2020 2320 746f 2073            # to s
+00008bb0: 6c69 6365 2066 726f 6d20 7468 6520 656e  lice from the en
+00008bc0: 640a 2020 2020 2020 2020 2020 2020 736c  d.            sl
+00008bd0: 6963 655f 6c65 6e20 3d20 6162 7328 7072  ice_len = abs(pr
+00008be0: 6576 6965 775f 726f 7773 290a 2020 2020  eview_rows).    
+00008bf0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00008c00: 6e66 6f28 2250 7265 7061 7269 6e67 207b  nfo("Preparing {
+00008c10: 3a2c 7d2d 726f 7720 7072 6576 6965 7720  :,}-row preview 
+00008c20: 6672 6f6d 2074 6865 2065 6e64 2e2e 2e22  from the end..."
+00008c30: 2e66 6f72 6d61 7428 736c 6963 655f 6c65  .format(slice_le
+00008c40: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
+00008c50: 7173 765f 736c 6963 655f 6373 7620 3d20  qsv_slice_csv = 
+00008c60: 7465 6d70 6669 6c65 2e4e 616d 6564 5465  tempfile.NamedTe
+00008c70: 6d70 6f72 6172 7946 696c 6528 7375 6666  mporaryFile(suff
+00008c80: 6978 3d22 2e63 7376 2229 0a20 2020 2020  ix=".csv").     
+00008c90: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00008ca0: 2020 2020 2020 2020 2020 2020 7173 765f              qsv_
+00008cb0: 736c 6963 6520 3d20 7375 6270 726f 6365  slice = subproce
+00008cc0: 7373 2e72 756e 280a 2020 2020 2020 2020  ss.run(.        
+00008cd0: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cf0: 2020 2020 2020 7173 765f 6269 6e2c 0a20        qsv_bin,. 
+00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d10: 2020 2020 2020 2022 736c 6963 6522 2c0a         "slice",.
+00008d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d30: 2020 2020 2020 2020 222d 2d73 7461 7274          "--start
+00008d40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00008d50: 2020 2020 2020 2020 2020 2022 2d31 222c             "-1",
+00008d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008d70: 2020 2020 2020 2020 2022 2d2d 6c65 6e22           "--len"
+00008d80: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008d90: 2020 2020 2020 2020 2020 7374 7228 736c            str(sl
+00008da0: 6963 655f 6c65 6e29 2c0a 2020 2020 2020  ice_len),.      
+00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008dc0: 2020 746d 702e 6e61 6d65 2c0a 2020 2020    tmp.name,.    
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 2020 2020 222d 2d6f 7574 7075 7422 2c0a      "--output",.
+00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e00: 2020 2020 2020 2020 7173 765f 736c 6963          qsv_slic
+00008e10: 655f 6373 762e 6e61 6d65 2c0a 2020 2020  e_csv.name,.    
+00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e30: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00008e40: 2020 2020 2020 2063 6865 636b 3d54 7275         check=Tru
+00008e50: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00008e60: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00008e70: 2065 7863 6570 7420 7375 6270 726f 6365   except subproce
+00008e80: 7373 2e43 616c 6c65 6450 726f 6365 7373  ss.CalledProcess
+00008e90: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+00008ea0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00008eb0: 6520 7574 696c 2e4a 6f62 4572 726f 7228  e util.JobError(
+00008ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008ed0: 2020 2020 2022 4361 6e6e 6f74 2063 7265       "Cannot cre
+00008ee0: 6174 6520 6120 7072 6576 6965 7720 736c  ate a preview sl
+00008ef0: 6963 6520 6672 6f6d 2074 6865 2065 6e64  ice from the end
+00008f00: 3a20 7b7d 222e 666f 726d 6174 2865 290a  : {}".format(e).
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 290a 2020 2020 2020 2020 2020 2020 726f  ).            ro
+00008f30: 7773 5f74 6f5f 636f 7079 203d 2073 6c69  ws_to_copy = sli
+00008f40: 6365 5f6c 656e 0a20 2020 2020 2020 2020  ce_len.         
+00008f50: 2020 2074 6d70 203d 2071 7376 5f73 6c69     tmp = qsv_sli
+00008f60: 6365 5f63 7376 0a0a 2020 2020 2320 2d2d  ce_csv..    # --
+00008f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 204e  -------------- N
+00008f80: 6f72 6d61 6c69 7a65 2064 6174 6573 2074  ormalize dates t
+00008f90: 6f20 5246 4333 3333 3920 666f 726d 6174  o RFC3339 format
+00008fa0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00008fb0: 2d2d 2d2d 2d0a 2020 2020 2320 6966 2074  -----.    # if t
+00008fc0: 6865 7265 2061 7265 2061 6e79 2064 6174  here are any dat
+00008fd0: 6574 696d 6520 6669 656c 6473 2c20 6e6f  etime fields, no
+00008fe0: 726d 616c 697a 6520 7468 656d 2074 6f20  rmalize them to 
+00008ff0: 5246 4333 3333 3920 666f 726d 6174 0a20  RFC3339 format. 
+00009000: 2020 2023 2073 6f20 7765 2063 616e 2072     # so we can r
+00009010: 6561 6469 6c79 2069 6e73 6572 7420 7468  eadily insert th
+00009020: 656d 2061 7320 7469 6d65 7374 616d 7073  em as timestamps
+00009030: 2069 6e74 6f20 706f 7374 6772 6573 716c   into postgresql
+00009040: 2077 6974 6820 434f 5059 0a20 2020 2069   with COPY.    i
+00009050: 6620 6461 7465 7469 6d65 636f 6c73 5f6c  f datetimecols_l
+00009060: 6973 743a 0a20 2020 2020 2020 2071 7376  ist:.        qsv
+00009070: 5f61 7070 6c79 6470 5f63 7376 203d 2074  _applydp_csv = t
+00009080: 656d 7066 696c 652e 4e61 6d65 6454 656d  empfile.NamedTem
+00009090: 706f 7261 7279 4669 6c65 2873 7566 6669  poraryFile(suffi
+000090a0: 783d 222e 6373 7622 290a 2020 2020 2020  x=".csv").      
+000090b0: 2020 6461 7465 636f 6c73 203d 2022 2c22    datecols = ","
+000090c0: 2e6a 6f69 6e28 6461 7465 7469 6d65 636f  .join(datetimeco
+000090d0: 6c73 5f6c 6973 7429 0a0a 2020 2020 2020  ls_list)..      
+000090e0: 2020 7173 765f 6170 706c 7964 705f 636d    qsv_applydp_cm
+000090f0: 6420 3d20 5b0a 2020 2020 2020 2020 2020  d = [.          
+00009100: 2020 7173 765f 6269 6e2c 0a20 2020 2020    qsv_bin,.     
+00009110: 2020 2020 2020 2022 6170 706c 7964 7022         "applydp"
+00009120: 2c0a 2020 2020 2020 2020 2020 2020 2264  ,.            "d
+00009130: 6174 6566 6d74 222c 0a20 2020 2020 2020  atefmt",.       
+00009140: 2020 2020 2064 6174 6563 6f6c 732c 0a20       datecols,. 
+00009150: 2020 2020 2020 2020 2020 2074 6d70 2e6e             tmp.n
+00009160: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00009170: 2022 2d2d 6f75 7470 7574 222c 0a20 2020   "--output",.   
+00009180: 2020 2020 2020 2020 2071 7376 5f61 7070           qsv_app
+00009190: 6c79 6470 5f63 7376 2e6e 616d 652c 0a20  lydp_csv.name,. 
+000091a0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+000091b0: 2069 6620 7072 6566 6572 5f64 6d79 3a0a   if prefer_dmy:.
+000091c0: 2020 2020 2020 2020 2020 2020 7173 765f              qsv_
+000091d0: 6170 706c 7964 705f 636d 642e 6170 7065  applydp_cmd.appe
+000091e0: 6e64 2822 2d2d 7072 6566 6572 5f64 6d79  nd("--prefer_dmy
+000091f0: 2229 0a20 2020 2020 2020 206c 6f67 6765  ").        logge
+00009200: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
+00009210: 2020 2020 2746 6f72 6d61 7474 696e 6720      'Formatting 
+00009220: 6461 7465 7320 227b 7d22 2074 6f20 4953  dates "{}" to IS
+00009230: 4f20 3836 3031 2f52 4643 2033 3333 3920  O 8601/RFC 3339 
+00009240: 666f 726d 6174 2077 6974 6820 5052 4546  format with PREF
+00009250: 4552 5f44 4d59 3a20 7b7d 2e2e 2e27 2e66  ER_DMY: {}...'.f
+00009260: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+00009270: 2020 2020 2020 2064 6174 6563 6f6c 732c         datecols,
+00009280: 2070 7265 6665 725f 646d 790a 2020 2020   prefer_dmy.    
+00009290: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000092a0: 2020 290a 2020 2020 2020 2020 7472 793a    ).        try:
+000092b0: 0a20 2020 2020 2020 2020 2020 2071 7376  .            qsv
+000092c0: 5f61 7070 6c79 6470 203d 2073 7562 7072  _applydp = subpr
+000092d0: 6f63 6573 732e 7275 6e28 7173 765f 6170  ocess.run(qsv_ap
+000092e0: 706c 7964 705f 636d 642c 2063 6865 636b  plydp_cmd, check
+000092f0: 3d54 7275 6529 0a20 2020 2020 2020 2065  =True).        e
+00009300: 7863 6570 7420 7375 6270 726f 6365 7373  xcept subprocess
+00009310: 2e43 616c 6c65 6450 726f 6365 7373 4572  .CalledProcessEr
+00009320: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
+00009330: 2020 2020 2020 7261 6973 6520 7574 696c        raise util
+00009340: 2e4a 6f62 4572 726f 7228 2241 7070 6c79  .JobError("Apply
+00009350: 6470 2065 7272 6f72 3a20 7b7d 222e 666f  dp error: {}".fo
+00009360: 726d 6174 2865 2929 0a20 2020 2020 2020  rmat(e)).       
+00009370: 2074 6d70 203d 2071 7376 5f61 7070 6c79   tmp = qsv_apply
+00009380: 6470 5f63 7376 0a0a 2020 2020 2320 2d2d  dp_csv..    # --
+00009390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000093a0: 2d2d 2051 5356 2041 4e41 4c59 5349 5320  -- QSV ANALYSIS 
+000093b0: 444f 4e45 202d 2d2d 2d2d 2d2d 2d2d 2d2d  DONE -----------
+000093c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 616e  ---------.    an
+000093d0: 616c 7973 6973 5f65 6c61 7073 6564 203d  alysis_elapsed =
+000093e0: 2074 696d 652e 7065 7266 5f63 6f75 6e74   time.perf_count
+000093f0: 6572 2829 202d 2061 6e61 6c79 7369 735f  er() - analysis_
+00009400: 7374 6172 740a 2020 2020 6c6f 6767 6572  start.    logger
+00009410: 2e69 6e66 6f28 0a20 2020 2020 2020 2022  .info(.        "
+00009420: 414e 414c 5953 4953 2044 4f4e 4521 2041  ANALYSIS DONE! A
+00009430: 6e61 6c79 7a65 6420 616e 6420 7072 6570  nalyzed and prep
+00009440: 7065 6420 696e 207b 3a2c 2e32 667d 2073  ped in {:,.2f} s
+00009450: 6563 6f6e 6473 2e22 2e66 6f72 6d61 7428  econds.".format(
+00009460: 0a20 2020 2020 2020 2020 2020 2061 6e61  .            ana
+00009470: 6c79 7369 735f 656c 6170 7365 640a 2020  lysis_elapsed.  
+00009480: 2020 2020 2020 290a 2020 2020 290a 0a20        ).    ).. 
+00009490: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 2d2d     # -----------
+000094a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000094b0: 2d2d 2050 4949 2053 6372 6565 6e69 6e67  -- PII Screening
+000094c0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000094d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+000094e0: 2020 2020 2320 7765 2073 6361 6e20 666f      # we scan fo
+000094f0: 7220 5065 7273 6f6e 616c 6c79 2049 6465  r Personally Ide
+00009500: 6e74 6966 6961 626c 6520 496e 666f 726d  ntifiable Inform
+00009510: 6174 696f 6e20 2850 4949 2920 7573 696e  ation (PII) usin
+00009520: 6720 7173 7627 7320 706f 7765 7266 756c  g qsv's powerful
+00009530: 0a20 2020 2023 2073 6561 7263 6873 6574  .    # searchset
+00009540: 2063 6f6d 6d61 6e64 2077 6869 6368 2063   command which c
+00009550: 616e 2053 494d 554c 5441 4e45 4f55 534c  an SIMULTANEOUSL
+00009560: 5920 636f 6d70 6172 6520 7365 7665 7261  Y compare severa
+00009570: 6c20 7265 6765 7865 7320 7065 720a 2020  l regexes per.  
+00009580: 2020 2320 6669 656c 6420 696e 206f 6e65    # field in one
+00009590: 2070 6173 730a 2020 2020 7069 6973 6372   pass.    piiscr
+000095a0: 6565 6e69 6e67 5f73 7461 7274 203d 2030  eening_start = 0
+000095b0: 0a20 2020 2070 6969 7363 7265 656e 696e  .    piiscreenin
+000095c0: 675f 656c 6170 7365 6420 3d20 300a 2020  g_elapsed = 0.  
+000095d0: 2020 6966 2063 6f6e 6669 672e 6765 7428    if config.get(
+000095e0: 2250 4949 5f53 4352 4545 4e49 4e47 2229  "PII_SCREENING")
+000095f0: 3a0a 2020 2020 2020 2020 7069 6973 6372  :.        piiscr
+00009600: 6565 6e69 6e67 5f73 7461 7274 203d 2074  eening_start = t
+00009610: 696d 652e 7065 7266 5f63 6f75 6e74 6572  ime.perf_counter
+00009620: 2829 0a20 2020 2020 2020 2070 6969 5f66  ().        pii_f
+00009630: 6f75 6e64 5f61 626f 7274 203d 2063 6f6e  ound_abort = con
+00009640: 6669 672e 6765 7428 2250 4949 5f46 4f55  fig.get("PII_FOU
+00009650: 4e44 5f41 424f 5254 2229 0a0a 2020 2020  ND_ABORT")..    
+00009660: 2020 2020 2320 4450 2b20 636f 6d65 7320      # DP+ comes 
+00009670: 7769 7468 2064 6566 6175 6c74 2072 6567  with default reg
+00009680: 6578 2070 6174 7465 726e 7320 666f 7220  ex patterns for 
+00009690: 5049 4920 2853 534e 2c20 6372 6564 6974  PII (SSN, credit
+000096a0: 2063 6172 6473 2c0a 2020 2020 2020 2020   cards,.        
+000096b0: 2320 656d 6169 6c2c 2062 616e 6b20 6163  # email, bank ac
+000096c0: 636f 756e 7420 6e75 6d62 6572 732c 2026  count numbers, &
+000096d0: 2070 686f 6e65 206e 756d 6265 7229 2e20   phone number). 
+000096e0: 5468 6520 4450 2b20 6164 6d69 6e20 6361  The DP+ admin ca
+000096f0: 6e0a 2020 2020 2020 2020 2320 7573 6520  n.        # use 
+00009700: 6120 6375 7374 6f6d 2073 6574 206f 6620  a custom set of 
+00009710: 7265 6765 7820 7061 7474 6572 6e73 2062  regex patterns b
+00009720: 7920 706f 696e 7469 6e67 2074 6f20 6120  y pointing to a 
+00009730: 7265 736f 7572 6365 2077 6974 680a 2020  resource with.  
+00009740: 2020 2020 2020 2320 6120 7465 7874 2066        # a text f
+00009750: 696c 652c 2077 6974 6820 6561 6368 206c  ile, with each l
+00009760: 696e 6520 6861 7669 6e67 2061 2072 6567  ine having a reg
+00009770: 6578 2070 6174 7465 726e 2c20 616e 6420  ex pattern, and 
+00009780: 616e 206f 7074 696f 6e61 6c0a 2020 2020  an optional.    
+00009790: 2020 2020 2320 6c61 6265 6c20 636f 6d6d      # label comm
+000097a0: 656e 7420 7072 6566 6978 6564 2077 6974  ent prefixed wit
+000097b0: 6820 2223 2220 2865 2e67 2e20 2353 534e  h "#" (e.g. #SSN
+000097c0: 2c20 2345 6d61 696c 2c20 2356 6973 612c  , #Email, #Visa,
+000097d0: 2065 7463 2e29 0a20 2020 2020 2020 2070   etc.).        p
+000097e0: 6969 5f72 6567 6578 5f72 6573 6f75 7263  ii_regex_resourc
+000097f0: 655f 6964 203d 2063 6f6e 6669 672e 6765  e_id = config.ge
+00009800: 7428 2250 4949 5f52 4547 4558 5f52 4553  t("PII_REGEX_RES
+00009810: 4f55 5243 455f 4944 5f4f 525f 414c 4941  OURCE_ID_OR_ALIA
+00009820: 5322 290a 2020 2020 2020 2020 6966 2070  S").        if p
+00009830: 6969 5f72 6567 6578 5f72 6573 6f75 7263  ii_regex_resourc
+00009840: 655f 6964 3a0a 2020 2020 2020 2020 2020  e_id:.          
+00009850: 2020 7069 695f 7265 6765 785f 7265 736f    pii_regex_reso
+00009860: 7572 6365 5f65 7869 7374 203d 2064 6174  urce_exist = dat
+00009870: 6173 746f 7265 5f72 6573 6f75 7263 655f  astore_resource_
+00009880: 6578 6973 7473 280a 2020 2020 2020 2020  exists(.        
+00009890: 2020 2020 2020 2020 7069 695f 7265 6765          pii_rege
+000098a0: 785f 7265 736f 7572 6365 5f69 642c 2061  x_resource_id, a
+000098b0: 7069 5f6b 6579 2c20 636b 616e 5f75 726c  pi_key, ckan_url
+000098c0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+000098d0: 2020 2020 2020 2020 2020 2069 6620 7069             if pi
+000098e0: 695f 7265 6765 785f 7265 736f 7572 6365  i_regex_resource
+000098f0: 5f65 7869 7374 3a0a 2020 2020 2020 2020  _exist:.        
+00009900: 2020 2020 2020 2020 7069 695f 7265 736f          pii_reso
+00009910: 7572 6365 203d 2067 6574 5f72 6573 6f75  urce = get_resou
+00009920: 7263 6528 7069 695f 7265 6765 785f 7265  rce(pii_regex_re
+00009930: 736f 7572 6365 5f69 642c 2063 6b61 6e5f  source_id, ckan_
+00009940: 7572 6c2c 2061 7069 5f6b 6579 290a 2020  url, api_key).  
+00009950: 2020 2020 2020 2020 2020 2020 2020 7069                pi
+00009960: 695f 7265 6765 785f 7572 6c20 3d20 7069  i_regex_url = pi
+00009970: 695f 7265 736f 7572 6365 5b22 7572 6c22  i_resource["url"
+00009980: 5d0a 0a20 2020 2020 2020 2020 2020 2020  ]..             
+00009990: 2020 2072 203d 2072 6571 7565 7374 732e     r = requests.
+000099a0: 6765 7428 7069 695f 7265 6765 785f 7572  get(pii_regex_ur
+000099b0: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
+000099c0: 2020 2070 6969 5f72 6567 6578 5f66 696c     pii_regex_fil
+000099d0: 6520 3d20 7069 695f 7265 6765 785f 7572  e = pii_regex_ur
+000099e0: 6c2e 7370 6c69 7428 222f 2229 5b2d 315d  l.split("/")[-1]
+000099f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009a00: 2020 7020 3d20 5061 7468 285f 5f66 696c    p = Path(__fil
+00009a10: 655f 5f29 2e77 6974 685f 6e61 6d65 2822  e__).with_name("
+00009a20: 7573 6572 2d70 6969 2d72 6567 6578 6573  user-pii-regexes
+00009a30: 2e74 7874 2229 0a20 2020 2020 2020 2020  .txt").         
+00009a40: 2020 2020 2020 2077 6974 6820 702e 6f70         with p.op
+00009a50: 656e 2822 7762 2229 2061 7320 663a 0a20  en("wb") as f:. 
+00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a70: 2020 2066 2e77 7269 7465 2872 2e63 6f6e     f.write(r.con
+00009a80: 7465 6e74 290a 2020 2020 2020 2020 656c  tent).        el
+00009a90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009aa0: 7069 695f 7265 6765 785f 6669 6c65 203d  pii_regex_file =
+00009ab0: 2022 6465 6661 756c 742d 7069 692d 7265   "default-pii-re
+00009ac0: 6765 7865 732e 7478 7422 0a20 2020 2020  gexes.txt".     
+00009ad0: 2020 2020 2020 2070 203d 2050 6174 6828         p = Path(
+00009ae0: 5f5f 6669 6c65 5f5f 292e 7769 7468 5f6e  __file__).with_n
+00009af0: 616d 6528 7069 695f 7265 6765 785f 6669  ame(pii_regex_fi
+00009b00: 6c65 290a 0a20 2020 2020 2020 2070 6969  le)..        pii
+00009b10: 5f66 6f75 6e64 203d 2046 616c 7365 0a20  _found = False. 
+00009b20: 2020 2020 2020 2070 6969 5f72 6567 6578         pii_regex
+00009b30: 5f66 6e61 6d65 203d 2070 2e61 6273 6f6c  _fname = p.absol
+00009b40: 7574 6528 290a 0a20 2020 2020 2020 2070  ute()..        p
+00009b50: 6969 5f71 7569 636b 5f73 6372 6565 6e20  ii_quick_screen 
+00009b60: 3d20 636f 6e66 6967 2e67 6574 2822 5049  = config.get("PI
+00009b70: 495f 5155 4943 4b5f 5343 5245 454e 2229  I_QUICK_SCREEN")
+00009b80: 0a20 2020 2020 2020 2069 6620 7069 695f  .        if pii_
+00009b90: 7175 6963 6b5f 7363 7265 656e 3a0a 2020  quick_screen:.  
+00009ba0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00009bb0: 2e69 6e66 6f28 2251 7569 636b 6c79 2073  .info("Quickly s
+00009bc0: 6361 6e6e 696e 6720 666f 7220 5049 4920  canning for PII 
+00009bd0: 7573 696e 6720 7b7d 2e2e 2e22 2e66 6f72  using {}...".for
+00009be0: 6d61 7428 7069 695f 7265 6765 785f 6669  mat(pii_regex_fi
+00009bf0: 6c65 2929 0a20 2020 2020 2020 2020 2020  le)).           
+00009c00: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00009c10: 2020 2020 2020 7173 765f 7365 6172 6368        qsv_search
+00009c20: 7365 7420 3d20 7375 6270 726f 6365 7373  set = subprocess
+00009c30: 2e72 756e 280a 2020 2020 2020 2020 2020  .run(.          
+00009c40: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 2020 2020 7173 765f 6269 6e2c 0a20 2020      qsv_bin,.   
+00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c80: 2020 2020 2022 7365 6172 6368 7365 7422       "searchset"
+00009c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009ca0: 2020 2020 2020 2020 2020 222d 2d69 676e            "--ign
+00009cb0: 6f72 652d 6361 7365 222c 0a20 2020 2020  ore-case",.     
+00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cd0: 2020 2022 2d2d 7175 6963 6b22 2c0a 2020     "--quick",.  
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cf0: 2020 2020 2020 7069 695f 7265 6765 785f        pii_regex_
+00009d00: 666e 616d 652c 0a20 2020 2020 2020 2020  fname,.         
+00009d10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00009d20: 6d70 2e6e 616d 652c 0a20 2020 2020 2020  mp.name,.       
+00009d30: 2020 2020 2020 2020 2020 2020 205d 2c0a               ],.
+00009d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d50: 2020 2020 6361 7074 7572 655f 6f75 7470      capture_outp
+00009d60: 7574 3d54 7275 652c 0a20 2020 2020 2020  ut=True,.       
+00009d70: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+00009d80: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
+00009d90: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009da0: 2020 2020 2020 6578 6365 7074 2073 7562        except sub
+00009db0: 7072 6f63 6573 732e 4361 6c6c 6564 5072  process.CalledPr
+00009dc0: 6f63 6573 7345 7272 6f72 2061 7320 653a  ocessError as e:
+00009dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009de0: 2072 6169 7365 2075 7469 6c2e 4a6f 6245   raise util.JobE
+00009df0: 7272 6f72 2822 4361 6e6e 6f74 2071 7569  rror("Cannot qui
+00009e00: 636b 6c79 2073 6561 7263 6820 4353 5620  ckly search CSV 
+00009e10: 666f 7220 5049 493a 207b 7d22 2e66 6f72  for PII: {}".for
+00009e20: 6d61 7428 6529 290a 2020 2020 2020 2020  mat(e)).        
+00009e30: 2020 2020 7069 695f 6361 6e64 6964 6174      pii_candidat
+00009e40: 655f 726f 7720 3d20 7374 7228 7173 765f  e_row = str(qsv_
+00009e50: 7365 6172 6368 7365 742e 7374 6465 7272  searchset.stderr
+00009e60: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00009e70: 2070 6969 5f63 616e 6469 6461 7465 5f72   pii_candidate_r
+00009e80: 6f77 3a0a 2020 2020 2020 2020 2020 2020  ow:.            
+00009e90: 2020 2020 7069 695f 666f 756e 6420 3d20      pii_found = 
+00009ea0: 5472 7565 0a0a 2020 2020 2020 2020 656c  True..        el
+00009eb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00009ec0: 6c6f 6767 6572 2e69 6e66 6f28 2253 6361  logger.info("Sca
+00009ed0: 6e6e 696e 6720 666f 7220 5049 4920 7573  nning for PII us
+00009ee0: 696e 6720 7b7d 2e2e 2e22 2e66 6f72 6d61  ing {}...".forma
+00009ef0: 7428 7069 695f 7265 6765 785f 6669 6c65  t(pii_regex_file
+00009f00: 2929 0a20 2020 2020 2020 2020 2020 2071  )).            q
+00009f10: 7376 5f73 6561 7263 6873 6574 5f63 7376  sv_searchset_csv
+00009f20: 203d 2074 656d 7066 696c 652e 4e61 6d65   = tempfile.Name
+00009f30: 6454 656d 706f 7261 7279 4669 6c65 2873  dTemporaryFile(s
+00009f40: 7566 6669 783d 222e 6373 7622 290a 2020  uffix=".csv").  
+00009f50: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00009f60: 2020 2020 2020 2020 2020 2020 2020 2071                 q
+00009f70: 7376 5f73 6561 7263 6873 6574 203d 2073  sv_searchset = s
+00009f80: 7562 7072 6f63 6573 732e 7275 6e28 0a20  ubprocess.run(. 
+00009f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fa0: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+00009fb0: 2020 2020 2020 2020 2020 2020 2071 7376               qsv
+00009fc0: 5f62 696e 2c0a 2020 2020 2020 2020 2020  _bin,.          
+00009fd0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00009fe0: 6561 7263 6873 6574 222c 0a20 2020 2020  earchset",.     
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a000: 2020 2022 2d2d 6967 6e6f 7265 2d63 6173     "--ignore-cas
+0000a010: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+0000a020: 2020 2020 2020 2020 2020 2020 222d 2d66              "--f
+0000a030: 6c61 6722 2c0a 2020 2020 2020 2020 2020  lag",.          
+0000a040: 2020 2020 2020 2020 2020 2020 2020 2250                "P
+0000a050: 4949 5f69 6e66 6f22 2c0a 2020 2020 2020  II_info",.      
+0000a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a070: 2020 222d 2d66 6c61 672d 6d61 7463 6865    "--flag-matche
+0000a080: 732d 6f6e 6c79 222c 0a20 2020 2020 2020  s-only",.       
+0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0a0: 2022 2d2d 6a73 6f6e 222c 0a20 2020 2020   "--json",.     
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0c0: 2020 2070 6969 5f72 6567 6578 5f66 696c     pii_regex_fil
+0000a0d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000a0e0: 2020 2020 2020 2020 2020 2074 6d70 2e6e             tmp.n
+0000a0f0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+0000a100: 2020 2020 2020 2020 2020 2020 2022 2d2d               "--
+0000a110: 6f75 7470 7574 222c 0a20 2020 2020 2020  output",.       
+0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a130: 2071 7376 5f73 6561 7263 6873 6574 5f63   qsv_searchset_c
+0000a140: 7376 2e6e 616d 652c 0a20 2020 2020 2020  sv.name,.       
+0000a150: 2020 2020 2020 2020 2020 2020 205d 2c0a               ],.
+0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a170: 2020 2020 6361 7074 7572 655f 6f75 7470      capture_outp
+0000a180: 7574 3d54 7275 652c 0a20 2020 2020 2020  ut=True,.       
+0000a190: 2020 2020 2020 2020 2020 2020 2074 6578               tex
+0000a1a0: 743d 5472 7565 2c0a 2020 2020 2020 2020  t=True,.        
+0000a1b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000a1c0: 2020 2020 2020 6578 6365 7074 2073 7562        except sub
+0000a1d0: 7072 6f63 6573 732e 4361 6c6c 6564 5072  process.CalledPr
+0000a1e0: 6f63 6573 7345 7272 6f72 2061 7320 653a  ocessError as e:
+0000a1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a200: 2072 6169 7365 2075 7469 6c2e 4a6f 6245   raise util.JobE
+0000a210: 7272 6f72 2822 4361 6e6e 6f74 2073 6561  rror("Cannot sea
+0000a220: 7263 6820 4353 5620 666f 7220 5049 493a  rch CSV for PII:
+0000a230: 207b 7d22 2e66 6f72 6d61 7428 6529 290a   {}".format(e)).
+0000a240: 2020 2020 2020 2020 2020 2020 7069 695f              pii_
+0000a250: 6a73 6f6e 203d 206a 736f 6e2e 6c6f 6164  json = json.load
+0000a260: 7328 7374 7228 7173 765f 7365 6172 6368  s(str(qsv_search
+0000a270: 7365 742e 7374 6465 7272 2929 0a20 2020  set.stderr)).   
+0000a280: 2020 2020 2020 2020 2070 6969 5f74 6f74           pii_tot
+0000a290: 616c 5f6d 6174 6368 6573 203d 2069 6e74  al_matches = int
+0000a2a0: 2870 6969 5f6a 736f 6e5b 2274 6f74 616c  (pii_json["total
+0000a2b0: 5f6d 6174 6368 6573 225d 290a 2020 2020  _matches"]).    
+0000a2c0: 2020 2020 2020 2020 7069 695f 726f 7773          pii_rows
+0000a2d0: 5f77 6974 685f 6d61 7463 6865 7320 3d20  _with_matches = 
+0000a2e0: 696e 7428 7069 695f 6a73 6f6e 5b22 726f  int(pii_json["ro
+0000a2f0: 7773 5f77 6974 685f 6d61 7463 6865 7322  ws_with_matches"
+0000a300: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
+0000a310: 6620 7069 695f 746f 7461 6c5f 6d61 7463  f pii_total_matc
+0000a320: 6865 7320 3e20 303a 0a20 2020 2020 2020  hes > 0:.       
+0000a330: 2020 2020 2020 2020 2070 6969 5f66 6f75           pii_fou
+0000a340: 6e64 203d 2054 7275 650a 0a20 2020 2020  nd = True..     
+0000a350: 2020 2070 6969 5f73 686f 775f 6361 6e64     pii_show_cand
+0000a360: 6964 6174 6573 203d 2063 6f6e 6669 672e  idates = config.
+0000a370: 6765 7428 2250 4949 5f53 484f 575f 4341  get("PII_SHOW_CA
+0000a380: 4e44 4944 4154 4553 2229 0a20 2020 2020  NDIDATES").     
+0000a390: 2020 2069 6620 7069 695f 666f 756e 6420     if pii_found 
+0000a3a0: 616e 6420 7069 695f 666f 756e 645f 6162  and pii_found_ab
+0000a3b0: 6f72 7420 616e 6420 6e6f 7420 7069 695f  ort and not pii_
+0000a3c0: 7368 6f77 5f63 616e 6469 6461 7465 733a  show_candidates:
+0000a3d0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+0000a3e0: 6765 722e 6572 726f 7228 2250 4949 2043  ger.error("PII C
+0000a3f0: 616e 6469 6461 7465 2f73 2046 6f75 6e64  andidate/s Found
+0000a400: 2122 290a 2020 2020 2020 2020 2020 2020  !").            
+0000a410: 6966 2070 6969 5f71 7569 636b 5f73 6372  if pii_quick_scr
+0000a420: 6565 6e3a 0a20 2020 2020 2020 2020 2020  een:.           
+0000a430: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
+0000a440: 4a6f 6245 7272 6f72 280a 2020 2020 2020  JobError(.      
+0000a450: 2020 2020 2020 2020 2020 2020 2020 2250                "P
+0000a460: 4949 2043 414e 4449 4441 5445 2046 4f55  II CANDIDATE FOU
+0000a470: 4e44 206f 6e20 726f 7720 7b7d 2120 4a6f  ND on row {}! Jo
+0000a480: 6220 6162 6f72 7465 642e 222e 666f 726d  b aborted.".form
+0000a490: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+0000a4a0: 2020 2020 2020 2020 2020 2020 7069 695f              pii_
+0000a4b0: 6361 6e64 6964 6174 655f 726f 772e 7273  candidate_row.rs
+0000a4c0: 7472 6970 2829 0a20 2020 2020 2020 2020  trip().         
+0000a4d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000a4e0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000a4f0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000a500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a510: 2072 6169 7365 2075 7469 6c2e 4a6f 6245   raise util.JobE
+0000a520: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000a530: 2020 2020 2020 2020 2020 2250 4949 2043            "PII C
+0000a540: 414e 4449 4441 5445 2f53 2046 4f55 4e44  ANDIDATE/S FOUND
+0000a550: 2120 4a6f 6220 6162 6f72 7465 642e 2046  ! Job aborted. F
+0000a560: 6f75 6e64 207b 7d20 5049 4920 6361 6e64  ound {} PII cand
+0000a570: 6964 6174 652f 7320 696e 207b 7d20 726f  idate/s in {} ro
+0000a580: 772f 732e 222e 666f 726d 6174 280a 2020  w/s.".format(.  
+0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5a0: 2020 2020 2020 7069 695f 746f 7461 6c5f        pii_total_
+0000a5b0: 6d61 7463 6865 732c 2070 6969 5f72 6f77  matches, pii_row
+0000a5c0: 735f 7769 7468 5f6d 6174 6368 6573 0a20  s_with_matches. 
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5e0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000a5f0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+0000a600: 6c69 6620 7069 695f 666f 756e 6420 616e  lif pii_found an
+0000a610: 6420 7069 695f 7368 6f77 5f63 616e 6469  d pii_show_candi
+0000a620: 6461 7465 7320 616e 6420 6e6f 7420 7069  dates and not pi
+0000a630: 695f 7175 6963 6b5f 7363 7265 656e 3a0a  i_quick_screen:.
+0000a640: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
+0000a650: 444f 3a20 4372 6561 7465 2050 4949 2043  DO: Create PII C
+0000a660: 616e 6469 6461 7465 7320 7265 736f 7572  andidates resour
+0000a670: 6365 2061 6e64 2073 6574 2070 6163 6b61  ce and set packa
+0000a680: 6765 2074 6f20 7072 6976 6174 6520 6966  ge to private if
+0000a690: 2069 7473 206e 6f74 2070 7269 7661 7465   its not private
+0000a6a0: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
+0000a6b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 4372 6561  ----------- Crea
+0000a6c0: 7465 2050 4949 2050 7265 7669 6577 2052  te PII Preview R
+0000a6d0: 6573 6f75 7263 6520 2d2d 2d2d 2d2d 2d2d  esource --------
+0000a6e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0000a6f0: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+0000a700: 726e 696e 6728 0a20 2020 2020 2020 2020  rning(.         
+0000a710: 2020 2020 2020 2022 5049 4920 4341 4e44         "PII CAND
+0000a720: 4944 4154 452f 5320 464f 554e 4421 2046  IDATE/S FOUND! F
+0000a730: 6f75 6e64 207b 7d20 5049 4920 6361 6e64  ound {} PII cand
+0000a740: 6964 6174 652f 7320 696e 207b 7d20 726f  idate/s in {} ro
+0000a750: 772f 732e 2043 7265 6174 696e 6720 5049  w/s. Creating PI
+0000a760: 4920 7072 6576 6965 772e 2e2e 222e 666f  I preview...".fo
+0000a770: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+0000a780: 2020 2020 2020 2020 2020 7069 695f 746f            pii_to
+0000a790: 7461 6c5f 6d61 7463 6865 732c 2070 6969  tal_matches, pii
+0000a7a0: 5f72 6f77 735f 7769 7468 5f6d 6174 6368  _rows_with_match
+0000a7b0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+0000a7c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000a7d0: 2029 0a20 2020 2020 2020 2020 2020 2070   ).            p
+0000a7e0: 6969 5f72 6573 6f75 7263 655f 6964 203d  ii_resource_id =
+0000a7f0: 2072 6573 6f75 7263 655f 6964 202b 2022   resource_id + "
+0000a800: 2d70 6969 220a 0a20 2020 2020 2020 2020  -pii"..         
+0000a810: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000a820: 2020 2020 2020 2020 7261 775f 636f 6e6e          raw_conn
+0000a830: 6563 7469 6f6e 5f70 6969 203d 2070 7379  ection_pii = psy
+0000a840: 636f 7067 322e 636f 6e6e 6563 7428 636f  copg2.connect(co
+0000a850: 6e66 6967 2e67 6574 2822 5752 4954 455f  nfig.get("WRITE_
+0000a860: 454e 4749 4e45 5f55 524c 2229 290a 2020  ENGINE_URL")).  
+0000a870: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0000a880: 2070 7379 636f 7067 322e 4572 726f 7220   psycopg2.Error 
+0000a890: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+0000a8a0: 2020 2020 2020 7261 6973 6520 7574 696c        raise util
+0000a8b0: 2e4a 6f62 4572 726f 7228 2243 6f75 6c64  .JobError("Could
+0000a8c0: 206e 6f74 2063 6f6e 6e65 6374 2074 6f20   not connect to 
+0000a8d0: 7468 6520 4461 7461 7374 6f72 653a 207b  the Datastore: {
+0000a8e0: 7d22 2e66 6f72 6d61 7428 6529 290a 2020  }".format(e)).  
+0000a8f0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000a900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a910: 6375 725f 7069 6920 3d20 7261 775f 636f  cur_pii = raw_co
+0000a920: 6e6e 6563 7469 6f6e 5f70 6969 2e63 7572  nnection_pii.cur
+0000a930: 736f 7228 290a 0a20 2020 2020 2020 2020  sor()..         
+0000a940: 2020 2023 2063 6865 636b 2069 6620 7468     # check if th
+0000a950: 6520 7069 6920 616c 7265 6164 7920 6578  e pii already ex
+0000a960: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
+0000a970: 6578 6973 7469 6e67 5f70 6969 203d 2064  existing_pii = d
+0000a980: 6174 6173 746f 7265 5f72 6573 6f75 7263  atastore_resourc
+0000a990: 655f 6578 6973 7473 2870 6969 5f72 6573  e_exists(pii_res
+0000a9a0: 6f75 7263 655f 6964 2c20 6170 695f 6b65  ource_id, api_ke
+0000a9b0: 792c 2063 6b61 6e5f 7572 6c29 0a0a 2020  y, ckan_url)..  
+0000a9c0: 2020 2020 2020 2020 2020 2320 4465 6c65            # Dele
+0000a9d0: 7465 2065 7869 7374 696e 6720 7069 6920  te existing pii 
+0000a9e0: 7072 6576 6965 7720 6265 666f 7265 2070  preview before p
+0000a9f0: 726f 6365 6564 696e 672e 0a20 2020 2020  roceeding..     
+0000aa00: 2020 2020 2020 2069 6620 6578 6973 7469         if existi
+0000aa10: 6e67 5f70 6969 3a0a 2020 2020 2020 2020  ng_pii:.        
+0000aa20: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000aa30: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+0000aa40: 2020 2020 2020 2020 2027 4465 6c65 7469           'Deleti
+0000aa50: 6e67 2065 7869 7374 696e 6720 5049 4920  ng existing PII 
+0000aa60: 7072 6576 6965 7720 227b 7d22 2e27 2e66  preview "{}".'.f
+0000aa70: 6f72 6d61 7428 7069 695f 7265 736f 7572  ormat(pii_resour
+0000aa80: 6365 5f69 6429 0a20 2020 2020 2020 2020  ce_id).         
+0000aa90: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000aaa0: 2020 2020 2020 2020 2020 6375 725f 7069            cur_pi
+0000aab0: 692e 6578 6563 7574 6528 0a20 2020 2020  i.execute(.     
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000aad0: 5345 4c45 4354 2061 6c69 6173 5f6f 6620  SELECT alias_of 
+0000aae0: 4652 4f4d 205f 7461 626c 655f 6d65 7461  FROM _table_meta
+0000aaf0: 6461 7461 2077 6865 7265 206e 616d 6520  data where name 
+0000ab00: 6c69 6b65 2025 7320 6772 6f75 7020 6279  like %s group by
+0000ab10: 2061 6c69 6173 5f6f 663b 222c 0a20 2020   alias_of;",.   
+0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab30: 2028 7069 695f 7265 736f 7572 6365 5f69   (pii_resource_i
+0000ab40: 6420 2b20 2225 222c 292c 0a20 2020 2020  d + "%",),.     
+0000ab50: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000ab60: 2020 2020 2020 2020 2020 2020 2070 6969               pii
+0000ab70: 5f61 6c69 6173 5f72 6573 756c 7420 3d20  _alias_result = 
+0000ab80: 6375 725f 7069 692e 6665 7463 686f 6e65  cur_pii.fetchone
+0000ab90: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000aba0: 2020 2069 6620 7069 695f 616c 6961 735f     if pii_alias_
+0000abb0: 7265 7375 6c74 3a0a 2020 2020 2020 2020  result:.        
+0000abc0: 2020 2020 2020 2020 2020 2020 6578 6973              exis
+0000abd0: 7469 6e67 5f70 6969 5f61 6c69 6173 5f6f  ting_pii_alias_o
+0000abe0: 6620 3d20 7069 695f 616c 6961 735f 7265  f = pii_alias_re
+0000abf0: 7375 6c74 5b30 5d0a 0a20 2020 2020 2020  sult[0]..       
+0000ac00: 2020 2020 2020 2020 2020 2020 2064 656c               del
+0000ac10: 6574 655f 6461 7461 7374 6f72 655f 7265  ete_datastore_re
+0000ac20: 736f 7572 6365 2865 7869 7374 696e 675f  source(existing_
+0000ac30: 7069 695f 616c 6961 735f 6f66 2c20 6170  pii_alias_of, ap
+0000ac40: 695f 6b65 792c 2063 6b61 6e5f 7572 6c29  i_key, ckan_url)
+0000ac50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ac60: 2020 2020 2064 656c 6574 655f 7265 736f       delete_reso
+0000ac70: 7572 6365 2865 7869 7374 696e 675f 7069  urce(existing_pi
+0000ac80: 695f 616c 6961 735f 6f66 2c20 6170 695f  i_alias_of, api_
+0000ac90: 6b65 792c 2063 6b61 6e5f 7572 6c29 0a0a  key, ckan_url)..
+0000aca0: 2020 2020 2020 2020 2020 2020 7069 695f              pii_
+0000acb0: 616c 6961 7320 3d20 5b70 6969 5f72 6573  alias = [pii_res
+0000acc0: 6f75 7263 655f 6964 5d0a 0a20 2020 2020  ource_id]..     
+0000acd0: 2020 2020 2020 2023 2072 756e 2073 7461         # run sta
+0000ace0: 7473 206f 6e20 7069 6920 7072 6576 6965  ts on pii previe
+0000acf0: 7720 4353 5620 746f 2067 6574 2068 6561  w CSV to get hea
+0000ad00: 6465 7220 6e61 6d65 7320 616e 6420 696e  der names and in
+0000ad10: 6665 7220 6461 7461 2074 7970 6573 0a20  fer data types. 
+0000ad20: 2020 2020 2020 2020 2020 2023 2077 6520             # we 
+0000ad30: 646f 6e27 7420 6e65 6564 2073 756d 6d61  don't need summa
+0000ad40: 7279 2073 7461 7469 7374 6963 732c 2073  ry statistics, s
+0000ad50: 6f20 7573 6520 7468 6520 2d2d 7479 7065  o use the --type
+0000ad60: 736f 6e6c 7920 6f70 7469 6f6e 0a20 2020  sonly option.   
+0000ad70: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+0000ad80: 2020 2020 2020 2020 2020 2020 2020 7173                qs
+0000ad90: 765f 7069 695f 7374 6174 7320 3d20 7375  v_pii_stats = su
+0000ada0: 6270 726f 6365 7373 2e72 756e 280a 2020  bprocess.run(.  
+0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adc0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+0000add0: 2020 2020 2020 2020 2020 2020 7173 765f              qsv_
+0000ade0: 6269 6e2c 0a20 2020 2020 2020 2020 2020  bin,.           
+0000adf0: 2020 2020 2020 2020 2020 2020 2022 7374               "st
+0000ae00: 6174 7322 2c0a 2020 2020 2020 2020 2020  ats",.          
+0000ae10: 2020 2020 2020 2020 2020 2020 2020 222d                "-
+0000ae20: 2d74 7970 6573 6f6e 6c79 222c 0a20 2020  -typesonly",.   
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae40: 2020 2020 2071 7376 5f73 6561 7263 6873       qsv_searchs
+0000ae50: 6574 5f63 7376 2e6e 616d 652c 0a20 2020  et_csv.name,.   
+0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae70: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+0000ae80: 2020 2020 2020 2020 6361 7074 7572 655f          capture_
+0000ae90: 6f75 7470 7574 3d54 7275 652c 0a20 2020  output=True,.   
+0000aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aeb0: 2063 6865 636b 3d54 7275 652c 0a20 2020   check=True,.   
+0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aed0: 2074 6578 743d 5472 7565 2c0a 2020 2020   text=True,.    
+0000aee0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000aef0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0000af00: 2073 7562 7072 6f63 6573 732e 4361 6c6c   subprocess.Call
+0000af10: 6564 5072 6f63 6573 7345 7272 6f72 2061  edProcessError a
+0000af20: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+0000af30: 2020 2020 2072 6169 7365 2075 7469 6c2e       raise util.
+0000af40: 4a6f 6245 7272 6f72 2822 4361 6e6e 6f74  JobError("Cannot
+0000af50: 2072 756e 2073 7461 7473 206f 6e20 5049   run stats on PI
+0000af60: 4920 7072 6576 6965 7720 4353 563a 207b  I preview CSV: {
+0000af70: 7d22 2e66 6f72 6d61 7428 6529 290a 0a20  }".format(e)).. 
+0000af80: 2020 2020 2020 2020 2020 2070 6969 5f73             pii_s
+0000af90: 7461 7473 203d 2073 7472 2871 7376 5f70  tats = str(qsv_p
+0000afa0: 6969 5f73 7461 7473 2e73 7464 6f75 7429  ii_stats.stdout)
+0000afb0: 2e73 7472 6970 2829 0a20 2020 2020 2020  .strip().       
+0000afc0: 2020 2020 2070 6969 5f73 7461 7473 5f64       pii_stats_d
+0000afd0: 6963 7420 3d20 5b0a 2020 2020 2020 2020  ict = [.        
+0000afe0: 2020 2020 2020 2020 6469 6374 2869 643d          dict(id=
+0000aff0: 656c 652e 7370 6c69 7428 222c 2229 5b30  ele.split(",")[0
+0000b000: 5d2c 2074 7970 653d 7479 7065 5f6d 6170  ], type=type_map
+0000b010: 7069 6e67 5b65 6c65 2e73 706c 6974 2822  ping[ele.split("
+0000b020: 2c22 295b 315d 5d29 0a20 2020 2020 2020  ,")[1]]).       
+0000b030: 2020 2020 2020 2020 2066 6f72 2069 6478           for idx
+0000b040: 2c20 656c 6520 696e 2065 6e75 6d65 7261  , ele in enumera
+0000b050: 7465 2870 6969 5f73 7461 7473 2e73 706c  te(pii_stats.spl
+0000b060: 6974 6c69 6e65 7328 295b 313a 5d2c 2031  itlines()[1:], 1
+0000b070: 290a 2020 2020 2020 2020 2020 2020 5d0a  ).            ].
+0000b080: 0a20 2020 2020 2020 2020 2020 2070 6969  .            pii
+0000b090: 5f72 6573 6f75 7263 6520 3d20 7b0a 2020  _resource = {.  
+0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+0000b0b0: 6163 6b61 6765 5f69 6422 3a20 7265 736f  ackage_id": reso
+0000b0c0: 7572 6365 5b22 7061 636b 6167 655f 6964  urce["package_id
+0000b0d0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
+0000b0e0: 2020 2020 226e 616d 6522 3a20 7265 736f      "name": reso
+0000b0f0: 7572 6365 5b22 6e61 6d65 225d 202b 2022  urce["name"] + "
+0000b100: 202d 2050 4949 222c 0a20 2020 2020 2020   - PII",.       
+0000b110: 2020 2020 2020 2020 2022 666f 726d 6174           "format
+0000b120: 223a 2022 4353 5622 2c0a 2020 2020 2020  ": "CSV",.      
+0000b130: 2020 2020 2020 2020 2020 226d 696d 6574            "mimet
+0000b140: 7970 6522 3a20 2274 6578 742f 6373 7622  ype": "text/csv"
+0000b150: 2c0a 2020 2020 2020 2020 2020 2020 7d0a  ,.            }.
+0000b160: 2020 2020 2020 2020 2020 2020 7069 695f              pii_
+0000b170: 7265 7370 6f6e 7365 203d 2073 656e 645f  response = send_
+0000b180: 7265 736f 7572 6365 5f74 6f5f 6461 7461  resource_to_data
+0000b190: 7374 6f72 6528 0a20 2020 2020 2020 2020  store(.         
+0000b1a0: 2020 2020 2020 2070 6969 5f72 6573 6f75         pii_resou
+0000b1b0: 7263 652c 0a20 2020 2020 2020 2020 2020  rce,.           
+0000b1c0: 2020 2020 2072 6573 6f75 7263 655f 6964       resource_id
+0000b1d0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
+0000b1e0: 2020 2020 2020 2068 6561 6465 7273 3d70         headers=p
+0000b1f0: 6969 5f73 7461 7473 5f64 6963 742c 0a20  ii_stats_dict,. 
+0000b200: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000b210: 7069 5f6b 6579 3d61 7069 5f6b 6579 2c0a  pi_key=api_key,.
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b230: 636b 616e 5f75 726c 3d63 6b61 6e5f 7572  ckan_url=ckan_ur
+0000b240: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+0000b250: 2020 2072 6563 6f72 6473 3d4e 6f6e 652c     records=None,
+0000b260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b270: 2061 6c69 6173 6573 3d70 6969 5f61 6c69   aliases=pii_ali
+0000b280: 6173 2c0a 2020 2020 2020 2020 2020 2020  as,.            
+0000b290: 2020 2020 6361 6c63 756c 6174 655f 7265      calculate_re
+0000b2a0: 636f 7264 5f63 6f75 6e74 3d46 616c 7365  cord_count=False
+0000b2b0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+0000b2c0: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
+0000b2d0: 5f70 6969 5f72 6573 6f75 7263 655f 6964  _pii_resource_id
+0000b2e0: 203d 2070 6969 5f72 6573 706f 6e73 655b   = pii_response[
+0000b2f0: 2272 6573 756c 7422 5d5b 2272 6573 6f75  "result"]["resou
+0000b300: 7263 655f 6964 225d 0a0a 2020 2020 2020  rce_id"]..      
+0000b310: 2020 2020 2020 2320 6e6f 7720 434f 5059        # now COPY
+0000b320: 2074 6865 2050 4949 2070 7265 7669 6577   the PII preview
+0000b330: 2074 6f20 7468 6520 6461 7461 7374 6f72   to the datastor
+0000b340: 650a 2020 2020 2020 2020 2020 2020 6c6f  e.            lo
+0000b350: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
+0000b360: 2020 2020 2020 2020 2020 2027 4144 4449             'ADDI
+0000b370: 4e47 2050 4949 2050 5245 5649 4557 2069  NG PII PREVIEW i
+0000b380: 6e20 227b 7d22 2077 6974 6820 616c 6961  n "{}" with alia
+0000b390: 7320 227b 7d22 2e2e 2e27 2e66 6f72 6d61  s "{}"...'.forma
+0000b3a0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000b3b0: 2020 2020 2020 206e 6577 5f70 6969 5f72         new_pii_r
+0000b3c0: 6573 6f75 7263 655f 6964 2c0a 2020 2020  esource_id,.    
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3e0: 7069 695f 616c 6961 732c 0a20 2020 2020  pii_alias,.     
+0000b3f0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000b400: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000b410: 2020 2020 2020 2063 6f6c 5f6e 616d 6573         col_names
+0000b420: 5f6c 6973 7420 3d20 5b68 5b22 6964 225d  _list = [h["id"]
+0000b430: 2066 6f72 2068 2069 6e20 7069 695f 7374   for h in pii_st
+0000b440: 6174 735f 6469 6374 5d0a 2020 2020 2020  ats_dict].      
+0000b450: 2020 2020 2020 636f 6c75 6d6e 5f6e 616d        column_nam
+0000b460: 6573 203d 2073 716c 2e53 514c 2822 2c22  es = sql.SQL(","
+0000b470: 292e 6a6f 696e 2873 716c 2e49 6465 6e74  ).join(sql.Ident
+0000b480: 6966 6965 7228 6329 2066 6f72 2063 2069  ifier(c) for c i
+0000b490: 6e20 636f 6c5f 6e61 6d65 735f 6c69 7374  n col_names_list
+0000b4a0: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
+0000b4b0: 6f70 795f 7371 6c20 3d20 7371 6c2e 5351  opy_sql = sql.SQ
+0000b4c0: 4c28 0a20 2020 2020 2020 2020 2020 2020  L(.             
+0000b4d0: 2020 2022 434f 5059 207b 7d20 287b 7d29     "COPY {} ({})
+0000b4e0: 2046 524f 4d20 5354 4449 4e20 220a 2020   FROM STDIN ".  
+0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2257                "W
+0000b500: 4954 4820 2846 4f52 4d41 5420 4353 562c  ITH (FORMAT CSV,
+0000b510: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+0000b520: 2020 2022 4845 4144 4552 2031 2c20 454e     "HEADER 1, EN
+0000b530: 434f 4449 4e47 2027 5554 4638 2729 3b22  CODING 'UTF8');"
+0000b540: 0a20 2020 2020 2020 2020 2020 2029 2e66  .            ).f
+0000b550: 6f72 6d61 7428 0a20 2020 2020 2020 2020  ormat(.         
+0000b560: 2020 2020 2020 2073 716c 2e49 6465 6e74         sql.Ident
+0000b570: 6966 6965 7228 6e65 775f 7069 695f 7265  ifier(new_pii_re
+0000b580: 736f 7572 6365 5f69 6429 2c0a 2020 2020  source_id),.    
+0000b590: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
+0000b5a0: 6d6e 5f6e 616d 6573 2c0a 2020 2020 2020  mn_names,.      
+0000b5b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+0000b5c0: 2020 2020 2077 6974 6820 6f70 656e 2871       with open(q
+0000b5d0: 7376 5f73 6561 7263 6873 6574 5f63 7376  sv_searchset_csv
+0000b5e0: 2e6e 616d 652c 2022 7262 2229 2061 7320  .name, "rb") as 
+0000b5f0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
+0000b600: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000b610: 2020 2020 2020 2020 2020 2020 6375 725f              cur_
+0000b620: 7069 692e 636f 7079 5f65 7870 6572 7428  pii.copy_expert(
+0000b630: 636f 7079 5f73 716c 2c20 6629 0a20 2020  copy_sql, f).   
+0000b640: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+0000b650: 6570 7420 7073 7963 6f70 6732 2e45 7272  ept psycopg2.Err
+0000b660: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
+0000b670: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000b680: 7365 2075 7469 6c2e 4a6f 6245 7272 6f72  se util.JobError
+0000b690: 2822 506f 7374 6772 6573 2043 4f50 5920  ("Postgres COPY 
+0000b6a0: 6661 696c 6564 3a20 7b7d 222e 666f 726d  failed: {}".form
+0000b6b0: 6174 2865 2929 0a20 2020 2020 2020 2020  at(e)).         
+0000b6c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6e0: 2070 6969 5f63 6f70 6965 645f 636f 756e   pii_copied_coun
+0000b6f0: 7420 3d20 6375 725f 7069 692e 726f 7763  t = cur_pii.rowc
+0000b700: 6f75 6e74 0a0a 2020 2020 2020 2020 2020  ount..          
+0000b710: 2020 7261 775f 636f 6e6e 6563 7469 6f6e    raw_connection
+0000b720: 5f70 6969 2e63 6f6d 6d69 7428 290a 2020  _pii.commit().  
+0000b730: 2020 2020 2020 2020 2020 6375 725f 7069            cur_pi
+0000b740: 692e 636c 6f73 6528 290a 0a20 2020 2020  i.close()..     
+0000b750: 2020 2020 2020 2070 6969 5f72 6573 6f75         pii_resou
+0000b760: 7263 655b 2269 6422 5d20 3d20 6e65 775f  rce["id"] = new_
+0000b770: 7069 695f 7265 736f 7572 6365 5f69 640a  pii_resource_id.
+0000b780: 2020 2020 2020 2020 2020 2020 7069 695f              pii_
+0000b790: 7265 736f 7572 6365 5b22 7069 695f 7072  resource["pii_pr
+0000b7a0: 6576 6965 7722 5d20 3d20 5472 7565 0a20  eview"] = True. 
+0000b7b0: 2020 2020 2020 2020 2020 2070 6969 5f72             pii_r
+0000b7c0: 6573 6f75 7263 655b 2270 6969 5f6f 665f  esource["pii_of_
+0000b7d0: 7265 736f 7572 6365 225d 203d 2072 6573  resource"] = res
+0000b7e0: 6f75 7263 655f 6964 0a20 2020 2020 2020  ource_id.       
+0000b7f0: 2020 2020 2070 6969 5f72 6573 6f75 7263       pii_resourc
+0000b800: 655b 2274 6f74 616c 5f72 6563 6f72 645f  e["total_record_
+0000b810: 636f 756e 7422 5d20 3d20 7069 695f 726f  count"] = pii_ro
+0000b820: 7773 5f77 6974 685f 6d61 7463 6865 730a  ws_with_matches.
+0000b830: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+0000b840: 7465 5f72 6573 6f75 7263 6528 7069 695f  te_resource(pii_
+0000b850: 7265 736f 7572 6365 2c20 636b 616e 5f75  resource, ckan_u
+0000b860: 726c 2c20 6170 695f 6b65 7929 0a0a 2020  rl, api_key)..  
+0000b870: 2020 2020 2020 2020 2020 7069 695f 6d73            pii_ms
+0000b880: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
+0000b890: 2020 2020 2020 227b 7d20 5049 4920 6361        "{} PII ca
+0000b8a0: 6e64 6964 6174 652f 7320 696e 207b 7d20  ndidate/s in {} 
+0000b8b0: 726f 772f 7320 6172 6520 6176 6169 6c61  row/s are availa
+0000b8c0: 626c 6520 6174 207b 7d20 666f 7220 7265  ble at {} for re
+0000b8d0: 7669 6577 222e 666f 726d 6174 280a 2020  view".format(.  
+0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8f0: 2020 7069 695f 746f 7461 6c5f 6d61 7463    pii_total_matc
+0000b900: 6865 732c 0a20 2020 2020 2020 2020 2020  hes,.           
+0000b910: 2020 2020 2020 2020 2070 6969 5f63 6f70           pii_cop
+0000b920: 6965 645f 636f 756e 742c 0a20 2020 2020  ied_count,.     
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000b940: 6573 6f75 7263 655b 2275 726c 225d 5b3a  esource["url"][:
+0000b950: 2072 6573 6f75 7263 655b 2275 726c 225d   resource["url"]
+0000b960: 2e66 696e 6428 222f 7265 736f 7572 6365  .find("/resource
+0000b970: 2f22 295d 0a20 2020 2020 2020 2020 2020  /")].           
+0000b980: 2020 2020 2020 2020 202b 2022 2f72 6573           + "/res
+0000b990: 6f75 7263 652f 220a 2020 2020 2020 2020  ource/".        
+0000b9a0: 2020 2020 2020 2020 2020 2020 2b20 6e65              + ne
+0000b9b0: 775f 7069 695f 7265 736f 7572 6365 5f69  w_pii_resource_i
+0000b9c0: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+0000b9d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000b9e0: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
+0000b9f0: 6620 7069 695f 666f 756e 645f 6162 6f72  f pii_found_abor
+0000ba00: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000ba10: 2020 2072 6169 7365 2075 7469 6c2e 4a6f     raise util.Jo
+0000ba20: 6245 7272 6f72 2870 6969 5f6d 7367 290a  bError(pii_msg).
+0000ba30: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000ba40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ba50: 2020 6c6f 6767 6572 2e77 6172 6e69 6e67    logger.warning
+0000ba60: 2870 6969 5f6d 7367 290a 2020 2020 2020  (pii_msg).      
+0000ba70: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000ba80: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 2250                "P
+0000baa0: 4949 2043 414e 4449 4441 5445 2f53 2046  II CANDIDATE/S F
+0000bab0: 4f55 4e44 2062 7574 2070 726f 6365 6564  OUND but proceed
+0000bac0: 696e 6720 7769 7468 206a 6f62 2070 6572  ing with job per
+0000bad0: 2044 6174 6170 7573 6865 722b 2063 6f6e   Datapusher+ con
+0000bae0: 6669 6775 7261 7469 6f6e 2e22 0a20 2020  figuration.".   
+0000baf0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+0000bb00: 2020 2020 2020 2065 6c69 6620 6e6f 7420         elif not 
+0000bb10: 7069 695f 666f 756e 643a 0a20 2020 2020  pii_found:.     
+0000bb20: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000bb30: 666f 2822 5049 4920 5363 616e 2063 6f6d  fo("PII Scan com
+0000bb40: 706c 6574 652e 204e 6f20 5049 4920 6361  plete. No PII ca
+0000bb50: 6e64 6964 6174 652f 7320 666f 756e 642e  ndidate/s found.
+0000bb60: 2229 0a0a 2020 2020 2020 2020 7069 6973  ")..        piis
+0000bb70: 6372 6565 6e69 6e67 5f65 6c61 7073 6564  creening_elapsed
+0000bb80: 203d 2074 696d 652e 7065 7266 5f63 6f75   = time.perf_cou
+0000bb90: 6e74 6572 2829 202d 2070 6969 7363 7265  nter() - piiscre
+0000bba0: 656e 696e 675f 7374 6172 740a 0a20 2020  ening_start..   
+0000bbb0: 2023 2064 656c 6574 6520 7468 6520 7173   # delete the qs
+0000bbc0: 7620 696e 6465 7820 6669 6c65 206d 616e  v index file man
+0000bbd0: 7561 6c6c 790a 2020 2020 2320 6173 2069  ually.    # as i
+0000bbe0: 7420 7761 7320 6372 6561 7465 6420 6279  t was created by
+0000bbf0: 2071 7376 2069 6e64 6578 2c20 616e 6420   qsv index, and 
+0000bc00: 6e6f 7420 6279 2074 656d 7066 696c 650a  not by tempfile.
+0000bc10: 2020 2020 6f73 2e72 656d 6f76 6528 7173      os.remove(qs
+0000bc20: 765f 696e 6465 785f 6669 6c65 290a 0a20  v_index_file).. 
+0000bc30: 2020 2023 2061 7420 7468 6973 2073 7461     # at this sta
+0000bc40: 6765 2c20 7468 6520 7265 736f 7572 6365  ge, the resource
+0000bc50: 2069 7320 7265 6164 7920 666f 7220 434f   is ready for CO
+0000bc60: 5059 696e 6720 746f 2074 6865 2044 6174  PYing to the Dat
+0000bc70: 6173 746f 7265 0a0a 2020 2020 6966 2064  astore..    if d
+0000bc80: 7279 5f72 756e 3a0a 2020 2020 2020 2020  ry_run:.        
+0000bc90: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
+0000bca0: 4472 7920 7275 6e20 6f6e 6c79 2e20 5265  Dry run only. Re
+0000bcb0: 7475 726e 696e 6720 7769 7468 6f75 7420  turning without 
+0000bcc0: 636f 7079 696e 6720 746f 2074 6865 2044  copying to the D
+0000bcd0: 6174 6173 746f 7265 2e2e 2e22 290a 2020  atastore...").  
+0000bce0: 2020 2020 2020 7265 7475 726e 2068 6561        return hea
+0000bcf0: 6465 7273 5f64 6963 7473 0a0a 2020 2020  ders_dicts..    
+0000bd00: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
+0000bd10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000bd20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000bd30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
+0000bd40: 2020 2023 2043 4f50 5920 746f 2044 6174     # COPY to Dat
+0000bd50: 6173 746f 7265 0a20 2020 2023 203d 3d3d  astore.    # ===
+0000bd60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000bd70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000bd80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000bd90: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 636f  =========.    co
+0000bda0: 7079 5f73 7461 7274 203d 2074 696d 652e  py_start = time.
+0000bdb0: 7065 7266 5f63 6f75 6e74 6572 2829 0a0a  perf_counter()..
+0000bdc0: 2020 2020 6966 2070 7265 7669 6577 5f72      if preview_r
+0000bdd0: 6f77 733a 0a20 2020 2020 2020 206c 6f67  ows:.        log
+0000bde0: 6765 722e 696e 666f 2822 434f 5059 494e  ger.info("COPYIN
+0000bdf0: 4720 7b3a 2c7d 2d72 6f77 2070 7265 7669  G {:,}-row previ
+0000be00: 6577 2074 6f20 4461 7461 7374 6f72 652e  ew to Datastore.
+0000be10: 2e2e 222e 666f 726d 6174 2872 6f77 735f  ..".format(rows_
+0000be20: 746f 5f63 6f70 7929 290a 2020 2020 656c  to_copy)).    el
+0000be30: 7365 3a0a 2020 2020 2020 2020 6c6f 6767  se:.        logg
+0000be40: 6572 2e69 6e66 6f28 2243 4f50 5949 4e47  er.info("COPYING
+0000be50: 207b 3a2c 7d20 726f 7773 2074 6f20 4461   {:,} rows to Da
+0000be60: 7461 7374 6f72 652e 2e2e 222e 666f 726d  tastore...".form
+0000be70: 6174 2872 6f77 735f 746f 5f63 6f70 7929  at(rows_to_copy)
+0000be80: 290a 0a20 2020 2023 2066 6972 7374 2c20  )..    # first, 
+0000be90: 6c65 7427 7320 6372 6561 7465 2061 6e20  let's create an 
+0000bea0: 656d 7074 7920 6461 7461 7374 6f72 6520  empty datastore 
+0000beb0: 7461 626c 6520 772f 2067 7565 7373 6564  table w/ guessed
+0000bec0: 2074 7970 6573 0a20 2020 2073 656e 645f   types.    send_
+0000bed0: 7265 736f 7572 6365 5f74 6f5f 6461 7461  resource_to_data
+0000bee0: 7374 6f72 6528 0a20 2020 2020 2020 2072  store(.        r
+0000bef0: 6573 6f75 7263 653d 4e6f 6e65 2c0a 2020  esource=None,.  
+0000bf00: 2020 2020 2020 7265 736f 7572 6365 5f69        resource_i
+0000bf10: 643d 7265 736f 7572 6365 5b22 6964 225d  d=resource["id"]
+0000bf20: 2c0a 2020 2020 2020 2020 6865 6164 6572  ,.        header
+0000bf30: 733d 6865 6164 6572 735f 6469 6374 732c  s=headers_dicts,
+0000bf40: 0a20 2020 2020 2020 2061 7069 5f6b 6579  .        api_key
+0000bf50: 3d61 7069 5f6b 6579 2c0a 2020 2020 2020  =api_key,.      
+0000bf60: 2020 636b 616e 5f75 726c 3d63 6b61 6e5f    ckan_url=ckan_
+0000bf70: 7572 6c2c 0a20 2020 2020 2020 2072 6563  url,.        rec
+0000bf80: 6f72 6473 3d4e 6f6e 652c 0a20 2020 2020  ords=None,.     
+0000bf90: 2020 2061 6c69 6173 6573 3d4e 6f6e 652c     aliases=None,
+0000bfa0: 0a20 2020 2020 2020 2063 616c 6375 6c61  .        calcula
+0000bfb0: 7465 5f72 6563 6f72 645f 636f 756e 743d  te_record_count=
+0000bfc0: 4661 6c73 652c 0a20 2020 2029 0a0a 2020  False,.    )..  
+0000bfd0: 2020 636f 7069 6564 5f63 6f75 6e74 203d    copied_count =
+0000bfe0: 2030 0a20 2020 2074 7279 3a0a 2020 2020   0.    try:.    
+0000bff0: 2020 2020 7261 775f 636f 6e6e 6563 7469      raw_connecti
+0000c000: 6f6e 203d 2070 7379 636f 7067 322e 636f  on = psycopg2.co
+0000c010: 6e6e 6563 7428 636f 6e66 6967 2e67 6574  nnect(config.get
+0000c020: 2822 5752 4954 455f 454e 4749 4e45 5f55  ("WRITE_ENGINE_U
+0000c030: 524c 2229 290a 2020 2020 6578 6365 7074  RL")).    except
+0000c040: 2070 7379 636f 7067 322e 4572 726f 7220   psycopg2.Error 
+0000c050: 6173 2065 3a0a 2020 2020 2020 2020 7261  as e:.        ra
+0000c060: 6973 6520 7574 696c 2e4a 6f62 4572 726f  ise util.JobErro
+0000c070: 7228 2243 6f75 6c64 206e 6f74 2063 6f6e  r("Could not con
+0000c080: 6e65 6374 2074 6f20 7468 6520 4461 7461  nect to the Data
+0000c090: 7374 6f72 653a 207b 7d22 2e66 6f72 6d61  store: {}".forma
+0000c0a0: 7428 6529 290a 2020 2020 656c 7365 3a0a  t(e)).    else:.
+0000c0b0: 2020 2020 2020 2020 6375 7220 3d20 7261          cur = ra
+0000c0c0: 775f 636f 6e6e 6563 7469 6f6e 2e63 7572  w_connection.cur
+0000c0d0: 736f 7228 290a 2020 2020 2020 2020 2222  sor().        ""
+0000c0e0: 220a 2020 2020 2020 2020 7472 756e 6361  ".        trunca
+0000c0f0: 7465 2074 6162 6c65 2074 6f20 7573 6520  te table to use 
+0000c100: 636f 7079 2066 7265 657a 6520 6f70 7469  copy freeze opti
+0000c110: 6f6e 2061 6e64 2066 7572 7468 6572 2069  on and further i
+0000c120: 6e63 7265 6173 650a 2020 2020 2020 2020  ncrease.        
+0000c130: 7065 7266 6f72 6d61 6e63 6520 6173 2074  performance as t
+0000c140: 6865 7265 2069 7320 6e6f 206e 6565 6420  here is no need 
+0000c150: 666f 7220 5741 4c20 6c6f 6773 2074 6f20  for WAL logs to 
+0000c160: 6265 206d 6169 6e74 6169 6e65 640a 2020  be maintained.  
+0000c170: 2020 2020 2020 6874 7470 733a 2f2f 7777        https://ww
+0000c180: 772e 706f 7374 6772 6573 716c 2e6f 7267  w.postgresql.org
+0000c190: 2f64 6f63 732f 6375 7272 656e 742f 706f  /docs/current/po
+0000c1a0: 7075 6c61 7465 2e68 746d 6c23 504f 5055  pulate.html#POPU
+0000c1b0: 4c41 5445 2d43 4f50 592d 4652 4f4d 0a20  LATE-COPY-FROM. 
+0000c1c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c1d0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0000c1e0: 2020 2020 6375 722e 6578 6563 7574 6528      cur.execute(
+0000c1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c200: 2073 716c 2e53 514c 2822 5452 554e 4341   sql.SQL("TRUNCA
+0000c210: 5445 2054 4142 4c45 207b 7d22 292e 666f  TE TABLE {}").fo
+0000c220: 726d 6174 2873 716c 2e49 6465 6e74 6966  rmat(sql.Identif
+0000c230: 6965 7228 7265 736f 7572 6365 5f69 6429  ier(resource_id)
+0000c240: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+0000c250: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+0000c260: 7073 7963 6f70 6732 2e45 7272 6f72 2061  psycopg2.Error a
+0000c270: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+0000c280: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+0000c290: 2243 6f75 6c64 206e 6f74 2054 5255 4e43  "Could not TRUNC
+0000c2a0: 4154 453a 207b 7d22 2e66 6f72 6d61 7428  ATE: {}".format(
+0000c2b0: 6529 290a 0a20 2020 2020 2020 2063 6f6c  e))..        col
+0000c2c0: 5f6e 616d 6573 5f6c 6973 7420 3d20 5b68  _names_list = [h
+0000c2d0: 5b22 6964 225d 2066 6f72 2068 2069 6e20  ["id"] for h in 
+0000c2e0: 6865 6164 6572 735f 6469 6374 735d 0a20  headers_dicts]. 
+0000c2f0: 2020 2020 2020 2063 6f6c 756d 6e5f 6e61         column_na
+0000c300: 6d65 7320 3d20 7371 6c2e 5351 4c28 222c  mes = sql.SQL(",
+0000c310: 2229 2e6a 6f69 6e28 7371 6c2e 4964 656e  ").join(sql.Iden
+0000c320: 7469 6669 6572 2863 2920 666f 7220 6320  tifier(c) for c 
+0000c330: 696e 2063 6f6c 5f6e 616d 6573 5f6c 6973  in col_names_lis
+0000c340: 7429 0a20 2020 2020 2020 2063 6f70 795f  t).        copy_
+0000c350: 7371 6c20 3d20 7371 6c2e 5351 4c28 0a20  sql = sql.SQL(. 
+0000c360: 2020 2020 2020 2020 2020 2022 434f 5059             "COPY
+0000c370: 207b 7d20 287b 7d29 2046 524f 4d20 5354   {} ({}) FROM ST
+0000c380: 4449 4e20 220a 2020 2020 2020 2020 2020  DIN ".          
+0000c390: 2020 2257 4954 4820 2846 4f52 4d41 5420    "WITH (FORMAT 
+0000c3a0: 4353 562c 2046 5245 455a 4520 312c 2022  CSV, FREEZE 1, "
+0000c3b0: 0a20 2020 2020 2020 2020 2020 2022 4845  .            "HE
+0000c3c0: 4144 4552 2031 2c20 454e 434f 4449 4e47  ADER 1, ENCODING
+0000c3d0: 2027 5554 4638 2729 3b22 0a20 2020 2020   'UTF8');".     
+0000c3e0: 2020 2029 2e66 6f72 6d61 7428 0a20 2020     ).format(.   
+0000c3f0: 2020 2020 2020 2020 2073 716c 2e49 6465           sql.Ide
+0000c400: 6e74 6966 6965 7228 7265 736f 7572 6365  ntifier(resource
+0000c410: 5f69 6429 2c0a 2020 2020 2020 2020 2020  _id),.          
+0000c420: 2020 636f 6c75 6d6e 5f6e 616d 6573 2c0a    column_names,.
+0000c430: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000c440: 2020 7769 7468 206f 7065 6e28 746d 702e    with open(tmp.
+0000c450: 6e61 6d65 2c20 2272 6222 2920 6173 2066  name, "rb") as f
+0000c460: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
+0000c470: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+0000c480: 2020 2063 7572 2e63 6f70 795f 6578 7065     cur.copy_expe
+0000c490: 7274 2863 6f70 795f 7371 6c2c 2066 290a  rt(copy_sql, f).
+0000c4a0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+0000c4b0: 7074 2070 7379 636f 7067 322e 4572 726f  pt psycopg2.Erro
+0000c4c0: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
+0000c4d0: 2020 2020 2020 2020 7261 6973 6520 7574          raise ut
+0000c4e0: 696c 2e4a 6f62 4572 726f 7228 2250 6f73  il.JobError("Pos
+0000c4f0: 7467 7265 7320 434f 5059 2066 6169 6c65  tgres COPY faile
+0000c500: 643a 207b 7d22 2e66 6f72 6d61 7428 6529  d: {}".format(e)
+0000c510: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+0000c520: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000c530: 2020 2020 636f 7069 6564 5f63 6f75 6e74      copied_count
+0000c540: 203d 2063 7572 2e72 6f77 636f 756e 740a   = cur.rowcount.
+0000c550: 0a20 2020 2020 2020 2072 6177 5f63 6f6e  .        raw_con
+0000c560: 6e65 6374 696f 6e2e 636f 6d6d 6974 2829  nection.commit()
+0000c570: 0a20 2020 2020 2020 2023 2074 6869 7320  .        # this 
+0000c580: 6973 206e 6565 6465 6420 746f 2069 7373  is needed to iss
+0000c590: 7565 2061 2056 4143 5555 4d20 414e 414c  ue a VACUUM ANAL
+0000c5a0: 595a 450a 2020 2020 2020 2020 7261 775f  YZE.        raw_
+0000c5b0: 636f 6e6e 6563 7469 6f6e 2e73 6574 5f69  connection.set_i
+0000c5c0: 736f 6c61 7469 6f6e 5f6c 6576 656c 280a  solation_level(.
+0000c5d0: 2020 2020 2020 2020 2020 2020 7073 7963              psyc
+0000c5e0: 6f70 6732 2e65 7874 656e 7369 6f6e 732e  opg2.extensions.
+0000c5f0: 4953 4f4c 4154 494f 4e5f 4c45 5645 4c5f  ISOLATION_LEVEL_
+0000c600: 4155 544f 434f 4d4d 4954 0a20 2020 2020  AUTOCOMMIT.     
+0000c610: 2020 2029 0a20 2020 2020 2020 2061 6e61     ).        ana
+0000c620: 6c79 7a65 5f63 7572 203d 2072 6177 5f63  lyze_cur = raw_c
+0000c630: 6f6e 6e65 6374 696f 6e2e 6375 7273 6f72  onnection.cursor
+0000c640: 2829 0a20 2020 2020 2020 2061 6e61 6c79  ().        analy
+0000c650: 7a65 5f63 7572 2e65 7865 6375 7465 280a  ze_cur.execute(.
+0000c660: 2020 2020 2020 2020 2020 2020 7371 6c2e              sql.
+0000c670: 5351 4c28 2256 4143 5555 4d20 414e 414c  SQL("VACUUM ANAL
+0000c680: 595a 4520 7b7d 2229 2e66 6f72 6d61 7428  YZE {}").format(
+0000c690: 7371 6c2e 4964 656e 7469 6669 6572 2872  sql.Identifier(r
+0000c6a0: 6573 6f75 7263 655f 6964 2929 0a20 2020  esource_id)).   
+0000c6b0: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
+0000c6c0: 6e61 6c79 7a65 5f63 7572 2e63 6c6f 7365  nalyze_cur.close
+0000c6d0: 2829 0a0a 2020 2020 636f 7079 5f65 6c61  ()..    copy_ela
+0000c6e0: 7073 6564 203d 2074 696d 652e 7065 7266  psed = time.perf
+0000c6f0: 5f63 6f75 6e74 6572 2829 202d 2063 6f70  _counter() - cop
+0000c700: 795f 7374 6172 740a 2020 2020 6c6f 6767  y_start.    logg
+0000c710: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+0000c720: 2027 2e2e 2e63 6f70 7969 6e67 2064 6f6e   '...copying don
+0000c730: 652e 2043 6f70 6965 6420 7b6e 7d20 726f  e. Copied {n} ro
+0000c740: 7773 2074 6f20 227b 7265 735f 6964 7d22  ws to "{res_id}"
+0000c750: 2069 6e20 7b63 6f70 795f 656c 6170 7365   in {copy_elapse
+0000c760: 647d 2073 6563 6f6e 6473 2e27 2e66 6f72  d} seconds.'.for
+0000c770: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+0000c780: 206e 3d22 7b3a 2c7d 222e 666f 726d 6174   n="{:,}".format
+0000c790: 2863 6f70 6965 645f 636f 756e 7429 2c0a  (copied_count),.
+0000c7a0: 2020 2020 2020 2020 2020 2020 7265 735f              res_
+0000c7b0: 6964 3d72 6573 6f75 7263 655f 6964 2c0a  id=resource_id,.
+0000c7c0: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+0000c7d0: 5f65 6c61 7073 6564 3d22 7b3a 2c2e 3266  _elapsed="{:,.2f
+0000c7e0: 7d22 2e66 6f72 6d61 7428 636f 7079 5f65  }".format(copy_e
+0000c7f0: 6c61 7073 6564 292c 0a20 2020 2020 2020  lapsed),.       
+0000c800: 2029 0a20 2020 2029 0a0a 2020 2020 2320   ).    )..    # 
+0000c810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c820: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c830: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
+0000c850: 2023 2055 5044 4154 4520 4d45 5441 4441   # UPDATE METADA
+0000c860: 5441 0a20 2020 2023 203d 3d3d 3d3d 3d3d  TA.    # =======
+0000c870: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c880: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000c8a0: 3d3d 3d3d 3d0a 2020 2020 6d65 7461 6461  =====.    metada
+0000c8b0: 7461 5f73 7461 7274 203d 2074 696d 652e  ta_start = time.
+0000c8c0: 7065 7266 5f63 6f75 6e74 6572 2829 0a20  perf_counter(). 
+0000c8d0: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
+0000c8e0: 5550 4441 5449 4e47 2052 4553 4f55 5243  UPDATING RESOURC
+0000c8f0: 4520 4d45 5441 4441 5441 2e2e 2e22 290a  E METADATA...").
+0000c900: 0a20 2020 2023 202d 2d2d 2d2d 2d2d 2d2d  .    # ---------
+0000c910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2041 5554  ------------ AUT
+0000c920: 4f2d 414c 4941 5349 4e47 202d 2d2d 2d2d  O-ALIASING -----
+0000c930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c940: 2d2d 2d0a 2020 2020 2320 616c 6961 7365  ---.    # aliase
+0000c950: 7320 6172 6520 6875 6d61 6e2d 7265 6164  s are human-read
+0000c960: 6162 6c65 2c20 616e 6420 6d61 6b65 2069  able, and make i
+0000c970: 7420 6561 7369 6572 2074 6f20 7573 6520  t easier to use 
+0000c980: 7468 616e 2072 6573 6f75 7263 6520 6964  than resource id
+0000c990: 2068 6173 680a 2020 2020 2320 7768 656e   hash.    # when
+0000c9a0: 2075 7369 6e67 2074 6865 2044 6174 6173   using the Datas
+0000c9b0: 746f 7265 2041 5049 2061 6e64 2069 6e20  tore API and in 
+0000c9c0: 5351 4c20 7175 6572 6965 730a 2020 2020  SQL queries.    
+0000c9d0: 6175 746f 5f61 6c69 6173 203d 2063 6f6e  auto_alias = con
+0000c9e0: 6669 672e 6765 7428 2241 5554 4f5f 414c  fig.get("AUTO_AL
+0000c9f0: 4941 5322 290a 2020 2020 6175 746f 5f61  IAS").    auto_a
+0000ca00: 6c69 6173 5f75 6e69 7175 6520 3d20 636f  lias_unique = co
+0000ca10: 6e66 6967 2e67 6574 2822 4155 544f 5f41  nfig.get("AUTO_A
+0000ca20: 4c49 4153 5f55 4e49 5155 4522 290a 2020  LIAS_UNIQUE").  
+0000ca30: 2020 616c 6961 7320 3d20 4e6f 6e65 0a20    alias = None. 
+0000ca40: 2020 2069 6620 6175 746f 5f61 6c69 6173     if auto_alias
+0000ca50: 3a0a 2020 2020 2020 2020 6c6f 6767 6572  :.        logger
+0000ca60: 2e69 6e66 6f28 0a20 2020 2020 2020 2020  .info(.         
+0000ca70: 2020 2022 4155 544f 2d41 4c49 4153 494e     "AUTO-ALIASIN
+0000ca80: 472e 2041 7574 6f2d 616c 6961 732d 756e  G. Auto-alias-un
+0000ca90: 6971 7565 3a20 7b7d 202e 2e2e 222e 666f  ique: {} ...".fo
+0000caa0: 726d 6174 2861 7574 6f5f 616c 6961 735f  rmat(auto_alias_
+0000cab0: 756e 6971 7565 290a 2020 2020 2020 2020  unique).        
+0000cac0: 290a 2020 2020 2020 2020 2320 6765 7420  ).        # get 
+0000cad0: 7061 636b 6167 6520 696e 666f 2c20 736f  package info, so
+0000cae0: 2077 6520 6361 6e20 636f 6e73 7472 7563   we can construc
+0000caf0: 7420 7468 6520 616c 6961 730a 2020 2020  t the alias.    
+0000cb00: 2020 2020 7061 636b 6167 6520 3d20 6765      package = ge
+0000cb10: 745f 7061 636b 6167 6528 7265 736f 7572  t_package(resour
+0000cb20: 6365 5b22 7061 636b 6167 655f 6964 225d  ce["package_id"]
+0000cb30: 2c20 636b 616e 5f75 726c 2c20 6170 695f  , ckan_url, api_
+0000cb40: 6b65 7929 0a0a 2020 2020 2020 2020 7265  key)..        re
+0000cb50: 736f 7572 6365 5f6e 616d 6520 3d20 7265  source_name = re
+0000cb60: 736f 7572 6365 2e67 6574 2822 6e61 6d65  source.get("name
+0000cb70: 2229 0a20 2020 2020 2020 2070 6163 6b61  ").        packa
+0000cb80: 6765 5f6e 616d 6520 3d20 7061 636b 6167  ge_name = packag
+0000cb90: 652e 6765 7428 226e 616d 6522 290a 2020  e.get("name").  
+0000cba0: 2020 2020 2020 6f77 6e65 725f 6f72 6720        owner_org 
+0000cbb0: 3d20 7061 636b 6167 652e 6765 7428 226f  = package.get("o
+0000cbc0: 7267 616e 697a 6174 696f 6e22 290a 2020  rganization").  
+0000cbd0: 2020 2020 2020 6f77 6e65 725f 6f72 675f        owner_org_
+0000cbe0: 6e61 6d65 203d 2022 220a 2020 2020 2020  name = "".      
+0000cbf0: 2020 6966 206f 776e 6572 5f6f 7267 3a0a    if owner_org:.
+0000cc00: 2020 2020 2020 2020 2020 2020 6f77 6e65              owne
+0000cc10: 725f 6f72 675f 6e61 6d65 203d 206f 776e  r_org_name = own
+0000cc20: 6572 5f6f 7267 2e67 6574 2822 6e61 6d65  er_org.get("name
+0000cc30: 2229 0a20 2020 2020 2020 2069 6620 7265  ").        if re
+0000cc40: 736f 7572 6365 5f6e 616d 6520 616e 6420  source_name and 
+0000cc50: 7061 636b 6167 655f 6e61 6d65 2061 6e64  package_name and
+0000cc60: 206f 776e 6572 5f6f 7267 5f6e 616d 653a   owner_org_name:
+0000cc70: 0a20 2020 2020 2020 2020 2020 2023 2077  .            # w
+0000cc80: 6520 6c69 6d69 7420 6974 2074 6f20 3535  e limit it to 55
+0000cc90: 2c20 736f 2077 6520 7374 696c 6c20 6861  , so we still ha
+0000cca0: 7665 2073 7061 6365 2066 6f72 2073 6571  ve space for seq
+0000ccb0: 7565 6e63 6520 2620 7374 6174 7320 7375  uence & stats su
+0000ccc0: 6666 6978 0a20 2020 2020 2020 2020 2020  ffix.           
+0000ccd0: 2023 2070 6f73 7467 7265 7320 6d61 7820   # postgres max 
+0000cce0: 6964 656e 7469 6669 6572 206c 656e 6774  identifier lengt
+0000ccf0: 6820 6973 2036 330a 2020 2020 2020 2020  h is 63.        
+0000cd00: 2020 2020 616c 6961 7320 3d20 6622 7b72      alias = f"{r
+0000cd10: 6573 6f75 7263 655f 6e61 6d65 7d2d 7b70  esource_name}-{p
+0000cd20: 6163 6b61 6765 5f6e 616d 657d 2d7b 6f77  ackage_name}-{ow
+0000cd30: 6e65 725f 6f72 675f 6e61 6d65 7d22 5b3a  ner_org_name}"[:
+0000cd40: 3535 5d0a 2020 2020 2020 2020 2020 2020  55].            
+0000cd50: 2320 6966 2041 5554 4f5f 414c 4941 535f  # if AUTO_ALIAS_
+0000cd60: 554e 4951 5545 2069 7320 7472 7565 2c20  UNIQUE is true, 
+0000cd70: 6368 6563 6b20 6966 2074 6865 2061 6c69  check if the ali
+0000cd80: 6173 2061 6c72 6561 6479 2065 7869 7374  as already exist
+0000cd90: 2c20 6966 2069 7420 646f 6573 0a20 2020  , if it does.   
+0000cda0: 2020 2020 2020 2020 2023 2061 6464 2061           # add a
+0000cdb0: 2073 6571 7565 6e63 6520 7375 6666 6978   sequence suffix
+0000cdc0: 2073 6f20 7468 6520 6e65 7720 616c 6961   so the new alia
+0000cdd0: 7320 6361 6e20 6265 2063 7265 6174 6564  s can be created
+0000cde0: 0a20 2020 2020 2020 2020 2020 2063 7572  .            cur
+0000cdf0: 2e65 7865 6375 7465 280a 2020 2020 2020  .execute(.      
+0000ce00: 2020 2020 2020 2020 2020 2253 454c 4543            "SELEC
+0000ce10: 5420 434f 554e 5428 2a29 2c20 616c 6961  T COUNT(*), alia
+0000ce20: 735f 6f66 2046 524f 4d20 5f74 6162 6c65  s_of FROM _table
+0000ce30: 5f6d 6574 6164 6174 6120 7768 6572 6520  _metadata where 
+0000ce40: 6e61 6d65 206c 696b 6520 2573 2067 726f  name like %s gro
+0000ce50: 7570 2062 7920 616c 6961 735f 6f66 222c  up by alias_of",
+0000ce60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ce70: 2028 616c 6961 7320 2b20 2225 222c 292c   (alias + "%",),
+0000ce80: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000ce90: 2020 2020 2020 2020 2020 2061 6c69 6173             alias
+0000cea0: 5f71 7565 7279 5f72 6573 756c 7420 3d20  _query_result = 
+0000ceb0: 6375 722e 6665 7463 686f 6e65 2829 0a20  cur.fetchone(). 
+0000cec0: 2020 2020 2020 2020 2020 2069 6620 616c             if al
+0000ced0: 6961 735f 7175 6572 795f 7265 7375 6c74  ias_query_result
+0000cee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cef0: 2020 616c 6961 735f 636f 756e 7420 3d20    alias_count = 
+0000cf00: 616c 6961 735f 7175 6572 795f 7265 7375  alias_query_resu
+0000cf10: 6c74 5b30 5d0a 2020 2020 2020 2020 2020  lt[0].          
+0000cf20: 2020 2020 2020 6578 6973 7469 6e67 5f61        existing_a
+0000cf30: 6c69 6173 5f6f 6620 3d20 616c 6961 735f  lias_of = alias_
+0000cf40: 7175 6572 795f 7265 7375 6c74 5b31 5d0a  query_result[1].
+0000cf50: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000cf60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cf70: 2020 616c 6961 735f 636f 756e 7420 3d20    alias_count = 
+0000cf80: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+0000cf90: 2020 6578 6973 7469 6e67 5f61 6c69 6173    existing_alias
+0000cfa0: 5f6f 6620 3d20 2222 0a20 2020 2020 2020  _of = "".       
+0000cfb0: 2020 2020 2069 6620 6175 746f 5f61 6c69       if auto_ali
+0000cfc0: 6173 5f75 6e69 7175 6520 616e 6420 616c  as_unique and al
+0000cfd0: 6961 735f 636f 756e 7420 3e20 313a 0a20  ias_count > 1:. 
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000cff0: 6c69 6173 5f73 6571 7565 6e63 6520 3d20  lias_sequence = 
+0000d000: 616c 6961 735f 636f 756e 7420 2b20 310a  alias_count + 1.
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 7768 696c 6520 5472 7565 3a0a 2020 2020  while True:.    
+0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d040: 2320 7765 2064 6f20 7468 6973 2c20 736f  # we do this, so
+0000d050: 2077 6527 7265 2063 6572 7461 696e 2074   we're certain t
+0000d060: 6865 206e 6577 2061 6c69 6173 2064 6f65  he new alias doe
+0000d070: 7320 6e6f 7420 6578 6973 740a 2020 2020  s not exist.    
+0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d090: 2320 6a75 7374 2069 6e20 6361 7365 2074  # just in case t
+0000d0a0: 6865 7920 6465 6c65 7465 6420 616e 206f  hey deleted an o
+0000d0b0: 6c64 6572 2061 6c69 6173 2077 6974 6820  lder alias with 
+0000d0c0: 6120 6c6f 7765 7220 7365 7175 656e 6365  a lower sequence
+0000d0d0: 2023 0a20 2020 2020 2020 2020 2020 2020   #.             
+0000d0e0: 2020 2020 2020 2061 6c69 6173 203d 2066         alias = f
+0000d0f0: 227b 616c 6961 737d 2d7b 616c 6961 735f  "{alias}-{alias_
+0000d100: 7365 7175 656e 6365 3a30 337d 220a 2020  sequence:03}".  
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2020 6375 722e 6578 6563 7574 6528 0a20    cur.execute(. 
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2020 2020 2020 2022 5345 4c45 4354 2043         "SELECT C
+0000d150: 4f55 4e54 282a 292c 2061 6c69 6173 5f6f  OUNT(*), alias_o
+0000d160: 6620 4652 4f4d 205f 7461 626c 655f 6d65  f FROM _table_me
+0000d170: 7461 6461 7461 2077 6865 7265 206e 616d  tadata where nam
+0000d180: 6520 6c69 6b65 2025 7320 6772 6f75 7020  e like %s group 
+0000d190: 6279 2061 6c69 6173 5f6f 663b 222c 0a20  by alias_of;",. 
+0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1b0: 2020 2020 2020 2028 616c 6961 7320 2b20         (alias + 
+0000d1c0: 2225 222c 292c 0a20 2020 2020 2020 2020  "%",),.         
+0000d1d0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1f0: 2061 6c69 6173 5f65 7869 7374 7320 3d20   alias_exists = 
+0000d200: 6375 722e 6665 7463 686f 6e65 2829 5b30  cur.fetchone()[0
+0000d210: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000d220: 2020 2020 2020 6966 206e 6f74 2061 6c69        if not ali
+0000d230: 6173 5f65 7869 7374 733a 0a20 2020 2020  as_exists:.     
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+0000d260: 2020 2020 2020 2020 2020 2020 2061 6c69               ali
+0000d270: 6173 5f73 6571 7565 6e63 6520 2b3d 2031  as_sequence += 1
+0000d280: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000d290: 6620 616c 6961 735f 636f 756e 7420 3d3d  f alias_count ==
+0000d2a0: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000d2b0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+0000d2c0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0000d2d0: 2020 2020 2020 2020 2744 726f 7070 696e          'Droppin
+0000d2e0: 6720 6578 6973 7469 6e67 2061 6c69 6173  g existing alias
+0000d2f0: 2022 7b7d 2220 666f 7220 7265 736f 7572   "{}" for resour
+0000d300: 6365 2022 7b7d 222e 2e2e 272e 666f 726d  ce "{}"...'.form
+0000d310: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+0000d320: 2020 2020 2020 2020 2020 2020 616c 6961              alia
+0000d330: 732c 2065 7869 7374 696e 675f 616c 6961  s, existing_alia
+0000d340: 735f 6f66 0a20 2020 2020 2020 2020 2020  s_of.           
+0000d350: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000d360: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000d370: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0000d380: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d390: 2020 2020 2020 6375 722e 6578 6563 7574        cur.execut
+0000d3a0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+0000d3b0: 2020 2020 2020 2020 2020 2073 716c 2e53             sql.S
+0000d3c0: 514c 2822 4452 4f50 2056 4945 5720 4946  QL("DROP VIEW IF
+0000d3d0: 2045 5849 5354 5320 7b7d 2229 2e66 6f72   EXISTS {}").for
+0000d3e0: 6d61 7428 7371 6c2e 4964 656e 7469 6669  mat(sql.Identifi
+0000d3f0: 6572 2861 6c69 6173 2929 0a20 2020 2020  er(alias)).     
+0000d400: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000d410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d420: 2065 7863 6570 7420 7073 7963 6f70 6732   except psycopg2
+0000d430: 2e45 7272 6f72 2061 7320 653a 0a20 2020  .Error as e:.   
+0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d450: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+0000d460: 2243 6f75 6c64 206e 6f74 2064 726f 7020  "Could not drop 
+0000d470: 616c 6961 732f 7669 6577 3a20 7b7d 222e  alias/view: {}".
+0000d480: 666f 726d 6174 2865 2929 0a0a 2020 2020  format(e))..    
+0000d490: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000d4a0: 2020 2020 2020 6c6f 6767 6572 2e77 6172        logger.war
+0000d4b0: 6e69 6e67 280a 2020 2020 2020 2020 2020  ning(.          
+0000d4c0: 2020 2020 2020 2243 616e 6e6f 7420 6372        "Cannot cr
+0000d4d0: 6561 7465 2061 6c69 6173 3a20 7b7d 2d7b  eate alias: {}-{
+0000d4e0: 7d2d 7b7d 222e 666f 726d 6174 280a 2020  }-{}".format(.  
+0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d500: 2020 7265 736f 7572 6365 5f6e 616d 652c    resource_name,
+0000d510: 2070 6163 6b61 6765 5f6e 616d 652c 206f   package_name, o
+0000d520: 776e 6572 5f6f 7267 0a20 2020 2020 2020  wner_org.       
+0000d530: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000d540: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d550: 2020 2020 2061 6c69 6173 203d 204e 6f6e       alias = Non
+0000d560: 650a 0a20 2020 2023 202d 2d2d 2d2d 2d2d  e..    # -------
+0000d570: 2d20 7368 6f75 6c64 2077 6520 4144 445f  - should we ADD_
+0000d580: 5355 4d4d 4152 595f 5354 4154 535f 5245  SUMMARY_STATS_RE
+0000d590: 534f 5552 4345 3f20 2d2d 2d2d 2d2d 2d2d  SOURCE? --------
+0000d5a0: 2d2d 2d2d 2d0a 2020 2020 2320 6279 2064  -----.    # by d
+0000d5b0: 6566 6175 6c74 2c20 7765 206f 6e6c 7920  efault, we only 
+0000d5c0: 6164 6420 7375 6d6d 6172 7920 7374 6174  add summary stat
+0000d5d0: 7320 6966 2077 6527 7265 206e 6f74 2064  s if we're not d
+0000d5e0: 6f69 6e67 2061 2070 6172 7469 616c 2064  oing a partial d
+0000d5f0: 6f77 6e6c 6f61 640a 2020 2020 2320 286f  ownload.    # (o
+0000d600: 7468 6572 7769 7365 2c20 796f 7527 7265  therwise, you're
+0000d610: 2073 756d 6d61 7269 7a69 6e67 2074 6865   summarizing the
+0000d620: 2070 7265 7669 6577 2c20 6e6f 7420 7468   preview, not th
+0000d630: 6520 7768 6f6c 6520 6669 6c65 290a 2020  e whole file).  
+0000d640: 2020 2320 5468 6174 2069 732c 2075 6e6c    # That is, unl
+0000d650: 6573 7320 5355 4d4d 4152 595f 5354 4154  ess SUMMARY_STAT
+0000d660: 535f 5749 5448 5f50 5245 5649 4557 2069  S_WITH_PREVIEW i
+0000d670: 7320 7365 7420 746f 2074 7275 650a 2020  s set to true.  
+0000d680: 2020 6966 2028 636f 6e66 6967 2e67 6574    if (config.get
+0000d690: 2822 4144 445f 5355 4d4d 4152 595f 5354  ("ADD_SUMMARY_ST
+0000d6a0: 4154 535f 5245 534f 5552 4345 2229 2061  ATS_RESOURCE") a
+0000d6b0: 6e64 206e 6f74 2064 6f77 6e6c 6f61 645f  nd not download_
+0000d6c0: 7072 6576 6965 775f 6f6e 6c79 2920 6f72  preview_only) or
+0000d6d0: 2028 0a20 2020 2020 2020 2064 6f77 6e6c   (.        downl
+0000d6e0: 6f61 645f 7072 6576 6965 775f 6f6e 6c79  oad_preview_only
+0000d6f0: 2061 6e64 2063 6f6e 6669 672e 6765 7428   and config.get(
+0000d700: 2253 554d 4d41 5259 5f53 5441 5453 5f57  "SUMMARY_STATS_W
+0000d710: 4954 485f 5052 4556 4945 5722 290a 2020  ITH_PREVIEW").  
+0000d720: 2020 293a 0a0a 2020 2020 2020 2020 7374    ):..        st
+0000d730: 6174 735f 7265 736f 7572 6365 5f69 6420  ats_resource_id 
+0000d740: 3d20 7265 736f 7572 6365 5f69 6420 2b20  = resource_id + 
+0000d750: 222d 7374 6174 7322 0a0a 2020 2020 2020  "-stats"..      
+0000d760: 2020 2320 6368 6563 6b20 6966 2074 6865    # check if the
+0000d770: 2073 7461 7473 2061 6c72 6561 6479 2065   stats already e
+0000d780: 7869 7374 0a20 2020 2020 2020 2065 7869  xist.        exi
+0000d790: 7374 696e 675f 7374 6174 7320 3d20 6461  sting_stats = da
+0000d7a0: 7461 7374 6f72 655f 7265 736f 7572 6365  tastore_resource
+0000d7b0: 5f65 7869 7374 7328 7374 6174 735f 7265  _exists(stats_re
+0000d7c0: 736f 7572 6365 5f69 642c 2061 7069 5f6b  source_id, api_k
+0000d7d0: 6579 2c20 636b 616e 5f75 726c 290a 2020  ey, ckan_url).  
+0000d7e0: 2020 2020 2020 2320 4465 6c65 7465 2065        # Delete e
+0000d7f0: 7869 7374 696e 6720 7375 6d6d 6172 792d  xisting summary-
+0000d800: 7374 6174 7320 6265 666f 7265 2070 726f  stats before pro
+0000d810: 6365 6564 696e 672e 0a20 2020 2020 2020  ceeding..       
+0000d820: 2069 6620 6578 6973 7469 6e67 5f73 7461   if existing_sta
+0000d830: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+0000d840: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+0000d850: 2020 2020 2020 2020 2020 2020 2027 4465               'De
+0000d860: 6c65 7469 6e67 2065 7869 7374 696e 6720  leting existing 
+0000d870: 7375 6d6d 6172 7920 7374 6174 7320 227b  summary stats "{
+0000d880: 7d22 2e27 2e66 6f72 6d61 7428 7374 6174  }".'.format(stat
+0000d890: 735f 7265 736f 7572 6365 5f69 6429 0a20  s_resource_id). 
+0000d8a0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000d8b0: 2020 2020 2020 2020 2020 6375 722e 6578            cur.ex
+0000d8c0: 6563 7574 6528 0a20 2020 2020 2020 2020  ecute(.         
+0000d8d0: 2020 2020 2020 2022 5345 4c45 4354 2061         "SELECT a
+0000d8e0: 6c69 6173 5f6f 6620 4652 4f4d 205f 7461  lias_of FROM _ta
+0000d8f0: 626c 655f 6d65 7461 6461 7461 2077 6865  ble_metadata whe
+0000d900: 7265 206e 616d 6520 6c69 6b65 2025 7320  re name like %s 
+0000d910: 6772 6f75 7020 6279 2061 6c69 6173 5f6f  group by alias_o
+0000d920: 663b 222c 0a20 2020 2020 2020 2020 2020  f;",.           
+0000d930: 2020 2020 2028 7374 6174 735f 7265 736f       (stats_reso
+0000d940: 7572 6365 5f69 6420 2b20 2225 222c 292c  urce_id + "%",),
+0000d950: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000d960: 2020 2020 2020 2020 2020 2073 7461 7473             stats
+0000d970: 5f61 6c69 6173 5f72 6573 756c 7420 3d20  _alias_result = 
+0000d980: 6375 722e 6665 7463 686f 6e65 2829 0a20  cur.fetchone(). 
+0000d990: 2020 2020 2020 2020 2020 2069 6620 7374             if st
+0000d9a0: 6174 735f 616c 6961 735f 7265 7375 6c74  ats_alias_result
+0000d9b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d9c0: 2020 6578 6973 7469 6e67 5f73 7461 7473    existing_stats
+0000d9d0: 5f61 6c69 6173 5f6f 6620 3d20 7374 6174  _alias_of = stat
+0000d9e0: 735f 616c 6961 735f 7265 7375 6c74 5b30  s_alias_result[0
+0000d9f0: 5d0a 0a20 2020 2020 2020 2020 2020 2020  ]..             
+0000da00: 2020 2064 656c 6574 655f 6461 7461 7374     delete_datast
+0000da10: 6f72 655f 7265 736f 7572 6365 2865 7869  ore_resource(exi
+0000da20: 7374 696e 675f 7374 6174 735f 616c 6961  sting_stats_alia
+0000da30: 735f 6f66 2c20 6170 695f 6b65 792c 2063  s_of, api_key, c
+0000da40: 6b61 6e5f 7572 6c29 0a20 2020 2020 2020  kan_url).       
+0000da50: 2020 2020 2020 2020 2064 656c 6574 655f           delete_
+0000da60: 7265 736f 7572 6365 2865 7869 7374 696e  resource(existin
+0000da70: 675f 7374 6174 735f 616c 6961 735f 6f66  g_stats_alias_of
+0000da80: 2c20 6170 695f 6b65 792c 2063 6b61 6e5f  , api_key, ckan_
+0000da90: 7572 6c29 0a0a 2020 2020 2020 2020 7374  url)..        st
+0000daa0: 6174 735f 616c 6961 7365 7320 3d20 5b73  ats_aliases = [s
+0000dab0: 7461 7473 5f72 6573 6f75 7263 655f 6964  tats_resource_id
+0000dac0: 5d0a 2020 2020 2020 2020 6966 2061 7574  ].        if aut
+0000dad0: 6f5f 616c 6961 733a 0a20 2020 2020 2020  o_alias:.       
+0000dae0: 2020 2020 2061 7574 6f5f 616c 6961 735f       auto_alias_
+0000daf0: 7374 6174 735f 6964 203d 2061 6c69 6173  stats_id = alias
+0000db00: 202b 2022 2d73 7461 7473 220a 2020 2020   + "-stats".    
+0000db10: 2020 2020 2020 2020 7374 6174 735f 616c          stats_al
+0000db20: 6961 7365 732e 6170 7065 6e64 2861 7574  iases.append(aut
+0000db30: 6f5f 616c 6961 735f 7374 6174 735f 6964  o_alias_stats_id
+0000db40: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+0000db50: 2063 6865 636b 2069 6620 7468 6520 7375   check if the su
+0000db60: 6d6d 6172 792d 7374 6174 7320 616c 6961  mmary-stats alia
+0000db70: 7320 616c 7265 6164 7920 6578 6973 742e  s already exist.
+0000db80: 2057 6520 6e65 6564 2074 6f20 646f 2074   We need to do t
+0000db90: 6869 7320 6173 2073 756d 6d61 7279 2d73  his as summary-s
+0000dba0: 7461 7473 2072 6573 6f75 7263 6573 0a20  tats resources. 
+0000dbb0: 2020 2020 2020 2020 2020 2023 206d 6179             # may
+0000dbc0: 2065 6e64 2075 7020 6861 7669 6e67 2074   end up having t
+0000dbd0: 6865 2073 616d 6520 616c 6961 7320 6966  he same alias if
+0000dbe0: 2041 5554 4f5f 414c 4941 535f 554e 4951   AUTO_ALIAS_UNIQ
+0000dbf0: 5545 2069 7320 4661 6c73 652c 2073 6f20  UE is False, so 
+0000dc00: 7765 206e 6565 6420 746f 2064 726f 7020  we need to drop 
+0000dc10: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0000dc20: 2320 6578 6973 7469 6e67 2073 756d 6d61  # existing summa
+0000dc30: 7279 2073 7461 7473 2d61 6c69 6173 2e0a  ry stats-alias..
+0000dc40: 2020 2020 2020 2020 2020 2020 6578 6973              exis
+0000dc50: 7469 6e67 5f61 6c69 6173 5f73 7461 7473  ting_alias_stats
+0000dc60: 203d 2064 6174 6173 746f 7265 5f72 6573   = datastore_res
+0000dc70: 6f75 7263 655f 6578 6973 7473 280a 2020  ource_exists(.  
+0000dc80: 2020 2020 2020 2020 2020 2020 2020 6175                au
+0000dc90: 746f 5f61 6c69 6173 5f73 7461 7473 5f69  to_alias_stats_i
+0000dca0: 642c 2061 7069 5f6b 6579 2c20 636b 616e  d, api_key, ckan
+0000dcb0: 5f75 726c 0a20 2020 2020 2020 2020 2020  _url.           
+0000dcc0: 2029 0a20 2020 2020 2020 2020 2020 2023   ).            #
+0000dcd0: 2044 656c 6574 6520 6578 6973 7469 6e67   Delete existing
+0000dce0: 2061 7574 6f2d 616c 6961 7365 6420 7375   auto-aliased su
+0000dcf0: 6d6d 6172 792d 7374 6174 7320 6265 666f  mmary-stats befo
+0000dd00: 7265 2070 726f 6365 6564 696e 672e 0a20  re proceeding.. 
+0000dd10: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
+0000dd20: 6973 7469 6e67 5f61 6c69 6173 5f73 7461  isting_alias_sta
+0000dd30: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+0000dd40: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+0000dd50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd60: 2020 2020 2027 4465 6c65 7469 6e67 2065       'Deleting e
+0000dd70: 7869 7374 696e 6720 616c 6961 7320 7375  xisting alias su
+0000dd80: 6d6d 6172 7920 7374 6174 7320 227b 7d22  mmary stats "{}"
+0000dd90: 2e27 2e66 6f72 6d61 7428 0a20 2020 2020  .'.format(.     
+0000dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddb0: 2020 2061 7574 6f5f 616c 6961 735f 7374     auto_alias_st
+0000ddc0: 6174 735f 6964 0a20 2020 2020 2020 2020  ats_id.         
+0000ddd0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000dde0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de00: 6375 722e 6578 6563 7574 6528 0a20 2020  cur.execute(.   
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2022 5345 4c45 4354 2061 6c69 6173 5f6f   "SELECT alias_o
+0000de30: 6620 4652 4f4d 205f 7461 626c 655f 6d65  f FROM _table_me
+0000de40: 7461 6461 7461 2077 6865 7265 206e 616d  tadata where nam
+0000de50: 6520 6c69 6b65 2025 7320 6772 6f75 7020  e like %s group 
+0000de60: 6279 2061 6c69 6173 5f6f 663b 222c 0a20  by alias_of;",. 
+0000de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de80: 2020 2028 6175 746f 5f61 6c69 6173 5f73     (auto_alias_s
+0000de90: 7461 7473 5f69 6420 2b20 2225 222c 292c  tats_id + "%",),
+0000dea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000deb0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000dec0: 2020 2072 6573 756c 7420 3d20 6375 722e     result = cur.
+0000ded0: 6665 7463 686f 6e65 2829 0a20 2020 2020  fetchone().     
+0000dee0: 2020 2020 2020 2020 2020 2069 6620 7265             if re
+0000def0: 7375 6c74 3a0a 2020 2020 2020 2020 2020  sult:.          
+0000df00: 2020 2020 2020 2020 2020 6578 6973 7469            existi
+0000df10: 6e67 5f73 7461 7473 5f61 6c69 6173 5f6f  ng_stats_alias_o
+0000df20: 6620 3d20 7265 7375 6c74 5b30 5d0a 0a20  f = result[0].. 
+0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df40: 2020 2064 656c 6574 655f 6461 7461 7374     delete_datast
+0000df50: 6f72 655f 7265 736f 7572 6365 280a 2020  ore_resource(.  
+0000df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df70: 2020 2020 2020 6578 6973 7469 6e67 5f73        existing_s
+0000df80: 7461 7473 5f61 6c69 6173 5f6f 662c 2061  tats_alias_of, a
+0000df90: 7069 5f6b 6579 2c20 636b 616e 5f75 726c  pi_key, ckan_url
+0000dfa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dfb0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000dfc0: 2020 2020 2020 2020 2020 2064 656c 6574             delet
+0000dfd0: 655f 7265 736f 7572 6365 2865 7869 7374  e_resource(exist
+0000dfe0: 696e 675f 7374 6174 735f 616c 6961 735f  ing_stats_alias_
+0000dff0: 6f66 2c20 6170 695f 6b65 792c 2063 6b61  of, api_key, cka
+0000e000: 6e5f 7572 6c29 0a0a 2020 2020 2020 2020  n_url)..        
+0000e010: 2320 7275 6e20 7374 6174 7320 6f6e 2073  # run stats on s
+0000e020: 7461 7473 2043 5356 2074 6f20 6765 7420  tats CSV to get 
+0000e030: 6865 6164 6572 206e 616d 6573 2061 6e64  header names and
+0000e040: 2069 6e66 6572 2064 6174 6120 7479 7065   infer data type
+0000e050: 730a 2020 2020 2020 2020 2320 7765 2064  s.        # we d
+0000e060: 6f6e 2774 206e 6565 6420 7375 6d6d 6172  on't need summar
+0000e070: 7920 7374 6174 6973 7469 6373 2c20 736f  y statistics, so
+0000e080: 2075 7365 2074 6865 202d 2d74 7970 6573   use the --types
+0000e090: 6f6e 6c79 206f 7074 696f 6e0a 2020 2020  only option.    
+0000e0a0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+0000e0b0: 2020 2020 2071 7376 5f73 7461 7473 5f73       qsv_stats_s
+0000e0c0: 7461 7473 203d 2073 7562 7072 6f63 6573  tats = subproces
+0000e0d0: 732e 7275 6e28 0a20 2020 2020 2020 2020  s.run(.         
+0000e0e0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+0000e0f0: 2020 2020 2020 2020 2020 2020 2071 7376               qsv
+0000e100: 5f62 696e 2c0a 2020 2020 2020 2020 2020  _bin,.          
+0000e110: 2020 2020 2020 2020 2020 2273 7461 7473            "stats
+0000e120: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000e130: 2020 2020 2020 2022 2d2d 7479 7065 736f         "--typeso
+0000e140: 6e6c 7922 2c0a 2020 2020 2020 2020 2020  nly",.          
+0000e150: 2020 2020 2020 2020 2020 7173 765f 7374            qsv_st
+0000e160: 6174 735f 6373 762e 6e61 6d65 2c0a 2020  ats_csv.name,.  
+0000e170: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
+0000e180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e190: 2063 6170 7475 7265 5f6f 7574 7075 743d   capture_output=
+0000e1a0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+0000e1b0: 2020 2020 2020 6368 6563 6b3d 5472 7565        check=True
+0000e1c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e1d0: 2020 7465 7874 3d54 7275 652c 0a20 2020    text=True,.   
+0000e1e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000e1f0: 2020 2065 7863 6570 7420 7375 6270 726f     except subpro
+0000e200: 6365 7373 2e43 616c 6c65 6450 726f 6365  cess.CalledProce
+0000e210: 7373 4572 726f 7220 6173 2065 3a0a 2020  ssError as e:.  
+0000e220: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000e230: 7574 696c 2e4a 6f62 4572 726f 7228 2243  util.JobError("C
+0000e240: 616e 6e6f 7420 7275 6e20 7374 6174 7320  annot run stats 
+0000e250: 6f6e 2043 5356 2073 7461 7473 3a20 7b7d  on CSV stats: {}
+0000e260: 222e 666f 726d 6174 2865 2929 0a0a 2020  ".format(e))..  
+0000e270: 2020 2020 2020 7374 6174 735f 7374 6174        stats_stat
+0000e280: 7320 3d20 7374 7228 7173 765f 7374 6174  s = str(qsv_stat
+0000e290: 735f 7374 6174 732e 7374 646f 7574 292e  s_stats.stdout).
+0000e2a0: 7374 7269 7028 290a 2020 2020 2020 2020  strip().        
+0000e2b0: 7374 6174 735f 7374 6174 735f 6469 6374  stats_stats_dict
+0000e2c0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+0000e2d0: 2064 6963 7428 6964 3d65 6c65 2e73 706c   dict(id=ele.spl
+0000e2e0: 6974 2822 2c22 295b 305d 2c20 7479 7065  it(",")[0], type
+0000e2f0: 3d74 7970 655f 6d61 7070 696e 675b 656c  =type_mapping[el
+0000e300: 652e 7370 6c69 7428 222c 2229 5b31 5d5d  e.split(",")[1]]
+0000e310: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000e320: 7220 6964 782c 2065 6c65 2069 6e20 656e  r idx, ele in en
+0000e330: 756d 6572 6174 6528 7374 6174 735f 7374  umerate(stats_st
+0000e340: 6174 732e 7370 6c69 746c 696e 6573 2829  ats.splitlines()
+0000e350: 5b31 3a5d 2c20 3129 0a20 2020 2020 2020  [1:], 1).       
+0000e360: 205d 0a0a 2020 2020 2020 2020 7374 6174   ]..        stat
+0000e370: 735f 7265 736f 7572 6365 203d 207b 0a20  s_resource = {. 
+0000e380: 2020 2020 2020 2020 2020 2022 7061 636b             "pack
+0000e390: 6167 655f 6964 223a 2072 6573 6f75 7263  age_id": resourc
+0000e3a0: 655b 2270 6163 6b61 6765 5f69 6422 5d2c  e["package_id"],
+0000e3b0: 0a20 2020 2020 2020 2020 2020 2022 6e61  .            "na
+0000e3c0: 6d65 223a 2072 6573 6f75 7263 655f 6e61  me": resource_na
+0000e3d0: 6d65 202b 2022 202d 2053 756d 6d61 7279  me + " - Summary
+0000e3e0: 2053 7461 7469 7374 6963 7322 2c0a 2020   Statistics",.  
+0000e3f0: 2020 2020 2020 2020 2020 2266 6f72 6d61            "forma
+0000e400: 7422 3a20 2243 5356 222c 0a20 2020 2020  t": "CSV",.     
+0000e410: 2020 2020 2020 2022 6d69 6d65 7479 7065         "mimetype
+0000e420: 223a 2022 7465 7874 2f63 7376 222c 0a20  ": "text/csv",. 
+0000e430: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+0000e440: 2073 7461 7473 5f72 6573 706f 6e73 6520   stats_response 
+0000e450: 3d20 7365 6e64 5f72 6573 6f75 7263 655f  = send_resource_
+0000e460: 746f 5f64 6174 6173 746f 7265 280a 2020  to_datastore(.  
+0000e470: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
+0000e480: 7265 736f 7572 6365 2c0a 2020 2020 2020  resource,.      
+0000e490: 2020 2020 2020 7265 736f 7572 6365 5f69        resource_i
+0000e4a0: 643d 4e6f 6e65 2c0a 2020 2020 2020 2020  d=None,.        
+0000e4b0: 2020 2020 6865 6164 6572 733d 7374 6174      headers=stat
+0000e4c0: 735f 7374 6174 735f 6469 6374 2c0a 2020  s_stats_dict,.  
+0000e4d0: 2020 2020 2020 2020 2020 6170 695f 6b65            api_ke
+0000e4e0: 793d 6170 695f 6b65 792c 0a20 2020 2020  y=api_key,.     
+0000e4f0: 2020 2020 2020 2063 6b61 6e5f 7572 6c3d         ckan_url=
+0000e500: 636b 616e 5f75 726c 2c0a 2020 2020 2020  ckan_url,.      
+0000e510: 2020 2020 2020 7265 636f 7264 733d 4e6f        records=No
+0000e520: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+0000e530: 616c 6961 7365 733d 7374 6174 735f 616c  aliases=stats_al
+0000e540: 6961 7365 732c 0a20 2020 2020 2020 2020  iases,.         
+0000e550: 2020 2063 616c 6375 6c61 7465 5f72 6563     calculate_rec
+0000e560: 6f72 645f 636f 756e 743d 4661 6c73 652c  ord_count=False,
+0000e570: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+0000e580: 2020 2020 6e65 775f 7374 6174 735f 7265      new_stats_re
+0000e590: 736f 7572 6365 5f69 6420 3d20 7374 6174  source_id = stat
+0000e5a0: 735f 7265 7370 6f6e 7365 5b22 7265 7375  s_response["resu
+0000e5b0: 6c74 225d 5b22 7265 736f 7572 6365 5f69  lt"]["resource_i
+0000e5c0: 6422 5d0a 0a20 2020 2020 2020 2023 206e  d"]..        # n
+0000e5d0: 6f77 2043 4f50 5920 7468 6520 7374 6174  ow COPY the stat
+0000e5e0: 7320 746f 2074 6865 2064 6174 6173 746f  s to the datasto
+0000e5f0: 7265 0a20 2020 2020 2020 2063 6f6c 5f6e  re.        col_n
+0000e600: 616d 6573 5f6c 6973 7420 3d20 5b68 5b22  ames_list = [h["
+0000e610: 6964 225d 2066 6f72 2068 2069 6e20 7374  id"] for h in st
+0000e620: 6174 735f 7374 6174 735f 6469 6374 5d0a  ats_stats_dict].
+0000e630: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000e640: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
+0000e650: 2027 4144 4449 4e47 2053 554d 4d41 5259   'ADDING SUMMARY
+0000e660: 2053 5441 5449 5354 4943 5320 7b7d 2069   STATISTICS {} i
+0000e670: 6e20 227b 7d22 2077 6974 6820 616c 6961  n "{}" with alia
+0000e680: 732f 6573 2022 7b7d 222e 2e2e 272e 666f  s/es "{}"...'.fo
+0000e690: 726d 6174 280a 2020 2020 2020 2020 2020  rmat(.          
+0000e6a0: 2020 2020 2020 636f 6c5f 6e61 6d65 735f        col_names_
+0000e6b0: 6c69 7374 2c0a 2020 2020 2020 2020 2020  list,.          
+0000e6c0: 2020 2020 2020 6e65 775f 7374 6174 735f        new_stats_
+0000e6d0: 7265 736f 7572 6365 5f69 642c 0a20 2020  resource_id,.   
+0000e6e0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0000e6f0: 7473 5f61 6c69 6173 6573 2c0a 2020 2020  ts_aliases,.    
+0000e700: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e710: 2020 290a 0a20 2020 2020 2020 2063 6f6c    )..        col
+0000e720: 756d 6e5f 6e61 6d65 7320 3d20 7371 6c2e  umn_names = sql.
+0000e730: 5351 4c28 222c 2229 2e6a 6f69 6e28 7371  SQL(",").join(sq
+0000e740: 6c2e 4964 656e 7469 6669 6572 2863 2920  l.Identifier(c) 
+0000e750: 666f 7220 6320 696e 2063 6f6c 5f6e 616d  for c in col_nam
+0000e760: 6573 5f6c 6973 7429 0a0a 2020 2020 2020  es_list)..      
+0000e770: 2020 636f 7079 5f73 716c 203d 2073 716c    copy_sql = sql
+0000e780: 2e53 514c 280a 2020 2020 2020 2020 2020  .SQL(.          
+0000e790: 2020 2243 4f50 5920 7b7d 2028 7b7d 2920    "COPY {} ({}) 
+0000e7a0: 4652 4f4d 2053 5444 494e 2022 0a20 2020  FROM STDIN ".   
+0000e7b0: 2020 2020 2020 2020 2022 5749 5448 2028           "WITH (
+0000e7c0: 464f 524d 4154 2043 5356 2c20 220a 2020  FORMAT CSV, ".  
+0000e7d0: 2020 2020 2020 2020 2020 2248 4541 4445            "HEADE
+0000e7e0: 5220 312c 2045 4e43 4f44 494e 4720 2755  R 1, ENCODING 'U
+0000e7f0: 5446 3827 293b 220a 2020 2020 2020 2020  TF8');".        
+0000e800: 292e 666f 726d 6174 280a 2020 2020 2020  ).format(.      
+0000e810: 2020 2020 2020 7371 6c2e 4964 656e 7469        sql.Identi
+0000e820: 6669 6572 286e 6577 5f73 7461 7473 5f72  fier(new_stats_r
+0000e830: 6573 6f75 7263 655f 6964 292c 0a20 2020  esource_id),.   
+0000e840: 2020 2020 2020 2020 2063 6f6c 756d 6e5f           column_
+0000e850: 6e61 6d65 732c 0a20 2020 2020 2020 2029  names,.        )
+0000e860: 0a0a 2020 2020 2020 2020 7769 7468 206f  ..        with o
+0000e870: 7065 6e28 7173 765f 7374 6174 735f 6373  pen(qsv_stats_cs
+0000e880: 762e 6e61 6d65 2c20 2272 6222 2920 6173  v.name, "rb") as
+0000e890: 2066 3a0a 2020 2020 2020 2020 2020 2020   f:.            
+0000e8a0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000e8b0: 2020 2020 2063 7572 2e63 6f70 795f 6578       cur.copy_ex
+0000e8c0: 7065 7274 2863 6f70 795f 7371 6c2c 2066  pert(copy_sql, f
+0000e8d0: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+0000e8e0: 6365 7074 2070 7379 636f 7067 322e 4572  cept psycopg2.Er
+0000e8f0: 726f 7220 6173 2065 3a0a 2020 2020 2020  ror as e:.      
+0000e900: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000e910: 7574 696c 2e4a 6f62 4572 726f 7228 2250  util.JobError("P
+0000e920: 6f73 7467 7265 7320 434f 5059 2066 6169  ostgres COPY fai
+0000e930: 6c65 643a 207b 7d22 2e66 6f72 6d61 7428  led: {}".format(
+0000e940: 6529 290a 0a20 2020 2020 2020 2073 7461  e))..        sta
+0000e950: 7473 5f72 6573 6f75 7263 655b 2269 6422  ts_resource["id"
+0000e960: 5d20 3d20 6e65 775f 7374 6174 735f 7265  ] = new_stats_re
+0000e970: 736f 7572 6365 5f69 640a 2020 2020 2020  source_id.      
+0000e980: 2020 7374 6174 735f 7265 736f 7572 6365    stats_resource
+0000e990: 5b22 7375 6d6d 6172 795f 7374 6174 6973  ["summary_statis
+0000e9a0: 7469 6373 225d 203d 2054 7275 650a 2020  tics"] = True.  
+0000e9b0: 2020 2020 2020 7374 6174 735f 7265 736f        stats_reso
+0000e9c0: 7572 6365 5b22 7375 6d6d 6172 795f 6f66  urce["summary_of
+0000e9d0: 5f72 6573 6f75 7263 6522 5d20 3d20 7265  _resource"] = re
+0000e9e0: 736f 7572 6365 5f69 640a 2020 2020 2020  source_id.      
+0000e9f0: 2020 7570 6461 7465 5f72 6573 6f75 7263    update_resourc
+0000ea00: 6528 7374 6174 735f 7265 736f 7572 6365  e(stats_resource
+0000ea10: 2c20 636b 616e 5f75 726c 2c20 6170 695f  , ckan_url, api_
+0000ea20: 6b65 7929 0a0a 2020 2020 6375 722e 636c  key)..    cur.cl
+0000ea30: 6f73 6528 290a 2020 2020 7261 775f 636f  ose().    raw_co
+0000ea40: 6e6e 6563 7469 6f6e 2e63 6f6d 6d69 7428  nnection.commit(
+0000ea50: 290a 0a20 2020 2072 6573 6f75 7263 655b  )..    resource[
+0000ea60: 2264 6174 6173 746f 7265 5f61 6374 6976  "datastore_activ
+0000ea70: 6522 5d20 3d20 5472 7565 0a20 2020 2072  e"] = True.    r
+0000ea80: 6573 6f75 7263 655b 2274 6f74 616c 5f72  esource["total_r
+0000ea90: 6563 6f72 645f 636f 756e 7422 5d20 3d20  ecord_count"] = 
+0000eaa0: 7265 636f 7264 5f63 6f75 6e74 0a20 2020  record_count.   
+0000eab0: 2069 6620 7072 6576 6965 775f 726f 7773   if preview_rows
+0000eac0: 203c 2072 6563 6f72 645f 636f 756e 7420   < record_count 
+0000ead0: 6f72 2028 7072 6576 6965 775f 726f 7773  or (preview_rows
+0000eae0: 203e 2030 2061 6e64 2064 6f77 6e6c 6f61   > 0 and downloa
+0000eaf0: 645f 7072 6576 6965 775f 6f6e 6c79 293a  d_preview_only):
+0000eb00: 0a20 2020 2020 2020 2072 6573 6f75 7263  .        resourc
+0000eb10: 655b 2270 7265 7669 6577 225d 203d 2054  e["preview"] = T
+0000eb20: 7275 650a 2020 2020 2020 2020 7265 736f  rue.        reso
+0000eb30: 7572 6365 5b22 7072 6576 6965 775f 726f  urce["preview_ro
+0000eb40: 7773 225d 203d 2063 6f70 6965 645f 636f  ws"] = copied_co
+0000eb50: 756e 740a 2020 2020 2020 2020 7265 736f  unt.        reso
+0000eb60: 7572 6365 5b22 7061 7274 6961 6c5f 646f  urce["partial_do
+0000eb70: 776e 6c6f 6164 225d 203d 2064 6f77 6e6c  wnload"] = downl
+0000eb80: 6f61 645f 7072 6576 6965 775f 6f6e 6c79  oad_preview_only
+0000eb90: 0a20 2020 2075 7064 6174 655f 7265 736f  .    update_reso
+0000eba0: 7572 6365 2872 6573 6f75 7263 652c 2063  urce(resource, c
+0000ebb0: 6b61 6e5f 7572 6c2c 2061 7069 5f6b 6579  kan_url, api_key
+0000ebc0: 290a 0a20 2020 2023 2074 656c 6c20 434b  )..    # tell CK
+0000ebd0: 414e 2074 6f20 6361 6c63 756c 6174 655f  AN to calculate_
+0000ebe0: 7265 636f 7264 5f63 6f75 6e74 2061 6e64  record_count and
+0000ebf0: 2073 6574 2061 6c69 6173 2069 6620 7365   set alias if se
+0000ec00: 740a 2020 2020 7365 6e64 5f72 6573 6f75  t.    send_resou
+0000ec10: 7263 655f 746f 5f64 6174 6173 746f 7265  rce_to_datastore
+0000ec20: 280a 2020 2020 2020 2020 7265 736f 7572  (.        resour
+0000ec30: 6365 3d4e 6f6e 652c 0a20 2020 2020 2020  ce=None,.       
+0000ec40: 2072 6573 6f75 7263 655f 6964 3d72 6573   resource_id=res
+0000ec50: 6f75 7263 655b 2269 6422 5d2c 0a20 2020  ource["id"],.   
+0000ec60: 2020 2020 2068 6561 6465 7273 3d68 6561       headers=hea
+0000ec70: 6465 7273 5f64 6963 7473 2c0a 2020 2020  ders_dicts,.    
+0000ec80: 2020 2020 6170 695f 6b65 793d 6170 695f      api_key=api_
+0000ec90: 6b65 792c 0a20 2020 2020 2020 2063 6b61  key,.        cka
+0000eca0: 6e5f 7572 6c3d 636b 616e 5f75 726c 2c0a  n_url=ckan_url,.
+0000ecb0: 2020 2020 2020 2020 7265 636f 7264 733d          records=
+0000ecc0: 4e6f 6e65 2c0a 2020 2020 2020 2020 616c  None,.        al
+0000ecd0: 6961 7365 733d 616c 6961 732c 0a20 2020  iases=alias,.   
+0000ece0: 2020 2020 2063 616c 6375 6c61 7465 5f72       calculate_r
+0000ecf0: 6563 6f72 645f 636f 756e 743d 5472 7565  ecord_count=True
+0000ed00: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
+0000ed10: 616c 6961 733a 0a20 2020 2020 2020 206c  alias:.        l
+0000ed20: 6f67 6765 722e 696e 666f 2827 4372 6561  ogger.info('Crea
+0000ed30: 7465 6420 616c 6961 7320 227b 7d22 2066  ted alias "{}" f
+0000ed40: 6f72 2022 7b7d 222e 2e2e 272e 666f 726d  or "{}"...'.form
+0000ed50: 6174 2861 6c69 6173 2c20 7265 736f 7572  at(alias, resour
+0000ed60: 6365 5f69 6429 290a 0a20 2020 206d 6574  ce_id))..    met
+0000ed70: 6164 6174 615f 656c 6170 7365 6420 3d20  adata_elapsed = 
+0000ed80: 7469 6d65 2e70 6572 665f 636f 756e 7465  time.perf_counte
+0000ed90: 7228 2920 2d20 6d65 7461 6461 7461 5f73  r() - metadata_s
+0000eda0: 7461 7274 0a20 2020 206c 6f67 6765 722e  tart.    logger.
+0000edb0: 696e 666f 280a 2020 2020 2020 2020 224d  info(.        "M
+0000edc0: 4554 4144 4154 4120 5550 4441 5445 5320  ETADATA UPDATES 
+0000edd0: 444f 4e45 2120 5265 736f 7572 6365 206d  DONE! Resource m
+0000ede0: 6574 6164 6174 6120 7570 6461 7465 6420  etadata updated 
+0000edf0: 696e 207b 3a2e 3266 7d20 7365 636f 6e64  in {:.2f} second
+0000ee00: 732e 222e 666f 726d 6174 280a 2020 2020  s.".format(.    
+0000ee10: 2020 2020 2020 2020 6d65 7461 6461 7461          metadata
+0000ee20: 5f65 6c61 7073 6564 0a20 2020 2020 2020  _elapsed.       
+0000ee30: 2029 0a20 2020 2029 0a0a 2020 2020 2320   ).    )..    # 
+0000ee40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ee50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ee60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ee70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ee80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ee90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000eea0: 3d0a 2020 2020 2320 494e 4445 5849 4e47  =.    # INDEXING
+0000eeb0: 0a20 2020 2023 203d 3d3d 3d3d 3d3d 3d3d  .    # =========
+0000eec0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000eed0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000eee0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000eef0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ef00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ef10: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2023 2069  ========.    # i
+0000ef20: 6620 4155 544f 5f49 4e44 4558 5f54 4852  f AUTO_INDEX_THR
+0000ef30: 4553 484f 4c44 203e 2030 206f 7220 4155  ESHOLD > 0 or AU
+0000ef40: 544f 5f49 4e44 4558 5f44 4154 4553 2069  TO_INDEX_DATES i
+0000ef50: 7320 7472 7565 0a20 2020 2023 2063 7265  s true.    # cre
+0000ef60: 6174 6520 696e 6469 6365 7320 6175 746f  ate indices auto
+0000ef70: 6d61 7469 6361 6c6c 7920 6261 7365 6420  matically based 
+0000ef80: 6f6e 2073 756d 6d61 7279 2073 7461 7469  on summary stati
+0000ef90: 7374 6963 730a 2020 2020 2320 466f 7220  stics.    # For 
+0000efa0: 636f 6c75 6d6e 7320 772f 2063 6172 6469  columns w/ cardi
+0000efb0: 6e61 6c69 7479 203d 2072 6563 6f72 645f  nality = record_
+0000efc0: 636f 756e 742c 2069 7427 7320 616c 6c20  count, it's all 
+0000efd0: 756e 6971 7565 2076 616c 7565 732c 2063  unique values, c
+0000efe0: 7265 6174 6520 6120 756e 6971 7565 2069  reate a unique i
+0000eff0: 6e64 6578 0a20 2020 2023 2049 6620 4155  ndex.    # If AU
+0000f000: 544f 5f49 4e44 4558 5f44 4154 4553 2069  TO_INDEX_DATES i
+0000f010: 7320 7472 7565 2c20 696e 6465 7820 616c  s true, index al
+0000f020: 6c20 6461 7465 2063 6f6c 756d 6e73 0a20  l date columns. 
+0000f030: 2020 2023 2069 6620 6120 636f 6c75 6d6e     # if a column
+0000f040: 2773 2063 6172 6469 6e61 6c69 7479 203c  's cardinality <
+0000f050: 3d20 4155 544f 5f49 4e44 4558 5f54 4852  = AUTO_INDEX_THR
+0000f060: 4553 484f 4c44 2c20 6372 6561 7465 2061  ESHOLD, create a
+0000f070: 6e20 696e 6465 7820 666f 7220 7468 6174  n index for that
+0000f080: 2063 6f6c 756d 6e0a 2020 2020 6175 746f   column.    auto
+0000f090: 5f69 6e64 6578 5f64 6174 6573 203d 2063  _index_dates = c
+0000f0a0: 6f6e 6669 672e 6765 7428 2241 5554 4f5f  onfig.get("AUTO_
+0000f0b0: 494e 4445 585f 4441 5445 5322 290a 2020  INDEX_DATES").  
+0000f0c0: 2020 6966 2061 7574 6f5f 696e 6465 785f    if auto_index_
+0000f0d0: 7468 7265 7368 6f6c 6420 6f72 2028 6175  threshold or (au
+0000f0e0: 746f 5f69 6e64 6578 5f64 6174 6573 2061  to_index_dates a
+0000f0f0: 6e64 2064 6174 6574 696d 6563 6f6c 735f  nd datetimecols_
+0000f100: 6c69 7374 293a 0a20 2020 2020 2020 2069  list):.        i
+0000f110: 6e64 6578 5f73 7461 7274 203d 2074 696d  ndex_start = tim
+0000f120: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
+0000f130: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000f140: 696e 666f 280a 2020 2020 2020 2020 2020  info(.          
+0000f150: 2020 2241 5554 4f2d 494e 4445 5849 4e47    "AUTO-INDEXING
+0000f160: 2e20 4175 746f 2d69 6e64 6578 2074 6872  . Auto-index thr
+0000f170: 6573 686f 6c64 3a20 7b3a 2c7d 2075 6e69  eshold: {:,} uni
+0000f180: 7175 6520 7661 6c75 652f 732e 2041 7574  que value/s. Aut
+0000f190: 6f2d 696e 6465 7820 6461 7465 733a 207b  o-index dates: {
+0000f1a0: 7d20 2e2e 2e22 2e66 6f72 6d61 7428 0a20  } ...".format(. 
+0000f1b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000f1c0: 7574 6f5f 696e 6465 785f 7468 7265 7368  uto_index_thresh
+0000f1d0: 6f6c 642c 2061 7574 6f5f 696e 6465 785f  old, auto_index_
+0000f1e0: 6461 7465 730a 2020 2020 2020 2020 2020  dates.          
+0000f1f0: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
+0000f200: 2020 2020 2020 696e 6465 785f 6375 7220        index_cur 
+0000f210: 3d20 7261 775f 636f 6e6e 6563 7469 6f6e  = raw_connection
+0000f220: 2e63 7572 736f 7228 290a 0a20 2020 2020  .cursor()..     
+0000f230: 2020 2023 2069 6620 6175 746f 5f69 6e64     # if auto_ind
+0000f240: 6578 5f74 6872 6573 686f 6c64 203d 3d20  ex_threshold == 
+0000f250: 2d31 0a20 2020 2020 2020 2023 2077 6520  -1.        # we 
+0000f260: 696e 6465 7820 616c 6c20 7468 6520 636f  index all the co
+0000f270: 6c75 6d6e 730a 2020 2020 2020 2020 6966  lumns.        if
+0000f280: 2061 7574 6f5f 696e 6465 785f 7468 7265   auto_index_thre
+0000f290: 7368 6f6c 6420 3d3d 202d 313a 0a20 2020  shold == -1:.   
+0000f2a0: 2020 2020 2020 2020 2061 7574 6f5f 696e           auto_in
+0000f2b0: 6465 785f 7468 7265 7368 6f6c 6420 3d20  dex_threshold = 
+0000f2c0: 7265 636f 7264 5f63 6f75 6e74 0a0a 2020  record_count..  
+0000f2d0: 2020 2020 2020 696e 6465 785f 636f 756e        index_coun
+0000f2e0: 7420 3d20 300a 2020 2020 2020 2020 666f  t = 0.        fo
+0000f2f0: 7220 6964 782c 2063 6172 6469 6e61 6c69  r idx, cardinali
+0000f300: 7479 2069 6e20 656e 756d 6572 6174 6528  ty in enumerate(
+0000f310: 6865 6164 6572 735f 6361 7264 696e 616c  headers_cardinal
+0000f320: 6974 7929 3a0a 0a20 2020 2020 2020 2020  ity):..         
+0000f330: 2020 2063 7572 725f 636f 6c20 3d20 6865     curr_col = he
+0000f340: 6164 6572 735b 6964 785d 0a20 2020 2020  aders[idx].     
+0000f350: 2020 2020 2020 2069 6620 6175 746f 5f69         if auto_i
+0000f360: 6e64 6578 5f74 6872 6573 686f 6c64 203e  ndex_threshold >
+0000f370: 2030 206f 7220 6175 746f 5f69 6e64 6578   0 or auto_index
+0000f380: 5f64 6174 6573 3a0a 2020 2020 2020 2020  _dates:.        
+0000f390: 2020 2020 2020 2020 6966 2063 6172 6469          if cardi
+0000f3a0: 6e61 6c69 7479 203d 3d20 7265 636f 7264  nality == record
+0000f3b0: 5f63 6f75 6e74 3a0a 2020 2020 2020 2020  _count:.        
+0000f3c0: 2020 2020 2020 2020 2020 2020 2320 616c              # al
+0000f3d0: 6c20 7468 6520 7661 6c75 6573 2061 7265  l the values are
+0000f3e0: 2075 6e69 7175 6520 666f 7220 7468 6973   unique for this
+0000f3f0: 2063 6f6c 756d 6e2c 2063 7265 6174 6520   column, create 
+0000f400: 6120 756e 6971 7565 2069 6e64 6578 0a20  a unique index. 
+0000f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f420: 2020 2075 6e69 7175 655f 7661 6c75 655f     unique_value_
+0000f430: 636f 756e 7420 3d20 6d69 6e28 7072 6576  count = min(prev
+0000f440: 6965 775f 726f 7773 2c20 6361 7264 696e  iew_rows, cardin
+0000f450: 616c 6974 7929 0a20 2020 2020 2020 2020  ality).         
+0000f460: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+0000f470: 722e 696e 666f 280a 2020 2020 2020 2020  r.info(.        
+0000f480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f490: 2743 7265 6174 696e 6720 554e 4951 5545  'Creating UNIQUE
+0000f4a0: 2069 6e64 6578 206f 6e20 227b 7d22 2066   index on "{}" f
+0000f4b0: 6f72 207b 3a2c 7d20 756e 6971 7565 2076  or {:,} unique v
+0000f4c0: 616c 7565 732e 2e2e 272e 666f 726d 6174  alues...'.format
+0000f4d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000f4e0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
+0000f4f0: 7272 5f63 6f6c 2c20 756e 6971 7565 5f76  rr_col, unique_v
+0000f500: 616c 7565 5f63 6f75 6e74 0a20 2020 2020  alue_count.     
+0000f510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f520: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000f530: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000f540: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000f550: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000f560: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+0000f570: 785f 6375 722e 6578 6563 7574 6528 0a20  x_cur.execute(. 
+0000f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f590: 2020 2020 2020 2020 2020 2073 716c 2e53             sql.S
+0000f5a0: 514c 2822 4352 4541 5445 2055 4e49 5155  QL("CREATE UNIQU
+0000f5b0: 4520 494e 4445 5820 4f4e 207b 7d20 287b  E INDEX ON {} ({
+0000f5c0: 7d29 2229 2e66 6f72 6d61 7428 0a20 2020  })").format(.   
+0000f5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5e0: 2020 2020 2020 2020 2020 2020 2073 716c               sql
+0000f5f0: 2e49 6465 6e74 6966 6965 7228 7265 736f  .Identifier(reso
+0000f600: 7572 6365 5f69 6429 2c0a 2020 2020 2020  urce_id),.      
+0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f620: 2020 2020 2020 2020 2020 7371 6c2e 4964            sql.Id
+0000f630: 656e 7469 6669 6572 2863 7572 725f 636f  entifier(curr_co
+0000f640: 6c29 2c0a 2020 2020 2020 2020 2020 2020  l),.            
+0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f660: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000f670: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f690: 6578 6365 7074 2070 7379 636f 7067 322e  except psycopg2.
+0000f6a0: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
+0000f6d0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6f0: 2743 6f75 6c64 206e 6f74 2043 5245 4154  'Could not CREAT
+0000f700: 4520 554e 4951 5545 2049 4e44 4558 206f  E UNIQUE INDEX o
+0000f710: 6e20 227b 7d22 3a20 7b7d 272e 666f 726d  n "{}": {}'.form
+0000f720: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f740: 2020 2020 6375 7272 5f63 6f6c 2c20 650a      curr_col, e.
+0000f750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f760: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000f770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f780: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000f790: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+0000f7a0: 785f 636f 756e 7420 2b3d 2031 0a20 2020  x_count += 1.   
+0000f7b0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0000f7c0: 6620 6361 7264 696e 616c 6974 7920 3c3d  f cardinality <=
+0000f7d0: 2061 7574 6f5f 696e 6465 785f 7468 7265   auto_index_thre
+0000f7e0: 7368 6f6c 6420 6f72 2028 0a20 2020 2020  shold or (.     
+0000f7f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000f800: 7574 6f5f 696e 6465 785f 6461 7465 7320  uto_index_dates 
+0000f810: 616e 6420 2863 7572 725f 636f 6c20 696e  and (curr_col in
+0000f820: 2064 6174 6574 696d 6563 6f6c 735f 6c69   datetimecols_li
+0000f830: 7374 290a 2020 2020 2020 2020 2020 2020  st).            
+0000f840: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+0000f850: 2020 2020 2020 2020 2020 2023 2063 6172             # car
+0000f860: 6469 6e61 6c69 7479 203c 3d20 6175 746f  dinality <= auto
+0000f870: 5f69 6e64 6578 5f74 6872 6573 686f 6c64  _index_threshold
+0000f880: 206f 7220 6974 7320 6120 6461 7465 2061   or its a date a
+0000f890: 6e64 2061 7574 6f5f 696e 6465 785f 6461  nd auto_index_da
+0000f8a0: 7465 2069 7320 7472 7565 0a20 2020 2020  te is true.     
+0000f8b0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f8c0: 2063 7265 6174 6520 616e 2069 6e64 6578   create an index
+0000f8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f8e0: 2020 2020 2069 6620 6375 7272 5f63 6f6c       if curr_col
+0000f8f0: 2069 6e20 6461 7465 7469 6d65 636f 6c73   in datetimecols
+0000f900: 5f6c 6973 743a 0a20 2020 2020 2020 2020  _list:.         
+0000f910: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000f920: 6f67 6765 722e 696e 666f 280a 2020 2020  ogger.info(.    
+0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f940: 2020 2020 2020 2020 2743 7265 6174 696e          'Creatin
+0000f950: 6720 696e 6465 7820 6f6e 2022 7b7d 2220  g index on "{}" 
+0000f960: 6461 7465 2063 6f6c 756d 6e20 666f 7220  date column for 
+0000f970: 7b3a 2c7d 2075 6e69 7175 6520 7661 6c75  {:,} unique valu
+0000f980: 652f 732e 2e2e 272e 666f 726d 6174 280a  e/s...'.format(.
+0000f990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9b0: 6375 7272 5f63 6f6c 2c20 6361 7264 696e  curr_col, cardin
+0000f9c0: 616c 6974 790a 2020 2020 2020 2020 2020  ality.          
+0000f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f9e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000f9f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000fa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa30: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa50: 2020 2020 2020 2020 2027 4372 6561 7469           'Creati
+0000fa60: 6e67 2069 6e64 6578 206f 6e20 227b 7d22  ng index on "{}"
+0000fa70: 2066 6f72 207b 3a2c 7d20 756e 6971 7565   for {:,} unique
+0000fa80: 2076 616c 7565 2f73 2e2e 2e27 2e66 6f72   value/s...'.for
+0000fa90: 6d61 7428 0a20 2020 2020 2020 2020 2020  mat(.           
+0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fab0: 2020 2020 2063 7572 725f 636f 6c2c 2063       curr_col, c
+0000fac0: 6172 6469 6e61 6c69 7479 0a20 2020 2020  ardinality.     
+0000fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fae0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb00: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000fb10: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+0000fb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb30: 2020 2020 696e 6465 785f 6375 722e 6578      index_cur.ex
+0000fb40: 6563 7574 6528 0a20 2020 2020 2020 2020  ecute(.         
+0000fb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb60: 2020 2073 716c 2e53 514c 2822 4352 4541     sql.SQL("CREA
+0000fb70: 5445 2049 4e44 4558 204f 4e20 7b7d 2028  TE INDEX ON {} (
+0000fb80: 7b7d 2922 292e 666f 726d 6174 280a 2020  {})").format(.  
+0000fb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fba0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+0000fbb0: 6c2e 4964 656e 7469 6669 6572 2872 6573  l.Identifier(res
+0000fbc0: 6f75 7263 655f 6964 292c 0a20 2020 2020  ource_id),.     
+0000fbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fbe0: 2020 2020 2020 2020 2020 2073 716c 2e49             sql.I
+0000fbf0: 6465 6e74 6966 6965 7228 6375 7272 5f63  dentifier(curr_c
+0000fc00: 6f6c 292c 0a20 2020 2020 2020 2020 2020  ol),.           
+0000fc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc20: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000fc30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000fc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc50: 2065 7863 6570 7420 7073 7963 6f70 6732   except psycopg2
+0000fc60: 2e45 7272 6f72 2061 7320 653a 0a20 2020  .Error as e:.   
+0000fc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc80: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
+0000fc90: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
+0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcb0: 2027 436f 756c 6420 6e6f 7420 4352 4541   'Could not CREA
+0000fcc0: 5445 2049 4e44 4558 206f 6e20 227b 7d22  TE INDEX on "{}"
+0000fcd0: 3a20 7b7d 272e 666f 726d 6174 2863 7572  : {}'.format(cur
+0000fce0: 725f 636f 6c2c 2065 290a 2020 2020 2020  r_col, e).      
+0000fcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd00: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000fd10: 2020 2020 2020 2020 696e 6465 785f 636f          index_co
+0000fd20: 756e 7420 2b3d 2031 0a0a 2020 2020 2020  unt += 1..      
+0000fd30: 2020 696e 6465 785f 6375 722e 636c 6f73    index_cur.clos
+0000fd40: 6528 290a 2020 2020 2020 2020 7261 775f  e().        raw_
+0000fd50: 636f 6e6e 6563 7469 6f6e 2e63 6f6d 6d69  connection.commi
+0000fd60: 7428 290a 0a20 2020 2020 2020 206c 6f67  t()..        log
+0000fd70: 6765 722e 696e 666f 2822 5661 6375 756d  ger.info("Vacuum
+0000fd80: 2041 6e61 6c79 7a69 6e67 2074 6162 6c65   Analyzing table
+0000fd90: 2074 6f20 6f70 7469 6d69 7a65 2069 6e64   to optimize ind
+0000fda0: 6963 6573 2e2e 2e22 290a 0a20 2020 2020  ices...")..     
+0000fdb0: 2020 2023 2074 6869 7320 6973 206e 6565     # this is nee
+0000fdc0: 6465 6420 746f 2069 7373 7565 2061 2056  ded to issue a V
+0000fdd0: 4143 5555 4d20 414e 414c 595a 450a 2020  ACUUM ANALYZE.  
+0000fde0: 2020 2020 2020 7261 775f 636f 6e6e 6563        raw_connec
+0000fdf0: 7469 6f6e 2e73 6574 5f69 736f 6c61 7469  tion.set_isolati
+0000fe00: 6f6e 5f6c 6576 656c 280a 2020 2020 2020  on_level(.      
+0000fe10: 2020 2020 2020 7073 7963 6f70 6732 2e65        psycopg2.e
+0000fe20: 7874 656e 7369 6f6e 732e 4953 4f4c 4154  xtensions.ISOLAT
+0000fe30: 494f 4e5f 4c45 5645 4c5f 4155 544f 434f  ION_LEVEL_AUTOCO
+0000fe40: 4d4d 4954 0a20 2020 2020 2020 2029 0a20  MMIT.        ). 
+0000fe50: 2020 2020 2020 2061 6e61 6c79 7a65 5f63         analyze_c
+0000fe60: 7572 203d 2072 6177 5f63 6f6e 6e65 6374  ur = raw_connect
+0000fe70: 696f 6e2e 6375 7273 6f72 2829 0a20 2020  ion.cursor().   
+0000fe80: 2020 2020 2061 6e61 6c79 7a65 5f63 7572       analyze_cur
+0000fe90: 2e65 7865 6375 7465 280a 2020 2020 2020  .execute(.      
+0000fea0: 2020 2020 2020 7371 6c2e 5351 4c28 2256        sql.SQL("V
+0000feb0: 4143 5555 4d20 414e 414c 595a 4520 7b7d  ACUUM ANALYZE {}
+0000fec0: 2229 2e66 6f72 6d61 7428 7371 6c2e 4964  ").format(sql.Id
+0000fed0: 656e 7469 6669 6572 2872 6573 6f75 7263  entifier(resourc
+0000fee0: 655f 6964 2929 0a20 2020 2020 2020 2029  e_id)).        )
+0000fef0: 0a20 2020 2020 2020 2061 6e61 6c79 7a65  .        analyze
+0000ff00: 5f63 7572 2e63 6c6f 7365 2829 0a0a 2020  _cur.close()..  
+0000ff10: 2020 2020 2020 696e 6465 785f 656c 6170        index_elap
+0000ff20: 7365 6420 3d20 7469 6d65 2e70 6572 665f  sed = time.perf_
+0000ff30: 636f 756e 7465 7228 2920 2d20 696e 6465  counter() - inde
+0000ff40: 785f 7374 6172 740a 2020 2020 2020 2020  x_start.        
+0000ff50: 6c6f 6767 6572 2e69 6e66 6f28 0a20 2020  logger.info(.   
+0000ff60: 2020 2020 2020 2020 2027 2e2e 2e69 6e64           '...ind
+0000ff70: 6578 696e 672f 7661 6375 756d 2061 6e61  exing/vacuum ana
+0000ff80: 6c79 7369 7320 646f 6e65 2e20 496e 6465  lysis done. Inde
+0000ff90: 7865 6420 7b6e 7d20 636f 6c75 6d6e 2f73  xed {n} column/s
+0000ffa0: 2069 6e20 227b 7265 735f 6964 7d22 2069   in "{res_id}" i
+0000ffb0: 6e20 7b69 6e64 6578 5f65 6c61 7073 6564  n {index_elapsed
+0000ffc0: 7d20 7365 636f 6e64 732e 272e 666f 726d  } seconds.'.form
+0000ffd0: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+0000ffe0: 2020 2020 6e3d 227b 3a2c 7d22 2e66 6f72      n="{:,}".for
+0000fff0: 6d61 7428 696e 6465 785f 636f 756e 7429  mat(index_count)
+00010000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010010: 2020 7265 735f 6964 3d72 6573 6f75 7263    res_id=resourc
+00010020: 655f 6964 2c0a 2020 2020 2020 2020 2020  e_id,.          
+00010030: 2020 2020 2020 696e 6465 785f 656c 6170        index_elap
+00010040: 7365 643d 227b 3a2c 2e32 667d 222e 666f  sed="{:,.2f}".fo
+00010050: 726d 6174 2869 6e64 6578 5f65 6c61 7073  rmat(index_elaps
+00010060: 6564 292c 0a20 2020 2020 2020 2020 2020  ed),.           
+00010070: 2029 0a20 2020 2020 2020 2029 0a0a 2020   ).        )..  
+00010080: 2020 7261 775f 636f 6e6e 6563 7469 6f6e    raw_connection
+00010090: 2e63 6c6f 7365 2829 0a20 2020 2074 6f74  .close().    tot
+000100a0: 616c 5f65 6c61 7073 6564 203d 2074 696d  al_elapsed = tim
+000100b0: 652e 7065 7266 5f63 6f75 6e74 6572 2829  e.perf_counter()
+000100c0: 202d 2074 696d 6572 5f73 7461 7274 0a20   - timer_start. 
+000100d0: 2020 206e 6577 6c69 6e65 5f76 6172 203d     newline_var =
+000100e0: 2022 5c6e 220a 2020 2020 656e 645f 6d73   "\n".    end_ms
+000100f0: 6720 3d20 6622 2222 0a20 2020 2044 4154  g = f""".    DAT
+00010100: 4150 5553 4845 522b 204a 4f42 2044 4f4e  APUSHER+ JOB DON
+00010110: 4521 0a20 2020 20c2 a0c2 a044 6f77 6e6c  E!.    ....Downl
+00010120: 6f61 643a 207b 6665 7463 685f 656c 6170  oad: {fetch_elap
+00010130: 7365 643a 2c2e 3266 7d0a 2020 2020 c2a0  sed:,.2f}.    ..
+00010140: c2a0 416e 616c 7973 6973 3a20 7b61 6e61  ..Analysis: {ana
+00010150: 6c79 7369 735f 656c 6170 7365 643a 2c2e  lysis_elapsed:,.
+00010160: 3266 7d7b 286e 6577 6c69 6e65 5f76 6172  2f}{(newline_var
+00010170: 202b 2066 22c2 a0c2 a050 4949 2053 6372   + f"....PII Scr
+00010180: 6565 6e69 6e67 3a20 7b70 6969 7363 7265  eening: {piiscre
+00010190: 656e 696e 675f 656c 6170 7365 643a 2c2e  ening_elapsed:,.
+000101a0: 3266 7d22 2920 6966 2070 6969 7363 7265  2f}") if piiscre
+000101b0: 656e 696e 675f 656c 6170 7365 6420 3e20  ening_elapsed > 
+000101c0: 3020 656c 7365 2022 227d 0a20 2020 20c2  0 else ""}.    .
+000101d0: a0c2 a043 4f50 5969 6e67 3a20 7b63 6f70  ...COPYing: {cop
+000101e0: 795f 656c 6170 7365 643a 2c2e 3266 7d0a  y_elapsed:,.2f}.
+000101f0: 2020 2020 c2a0 c2a0 4d65 7461 6461 7461      ....Metadata
+00010200: 2075 7064 6174 6573 3a20 7b6d 6574 6164   updates: {metad
+00010210: 6174 615f 656c 6170 7365 643a 2c2e 3266  ata_elapsed:,.2f
+00010220: 7d0a 2020 2020 c2a0 c2a0 496e 6465 7869  }.    ....Indexi
+00010230: 6e67 3a20 7b69 6e64 6578 5f65 6c61 7073  ng: {index_elaps
+00010240: 6564 3a2c 2e32 667d 0a20 2020 2054 4f54  ed:,.2f}.    TOT
+00010250: 414c 2045 4c41 5053 4544 2054 494d 453a  AL ELAPSED TIME:
+00010260: 207b 746f 7461 6c5f 656c 6170 7365 643a   {total_elapsed:
+00010270: 2c2e 3266 7d0a 2020 2020 2222 220a 2020  ,.2f}.    """.  
+00010280: 2020 6c6f 6767 6572 2e69 6e66 6f28 656e    logger.info(en
+00010290: 645f 6d73 6729 0a                        d_msg).
```

### Comparing `datapusher-plus-0.8.0/datapusher/main.py` & `datapusher-plus-0.9.0/datapusher/main.py`

 * *Files identical despite different names*

### Comparing `datapusher-plus-0.8.0/datapusher/settings_local.py` & `datapusher-plus-0.9.0/datapusher/settings_local.py`

 * *Files identical despite different names*

### Comparing `datapusher-plus-0.8.0/datapusher_plus.egg-info/PKG-INFO` & `datapusher-plus-0.9.0/datapusher_plus.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapusher-plus
-Version: 0.8.0
+Version: 0.9.0
 Summary: A standalone web service that parses the contents of a CKAN site's data files (CSV, TSV, Excel and ODS) and pushes them into its DataStore. Accelerated by qsv.
 Home-page: https://github.com/dathere/datapusher-plus
 License: AGPL
 Keywords: ckan csv tsv xls ods excel qsv
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.8
@@ -23,14 +23,16 @@
 [ckanext-xloader](https://github.com/ckan/ckanext-xloader) with the data type guessing of Datapusher.
 
 Datapusher+ is built using [CKAN Service Provider][], with [Messytables] replaced by [qsv].
 
 [TNRIS](https://tnris.org)/[TWDB](https://www.twdb.texas.gov/) provided the use cases that informed and supported the development
 of Datapusher+, specifically, to support a [Resource-first upload workflow](docs/RESOURCE_FIRST_WORKFLOW.md#Resource-first-Upload-Workflow).
 
+For a more detailed overview, see the [CKAN Monthly Live Jan 2023 presentation](https://docs.google.com/presentation/d/e/2PACX-1vT0BfmrrtaEINRGg4UI_m7B02_X6HlFr4yN_DXmgX9goVtgu2DNmZjl-SowL9ZA2ibQhDjScRRJh95q/pub?start=false&loop=false&delayms=3000).
+
 It features:
 
 * **"Bullet-proof", ultra-fast data type inferencing with qsv**
 
   Unlike [Messytables][] which scans only the the first few rows to guess the type of
   a column, [qsv][] scans the entire table so its data type inferences are guaranteed[^1].
 
@@ -123,17 +125,17 @@
     pip install -e .
 
 Install qsv:
 
 [Download the appropriate precompiled binaries](https://github.com/jqnatividad/qsv/releases/latest) for your platform and copy
 it to the appropriate directory, e.g. for Linux:
 
-    wget https://github.com/jqnatividad/qsv/releases/download/0.84.0/qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    unzip qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    rm qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    wget https://github.com/jqnatividad/qsv/releases/download/0.87.0/qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    unzip qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    rm qsv-0.87.0-x86_64-unknown-linux-gnu.zip
     sudo mv qsv* /usr/local/bin
 
 Alternatively, if you want to install qsv from source, follow
 the instructions [here](https://github.com/jqnatividad/qsv#installation). Note that when compiling from source,
 you may want to look into the [Performance Tuning](https://github.com/jqnatividad/qsv#performance-tuning)
 section to squeeze even more performance from qsv.
 
@@ -145,23 +147,23 @@
     qsvdp --update
 
 
 > ℹ️ **NOTE:** qsv is a general purpose CSV data-wrangling toolkit that gets regular updates. To update to the latest version, just run
 qsv with the `--update` option and it will check for the latest version and update as required.
 
 
-Copy `datapusher/config.py` to a new file like `config_local.py` and modify your configuration as required.
+Copy the `datapusher/dot-env.template` to file `datapusher/.env` and modify your configuration as required.
 Make sure to create the `datapusher` PostgreSQL user and the `datapusher_jobs` database (see [DataPusher+ Database Setup](#DataPusher+_Database_Setup)).
 
     cd datapusher
-    cp config.py config_local.py
+    cp dot-env.template .env
     # configure your installation as required
-    nano config_local.py
+    nano .env
 
-    python3 datapusher/main.py datapusher/config_local.py
+    python3 datapusher/main.py datapusher/config.py
 
 By default, DataPusher+ should be running at the following port:
 
     http://localhost:8800/
 
 ## Production deployment
 
@@ -177,41 +179,45 @@
 can be easily adapted to other WSGI servers like Gunicorn. You'll probably need
 to set up Nginx as a reverse proxy in front of it and something like Supervisor
 to keep the process up.
 
 
     # Install requirements for DataPusher+. Be sure to have at least Python 3.8
     sudo apt install python3-venv python3-dev build-essential libxslt1-dev libxml2-dev libffi-dev
-
+     
     cd /usr/lib/ckan
 
     # Create a virtualenv for DataPusher+. DP+ requires at least python 3.8.
     sudo python3.8 -m venv /usr/lib/ckan/dpplus_venv
 
     # Install qsv binary, if required
-    wget https://github.com/jqnatividad/qsv/releases/download/0.84.0/qsv-0.84.0-x86_64-unknown-linux-gnu.zip
-    unzip qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    wget https://github.com/jqnatividad/qsv/releases/download/0.87.0/qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    unzip qsv-0.87.0-x86_64-unknown-linux-gnu.zip
     sudo mv qsv* /usr/local/bin
-    rm qsv-0.84.0-x86_64-unknown-linux-gnu.zip
+    rm qsv-0.87.0-x86_64-unknown-linux-gnu.zip
+    
+    # Set Locales
+    export LC_ALL="en_US.UTF-8"
+    export LC_CTYPE="en_US.UTF-8"
+    sudo dpkg-reconfigure locales
 
     # if qsv is already installed, be sure to update it to the latest release
     sudo qsvdp --update
 
-    # ensure datapusher-plus and uwsgi are installed in the virtual environment
+    # install datapusher-plus in the virtual environment
     . /usr/lib/ckan/dpplus_venv/bin/activate
     pip3 install datapusher-plus
 
-    # generate a settings file and tune it, as well as a uwsgi ini file
+    # create an .env file and tune DP+ settings. Tune the uwsgi.ini file as well
     sudo mkdir -p /etc/ckan/datapusher-plus
-    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/settings.py -o /etc/ckan/datapusher-plus/settings.py
-    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/.env -o /etc/ckan/datapusher-plus/.env
+    sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/datapusher/dot-env.template -o /etc/ckan/datapusher-plus/.env
     sudo curl https://raw.githubusercontent.com/dathere/datapusher-plus/master/deployment/datapusher-uwsgi.ini -o /etc/ckan/datapusher-plus/uwsgi.ini
 
     # Be sure to initialize the database if required. (See Database Setup section below)
-    # Be sure to the .env and settings.py files have the right connect strings!
+    # Be sure to the .env file have the right connect strings!
 
     # Create a user to run the web service (if necessary)
     sudo addgroup www-data
     sudo adduser -G www-data www-data
 
 At this point you can run DataPusher+ with the following command:
 
@@ -262,43 +268,20 @@
 >```
 > ["TAB", "Tab Separated Values File", "text/tab-separated-values", []],
 >```
 
 
 ### DataPusher+ Configuration
 
-The DataPusher+ instance is configured in the `config_local.py`
-file. The location of this file can be adjusted using the `JOB_CONFIG`
-environment variable which should provide an absolute path to a python-formatted
-config file.
-
-Here's a summary of the options available.
-
-| Name | Default | Description |
-| -- | -- | -- |
-| HOST | '0.0.0.0' | Web server host |
-| PORT | 8800 | Web server port |
-| SQLALCHEMY_DATABASE_URI | 'postgresql://datapusher_jobs:<br/>YOURPASSWORD<br/>@localhost/datapusher_jobs' | SQLAlchemy Database URL. See note below about setting up the `datapusher_jobs` db beforehand. |
-| MAX_CONTENT_LENGTH | '1024000' | Max size of files to process in bytes |
-| CHUNK_SIZE | '16384' | Chunk size when processing the data file |
-| DOWNLOAD_TIMEOUT | '30' | Download timeout for requesting the file |
-| SSL_VERIFY | False | Do not validate SSL certificates when requesting the data file (*Warning*: Do not use this setting in production) |
-| TYPES | 'String', 'Float', 'Integer', 'DateTime', 'Date', 'NULL' | These are the types that qsv can infer. |
-| TYPE_MAPPING | {'String': 'text', 'Integer': 'numeric', 'Float': 'numeric', 'DateTime': 'timestamp', 'Date': 'timestamp', 'NULL': 'text'} | Internal qsv type mapping to PostgreSQL types |
-| LOG_FILE | `/tmp/ckan_service.log` | Where to write the logs. Use an empty string to disable |
-| STDERR | `True` | Log to stderr? |
-| QSV_BIN | /usr/local/bin/qsvdp | The location of the qsv binary to use. qsvdp is the DP+ optimized version of qsv. It only has the commands used by DP+, has the self-update engine removed, and is 6x smaller than qsv and 3x smaller than qsvlite. You may also want to look into using `qsvdp_nightly`, for even more performance. |
-| PREVIEW_ROWS | 1000 | The number of rows to insert to the data store. Set to 0 to insert all rows |
-| QSV_DEDUP | `True` | Automatically deduplicate rows? |
-| DEFAULT_EXCEL_SHEET | 0 | The zero-based index of the Excel sheet to export to CSV and insert into the Datastore. Negative values are accepted, i.e. -1 is the last sheet, -2 is 2nd to the last, etc. |
-| AUTO_ALIAS | `True` | Automatically create a resource alias - RESOURCE_NAME-PACKAGE_NAME-OWNER_ORG, that's easier to use in API calls and with the scheming datastore_choices helper |
-| WRITE_ENGINE_URL | | The Postgres connection string to use to write to the Datastore using Postgres COPY. This should be **similar** to your `ckan.datastore.write_url`, except you'll need to use the `datapusher` user |
+The DataPusher+ instance is configured in the `.env` file located in the working directory of DP+
+(`/etc/ckan/datapusher-plus` when running a production deployment. The root of the datapusher-plus
+source directory when running a development installation.)
+
+See [dot-env.template](datapusher/dot-env.template) for a summary of configuration options available.
 
-All of the configuration options above can be also provided as environment
-variables, which can be set by setting key-value pairs in a `.env` file. For variables with boolean values you must use `1` or `0`.
 
 ### DataPusher+ Database Setup
 
 DP+ requires a dedicated PostgreSQL account named `datapusher` to connect to the CKAN Datastore.
 
 To create the `datapusher` user and give it the required privileges to the `datastore_default` database:
```

### Comparing `datapusher-plus-0.8.0/setup.py` & `datapusher-plus-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 setup(
     name='datapusher-plus',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='0.8.0',
+    version='0.9.0',
 
     description="A standalone web service that parses the contents of a CKAN site's data files (CSV, TSV, Excel and ODS) and pushes them into its DataStore. Accelerated by qsv.",
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/dathere/datapusher-plus',
@@ -58,14 +58,15 @@
     install_requires=[
         "python-dotenv",
         'wheel',
         'ckanserviceprovider >= 1.0',
         'requests',
         "psycopg2-binary",
         'datasize',
+        'semver',
         'uwsgi',
     ],
 
     # If there are data files included in your packages that need to be
     # installed, specify them here.  If using Python 2.6 or less, then these
     # have to be included in MANIFEST.in as well.
     package_data={
```

