# Comparing `tmp/eons-2.6.4.tar.gz` & `tmp/eons-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.6.4.tar", last modified: Tue Jun 20 04:20:16 2023, max compression
+gzip compressed data, was "eons-2.6.5.tar", last modified: Sun Jun 25 22:38:26 2023, max compression
```

## Comparing `eons-2.6.4.tar` & `eons-2.6.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.226518 eons-2.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-20 04:20:16.226518 eons-2.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-20 04:19:57.000000 eons-2.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.218517 eons-2.6.4/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.222517 eons-2.6.4/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 04:20:06.000000 eons-2.6.4/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92334 2023-06-20 04:20:06.000000 eons-2.6.4/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.222517 eons-2.6.4/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:20:06.000000 eons-2.6.4/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.226518 eons-2.6.4/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:20:06.000000 eons-2.6.4/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 04:19:47.000000 eons-2.6.4/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 04:20:16.222517 eons-2.6.4/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 04:20:16.000000 eons-2.6.4/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-20 04:20:06.000000 eons-2.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 04:20:16.226518 eons-2.6.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-25 22:38:26.756589 eons-2.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22218 2023-06-25 22:38:08.000000 eons-2.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.752589 eons-2.6.5/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 22:38:17.000000 eons-2.6.5/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92334 2023-06-25 22:38:17.000000 eons-2.6.5/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:38:17.000000 eons-2.6.5/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:38:17.000000 eons-2.6.5/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-25 22:37:56.000000 eons-2.6.5/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 22:38:26.756589 eons-2.6.5/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22424 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-25 22:38:26.000000 eons-2.6.5/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-25 22:38:17.000000 eons-2.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-25 22:38:26.760589 eons-2.6.5/setup.cfg
```

### Comparing `eons-2.6.4/PKG-INFO` & `eons-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.4
+Version: 2.6.5
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.4/README.md` & `eons-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.6.4/pkg/eons/eons.py` & `eons-2.6.5/pkg/eons/eons.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 import logging
-import os
-import shutil
+import operator
+import traceback
+import jsonpickle
 from copy import deepcopy
-import builtins
+import os
 import sys
 import pkgutil
 import importlib.machinery
 import importlib.util
 import types
-import traceback
-import jsonpickle
+import inspect
+import shutil
+import builtins
+from pathlib import Path
+from subprocess import Popen
+from subprocess import PIPE
+from subprocess import STDOUT
 import argparse
 import requests
 import yaml
 from requests_futures.sessions import FuturesSession
-from pathlib import Path
 from tqdm import tqdm
 from zipfile import ZipFile
 from distutils.dir_util import mkpath
 from eot import EOT
-import operator
-from subprocess import Popen
-from subprocess import PIPE
-from subprocess import STDOUT
-import inspect
 import re
 
 ######## START CONTENT ########
-def INVALID_NAME():
-	return "INVALID_NAME"
-
 class ActualType(type):
 	def __repr__(self):
 		return self.__name__
 
 class GlobalError(Exception, metaclass=ActualType): pass
 
 class NotInstantiableError(Exception, metaclass=ActualType): pass
@@ -61,14 +58,160 @@
 class FatalCannotExecute(Fatal, metaclass=ActualType): pass
 
 class PackageError(Exception, metaclass=ActualType): pass
 
 class MethodPendingPopulation(Exception, metaclass=ActualType): pass
 
 
+# util is a namespace for any miscellaneous utilities.
+# You cannot create a util.
+class util:
+	def __init__(this):
+		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
+
+	#dot.notation access to dictionary attributes
+	class DotDict(dict):
+		__getattr__ = dict.get
+		__setattr__ = dict.__setitem__
+		__delattr__ = dict.__delitem__
+
+		def __deepcopy__(this, memo=None):
+			return util.DotDict(deepcopy(dict(this), memo=memo))
+
+	# DotDict doesn't pickle right, since it's a class and not a native dict.
+	class DotDictPickler(jsonpickle.handlers.BaseHandler):
+		def flatten(this, dotdict, data):
+			return dict(dotdict)
+
+	@staticmethod
+	def RecursiveAttrFunc(func, obj, attrList):
+		attr = attrList.pop(0)
+		if (not attrList):
+			return eval(f"{func}attr(obj, attr)")
+		if (not hasattr(obj, attr)):
+			raise AttributeError(f"{obj} has not attribute '{attr}'")
+		return util.RecursiveAttrFunc(func, getattr(obj, attr), attrList)
+
+	@staticmethod
+	def HasAttr(obj, attrStr):
+		return util.RecursiveAttrFunc('has', obj, attrStr.split('.'))
+
+	@staticmethod
+	def GetAttr(obj, attrStr):
+		return util.RecursiveAttrFunc('get', obj, attrStr.split('.'))
+
+	@staticmethod
+	def SetAttr(obj, attrStr):
+		raise NotImplementedError(f"util.SetAttr has not been implemented yet.")
+
+
+	@staticmethod
+	def LogStack():
+		logging.debug(traceback.format_exc())
+
+
+	class console:
+
+		# Read this (just do it): https://stackoverflow.com/questions/4842424/list-of-ansi-color-escape-sequences
+
+		saturationCode = {
+			'dark': 3,
+			'light': 9
+		}
+
+		foregroundCodes = {
+			'black': 0,
+			'red': 1,
+			'green': 2,
+			'yellow': 3,
+			'blue': 4,
+			'magenta': 5,
+			'cyan': 6,
+			'white': 7
+		}
+
+		backgroundCodes = {
+			'none': 0,
+			'black': 40,
+			'red': 41,
+			'green': 42,
+			'yellow': 43,
+			'blue': 44,
+			'magenta': 45,
+			'cyan': 46,
+			'white': 47,
+		}
+
+		styleCodes = {
+			'none': 0,
+			'bold': 1,
+			'faint': 2, # Not widely supported.
+			'italic': 3, # Not widely supported.
+			'underline': 4,
+			'blink_slow': 5,
+			'blink_fast': 6, # Not widely supported.
+			'invert': 7,
+			'conceal': 8, # Not widely supported.
+			'strikethrough': 9, # Not widely supported.
+			'frame': 51,
+			'encircle': 52,
+			'overline': 53
+		}
+
+		@classmethod
+		def GetColorCode(cls, foreground, saturation='dark', background='none', styles=None):
+			if (styles is None):
+				styles = []
+			#\x1b may also work.
+			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
+			if (background != 'none'):
+				compiledCode += f";{cls.backgroundCodes[background]}"
+			if (styles):
+				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in list(styles)])
+			compiledCode += 'm'
+			return compiledCode
+
+		resetStyle = "\033[0m"
+
+
+	# Add a logging level
+	# per: https://stackoverflow.com/questions/2183233/how-to-add-a-custom-loglevel-to-pythons-logging-facility/35804945#35804945
+	@staticmethod
+	def AddLoggingLevel(level, value):
+		levelName = level.upper()
+		methodName = level.lower()
+
+		if hasattr(logging, levelName):
+			raise AttributeError('{} already defined in logging module'.format(levelName))
+		if hasattr(logging, methodName):
+			raise AttributeError('{} already defined in logging module'.format(methodName))
+		if hasattr(logging.getLogger(), methodName):
+			raise AttributeError('{} already defined in logger class'.format(methodName))
+
+		# This method was inspired by the answers to Stack Overflow post
+		# http://stackoverflow.com/q/2183233/2988730, especially
+		# http://stackoverflow.com/a/13638084/2988730
+		def logForLevel(this, message, *args, **kwargs):
+			if this.isEnabledFor(value):
+				this._log(value, message, args, **kwargs)
+		def logToRoot(message, *args, **kwargs):
+			logging.log(value, message, *args, **kwargs)
+
+		logging.addLevelName(value, levelName)
+		setattr(logging, levelName, value)
+		setattr(logging.getLogger(), methodName, logForLevel)
+		setattr(logging, methodName, logToRoot)
+
+
+jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
+
+def INVALID_NAME():
+	return "INVALID_NAME"
+
+
 #Self registration for use with json loading.
 #Any class that derives from SelfRegistering can be instantiated with:
 #   SelfRegistering("ClassName")
 #Based on: https://stackoverflow.com/questions/55973284/how-to-create-this-registering-factory-in-python/55973426
 class SelfRegistering(object):
 
 	def __init__(this, *args, **kwargs):
