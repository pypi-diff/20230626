# Comparing `tmp/alpha_dom-0.1.1.tar.gz` & `tmp/alpha_dom-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha_dom-0.1.1.tar", max compression
+gzip compressed data, was "alpha_dom-0.1.2.tar", max compression
```

## Comparing `alpha_dom-0.1.1.tar` & `alpha_dom-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1085 2023-06-19 20:54:24.806605 alpha_dom-0.1.1/LICENSE
--rw-r--r--   0        0        0       72 2023-06-19 20:54:24.806605 alpha_dom-0.1.1/README.md
--rw-r--r--   0        0        0      640 2023-06-19 20:54:24.806605 alpha_dom-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       61 2023-06-19 20:54:24.806605 alpha_dom-0.1.1/python/alpha_dom/__init__.py
--rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 alpha_dom-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-26 00:26:42.691291 alpha_dom-0.1.2/LICENSE
+-rw-r--r--   0        0        0      340 2023-06-26 00:26:42.691291 alpha_dom-0.1.2/README.md
+-rw-r--r--   0        0        0      640 2023-06-26 00:26:42.691291 alpha_dom-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-06-26 00:26:42.691291 alpha_dom-0.1.2/python/alpha_dom/__init__.py
+-rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 alpha_dom-0.1.2/PKG-INFO
```

### Comparing `alpha_dom-0.1.1/LICENSE` & `alpha_dom-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alpha_dom-0.1.1/pyproject.toml` & `alpha_dom-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpha-dom"
-version = "0.1.1"
+version = "0.1.2"
 description = "Playing Dominion with Deep Reinforcement Learning"
 authors = [
     "Najib Ishaq <najib_ishaq@zoho.com>",
     "Morgan Prior <meprior424@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

