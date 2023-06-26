# Comparing `tmp/costeopy_package-0.2.0.tar.gz` & `tmp/costeopy_package-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "costeopy_package-0.2.0.tar", last modified: Tue Apr  4 04:11:24 2023, max compression
+gzip compressed data, was "costeopy_package-0.2.1.tar", last modified: Mon Jun 26 08:24:21 2023, max compression
```

## Comparing `costeopy_package-0.2.0.tar` & `costeopy_package-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 04:11:24.648800 costeopy_package-0.2.0/
--rw-rw-rw-   0        0        0     1069 2022-03-17 16:58:55.000000 costeopy_package-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1438 2023-04-04 04:11:24.648800 costeopy_package-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      924 2023-04-04 04:11:05.000000 costeopy_package-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 04:11:24.628844 costeopy_package-0.2.0/micospy/
-drwxrwxrwx   0        0        0        0 2023-04-04 04:11:24.633847 costeopy_package-0.2.0/micospy/costeopy_package/
--rw-rw-rw-   0        0        0       27 2022-03-17 16:51:11.000000 costeopy_package-0.2.0/micospy/costeopy_package/__init__.py
--rw-rw-rw-   0        0        0    37056 2023-04-04 04:00:46.000000 costeopy_package-0.2.0/micospy/costeopy_package/costeopy.py
-drwxrwxrwx   0        0        0        0 2023-04-04 04:11:24.647796 costeopy_package-0.2.0/micospy/costeopy_package.egg-info/
--rw-rw-rw-   0        0        0     1438 2023-04-04 04:11:24.000000 costeopy_package-0.2.0/micospy/costeopy_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-04-04 04:11:24.000000 costeopy_package-0.2.0/micospy/costeopy_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 04:11:24.000000 costeopy_package-0.2.0/micospy/costeopy_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-04 04:11:24.000000 costeopy_package-0.2.0/micospy/costeopy_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-03-17 16:58:55.000000 costeopy_package-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      659 2023-04-04 04:11:24.649795 costeopy_package-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 08:24:21.583370 costeopy_package-0.2.1/
+-rw-rw-rw-   0        0        0     1069 2022-03-17 16:58:55.000000 costeopy_package-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-06-26 08:24:21.583370 costeopy_package-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      606 2023-06-26 08:22:09.000000 costeopy_package-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 08:24:21.559461 costeopy_package-0.2.1/micospy/
+drwxrwxrwx   0        0        0        0 2023-06-26 08:24:21.566853 costeopy_package-0.2.1/micospy/costeopy_package/
+-rw-rw-rw-   0        0        0       27 2022-03-17 16:51:11.000000 costeopy_package-0.2.1/micospy/costeopy_package/__init__.py
+-rw-rw-rw-   0        0        0    54931 2023-06-26 08:22:09.000000 costeopy_package-0.2.1/micospy/costeopy_package/costeopy.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:24:21.583370 costeopy_package-0.2.1/micospy/costeopy_package.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-06-26 08:24:21.000000 costeopy_package-0.2.1/micospy/costeopy_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-06-26 08:24:21.000000 costeopy_package-0.2.1/micospy/costeopy_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:24:21.000000 costeopy_package-0.2.1/micospy/costeopy_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-26 08:24:21.000000 costeopy_package-0.2.1/micospy/costeopy_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-03-17 16:58:55.000000 costeopy_package-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      659 2023-06-26 08:24:21.592974 costeopy_package-0.2.1/setup.cfg
```

### Comparing `costeopy_package-0.2.0/LICENSE` & `costeopy_package-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `costeopy_package-0.2.0/PKG-INFO` & `costeopy_package-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: costeopy_package
-Version: 0.2.0
+Version: 0.2.1
 Summary: Costeo de cas
 Home-page: https://github.com/francomrf/Costeo_Python.git
 Author: Franco F
 Author-email: francomrf@gmail.com
 Project-URL: Bug Tracker, https://github.com/francomrf/Costeo_Python.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Bienvenido al documento guía del paquete de Python creado por el equipo de Analítica de Datos. Este paquete ha sido diseñado para ayudar a los científicos de datos, analistas y programadores a trabajar de manera más eficiente con sus datos.
+Bienvenido al paquete de Costeo para intervenciones pedagógicas en Python creado por el equipo de Analítica de Datos. Este paquete ha sido diseñado para ayudar a los científicos de datos, analistas y programadores a trabajar de manera más eficiente con sus datos.
 
 Nuestro equipo ha invertido tiempo y esfuerzo en desarrollar una herramienta de análisis de datos poderosa, fácil de usar y flexible que pueda satisfacer las necesidades de cualquier usuario.
 
-Este documento guía proporcionará una visión general detallada de todas las funcionalidades del paquete, así como instrucciones paso a paso sobre cómo utilizarlo. Ya sea que seas un usuario experimentado o un principiante en programación, este paquete te permitirá realizar análisis de datos más rápidos y eficientes en Python.
-
 Esperamos que encuentres este paquete útil y esperamos recibir tus comentarios y sugerencias para mejorar continuamente nuestro trabajo.
```