@@ -178,155 +321,171 @@
 
 
 	# Sets valid to false.
 	def Invalidate(this):
 		this.valid = False
 
 
-# util is a namespace for any miscellaneous utilities.
-# You cannot create a util.
-class util:
-	def __init__(this):
-		raise NotInstantiableError("util is a namespace, not a class; it cannot be instantiated.")
+# A DataContainer allows Data to be stored and worked with.
+# This class is intended to be derived from and added to.
+# Each DataContainer is comprised of multiple Data (see Datum.py for more).
+# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
+class DataContainer(Datum):
 
-	#dot.notation access to dictionary attributes
-	class DotDict(dict):
-		__getattr__ = dict.get
-		__setattr__ = dict.__setitem__
-		__delattr__ = dict.__delitem__
+	def __init__(this, name=INVALID_NAME()):
+		super().__init__(name)
 
-		def __deepcopy__(this, memo=None):
-			return util.DotDict(deepcopy(dict(this), memo=memo))
+		# The data *this contains.
+		this.data = []
 
-	# DotDict doesn't pickle right, since it's a class and not a native dict.
-	class DotDictPickler(jsonpickle.handlers.BaseHandler):
-		def flatten(this, dotdict, data):
-			return dict(dotdict)
 
-	@staticmethod
-	def RecursiveAttrFunc(func, obj, attrList):
-		attr = attrList.pop(0)
-		if (not attrList):
-			return eval(f"{func}attr(obj, attr)")
-		if (not hasattr(obj, attr)):
-			raise AttributeError(f"{obj} has not attribute '{attr}'")
-		return util.RecursiveAttrFunc(func, getattr(obj, attr), attrList)
+	# RETURNS: an empty, invalid Datum.
+	def InvalidDatum(this):
+		ret = Datum()
+		ret.Invalidate()
+		return ret
 
-	@staticmethod
-	def HasAttr(obj, attrStr):
-		return util.RecursiveAttrFunc('has', obj, attrStr.split('.'))
 
-	@staticmethod
-	def GetAttr(obj, attrStr):
-		return util.RecursiveAttrFunc('get', obj, attrStr.split('.'))
+	# Sort things! Requires by be a valid attribute of all Data.
+	def SortData(this, by):
+		this.data.sort(key=operator.attrgetter(by))
 
-	@staticmethod
-	def SetAttr(obj, attrStr):
-		raise NotImplementedError(f"util.SetAttr has not been implemented yet.")
 
+	# Adds a Datum to *this
+	def AddDatum(this, datum):
+		this.data.append(datum)
 
-	@staticmethod
-	def LogStack():
-		logging.debug(traceback.format_exc())
 
+	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
+	def GetDatumBy(this, datumAttribute, match):
+		for d in this.data:
+			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
+				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
+					return d
+			except Exception as e:
+				logging.error(f"{this.name} - {e.message}")
+				continue
+		return this.InvalidDatum()
 
-	class console:
 
-		# Read this (just do it): https://stackoverflow.com/questions/4842424/list-of-ansi-color-escape-sequences
+	# RETURNS: a Datum of the given name, an invalid Datum if none found.
+	def GetDatum(this, name):
+		return this.GetDatumBy('name', name)
 
-		saturationCode = {
-			'dark': 3,
-			'light': 9
-		}
 
-		foregroundCodes = {
-			'black': 0,
-			'red': 1,
-			'green': 2,
-			'yellow': 3,
-			'blue': 4,
-			'magenta': 5,
-			'cyan': 6,
-			'white': 7
-		}
+	# Removes all Data in toRem from *this.
+	# RETURNS: the Data removed
+	def RemoveData(this, toRem):
+		# logging.debug(f"Removing {toRem}")
+		this.data = [d for d in this.data if d not in toRem]
+		return toRem
 
-		backgroundCodes = {
-			'none': 0,
-			'black': 40,
-			'red': 41,
-			'green': 42,
-			'yellow': 43,
-			'blue': 44,
-			'magenta': 45,
-			'cyan': 46,
-			'white': 47,
-		}
 
