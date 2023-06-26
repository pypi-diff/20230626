# Comparing `tmp/onedep_deposition-0.1.dev7.tar.gz` & `tmp/onedep_deposition-0.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onedep_deposition-0.1.dev7.tar", last modified: Fri Jun 23 11:14:01 2023, max compression
+gzip compressed data, was "onedep_deposition-0.1.dev8.tar", last modified: Mon Jun 26 12:03:08 2023, max compression
```

## Comparing `onedep_deposition-0.1.dev7.tar` & `onedep_deposition-0.1.dev8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-23 11:14:01.028679 onedep_deposition-0.1.dev7/
--rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev7/LICENSE
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-23 11:14:01.028335 onedep_deposition-0.1.dev7/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev7/README.md
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-23 11:14:01.021743 onedep_deposition-0.1.dev7/onedep_deposition/
--rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-23 11:13:09.000000 onedep_deposition-0.1.dev7/onedep_deposition/__init__.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-23 11:14:01.027718 onedep_deposition-0.1.dev7/onedep_deposition/cli/
--rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev7/onedep_deposition/cli/__init__.py
--rw-r--r--   0 peisach    (502) staff       (20)    13091 2023-06-23 11:13:00.000000 onedep_deposition-0.1.dev7/onedep_deposition/cli/cli.py
--rw-r--r--   0 peisach    (502) staff       (20)      589 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev7/onedep_deposition/decorators.py
--rw-r--r--   0 peisach    (502) staff       (20)    15606 2023-06-23 11:13:00.000000 onedep_deposition-0.1.dev7/onedep_deposition/deposit_api.py
--rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev7/onedep_deposition/enum.py
--rw-r--r--   0 peisach    (502) staff       (20)      316 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev7/onedep_deposition/exceptions.py
--rw-r--r--   0 peisach    (502) staff       (20)    13030 2023-06-23 11:13:00.000000 onedep_deposition-0.1.dev7/onedep_deposition/models.py
--rw-r--r--   0 peisach    (502) staff       (20)     6182 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev7/onedep_deposition/rest_adapter.py
-drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-23 11:14:01.026226 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/
--rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/PKG-INFO
--rw-r--r--   0 peisach    (502) staff       (20)      558 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/SOURCES.txt
--rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/dependency_links.txt
--rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/entry_points.txt
--rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/requires.txt
--rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-23 11:14:01.000000 onedep_deposition-0.1.dev7/onedep_deposition.egg-info/top_level.txt
--rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev7/pyproject.toml
--rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-23 11:14:01.028802 onedep_deposition-0.1.dev7/setup.cfg
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-26 12:03:08.732118 onedep_deposition-0.1.dev8/
+-rw-r--r--   0 peisach    (502) staff       (20)      552 2023-06-13 13:04:02.000000 onedep_deposition-0.1.dev8/LICENSE
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-26 12:03:08.731805 onedep_deposition-0.1.dev8/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)     4641 2023-06-17 15:30:45.000000 onedep_deposition-0.1.dev8/README.md
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-26 12:03:08.727370 onedep_deposition-0.1.dev8/onedep_deposition/
+-rw-r--r--   0 peisach    (502) staff       (20)       25 2023-06-26 12:02:43.000000 onedep_deposition-0.1.dev8/onedep_deposition/__init__.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-26 12:03:08.731084 onedep_deposition-0.1.dev8/onedep_deposition/cli/
+-rw-r--r--   0 peisach    (502) staff       (20)        0 2023-06-17 17:42:03.000000 onedep_deposition-0.1.dev8/onedep_deposition/cli/__init__.py
+-rw-r--r--   0 peisach    (502) staff       (20)    13336 2023-06-26 12:01:58.000000 onedep_deposition-0.1.dev8/onedep_deposition/cli/cli.py
+-rw-r--r--   0 peisach    (502) staff       (20)      589 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev8/onedep_deposition/decorators.py
+-rw-r--r--   0 peisach    (502) staff       (20)    15722 2023-06-26 12:01:58.000000 onedep_deposition-0.1.dev8/onedep_deposition/deposit_api.py
+-rw-r--r--   0 peisach    (502) staff       (20)     9006 2023-06-15 13:32:19.000000 onedep_deposition-0.1.dev8/onedep_deposition/enum.py
+-rw-r--r--   0 peisach    (502) staff       (20)      316 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev8/onedep_deposition/exceptions.py
+-rw-r--r--   0 peisach    (502) staff       (20)    13115 2023-06-26 12:01:58.000000 onedep_deposition-0.1.dev8/onedep_deposition/models.py
+-rw-r--r--   0 peisach    (502) staff       (20)     6182 2023-06-20 13:27:14.000000 onedep_deposition-0.1.dev8/onedep_deposition/rest_adapter.py
+drwxr-xr-x   0 peisach    (502) staff       (20)        0 2023-06-26 12:03:08.730280 onedep_deposition-0.1.dev8/onedep_deposition.egg-info/
+-rw-r--r--   0 peisach    (502) staff       (20)     5174 2023-06-26 12:03:08.000000 onedep_deposition-0.1.dev8/onedep_deposition.egg-info/PKG-INFO
+-rw-r--r--   0 peisach    (502) staff       (20)      558 2023-06-26 12:03:08.000000 onedep_deposition-0.1.dev8/onedep_deposition.egg-info/SOURCES.txt
+-rw-r--r--   0 peisach    (502) staff       (20)        1 2023-06-26 12:03:08.000000 onedep_deposition-0.1.dev8/onedep_deposition.egg-info/dependency_links.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       68 2023-06-26 12:03:08.000000 onedep_deposition-0.1.dev8/onedep_deposition.egg-info/entry_points.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       15 2023-06-26 12:03:08.000000 onedep_deposition-0.1.dev8/onedep_deposition.egg-info/requires.txt
+-rw-r--r--   0 peisach    (502) staff       (20)       18 2023-06-26 12:03:08.000000 onedep_deposition-0.1.dev8/onedep_deposition.egg-info/top_level.txt
+-rw-r--r--   0 peisach    (502) staff       (20)     1039 2023-06-17 17:50:36.000000 onedep_deposition-0.1.dev8/pyproject.toml
+-rw-r--r--   0 peisach    (502) staff       (20)       38 2023-06-26 12:03:08.732227 onedep_deposition-0.1.dev8/setup.cfg
```

### Comparing `onedep_deposition-0.1.dev7/LICENSE` & `onedep_deposition-0.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev7/PKG-INFO` & `onedep_deposition-0.1.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep_deposition
-Version: 0.1.dev7
+Version: 0.1.dev8
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev7/README.md` & `onedep_deposition-0.1.dev8/README.md`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev7/onedep_deposition/cli/cli.py` & `onedep_deposition-0.1.dev8/onedep_deposition/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 import re
 import os
 import json
+import logging
 from typing import List, Union, Dict
 from onedep_deposition.deposit_api import DepositApi
 from onedep_deposition.enum import Country, FileType
 from onedep_deposition.__init__ import __version__ as VERSION
 
 
 def get_api_key():
@@ -73,20 +74,21 @@
 @click.option("-t", "--type", "dep_type", help="Experiment type [em, xray, fiber, neutron, ec, nmr, ssnmr]")
 @click.option("-e", "--email", "email", help="Main depositor email")
 @click.option("-u", "--users", "users", multiple=True, help="List of users to add to the deposition")
 @click.option("-c", "--country", "country_string", help="Country of the main depositor")
 @click.option("-s", "--subtype", "subtype", help="Experiment subtype, only valid if type is EM")
 @click.option("-E", "--related_emdb", "related_emdb", help="Related EMDB code. Only valid for EM and EC")
 @click.option("-B", "--related_bmrb", "related_bmrb", help="Related BMRB code. Only valid for NMR")
-@click.option("--no_coordinates", "no_coordinates", is_flag=True, help="Depositing coordinates file? (y/n)")
+@click.option("--no_coordinates", "no_coordinates", is_flag=True, help="Not including coordinates file")
+@click.option("--no_map", "no_map", is_flag=True, help="Not including map file (only for EC)")
 @click.option("-p", "--password", "password", help="Deposition password")
 @click.pass_context
 @create_api
 def create(api: DepositApi, ctx: Dict, dep_type: str, email: str, users: List[str], country_string: str, subtype: str,
-           related_emdb: str, related_bmrb: str, password: str, no_coordinates: bool = False):
+           related_emdb: str, related_bmrb: str, password: str, no_coordinates: bool = False, no_map: bool = False):
     """`create` deposition command handler"""
     if subtype:
         if subtype not in ["helical", "single", "subtomogram", "tomography"]:
             raise click.BadParameter("Invalid experiment subtype, options are: helical, single, subtomogram, tomography")
     if not email:
         raise click.BadParameter("Email is required")
     if not re.match(r'^[\w\.-]+@[\w\.-]+\.\w+$', email):
@@ -102,31 +104,33 @@
             raise click.BadParameter("Invalid BMRB code")
     if related_emdb:
         if not re.match(r'^EMD-\d{4,5}$', related_emdb):
             raise click.BadParameter("Invalid EMDB code")
     if no_coordinates:
         if dep_type in ["xray", "fiber", "neutron"]:
             raise click.BadParameter("Coordinates are mandatory for X-ray, fiber and neutron diffraction")
+    if dep_type != "ec" and no_map:
+        logging.warning("--no_map flag is only used in EC depositions.")
     country = get_country_enum(country_string)
     coordinates = not no_coordinates
 
     if dep_type == "em":
         deposition = api.create_em_deposition(email, users, country, subtype, coordinates, related_emdb, password)
     elif dep_type == "xray":
         deposition = api.create_xray_deposition(email, users, country, password)
     elif dep_type == "fiber":
         deposition = api.create_fiber_deposition(email, users, country, password)
     elif dep_type == "neutron":
         deposition = api.create_neutron_deposition(email, users, country, password)
     elif dep_type == "ec":
-        deposition = api.create_ec_deposition(email, users, country, coordinates, related_emdb, password)
+        deposition = api.create_ec_deposition(email, users, country, coordinates, password, related_emdb, no_map)
     elif dep_type == "nmr":
-        deposition = api.create_nmr_deposition(email, users, country, coordinates, related_bmrb, password)
+        deposition = api.create_nmr_deposition(email, users, country, coordinates, password, related_bmrb)
     elif dep_type == "ssnmr":
-        deposition = api.create_ssnmr_deposition(email, users, country, coordinates, related_bmrb, password)
+        deposition = api.create_ssnmr_deposition(email, users, country, coordinates, password, related_bmrb)
     else:
         raise click.BadParameter("Invalid experiment type, options are: em, xray, fiber, neutron, ec, nmr, ssnmr")
     click.echo(deposition)
 
 
 @deposition_group.command(name="get", help="Get deposition info")
 @click.argument("dep_id")
```

