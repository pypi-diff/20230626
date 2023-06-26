# Comparing `tmp/mkdocs_caption-0.0.3.tar.gz` & `tmp/mkdocs_caption-0.0.4.tar.gz`

## Comparing `mkdocs_caption-0.0.3.tar` & `mkdocs_caption-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/_version.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/config.py
--rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/custom.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/helper.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/image.py
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/plugin.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/src/mkdocs_caption/table.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/LICENSE
--rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/README.md
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/_version.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/config.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/custom.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/helper.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/image.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/logger.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/plugin.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/src/mkdocs_caption/table.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/LICENSE
+-rw-r--r--   0        0        0     7581 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/README.md
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8537 2020-02-02 00:00:00.000000 mkdocs_caption-0.0.4/PKG-INFO
```

### Comparing `mkdocs_caption-0.0.3/src/mkdocs_caption/config.py` & `mkdocs_caption-0.0.4/src/mkdocs_caption/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,23 @@
     reference_text = config_options.Type(str, default="{identifier} {index}")
     caption_prefix = config_options.Type(str, default="{identifier} {index}:")
 
 
 class CaptionConfig(base.Config):
     """The configuration options for the Caption plugin."""
 
-    additional_identifier = config_options.ListOfItems(config_options.Type(str), default=[])
+    additional_identifier = config_options.ListOfItems(
+        config_options.Type(str), default=[]
+    )
     table = config_options.SubConfig(IdentifierCaption)
     figure = config_options.SubConfig(IdentifierCaption)
     custom = config_options.SubConfig(IdentifierCaption)
 
 
 def update_config(config: CaptionConfig, updates: t.Dict[str, t.Any]) -> CaptionConfig:
-    config.additional_identifier = updates.get("additional_identifier", config.additional_identifier)
+    config.additional_identifier = updates.get(
+        "additional_identifier", config.additional_identifier
+    )
     config.table.load_dict(updates.get("table", {}))
     config.figure.load_dict(updates.get("figure", {}))
     config.custom.load_dict(updates.get("custom", {}))
     return config
```

### Comparing `mkdocs_caption-0.0.3/src/mkdocs_caption/custom.py` & `mkdocs_caption-0.0.4/src/mkdocs_caption/custom.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing as t
 
 from lxml import etree
 
 from mkdocs_caption.config import IdentifierCaption
 from mkdocs_caption.helper import update_references, wrap_md_captions
+from mkdocs_caption.logger import PluginLogger
 
 CAPTION_TAG = "custom-caption"
 
 
 def preprocess_markdown(markdown: str, identifier: t.List[str]) -> str:
     """Preprocess markdown to wrap custom captions
 
@@ -20,76 +21,98 @@
     Returns:
         markdown string with custom captions wrapped
     """
     return wrap_md_captions(markdown, identifier, CAPTION_TAG)
 
 
 def _wrap_in_figure(
-    tree: etree._Element,
     caption_element: etree._Element,
+    *,
+    tree: etree._Element,
     index: int,
     identifier: str,
     config: IdentifierCaption,
+    logger: PluginLogger,
 ) -> None:
     """Wrap an element in a figure element with a custom caption.
 
     This function takes an XML tree, a target element, a caption element, an
     index, and an identifier, and wraps the target element in a figure element
     with a custom caption based on the caption element, index, and identifier.
 
     Args:
-        tree: The root element of the XML tree.
         target_element: The element to wrap in a figure element.
+        tree: The root element of the XML tree.
         caption_element: The caption element to use for the caption text.
         index: The index of the figure element.
         identifier: The identifier of the custom caption.
+        logger: Current plugin logger.
     """
     a_wrapper = caption_element.getparent()
     if a_wrapper is None:
-        cause = "Custom caption is not wrapped in a link"
-        raise RuntimeError(cause)
+        logger.error("Custom caption is not wrapped in a link")
+        return
     target_element = a_wrapper.getnext()
     if target_element is None:
-        cause = "Custom caption does not semm to have a element that follows it"
-        raise RuntimeError(cause)
+        logger.error("Custom caption does not semm to have a element that follows it")
+        return
 
     figure_element = etree.Element("figure", None, None)
     figure_element.attrib.update(caption_element.attrib)
     # wrap target element
     target_element.addprevious(figure_element)
     figure_element.insert(0, target_element)
 
     # add caption
     caption_prefix = config.caption_prefix.format(identifier=identifier, index=index)
     try:
-        fig_caption_element = etree.fromstring(f"<figcaption>{caption_prefix} {caption_element.text}</figcaption>")
-    except etree.XMLSyntaxError as e:
-        e.msg = f"Invalid XML in caption: {caption_element.text}"
-        raise e
+        fig_caption_element = etree.fromstring(
+            f"<figcaption>{caption_prefix} {caption_element.text}</figcaption>"
+        )
+    except etree.XMLSyntaxError:
+        logger.error(f"Invalid XML in caption: {caption_element.text}")
+        return
     figure_element.append(fig_caption_element)
 