-		styleCodes = {
-			'none': 0,
-			'bold': 1,
-			'faint': 2, # Not widely supported.
-			'italic': 3, # Not widely supported.
-			'underline': 4,
-			'blink_slow': 5,
-			'blink_fast': 6, # Not widely supported.
-			'invert': 7,
-			'conceal': 8, # Not widely supported.
-			'strikethrough': 9, # Not widely supported.
-			'frame': 51,
-			'encircle': 52,
-			'overline': 53
-		}
+	# Removes all Data which match toRem along the given attribute
+	def RemoveDataBy(this, datumAttribute, toRem):
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
+		return this.RemoveData(toRem)
 
-		@classmethod
-		def GetColorCode(cls, foreground, saturation='dark', background='none', styles=None):
-			if (styles is None):
-				styles = []
-			#\x1b may also work.
-			compiledCode = f"\033[{cls.saturationCode[saturation]}{cls.foregroundCodes[foreground]}"
-			if (background != 'none'):
-				compiledCode += f";{cls.backgroundCodes[background]}"
-			if (styles):
-				compiledCode += ';' + ';'.join([str(cls.styleCodes[s]) for s in list(styles)])
-			compiledCode += 'm'
-			return compiledCode
 
-		resetStyle = "\033[0m"
+	# Removes all Data in *this except toKeep.
+	# RETURNS: the Data removed
+	def KeepOnlyData(this, toKeep):
+		toRem = [d for d in this.data if d not in toKeep]
+		return this.RemoveData(toRem)
 
 
-	# Add a logging level
-	# per: https://stackoverflow.com/questions/2183233/how-to-add-a-custom-loglevel-to-pythons-logging-facility/35804945#35804945
-	@staticmethod
-	def AddLoggingLevel(level, value):
-		levelName = level.upper()
-		methodName = level.lower()
+	# Removes all Data except those that match toKeep along the given attribute
+	# RETURNS: the Data removed
+	def KeepOnlyDataBy(this, datumAttribute, toKeep):
+		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
+		# toRem = []
+		# for d in this.class:
+		#	 shouldRem = False
+		#	 for k in toKeep:
+		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
+		#			 logging.debug(f"found {k} in {d.__dict__}")
+		#			 shouldRem = True
+		#			 break
+		#	 if (shouldRem):
+		#		 toRem.append(d)
+		#	 else:
+		#		 logging.debug(f"{k} not found in {d.__dict__}")
+		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
+		return this.RemoveData(toRem)
 
-		if hasattr(logging, levelName):
-			raise AttributeError('{} already defined in logging module'.format(levelName))
-		if hasattr(logging, methodName):
-			raise AttributeError('{} already defined in logging module'.format(methodName))
-		if hasattr(logging.getLogger(), methodName):
-			raise AttributeError('{} already defined in logger class'.format(methodName))
 
-		# This method was inspired by the answers to Stack Overflow post
-		# http://stackoverflow.com/q/2183233/2988730, especially
-		# http://stackoverflow.com/a/13638084/2988730
-		def logForLevel(this, message, *args, **kwargs):
-			if this.isEnabledFor(value):
-				this._log(value, message, args, **kwargs)
-		def logToRoot(message, *args, **kwargs):
-			logging.log(value, message, *args, **kwargs)
+	# Removes all Data with the name "INVALID NAME"
+	# RETURNS: the removed Data
+	def RemoveAllUnlabeledData(this):
+		toRem = []
+		for d in this.data:
+			if (d.name =="INVALID NAME"):
+				toRem.append(d)
+		return this.RemoveData(toRem)
 
-		logging.addLevelName(value, levelName)
-		setattr(logging, levelName, value)
-		setattr(logging.getLogger(), methodName, logForLevel)
-		setattr(logging, methodName, logToRoot)
 
+	# Removes all invalid Data
+	# RETURNS: the removed Data
+	def RemoveAllInvalidData(this):
+		toRem = []
+		for d in this.data:
+			if (not d.IsValid()):
+				toRem.append(d)
+		return this.RemoveData(toRem)
+
+
+	# Removes all Data that have an attribute value relative to target.
+	# The given relation can be things like operator.le (i.e. <=)
+	#   See https://docs.python.org/3/library/operator.html for more info.
+	# If ignoreNames is specified, any Data of those names will be ignored.
+	# RETURNS: the Data removed
+	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
+		try:
+			toRem = []
+			for d in this.data:
+				if (ignoreNames and d.name in ignoreNames):
+					continue
+				if (relation(util.GetAttr(d, datumAttribute), target)):
+					toRem.append(d)
+			return this.RemoveData(toRem)
+		except Exception as e:
+			logging.error(f"{this.name} - {e.message}")
+			return []
+
+
+	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
+	# RETURNS: The Data removed
+	def RemoveDuplicateDataOf(this, datumAttribute):
+		toRem = [] # list of Data
+		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
+		for d1 in this.data:
+			skip = False
+			for dp in alreadyProcessed:
+				if (str(util.GetAttr(d1, datumAttribute)) == dp):
+					skip = True
+					break
+			if (skip):
+				continue
+			for d2 in this.data:
+				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
+					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
+					toRem.append(d2)
+					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
+		return this.RemoveData(toRem)
+
+
+	# Adds all Data from otherDataContainer to *this.
+	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
+	# RETURNS: the Data removed, if any.
+	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
+		this.data.extend(otherDataContainer.data);
+		if (preventDuplicatesOf is not None):
+			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
+		return []
 
-jsonpickle.handlers.registry.register(util.DotDict, util.DotDictPickler)
 
 
 # FunctorTracker is a global singleton which keeps a record of all functors that are currently in the call stack.
 # Functors should add and remove themselves from this list when they are called.
 class FunctorTracker:
 	def __init__(this):
 		# Singletons man...
@@ -1060,26 +1219,198 @@
 		if (envVar is not None):
 			return envVar, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
 
-class FetchCallbackFunctor(Functor):
+def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
+	raise MethodPendingPopulation("METHOD PENDING POPULATION")
 
