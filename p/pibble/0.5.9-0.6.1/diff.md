# Comparing `tmp/pibble-0.5.9.tar.gz` & `tmp/pibble-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pibble-0.5.9.tar", last modified: Wed Jun 14 13:30:45 2023, max compression
+gzip compressed data, was "pibble-0.6.1.tar", last modified: Mon Jun 26 01:58:36 2023, max compression
```

## Comparing `pibble-0.5.9.tar` & `pibble-0.6.1.tar`

### file list

```diff
@@ -1,215 +1,215 @@
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-06-14 13:30:45.286949 pibble-0.5.9/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5919 2023-06-14 13:30:45.000000 pibble-0.5.9/README.md
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.274949 pibble-0.5.9/pibble/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9049 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/__main__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/client/apachethrift/
--rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/apachethrift/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/client/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/file/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/file/hdfs.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/file/local.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/client/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/jsonapi.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/client/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/soap.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/webservice/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/client/wrapper.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/api/configuration.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6402 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/exceptions.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/helpers/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/helpers/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/helpers/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/helpers/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/helpers/googlerpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/helpers/store.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/helpers/wrappers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/meta/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/meta/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/meta/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/meta/helpers.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/middleware/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/middleware/apachethrift/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/apachethrift/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/apachethrift/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/apachethrift/screening.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/middleware/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/database/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2841 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/database/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/middleware/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/file/temp.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble/api/middleware/googlerpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/googlerpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/googlerpc/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/googlerpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/googlerpc/metadata.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/middleware/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/middleware/webservice/authentication/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/authentication/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/authentication/basic.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/authentication/bearer.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/authentication/digest.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/authentication/header.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/authentication/oauth.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/limit.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2010 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/origin.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/middleware/webservice/screening.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/protocol/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/api/protocol/__init__.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/api/protocol/apachethrift.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2080 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/server/file/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/server/file/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/server/file/ftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/server/file/sftp.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/googlerpc.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/server/webservice/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/server/webservice/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2296 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/apachethrift.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/awslambda.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    39048 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/server/webservice/drivers/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/drivers/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1600 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/drivers/driver_cherrypy.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2318 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/drivers/driver_gunicorn.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1120 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/drivers/driver_werkzeug.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    15947 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/handler.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/jsonapi.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/orm.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/server/webservice/rpc/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/api/server/webservice/rpc/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     4149 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/rpc/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/rpc/jsonrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/rpc/xmlrpc.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16963 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/soap.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/api/server/webservice/template/
--rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/template/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/template/extensions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-06-14 13:30:43.000000 pibble-0.5.9/pibble/api/server/webservice/template/loader.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/database/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/database/dedupe.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10591 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/database/engine.py
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-06-14 13:30:45.000000 pibble-0.5.9/pibble/database/exceptions.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    28607 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/database/orm.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/database/util.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/ext/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/ext/cms/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/ext/cms/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/database/interface.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/database/menu.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/database/view.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/middleware.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.282949 pibble-0.5.9/pibble/ext/cms/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6660 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/server/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/cms/server/extension.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/dam/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/dam/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/dam/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/dam/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/dam/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/dam/database/files.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/dam/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/dam/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/dam/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/rest/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/rest/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/rest/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/rest/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/rest/database/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/rest/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/rest/server/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16218 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/rest/server/base.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7474 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/rest/server/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/session/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/session/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/session/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/session/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/session/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/session/database/session.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/session/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/session/server/__init__.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5087 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/session/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/user/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/__init__.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/user/client/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/client/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      985 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/client/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/user/database/
--rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/database/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/database/authentication.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/database/base.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/database/notification.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     5865 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/database/permission.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      611 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/database/user.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/ext/user/server/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/server/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    24936 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/ext/user/server/base.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/hooks/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/hooks/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/hooks/aws.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/media/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/media/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/media/thumbnail.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/resources/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/resources/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/resources/retriever.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/scripts/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/scripts/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/scripts/importcheck.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/scripts/templatefiles.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-06-14 13:30:45.000000 pibble-0.5.9/pibble/setup.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/util/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/util/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/util/encryption.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/util/files.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    32914 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/util/helpers.py
--rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/util/imaging.py
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6634 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/util/log.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/util/numeric.py
--rw-------   0 benjamin  (1000) benjamin  (1000)    27432 2023-06-14 13:30:44.000000 pibble-0.5.9/pibble/util/strings.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.286949 pibble-0.5.9/pibble/web/
--rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/web/__init__.py
--rw-------   0 benjamin  (1000) benjamin  (1000)     3220 2023-06-14 13:30:42.000000 pibble-0.5.9/pibble/web/scraper.py
-drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-14 13:30:45.278949 pibble-0.5.9/pibble.egg-info/
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-06-14 13:30:45.000000 pibble-0.5.9/pibble.egg-info/PKG-INFO
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5670 2023-06-14 13:30:45.000000 pibble-0.5.9/pibble.egg-info/SOURCES.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-06-14 13:30:45.000000 pibble-0.5.9/pibble.egg-info/dependency_links.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-06-14 13:30:45.000000 pibble-0.5.9/pibble.egg-info/entry_points.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-06-14 13:30:45.000000 pibble-0.5.9/pibble.egg-info/requires.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-06-14 13:30:45.000000 pibble-0.5.9/pibble.egg-info/top_level.txt
--rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-06-14 13:30:45.286949 pibble-0.5.9/setup.cfg
--rw-------   0 benjamin  (1000) benjamin  (1000)     2732 2023-06-14 13:30:45.000000 pibble-0.5.9/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.916213 pibble-0.6.1/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-06-26 01:58:36.912213 pibble-0.6.1/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5919 2023-06-26 01:58:36.000000 pibble-0.6.1/README.md
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9049 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/__main__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3374 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/client/apachethrift/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6195 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1865 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/apachethrift/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1340 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/client/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    14230 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/file/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9726 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11561 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/file/hdfs.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12782 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/file/local.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    19652 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4132 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/client/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4728 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16837 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2312 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/jsonapi.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/client/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    11386 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4766 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10690 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6689 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/soap.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7333 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/webservice/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      631 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/client/wrapper.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4087 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/configuration.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6402 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/exceptions.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/helpers/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/helpers/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15706 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/helpers/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    20612 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/helpers/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    24691 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/helpers/googlerpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13415 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/helpers/store.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13868 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/helpers/wrappers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/meta/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/meta/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9492 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/meta/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2952 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/meta/helpers.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/middleware/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble/api/middleware/apachethrift/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/apachethrift/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/apachethrift/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1276 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/apachethrift/screening.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      167 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/middleware/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/database/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2841 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/database/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/middleware/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/middleware/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      454 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/middleware/file/temp.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/middleware/googlerpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/googlerpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2976 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/googlerpc/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1176 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/googlerpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1028 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/googlerpc/metadata.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3703 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/middleware/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/middleware/webservice/authentication/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/authentication/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5161 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/authentication/basic.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4338 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/authentication/bearer.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    13472 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/authentication/digest.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2134 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/authentication/header.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    17704 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/authentication/oauth.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1623 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3256 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/limit.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2249 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/origin.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1908 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/middleware/webservice/screening.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/protocol/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/protocol/__init__.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)    19486 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/api/protocol/apachethrift.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2451 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/apachethrift.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2836 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/server/file/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/file/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1419 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/file/ftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15640 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/file/sftp.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     5453 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/googlerpc.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/server/webservice/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2296 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/apachethrift.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7311 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/awslambda.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    39158 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/server/webservice/drivers/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/drivers/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1710 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/drivers/driver_cherrypy.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2318 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/drivers/driver_gunicorn.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1120 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/drivers/driver_werkzeug.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    15947 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/handler.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3164 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/jsonapi.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      969 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/orm.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/server/webservice/rpc/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/rpc/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     4149 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/rpc/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6457 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/rpc/jsonrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    12004 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/rpc/xmlrpc.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16963 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/soap.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/api/server/webservice/template/
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9717 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/template/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9201 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/template/extensions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     9770 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/api/server/webservice/template/loader.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/database/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     7797 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/database/dedupe.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    10968 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/database/engine.py
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)      306 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/database/exceptions.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    28607 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/database/orm.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2694 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/database/util.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/ext/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.908213 pibble-0.6.1/pibble/ext/cms/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/cms/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      721 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      124 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3129 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/database/interface.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1434 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/database/menu.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     2531 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/database/view.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1366 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/middleware.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/cms/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6660 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/server/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3012 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/cms/server/extension.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/dam/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/dam/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/dam/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      229 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/dam/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      117 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/dam/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1110 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/dam/database/files.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/dam/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/dam/server/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      494 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/dam/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/rest/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/rest/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/rest/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/rest/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)       94 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/rest/database/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/rest/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/rest/server/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    16139 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/rest/server/base.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7477 2023-06-26 01:58:35.000000 pibble-0.6.1/pibble/ext/rest/server/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/session/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/session/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/session/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      260 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/session/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      172 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/session/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      776 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/session/database/session.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/session/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/session/server/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5087 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/session/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/user/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/__init__.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/user/client/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/client/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1003 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/client/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/user/database/
+-rw-------   0 benjamin  (1000) benjamin  (1000)      933 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/database/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      860 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/database/authentication.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      103 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/database/base.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      720 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/database/notification.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5902 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/database/permission.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)      614 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/database/user.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/ext/user/server/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/server/__init__.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)    25456 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/ext/user/server/base.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/hooks/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/hooks/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     6037 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/hooks/aws.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/media/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/media/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10388 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/media/thumbnail.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/resources/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/resources/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    10655 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/resources/retriever.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/scripts/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/scripts/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1909 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/scripts/importcheck.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1726 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/scripts/templatefiles.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2732 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/setup.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/util/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/util/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     8357 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/util/encryption.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    16171 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/util/files.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    32914 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/util/helpers.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)      563 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/util/imaging.py
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     7498 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/util/log.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     1701 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/util/numeric.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)    27432 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble/util/strings.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.912213 pibble-0.6.1/pibble/web/
+-rwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/web/__init__.py
+-rw-------   0 benjamin  (1000) benjamin  (1000)     3220 2023-06-26 01:58:34.000000 pibble-0.6.1/pibble/web/scraper.py
+drwxrwxr-x   0 benjamin  (1000) benjamin  (1000)        0 2023-06-26 01:58:36.904213 pibble-0.6.1/pibble.egg-info/
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     6444 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble.egg-info/PKG-INFO
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     5670 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble.egg-info/SOURCES.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        1 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble.egg-info/dependency_links.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       48 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble.egg-info/entry_points.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     1936 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble.egg-info/requires.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)        7 2023-06-26 01:58:36.000000 pibble-0.6.1/pibble.egg-info/top_level.txt
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)       38 2023-06-26 01:58:36.916213 pibble-0.6.1/setup.cfg
+-rw-rw-r--   0 benjamin  (1000) benjamin  (1000)     2732 2023-06-26 01:58:36.000000 pibble-0.6.1/setup.py
```

### Comparing `pibble-0.5.9/PKG-INFO` & `pibble-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.9
+Version: 0.6.1
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.9/README.md` & `pibble-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/__main__.py` & `pibble-0.6.1/pibble/__main__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/base.py` & `pibble-0.6.1/pibble/api/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/apachethrift/__init__.py` & `pibble-0.6.1/pibble/api/client/apachethrift/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/apachethrift/wrapper.py` & `pibble-0.6.1/pibble/api/client/apachethrift/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/base.py` & `pibble-0.6.1/pibble/api/client/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/file/base.py` & `pibble-0.6.1/pibble/api/client/file/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/file/ftp.py` & `pibble-0.6.1/pibble/api/client/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/file/hdfs.py` & `pibble-0.6.1/pibble/api/client/file/hdfs.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/file/local.py` & `pibble-0.6.1/pibble/api/client/file/local.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/file/sftp.py` & `pibble-0.6.1/pibble/api/client/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/googlerpc.py` & `pibble-0.6.1/pibble/api/client/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/webservice/apachethrift.py` & `pibble-0.6.1/pibble/api/client/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/webservice/base.py` & `pibble-0.6.1/pibble/api/client/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/webservice/jsonapi.py` & `pibble-0.6.1/pibble/api/client/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/webservice/rpc/base.py` & `pibble-0.6.1/pibble/api/client/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/webservice/rpc/jsonrpc.py` & `pibble-0.6.1/pibble/api/client/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/webservice/rpc/xmlrpc.py` & `pibble-0.6.1/pibble/api/client/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/webservice/soap.py` & `pibble-0.6.1/pibble/api/client/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/webservice/wrapper.py` & `pibble-0.6.1/pibble/api/client/webservice/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/client/wrapper.py` & `pibble-0.6.1/pibble/api/client/wrapper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/configuration.py` & `pibble-0.6.1/pibble/api/configuration.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/exceptions.py` & `pibble-0.6.1/pibble/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/helpers/apachethrift.py` & `pibble-0.6.1/pibble/api/helpers/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/helpers/authentication.py` & `pibble-0.6.1/pibble/api/helpers/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/helpers/googlerpc.py` & `pibble-0.6.1/pibble/api/helpers/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/helpers/store.py` & `pibble-0.6.1/pibble/api/helpers/store.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/helpers/wrappers.py` & `pibble-0.6.1/pibble/api/helpers/wrappers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/meta/base.py` & `pibble-0.6.1/pibble/api/meta/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/meta/helpers.py` & `pibble-0.6.1/pibble/api/meta/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/apachethrift/base.py` & `pibble-0.6.1/pibble/api/middleware/apachethrift/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/apachethrift/screening.py` & `pibble-0.6.1/pibble/api/middleware/apachethrift/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/database/orm.py` & `pibble-0.6.1/pibble/api/middleware/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/googlerpc/authentication.py` & `pibble-0.6.1/pibble/api/middleware/googlerpc/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/googlerpc/base.py` & `pibble-0.6.1/pibble/api/middleware/googlerpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/googlerpc/metadata.py` & `pibble-0.6.1/pibble/api/middleware/googlerpc/metadata.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/screening.py` & `pibble-0.6.1/pibble/api/middleware/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/authentication/basic.py` & `pibble-0.6.1/pibble/api/middleware/webservice/authentication/basic.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/authentication/bearer.py` & `pibble-0.6.1/pibble/api/middleware/webservice/authentication/bearer.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/authentication/digest.py` & `pibble-0.6.1/pibble/api/middleware/webservice/authentication/digest.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/authentication/header.py` & `pibble-0.6.1/pibble/api/middleware/webservice/authentication/header.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/authentication/oauth.py` & `pibble-0.6.1/pibble/api/middleware/webservice/authentication/oauth.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/base.py` & `pibble-0.6.1/pibble/api/middleware/webservice/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/limit.py` & `pibble-0.6.1/pibble/api/middleware/webservice/limit.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/origin.py` & `pibble-0.6.1/pibble/api/middleware/webservice/origin.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pibble.api.helpers.wrappers import (
     RequestWrapper,
     ResponseWrapper,
 )
 
 from pibble.api.exceptions import AuthenticationError
 from pibble.api.middleware.webservice.base import WebServiceAPIMiddlewareBase
