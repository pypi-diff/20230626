# Comparing `tmp/pythorhead-0.9.1.tar.gz` & `tmp/pythorhead-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.9.1.tar", last modified: Sun Jun 25 13:05:13 2023, max compression
+gzip compressed data, was "pythorhead-0.9.2.tar", last modified: Mon Jun 26 17:35:16 2023, max compression
```

## Comparing `pythorhead-0.9.1.tar` & `pythorhead-0.9.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:05:13.746635 pythorhead-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:05:13.742635 pythorhead-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:05:13.742635 pythorhead-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-25 13:04:56.000000 pythorhead-0.9.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-25 13:04:56.000000 pythorhead-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-06-25 13:05:03.000000 pythorhead-0.9.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-25 13:04:56.000000 pythorhead-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-25 13:05:13.746635 pythorhead-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-25 13:04:56.000000 pythorhead-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:05:13.742635 pythorhead-0.9.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-25 13:04:56.000000 pythorhead-0.9.1/examples/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-25 13:04:56.000000 pythorhead-0.9.1/examples/site.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-25 13:04:56.000000 pythorhead-0.9.1/examples/user.py
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-25 13:04:56.000000 pythorhead-0.9.1/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-25 13:05:03.000000 pythorhead-0.9.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:05:13.746635 pythorhead-0.9.1/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/community.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:05:13.746635 pythorhead-0.9.1/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/types/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-25 13:04:56.000000 pythorhead-0.9.1/pythorhead/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 13:05:13.746635 pythorhead-0.9.1/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-25 13:05:13.000000 pythorhead-0.9.1/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-25 13:05:13.000000 pythorhead-0.9.1/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 13:05:13.000000 pythorhead-0.9.1/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-25 13:05:13.000000 pythorhead-0.9.1/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 13:04:56.000000 pythorhead-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 13:05:13.746635 pythorhead-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.923235 pythorhead-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.923235 pythorhead-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-26 17:34:58.000000 pythorhead-0.9.2/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-26 17:34:58.000000 pythorhead-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7658 2023-06-26 17:35:06.000000 pythorhead-0.9.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-26 17:34:58.000000 pythorhead-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-26 17:35:16.927235 pythorhead-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-26 17:34:58.000000 pythorhead-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-26 17:34:58.000000 pythorhead-0.9.2/examples/pic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-26 17:34:58.000000 pythorhead-0.9.2/examples/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-26 17:34:58.000000 pythorhead-0.9.2/examples/site.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-06-26 17:34:58.000000 pythorhead-0.9.2/examples/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-26 17:34:58.000000 pythorhead-0.9.2/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-26 17:35:06.000000 pythorhead-0.9.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/community.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5874 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/types/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-26 17:34:58.000000 pythorhead-0.9.2/pythorhead/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:35:16.927235 pythorhead-0.9.2/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-26 17:35:16.000000 pythorhead-0.9.2/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-26 17:35:16.000000 pythorhead-0.9.2/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:35:16.000000 pythorhead-0.9.2/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 17:35:16.000000 pythorhead-0.9.2/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:34:58.000000 pythorhead-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:35:16.927235 pythorhead-0.9.2/setup.cfg
```

### Comparing `pythorhead-0.9.1/.github/workflows/pypi.yml` & `pythorhead-0.9.2/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/.gitignore` & `pythorhead-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/CHANGELOG.md` & `pythorhead-0.9.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # Changelog
 
