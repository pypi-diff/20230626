# Comparing `tmp/catleg-0.1.0rc2.tar.gz` & `tmp/catleg-0.1.0rc3.tar.gz`

## Comparing `catleg-0.1.0rc2.tar` & `catleg-0.1.0rc3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.catleg.toml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/_version.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/tox.ini
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.github/dependabot.yml
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.github/workflows/check.yml
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.github/workflows/publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/catleg.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/cli_util.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/config.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/find_changes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/git_diff.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/law_text_fr.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/parse_catala_markdown.py
--rw-r--r--   0        0        0     6402 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/query.py
--rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/skeleton.py
--rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/src/catleg/markdown_it/heading_extension.py
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/tests/test_catala_parsing.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/tests/test_legifrance_queries.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/LICENSE
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/README.md
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 catleg-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/.catleg.toml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/_version.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/tox.ini
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/.github/dependabot.yml
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/.github/workflows/check.yml
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/__init__.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/catleg.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/cli_util.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/config.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/find_changes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/git_diff.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/law_text_fr.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/parse_catala_markdown.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/query.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/skeleton.py
+-rw-r--r--   0        0        0     3554 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/src/catleg/markdown_it/heading_extension.py
+-rw-r--r--   0        0        0     9966 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/tests/LEGIARTI000038814944.json
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/tests/LEGIARTI000046790860.json
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/tests/test_catala_parsing.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/tests/test_legifrance_queries.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/LICENSE
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    14983 2020-02-02 00:00:00.000000 catleg-0.1.0rc3/PKG-INFO
```

### Comparing `catleg-0.1.0rc2/CONTRIBUTING.md` & `catleg-0.1.0rc3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/tox.ini` & `catleg-0.1.0rc3/tox.ini`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/.github/dependabot.yml` & `catleg-0.1.0rc3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/.github/workflows/check.yml` & `catleg-0.1.0rc3/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/.github/workflows/publish.yml` & `catleg-0.1.0rc3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/src/catleg/catleg.py` & `catleg-0.1.0rc3/src/catleg/catleg.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,14 +41,27 @@
     Output a given section of a law text.
     """
     skel = asyncio.run(markdown_skeleton(textid, sectionid))
     print(skel)
 
 
 @lf.command()
+def article(article_id: str):
+    """Retrieve an article from Legifrance"""
+    back = get_backend("legifrance")
+    print(
+        json.dumps(
+            asyncio.run(back.query_article_legi(article_id)),
+            indent=2,
+            ensure_ascii=False,
+        )
+    )
+
+
+@lf.command()
 def codes():
     """
     Retrieve a list of available codes.
     """
     back = get_backend("legifrance")
     print(json.dumps(asyncio.run(back.list_codes()), indent=2, ensure_ascii=False))
```

### Comparing `catleg-0.1.0rc2/src/catleg/find_changes.py` & `catleg-0.1.0rc3/src/catleg/find_changes.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/src/catleg/git_diff.py` & `catleg-0.1.0rc3/src/catleg/git_diff.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/src/catleg/law_text_fr.py` & `catleg-0.1.0rc3/src/catleg/law_text_fr.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/src/catleg/parse_catala_markdown.py` & `catleg-0.1.0rc3/src/catleg/parse_catala_markdown.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/src/catleg/query.py` & `catleg-0.1.0rc3/src/catleg/query.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,19 @@
   - legistix database (standalone)
   - legistix database (auto-api via datasette)
 """
 
 import datetime
 import functools
 import logging
-from types import SimpleNamespace
 from typing import Iterable, Optional, Protocol
 
 import aiometer
 import httpx
+from markdownify import markdownify as md  # type: ignore
 
 from catleg.config import settings
 
 from catleg.law_text_fr import Article, ArticleType, parse_article_id
 
 
 class Backend(Protocol):
@@ -50,22 +50,22 @@
     def __init__(self, client_id, client_secret):
         headers = {"Accept": "application/json"}
         self.client = httpx.AsyncClient(
             auth=LegifranceAuth(client_id, client_secret), headers=headers
         )
 
     async def article(self, id: str) -> Optional[Article]:
-        reply = await self._query_article_legi(id)
+        reply = await self.query_article_legi(id)
         article = _article_from_legifrance_reply(reply)
         if article is None:
             logging.warning(f"Could not retrieve article {id} (wrong identifier?)")
         return article
 
     async def articles(self, ids: Iterable[str]) -> Iterable[Optional[Article]]:
-        jobs = [functools.partial(self._query_article_legi, id) for id in ids]
+        jobs = [functools.partial(self.query_article_legi, id) for id in ids]
         replies = await aiometer.run_all(jobs, max_at_once=10, max_per_second=15)
         return [_article_from_legifrance_reply(reply) for reply in replies]
 
     async def list_codes(self):
         # TODO pagination
         params = {"pageSize": 100, "pageNumber": 1, "states": ["VIGUEUR"]}
         reply = await self.client.post(f"{self.API_BASE_URL}/list/code", json=params)
@@ -79,15 +79,15 @@
             f"{self.API_BASE_URL}/consult/legi/tableMatieres", json=params
         )
         reply.raise_for_status()
         if "sections" not in reply.json():
             raise ValueError(f"Could not retrieve TOC for text {id}")
         return reply.json()
 
-    async def _query_article_legi(self, id: str):
+    async def query_article_legi(self, id: str):
         typ, id = parse_article_id(id)
         match typ:
             case ArticleType.LEGIARTI | ArticleType.JORFARTI:
                 url = f"{self.API_BASE_URL}/consult/getArticle"
                 params = {"id": id}
             case ArticleType.CETATEXT:
                 url = f"{self.API_BASE_URL}/consult/juri"
@@ -106,14 +106,54 @@
 def get_backend(spec: str):
     # TODO: multiple backends, fallbacks...
     assert spec == "legifrance"
     client_id, client_secret = _get_legifrance_credentials(raise_if_missing=True)
     return LegifranceBackend(client_id, client_secret)
 
 
+class LegifranceArticle(Article):
+    def __init__(self, id: str, text: str, text_html: str, nota: str, nota_html: str):
+        self._id = id
+        self._text = text
+        self._text_html = text_html
+        self._nota = nota
+        self._nota_html = nota_html
+
+    @property
+    def id(self) -> str:
+        return self._id
+
+    @property
+    def text(self) -> str:
+        return self._text
+
+    @property
+    def text_html(self) -> str:
+        return self._text_html
+
+    @property
+    def nota(self) -> str:
+        return self._nota
+
+    @property
+    def nota_html(self) -> str:
+        return self._nota_html
+
+    @property
+    def type(self) -> ArticleType:
+        return parse_article_id(self.id)[0]
+
+    def to_markdown(self) -> str:
+        text_md = md(self.text_html).strip()
+        if len(self.nota_html):
+            nota_md = md(self.nota_html).strip()
+            text_md += f"\n\nNOTA :\n\n{nota_md}"
+        return text_md
+
+
 def _get_legifrance_credentials(*, raise_if_missing=True):
     client_id = settings.get("lf_client_id")
     client_secret = settings.get("lf_client_secret")
     if raise_if_missing:
         if (client_id is None) or (client_secret is None):
             raise ValueError(
                 "Please supply Legifrance credentials \
@@ -127,23 +167,21 @@
         article = reply["article"]
         if article is None:
             return None
     elif "text" in reply:
         article = reply["article"]
     else:
         raise ValueError("Could not parse Legifrance reply")
-    text = article["texte"]
-    if "nota" in article and len(article["nota"]):
-        text += f" NOTA : {article['nota']}"
-    id = article["id"]
-    return SimpleNamespace(
-        text=text,
-        id=id,
-        expiration_date=None,
-        new_version=None,
+
+    return LegifranceArticle(
+        id=article["id"],
+        text=article["texte"],
+        text_html=article["texteHtml"],
+        nota=article["nota"],
+        nota_html=article["notaHtml"],
     )
 
 
 class LegifranceAuth(httpx.Auth):
     """
     Manages authentication for Legifrance API access
     Requires a client id and a client secret, uses those