+from pibble.util.log import logger
 
 
 class CrossOriginWebServiceAPIMiddleware(WebServiceAPIMiddlewareBase):
     """
     Extends the base WebServiceAPIMiddlewareBase to read origins from requests
     and send necessary headers to permit or disallow requests.
     """
@@ -35,19 +36,22 @@
         ] = None,
     ) -> None:
         if isinstance(request, WebobRequest) or isinstance(request, RequestWrapper):
             origin: Optional[str] = None
             if "Origin" in request.headers:
                 origin = request.headers["Origin"]
             elif "Referer" in request.headers:
-                origin = urlparse(request.headers["Referer"]).netloc
+                origin = request.headers["Referer"]
             elif not self.allow_missing:
                 raise AuthenticationError(
                     "Your request does not indicate where it came from, and network policy rejects unknown origins."
                 )
             if origin is not None:
+                if "/" in origin:
+                    origin = urlparse(origin).netloc
                 for allowed_origin in self.origins:
                     if re.match(allowed_origin, origin):
                         return
+                logger.warning(f"Request received from {origin}, but this is not in the list of allowed origins. Screening request.")
                 raise AuthenticationError(
                     "Your request was screened by network policy."
                 )
```

### Comparing `pibble-0.5.9/pibble/api/middleware/webservice/screening.py` & `pibble-0.6.1/pibble/api/middleware/webservice/screening.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/protocol/apachethrift.py` & `pibble-0.6.1/pibble/api/protocol/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/apachethrift.py` & `pibble-0.6.1/pibble/api/server/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/base.py` & `pibble-0.6.1/pibble/api/server/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from __future__ import annotations
 
