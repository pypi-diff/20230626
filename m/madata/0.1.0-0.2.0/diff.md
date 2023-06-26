# Comparing `tmp/madata-0.1.0.tar.gz` & `tmp/madata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/teddy/Documents/madata/dist/.tmp-feq9r_8f/madata-0.1.0.tar", last modified: Thu Jun 22 14:14:02 2023, max compression
+gzip compressed data, was "/Users/teddy/Documents/madata/dist/.tmp-j6xdopt8/madata-0.2.0.tar", last modified: Mon Jun 26 13:59:44 2023, max compression
```

## Comparing `madata-0.1.0.tar` & `madata-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 teddy      (502) staff       (20)        0 2023-06-22 14:14:02.000000 madata-0.1.0/
--rw-r--r--   0 teddy      (502) staff       (20)     1072 2023-06-12 09:50:02.000000 madata-0.1.0/LICENSE
--rw-r--r--   0 teddy      (502) staff       (20)     2143 2023-06-22 14:14:02.000000 madata-0.1.0/PKG-INFO
--rw-r--r--   0 teddy      (502) staff       (20)     1699 2023-06-22 13:28:04.000000 madata-0.1.0/README.md
-drwxr-xr-x   0 teddy      (502) staff       (20)        0 2023-06-22 14:14:02.000000 madata-0.1.0/madata/
--rw-r--r--   0 teddy      (502) staff       (20)       30 2023-06-22 13:31:08.000000 madata-0.1.0/madata/__init__.py
--rw-r--r--   0 teddy      (502) staff       (20)    10107 2023-06-22 14:00:02.000000 madata-0.1.0/madata/metadata.py
-drwxr-xr-x   0 teddy      (502) staff       (20)        0 2023-06-22 14:14:02.000000 madata-0.1.0/madata.egg-info/
--rw-r--r--   0 teddy      (502) staff       (20)     2143 2023-06-22 14:14:02.000000 madata-0.1.0/madata.egg-info/PKG-INFO
--rw-r--r--   0 teddy      (502) staff       (20)      228 2023-06-22 14:14:02.000000 madata-0.1.0/madata.egg-info/SOURCES.txt
--rw-r--r--   0 teddy      (502) staff       (20)        1 2023-06-22 14:14:02.000000 madata-0.1.0/madata.egg-info/dependency_links.txt
--rw-r--r--   0 teddy      (502) staff       (20)       73 2023-06-22 14:14:02.000000 madata-0.1.0/madata.egg-info/requires.txt
--rw-r--r--   0 teddy      (502) staff       (20)        7 2023-06-22 14:14:02.000000 madata-0.1.0/madata.egg-info/top_level.txt
--rw-r--r--   0 teddy      (502) staff       (20)       87 2023-06-22 13:34:13.000000 madata-0.1.0/pyproject.toml
--rw-r--r--   0 teddy      (502) staff       (20)       38 2023-06-22 14:14:02.000000 madata-0.1.0/setup.cfg
--rw-r--r--   0 teddy      (502) staff       (20)      802 2023-06-22 13:54:08.000000 madata-0.1.0/setup.py
+drwxr-xr-x   0 teddy      (502) staff       (20)        0 2023-06-26 13:59:44.000000 madata-0.2.0/
+-rw-r--r--   0 teddy      (502) staff       (20)     1072 2023-06-12 09:50:02.000000 madata-0.2.0/LICENSE
+-rw-r--r--   0 teddy      (502) staff       (20)     2340 2023-06-26 13:59:44.000000 madata-0.2.0/PKG-INFO
+-rw-r--r--   0 teddy      (502) staff       (20)     1896 2023-06-23 09:26:41.000000 madata-0.2.0/README.md
+drwxr-xr-x   0 teddy      (502) staff       (20)        0 2023-06-26 13:59:44.000000 madata-0.2.0/madata/
+-rw-r--r--   0 teddy      (502) staff       (20)       31 2023-06-26 11:52:03.000000 madata-0.2.0/madata/__init__.py
+-rw-r--r--   0 teddy      (502) staff       (20)    10345 2023-06-26 13:53:56.000000 madata-0.2.0/madata/metadata.py
+drwxr-xr-x   0 teddy      (502) staff       (20)        0 2023-06-26 13:59:44.000000 madata-0.2.0/madata.egg-info/
+-rw-r--r--   0 teddy      (502) staff       (20)     2340 2023-06-26 13:59:44.000000 madata-0.2.0/madata.egg-info/PKG-INFO
+-rw-r--r--   0 teddy      (502) staff       (20)      228 2023-06-26 13:59:44.000000 madata-0.2.0/madata.egg-info/SOURCES.txt
+-rw-r--r--   0 teddy      (502) staff       (20)        1 2023-06-26 13:59:44.000000 madata-0.2.0/madata.egg-info/dependency_links.txt
+-rw-r--r--   0 teddy      (502) staff       (20)       73 2023-06-26 13:59:44.000000 madata-0.2.0/madata.egg-info/requires.txt
+-rw-r--r--   0 teddy      (502) staff       (20)        7 2023-06-26 13:59:44.000000 madata-0.2.0/madata.egg-info/top_level.txt
+-rw-r--r--   0 teddy      (502) staff       (20)       87 2023-06-22 13:34:13.000000 madata-0.2.0/pyproject.toml
+-rw-r--r--   0 teddy      (502) staff       (20)       38 2023-06-26 13:59:44.000000 madata-0.2.0/setup.cfg
+-rw-r--r--   0 teddy      (502) staff       (20)      802 2023-06-26 13:56:14.000000 madata-0.2.0/setup.py
```

### Comparing `madata-0.1.0/LICENSE` & `madata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `madata-0.1.0/PKG-INFO` & `madata-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: madata
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool for syncing the dataset-metadata between MADATA and Wikidata
 Home-page: https://github.com/UB-Mannheim/madata
 Author: Renat Shigapov
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # madata
 
+[![PyPI version](https://badge.fury.io/py/madata.svg)](https://badge.fury.io/py/madata)
+
 `madata` syncs the metadata of datasets between [MADATA](https://madata.bib.uni-mannheim.de) (Mannheim Data Repository) and [Wikidata](https://www.wikidata.org). It provides access to the MADATA metadata records directly in Python.
 
 ## Table of contents
 * [Installation](#installation)
 * [Initialization](#initialization)
 * [Syncing](#syncing)
+* [SPARQL queries](#sparql-queries)
 
 ## Installation
 
 ```
 pip install madata
 ```
 
@@ -60,7 +63,11 @@
 records = Metadata()
 records._sync()
 >>> Wikidata username: 
 >>> Wikidata password: 
 ```
 
 Type your username and password, then `madata` starts to sync the metadata records at MADATA and Wikidata.