-    figure_id = caption_element.attrib.get("id", config.identifier.format(identifier=identifier, index=index))
+    figure_id = caption_element.attrib.get(
+        "id", config.identifier.format(identifier=identifier, index=index)
+    )
     figure_element.attrib["id"] = figure_id
-    update_references(tree, figure_id, config.reference_text.format(identifier=identifier, index=index))
+    update_references(
+        tree,
+        figure_id,
+        config.reference_text.format(identifier=identifier, index=index),
+    )
     a_wrapper.remove(caption_element)
     parent = a_wrapper.getparent()
     if parent is not None:
         parent.remove(a_wrapper)
 
 
-def postprocess_html(tree: etree._Element, config: IdentifierCaption) -> None:
+def postprocess_html(
+    tree: etree._Element, config: IdentifierCaption, logger: PluginLogger
+) -> None:
     """Handle custom captions in an XML tree.
 
     This function takes an XML tree and replaces all custom captions in the tree
     with custom HTML tags.
 
     Args:
         tree: The root element of the XML tree.
+        config: The plugin configuration.
+        logger: Current plugin logger.
     """
     if not config.enable:
         return
     index_dict: t.Dict[str, int] = {}
     for custom_caption in tree.xpath(f"//{CAPTION_TAG}"):
         identifier = custom_caption.attrib.pop("identifier")
         index = index_dict.get(identifier, 1)
         index_dict[identifier] = index + 1
-        _wrap_in_figure(tree, custom_caption, index, identifier, config)
+        _wrap_in_figure(
+            custom_caption,
+            tree=tree,
+            index=index,
+            identifier=identifier,
+            config=config,
+            logger=logger,
+        )
```

### Comparing `mkdocs_caption-0.0.3/src/mkdocs_caption/helper.py` & `mkdocs_caption-0.0.4/src/mkdocs_caption/helper.py`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.3/src/mkdocs_caption/image.py` & `mkdocs_caption-0.0.4/src/mkdocs_caption/image.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from lxml import etree
 
 from mkdocs_caption.config import IdentifierCaption
 from mkdocs_caption.helper import update_references
+from mkdocs_caption.logger import PluginLogger
 
 
-def wrap_image(img: etree._Element, custom_id: str, caption: etree._Element, position: str) -> None:
+def wrap_image(
+    img: etree._Element, custom_id: str, caption: etree._Element, position: str
+) -> None:
     """Wrap an image element in a figure element with a custom caption.
 
     This function takes an image element and wraps it in a figure element with the
     custom caption. If the image element is already wrapped in an anchor element,
     the figure element is inserted after the anchor element instead.
 
     Args:
@@ -27,38 +30,48 @@
         figure_element.append(caption)
         figure_element.append(target)
     else:
         figure_element.append(target)
         figure_element.append(caption)
 
 
-def postprocess_html(tree: etree._Element, config: IdentifierCaption) -> None:
+def postprocess_html(
+    tree: etree._Element, config: IdentifierCaption, logger: PluginLogger
+) -> None:
     """Postprocess an XML tree to handle custom image captions.
 
     This function takes an XML tree and postprocesses it to handle custom image
     captions. It searches for all image elements in the tree, and if an image
     has a title attribute, it wraps the image in a figure element with a custom
     caption.
 
     Args:
         tree: The root element of the XML tree.
+        config: The plugin configuration.
+        logger: Current plugin logger.
     """
     if not config.enable:
         return
     index = config.start_index
     for img_element in tree.xpath("//p/a/img|//p/img"):
         title = img_element.get("title", img_element.get("alt", None))
-        custom_id = img_element.get("id", config.identifier.format(index=index, identifier="figure"))
+        custom_id = img_element.get(
+            "id", config.identifier.format(index=index, identifier="figure")
+        )
         update_references(
             tree,
             custom_id,
             config.reference_text.format(index=index, identifier="Figure"),
         )
         if title:
-            caption_prefix = config.caption_prefix.format(index=index, identifier="Figure")
+            caption_prefix = config.caption_prefix.format(
+                index=index, identifier="Figure"
+            )
             try:
-                caption_element = etree.fromstring(f"<figcaption>{caption_prefix} {title}</figcaption>")
-            except etree.XMLSyntaxError as e:
-                e.msg = f"Invalid XML in caption: {title}"
-                raise e
+                caption_element = etree.fromstring(
+                    f"<figcaption>{caption_prefix} {title}</figcaption>"
+                )
+            except etree.XMLSyntaxError:
+                logger.error(f"Invalid XML in caption: {title}")
+                continue
             wrap_image(img_element, custom_id, caption_element, config.position)
             index += config.increment_index
```