### Comparing `onedep_deposition-0.1.dev7/onedep_deposition/decorators.py` & `onedep_deposition-0.1.dev8/onedep_deposition/decorators.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev7/onedep_deposition/deposit_api.py` & `onedep_deposition-0.1.dev8/onedep_deposition/deposit_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,26 +124,28 @@
         :param password: Password
         :return: Response
         """
         experiment = Experiment(exp_type="neutron", coordinates=True)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
-    def create_ec_deposition(self, email: str, users: List[str], country: Country, coordinates: bool, password: str = "", related_emdb: str = None, **kwargs) -> Deposit:  # pylint: disable=unused-argument
+    def create_ec_deposition(self, email: str, users: List[str], country: Country, coordinates: bool, password: str = "",
+                             related_emdb: str = None, sf_only: bool = False, **kwargs) -> Deposit:  # pylint: disable=unused-argument
         """
         Create an Electron crystallography deposition
         :param email: User e-mail
         :param users: List of ORCID ids that can access this deposition
         :param country: Country from enum list
         :param coordinates: Depositing coordinates file?
         :param password: Password
         :param related_emdb: Related EMDB id
+        :param sf_only: Structure factor only?
         :return: Response
         """
-        experiment = Experiment(exp_type="ec", related_emdb=related_emdb, coordinates=coordinates)
+        experiment = Experiment(exp_type="ec", related_emdb=related_emdb, coordinates=coordinates, sf_only=sf_only)
         deposit = self.create_deposition(email=email, users=users, country=country, experiments=[experiment], password=password)
         return deposit
 
     def create_nmr_deposition(self, email: str, users: List[str], country: Country, coordinates: bool, password: str = "",  # pylint: disable=unused-argument
                               related_bmrb: str = None, **kwargs) -> Deposit:
         """
         Create a NMR deposition