+## [v0.9.2](https://github.com/db0/pythorhead/tree/v0.9.2) (2023-06-26)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.9.1...v0.9.2)
+
+**Closed issues:**
+
+- Changelog [\#27](https://github.com/db0/pythorhead/issues/27)
+
+**Merged pull requests:**
+
+- Added get and list to community [\#31](https://github.com/db0/pythorhead/pull/31) ([NicKoehler](https://github.com/NicKoehler))
+- Added pic example [\#30](https://github.com/db0/pythorhead/pull/30) ([NicKoehler](https://github.com/NicKoehler))
+
 ## [v0.9.1](https://github.com/db0/pythorhead/tree/v0.9.1) (2023-06-25)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.9.0...v0.9.1)
 
 **Merged pull requests:**
 
 - chore: changelog [\#29](https://github.com/db0/pythorhead/pull/29) ([db0](https://github.com/db0))
```

### Comparing `pythorhead-0.9.1/LICENSE` & `pythorhead-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/PKG-INFO` & `pythorhead-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.9.1
+Version: 0.9.2
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.9.1/README.md` & `pythorhead-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/examples/pm.py` & `pythorhead-0.9.2/examples/pm.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/examples/site.py` & `pythorhead-0.9.2/examples/site.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/examples/user.py` & `pythorhead-0.9.2/examples/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/logo.png` & `pythorhead-0.9.2/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/pyproject.toml` & `pythorhead-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.9.1"
+version = "v0.9.2"
 readme = "README.md"
 requires-python = ">=3.8,<3.12"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.9.1/pythorhead/comment.py` & `pythorhead-0.9.2/pythorhead/comment.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/pythorhead/community.py` & `pythorhead-0.9.2/pythorhead/community.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from typing import Optional
+from typing import List, Optional
 
-from pythorhead.requestor import Requestor, Request
+from pythorhead.requestor import Request, Requestor
+from pythorhead.types import ListingType, SortType
 
 
 class Community:
     def __init__(self, _requestor: Requestor):
         self._requestor = _requestor
 
     def create(
-            self,
-            name: str,
-            title: str,
-            description: Optional[str] = None,
-            icon: Optional[str] = None,
-            nsfw: Optional[bool] = None,
-            posting_restricted_to_mods: Optional[bool] = None
+        self,
+        name: str,
+        title: str,
+        description: Optional[str] = None,
+        icon: Optional[str] = None,
+        nsfw: Optional[bool] = None,
+        posting_restricted_to_mods: Optional[bool] = None,
     ) -> Optional[dict]:
         """
         Create a community
 
         Args:
             name (str)
             title (str)
@@ -26,22 +27,76 @@
             icon (str, optional): Defaults to None
             nsfw (bool, optional): Defaults to None
             posting_restricted_to_mods (bool, optional): Defaults to None
 
         Returns:
             Optional[dict]: post data if successful
         """
-        new_community = {
+        new_community: dict = {
             "name": name,
             "title": title,
-
         }
         if description is not None:
-            new_community['description'] = description
+            new_community["description"] = description
         if icon is not None:
-            new_community['icon'] = icon
+            new_community["icon"] = icon
         if nsfw is not None:
-            new_community['nsfw'] = nsfw
+            new_community["nsfw"] = nsfw
         if [posting_restricted_to_mods] is not None:
-            new_community['[posting_restricted_to_mods]'] = [posting_restricted_to_mods]
+            new_community["[posting_restricted_to_mods]"] = [posting_restricted_to_mods]
 
         return self._requestor.api(Request.POST, "/post", json=new_community)
+
+    def get(self, id: Optional[int] = None, name: Optional[str] = None) -> Optional[dict]:
+        """
+        Get a community by id or name
+
+        Args:
+            id (Optional[int]): Defaults to None
+            name (Optional[str]): Defaults to None
+
+        Returns:
+            Optional[dict]: community data if successful
+        """
+        get_community: dict = {}
+
+        if id is not None:
+            get_community["id"] = id
+        if name is not None:
+            get_community["name"] = name
+
+        return self._requestor.api(Request.GET, "/community", params=get_community)
+
+    def list(  # noqa: A003
+        self,
+        limit: Optional[int] = None,
+        page: Optional[int] = None,
+        sort: Optional[SortType] = None,
+        type_: Optional[ListingType] = None,
+    ) -> List[dict]:
+        """
+
+        Get communities, with various filters.
+
+        Args:
+            limit (Optional[int], optional): Defaults to None.
+            page (Optional[int], optional): Defaults to None.
+            sort (Optional[SortType], optional): Defaults to None.
+            type_ (Optional[ListingType], optional): Defaults to None.
+
+        Returns:
+            List[dict]: list of communities
+        """
+        list_community: dict = {}
+
+        if limit is not None:
+            list_community["limit"] = limit
+        if page is not None:
+            list_community["page"] = page
+        if sort is not None:
+            list_community["sort"] = sort.value
+        if type_ is not None:
+            list_community["type"] = type_.value
+
+        if data := self._requestor.api(Request.GET, "/community/list", params=list_community):
+            return data["communities"]
+        return []
```

### Comparing `pythorhead-0.9.1/pythorhead/image.py` & `pythorhead-0.9.2/pythorhead/image.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/pythorhead/lemmy.py` & `pythorhead-0.9.2/pythorhead/lemmy.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional
 
 from pythorhead.comment import Comment
 from pythorhead.community import Community
 from pythorhead.image import Image
 from pythorhead.post import Post
 from pythorhead.private_message import PrivateMessage
-from pythorhead.requestor import Request, Requestor
+from pythorhead.requestor import Requestor
 from pythorhead.site import Site
 from pythorhead.user import User
 
 logging.basicConfig(format="%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 
 
 class Lemmy:
@@ -35,13 +35,13 @@
     def log_in(self, username_or_email: str, password: str) -> bool:
         return self._requestor.log_in(username_or_email, password)
 
     def discover_community(self, community_name: str) -> Optional[int]:
         if community_name in self._known_communities:
             return self._known_communities[community_name]
 
-        request = self._requestor.api(Request.GET, "/community", params={"name": community_name})
+        request = self.community.get(name=community_name)
 
         if request is not None:
             community_id = request["community_view"]["community"]["id"]
             self._known_communities[community_name] = community_id
             return community_id
```

### Comparing `pythorhead-0.9.1/pythorhead/post.py` & `pythorhead-0.9.2/pythorhead/post.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, List, Literal, Optional
 
 from pythorhead.requestor import Request, Requestor
-from pythorhead.types import FeatureType, ListingType, PostSortType
+from pythorhead.types import FeatureType, ListingType, SortType
 
 
 class Post:
     def __init__(self, _requestor: Requestor):
         self._requestor = _requestor
 
     def get(
@@ -35,15 +35,15 @@
     def list(  # noqa: A003
         self,
         community_id: Optional[int] = None,
         community_name: Optional[str] = None,
         limit: Optional[int] = None,
         page: Optional[int] = None,
         saved_only: Optional[bool] = None,
-        sort: Optional[PostSortType] = None,
+        sort: Optional[SortType] = None,
         type_: Optional[ListingType] = None,
     ) -> List[dict]:
         """
 
         Get posts, with various filters.
 
         Args:
```

### Comparing `pythorhead-0.9.1/pythorhead/private_message.py` & `pythorhead-0.9.2/pythorhead/private_message.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/pythorhead/requestor.py` & `pythorhead-0.9.2/pythorhead/requestor.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/pythorhead/site.py` & `pythorhead-0.9.2/pythorhead/site.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.9.1/pythorhead/user.py` & `pythorhead-0.9.2/pythorhead/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any, List, Literal, Optional
 
 from pythorhead.requestor import Request, Requestor
-from pythorhead.types import PostSortType
+from pythorhead.types import SortType
 
 
 class User:
     def __init__(self, _requestor: Requestor):
         self._requestor = _requestor
 
     def get(
         self,
         person_id: Optional[str] = None,
         username: Optional[str] = None,
-        sort: Optional[PostSortType] = None,
+        sort: Optional[SortType] = None,
         page: Optional[int] = None,
         limit: Optional[int] = None,
         community_id: Optional[int] = None,
         saved_only: Optional[bool] = None,
     ) -> Optional[dict]:
         """
         Get user details with various filters.
```

### Comparing `pythorhead-0.9.1/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.9.2/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.9.1
+Version: 0.9.2
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.9.1/pythorhead.egg-info/SOURCES.txt` & `pythorhead-0.9.2/pythorhead.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 CHANGELOG.md
 LICENSE
 README.md
 logo.png
 pyproject.toml
 requirements.txt
 .github/workflows/pypi.yml
+examples/pic.py
 examples/pm.py
 examples/site.py
 examples/user.py
 pythorhead/__init__.py
 pythorhead/auth.py
 pythorhead/comment.py
 pythorhead/community.py
```