-	def __init__(this, name = "FetchCallbackFunctor"):
+# Use the @method() decorator to turn any class function into an eons Method Functor.
+# Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
+# Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
+# All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
+#
+# If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
+# Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
+# For example, to set whether or not the Method should be propagated, you can use @method(propagate=True).
+# This means, you can create a custom means of interpreting your code with your own feature set and still use this @method decorator.
+# Perhaps you'd like something along the lines of: @method(impl='MakeAwesome', awesomeness=10000).
+# NOTE: in order for impl to work, the implementation class must already be Registered (or this must be called from an appropriate @recoverable function).
+def method(impl='Method', **kwargs):
+
+	# Class decorator with __set_name__, as described here: https://stackoverflow.com/questions/2366713/can-a-decorator-of-an-instance-method-access-the-class
+	class MethodDecorator:
+		def __init__(this, function):
+			this.function = function
+
+		# Apparently, this is called when the decorated function is constructed.
+		def __set_name__(this, cls, functionName):
+			logging.debug(f"Constructing new method for {this.function} in {cls}")
+
+			# Create and configure a new Method
+
+			method = SelfRegistering(impl)
+			method.Constructor(this.function, cls)
+			for key, value in kwargs.items():
+				setattr(method, key, value)
+
+			# Store the new method in the class
+			# There is a potential bug here: if the class derives from a class which already has the classMethods static member, this will add to the PARENT class's classMethods. Thus, 2 classes with different methods will share those methods via their shared parent.
+			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
+				cls.classMethods = {}
+			else:
+				# to account for the bug above, shadow classMethods out of the base class & into the derived.
+				setattr(cls, 'classMethods', getattr(cls, 'classMethods').copy())
+			
+			cls.classMethods[functionName] = method
+
+			# Self-destruct by replacing the decorated function.
+			# We rely on Functor.PopulateMethods to re-establish the method as callable.
+			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
+			# Regardless deleting the method is okay as long as we add it back before anyone notices.
+			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
+
+	return MethodDecorator
+
+class Method(Functor):
+
+	def __init__(this, name=INVALID_NAME()):
 		super().__init__(name)
 
-		this.requiredKWArgs.append('varName')
-		this.requiredKWArgs.append('location')
-		this.requiredKWArgs.append('value')
+		# Methods do not fetch from the environment by default.
+		this.fetchFrom.remove('environment')
+
+		# Whether or not *this should be combined with other Methods of the same name.
+		this.inheritMethods = True
+
+		# Where should inherited methods be inserted?
+		# First here means "before *this".
+		# If False, inherited code will be run after *this.
+		this.inheritedMethodsFirst = True # otherwise ...Last
 
+		# Propagation allows for Functors called after that which defines *this to also call *this.
+		# This system allows for partial, implicit inheritance.
+		# By default, Methods will not be propagated. Use @propagate to enable propagation.
+		this.propagate = False
+
+		# We don't care about these checks right now.
+		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
 		this.functionSucceeded = True
+		this.rollbackSucceeded = True
 		this.enableRollback = False
 
+		# The source code of the function we're implementing.
+		this.source = ""
+
+		# The instance of the class to which *this belongs.
+		# i.e. the object that called *this, aka 'owner', 'caller', etc.
+		this.object = None
+
+		this.original = util.DotDict()
+		this.original.cls = None
+		this.original.function = None
+
+
+	# Make *this execute the code in this.source
+	def UpdateSource(this):
+		wrappedFunctionName = f'_eons_method_{this.name}'
+		completeSource = f'''\
+def {wrappedFunctionName}(this):
+{this.source}
+'''
+		if (this.executor and this.executor.verbosity > 3):
+			logging.debug(f"Source for {this.name} is:\n{completeSource}")
+		code = compile(completeSource, '', 'exec')
+		exec(code)
+		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
+
+
+
+	# Parse arguments and update the source code
+	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
+	def PopulateFrom(this, function):
+		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
+
+		args = inspect.signature(function, follow_wrapped=False).parameters
+		thisSymbol = next(iter(args))
+		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
+		this.source = this.source.replace(thisSymbol, 'this.object')
+
+		first = True
+		for arg in args.values(): #args.values[1:] also doesn't work.
+			if (first):
+				first = False
+				continue
+
+			replaceWith = arg.name
+
+			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
+				replaceWith = 'this.args'
+
+			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
+				replaceWith = 'this.kwargs'
+
+			else:
+				if (arg.default != inspect.Parameter.empty):
+					this.optionalKWArgs[arg.name] = arg.default
+				else:
+					this.requiredKWArgs.append(arg.name)
+				replaceWith = f'this.{arg.name}'
+
+				if (arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]):
+					this.argMapping.append(arg.name)
+
+			this.source = this.source.replace(arg.name, replaceWith)
+
+
+	# When properly constructing a Method, rely only on the function *this should implement.
+	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
+	def Constructor(this, function, cls):
+		this.name = function.__name__
+		this.original.cls = cls
+		this.original.function = function
+
+		this.PopulateFrom(function)
+		
+		# UpdateSource is called by Functor.PopulateMethods()
+		# this.UpdateSource()
+
+
+	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
+	def PopulatePrecursor(this):
+		if (not this.object):
+			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
+
+		this.executor = this.object.executor
+
+		if ('precursor' in this.kwargs):
+			this.precursor = this.kwargs.pop('precursor')
+		else:
+			this.precursor = None
+
+
+	# Next is set by Functor.PopulateMethods.
+	# We  definitely don't want to Fetch 'next'.
+	def PopulateNext(this):
+		pass
+
+
+	# Method.next should be a list of other Methods, as opposed to the standard string; so, instead of Executor.Execute..., we can directly invoke whatever is next.
+	# We skip all validation here.
+	# We also don't pass any args that were given in the initial function call. Those can all be Fetched from 'precursor'.
+	def CallNext(this):
+		if (not this.next):
+			return None
+
+		for next in this.next:
+			next(precursor=this)
+
+
 # ExecutorTracker is a global singleton which keeps a record of all Executors that have been launched.
 # This can be abused quite a bit, so please try to restrict usage of this to only:
 # * Ease of use global functions
 #
 # Thanks! 
 class ExecutorTracker:
 	def __init__(this):
@@ -1122,171 +1453,143 @@
 			pass
 
 	@staticmethod
 	def GetLatest():
 		return ExecutorTracker.Instance().executors[-1]
 
 