+
+## SPARQL queries
+
+The MADATA-subset at Wikidata: https://w.wiki/6s7R.
```

### Comparing `madata-0.1.0/README.md` & `madata-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # madata
 
+[![PyPI version](https://badge.fury.io/py/madata.svg)](https://badge.fury.io/py/madata)
+
 `madata` syncs the metadata of datasets between [MADATA](https://madata.bib.uni-mannheim.de) (Mannheim Data Repository) and [Wikidata](https://www.wikidata.org). It provides access to the MADATA metadata records directly in Python.
 
 ## Table of contents
 * [Installation](#installation)
 * [Initialization](#initialization)
 * [Syncing](#syncing)
+* [SPARQL queries](#sparql-queries)
 
 ## Installation
 
 ```
 pip install madata
 ```
 
@@ -46,7 +49,11 @@
 records = Metadata()
 records._sync()
 >>> Wikidata username: 
 >>> Wikidata password: 
 ```
 
 Type your username and password, then `madata` starts to sync the metadata records at MADATA and Wikidata.
+
+## SPARQL queries
+
+The MADATA-subset at Wikidata: https://w.wiki/6s7R.
```

### Comparing `madata-0.1.0/madata/metadata.py` & `madata-0.2.0/madata/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         """
         WDUSER = getpass(prompt="Wikidata username: ")
         WDPASS = getpass(prompt="Wikidata password: ")
         login = wdi_login.WDLogin(WDUSER, WDPASS)
 
         for index, row in tqdm(self.OAI_DC_df.iterrows()):
             MADATA_URL, DOI = row.relation
-            if DOI not in list(self.QID_DOI_URL.DOI):
+            if MADATA_URL not in list(self.QID_DOI_URL.URL):
                 creators = [self.reorder(c).strip() for c in row.creator]
                 data = [wdi_core.WDItemID('Q1172284', prop_nr='P31'), # instance of dataset
                         wdi_core.WDMonolingualText(row.title[0].strip(), prop_nr='P1476')] # title
                 for i, creator in enumerate(creators):
                     qualifiers = [wdi_core.WDString(str(i + 1), prop_nr='P1545', is_qualifier=True)]
                     data.append(
                         wdi_core.WDString(creator, prop_nr='P2093', qualifiers=qualifiers))  # author name string
@@ -144,15 +144,16 @@
                         if language == 'eng':
                             data.append(wdi_core.WDItemID('Q1860', prop_nr='P407'))
                         if language == 'ger':
                             data.append(wdi_core.WDItemID('Q188', prop_nr='P407'))
                         if language == 'fre':
                             data.append(wdi_core.WDItemID('Q150', prop_nr='P407'))
                 if row.description:
-                    data.append(wdi_core.WDMonolingualText(row.description[0].strip(), prop_nr='P7535')) # scope and content for abstract
+                    abstract = row.description[0][0:1500].strip() # Wikidata allow only 1500 symbols
+                    data.append(wdi_core.WDMonolingualText(abstract, prop_nr='P7535')) # scope and content for abstract
                 if row.get('rights'):
                     rights = list(set(row.rights))
                     for right in rights:
                         if right == 'cc0':
                             data.append(wdi_core.WDItemID('Q6938433', prop_nr='P275'))
                         if right == 'cc_by_nc_sa':  # Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported
                             data.append(wdi_core.WDItemID('Q15643954', prop_nr='P275'))
@@ -176,14 +177,17 @@
                 if row.get('identifier'):
                     for ident in row.identifier:
                         if ident.startswith('https://madata'):
                             data.append(wdi_core.WDUrl(ident, prop_nr='P4945'))  # download link
                 if row.get('ubma_url_external'):
                     for URLext in row.get('ubma_url_external'):
                         data.append(wdi_core.WDUrl(URLext, prop_nr='P973'))  # described at
-                wd_item = wdi_core.WDItemEngine(data=data)
-                wd_item.set_label(label=row.title[0].strip())  # set label
-                if row.get('ubma_additional_title'):
-                    wd_item.set_description(description=row.ubma_additional_title[0].strip())  # set description
-                wd_item.write(login, bot_account=False)
+                try:
+                    wd_item = wdi_core.WDItemEngine(data=data)
+                    wd_item.set_label(label=row.title[0].strip())  # set label
+                    if row.get('ubma_additional_title'):
+                        wd_item.set_description(description=row.ubma_additional_title[0].strip())  # set description
+                    wd_item.write(login, bot_account=False)
+                except Exception as e:
+                    print(e)
             else:
-                print('DOI: ' + DOI + ' is already at Wikidata.')
+                print('DOI: ' + DOI + ' is already at Wikidata for the MADATA record at: ' + MADATA_URL)
```

### Comparing `madata-0.1.0/madata.egg-info/PKG-INFO` & `madata-0.2.0/madata.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: madata
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool for syncing the dataset-metadata between MADATA and Wikidata
 Home-page: https://github.com/UB-Mannheim/madata
 Author: Renat Shigapov
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # madata
 
+[![PyPI version](https://badge.fury.io/py/madata.svg)](https://badge.fury.io/py/madata)
+
 `madata` syncs the metadata of datasets between [MADATA](https://madata.bib.uni-mannheim.de) (Mannheim Data Repository) and [Wikidata](https://www.wikidata.org). It provides access to the MADATA metadata records directly in Python.
 
 ## Table of contents
 * [Installation](#installation)
 * [Initialization](#initialization)
 * [Syncing](#syncing)
+* [SPARQL queries](#sparql-queries)
 
 ## Installation
 
 ```
 pip install madata
 ```
 
@@ -60,7 +63,11 @@
 records = Metadata()
 records._sync()
 >>> Wikidata username: 
 >>> Wikidata password: 
 ```
 
 Type your username and password, then `madata` starts to sync the metadata records at MADATA and Wikidata.
+
+## SPARQL queries
+
+The MADATA-subset at Wikidata: https://w.wiki/6s7R.
```

### Comparing `madata-0.1.0/setup.py` & `madata-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="madata",
-    version='0.1.0',
+    version='0.2.0',
     author="Renat Shigapov",
     license="MIT",
     description="A tool for syncing the dataset-metadata between MADATA and Wikidata",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/UB-Mannheim/madata",
     install_requires=['sickle', 'pandas', 'requests', 'wikidataintegrator', 'tqdm', 'appengine-python-standard'],
```

