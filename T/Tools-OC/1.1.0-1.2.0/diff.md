# Comparing `tmp/Tools-OC-1.1.0.tar.gz` & `tmp/Tools-OC-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tools-OC-1.1.0.tar", last modified: Mon May 29 10:55:59 2023, max compression
+gzip compressed data, was "Tools-OC-1.2.0.tar", last modified: Sun Jun 25 22:43:12 2023, max compression
```

## Comparing `Tools-OC-1.1.0.tar` & `Tools-OC-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/
--rw-rw-r--   0 bast      (1002) bast      (1002)     1078 2023-03-18 20:50:27.000000 Tools-OC-1.1.0/LICENSE
--rw-rw-r--   0 bast      (1002) bast      (1002)      604 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)       57 2023-03-18 20:50:27.000000 Tools-OC-1.1.0/README.md
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/Tools_OC.egg-info/
--rw-rw-r--   0 bast      (1002) bast      (1002)      604 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      258 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)       20 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/requires.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        6 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-03-18 21:13:36.000000 Tools-OC-1.1.0/Tools_OC.egg-info/zip-safe
--rw-rw-r--   0 bast      (1002) bast      (1002)       79 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/setup.cfg
--rw-rw-r--   0 bast      (1002) bast      (1002)      755 2023-05-29 10:55:32.000000 Tools-OC-1.1.0/setup.py
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/tools/
--rw-rw-r--   0 bast      (1002) bast      (1002)     9404 2023-05-29 10:55:32.000000 Tools-OC-1.1.0/tools/__init__.py
--rw-rw-r--   0 bast      (1002) bast      (1002)     1232 2023-05-29 10:55:32.000000 Tools-OC-1.1.0/tools/__main__.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-25 22:43:12.721048 Tools-OC-1.2.0/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1078 2023-03-18 20:50:27.000000 Tools-OC-1.2.0/LICENSE
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5408 2023-06-25 22:43:12.721048 Tools-OC-1.2.0/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)     4861 2023-06-24 22:13:06.000000 Tools-OC-1.2.0/README.md
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-25 22:43:12.721048 Tools-OC-1.2.0/Tools_OC.egg-info/
+-rw-rw-r--   0 bast      (1000) bast      (1000)     5408 2023-06-25 22:43:12.000000 Tools-OC-1.2.0/Tools_OC.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1000) bast      (1000)      258 2023-06-25 22:43:12.000000 Tools-OC-1.2.0/Tools_OC.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-06-25 22:43:12.000000 Tools-OC-1.2.0/Tools_OC.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)       20 2023-06-25 22:43:12.000000 Tools-OC-1.2.0/Tools_OC.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        6 2023-06-25 22:43:12.000000 Tools-OC-1.2.0/Tools_OC.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1000) bast      (1000)        1 2023-03-18 21:13:36.000000 Tools-OC-1.2.0/Tools_OC.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1000) bast      (1000)       79 2023-06-25 22:43:12.721048 Tools-OC-1.2.0/setup.cfg
+-rw-rw-r--   0 bast      (1000) bast      (1000)      755 2023-06-08 15:03:11.000000 Tools-OC-1.2.0/setup.py
+drwxrwxr-x   0 bast      (1000) bast      (1000)        0 2023-06-25 22:43:12.721048 Tools-OC-1.2.0/tools/
+-rw-rw-r--   0 bast      (1000) bast      (1000)    11117 2023-06-24 22:06:37.000000 Tools-OC-1.2.0/tools/__init__.py
+-rw-rw-r--   0 bast      (1000) bast      (1000)     1331 2023-06-24 22:06:35.000000 Tools-OC-1.2.0/tools/__main__.py
```

### Comparing `Tools-OC-1.1.0/LICENSE` & `Tools-OC-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Tools-OC-1.1.0/setup.py` & `Tools-OC-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='Tools-OC',
-	version='1.1.0',
+	version='1.2.0',
 	description='A set of tools for common python problems',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/ouroboroscoding/tools-python',
 	project_urls={
 		'Source': 'https://github.com/ouroboroscoding/tools-python',
 		'Tracker': 'https://github.com/ouroboroscoding/tools-python/issues'
```

### Comparing `Tools-OC-1.1.0/tools/__init__.py` & `Tools-OC-1.2.0/tools/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,40 +7,48 @@
 __author__		= "Chris Nasr"
 __copyright__	= "Ouroboros Coding Inc."
 __email__		= "chris@ouroboroscoding.com"
 __created__		= "2023-03-18"
 
 # Limit exports
 __all__ = [
-	'clone', 'combine', 'compare', 'eval', 'get_client_ip', 'keys_to_ints',
+	'clone', 'combine', 'compare', 'evaluate', 'get_client_ip', 'keys_to_ints',
 	'lfindi', 'lfindd', 'merge', 'without'
 ]
 
 # Python imports
 import sys
 
 # Pip imports
 from jobject import jobject
 
-def clone(src):
+def clone(src: dict) -> dict:
 	"""Clone
 
-	Goes through the dict and any child dicts copying the values so that we
+	Goes through the dict and any child dicts copying the values so that we \
 	don't have any references
 
 	Arguments:
 		src (dict): The source dict
 
+	Raises:
+		ValueError
+
 	Returns:
 		dict
 	"""
 
 	# Check the argument
 	if not isinstance(src, dict):
-		raise ValueError('%s is not a valid value for src argument of %s' % (str(src), sys._getframe().f_code.co_name))
+		raise ValueError(
+			'%s is not a valid value for src argument of %s' % (
+				str(src),
+				sys._getframe().f_code.co_name
+			)
+		)
 
 	# Initialise the new dict
 	if isinstance(src, jobject):
 		dRet = jobject()
 	else:
 		dRet = {}
 
@@ -62,33 +70,43 @@
 		# Else it's a standard variable
 		else:
 			dRet[k] = src[k]
 
 	# Return the new dict
 	return dRet
 
-def combine(first, second):
+def combine(first: dict, second: dict) -> dict:
 	"""Combine
 
-	Generates a new dict by combining the two passed, values in second will
+	Generates a new dict by combining the two passed, values in second will \
 	overwrite values in first
 
 	Arguments:
 		first (dict): The dict to be changed/overwritten
 		second (dict): The dict that will do the overwriting
 
 	Returns:
 		dict
 	"""
 
 	# Make sure both arguments are actual dicts
 	if not isinstance(first, dict):
-		raise ValueError('%s is not a valid value for first of %s' % (str(first), sys._getframe().f_code.co_name))
+		raise ValueError(
+			'%s is not a valid value for first of %s' % (
+				str(first),
+				sys._getframe().f_code.co_name
+			)
+		)
 	if not isinstance(second, dict):
-		raise ValueError('%s is not a valid value for second of %s' % (str(second), sys._getframe().f_code.co_name))
+		raise ValueError(
+			'%s is not a valid value for second of %s' % (
+				str(second),
+				sys._getframe().f_code.co_name
+			)
+		)
 
 	# Copy the first dict
 	dRet = clone(first)
 
 	# Call merge to avoid duplicate code and return the cloned dict
 	return merge(dRet, second)
 
@@ -137,27 +155,27 @@
 	else:
 		if a != b:
 			return False
 
 	# Return equal
 	return True
 
-def eval(src, contains):
-	"""Eval(uate)
+def evaluate(src: dict, contains: list) -> None:
+	"""Evaluate
 
 	Goes through a dict looking for keys from `contains`
 
 	Arguments:
 		src (dict): The dict we are evaluating
-		contains (list): A list of values to check for, if the value is a dict
-			rather than a string, expects keys to be keys pointing to further
+		contains (list): A list of values to check for, if the value is a dict \
+			rather than a string, expects keys to be keys pointing to further \
 			lists of keys
 
-	Return:
-		list | None
+	Raises:
+		A ValueError with each arg being a key that is missing from the src
 	"""
 
 	# Initialise the list of errors
 	lErrs = []
 
 	# Go through each contains value
 	for s in contains:
@@ -179,34 +197,34 @@
 				if k not in src or not src[k]:
 					lErrs.append(k)
 
 				# Else, check the children
 				else:
 
 					# Call the eval on the child dict
-					lChildErrs = eval(src[k], v)
+					lChildErrs = evaluate(src[k], v)
 
 					# Add errors to the list
 					if lChildErrs:
 						for sErr in lChildErrs:
 							lErrs.append(k + '.' + sErr)
 
 		# We got an unknown type of key
 		else:
 			lErrs.append(str(s))
 
 	# If there's any errors
 	if lErrs:
 		raise ValueError(*lErrs)
 
-def get_client_ip(environ):
+def get_client_ip(environ: dict) -> str:
 	"""Get Client IP
 
-	Returns the IP of the client based on all the environment data passed to
-	the current webserver request
+	Returns the IP of the client based on all the environment data passed to \
+	the current webserver request, or whatever dict based value you pass to it
 
 	Arguments:
 		environ (dict): A dictionary of environment variables
 
 	Returns:
 		str
 	"""
@@ -230,32 +248,35 @@
 	if sIP.find(','):
 		lIPs = sIP.split(',')
 		sIP = lIPs[-1].strip()
 
 	# Return the IP
 	return sIP
 
-def keys_to_ints(src):
+def keys_to_ints(src: dict | list) -> dict | list:
 	"""Keys To Ints
 
-	Recursively goes through a dictionary and converts all keys that are
-	numeric but stored as strings to integers. Returns a new dict and doesn't
+	Recursively goes through a dictionary and converts all keys that are \
+	numeric but stored as strings to integers. Returns a new dict and doesn't \
 	alter the original.
 
-	PLEASE NOTE: this method is not useful for classes, or anything complex, it
-	is meant primarily for converting JSON objects which don't allow ints as
-	keys. Passing a set, tuple, or iterable class will not result in the
+	PLEASE NOTE: this method is not useful for classes, or anything complex, \
+	it is meant primarily for converting JSON objects which don't allow ints \
+	as keys. Passing a set, tuple, or iterable class will not result in the \
 	expected result
 
 	Arguments:
-		src (dict|list): The dict we are modifying, accepts lists in order to
-							handle recursive following the data
+		src (dict|list): The dict we are modifying, accepts lists in order to \
+							handle recursively following the data
+
+	Raises:
+		ValueError
 
 	Returns:
-		dict|list
+		dict | list
 	"""
 
 	# If we got a dict
 	if isinstance(src, dict):
 
 		# Init the return value to an empty dict
 		mRet = isinstance(src, jobject) and jobject() or {}
@@ -290,24 +311,29 @@
 
 			# Else, store as is
 			else:
 				mRet.append(src[k])
 
 	# Else, raise an error
 	else:
-		raise ValueError('src of %s must be a dict or list, received %s' % (sys._getframe().f_code.co_name, str(type(src))))
+		raise ValueError(
+			'src of %s must be a dict or list, received %s' % (
+				sys._getframe().f_code.co_name,
+				str(type(src))
+			)
+		)
 
 	# Return the new data
 	return mRet
 
 def lfindi(l: list, k: str, v: any) -> int:
 	"""List Find Index
 
-	Finds a specific dict in a list based on key name and value and returns its
-	index. Returns -1 on failure to find
+	Finds a specific dict in a list based on key name and value and returns \
+	its index. Returns -1 on failure to find
 
 	Arguments:
 		l (list): The list to search
 		k (str): The key to check in each dict
 		v (any): The value of the key
 
 	Returns:
@@ -317,70 +343,130 @@
 		if l[i][k] == v:
 			return i
 	return -1
 
 def lfindd(l: list, k: str, v: any) -> dict | None:
 	"""List Find Dictionary
 
-	Finds a specific dict in a list based on key name and value and returns it.
-	Returns None on failure to find
+	Finds a specific dict in a list based on key name and value and returns \
+	it. Returns None on failure to find
 
 	Arguments:
 		l (list): The list to search
 		k (str): The key to check in each dict
 		v (any): The value of the key
 
 	Returns:
 		dict | None
 	"""
 	for d in l:
 		if d[k] == v:
 			return d
 	return None
 
-def merge(first, second):
+def merge(
+	first: dict,
+	second: dict,
+	return_changes: bool = False
+) -> dict | None:
 	"""Merge
 
-	Overwrites the first dict by adding the values from the second. Returns the
-	first for chaining / ease of use
+	Overwrites the first dict by adding the values from the second. Returns \
+	the first for chaining / ease of use, unless return_changes is set to \
+	True, in which case, a dict of changes will be returned
 
 	Arguments:
 		first (dict): The dict to be changed/overwritten
 		second (dict): The dict that will do the overwriting
+		return_changes (bool): Optional, by default merge will not keep track \
+							of changes between the two dicts. If set to True, \
+							a dict of changes, possible empty, will be \
+							returned instead of the first argument
 
 	Returns:
-		dict
+		the first argument, or a dict of changes, or none for no changes
 	"""
 
+	# If we want changes
+	if return_changes:
+		dChanges = {}
+
 	# Make sure both arguments are actual dicts
 	if not isinstance(first, dict):
-		raise ValueError('%s is not a valid value for first of %s' % (str(first), sys._getframe().f_code.co_name))
+		raise ValueError(
+			'%s is not a valid value for first of %s' % (
+				str(first),
+				sys._getframe().f_code.co_name
+			)
+		)
 	if not isinstance(second, dict):
-		raise ValueError('%s is not a valid value for second of %s' % (str(second), sys._getframe().f_code.co_name))
+		raise ValueError(
+			'%s is not a valid value for second of %s' % (
+				str(second),
+				sys._getframe().f_code.co_name
+			)
+		)
 
-	# Get each key of the second dict
-	for m in second:
+	# If we want changes
+	if return_changes:
 
-		# If the value is another dict and it exists in first as well
-		if isinstance(second[m], dict) and m in first and isinstance(first[m], dict):
+		# Get each key of the second dict
+		for k in second:
 
-			# Call merge
-			merge(first[m], second[m])
+			# If the value is another dict and it exists in first as well
+			if isinstance(second[k], dict) and \
+				k in first and isinstance(first[k], dict):
 
-		# else we overwrite the value as is
-		else:
-			first[m] = second[m]
+				# Get the diff
+				dDiff = merge(first[k], second[k], True)
 
-	# Return the new dict
-	return first
+				# If there is any, add it to the changes
+				if dDiff:
+					dChanges[k] = dDiff
+
+			# else, if the key doesn't exist in the first, or there is a
+			#	difference between the keys
+			elif k not in first or first[k] != second[k]:
+
+				# Store the new value
+				first[k] = second[k]
+
+				# Set the changes
+				dChanges[k] = second[k]
+
+		# Return the changes or nothing
+		return dChanges or None
+
+	# Else, just call without changes
+	else:
+
+		# Get each key of the second dict
+		for k in second:
+
+			# If the value is another dict and it exists in first as well
+			if isinstance(second[k], dict) and \
+				k in first and isinstance(first[k], dict):
+
+				# Merge it
+				merge(first[k], second[k])
+
+			# else we overwrite the value as is
+			else:
+				first[k] = second[k]
+
+		# Return the existing first argument for chaining
+		return first
 
-def without(data: dict | list[dict], keys: str | list[str]) -> dict | list[dict]:
+def without(
+	data: dict | list[dict],
+	keys: str | list[str]
+) -> dict | list[dict]:
 	"""Without
 
-	Copies one or more dictionaries and returns them without the key or keys
+	Copies one or more dictionaries and returns them without the key or keys \
 	passed
 
 	Arguments:
 		data (dict | dict[]): The dictionary(s) to remove keys from
 		keys (str | str[]): The key or keys to remove
 
 	Returns:
```

### Comparing `Tools-OC-1.1.0/tools/__main__.py` & `Tools-OC-1.2.0/tools/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from jobject import jobject
 
 # Import everything
 from . import \
 	clone, \
 	combine, \
 	compare, \
-	eval, \
+	evaluate, \
 	get_client_ip, \
 	keys_to_ints, \
 	lfindi, \
 	lfindd, \
 	merge, \
 	without
 
@@ -40,16 +40,18 @@
 jo = combine(jo, {'four': '4'})
 
 print('compare & without')
 print('%s is True' % str(compare(without(o, ['4', '5']), _o)))
 print('%s is False' % str(compare(without(o, '4'), jo)))
 
 print('merge')
-merge(o, {'5': 'five'})
-merge(jo, {'five': '5'})
+print(merge(o, {'5': 'five'}))
+print(merge(jo, {'five': '5'}))
+print(merge(o, {'6': 'six'}, True))
+print(merge(o, {'5': 'five'}, True))
 
 print('keys_to_ints')
 print(keys_to_ints(o))
 print(keys_to_ints(jo))
 
 l = [{'key': 1}, {'key': 2}, {'key': 3}]
 print('lfindi')
@@ -57,17 +59,17 @@
 print('lfindd')
 print('{\'key\': 3} = %s' % str(lfindd(l, 'key', 3)))
 
 print(without(jo, 'four'))
 print(without(jo, ['four', 'five']))
 print(without([o, jo], ['4', '5', 'four', 'five']))
 
-print('eval')
+print('evaluate')
 try:
-	eval(o, [6, 7])
+	evaluate(o, [6, 7])
 except ValueError as e:
 	print(e.args)
 
 get_client_ip({})
 
 # If we got here, everything seems fine
 print('I work')
```