-# A DataContainer allows Data to be stored and worked with.
-# This class is intended to be derived from and added to.
-# Each DataContainer is comprised of multiple Data (see Datum.py for more).
-# NOTE: DataContainers are, themselves Data. Thus, you can nest your child classes however you would like.
-class DataContainer(Datum):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# The data *this contains.
-		this.data = []
-
-
-	# RETURNS: an empty, invalid Datum.
-	def InvalidDatum(this):
-		ret = Datum()
-		ret.Invalidate()
-		return ret
-
-
-	# Sort things! Requires by be a valid attribute of all Data.
-	def SortData(this, by):
-		this.data.sort(key=operator.attrgetter(by))
-
-
-	# Adds a Datum to *this
-	def AddDatum(this, datum):
-		this.data.append(datum)
-
-
-	# RETURNS: a Datum with datumAttribute equal to match, an invalid Datum if none found.
-	def GetDatumBy(this, datumAttribute, match):
-		for d in this.data:
-			try: # within for loop 'cause maybe there's an issue with only 1 Datum and the rest are fine.
-				if (str(util.GetAttr(d, datumAttribute)) == str(match)):
-					return d
-			except Exception as e:
-				logging.error(f"{this.name} - {e.message}")
-				continue
-		return this.InvalidDatum()
-
-
-	# RETURNS: a Datum of the given name, an invalid Datum if none found.
-	def GetDatum(this, name):
-		return this.GetDatumBy('name', name)
-
-
-	# Removes all Data in toRem from *this.
-	# RETURNS: the Data removed
-	def RemoveData(this, toRem):
-		# logging.debug(f"Removing {toRem}")
-		this.data = [d for d in this.data if d not in toRem]
-		return toRem
+# Global Fetch() function.
+# Uses the latest registered Executor
+def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
 
+# Ease-of-use wrapper for the global Fetch()
+def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
+    Fetch(varName, default, fetchFrom, start, attempted)
 
-	# Removes all Data which match toRem along the given attribute
-	def RemoveDataBy(this, datumAttribute, toRem):
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) in list(map(str, toRem))]
-		return this.RemoveData(toRem)
+# The standard Functor extends Functor to add a set of standard members and methods.
+# This is similar to the standard library in C and C++
+# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
+class StandardFunctor(Functor):
+	def __init__(this, name="Standard Functor"):
+		super().__init__(name)
 
+	# Override this and do whatever!
+	# This is purposefully vague.
+	def Function(this):
+		pass
 
-	# Removes all Data in *this except toKeep.
-	# RETURNS: the Data removed
-	def KeepOnlyData(this, toKeep):
-		toRem = [d for d in this.data if d not in toKeep]
-		return this.RemoveData(toRem)
 
+	# Undo any changes made by UserFunction.
+	# Please override this too!
+	def Rollback(this):
+		pass
 
-	# Removes all Data except those that match toKeep along the given attribute
-	# RETURNS: the Data removed
-	def KeepOnlyDataBy(this, datumAttribute, toKeep):
-		# logging.debug(f"Keeping only class with a {datumAttribute} of {toKeep}")
-		# toRem = []
-		# for d in this.class:
-		#	 shouldRem = False
-		#	 for k in toKeep:
-		#		 if (str(util.GetAttr(d, datumAttribute)) == str(k)):
-		#			 logging.debug(f"found {k} in {d.__dict__}")
-		#			 shouldRem = True
-		#			 break
-		#	 if (shouldRem):
-		#		 toRem.append(d)
-		#	 else:
-		#		 logging.debug(f"{k} not found in {d.__dict__}")
-		toRem = [d for d in this.data if str(util.GetAttr(d, datumAttribute)) not in list(map(str, toKeep))]
-		return this.RemoveData(toRem)
 
+	# Override this to check results of operation and report on status.
+	# Override this to perform whatever success checks are necessary.
+	def DidFunctionSucceed(this):
+		return this.functionSucceeded
 
-	# Removes all Data with the name "INVALID NAME"
-	# RETURNS: the removed Data
-	def RemoveAllUnlabeledData(this):
-		toRem = []
-		for d in this.data:
-			if (d.name =="INVALID NAME"):
-				toRem.append(d)
-		return this.RemoveData(toRem)
 
+	# RETURN whether or not the Rollback was successful.
+	# Override this to perform whatever success checks are necessary.
+	def DidRollbackSucceed(this):
+		return this.rollbackSucceeded
 
-	# Removes all invalid Data
-	# RETURNS: the removed Data
-	def RemoveAllInvalidData(this):
-		toRem = []
-		for d in this.data:
-			if (not d.IsValid()):
-				toRem.append(d)
-		return this.RemoveData(toRem)
 
+	######## START: UTILITIES ########
 
-	# Removes all Data that have an attribute value relative to target.
-	# The given relation can be things like operator.le (i.e. <=)
-	#   See https://docs.python.org/3/library/operator.html for more info.
-	# If ignoreNames is specified, any Data of those names will be ignored.
-	# RETURNS: the Data removed
-	def RemoveDataRelativeToTarget(this, datumAttribute, relation, target, ignoreNames = []):
-		try:
-			toRem = []
-			for d in this.data:
-				if (ignoreNames and d.name in ignoreNames):
-					continue
-				if (relation(util.GetAttr(d, datumAttribute), target)):
-					toRem.append(d)
-			return this.RemoveData(toRem)
-		except Exception as e:
-			logging.error(f"{this.name} - {e.message}")
-			return []
+	# RETURNS: an opened file object for writing.
+	# Creates the path if it does not exist.
+	@method()
+	def CreateFile(this, file, mode="w+"):
+		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
+		return open(file, mode)
 
+	# Copy a file or folder from source to destination.
+	# This really shouldn't be so hard...
+	# root allows us to interpret '/' as something other than the top of the filesystem.
+	@method()
+	def Copy(this, source, destination, root='/'):
+		if (source.startswith('/')):
+			source = str(Path(root).joinpath(source[1:]).resolve())
+		else:
+			source = str(Path(source).resolve())
+		
+		destination = str(Path(destination).resolve())
+		
+		Path(destination).parent.mkdir(parents=True, exist_ok=True)
 