```

### Comparing `catleg-0.1.0rc2/src/catleg/skeleton.py` & `catleg-0.1.0rc3/src/catleg/skeleton.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,35 +10,36 @@
     Return a skeleton (formatted law text section)
     """
     if sectionid[:8].upper() != "LEGISCTA":
         raise ValueError("Expected section identifier (should start with 'SCTA')")
 
     back = get_backend("legifrance")
     toc = await back.code_toc(textid)
+
     nodes = dropwhile(
         lambda node_level: node_level[0]["cid"] != sectionid, _preorder(toc)
     )
 
     # some existence checking is needed here
     root, root_level = next(nodes)
     parts = []
 
     for node, level in _preorder(root, root_level):
         if node["id"][:8] != "LEGISCTA":
             # If it is not a section, then it is an article
             parts.append(f"{'#' * (level + 1)} Article {node['num']} | {node['id']}")
             article = await back.article(node["id"])
-            formatted = mdformat.text(article.text, options={"wrap": 80})
+            formatted = mdformat.text(article.to_markdown(), options={"wrap": 80})
             parts.append(formatted)
         else:
             parts.append(f"{'#' * level} {node['title']}")
 
     return "\n\n".join(parts)
 
 
-def _preorder(node, level=0):
+def _preorder(node, level=1):
     """Preorder traversal of articles and sections"""
     yield node, level
     for article in node["articles"]:
         yield article, level
     for section in node["sections"]:
         yield from _preorder(section, level + 1)
```

### Comparing `catleg-0.1.0rc2/src/catleg/markdown_it/heading_extension.py` & `catleg-0.1.0rc3/src/catleg/markdown_it/heading_extension.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/tests/test_catala_parsing.py` & `catleg-0.1.0rc3/tests/test_catala_parsing.py`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/LICENSE` & `catleg-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/README.md` & `catleg-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `catleg-0.1.0rc2/pyproject.toml` & `catleg-0.1.0rc3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "aiometer",
   "dynaconf",
   "httpx",
+  "markdownify",  # convert pre-formatted HTML from Legifrance to markdown for skeletons
   "markdown-it-py[plugins]",
   "mdformat>=0.7.16",
   "more-itertools",
   "typer[all]",
 ]
 dynamic = ["version"]
 
@@ -41,7 +42,10 @@
 
 [project.scripts]
 catleg = "catleg.catleg:main"
 
 [project.urls]
 "Homepage" = "https://github.com/CatalaLang/catleg/"
 "Bug Tracker" = "https://github.com/CatalaLang/catleg/issues"
+
+[tool.ruff]
+select = ["E", "F", "T100"]
```

### Comparing `catleg-0.1.0rc2/PKG-INFO` & `catleg-0.1.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catleg
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: A library of helper tools for catala programming in the context of French legislative texts.
 Project-URL: Homepage, https://github.com/CatalaLang/catleg/
 Project-URL: Bug Tracker, https://github.com/CatalaLang/catleg/issues
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -210,14 +210,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: aiometer
 Requires-Dist: dynaconf
 Requires-Dist: httpx
 Requires-Dist: markdown-it-py[plugins]
+Requires-Dist: markdownify
 Requires-Dist: mdformat>=0.7.16
 Requires-Dist: more-itertools
 Requires-Dist: typer[all]
 Provides-Extra: dev
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
```