```

### Comparing `onedep_deposition-0.1.dev7/onedep_deposition/enum.py` & `onedep_deposition-0.1.dev8/onedep_deposition/enum.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev7/onedep_deposition/models.py` & `onedep_deposition-0.1.dev8/onedep_deposition/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,28 +35,30 @@
         """
         return f"STATUS: {self._status_code}, MESSAGE: {self._message}\n{self._data}"
 
 
 class Experiment:
     """Class representing an experiment"""
     def __init__(self, exp_type: Union[ExperimentType, str], coordinates: bool = True, subtype: Union[EMSubType, str] = None,
-                 related_emdb: str = None, related_bmrb: str = None):
+                 related_emdb: str = None, related_bmrb: str = None, sf_only: bool = False):
         """
         Constructor for Experiment
         :param exp_type:
         :param coordinates:
         :param subtype:
         :param related_emdb:
         :param related_bmrb:
+        :param sf_only:
         """
         self._coordinates = bool(coordinates)
         self._type = None
         self._subtype = None
         self._related_emdb = str(related_emdb) if related_emdb is not None else None
         self._related_bmrb = str(related_bmrb) if related_bmrb is not None else None
+        self._sf_only = bool(sf_only)
 
         if type(exp_type) == ExperimentType:
             self._type = exp_type
         elif exp_type:
             self._type = ExperimentType(exp_type)
         if type(subtype) == EMSubType:
             self._subtype = subtype
```

### Comparing `onedep_deposition-0.1.dev7/onedep_deposition/rest_adapter.py` & `onedep_deposition-0.1.dev8/onedep_deposition/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev7/onedep_deposition.egg-info/PKG-INFO` & `onedep_deposition-0.1.dev8/onedep_deposition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onedep-deposition
-Version: 0.1.dev7
+Version: 0.1.dev8
 Summary: Package for wrapping the OneDep deposition API services
 Author-email: Neli Jose da Fonseca Junior <neli@ebi.ac.uk>
 License: apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `onedep_deposition-0.1.dev7/onedep_deposition.egg-info/SOURCES.txt` & `onedep_deposition-0.1.dev8/onedep_deposition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onedep_deposition-0.1.dev7/pyproject.toml` & `onedep_deposition-0.1.dev8/pyproject.toml`

 * *Files identical despite different names*