### Comparing `mkdocs_caption-0.0.3/src/mkdocs_caption/plugin.py` & `mkdocs_caption-0.0.4/src/mkdocs_caption/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from lxml import etree
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.pages import Page
 
 from mkdocs_caption import config, custom, image, table
+from mkdocs_caption.logger import get_logger
 
 
 class CaptionPlugin(BasePlugin[config.CaptionConfig]):
     """A MkDocs plugin for custom image and table captions.
 
     This plugin provides custom image and table caption functionality for
     MkDocs. It allows users to specify custom captions for images and tables
@@ -48,23 +49,27 @@
             page: `mkdocs.nav.Page` instance
             config: global configuration object
             files: global files collection
 
         Returns:
             The processed Markdown content of the page.
         """
+        logger = get_logger(page.file.src_path)
         config = self._get_config(page)
-        if self._config["table"]["enable"]:
-            markdown = table.preprocess_markdown(markdown, ["Table"])
-        identifier = []
-        if config["custom"]["enable"]:
-            identifier += config["additional_identifier"]
-            if config["figure"]["enable"]:
-                identifier += ["Figure"]
-            markdown = custom.preprocess_markdown(markdown, identifier)
+        try:
+            if self._config["table"]["enable"]:
+                markdown = table.preprocess_markdown(markdown, ["Table"])
+            identifier = []
+            if config["custom"]["enable"]:
+                identifier += config["additional_identifier"]
+                if config["figure"]["enable"]:
+                    identifier += ["Figure"]
+                markdown = custom.preprocess_markdown(markdown, identifier)
+        except Exception as e:
+            logger.error(f"Unexpected Error while preprocessing, skipping: {e}")
         return markdown
 
     def on_page_content(self, html: str, *, page: Page, **_) -> str:
         """Process the HTML content of a rendered page.
 
         The `page_content` event is called after the Markdown text is rendered to
         HTML (but before being passed to a template) and can be used to alter the
@@ -75,14 +80,21 @@
             page: `mkdocs.nav.Page` instance
             config: global configuration object
             files: global files collection
 
         Returns:
             The processed HTML content of the page.
         """
+        logger = get_logger(page.file.src_path)
         config = self._get_config(page)
-        parser = etree.HTMLParser()
-        tree = etree.fromstring(html, parser)
-        table.postprocess_html(tree, config["table"])
-        custom.postprocess_html(tree, config["custom"])
-        image.postprocess_html(tree, config["figure"])
-        return etree.tostring(tree, encoding="unicode")
+        try:
+            parser = etree.HTMLParser()
+            tree = etree.fromstring(html, parser)
+            if not tree:
+                return html
+            table.postprocess_html(tree, config["table"], logger)
+            custom.postprocess_html(tree, config["custom"], logger)
+            image.postprocess_html(tree, config["figure"], logger)
+            return etree.tostring(tree, encoding="unicode")
+        except Exception as e:
+            logger.error(f"Unexpected Error skipping: {e}")
+            return html
```

### Comparing `mkdocs_caption-0.0.3/src/mkdocs_caption/table.py` & `mkdocs_caption-0.0.4/src/mkdocs_caption/table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import typing as t
 
 from lxml import etree
 
 from mkdocs_caption.config import IdentifierCaption
 from mkdocs_caption.helper import update_references, wrap_md_captions
+from mkdocs_caption.logger import PluginLogger
 
 TABLE_CAPTION_TAG = "table-caption"
 
 
 def preprocess_markdown(markdown: str, identifier: t.List[str]) -> str:
     """Preprocess markdown to wrap custom captions
 
@@ -42,51 +43,66 @@
     for width in widths:
         col = etree.Element("col", {"span": "1", "width": f"{width/total*100}%"}, None)
         colgroup.append(col)
     return colgroup
 
 
 def _add_caption_to_table(
-    tree: etree._Element,
     table_element: etree._Element,
+    *,
+    tree: etree._Element,
     caption_element: etree._Element,
     index: int,
     config: IdentifierCaption,
+    logger: PluginLogger,
 ) -> None:
     """Add a caption to a table element in an XML tree.
 
     This function takes an XML tree, a table element, a caption element, and an
     index, and adds a caption to the table element based on the caption element
     and index.
 
     Args:
-        tree: The root element of the XML tree.
         table_element: The table element to add the caption to.
