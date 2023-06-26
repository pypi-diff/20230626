# Comparing `tmp/MotorDeCalidad-1.9.8.tar.gz` & `tmp/MotorDeCalidad-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MotorDeCalidad-1.9.8.tar", last modified: Fri Mar 10 20:41:36 2023, max compression
+gzip compressed data, was "MotorDeCalidad-1.9.9.tar", last modified: Fri Mar 10 20:57:37 2023, max compression
```

## Comparing `MotorDeCalidad-1.9.8.tar` & `MotorDeCalidad-1.9.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:41:36.146036 MotorDeCalidad-1.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:41:36.142036 MotorDeCalidad-1.9.8/MotorDeCalidad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-03-10 20:41:36.000000 MotorDeCalidad-1.9.8/MotorDeCalidad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-10 20:41:36.000000 MotorDeCalidad-1.9.8/MotorDeCalidad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:41:36.000000 MotorDeCalidad-1.9.8/MotorDeCalidad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:41:35.000000 MotorDeCalidad-1.9.8/MotorDeCalidad.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-10 20:41:36.000000 MotorDeCalidad-1.9.8/MotorDeCalidad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-03-10 20:41:36.146036 MotorDeCalidad-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-10 20:41:19.000000 MotorDeCalidad-1.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:41:36.146036 MotorDeCalidad-1.9.8/motordecalidad/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 20:41:19.000000 MotorDeCalidad-1.9.8/motordecalidad/_init_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-03-10 20:41:19.000000 MotorDeCalidad-1.9.8/motordecalidad/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    29494 2023-03-10 20:41:19.000000 MotorDeCalidad-1.9.8/motordecalidad/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-03-10 20:41:19.000000 MotorDeCalidad-1.9.8/motordecalidad/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-10 20:41:19.000000 MotorDeCalidad-1.9.8/motordecalidad/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 20:41:36.146036 MotorDeCalidad-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-10 20:41:19.000000 MotorDeCalidad-1.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:57:37.674375 MotorDeCalidad-1.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:57:37.674375 MotorDeCalidad-1.9.9/MotorDeCalidad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-03-10 20:57:37.000000 MotorDeCalidad-1.9.9/MotorDeCalidad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-10 20:57:37.000000 MotorDeCalidad-1.9.9/MotorDeCalidad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:57:37.000000 MotorDeCalidad-1.9.9/MotorDeCalidad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 20:57:37.000000 MotorDeCalidad-1.9.9/MotorDeCalidad.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-10 20:57:37.000000 MotorDeCalidad-1.9.9/MotorDeCalidad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 2023-03-10 20:57:37.674375 MotorDeCalidad-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-03-10 20:57:19.000000 MotorDeCalidad-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 20:57:37.674375 MotorDeCalidad-1.9.9/motordecalidad/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 20:57:19.000000 MotorDeCalidad-1.9.9/motordecalidad/_init_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-03-10 20:57:19.000000 MotorDeCalidad-1.9.9/motordecalidad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29494 2023-03-10 20:57:19.000000 MotorDeCalidad-1.9.9/motordecalidad/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19346 2023-03-10 20:57:19.000000 MotorDeCalidad-1.9.9/motordecalidad/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-10 20:57:19.000000 MotorDeCalidad-1.9.9/motordecalidad/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 20:57:37.674375 MotorDeCalidad-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-10 20:57:19.000000 MotorDeCalidad-1.9.9/setup.py
```

### Comparing `MotorDeCalidad-1.9.8/MotorDeCalidad.egg-info/PKG-INFO` & `MotorDeCalidad-1.9.9/MotorDeCalidad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MotorDeCalidad
-Version: 1.9.8
+Version: 1.9.9
 Summary: Paquete demo de Motor de Calidad
 Author: Enzo Ipanaque
 Author-email: enzo.ipanaque@ms-peru.com
 License: Management Solutions
 Description-Content-Type: text/markdown
 
 # Motor de Calidad de Datos
```

### Comparing `MotorDeCalidad-1.9.8/PKG-INFO` & `MotorDeCalidad-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MotorDeCalidad
-Version: 1.9.8
+Version: 1.9.9
 Summary: Paquete demo de Motor de Calidad
 Author: Enzo Ipanaque
 Author-email: enzo.ipanaque@ms-peru.com
 License: Management Solutions
 Description-Content-Type: text/markdown
 
 # Motor de Calidad de Datos
```

### Comparing `MotorDeCalidad-1.9.8/README.md` & `MotorDeCalidad-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `MotorDeCalidad-1.9.8/motordecalidad/constants.py` & `MotorDeCalidad-1.9.9/motordecalidad/constants.py`

 * *Files identical despite different names*

### Comparing `MotorDeCalidad-1.9.8/motordecalidad/functions.py` & `MotorDeCalidad-1.9.9/motordecalidad/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from motordecalidad.constants import *
 from motordecalidad.utilities import *
 import datetime
 import time
 from motordecalidad.rules import *
 
 
-print("Motor de Calidad Version Release 1.9.8")
+print("Motor de Calidad Version Release 1.9.9")
 
 # Main function, Invokes all the parameters from the json, Optionally filters, starts the rule validation
 # Writes and returns the summary of the validation 
 def startValidation(inputspark,config,dfltPath=""):
     global spark
     global dbutils
     global DefaultPath
```

### Comparing `MotorDeCalidad-1.9.8/motordecalidad/rules.py` & `MotorDeCalidad-1.9.9/motordecalidad/rules.py`

 * *Files identical despite different names*

### Comparing `MotorDeCalidad-1.9.8/motordecalidad/utilities.py` & `MotorDeCalidad-1.9.9/motordecalidad/utilities.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     from email.mime.text import MIMEText
     dataDict = data.collect()
     ok_rules = ""
     for i in dataDict:
         ok_rules = ok_rules + "\n" + str(i[0]) + ":" + str(i[1]) + "\n"
     sslPort = 465  # For SSL
     smtp_server = 'smtp.gmail.com'
-    sender_email = "motordecalidadtlfhispan@gmail.com"
-    password = "lblbnbwquhnlpofn"
+    sender_email = "correostelefonicahispan@gmail.com"
+    password = "xjldsavagzrobvqw"
     text = f"""\
     Hola,
     Su ejecucion del motor de calidad ha dado los siguientes resultados:
     Cantidad de Registros Evaluados: {registerAmount}
     Cantidad de Reglas Evaluadas: {rulesNumber}
     Tasa de éxito promedio por regla: {ok_rules}
     Se pueden consultar los resultados en {outputPath} """
```

