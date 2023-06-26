# Comparing `tmp/pubmedparser2-2.0.0a0.tar.gz` & `tmp/pubmedparser2-2.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubmedparser2-2.0.0a0.tar", max compression
+gzip compressed data, was "pubmedparser2-2.0.1a0.tar", max compression
```

## Comparing `pubmedparser2-2.0.0a0.tar` & `pubmedparser2-2.0.1a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35080 2023-06-26 18:02:08.990802 pubmedparser2-2.0.0a0/LICENSE
--rw-r--r--   0        0        0     9558 2023-06-26 18:02:08.991802 pubmedparser2-2.0.0a0/README.md
--rw-r--r--   0        0        0     1840 2023-06-26 18:02:08.991802 pubmedparser2-2.0.0a0/build.py
--rw-r--r--   0        0        0     3294 2023-06-26 18:02:08.993802 pubmedparser2-2.0.0a0/pubmedparser/__init__.py
--rw-r--r--   0        0        0     6017 2023-06-26 18:02:08.993802 pubmedparser2-2.0.0a0/pubmedparser/_readxml.c
--rw-r--r--   0        0        0      380 2023-06-26 18:02:08.993802 pubmedparser2-2.0.0a0/pubmedparser/_readxml.pyi
--rw-r--r--   0        0        0     7502 2023-06-26 18:02:08.993802 pubmedparser2-2.0.0a0/pubmedparser/ftp.py
--rw-r--r--   0        0        0     3597 2023-06-26 18:02:08.994802 pubmedparser2-2.0.0a0/pubmedparser/storage.py
--rw-r--r--   0        0        0      952 2023-06-26 18:21:36.044829 pubmedparser2-2.0.0a0/pyproject.toml
--rw-r--r--   0        0        0    10604 1970-01-01 00:00:00.000000 pubmedparser2-2.0.0a0/setup.py
--rw-r--r--   0        0        0    10353 1970-01-01 00:00:00.000000 pubmedparser2-2.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0    35080 2023-06-26 18:02:08.990802 pubmedparser2-2.0.1a0/LICENSE
+-rw-r--r--   0        0        0     9636 2023-06-26 18:32:12.125914 pubmedparser2-2.0.1a0/README.md
+-rw-r--r--   0        0        0     1840 2023-06-26 18:02:08.991802 pubmedparser2-2.0.1a0/build.py
+-rw-r--r--   0        0        0     3294 2023-06-26 18:02:08.993802 pubmedparser2-2.0.1a0/pubmedparser/__init__.py
+-rw-r--r--   0        0        0     6017 2023-06-26 18:02:08.993802 pubmedparser2-2.0.1a0/pubmedparser/_readxml.c
+-rw-r--r--   0        0        0      380 2023-06-26 18:02:08.993802 pubmedparser2-2.0.1a0/pubmedparser/_readxml.pyi
+-rw-r--r--   0        0        0     7502 2023-06-26 18:02:08.993802 pubmedparser2-2.0.1a0/pubmedparser/ftp.py
+-rw-r--r--   0        0        0     3597 2023-06-26 18:02:08.994802 pubmedparser2-2.0.1a0/pubmedparser/storage.py
+-rw-r--r--   0        0        0      951 2023-06-26 18:32:12.127914 pubmedparser2-2.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0    10681 1970-01-01 00:00:00.000000 pubmedparser2-2.0.1a0/setup.py
+-rw-r--r--   0        0        0    10431 1970-01-01 00:00:00.000000 pubmedparser2-2.0.1a0/PKG-INFO
```

### Comparing `pubmedparser2-2.0.0a0/LICENSE` & `pubmedparser2-2.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pubmedparser2-2.0.0a0/README.md` & `pubmedparser2-2.0.1a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,7 @@
----
-author: David R. Connell
-title: Pubmed parser
----
-
 Read XML files and pull out selected values. Values to collect are
 determined by paths found in a [structure file](#structure-file). The
 structure file also includes a key which associates the values with a
 parent element and names, which determine which file to place the
 elements in.
 
 Files can be passed as either gzipped or uncompressed XML files or from
@@ -21,26 +16,30 @@
 xml_read --cache-dir=cache --structure-file=structure.yml \
     data/*.xml.gz
 ```
 
 Or, with python:
 
 ``` python
-import pubmedparser
-import pubmedparser.ftp
+import pubmedparser2
+import pubmedparser2.ftp
 
 # Download data
-files = pubmedparser.ftp.download(range(1, 6))
+files = pubmedparser2.ftp.download(range(1, 6))
 
 # Read XML files using a YAML file to describe what data to collect.
 data_dir = "file_example"
 structure_file = "example/structure.yml"
-results = pubmedparser.read_xml(files, structure_file, data_dir)
+results = pubmedparser2.read_xml(files, structure_file, data_dir)
 ```
 
+See [the example
+file](https://gitlab.com/net-synergy/pubmedparser/-/blob/master/example/creating_graphs.py)
+for more options.
+
 In python, the structure file can be replaced with a dictionary of
 dictionaries as well.
 
 ## Building CLI
 
 Requires `zlib`.
 
@@ -55,15 +54,15 @@
 ``` bash
 nix shell "gitlab:DavidRConnell/pubmedparser"
 ```
 
 ## Installing with pip
 
 ``` bash
-pip install pubmedparser
+pip install pubmedparser2
 ```
 
 # Structure file
 
 The structure file is a YAML file containing key-value pairs for
 different tags and paths. There are two required keys: `root` and `key`.
 `Root` provide the top-level tag, in the case of the pubmed files this
```

### Comparing `pubmedparser2-2.0.0a0/build.py` & `pubmedparser2-2.0.1a0/build.py`

 * *Files identical despite different names*

### Comparing `pubmedparser2-2.0.0a0/pubmedparser/__init__.py` & `pubmedparser2-2.0.1a0/pubmedparser/__init__.py`

 * *Files identical despite different names*

### Comparing `pubmedparser2-2.0.0a0/pubmedparser/_readxml.c` & `pubmedparser2-2.0.1a0/pubmedparser/_readxml.c`

 * *Files identical despite different names*

### Comparing `pubmedparser2-2.0.0a0/pubmedparser/ftp.py` & `pubmedparser2-2.0.1a0/pubmedparser/ftp.py`

 * *Files identical despite different names*

### Comparing `pubmedparser2-2.0.0a0/pubmedparser/storage.py` & `pubmedparser2-2.0.1a0/pubmedparser/storage.py`

 * *Files identical despite different names*

### Comparing `pubmedparser2-2.0.0a0/pyproject.toml` & `pubmedparser2-2.0.1a0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "pubmedparser2"
-version = "2.0.0-alpha"
+version = "2.0.1-alpha"
 description = "Download and parse pubmed publication data"
 license = "MIT"
-keywords = ["publication", "network", "MEDLINE", "PubMed", "References"]
+keywords = ["publication", "network", "MEDLINE", "PubMed", "references"]
 repository = "https://gitlab.com/net-synergy/pubmedparser"
 readme = "README.md"
 authors = ["David Connell <davidconnell12@gmail.com>"]
 maintainers = ["David Connell <davidconnell12@gmail.com>"]
 packages = [{ include = "pubmedparser" }]
 
 [tool.poetry.dependencies]
@@ -35,8 +35,8 @@
 
 [tool.poetry.build]
 script = "build.py"
 generate-setup-file = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `pubmedparser2-2.0.0a0/setup.py` & `pubmedparser2-2.0.1a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['appdirs>=1.4.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pubmedparser2',
-    'version': '2.0.0a0',
+    'version': '2.0.1a0',
     'description': 'Download and parse pubmed publication data',
-    'long_description': '---\nauthor: David R. Connell\ntitle: Pubmed parser\n---\n\nRead XML files and pull out selected values. Values to collect are\ndetermined by paths found in a [structure file](#structure-file). The\nstructure file also includes a key which associates the values with a\nparent element and names, which determine which file to place the\nelements in.\n\nFiles can be passed as either gzipped or uncompressed XML files or from\nstandard in.\n\nFor more info on Pubmed\'s XML files see:\n[pubmed<sub>190101</sub>.dtd.](https://dtd.nlm.nih.gov/ncbi/pubmed/doc/out/190101/index.html)\n\nUsage:\n\n``` bash\nxml_read --cache-dir=cache --structure-file=structure.yml \\\n    data/*.xml.gz\n```\n\nOr, with python:\n\n``` python\nimport pubmedparser\nimport pubmedparser.ftp\n\n# Download data\nfiles = pubmedparser.ftp.download(range(1, 6))\n\n# Read XML files using a YAML file to describe what data to collect.\ndata_dir = "file_example"\nstructure_file = "example/structure.yml"\nresults = pubmedparser.read_xml(files, structure_file, data_dir)\n```\n\nIn python, the structure file can be replaced with a dictionary of\ndictionaries as well.\n\n## Building CLI\n\nRequires `zlib`.\n\nClone the repository and in the directory run:\n\n``` bash\nmake cli\n```\n\nor using nix:\n\n``` bash\nnix shell "gitlab:DavidRConnell/pubmedparser"\n```\n\n## Installing with pip\n\n``` bash\npip install pubmedparser\n```\n\n# Structure file\n\nThe structure file is a YAML file containing key-value pairs for\ndifferent tags and paths. There are two required keys: `root` and `key`.\n`Root` provide the top-level tag, in the case of the pubmed files this\nwill be `PubmedArticleSet`.\n\n``` bash\nroot: "/PubmedArticleSet"\n```\n\nThe `/` is not strictly required as the program will ignore them, but\nthey are used to conform to the\n[xpath](https://en.wikipedia.org/wiki/XPath) syntax (although this\nprogram does not handle all cases for `xpath`).\n\nOnly tags below the root tag will be considered and the parsing will\nterminate once the program has left the root of the tree.\n\n`Key` is a reference tag. In the pubmed case, all data is with respect\nto a publication, so the key should identify the publication the values\nare linked to. The `PMID` tag is a suitable candidate.\n\n``` bash\nkey: "/PubmedArticle/MedlineCitation/PMID"\n```\n\nAfter `root`, all paths are taken as relative to the root node.\n\nThe other name-pairs in the file determine what other items to collect.\nThese can either be a simple name and path, like the key, such as:\n\n``` bash\nLanguage: "/PubmedArticle/MedlineCitation/Article/Language"\nKeywords: "/PubmedArticle/MedlineCitation/KeywordList/Keyword"\n```\n\nOr they can use a hierarchical representation to get multiple values\nbelow a child. This is mainly used to handle lists of items where there\nis an indefinite number of items below the list.\n\n``` bash\nAuthor: {\n  root: "/PubmedArticle/MedlineCitation/Article/AuthorList",\n  key: "/Author/auto_index",\n  LastName: "/Author/LastName",\n  ForeName: "/Author/ForeName",\n  Affiliation: "/Author/AffiliationInfo/Affiliation",\n  Orcid: "/Author/Identifier/[@Source=\'ORCID\']"\n}\n```\n\nHere, all paths are relative to the sub-structures `root` path, which is\nin turn relative to the parent structure\'s `root`. This sub-structure\nuses the same rules as the parent structure, so it needs both a `root`\nand `key` name-value pair. The results of searching each path are\nwritten to separate files. Each file gets a column for the parent and\nchild key. So in this case, each element of the author is linked by an\nauthor key and that is related to the publication they authored through\nthe parent key.\n\nThe main parser is called recursively to parse this structure so it\'s\nworth thinking about what the root should be under the context that the\nparser will be called with that root. This means if, instead of stopping\nat `/AuthorList`, `/Author` was added to the end of the root, the parser\nwould be called for each individual author, instead of once per author\nlist, leading to all author\'s getting the index 0.\n\nThere are a number of additional syntax constructs to note in the above\nexample. The key uses the special name `auto_index`, since there is no\nauthor ID in the XML data, an index is used to count the authors in the\norder they appear. This resets for each publication and starts at 0.\nTreating the `auto_index` as the tail of a path allows you to control\nwhen the indexing occurs—the index is incremented whenever it hits a\n`/Author` tag.\n\nIn addition to the `auto_index` key, there is a second special index\nname, `condensed`.\n\n``` bash\nReference: {\n  root: "/PubmedArticle/PubmedData/ReferenceList/Reference/ArticleIdList"\n  key: "/condensed"\n  PMID: "/ArticleId/[@IdType=\'pubmed\']"\n  DOI: "/ArticleId/[@IdType=\'doi\']"\n}\n```\n\nIn the case of `condensed`, instead of writing the results to separate\nfiles, they will printed as columns in the same file, and therefore do\nnot need an additional key for the sub-structure. If any of the elements\nare missing, they will be left blank, for example, if the parser does\nnot find a pubmed ID for a given reference, the row will look like\n`"%s\\t\\t%s"` where the first string will contain the parent key (the\n`PMID` of the publication citing this reference) and the second string\nwill contain the reference\'s `DOI`.\n\nThe `/[@attribute=\'value\']` syntax at the end of a path tells the parser\nto only collect an element if it has an attribute and the attribute\'s\nvalue matches the supplied value. Similarly the `/@attribute` syntax,\ntells the parser to collect the value of the attribute `attribute` along\nwith the element\'s value. Then both values will be written to the output\nfile. Currently only a single attribute can be specified.\n\nLastly, there is a special syntax for writing condensed sub-structures:\n\n``` bash\nDate: "/PubmedArticle/MedlineCitation/Article/Journal/JournalIssue/PubDate/{Year,Month,Day}"\n```\n\nThe `{child,child,child}` syntax allows you to select multiple children\nat the same level to be printed to a single file. This is useful when\nmultiple children make up a single piece of information (i.e. the\npublication date).\n\nA similar example structure file can be found in the example directory\nof this project at:\n[file:./example/structure.yml](./example/structure.yml).\n\n# Structure dictionary\n\nThe structure of the xml data to read can also be described as a python\ndictionary of dictionaries.\n\nThe form is similar to the file:\n\n``` python\nstructure = {\n    "root": "//PubmedArticleSet",\n    "key": "/PubmedArticle/MedlineCitation/PMID",\n    "DOI": "/PubmedArticle/PubmedData/ArticleIdList/ArticleId/[@IdType=\'doi\']",\n    "Date": "/PubmedArticle/MedlineCitation/Article/Journal/JournalIssue/PubDate/{Year,Month,Day}",\n    "Journal": "/PubmedArticle/MedlineCitation/Article/Journal/{Title,ISOAbbreviation}",\n    "Language": "/PubmedArticle/MedlineCitation/Article/Language",\n    "Author": {\n        "root": "/PubmedArticle/MedlineCitation/Article/AuthorList",\n        "key": "/Author/auto_index",\n        "LastName": "/Author/LastName",\n        "ForName": "/Author/ForeName",\n        "Affiliation": "/Author/AffiliationInfo/Affiliation",\n        "Orcid": "/Author/Identifier/[@Source=\'ORCID\']",\n    },\n    "Grant": {\n        "root": "/PubmedArticle/MedlineCitation/Article/GrantList",\n        "key": "/Grant/auto_index",\n        "ID": "/Grant/GrantID",\n        "Agency": "/Grant/Agency",\n    },\n    "Chemical": "/PubmedArticle/MedlineCitation/ChemicalList/Chemical/NameOfSubstance/@UI",\n    "Qualifier": "/PubmedArticle/MedlineCitation/MeshHeadingList/MeshHeading/QualifierName/@UI",\n    "Descriptor": "/PubmedArticle/MedlineCitation/MeshHeadingList/MeshHeading/DescriptorName/@UI",\n    "Keywords": "/PubmedArticle/MedlineCitation/KeywordList/Keyword",\n    "Reference": {\n        "root": (\n            "/PubmedArticle/PubmedData/ReferenceList/Reference/ArticleIdList"\n        ),\n        "key": "/condensed",\n        "PMID": "/ArticleId/[@IdType=\'pubmed\']",\n        "DOI": "/ArticleId/[@IdType=\'doi\']",\n    },\n}\n```\n\nThis can then be passed to `pubmedparser.read_xml` in place of the\nstructure file.\n\n# Future goals\n\n## Improve printing logic\n\nCurrently, values are printed as they are read in. Since the results for\nthe different paths are written to separate files, this shouldn\'t\nmatter, except for the case of the key. The key is not printed to its\nown results file, instead whatever the last seen key was is printed as\nthe key for the current value being printed. If the key is not the first\nelement to be read in the subtree, there will be a mismatch between\nvalue and publication ID.\n\nIn the case of `PMID` this is consistently the first element, so there\nshould not be a problem, however, it could be in other scenarios.\n\n## Error handling\n\nAfter refactoring the code, I have started adding some error handling\ncode, however this has not been consistently applied. Ideally, the\ndefault behavior will be for functions to return error codes. Then use\nan error checking macro to test that the result was not an error. I\nwould also like to add a set error strings that would be printed\ndepending on the error code. Possibly use a structure to represent\nerrors so that the erroring function could supply an additional string\nalong with the error.\n\nBetter error handling like this could also allow the python package to\nwrite it\'s own error handling function in the C API to override the\ndefault error mechanism to use python level errors. This would be done\nby testing if an error handler function was defined, if so the error\nchecking macro would use that function, otherwise it would fallback to a\ndefault function.\n',
+    'long_description': 'Read XML files and pull out selected values. Values to collect are\ndetermined by paths found in a [structure file](#structure-file). The\nstructure file also includes a key which associates the values with a\nparent element and names, which determine which file to place the\nelements in.\n\nFiles can be passed as either gzipped or uncompressed XML files or from\nstandard in.\n\nFor more info on Pubmed\'s XML files see:\n[pubmed<sub>190101</sub>.dtd.](https://dtd.nlm.nih.gov/ncbi/pubmed/doc/out/190101/index.html)\n\nUsage:\n\n``` bash\nxml_read --cache-dir=cache --structure-file=structure.yml \\\n    data/*.xml.gz\n```\n\nOr, with python:\n\n``` python\nimport pubmedparser2\nimport pubmedparser2.ftp\n\n# Download data\nfiles = pubmedparser2.ftp.download(range(1, 6))\n\n# Read XML files using a YAML file to describe what data to collect.\ndata_dir = "file_example"\nstructure_file = "example/structure.yml"\nresults = pubmedparser2.read_xml(files, structure_file, data_dir)\n```\n\nSee [the example\nfile](https://gitlab.com/net-synergy/pubmedparser/-/blob/master/example/creating_graphs.py)\nfor more options.\n\nIn python, the structure file can be replaced with a dictionary of\ndictionaries as well.\n\n## Building CLI\n\nRequires `zlib`.\n\nClone the repository and in the directory run:\n\n``` bash\nmake cli\n```\n\nor using nix:\n\n``` bash\nnix shell "gitlab:DavidRConnell/pubmedparser"\n```\n\n## Installing with pip\n\n``` bash\npip install pubmedparser2\n```\n\n# Structure file\n\nThe structure file is a YAML file containing key-value pairs for\ndifferent tags and paths. There are two required keys: `root` and `key`.\n`Root` provide the top-level tag, in the case of the pubmed files this\nwill be `PubmedArticleSet`.\n\n``` bash\nroot: "/PubmedArticleSet"\n```\n\nThe `/` is not strictly required as the program will ignore them, but\nthey are used to conform to the\n[xpath](https://en.wikipedia.org/wiki/XPath) syntax (although this\nprogram does not handle all cases for `xpath`).\n\nOnly tags below the root tag will be considered and the parsing will\nterminate once the program has left the root of the tree.\n\n`Key` is a reference tag. In the pubmed case, all data is with respect\nto a publication, so the key should identify the publication the values\nare linked to. The `PMID` tag is a suitable candidate.\n\n``` bash\nkey: "/PubmedArticle/MedlineCitation/PMID"\n```\n\nAfter `root`, all paths are taken as relative to the root node.\n\nThe other name-pairs in the file determine what other items to collect.\nThese can either be a simple name and path, like the key, such as:\n\n``` bash\nLanguage: "/PubmedArticle/MedlineCitation/Article/Language"\nKeywords: "/PubmedArticle/MedlineCitation/KeywordList/Keyword"\n```\n\nOr they can use a hierarchical representation to get multiple values\nbelow a child. This is mainly used to handle lists of items where there\nis an indefinite number of items below the list.\n\n``` bash\nAuthor: {\n  root: "/PubmedArticle/MedlineCitation/Article/AuthorList",\n  key: "/Author/auto_index",\n  LastName: "/Author/LastName",\n  ForeName: "/Author/ForeName",\n  Affiliation: "/Author/AffiliationInfo/Affiliation",\n  Orcid: "/Author/Identifier/[@Source=\'ORCID\']"\n}\n```\n\nHere, all paths are relative to the sub-structures `root` path, which is\nin turn relative to the parent structure\'s `root`. This sub-structure\nuses the same rules as the parent structure, so it needs both a `root`\nand `key` name-value pair. The results of searching each path are\nwritten to separate files. Each file gets a column for the parent and\nchild key. So in this case, each element of the author is linked by an\nauthor key and that is related to the publication they authored through\nthe parent key.\n\nThe main parser is called recursively to parse this structure so it\'s\nworth thinking about what the root should be under the context that the\nparser will be called with that root. This means if, instead of stopping\nat `/AuthorList`, `/Author` was added to the end of the root, the parser\nwould be called for each individual author, instead of once per author\nlist, leading to all author\'s getting the index 0.\n\nThere are a number of additional syntax constructs to note in the above\nexample. The key uses the special name `auto_index`, since there is no\nauthor ID in the XML data, an index is used to count the authors in the\norder they appear. This resets for each publication and starts at 0.\nTreating the `auto_index` as the tail of a path allows you to control\nwhen the indexing occurs—the index is incremented whenever it hits a\n`/Author` tag.\n\nIn addition to the `auto_index` key, there is a second special index\nname, `condensed`.\n\n``` bash\nReference: {\n  root: "/PubmedArticle/PubmedData/ReferenceList/Reference/ArticleIdList"\n  key: "/condensed"\n  PMID: "/ArticleId/[@IdType=\'pubmed\']"\n  DOI: "/ArticleId/[@IdType=\'doi\']"\n}\n```\n\nIn the case of `condensed`, instead of writing the results to separate\nfiles, they will printed as columns in the same file, and therefore do\nnot need an additional key for the sub-structure. If any of the elements\nare missing, they will be left blank, for example, if the parser does\nnot find a pubmed ID for a given reference, the row will look like\n`"%s\\t\\t%s"` where the first string will contain the parent key (the\n`PMID` of the publication citing this reference) and the second string\nwill contain the reference\'s `DOI`.\n\nThe `/[@attribute=\'value\']` syntax at the end of a path tells the parser\nto only collect an element if it has an attribute and the attribute\'s\nvalue matches the supplied value. Similarly the `/@attribute` syntax,\ntells the parser to collect the value of the attribute `attribute` along\nwith the element\'s value. Then both values will be written to the output\nfile. Currently only a single attribute can be specified.\n\nLastly, there is a special syntax for writing condensed sub-structures:\n\n``` bash\nDate: "/PubmedArticle/MedlineCitation/Article/Journal/JournalIssue/PubDate/{Year,Month,Day}"\n```\n\nThe `{child,child,child}` syntax allows you to select multiple children\nat the same level to be printed to a single file. This is useful when\nmultiple children make up a single piece of information (i.e. the\npublication date).\n\nA similar example structure file can be found in the example directory\nof this project at:\n[file:./example/structure.yml](./example/structure.yml).\n\n# Structure dictionary\n\nThe structure of the xml data to read can also be described as a python\ndictionary of dictionaries.\n\nThe form is similar to the file:\n\n``` python\nstructure = {\n    "root": "//PubmedArticleSet",\n    "key": "/PubmedArticle/MedlineCitation/PMID",\n    "DOI": "/PubmedArticle/PubmedData/ArticleIdList/ArticleId/[@IdType=\'doi\']",\n    "Date": "/PubmedArticle/MedlineCitation/Article/Journal/JournalIssue/PubDate/{Year,Month,Day}",\n    "Journal": "/PubmedArticle/MedlineCitation/Article/Journal/{Title,ISOAbbreviation}",\n    "Language": "/PubmedArticle/MedlineCitation/Article/Language",\n    "Author": {\n        "root": "/PubmedArticle/MedlineCitation/Article/AuthorList",\n        "key": "/Author/auto_index",\n        "LastName": "/Author/LastName",\n        "ForName": "/Author/ForeName",\n        "Affiliation": "/Author/AffiliationInfo/Affiliation",\n        "Orcid": "/Author/Identifier/[@Source=\'ORCID\']",\n    },\n    "Grant": {\n        "root": "/PubmedArticle/MedlineCitation/Article/GrantList",\n        "key": "/Grant/auto_index",\n        "ID": "/Grant/GrantID",\n        "Agency": "/Grant/Agency",\n    },\n    "Chemical": "/PubmedArticle/MedlineCitation/ChemicalList/Chemical/NameOfSubstance/@UI",\n    "Qualifier": "/PubmedArticle/MedlineCitation/MeshHeadingList/MeshHeading/QualifierName/@UI",\n    "Descriptor": "/PubmedArticle/MedlineCitation/MeshHeadingList/MeshHeading/DescriptorName/@UI",\n    "Keywords": "/PubmedArticle/MedlineCitation/KeywordList/Keyword",\n    "Reference": {\n        "root": (\n            "/PubmedArticle/PubmedData/ReferenceList/Reference/ArticleIdList"\n        ),\n        "key": "/condensed",\n        "PMID": "/ArticleId/[@IdType=\'pubmed\']",\n        "DOI": "/ArticleId/[@IdType=\'doi\']",\n    },\n}\n```\n\nThis can then be passed to `pubmedparser.read_xml` in place of the\nstructure file.\n\n# Future goals\n\n## Improve printing logic\n\nCurrently, values are printed as they are read in. Since the results for\nthe different paths are written to separate files, this shouldn\'t\nmatter, except for the case of the key. The key is not printed to its\nown results file, instead whatever the last seen key was is printed as\nthe key for the current value being printed. If the key is not the first\nelement to be read in the subtree, there will be a mismatch between\nvalue and publication ID.\n\nIn the case of `PMID` this is consistently the first element, so there\nshould not be a problem, however, it could be in other scenarios.\n\n## Error handling\n\nAfter refactoring the code, I have started adding some error handling\ncode, however this has not been consistently applied. Ideally, the\ndefault behavior will be for functions to return error codes. Then use\nan error checking macro to test that the result was not an error. I\nwould also like to add a set error strings that would be printed\ndepending on the error code. Possibly use a structure to represent\nerrors so that the erroring function could supply an additional string\nalong with the error.\n\nBetter error handling like this could also allow the python package to\nwrite it\'s own error handling function in the C API to override the\ndefault error mechanism to use python level errors. This would be done\nby testing if an error handler function was defined, if so the error\nchecking macro would use that function, otherwise it would fallback to a\ndefault function.\n',
     'author': 'David Connell',
     'author_email': 'davidconnell12@gmail.com',
     'maintainer': 'David Connell',
     'maintainer_email': 'davidconnell12@gmail.com',
     'url': 'https://gitlab.com/net-synergy/pubmedparser',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pubmedparser2-2.0.0a0/PKG-INFO` & `pubmedparser2-2.0.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 Metadata-Version: 2.1
 Name: pubmedparser2
-Version: 2.0.0a0
+Version: 2.0.1a0
 Summary: Download and parse pubmed publication data
 Home-page: https://gitlab.com/net-synergy/pubmedparser
 License: MIT
-Keywords: publication,network,MEDLINE,PubMed,References
+Keywords: publication,network,MEDLINE,PubMed,references
 Author: David Connell
 Author-email: davidconnell12@gmail.com
 Maintainer: David Connell
 Maintainer-email: davidconnell12@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Project-URL: Repository, https://gitlab.com/net-synergy/pubmedparser
 Description-Content-Type: text/markdown
 
----
-author: David R. Connell
-title: Pubmed parser
----
-
 Read XML files and pull out selected values. Values to collect are
 determined by paths found in a [structure file](#structure-file). The
 structure file also includes a key which associates the values with a
 parent element and names, which determine which file to place the
 elements in.
 
 Files can be passed as either gzipped or uncompressed XML files or from
@@ -42,26 +37,30 @@
 xml_read --cache-dir=cache --structure-file=structure.yml \
     data/*.xml.gz
 ```
 
 Or, with python:
 
 ``` python
-import pubmedparser
-import pubmedparser.ftp
+import pubmedparser2
+import pubmedparser2.ftp
 
 # Download data
-files = pubmedparser.ftp.download(range(1, 6))
+files = pubmedparser2.ftp.download(range(1, 6))
 
 # Read XML files using a YAML file to describe what data to collect.
 data_dir = "file_example"
 structure_file = "example/structure.yml"
-results = pubmedparser.read_xml(files, structure_file, data_dir)
+results = pubmedparser2.read_xml(files, structure_file, data_dir)
 ```
 
+See [the example
+file](https://gitlab.com/net-synergy/pubmedparser/-/blob/master/example/creating_graphs.py)
+for more options.
+
 In python, the structure file can be replaced with a dictionary of
 dictionaries as well.
 
 ## Building CLI
 
 Requires `zlib`.
 
@@ -76,15 +75,15 @@
 ``` bash
 nix shell "gitlab:DavidRConnell/pubmedparser"
 ```
 
 ## Installing with pip
 
 ``` bash
-pip install pubmedparser
+pip install pubmedparser2
 ```
 
 # Structure file
 
 The structure file is a YAML file containing key-value pairs for
 different tags and paths. There are two required keys: `root` and `key`.
 `Root` provide the top-level tag, in the case of the pubmed files this
```