+        tree: The root element of the XML tree.
         caption_element: The caption element to use for the caption text.
         index: The index of the table element.
     """
     caption_prefix = config.caption_prefix.format(index=index, identifier="Table")
-    caption_text = caption_element.text.replace(" & ", " &amp; ") if caption_element.text else ""
+    caption_text = (
+        caption_element.text.replace(" & ", " &amp; ") if caption_element.text else ""
+    )
     try:
-        table_caption_element = etree.fromstring(f"<caption>{caption_prefix} {caption_text}</caption>")
-    except etree.XMLSyntaxError as e:
-        e.msg = f"Invalid XML in caption: <caption>{caption_prefix} {caption_text}</caption>"
-        raise e
+        table_caption_element = etree.fromstring(
+            f"<caption>{caption_prefix} {caption_text}</caption>"
+        )
+    except etree.XMLSyntaxError:
+        logger.error(
+            f"Invalid XML in caption: <caption>{caption_prefix} "
+            f"{caption_text}</caption>"
+        )
+        return
     table_element.insert(0, table_caption_element)
 
     if "cols" in caption_element.attrib:
         table_element.insert(0, _create_colgroups(caption_element.attrib["cols"]))
         caption_element.attrib.pop("cols")
     table_element.attrib.update(caption_element.attrib)
-    table_id = table_element.attrib.get("id", config.identifier.format(index=index, identifier="table"))
+    table_id = table_element.attrib.get(
+        "id", config.identifier.format(index=index, identifier="table")
+    )
     table_element.attrib["id"] = table_id
-    update_references(tree, table_id, config.reference_text.format(index=index, identifier="Table"))
+    update_references(
+        tree, table_id, config.reference_text.format(index=index, identifier="Table")
+    )
 
 
-def postprocess_html(tree: etree._Element, config: IdentifierCaption) -> None:
+def postprocess_html(
+    tree: etree._Element, config: IdentifierCaption, logger: PluginLogger
+) -> None:
     """Handle custom captions in an XML tree.
 
     This function takes an XML tree and replaces all custom captions in the tree
     with custom HTML tags.
 
     Args:
         tree: The root element of the XML tree.
@@ -97,12 +113,22 @@
     for custom_caption in tree.xpath(f"//{TABLE_CAPTION_TAG}"):
         identifier = custom_caption.attrib.pop("identifier")
         index = index_dict.get(identifier, config.start_index)
         index_dict[identifier] = index + config.increment_index
         a_wrapper = custom_caption.getparent()
         target_element = a_wrapper.getnext()
         if target_element.tag != "table":
-            msg = "Table caption must be followed by a table element."
-            raise RuntimeError(msg)
-        _add_caption_to_table(tree, target_element, custom_caption, index, config)
+            logger.error(
+                "Table caption must be followed by a table element. "
+                f"Skipping: {custom_caption.text}",
+            )
+            continue
+        _add_caption_to_table(
+            target_element,
+            tree=tree,
+            caption_element=custom_caption,
+            index=index,
+            config=config,
+            logger=logger,
+        )
         a_wrapper.remove(custom_caption)
         a_wrapper.getparent().remove(a_wrapper)
```

### Comparing `mkdocs_caption-0.0.3/LICENSE` & `mkdocs_caption-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.3/README.md` & `mkdocs_caption-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_caption-0.0.3/pyproject.toml` & `mkdocs_caption-0.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -97,20 +97,17 @@
 all = [
   "style",
   "typing",
 ]
 
 [tool.black]
 target-version = ["py37"]
-line-length = 120
-skip-string-normalization = true
 
 [tool.ruff]
 target-version = "py37"
-line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
@@ -133,14 +130,16 @@
   "UP",
   "W",
   "YTT",
 ]
 ignore = [
   # Using `xml` to parse untrusted data
   "S320",
+  # Too many arguments to function call
+  "PLR0913",
 ]
 
 [tool.ruff.isort]
 known-first-party = ["mkdocs_caption"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "all"
```

### Comparing `mkdocs_caption-0.0.3/PKG-INFO` & `mkdocs_caption-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-caption
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/tobiasah/mkdocs-caption#readme
 Project-URL: Issues, https://github.com/tobiasah/mkdocs-caption/issues
 Project-URL: Source, https://github.com/tobiasah/mkdocs-caption
 Author-email: Tobias Ahrens <tobias.ahrens@posteo.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-caption Version: 0.0.3 Project-URL:
+Metadata-Version: 2.1 Name: mkdocs-caption Version: 0.0.4 Project-URL:
 Documentation, https://github.com/tobiasah/mkdocs-caption#readme Project-URL:
 Issues, https://github.com/tobiasah/mkdocs-caption/issues Project-URL: Source,
 https://github.com/tobiasah/mkdocs-caption Author-email: Tobias Ahrens
 ahrens@posteo.de> License-Expression: MIT License-File: LICENSE Classifier:
 Development Status :: 4 - Beta Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