+from typing import Optional, Dict, Any
+
 from multiprocessing import Process
 from pibble.api.base import APIBase
 from pibble.util.helpers import Pause
 from pibble.util.log import logger
 
 
 class APIServerProcess(Process):
     """
     A small class that will run the server process in the background.
     """
 
-    def __init__(self, server: APIServerBase) -> None:
+    def __init__(self, server: APIServerBase, configuration: Optional[Dict[str, Any]] = None) -> None:
         super(APIServerProcess, self).__init__()
         self.server = server
+        self.configuration = configuration
 
     def run(self) -> None:
+        if self.configuration is not None:
+            self.server.configure(**self.configuration)
         try:
             self.server.serve()
         except Exception as ex:
             logger.critical("{0}(): {1}".format(type(ex).__name__, str(ex)))
             raise
 
 
@@ -43,14 +48,29 @@
 
     def running(self) -> bool:
         """
         Determines if the server is currently running (when used asynchronously.)
         """
         return hasattr(self, "_process") and self._process.is_alive()
 
+    def configure_start(self, **configuration: Any) -> None:
+        """
+        Starts the server, configuring itself after.
+        """
+        if hasattr(self, "_process"):
+            if self._process.is_alive():
+                logger.warning(
+                    "start() was called while process is still alive. Ignoring."
+                )
+                return
+            del self._process
+        self._process = APIServerProcess(self, configuration)
+        self._process.start()
+        Pause.milliseconds(250)
+
     def start(self) -> None:
         """
         Starts the server, which will serve asynchronously.
         """
         if hasattr(self, "_process"):
             if self._process.is_alive():
                 logger.warning(
```

### Comparing `pibble-0.5.9/pibble/api/server/file/ftp.py` & `pibble-0.6.1/pibble/api/server/file/ftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/file/sftp.py` & `pibble-0.6.1/pibble/api/server/file/sftp.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/googlerpc.py` & `pibble-0.6.1/pibble/api/server/googlerpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/apachethrift.py` & `pibble-0.6.1/pibble/api/server/webservice/apachethrift.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/awslambda.py` & `pibble-0.6.1/pibble/api/server/webservice/awslambda.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/base.py` & `pibble-0.6.1/pibble/api/server/webservice/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,19 @@
     }
 
     class_handlers: List[WebServiceAPIHandlerRegistry]
 
     def __init__(self) -> None:
         super(WebServiceAPIServerBase, self).__init__()
         self.class_handlers = []