### Comparing `costeopy_package-0.2.0/README.md` & `costeopy_package-0.2.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,5 @@
-Bienvenido al documento guía del paquete de Python creado por el equipo de Analítica de Datos. Este paquete ha sido diseñado para ayudar a los científicos de datos, analistas y programadores a trabajar de manera más eficiente con sus datos.
+Bienvenido al paquete de Costeo para intervenciones pedagógicas en Python creado por el equipo de Analítica de Datos. Este paquete ha sido diseñado para ayudar a los científicos de datos, analistas y programadores a trabajar de manera más eficiente con sus datos.
 
 Nuestro equipo ha invertido tiempo y esfuerzo en desarrollar una herramienta de análisis de datos poderosa, fácil de usar y flexible que pueda satisfacer las necesidades de cualquier usuario.
 
-Este documento guía proporcionará una visión general detallada de todas las funcionalidades del paquete, así como instrucciones paso a paso sobre cómo utilizarlo. Ya sea que seas un usuario experimentado o un principiante en programación, este paquete te permitirá realizar análisis de datos más rápidos y eficientes en Python.
-
 Esperamos que encuentres este paquete útil y esperamos recibir tus comentarios y sugerencias para mejorar continuamente nuestro trabajo.
```

### Comparing `costeopy_package-0.2.0/micospy/costeopy_package.egg-info/PKG-INFO` & `costeopy_package-0.2.1/micospy/costeopy_package.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: costeopy-package
-Version: 0.2.0
+Version: 0.2.1
 Summary: Costeo de cas
 Home-page: https://github.com/francomrf/Costeo_Python.git
 Author: Franco F
 Author-email: francomrf@gmail.com
 Project-URL: Bug Tracker, https://github.com/francomrf/Costeo_Python.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Bienvenido al documento guía del paquete de Python creado por el equipo de Analítica de Datos. Este paquete ha sido diseñado para ayudar a los científicos de datos, analistas y programadores a trabajar de manera más eficiente con sus datos.
+Bienvenido al paquete de Costeo para intervenciones pedagógicas en Python creado por el equipo de Analítica de Datos. Este paquete ha sido diseñado para ayudar a los científicos de datos, analistas y programadores a trabajar de manera más eficiente con sus datos.
 
 Nuestro equipo ha invertido tiempo y esfuerzo en desarrollar una herramienta de análisis de datos poderosa, fácil de usar y flexible que pueda satisfacer las necesidades de cualquier usuario.
 
-Este documento guía proporcionará una visión general detallada de todas las funcionalidades del paquete, así como instrucciones paso a paso sobre cómo utilizarlo. Ya sea que seas un usuario experimentado o un principiante en programación, este paquete te permitirá realizar análisis de datos más rápidos y eficientes en Python.
-
 Esperamos que encuentres este paquete útil y esperamos recibir tus comentarios y sugerencias para mejorar continuamente nuestro trabajo.
```

### Comparing `costeopy_package-0.2.0/setup.cfg` & `costeopy_package-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f73 7465 6f70 795f 7061 636b   = costeopy_pack
 00000020: 6167 650d 0a76 6572 7369 6f6e 203d 2030  age..version = 0
-00000030: 2e32 2e30 0d0a 6175 7468 6f72 203d 2046  .2.0..author = F
+00000030: 2e32 2e31 0d0a 6175 7468 6f72 203d 2046  .2.1..author = F
 00000040: 7261 6e63 6f20 460d 0a61 7574 686f 725f  ranco F..author_
 00000050: 656d 6169 6c20 3d20 6672 616e 636f 6d72  email = francomr
 00000060: 6640 676d 6169 6c2e 636f 6d0d 0a64 6573  f@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2043 6f73 7465  cription = Coste
 00000080: 6f20 6465 2063 6173 0d0a 6c6f 6e67 5f64  o de cas..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 000000a0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
```

