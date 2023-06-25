# Comparing `tmp/asBASE-0.4.tar.gz` & `tmp/asBASE-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asBASE-0.4.tar", last modified: Thu Jun  8 23:35:50 2023, max compression
+gzip compressed data, was "asBASE-0.5.tar", last modified: Sun Jun 25 22:42:16 2023, max compression
```

## Comparing `asBASE-0.4.tar` & `asBASE-0.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 23:35:50.681495 asBASE-0.4/
--rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-26 23:55:19.000000 asBASE-0.4/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)      320 2023-06-08 23:35:50.669495 asBASE-0.4/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      818 2023-05-27 00:54:02.000000 asBASE-0.4/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 23:35:50.581495 asBASE-0.4/asBASE/
--rw-rw----   0 root         (0) everybody  (9997)     2611 2023-06-08 23:34:26.000000 asBASE-0.4/asBASE/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-08 23:35:50.649495 asBASE-0.4/asBASE.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)      320 2023-06-08 23:35:50.000000 asBASE-0.4/asBASE.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      169 2023-06-08 23:35:50.000000 asBASE-0.4/asBASE.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-08 23:35:50.000000 asBASE-0.4/asBASE.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)        7 2023-06-08 23:35:50.000000 asBASE-0.4/asBASE.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-08 23:35:50.681495 asBASE-0.4/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      361 2023-06-08 23:35:35.000000 asBASE-0.4/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-25 22:42:16.924512 asBASE-0.5/
+-rw-rw----   0 root         (0) everybody  (9997)       20 2023-05-26 23:55:19.000000 asBASE-0.5/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)      320 2023-06-25 22:42:16.912512 asBASE-0.5/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-25 22:42:16.820512 asBASE-0.5/asBASE/
+-rw-rw----   0 root         (0) everybody  (9997)     2621 2023-06-25 22:41:49.000000 asBASE-0.5/asBASE/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-06-25 22:42:16.896512 asBASE-0.5/asBASE.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      320 2023-06-25 22:42:16.000000 asBASE-0.5/asBASE.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      159 2023-06-25 22:42:16.000000 asBASE-0.5/asBASE.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-06-25 22:42:16.000000 asBASE-0.5/asBASE.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)        7 2023-06-25 22:42:16.000000 asBASE-0.5/asBASE.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-06-25 22:42:16.928512 asBASE-0.5/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      361 2023-06-25 22:40:04.000000 asBASE-0.5/setup.py
```

### Comparing `asBASE-0.4/asBASE/__init__.py` & `asBASE-0.5/asBASE/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,10 +75,10 @@
 		try:
 			with open(self.filename, "r") as f:
 				json_str = f.read()
 				return json.loads(json_str)
 		except:
 			return {}
 	def write_json(self, json_dict):
-		json_str = json.dumps(json_dict)
+		json_str = json.dumps(json_dict, indent=4)
 		with open(self.filename, "w") as f:
 			f.write(json_str)
```