-	# Removes any Data that have the same datumAttribute as a previous Datum, keeping only the first.
-	# RETURNS: The Data removed
-	def RemoveDuplicateDataOf(this, datumAttribute):
-		toRem = [] # list of Data
-		alreadyProcessed = [] # list of strings, not whatever datumAttribute is.
-		for d1 in this.data:
-			skip = False
-			for dp in alreadyProcessed:
-				if (str(util.GetAttr(d1, datumAttribute)) == dp):
-					skip = True
-					break
-			if (skip):
-				continue
-			for d2 in this.data:
-				if (d1 is not d2 and str(util.GetAttr(d1, datumAttribute)) == str(util.GetAttr(d2, datumAttribute))):
-					logging.info(f"Removing duplicate Datum {d2} with unique id {util.GetAttr(d2, datumAttribute)}")
-					toRem.append(d2)
-					alreadyProcessed.append(str(util.GetAttr(d1, datumAttribute)))
-		return this.RemoveData(toRem)
+		if (os.path.isfile(source)):
+			logging.debug(f"Copying file {source} to {destination}")
+			try:
+				shutil.copy(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		elif (os.path.isdir(source)):
+			logging.debug(f"Copying directory {source} to {destination}")
+			try:
+				shutil.copytree(source, destination)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
+		else:
+			logging.error(f"Could not find source to copy: {source}")
 
+	# Delete a file or folder
+	@method()
+	def Delete(this, target):
+		if (not os.path.exists(target)):
+			logging.debug(f"Unable to delete nonexistent target: {target}")
+			return
+		if (os.path.isfile(target)):
+			logging.debug(f"Deleting file {target}")
+			os.remove(target)
+		elif (os.path.isdir(target)):
+			logging.debug(f"Deleting directory {target}")
+			try:
+				shutil.rmtree(target)
+			except shutil.Error as exc:
+				errors = exc.args[0]
+				for error in errors:
+					src, dst, msg = error
+					logging.debug(f"{msg}")
 
-	# Adds all Data from otherDataContainer to *this.
-	# If there are duplicate Data identified by the attribute preventDuplicatesOf, they are removed.
-	# RETURNS: the Data removed, if any.
-	def ImportDataFrom(this, otherDataContainer, preventDuplicatesOf=None):
-		this.data.extend(otherDataContainer.data);
-		if (preventDuplicatesOf is not None):
-			return this.RemoveDuplicateDataOf(preventDuplicatesOf)
-		return []
+	# Run whatever.
+	# DANGEROUS!!!!!
+	# RETURN: Return value and, optionally, the output as a list of lines.
+	@method()
+	def RunCommand(this, command, saveout=False, raiseExceptions=True):
+		logging.debug(f"================ Running command: {command} ================")
+		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
+		output = []
+		while process.poll() is None:
+			line = process.stdout.readline().decode('utf8')[:-1]
+			if (saveout):
+				output.append(line)
+			if (line):
+				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
 
+		message = f"Command returned {process.returncode}: {command}"
+		logging.debug(message)
+		if (raiseExceptions and process.returncode is not None and process.returncode):
+			raise CommandUnsuccessful(message)
+		
+		logging.debug(f"================ Completed command: {command} ================")
+		if (saveout):
+			return process.returncode, output
+		
+		return process.returncode
+	######## END: UTILITIES ########
 
 #from .Executor import Executor # don't import this, it'll be circular!
 
 # @recoverable
 # Decorating another function with this method will engage the error recovery system provided by *this.
 # To use this, you must define a GetExecutor() method in your class and decorate the functions you want to recover from.
 # For more info, see Executor.ResolveError and the README.md
@@ -1718,15 +2021,15 @@
 			this.RegisterAllClassesInDirectory(os.path.join(os.getcwd(), d))
 		this.RegisterAllClassesInDirectory(this.repo.store)
 
 
 	# Grok the configFile and populate this.config
 	def ParseConfigFile(this, configFile):
 		if (this.configType in ['py']):
-			this.RegisterAllClassesInDirectory(Path('./').joinpath('/'.join(this.parsedArgs.config.split['/'][:-1])))
+			this.RegisterAllClassesInDirectory(Path('./').joinpath('/'.join(this.parsedArgs.config.split('/')[:-1])))
 			functor = SelfRegistering(this.parsedArgs.config.split('/')[-1].split('.')[0])
 			this.config = functor(executor=this)
 		elif (this.configType in ['json', 'yml', 'yaml']):
 			# Yaml doesn't allow tabs. We do. Convert.
 			this.config = yaml.safe_load(configFile.read().replace('\t', '  '))
 		else:
 			raise ExecutorSetupError(f"Unknown configuration file type: {this.configType}")
@@ -2140,329 +2443,14 @@
 			if (key == varName):
 				return val, True
 		return default, False
 
 	######## END: Fetch Locations ########
 
 
-# Global Fetch() function.
-# Uses the latest registered Executor
-def Fetch(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    return ExecutorTracker.GetLatest().Fetch(varName, default, fetchFrom, start, attempted)
-
-# Ease-of-use wrapper for the global Fetch()
-def f(varName, default=None, fetchFrom=None, start=True, attempted=None):
-    Fetch(varName, default, fetchFrom, start, attempted)
-
-def METHOD_PENDING_POPULATION(obj, *args, **kwargs):
-	raise MethodPendingPopulation("METHOD PENDING POPULATION")
-
-# Use the @method() decorator to turn any class function into an eons Method Functor.
-# Methods are Functors which can be implicitly transferred between classes (see Functor.PopulateMethods)
-# Using Methods also gives us full control over the execution of your code; meaning, we can change how Python interprets what you wrote!
-# All Methods will be stored in the method member of your Functor. However, you shouldn't need to access that.
-#
-# If you would like to specify a custom implementation, set the 'impl' kwarg (e.g. @method(impl='MyMethodImplementation'))
-# Beside 'impl', all key-word arguments provided to the @method() decorator will be set as member variables of the created Method.
-# For example, to set whether or not the Method should be propagated, you can use @method(propagate=True).
-# This means, you can create a custom means of interpreting your code with your own feature set and still use this @method decorator.
-# Perhaps you'd like something along the lines of: @method(impl='MakeAwesome', awesomeness=10000).
-# NOTE: in order for impl to work, the implementation class must already be Registered (or this must be called from an appropriate @recoverable function).
-def method(impl='Method', **kwargs):
-
-	# Class decorator with __set_name__, as described here: https://stackoverflow.com/questions/2366713/can-a-decorator-of-an-instance-method-access-the-class
-	class MethodDecorator:
-		def __init__(this, function):
-			this.function = function
-
-		# Apparently, this is called when the decorated function is constructed.
-		def __set_name__(this, cls, functionName):
-			logging.debug(f"Constructing new method for {this.function} in {cls}")
-
-			# Create and configure a new Method
-
-			method = SelfRegistering(impl)
-			method.Constructor(this.function, cls)
-			for key, value in kwargs.items():
-				setattr(method, key, value)
-
-			# Store the new method in the class
-			# There is a potential bug here: if the class derives from a class which already has the classMethods static member, this will add to the PARENT class's classMethods. Thus, 2 classes with different methods will share those methods via their shared parent.
-			if (not hasattr(cls, 'classMethods') or not isinstance(cls.classMethods, dict)):
-				cls.classMethods = {}
-			else:
-				# to account for the bug above, shadow classMethods out of the base class & into the derived.
-				setattr(cls, 'classMethods', getattr(cls, 'classMethods').copy())
-			
-			cls.classMethods[functionName] = method
-
-			# Self-destruct by replacing the decorated function.
-			# We rely on Functor.PopulateMethods to re-establish the method as callable.
-			# It seems like this just outright removes the methods. There may be an issue with using __get__ this way.
-			# Regardless deleting the method is okay as long as we add it back before anyone notices.
-			setattr(cls, functionName, METHOD_PENDING_POPULATION.__get__(cls))
-
-	return MethodDecorator
-
-class Method(Functor):
-
-	def __init__(this, name=INVALID_NAME()):
-		super().__init__(name)
-
-		# Methods do not fetch from the environment by default.
-		this.fetchFrom.remove('environment')
-
-		# Whether or not *this should be combined with other Methods of the same name.
-		this.inheritMethods = True
-
-		# Where should inherited methods be inserted?
-		# First here means "before *this".
-		# If False, inherited code will be run after *this.
-		this.inheritedMethodsFirst = True # otherwise ...Last
-
-		# Propagation allows for Functors called after that which defines *this to also call *this.
-		# This system allows for partial, implicit inheritance.
-		# By default, Methods will not be propagated. Use @propagate to enable propagation.
-		this.propagate = False
-
-		# We don't care about these checks right now.
-		# Plus, we can't exactly wrap 2 functions even if we wanted to Rollback.
-		this.functionSucceeded = True
-		this.rollbackSucceeded = True
-		this.enableRollback = False
-
-		# The source code of the function we're implementing.
-		this.source = ""
-
-		# The instance of the class to which *this belongs.
-		# i.e. the object that called *this, aka 'owner', 'caller', etc.
-		this.object = None
-
-		this.original = util.DotDict()
-		this.original.cls = None
-		this.original.function = None
-
-
-	# Make *this execute the code in this.source
-	def UpdateSource(this):
-		wrappedFunctionName = f'_eons_method_{this.name}'
-		completeSource = f'''\
-def {wrappedFunctionName}(this):
-{this.source}
-'''
-		if (this.executor and this.executor.verbosity > 3):
-			logging.debug(f"Source for {this.name} is:\n{completeSource}")
-		code = compile(completeSource, '', 'exec')
-		exec(code)
-		exec(f'this.Function = {wrappedFunctionName}.__get__(this, this.__class__)')
-
-
-
-	# Parse arguments and update the source code
-	# TODO: Implement full python parser to avoid bad string replacement (e.g. "def func(self):... self.selfImprovement" => "... this.object.this.object.Improvement").
-	def PopulateFrom(this, function):
-		this.source = ':'.join(inspect.getsource(function).split(':')[1:]) #Remove the first function definition
-
-		args = inspect.signature(function, follow_wrapped=False).parameters
-		thisSymbol = next(iter(args))
-		#del args[thisSymbol] # ??? 'mappingproxy' object does not support item deletion
-		this.source = this.source.replace(thisSymbol, 'this.object')
-
-		first = True
-		for arg in args.values(): #args.values[1:] also doesn't work.
-			if (first):
-				first = False
-				continue
-
-			replaceWith = arg.name
-
-			if (arg.kind == inspect.Parameter.VAR_POSITIONAL):
-				replaceWith = 'this.args'
-
-			elif (arg.kind == inspect.Parameter.VAR_KEYWORD):
-				replaceWith = 'this.kwargs'
-
-			else:
-				if (arg.default != inspect.Parameter.empty):
-					this.optionalKWArgs[arg.name] = arg.default
-				else:
-					this.requiredKWArgs.append(arg.name)
-				replaceWith = f'this.{arg.name}'
-
-				if (arg.kind in [inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY]):
-					this.argMapping.append(arg.name)
-
-			this.source = this.source.replace(arg.name, replaceWith)
-
-
-	# When properly constructing a Method, rely only on the function *this should implement.
-	# The class and all other properties are irrelevant. However, they are provided and intended for debugging only.
-	def Constructor(this, function, cls):
-		this.name = function.__name__
-		this.original.cls = cls
-		this.original.function = function
-
-		this.PopulateFrom(function)
-		
-		# UpdateSource is called by Functor.PopulateMethods()
-		# this.UpdateSource()
-
-
-	# Grab any known and necessary args from this.kwargs before any Fetch calls are made.
-	def PopulatePrecursor(this):
-		if (not this.object):
-			raise MissingArgumentError(f"Call {this.name} from a class instance: {this.original.cls.__name__}.{this.name}(...). Maybe Functor.PopulateMethods() hasn't been called yet?")
-
-		this.executor = this.object.executor
-
-		if ('precursor' in this.kwargs):
-			this.precursor = this.kwargs.pop('precursor')
-		else:
-			this.precursor = None
-
-
-	# Next is set by Functor.PopulateMethods.
-	# We  definitely don't want to Fetch 'next'.
-	def PopulateNext(this):
-		pass
-
-
-	# Method.next should be a list of other Methods, as opposed to the standard string; so, instead of Executor.Execute..., we can directly invoke whatever is next.
-	# We skip all validation here.
-	# We also don't pass any args that were given in the initial function call. Those can all be Fetched from 'precursor'.
-	def CallNext(this):
-		if (not this.next):
-			return None
-
-		for next in this.next:
-			next(precursor=this)
-
-
-# The standard Functor extends Functor to add a set of standard members and methods.
-# This is similar to the standard library in C and C++
-# You must inherit from *this if you would like to use the functionality *this provides. The methods defined will not be propagated.
-class StandardFunctor(Functor):
-	def __init__(this, name="Standard Functor"):
-		super().__init__(name)
-
-	# Override this and do whatever!
-	# This is purposefully vague.
-	def Function(this):
-		pass
-
-
-	# Undo any changes made by UserFunction.
-	# Please override this too!
-	def Rollback(this):
-		pass
-
-
-	# Override this to check results of operation and report on status.
-	# Override this to perform whatever success checks are necessary.
-	def DidFunctionSucceed(this):
-		return this.functionSucceeded
-
-
-	# RETURN whether or not the Rollback was successful.
-	# Override this to perform whatever success checks are necessary.
-	def DidRollbackSucceed(this):
-		return this.rollbackSucceeded
-
-
-	######## START: UTILITIES ########
-
-	# RETURNS: an opened file object for writing.
-	# Creates the path if it does not exist.
-	@method()
-	def CreateFile(this, file, mode="w+"):
-		Path(os.path.dirname(os.path.abspath(file))).mkdir(parents=True, exist_ok=True)
-		return open(file, mode)
-
-	# Copy a file or folder from source to destination.
-	# This really shouldn't be so hard...
-	# root allows us to interpret '/' as something other than the top of the filesystem.
-	@method()
-	def Copy(this, source, destination, root='/'):
-		if (source.startswith('/')):
-			source = str(Path(root).joinpath(source[1:]).resolve())
-		else:
-			source = str(Path(source).resolve())
-		
-		destination = str(Path(destination).resolve())
-		
-		Path(destination).parent.mkdir(parents=True, exist_ok=True)
-
-		if (os.path.isfile(source)):
-			logging.debug(f"Copying file {source} to {destination}")
-			try:
-				shutil.copy(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		elif (os.path.isdir(source)):
-			logging.debug(f"Copying directory {source} to {destination}")
-			try:
-				shutil.copytree(source, destination)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-		else:
-			logging.error(f"Could not find source to copy: {source}")
-
-	# Delete a file or folder
-	@method()
-	def Delete(this, target):
-		if (not os.path.exists(target)):
-			logging.debug(f"Unable to delete nonexistent target: {target}")
-			return
-		if (os.path.isfile(target)):
-			logging.debug(f"Deleting file {target}")
-			os.remove(target)
-		elif (os.path.isdir(target)):
-			logging.debug(f"Deleting directory {target}")
-			try:
-				shutil.rmtree(target)
-			except shutil.Error as exc:
-				errors = exc.args[0]
-				for error in errors:
-					src, dst, msg = error
-					logging.debug(f"{msg}")
-
-	# Run whatever.
-	# DANGEROUS!!!!!
-	# RETURN: Return value and, optionally, the output as a list of lines.
-	@method()
-	def RunCommand(this, command, saveout=False, raiseExceptions=True):
-		logging.debug(f"================ Running command: {command} ================")
-		process = Popen(command, stdout=PIPE, stderr=STDOUT, shell=True)
-		output = []
-		while process.poll() is None:
-			line = process.stdout.readline().decode('utf8')[:-1]
-			if (saveout):
-				output.append(line)
-			if (line):
-				logging.debug(f"| {line}")  # [:-1] to strip excessive new lines.
-
-		message = f"Command returned {process.returncode}: {command}"
-		logging.debug(message)
-		if (raiseExceptions and process.returncode is not None and process.returncode):
-			raise CommandUnsuccessful(message)
-		
-		logging.debug(f"================ Completed command: {command} ================")
-		if (saveout):
-			return process.returncode, output
-		
-		return process.returncode
-	######## END: UTILITIES ########
-
-
 # Use an ErrorStringParser for each "parsers" in order to avoid having to override the GetObjectFromError method and create a new class for every error you want to handle.
 # ErrorStringParsers enable ErrorResolutions to be created on a per-functionality, rather than per-error basis, reducing the total amount of duplicate code.
 # Each error has a different string. In order to get the object of the error, we have to know where the object starts and ends.
 # NOTE: this assumes only 1 object per string. Maybe fancier parsing logic can be added in the future.
 #
 # startPosition is always positive
 # endPosition is always negative
@@ -2607,7 +2595,19 @@
 			logging.error(f"Error resolution with {this.name} failed: {e}")
 			util.LogStack()
 			this.functionSucceeded = False
 		
 		this.errorResolutionStack[this.errorString].append(this.name)
 		return this.errorResolutionStack, this.errorShouldBeResolved
 
+
+class FetchCallbackFunctor(Functor):
+
+	def __init__(this, name = "FetchCallbackFunctor"):
+		super().__init__(name)
+
+		this.requiredKWArgs.append('varName')
+		this.requiredKWArgs.append('location')
+		this.requiredKWArgs.append('value')
+
+		this.functionSucceeded = True
+		this.enableRollback = False
```

### Comparing `eons-2.6.4/pkg/eons/method/External.py` & `eons-2.6.5/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.4/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.6.5/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.4/pkg/eons/resolve/resolve_import_module.py` & `eons-2.6.5/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.4/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.6.5/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.6.4/pkg/eons.egg-info/PKG-INFO` & `eons-2.6.5/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.6.4
+Version: 2.6.5
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.6.4/pkg/eons.egg-info/SOURCES.txt` & `eons-2.6.5/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.6.4/setup.cfg` & `eons-2.6.5/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.6.4
+version = 2.6.5
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,20 +18,20 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
+	pyyaml
+	requests_futures
+	requests
 	jsonpickle
 	eot
-	requests
-	pyyaml
 	tqdm
-	requests_futures
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