+    
+    def on_configure(self) -> None:
+        """
+        On configuration, register handlers.
+        """
         self.register_all_handlers()
 
     def format_exception(
         self,
         exception: Exception,
         request: Union[Request, RequestWrapper],
         response: Union[Response, ResponseWrapper],
```

### Comparing `pibble-0.5.9/pibble/api/server/webservice/drivers/driver_cherrypy.py` & `pibble-0.6.1/pibble/api/server/webservice/drivers/driver_werkzeug.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,34 @@
 from __future__ import annotations
 
-import cherrypy
+import ssl
 from typing import Optional, TYPE_CHECKING
-from multiprocessing import cpu_count
+from werkzeug.serving import run_simple
 from pibble.util.log import logger
 
 if TYPE_CHECKING:
     from pibble.api.server.webservice.base import WebServiceAPIServerBase
 
 
-def run_cherrypy(
+def run_werkzeug(
     application: WebServiceAPIServerBase,
     host: str,
     port: int,
     secure: bool = False,
     cert: Optional[str] = None,
     key: Optional[str] = None,
     workers: Optional[int] = None,
 ) -> None:
     """
-    Runs the cherrypy engine synchronously.
+    Runs the werkzeug HTTP server synchronously.
     """
-    cherrypy.tree.graft(application.wsgi(), "/")
-    cherrypy.server.unsubscribe()
-    cherrypy.config.update(
-        {"global": {"environment": "production"}}
-    )  # Disable reloading
-
-    server = cherrypy._cpserver.Server()
-    server.socket_host = host
-    server.socket_port = port
-    server.thread_pool = workers if workers is not None else cpu_count() * 2 - 1
-
+    ssl_context = None
     if secure and cert is not None and key is not None:
-        server.ssl_model = "pyopenssl"
-        server.ssl_certificate = cert
-        server.ssl_private_key = key
         logger.info(
             f"Loading SSL certificate chain from keyfile {key:s}, certfile {cert:s}"
         )
+        ssl_context = ssl.SSLContext(ssl.PROTOCOL_SSLv23)
     elif secure:
         logger.warning(
             "No SSL keyfile/certfile specific, but SSL enabled. If this server is being proxied through another service that provides SSL context this is okay, otherwise connections will fail."
         )
-
-    server.subscribe()
-    cherrypy.engine.subscribe("exit", lambda: application.destroy())
-    cherrypy.engine.start()
-    cherrypy.engine.block()
+    run_simple(host, port, application.wsgi(), ssl_context=ssl_context)
```

### Comparing `pibble-0.5.9/pibble/api/server/webservice/drivers/driver_gunicorn.py` & `pibble-0.6.1/pibble/api/server/webservice/drivers/driver_gunicorn.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/handler.py` & `pibble-0.6.1/pibble/api/server/webservice/handler.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/jsonapi.py` & `pibble-0.6.1/pibble/api/server/webservice/jsonapi.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/orm.py` & `pibble-0.6.1/pibble/api/server/webservice/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/rpc/base.py` & `pibble-0.6.1/pibble/api/server/webservice/rpc/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/rpc/jsonrpc.py` & `pibble-0.6.1/pibble/api/server/webservice/rpc/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/rpc/xmlrpc.py` & `pibble-0.6.1/pibble/api/server/webservice/rpc/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/soap.py` & `pibble-0.6.1/pibble/api/server/webservice/soap.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/template/__init__.py` & `pibble-0.6.1/pibble/api/server/webservice/template/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/template/extensions.py` & `pibble-0.6.1/pibble/api/server/webservice/template/extensions.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/api/server/webservice/template/loader.py` & `pibble-0.6.1/pibble/api/server/webservice/template/loader.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/database/dedupe.py` & `pibble-0.6.1/pibble/database/dedupe.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/database/engine.py` & `pibble-0.6.1/pibble/database/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,21 @@
         self.engines = {}
         if "database" in self.connection_params:
             self._default_database = str(self.connection_params.pop("database"))
             if self.connection_params["drivername"].startswith(
                 "sqlite"
             ) and self._default_database.startswith("~"):
                 self._default_database = os.path.expanduser(self._default_database)
+                database_dir = os.path.dirname(self._default_database)
+                if not os.path.exists(database_dir):
+                    try:
+                        os.makedirs(database_dir)
+                    except:
+                        logger.error(f"Database directory {database_dir} does not exist, and it could not be created.")
+                        raise
         else:
             self._default_database = "default"
         self._create_engine(self._default_database)
 
     def __iter__(self) -> Self:
         self._iterkeys = list(self.engines.keys())
         self._iterindex = 0
```

### Comparing `pibble-0.5.9/pibble/database/orm.py` & `pibble-0.6.1/pibble/database/orm.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/database/util.py` & `pibble-0.6.1/pibble/database/util.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/cms/database/__init__.py` & `pibble-0.6.1/pibble/ext/cms/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/cms/database/interface.py` & `pibble-0.6.1/pibble/ext/cms/database/interface.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/cms/database/menu.py` & `pibble-0.6.1/pibble/ext/cms/database/menu.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/cms/database/view.py` & `pibble-0.6.1/pibble/ext/cms/database/view.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/cms/middleware.py` & `pibble-0.6.1/pibble/ext/cms/middleware.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/cms/server/base.py` & `pibble-0.6.1/pibble/ext/cms/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/cms/server/extension.py` & `pibble-0.6.1/pibble/ext/cms/server/extension.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/dam/database/files.py` & `pibble-0.6.1/pibble/ext/dam/database/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/rest/server/base.py` & `pibble-0.6.1/pibble/ext/rest/server/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,23 +142,19 @@
                 )
             else:
                 query = query.filter(apply_column(column))
 
             return query
 
         if ilikes:
+            conditions = []
             for ilike_string in ilikes:
                 column, _, value = ilike_string.partition(":")
-                query = apply_filters(
-                    query,
-                    obj,
-                    column,
-                    value,
-                    lambda column, value: column.ilike("%{:s}%".format(value.lower())),
-                )
+                conditions.append(getattr(obj, column).ilike("%{:s}%".format(value.lower())))
+            query = query.filter(or_(*conditions))
 
         if filters:
             for filter_string in filters:
                 column, _, value = filter_string.partition(":")
                 query = apply_filters(
                     query, obj, column, value, lambda column, value: column == value
                 )
```

### Comparing `pibble-0.5.9/pibble/ext/rest/server/user.py` & `pibble-0.6.1/pibble/ext/rest/server/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
                     raise PermissionError("Invalid or no credentials supplied.")
                 permission = self.check_user_permission(
                     request.token.user, handler_classname, action, **kwargs
                 )
                 if not permission:
                     raise PermissionError(
                         "User {0} is not authorized to {1} on {2}.".format(
-                            request.token.user.email, action, handler_classname
+                            request.token.user.username, action, handler_classname
                         )
                     )
 
             scope_user_fields = scope.get("user", {})
             for field in scope_user_fields:
                 kwargs[scope_user_fields[field]] = getattr(
                     request.token.user, field, None
```

### Comparing `pibble-0.5.9/pibble/ext/session/database/session.py` & `pibble-0.6.1/pibble/ext/session/database/session.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/session/server/base.py` & `pibble-0.6.1/pibble/ext/session/server/base.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/user/database/__init__.py` & `pibble-0.6.1/pibble/ext/user/database/__init__.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/user/database/authentication.py` & `pibble-0.6.1/pibble/ext/user/database/authentication.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/user/database/notification.py` & `pibble-0.6.1/pibble/ext/user/database/notification.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/ext/user/database/permission.py` & `pibble-0.6.1/pibble/ext/user/database/permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
       @handlers.secured("MySingularlyOwnedObject", "update")
       @handlers.path(r"^/singular/(?P<name>[a-zA-Z0-9_\-]+)$")
       def modifySingularObject(self, request, response, name = None):
         # this will only be allowed if the associated permission exists, so feel free
         # to just have this handler modify the object.
     """
 
-    __tablename__ = "pibble_user_permission"
+    __tablename__ = "pibble_permission"
 
     id = Column(Integer, autoincrement=True, primary_key=True)
     object_name = Column(String, nullable=False)
 
     action = Column(
         Enum("create", "read", "update", "delete", name="action_enum"),
         default="read",
@@ -81,22 +81,22 @@
     inherited_scope_source_attribute = Column(String)
     inherited_scope_target_attribute = Column(String)
     inherited_scope_action = Column(String)
     inherited_scope_secondary_action = Column(String)
 
 
 class PermissionGroup(UserExtensionObjectBase):
-    __tablename__ = "permission_group"
+    __tablename__ = "pibble_permission_group"
 
     id = Column(Integer, autoincrement=True, primary_key=True)
     label = Column(String)
 
 
 class PermissionGroupPermission(UserExtensionObjectBase):
-    __tablename__ = "permission_group_permission"
+    __tablename__ = "pibble_permission_group_permission"
 
     group_id = Column(
         Integer,
         PermissionGroup.ForeignKey("id", ondelete="CASCADE", onupdate="CASCADE"),
         primary_key=True,
     )
     permission_id = Column(
@@ -106,15 +106,15 @@
     )
 
     permission = Permission.Relationship()
     group = PermissionGroup.Relationship()
 
 
 class UserPermission(UserExtensionObjectBase):
-    __tablename__ = "user_permission"
+    __tablename__ = "pibble_user_permission"
 
     permission_id = Column(
         Integer,
         Permission.ForeignKey("id", ondelete="CASCADE", onupdate="CASCADE"),
         primary_key=True,
     )
     user_id = Column(
@@ -126,26 +126,26 @@
     permission = Permission.Relationship()
 
 
 User.Relate(UserPermission, name="permissions", backref="user")
 
 
 class GlobalPermission(UserExtensionObjectBase):
-    __tablename__ = "global_permission"
+    __tablename__ = "pibble_global_permission"
 
     permission_id = Column(
         Integer,
         Permission.ForeignKey("id", ondelete="CASCADE", onupdate="CASCADE"),
         primary_key=True,
     )
     permission = Permission.Relationship()
 
 
 class UserPermissionGroup(UserExtensionObjectBase):
-    __tablename__ = "user_permission_group"
+    __tablename__ = "pibble_user_permission_group"
 
     group_id = Column(
         Integer,
         PermissionGroup.ForeignKey("id", ondelete="CASCADE", onupdate="CASCADE"),
         primary_key=True,
     )
     user_id = Column(
@@ -157,15 +157,15 @@
     group = PermissionGroup.Relationship()
 
 
 User.Relate(UserPermissionGroup, name="permission_groups", backref="user")
 
 
 class GlobalPermissionGroup(UserExtensionObjectBase):
-    __tablename__ = "global_permission_group"
+    __tablename__ = "pibble_global_permission_group"
 
     group_id = Column(
         Integer,
         PermissionGroup.ForeignKey("id", ondelete="CASCADE", onupdate="CASCADE"),
         primary_key=True,
     )
     group = PermissionGroup.Relationship()
```

### Comparing `pibble-0.5.9/pibble/ext/user/database/user.py` & `pibble-0.6.1/pibble/ext/user/database/user.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class User(UserExtensionObjectBase):
     __tablename__ = "pibble_user"
 
     id = Column(Integer, autoincrement=True, primary_key=True)
 
-    email = Column(String, nullable=False, unique=True)
+    username = Column(String, nullable=False, unique=True)
     verified = Column(Boolean, default=False)
 
     superuser = Column(Boolean, default=False)
 
     first_name = Column(String)
     last_name = Column(String)
     password = Column(String)
```

### Comparing `pibble-0.5.9/pibble/ext/user/server/base.py` & `pibble-0.6.1/pibble/ext/user/server/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         if user.superuser:
             return True
 
         object_name = getattr(subject, "__name__", str(subject))
 
         logger.debug(
             "Checking permissions on user {0} for object {1}, action {2}, secondary action {3}".format(
-                user.email, object_name, action, secondary_action
+                user.username, object_name, action, secondary_action
             )
         )
 
         for permission in self.find_permissions_by_user(
             user, object_name, action=action, secondary_action=secondary_action
         ):
             if self.check_permission(user, permission, **kwargs):
@@ -285,15 +285,15 @@
             object_name,
             action,
             secondary_action=secondary_action,
             **kwargs,
         ):
             raise PermissionError(
                 "User {0} is not authorized to {1} on {2}.".format(
-                    request.token.user.email,
+                    request.token.user.username,
                     action
                     if not secondary_action
                     else "{0} - {1}".format(action, secondary_action),
                     object_name,
                 )
             )
 
@@ -363,88 +363,94 @@
                 **{inherited_scope_target_attribute: inherited_scope_passed_value},
             )
 
     def migrate_permissions(self) -> None:
         with self.orm.session() as session:
             for permission in self.configuration["user.permissions"]:
                 permission = {**permission}
+                actions = permission.pop("action")
+                if not isinstance(actions, list):
+                    actions = [actions]
                 is_global = permission.pop("global", False)
                 group = permission.pop("group", None)
-                existing = (
-                    session.query(self.orm.Permission)
-                    .filter_by(**permission)
-                    .one_or_none()
-                )
-                if not existing:
-                    existing = self.orm.Permission(**permission)
-                    session.add(existing)
-                    session.commit()
-                if is_global:
-                    existing_global = (
-                        session.query(self.orm.GlobalPermission)
-                        .filter(self.orm.GlobalPermission.permission_id == existing.id)
-                        .one_or_none()
-                    )
-                    if not existing_global:
-                        session.add(
-                            self.orm.GlobalPermission(permission_id=existing.id)
-                        )
-                if group:
-                    existing_group = (
-                        session.query(self.orm.PermissionGroup)
-                        .filter(self.orm.PermissionGroup.label == group)
+
+                for action in actions:
+                    existing = (
+                        session.query(self.orm.Permission)
+                        .filter(self.orm.Permission.action == action)
+                        .filter_by(**permission)
                         .one_or_none()
                     )
-                    if not existing_group:
-                        existing_group = self.orm.PermissionGroup(label=group)
-                        session.add(existing_group)
+                    if not existing:
+                        existing = self.orm.Permission(action=action, **permission)
+                        session.add(existing)
                         session.commit()
-                    existing_group_permission = (
-                        session.query(self.orm.PermissionGroupPermission)
-                        .filter(
-                            self.orm.PermissionGroupPermission.permission_id
-                            == existing.id
+                    if is_global:
+                        existing_global = (
+                            session.query(self.orm.GlobalPermission)
+                            .filter(self.orm.GlobalPermission.permission_id == existing.id)
+                            .one_or_none()
                         )
-                        .filter(
-                            self.orm.PermissionGroupPermission.group_id
-                            == existing_group.id
+                        if not existing_global:
+                            session.add(
+                                self.orm.GlobalPermission(permission_id=existing.id)
+                            )
+                    if group:
+                        existing_group = (
+                            session.query(self.orm.PermissionGroup)
+                            .filter(self.orm.PermissionGroup.label == group)
+                            .one_or_none()
                         )
-                        .one_or_none()
-                    )
-                    if not existing_group_permission:
-                        session.add(
-                            self.orm.PermissionGroupPermission(
-                                permission_id=existing.id, group_id=existing_group.id
+                        if not existing_group:
+                            existing_group = self.orm.PermissionGroup(label=group)
+                            session.add(existing_group)
+                            session.commit()
+                        existing_group_permission = (
+                            session.query(self.orm.PermissionGroupPermission)
+                            .filter(
+                                self.orm.PermissionGroupPermission.permission_id
+                                == existing.id
                             )
+                            .filter(
+                                self.orm.PermissionGroupPermission.group_id
+                                == existing_group.id
+                            )
+                            .one_or_none()
                         )
+                        if not existing_group_permission:
+                            session.add(
+                                self.orm.PermissionGroupPermission(
+                                    permission_id=existing.id, group_id=existing_group.id
+                                )
+                            )
             session.commit()
 
     def migrate_users(self) -> None:
         with self.orm.session() as session:
             for user in self.configuration["user.users"]:
                 user = {**user}
-                email = user.pop("email")
+                username = user.pop("username")
                 password = user.pop("password", None)
                 permissions = user.pop("permissions", [])
                 groups = user.pop("groups", [])
 
                 existing = (
                     session.query(self.orm.User)
-                    .filter(func.lower(self.orm.User.email) == email.lower())
+                    .filter(func.lower(self.orm.User.username) == username.lower())
                     .one_or_none()
                 )
 
                 if existing:
                     for key in user:
                         if key:
                             setattr(existing, key, user[key])
                 else:
                     if password:
                         password = Password.hash(password)
-                    existing = self.orm.User(password=password, email=email, **user)
+                    existing = self.orm.User(password=password, username=username, **user)
                     session.add(existing)
 
                 for permission in permissions:
                     pass
 
                 for group in groups:
                     group = (
@@ -494,38 +500,38 @@
             raise AuthenticationError("Not logged in.")
 
     def login(self, request: Request, response: Response) -> AuthenticationToken:
         """
         The main login handler.
         """
         if hasattr(request, "parsed") and request.parsed:
-            if "email" not in request.parsed or "password" not in request.parsed:
-                raise AuthenticationError("Missing email or password.")
+            if "username" not in request.parsed or "password" not in request.parsed:
+                raise AuthenticationError("Missing username or password.")
             else:
-                email = request.parsed["email"]
+                username = request.parsed["username"]
                 password = request.parsed["password"]
-        elif "email" not in request.POST or "password" not in request.POST:
-            raise AuthenticationError("Missing email or password.")
+        elif "username" not in request.POST or "password" not in request.POST:
+            raise AuthenticationError("Missing username or password.")
         else:
-            email = request.POST["email"]
+            username = request.POST["username"]
             password = request.POST["password"]
 
         user = (
             self.database.query(self.orm.User)
-            .filter(func.lower(self.orm.User.email) == email.lower())
+            .filter(func.lower(self.orm.User.username) == username.lower())
             .one_or_none()
         )
         if not user:
-            raise AuthenticationError("Incorrect email or password.")
+            raise AuthenticationError("Incorrect username or password.")
         if not user.password:
             raise AuthenticationError(
-                "Account for user '{0}' not activated.".format(email)
+                "Account for user '{0}' not activated.".format(username)
             )
         if not Password.verify(user.password, password):
-            raise AuthenticationError("Incorrect email or password.")
+            raise AuthenticationError("Incorrect username or password.")
 
         token = self.orm.AuthenticationToken(
             access_token=get_uuid(),
             refresh_token=get_uuid(),
             token_type=self.token_type,
             user_id=user.id,
         )
@@ -543,15 +549,15 @@
         """
         user = (
             self.database.query(self.orm.User)
             .filter(self.orm.User.id == 0)
             .one_or_none()
         )
         if not user:
-            user = self.orm.User(id=0, email="noauth", superuser=True)
+            user = self.orm.User(id=0, username="noauth", superuser=True)
             self.database.add(user)
             self.database.commit()
 
         token = self.orm.AuthenticationToken(
             access_token=get_uuid(),
             refresh_token=get_uuid(),
             token_type=self.token_type,
```

### Comparing `pibble-0.5.9/pibble/hooks/aws.py` & `pibble-0.6.1/pibble/hooks/aws.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/media/thumbnail.py` & `pibble-0.6.1/pibble/media/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/resources/retriever.py` & `pibble-0.6.1/pibble/resources/retriever.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/scripts/importcheck.py` & `pibble-0.6.1/pibble/scripts/importcheck.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/scripts/templatefiles.py` & `pibble-0.6.1/pibble/scripts/templatefiles.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/setup.py` & `pibble-0.6.1/pibble/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
-version_minor = "5"
-version_patch = "9"
+version_minor = "6"
+version_patch = "1"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

### Comparing `pibble-0.5.9/pibble/util/encryption.py` & `pibble-0.6.1/pibble/util/encryption.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/util/files.py` & `pibble-0.6.1/pibble/util/files.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/util/helpers.py` & `pibble-0.6.1/pibble/util/helpers.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/util/imaging.py` & `pibble-0.6.1/pibble/util/imaging.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/util/log.py` & `pibble-0.6.1/pibble/util/log.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Utilities for logging - the global logger, and contexts for debugging.
 """
-
+import os
 import sys
 import http.client
 import socket
 
 from logging import (
     Handler,
     StreamHandler,
-    FileHandler,
     Formatter,
     LogRecord,
     Logger,
     getLogger,
     DEBUG,
 )
 from typing import Any, List
-from logging.handlers import SysLogHandler
+from logging.handlers import (
+    SysLogHandler,
+    RotatingFileHandler
+)
 from termcolor import colored
 
 from pibble.api.configuration import APIConfiguration
 
 __all__ = [
     "logger",
     "ColoredLoggingFormatter",
@@ -170,15 +172,34 @@
             if isinstance(stream, str):
                 self.handler = StreamHandler(
                     sys.stdout if stream == "stdout" else sys.stderr
                 )
             else:
                 self.handler = StreamHandler(stream)
         elif handler_class == "file":
-            self.handler = FileHandler(configuration[f"{prefix}file"])
+            file_path = configuration.get(f"{prefix}file", None)
+            if file_path is None:
+                raise ValueError(f"Can't use 'file' handler without file - set {prefix}file")
+            if file_path.startswith("~"):
+                file_path = os.path.expanduser(file_path)
+            file_path = os.path.abspath(file_path)
+            backup_count = configuration.get(f"{prefix}backups", 2)
+            max_bytes = configuration.get(f"{prefix}maxbytes", 5*1024*1024)
+            if not isinstance(backup_count, int):
+                backup_count = 2
+            if not isinstance(max_bytes, int):
+                max_bytes = 5*1024*1024
+            self.handler = RotatingFileHandler(
+                file_path,
+                mode='a',
+                maxBytes=max_bytes,
+                backupCount=backup_count,
+                encoding=None,
+                delay=False
+            )
         elif handler_class == "syslog":
             self.handler = SysLogHandler(
                 address=(
                     configuration["host"],
                     int(configuration["port"]),
                 ),
                 facility=configuration["facility"],
```

### Comparing `pibble-0.5.9/pibble/util/numeric.py` & `pibble-0.6.1/pibble/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/util/strings.py` & `pibble-0.6.1/pibble/util/strings.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble/web/scraper.py` & `pibble-0.6.1/pibble/web/scraper.py`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble.egg-info/PKG-INFO` & `pibble-0.6.1/pibble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pibble
-Version: 0.5.9
+Version: 0.6.1
 Summary: A framework for developing webapps quickly and easily using Python
 Author: Benjamin Paine
 Author-email: painebenjamin@gmail.com
 License: gpl-3.0
 Description-Content-Type: text/markdown
 Provides-Extra: mysql
 Provides-Extra: postgresql
```

### Comparing `pibble-0.5.9/pibble.egg-info/SOURCES.txt` & `pibble-0.6.1/pibble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/pibble.egg-info/requires.txt` & `pibble-0.6.1/pibble.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pibble-0.5.9/setup.py` & `pibble-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 package_name = "pibble"
 version_major = "0"
-version_minor = "5"
-version_patch = "9"
+version_minor = "6"
+version_patch = "1"
 
 install_requires = [
     "bcrypt>=4.0,<4.1",
     "boto3>=1.26,<2.0",
     "chardet>=5.1,<5.2",
     "click>=8.0,<9.0",
     "configparser>=5.3,<5.4",
```

