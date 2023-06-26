# Comparing `tmp/provo-1.0.5.tar.gz` & `tmp/provo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "provo-1.0.5.tar", last modified: Wed May 24 12:30:45 2023, max compression
+gzip compressed data, was "provo-1.1.0.tar", last modified: Mon Jun 26 15:30:59 2023, max compression
```

## Comparing `provo-1.0.5.tar` & `provo-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 12:30:45.124736 provo-1.0.5/
--rw-rw-rw-   0        0        0     1070 2023-05-24 11:53:22.000000 provo-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     3315 2023-05-24 12:30:45.123738 provo-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    26043 2023-05-24 11:50:51.000000 provo-1.0.5/README.md
--rw-rw-rw-   0        0        0     2746 2022-11-24 15:51:36.000000 provo-1.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-24 12:30:45.095734 provo-1.0.5/provo/
--rw-rw-rw-   0        0        0       55 2022-11-19 11:48:56.000000 provo-1.0.5/provo/__init__.py
--rw-rw-rw-   0        0        0     1841 2022-11-20 14:42:08.000000 provo-1.0.5/provo/idvault.py
--rw-rw-rw-   0        0        0    25472 2023-01-26 14:06:59.000000 provo-1.0.5/provo/provontologygraph.py
--rw-rw-rw-   0        0        0    10948 2022-11-24 10:44:43.000000 provo-1.0.5/provo/startingpointclasses.py
--rw-rw-rw-   0        0        0      455 2022-11-24 10:52:04.000000 provo-1.0.5/provo/staticfunctions.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:30:45.121739 provo-1.0.5/provo/tests/
--rw-rw-rw-   0        0        0        0 2022-11-20 13:47:51.000000 provo-1.0.5/provo/tests/__init__.py
--rw-rw-rw-   0        0        0     1397 2022-11-24 10:26:09.000000 provo-1.0.5/provo/tests/test_provenance_graph.py
--rw-rw-rw-   0        0        0     3423 2022-11-24 10:28:08.000000 provo-1.0.5/provo/tests/test_starting_point_classes.py
--rw-rw-rw-   0        0        0     1526 2022-11-24 10:30:02.000000 provo-1.0.5/provo/tests/test_vault.py
-drwxrwxrwx   0        0        0        0 2023-05-24 12:30:45.114736 provo-1.0.5/provo.egg-info/
--rw-rw-rw-   0        0        0     3315 2023-05-24 12:30:45.000000 provo-1.0.5/provo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-05-24 12:30:45.000000 provo-1.0.5/provo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 12:30:45.000000 provo-1.0.5/provo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-05-24 12:30:45.000000 provo-1.0.5/provo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 12:30:45.000000 provo-1.0.5/provo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 12:30:45.125736 provo-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1047 2023-05-24 12:30:20.000000 provo-1.0.5/setup.py
+drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-26 15:30:59.951288 provo-1.1.0/
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1070 2023-06-23 06:54:13.000000 provo-1.1.0/LICENSE
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      515 2023-06-26 15:30:59.951288 provo-1.1.0/PKG-INFO
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    25679 2023-06-26 14:25:22.000000 provo-1.1.0/README.md
+drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-26 15:30:59.947288 provo-1.1.0/provo/
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       54 2023-06-23 06:54:13.000000 provo-1.1.0/provo/__init__.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     3627 2023-06-26 15:24:38.000000 provo-1.1.0/provo/idvault.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    25046 2023-06-26 14:28:15.000000 provo-1.1.0/provo/provontologygraph.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)    10519 2023-06-26 14:19:28.000000 provo-1.1.0/provo/startingpointclasses.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      442 2023-06-23 06:54:13.000000 provo-1.1.0/provo/staticfunctions.py
+drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-26 15:30:59.951288 provo-1.1.0/provo/tests/
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-23 06:54:13.000000 provo-1.1.0/provo/tests/__init__.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1363 2023-06-23 06:54:13.000000 provo-1.1.0/provo/tests/test_provenance_graph.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     4777 2023-06-26 15:25:26.000000 provo-1.1.0/provo/tests/test_rdf_output.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     3332 2023-06-23 06:54:13.000000 provo-1.1.0/provo/tests/test_starting_point_classes.py
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)     1423 2023-06-26 15:28:25.000000 provo-1.1.0/provo/tests/test_vault.py
+drwxr-xr-x   0 ruemmler (946828456) domänen-benutzer (946800513)        0 2023-06-26 15:30:59.951288 provo-1.1.0/provo.egg-info/
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      515 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/PKG-INFO
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      448 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/SOURCES.txt
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        1 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/dependency_links.txt
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       23 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/requires.txt
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)        6 2023-06-26 15:30:59.000000 provo-1.1.0/provo.egg-info/top_level.txt
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)       38 2023-06-26 15:30:59.951288 provo-1.1.0/setup.cfg
+-rw-r--r--   0 ruemmler (946828456) domänen-benutzer (946800513)      862 2023-06-26 14:25:41.000000 provo-1.1.0/setup.py
```

### Comparing `provo-1.0.5/LICENSE` & `provo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `provo-1.0.5/README.md` & `provo-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,611 +1,613 @@
-# README
-
-The package supports the creation of [PROV-O](https://www.w3.org/TR/prov-o/) compliant provenance graphs.
-
-The package requires __Python 3.11__.
-
-## Installation
-
-You can install the package from the Python Package Index (PyPI):
-
-`pip install provo`
-
-Or by downloading this repository:
-
-1. Download and unzip the repository
-2. Open Shell and _cd_ to unzipped repository
-3. Run `pip install -e .` (in the folder that contains ```setup.py```)
-
-## Contents
-
-The package is a Python API to PROV-O. It implements the [PROV-O starting point classes](https://www.w3.org/TR/prov-o/#starting-points-figure) __Entity__, __Activity__ and __Agent__ as Python classes with methods to establish the _PROV-O starting point properties_ between instances of these classes.
-
-## Features
-
-The package's objective is to support the programmatical creation of provenance graphs that are compliant with the W3C Recommendation PROV-O: The PROV Ontology. Users of the package shall be enabled to tightly couple the generation of data with the generation of their provenance. As the package implements PROV-O, the created graph is exportable as an RDF document. Finally, the graph can be exported as a mermaid flowchart with some configuration options to adjust the style of the resulting chart.
-
-### Compliance
-
-- The PROV-O classes __Entity__, __Activity__, and __Agent__ are implemented as Python classes.
-- The PROV-O properties _wasGeneratedBy_, _wasDerivedFrom_, _wasAttributedTo_, _startedAtTime_, _used_, _wasInformedBy_, _endedAtTime_, _wasAssociatedWith_, and _actedOnBehalfOf_ are implemented as instance methods of their according classes.
-- Attributes that are passed to these methods are type-checked to enforce compliance with PROV-O.
-- Node Ids are checked for validity.
-- Use of the same ID for different objects throws an error.
-
-### Ease of Use
-
-- The package implements full type hint support, thus enabling rich support from the IDE.
-- The classes `Provence_Ontology_Graph`, `Entity`, `Activity`, and `Agent` can be printed to terminal in a user-friendly, readable way with the default `print()` command.
-- Objects of the classes `Entity`, `Activity`, and `Agent` can be instantiated with auto-generated Ids (although it's not recommended using this for production).
-- Export as [mermaid flowchart](https://mermaid-js.github.io/mermaid/#/flowchart) to review the graph visually.
-
-### Interface to RDF via the [rdflib](https://rdflib.readthedocs.io/en/stable/) package
-
-- The graph's contents can be converted to an `rdflib.Graph` object.
-- The graph can be exported in various RDF serializations.
-
-## Manual
-
-The package is centered around the class `ProvenanceOntologyGraph`. Entities, Activities, and Agents are added to this graph using the according class methods. Relations between the PROV-O class objects are constructed using their respective class methods.
-
-### Create a Provenance Ontology Graph
-
-The graph can be initialized with default or user defined attributes. The graph can be printed to the terminal with `print(graph)`.
-
-```python
-# ex1 - create a provenance graph
-from provo import ProvOntologyGraph
-
-# __defaults__
-# namespace: str = "https://provo-example.org/",
-# namespace_abbreviation: str = "", 
-# lang: str = "en"
-provenance_graph = ProvOntologyGraph()
-
-prov_ontology_graph = ProvOntologyGraph(
-    namespace='http://example.org#',
-    namespace_abbreviation="ex",
-    lang="en"
-)
-```
-
-`namespace=`
-
-- Default is `"https://provo-example.org/"`.
-- Has to be valid url, validation is currently performed with the [validators](https://pypi.org/project/validators/) package.
-- Has to end with `/` or `#`.
-
-`namespace_abbreviation=`
-
-- Default is `""`.
-- Used when converting to other models, such as RDF (-> prefixes)
-- Only characters from the Latin alphabet are allowed.
-- RDF core prefixes (*owl*, *rdf*, *rdfs*, *xsd* and *xml*) are prohibited from use.
-
->**Note** 
-> Although not prohibited, the following prefixes are commonly used and thus recommended being avoided: *brick*, *csvw*, *dc*, *dcat*, *dcmitype*, *cdterms*, *dcam*, *doap*, *foaf*, *geo*, *odrl*, *org*, *prof*, *prov*, *qb*, *sdo*, *sh*, *skos*, *sosa*, *ssn*, *time*, *vann* and *void*.
-
-`lang=`
-
-- Default is `"en"`.
-- Used when converting to other models that support a *lang* tag.
-- Has to be compliant with [RFC 5646](https://www.rfc-editor.org/info/rfc5646) (Phillips, A., Ed., and M. Davis, Ed., "Tags for Identifying Languages", BCP 47, RFC 5646, September 2009). Compliance is not validated!
-
-### Create Entities, Activities and Agents and define relations between them
-
-The creation for classes follows the same pattern. The classes only differ in their methods. PROV-O Classes are instantiated by using the add methods of the provenance graph class. Below you find the `add_entity()` method of `ProvenanceOntologyGraph` for reference.
-
-```python
-# definition of add_entity() in ProvOntologyGraph()
-def add_entity(self, 
-    id_string: str = "", 
-    label: str = "", 
-    description: str = "", 
-    namespace: str = "") -> Entity:
-    """creates a new entity, adds it to the graph and returns it then"""
-
-    # the id of the PROV class objects is a combination of the 
-    # namespace and the id_string. The method _handle_id() builds 
-    # the actual id of the node, if checks whether the provided 
-    # namespace-id combination is already used for a node in the graph.
-    # if no namespace is provided: default namespace is used, 
-    # if no id is provided: id get automatically generated.
-    node_id = self._handle_id(namespace, id_string)
-    # the PROV class (in this case an Entity) is only created if everything with the ID is fine
-    entity = Entity(
-        # mandatory
-        node_id=node_id,
-        # optional
-        label=label,
-        # optional
-        description=description)
-    self._entities.append(entity)
-    return entity
-```
-
-The relations are defined by calling the respective methods of the PROV class instances.
-
-Example use of the provenance graph's add-methods and the definition of a *used*-relation between an Activity and an Entity:
-
-```python
-# ex2 - create entities, activities and agents, 
-# and define relation between them
-entity = prov_ontology_graph.add_entity(
-    id_string="example_entity",
-    label="Example Entity")
-
-activity = prov_ontology_graph.add_activity(
-    label="Anonymous activity",
-    description="An arbitrary activity."
-)
-
-entity.was_generated_by(activity)
-
-print(entity)
-# id: http://example.org#example_entity
-# label: Example Entity
-# was generated by: ['Anonymous activity']
-# ---
-
-print(activity)
-# id: http://example.org#94021a6a-40cd-4c02-9571-33480488ff82
-# label: Anonymous activity
-# description: An arbitrary activity.
-# ---
-```
-
-### RDF interface
-
-The graph can be directly serialized as RDF document or be converted to an `rdflib` Graph, for further manipulation.
-
-```python
-# ex3 - serialize provenance graph as RDF document
-prov_ontology_graph.serialize_as_rdf("manual_examples.ttl")
-```
-
-```
-@prefix : <http://example.org#> .
-@prefix prov: <http://www.w3.org/ns/prov#> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
-
-:example_entity a prov:Entity ;
-    rdfs:label "Example Entity"@en ;
-    prov:wasGeneratedBy :832b1ada-22f2-45b8-bdca-dfbe89fb68c8 .
-
-:832b1ada-22f2-45b8-bdca-dfbe89fb68c8 a prov:Activity ;
-    rdfs:label "Anonymous activity"@en ;
-    rdfs:comment "An arbitrary activity."@en .
-```
-
-```python
-# ex4 - interface with rdflib
-
-from rdflib import SKOS, Literal, URIRef
-
-rdflib_graph = prov_ontology_graph.get_rdflib_graph()
-
-rdflib_graph.bind("skos", SKOS)
-
-rdflib_graph.add((
-    URIRef(entity.get_id()), 
-    SKOS.prefLabel, 
-    Literal(entity.get_label(), lang="en")
-))
-
-rdflib_graph.serialize("examples/rdflib_interface.ttl")
-```
-```
-@prefix : <http://example.org#> .
-@prefix prov: <http://www.w3.org/ns/prov#> .
-@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
-@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
-
-:example_entity a prov:Entity ;
-    rdfs:label "Example Entity"@en ;
-    skos:prefLabel "Example Entity"@en ;
-    prov:wasGeneratedBy :832b1ada-22f2-45b8-bdca-dfbe89fb68c8 .
-
-:832b1ada-22f2-45b8-bdca-dfbe89fb68c8 a prov:Activity ;
-    rdfs:label "Anonymous activity"@en ;
-    rdfs:comment "An arbitrary activity."@en .
-```
-
-### Export as Mermaid Flowchart
-
-Mermaid is a"[...] diagramming and charting tool that renders Markdown-inspired text definitions [...]". It can be embedded in markdown documents like so:
-
-````markdown
-```mermaid
-flowchart LR
-    entity_id[Entity] -- was generated by --> activity_id[Activity]
-```
-````
-
-If the markdown interpreter supports mermaid, this results in:
-
-```mermaid
-flowchart LR
-    entity_id[Entity] -- was generated by --> activity_id[Activity]
-```
-
-To export the provenance graph as mermaid chart call the according export method:
-
-```python
-# ex5
-
-prov_ontology_graph.export_as_mermaid_flowchart(file_name="examples/manual_examples_flowchart_default.md")
-```
-
-```mermaid
-flowchart TD
-classDef entity fill:#fffedf
-classDef entity color:#000000
-classDef entity stroke:#a4a4a4
-classDef entity stroke-width:1px
-classDef activity fill:#cfceff
-classDef activity color:#000000
-classDef activity stroke:#a4a4a4
-classDef activity stroke-width:1px
-classDef agent fill:#ffebc3
-classDef agent color:#000000
-classDef agent stroke:#a4a4a4
-classDef agent stroke-width:1px
-http://example.org#example_entity([Example Entity]):::entity
-http://example.org#example_entity-- was generated by -->http://example.org#832b1ada-22f2-45b8-bdca-dfbe89fb68c8
-http://example.org#832b1ada-22f2-45b8-bdca-dfbe89fb68c8[[Anonymous activity]]:::activity
-```
-
-The style of the resulting graph is defined by a dictionary that holds the default style values. To change the styling, a dictionary can be passed to the method by using the `user_options` argument. If this is done, the configurations that are defined in the user options overwrite the according default configurations. A reference and some more details concerning the options dictionary can be found below.
-
-```python
-# ex6
-
-options = {
-    "orientation": "LR",
-    "revert-relations": True,
-    "activity": {
-        "fill": "#89e6dc",
-        "shape": "{{:}}"
-    }
-}
-
-prov_ontology_graph.export_as_mermaid_flowchart(
-    file_name="examples/manual_examples_flowchart.md", 
-    user_options = options)
-```
-
-```mermaid
-flowchart LR
-classDef entity fill:#fffedf
-classDef entity color:#000000
-classDef entity stroke:#a4a4a4
-classDef entity stroke-width:1px
-classDef activity fill:#89e6dc
-classDef activity color:#000000
-classDef activity stroke:#a4a4a4
-classDef activity stroke-width:1px
-classDef agent fill:#ffebc3
-classDef agent color:#000000
-classDef agent stroke:#a4a4a4
-classDef agent stroke-width:1px
-http://example.org#example_entity([Example Entity]):::entity
-http://example.org#832b1ada-22f2-45b8-bdca-dfbe89fb68c8-- generated -->http://example.org#example_entity
-http://example.org#832b1ada-22f2-45b8-bdca-dfbe89fb68c8{{Anonymous activity}}:::activity
-```
-
-#### User Options Reference
-
-The default styling configuration mimics the graph styling from the PROV-O reference page and is defined as follows:
-
-```python
-options = {
-    "revert-relations": False,
-    "orientation": "TD",            
-    "included-relations": [
-        "was_generated_by",
-        "was_attributed_to",
-        "used",
-        "was_associated_with",
-        "acted_on_behalf_of"
-    ],
-    "color": "#000000",
-    "stroke": "#a4a4a4",
-    "stroke-width": "1px",
-    "relation-style": "-",
-    "entity": {
-        "fill": "#fffedf",
-        "shape": "([:])",
-        "relation-style": None,
-        "color": None,
-        "stroke": None,
-        "stroke-width": None
-    },
-    "activity": {
-        "fill": "#cfceff",
-        "shape": "[[:]]",
-        "relation-style": None,
-        "color": None,
-        "stroke": None,
-        "stroke-width": None
-    },
-    "agent": {
-        "fill": "#ffebc3",
-        "shape": "[/:\\]",
-        "relation-style": ".",
-        "color": None,
-        "stroke":  None,
-        "stroke-width": None
-    }
-}
-```
-
-__Reference Table__
-
-| keyword            | options                                     | explanation                                                                                                                                                                                                                                                          |
-|--------------------|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| revert-relations   | True \| False                               | Reverts the arrows and changes the labels accordingly. The reverted labels are not defined by PROV, and thus they are not compliant to the PROV model.                                                                                                               |
-| orientation        | "TD" \| "LR"                                | Top-down or left-right orientation of the graph (mermaid syntax).                                                                                                                                                                                                    |
-| included-relations | list of displayed relations                 | Defines which relations should be displayed. Per default "was_derived_by" and "was_informed_by" are excluded. Possible values are: "was_generated_by", was_derived_by", "was_attributed_to", "used", "was_informed_by", "was_associated_with", "acted_on_behalf_of". |
-| fill               | "\<#color-hex-code\>", e.g. "#fffedf" | Defines the color of the nodes.                                                                                                                                                                                                                                      |
-| shape              | "\<shape identifier\>", e.g. "[:]"            | Uses [mermaid shape syntax](https://mermaid-js.github.io/mermaid/#/flowchart?id=node-shapes). The colon separates the opening symbols from the closing symbols.                                                                                                      |
-| color              |  "\<#color-hex-code\>"                |  Defines the color of the nodes' texts.                                                                                                                                                                                                                              |
-|  stroke            |  "\<#color-hex-code\>"                |  Defines the color of the nodes' borders                                                                                                                                                                                                                             |
-|  stroke-width      |  "\<border width in px\>", e.g. "1px"         |  Defines the width of the nodes' borders.                                                                                                                                                                                                                            |
-| relation-style     | "-" (solid) \| "." (dashed)                 | Defines the style of the relations. Only two options are available.                                                                                                                                                                                                  |
-| entity             | dict                                        | Specify fill, shape, color, stroke, stroke-with and relation-style for entities. If any value is `None`, it falls back to the op level definitions                                                                                                                    |
-| activity           | dict                                        | see entity                                                                                                                                                                                                                                                           |
-| agent              | dict                                        | see entity                                                                                                                                                                                                                                                           |
-
-If further styling configuration is required, users have to interact directly with the resulting mermaid-md.
-
-
-## Comprehensive Examples
-
-Code to create the PROV-O [example 1](https://www.w3.org/TR/prov-o/#narrative-example-simple-1)
-
-```python
-from datetime import datetime
-
-from provo import ProvOntologyGraph
-from rdflib import FOAF, RDF, Literal, URIRef
-
-# create example from: https://www.w3.org/TR/prov-o/#narrative-example-simple-1
-
-
-# create graph
-prov_ontology_graph = ProvOntologyGraph(
-    namespace='http://example.org#',
-    namespace_abbreviation=""
-)
-
-# create entities
-crime_data = prov_ontology_graph.add_entity(
-    id_string='crimeData', 
-    label='Crime Data')
-national_regions_list = prov_ontology_graph.add_entity(
-    id_string='nationalRegionsList', 
-    label='National Regions List')
-aggregated_by_regions = prov_ontology_graph.add_entity(
-    id_string='aggregatedByRegions', 
-    label='Aggregated by Regions')
-bar_chart = prov_ontology_graph.add_entity(
-    id_string='bar_chart', 
-    label='Bar Chart')
-
-# create activities
-aggregation_activity = prov_ontology_graph.add_activity(
-    id_string='aggregationActivity', 
-    label='Aggregation Activity')
-illustration_activity = prov_ontology_graph.add_activity(
-    ='illustrationActivity', 
-    label='Illustration Activity')
-
-# create agents
-government = prov_ontology_graph.add_agent(
-    id_string='government', 
-    label='Government')
-civil_action_group = prov_ontology_graph.add_agent(
-    id_string='civil_action_group', 
-    label='Civil Action Group')
-national_newspaper_inc = prov_ontology_graph.add_agent(
-    id_string='national_newspaper_inc', 
-    label='National Newspaper Inc.')
-derek = prov_ontology_graph.add_agent(
-    id_string='derek', 
-    label='Derek')
-
-# build relations
-crime_data.was_attributed_to(government)
-national_regions_list.was_attributed_to(civil_action_group)
-
-aggregation_activity.used(crime_data)
-aggregation_activity.used(national_regions_list)
-aggregation_activity.started_at_time(datetime(2011, 7, 14, 1, 1, 1))
-aggregation_activity.ended_at_time(datetime(2011, 7, 14, 2, 2, 2))
-aggregation_activity.was_associated_with(derek)
-
-aggregated_by_regions.was_generated_by(aggregation_activity)
-aggregated_by_regions.was_attributed_to(derek)
-
-illustration_activity.was_informed_by(aggregation_activity)
-illustration_activity.used(aggregated_by_regions)
-illustration_activity.was_associated_with(derek)
-
-bar_chart.was_generated_by(illustration_activity)
-bar_chart.was_derived_from(aggregated_by_regions)
-bar_chart.was_attributed_to(derek)
-
-derek.acted_on_behalf_of(national_newspaper_inc)
-
-# print graph to terminal
-print(prov_ontology_graph)
-
-# use rdflib interface to add FOAF triples
-rdflib_graph = prov_ontology_graph.get_rdflib_graph()
-
-rdflib_graph.bind("foaf", FOAF)
-
-rdflib_graph.add((
-    URIRef(government.get_id()),
-    RDF.type,
-    FOAF.Organization
-))
-
-rdflib_graph.add((
-    URIRef(civil_action_group.get_id()),
-    RDF.type,
-    FOAF.Organization
-))
-
-rdflib_graph.add((
-    URIRef(national_newspaper_inc.get_id()),
-    RDF.type,
-    FOAF.Organization
-))
-
-rdflib_graph.add((
-    URIRef(national_newspaper_inc.get_id()),
-    FOAF.name,
-    Literal(national_newspaper_inc.get_label(), lang="en")
-))
-
-rdflib_graph.add((
-    URIRef(derek.get_id()),
-    RDF.type,
-    FOAF.Person
-))
-
-rdflib_graph.add((
-    URIRef(derek.get_id()),
-    FOAF.givenName,
-    Literal(derek.get_label(), lang="en")
-))
-
-rdflib_graph.add((
-    URIRef(derek.get_id()),
-    FOAF.mbox,
-    URIRef("mailto:derek@example.org")
-))
-# serialize graph as rdf document
-rdflib_graph.serialize('examples/provenance_graph_example.ttl')
-
-
-
-# export mermaid-md with default_options
-prov_ontology_graph.export_as_mermaid_flowchart(file_name="examples/provenance_mermaid_default.md")
-
-# with adjusted options
-# prov_ontology_graph.export_as_mermaid_flowchart(
-#     file_name="examples/provenance_mermaid.md",
-#     user_options=options)
-
-```
-
-__Default mermaid graph:__
-```mermaid
-flowchart TD
-classDef entity fill:#fffedf
-classDef entity color:#000000
-classDef entity stroke:#a4a4a4
-classDef entity stroke-width:1px
-classDef activity fill:#cfceff
-classDef activity color:#000000
-classDef activity stroke:#a4a4a4
-classDef activity stroke-width:1px
-classDef agent fill:#ffebc3
-classDef agent color:#000000
-classDef agent stroke:#a4a4a4
-classDef agent stroke-width:1px
-http://example.org#crimeData([Crime Data]):::entity
-http://example.org#crimeData-. was attributed to .->http://example.org#government
-http://example.org#nationalRegionsList([National Regions List]):::entity
-http://example.org#nationalRegionsList-. was attributed to .->http://example.org#civil_action_group
-http://example.org#aggregatedByRegions([Aggregated by Regions]):::entity
-http://example.org#aggregatedByRegions-- was generated by -->http://example.org#aggregationActivity
-http://example.org#aggregatedByRegions-. was attributed to .->http://example.org#derek
-http://example.org#bar_chart([Bar Chart]):::entity
-http://example.org#bar_chart-- was generated by -->http://example.org#illustrationActivity
-http://example.org#bar_chart-. was attributed to .->http://example.org#derek
-http://example.org#aggregationActivity[[Aggregation Activity]]:::activity
-http://example.org#aggregationActivity-- used -->http://example.org#crimeData
-http://example.org#aggregationActivity-- used -->http://example.org#nationalRegionsList
-http://example.org#aggregationActivity-. was associated with .->http://example.org#derek
-http://example.org#illustrationActivity[[Illustration Activity]]:::activity
-http://example.org#illustrationActivity-- used -->http://example.org#aggregatedByRegions
-http://example.org#illustrationActivity-. was associated with .->http://example.org#derek
-http://example.org#government[/Government\]:::agent
-http://example.org#civil_action_group[/Civil Action Group\]:::agent
-http://example.org#national_newspaper_inc[/National Newspaper Inc.\]:::agent
-http://example.org#derek[/Derek\]:::agent
-http://example.org#derek-. acted on behalf of .->http://example.org#national_newspaper_inc
-```
-
-__User defined mermaid graph:__
-
-```python
-options = {
-    "revert-relations": True,
-    "entity": {
-        "shape": "[:]",
-        "fill": "#FC766AFF",
-        "stroke": "#FC766AFF",
-        "color": "333"
-    },
-    "agent": {
-        "shape": "[/:\\]",
-        "stroke":"#B0B8B4FF",
-        "fill": "#B0B8B4FF",               
-        "color": "333",
-        "relation-style": "."
-    },
-    "activity": {
-        "shape": "{{:}}",
-        "fill": "#184A45FF",
-        "stroke": "#184A45FF",
-        "color": "#eee"       
-    }
-}
-```
-
-```mermaid
-flowchart TD
-classDef entity fill:#FC766AFF
-classDef entity color:333
-classDef entity stroke:#FC766AFF
-classDef entity stroke-width:1px
-classDef activity fill:#184A45FF
-classDef activity color:#eee
-classDef activity stroke:#184A45FF
-classDef activity stroke-width:1px
-classDef agent fill:#B0B8B4FF
-classDef agent color:333
-classDef agent stroke:#B0B8B4FF
-classDef agent stroke-width:1px
-http://example.org#crimeData[Crime Data]:::entity
-http://example.org#government-. produced .->http://example.org#crimeData
-http://example.org#nationalRegionsList[National Regions List]:::entity
-http://example.org#civil_action_group-. produced .->http://example.org#nationalRegionsList
-http://example.org#aggregatedByRegions[Aggregated by Regions]:::entity
-http://example.org#aggregationActivity-- generated -->http://example.org#aggregatedByRegions
-http://example.org#derek-. produced .->http://example.org#aggregatedByRegions
-http://example.org#bar_chart[Bar Chart]:::entity
-http://example.org#illustrationActivity-- generated -->http://example.org#bar_chart
-http://example.org#derek-. produced .->http://example.org#bar_chart
-http://example.org#aggregationActivity{{Aggregation Activity}}:::activity
-http://example.org#crimeData-- was used by -->http://example.org#aggregationActivity
-http://example.org#nationalRegionsList-- was used by -->http://example.org#aggregationActivity
-http://example.org#derek-. initiated .->http://example.org#aggregationActivity
-http://example.org#illustrationActivity{{Illustration Activity}}:::activity
-http://example.org#aggregatedByRegions-- was used by -->http://example.org#illustrationActivity
-http://example.org#derek-. initiated .->http://example.org#illustrationActivity
-http://example.org#government[/Government\]:::agent
-http://example.org#civil_action_group[/Civil Action Group\]:::agent
-http://example.org#national_newspaper_inc[/National Newspaper Inc.\]:::agent
-http://example.org#derek[/Derek\]:::agent
-http://example.org#national_newspaper_inc-. instructed .->http://example.org#derek
-```
-
-
-## Contact
-
-Arne Rümmler ([arne.ruemmler@gmail.com](mailto:arne.ruemmler@gmail.com))
+# README
+
+The package supports the creation of [PROV-O](https://www.w3.org/TR/prov-o/) compliant provenance graphs.
+
+
+
+## Installation
+
+You can install the package from the Python Package Index (PyPI):
+
+`pip install provo`
+
+Or by downloading this repository:
+
+1. Download and unzip the repository
+2. Open Shell and _cd_ to unzipped repository
+3. Run `pip install -e .` (in the folder that contains ```setup.py```)
+
+## Contents
+
+The package is a Python API to PROV-O. It implements the [PROV-O starting point classes](https://www.w3.org/TR/prov-o/#starting-points-figure) __Entity__, __Activity__ and __Agent__ as Python classes with methods to establish the _PROV-O starting point properties_ between instances of these classes.
+
+## Features
+
+The package's objective is to support the programmatical creation of provenance graphs that are compliant with the W3C Recommendation PROV-O: The PROV Ontology. Users of the package shall be enabled to tightly couple the generation of data with the generation of their provenance. As the package implements PROV-O, the created graph is exportable as an RDF document. Finally, the graph can be exported as a mermaid flowchart with some configuration options to adjust the style of the resulting chart.
+
+### Compliance
+
+- The PROV-O classes __Entity__, __Activity__, and __Agent__ are implemented as Python classes.
+- The PROV-O properties _wasGeneratedBy_, _wasDerivedFrom_, _wasAttributedTo_, _startedAtTime_, _used_, _wasInformedBy_, _endedAtTime_, _wasAssociatedWith_, and _actedOnBehalfOf_ are implemented as instance methods of their according classes.
+- Attributes that are passed to these methods are type-checked to enforce compliance with PROV-O.
+- Node Ids are checked for validity.
+- Use of the same ID for different objects throws an error.
+
+### Ease of Use
+
+- IDE support is provided via the implementation as Python classes according methods, and through type hints.
+- The classes `Provence_Ontology_Graph`, `Entity`, `Activity`, and `Agent` can be printed to terminal in a user-friendly, readable way with the default `print()` command.
+- Objects of the classes `Entity`, `Activity`, and `Agent` can be instantiated with auto-generated Ids (although it's not recommended using this for production).
+- Export as [mermaid flowchart](https://mermaid-js.github.io/mermaid/#/flowchart) to review the graph visually.
+
+### Interface to RDF via the [rdflib](https://rdflib.readthedocs.io/en/stable/) package
+
+- The graph's contents can be converted to an `rdflib.Graph` object.
+- The graph can be exported in various RDF serializations.
+
+## Manual
+
+The package is centered around the class `ProvenanceOntologyGraph`. Entities, Activities, and Agents are added to this graph using the according class methods. Relations between the PROV-O class objects are constructed using their respective class methods.
+
+### Create a Provenance Ontology Graph
+
+The graph can be initialized with default or user defined attributes. The graph can be printed to the terminal with `print(graph)`.
+
+```python
+# ex1 - create a provenance graph
+from provo import ProvOntologyGraph
+
+# __defaults__
+# namespace: str = "https://provo-example.org/",
+# namespace_abbreviation: str = "", 
+# lang: str = "en"
+provenance_graph = ProvOntologyGraph()
+
+prov_ontology_graph = ProvOntologyGraph(
+    namespace='http://example.org#',
+    namespace_abbreviation="ex",
+    lang="en"
+)
+```
+
+`namespace=`
+
+- Default is `"https://provo-example.org/"`.
+- Has to be valid url, validation is currently performed with the [validators](https://pypi.org/project/validators/) package.
+- Has to end with `/` or `#`.
+
+`namespace_abbreviation=`
+
+- Default is `""`.
+- Used when converting to other models, such as RDF (-> prefixes)
+- Only characters from the Latin alphabet are allowed.
+- RDF core prefixes (*owl*, *rdf*, *rdfs*, *xsd* and *xml*) are prohibited from use.
+
+>**Note** 
+> Although not prohibited, the following prefixes are commonly used and thus recommended being avoided: *brick*, *csvw*, *dc*, *dcat*, *dcmitype*, *cdterms*, *dcam*, *doap*, *foaf*, *geo*, *odrl*, *org*, *prof*, *prov*, *qb*, *sdo*, *sh*, *skos*, *sosa*, *ssn*, *time*, *vann* and *void*.
+
+`lang=`
+
+- Default is `"en"`.
+- Used when converting to other models that support a *lang* tag.
+- Has to be compliant with [RFC 5646](https://www.rfc-editor.org/info/rfc5646) (Phillips, A., Ed., and M. Davis, Ed., "Tags for Identifying Languages", BCP 47, RFC 5646, September 2009). Compliance is not validated!
+
+### Create Entities, Activities and Agents and define relations between them
+
+The creation for classes follows the same pattern. The classes only differ in their methods. PROV-O Classes are instantiated by using the add methods of the provenance graph class. Below you find the `add_entity()` method of `ProvenanceOntologyGraph` for reference.
+
+```python
+# definition of add_entity() in ProvOntologyGraph()
+def add_entity(self, 
+    id: str = "", 
+    label: str = "", 
+    description: str = "", 
+    use_namespace: bool = False) -> Entity:
+    """creates a new entity, adds it to the graph and returns it then"""
+    # if use_namespace is set to True, the given id is concatenated with the namespace that was defined at the creation of the ProvenanceOntologyGraph object.
+    # The method _handle_id() checks whether the provided 
+    # namespace-id combination is already used for a node in the graph and if it is a valid IRI. 
+    # if no id is provided: id gets automatically generated, within the namespace of the ProvenanceOntologyGraph (Setting use_namespace to True and not providing an id, still creates a valid IRI).
+    
+    node_id = self._handle_id(id, use_namespace)
+    # the PROV class (in this case an Entity) is only created if everything with the ID is fine
+    entity = Entity(node_id=node_id, label=label,description=description)
+    self._entities.append(entity)
+    return entity
+```
+
+The relations are defined by calling the respective methods of the PROV class instances.
+
+Example use of the provenance graph's add-methods and the definition of a *used*-relation between an Activity and an Entity:
+
+```python
+# ex2 - create entities, activities and agents, 
+# and define relation between them
+entity = prov_ontology_graph.add_entity(
+    id="example_entity",
+    label="Example Entity",
+    use_namespace=True)
+
+activity = prov_ontology_graph.add_activity(
+    label="Anonymous activity",
+    description="An arbitrary activity."
+)
+
+entity.was_generated_by(activity)
+
+print(entity)
+# id: http://example.org#example_entity
+# label: Example Entity
+# was generated by: ['Anonymous activity']
+# ---
+
+print(activity)
+# id: http://example.org#94021a6a-40cd-4c02-9571-33480488ff82
+# label: Anonymous activity
+# description: An arbitrary activity.
+# ---
+```
+
+### RDF interface
+
+The graph can be directly serialized as RDF document or be converted to an `rdflib` Graph, for further manipulation.
+
+```python
+# ex3 - serialize provenance graph as RDF document
+prov_ontology_graph.serialize_as_rdf("manual_examples.ttl")
+```
+
+```
+@prefix : <http://example.org#> .
+@prefix prov: <http://www.w3.org/ns/prov#> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+
+:example_entity a prov:Entity ;
+    rdfs:label "Example Entity"@en ;
+    prov:wasGeneratedBy :832b1ada-22f2-45b8-bdca-dfbe89fb68c8 .
+
+:832b1ada-22f2-45b8-bdca-dfbe89fb68c8 a prov:Activity ;
+    rdfs:label "Anonymous activity"@en ;
+    rdfs:comment "An arbitrary activity."@en .
+```
+
+```python
+# ex4 - interface with rdflib
+
+from rdflib import SKOS, Literal, URIRef
+
+rdflib_graph = prov_ontology_graph.get_rdflib_graph()
+
+rdflib_graph.bind("skos", SKOS)
+
+rdflib_graph.add((
+    URIRef(entity.node_id), 
+    SKOS.prefLabel, 
+    Literal(entity.label, lang="en")
+))
+
+rdflib_graph.serialize("examples/rdflib_interface.ttl")
+```
+```
+@prefix : <http://example.org#> .
+@prefix prov: <http://www.w3.org/ns/prov#> .
+@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
+@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
+
+:example_entity a prov:Entity ;
+    rdfs:label "Example Entity"@en ;
+    skos:prefLabel "Example Entity"@en ;
+    prov:wasGeneratedBy :832b1ada-22f2-45b8-bdca-dfbe89fb68c8 .
+
+:832b1ada-22f2-45b8-bdca-dfbe89fb68c8 a prov:Activity ;
+    rdfs:label "Anonymous activity"@en ;
+    rdfs:comment "An arbitrary activity."@en .
+```
+
+### Export as Mermaid Flowchart
+
+Mermaid is a"[...] diagramming and charting tool that renders Markdown-inspired text definitions [...]". It can be embedded in markdown documents like so:
+
+````markdown
+```mermaid
+flowchart LR
+    entity_id[Entity] -- was generated by --> activity_id[Activity]
+```
+````
+
+If the markdown interpreter supports mermaid, this results in:
+
+```mermaid
+flowchart LR
+    entity_id[Entity] -- was generated by --> activity_id[Activity]
+```
+
+To export the provenance graph as mermaid chart call the according export method:
+
+```python
+# ex5
+
+prov_ontology_graph.export_as_mermaid_flowchart(file_name="examples/manual_examples_flowchart_default.md")
+```
+
+```mermaid
+flowchart TD
+classDef entity fill:#fffedf
+classDef entity color:#000000
+classDef entity stroke:#a4a4a4
+classDef entity stroke-width:1px
+classDef activity fill:#cfceff
+classDef activity color:#000000
+classDef activity stroke:#a4a4a4
+classDef activity stroke-width:1px
+classDef agent fill:#ffebc3
+classDef agent color:#000000
+classDef agent stroke:#a4a4a4
+classDef agent stroke-width:1px
+http://example.org#example_entity([Example Entity]):::entity
+http://example.org#example_entity-- was generated by -->http://example.org#832b1ada-22f2-45b8-bdca-dfbe89fb68c8
+http://example.org#832b1ada-22f2-45b8-bdca-dfbe89fb68c8[[Anonymous activity]]:::activity
+```
+
+The style of the resulting graph is defined by a dictionary that holds the default style values. To change the styling, a dictionary can be passed to the method by using the `user_options` argument. If this is done, the configurations that are defined in the user options overwrite the according default configurations. A reference and some more details concerning the options dictionary can be found below.
+
+```python
+# ex6
+
+options = {
+    "orientation": "LR",
+    "revert-relations": True,
+    "activity": {
+        "fill": "#89e6dc",
+        "shape": "{{:}}"
+    }
+}
+
+prov_ontology_graph.export_as_mermaid_flowchart(
+    file_name="examples/manual_examples_flowchart.md", 
+    user_options = options)
+```
+
+```mermaid
+flowchart LR
+classDef entity fill:#fffedf
+classDef entity color:#000000
+classDef entity stroke:#a4a4a4
+classDef entity stroke-width:1px
+classDef activity fill:#89e6dc
+classDef activity color:#000000
+classDef activity stroke:#a4a4a4
+classDef activity stroke-width:1px
+classDef agent fill:#ffebc3
+classDef agent color:#000000
+classDef agent stroke:#a4a4a4
+classDef agent stroke-width:1px
+http://example.org#example_entity([Example Entity]):::entity
+http://example.org#832b1ada-22f2-45b8-bdca-dfbe89fb68c8-- generated -->http://example.org#example_entity
+http://example.org#832b1ada-22f2-45b8-bdca-dfbe89fb68c8{{Anonymous activity}}:::activity
+```
+
+To adjust details and to generate PNGs or SVGs you can copy the mermaid graph content to the [Mermaid Live Editor](https://mermaid.live/).
+
+#### User Options Reference
+
+The default styling configuration mimics the graph styling from the PROV-O reference page and is defined as follows:
+
+```python
+options = {
+    "revert-relations": False,
+    "orientation": "TD",            
+    "included-relations": [
+        "was_generated_by",
+        "was_attributed_to",
+        "used",
+        "was_associated_with",
+        "acted_on_behalf_of"
+    ],
+    "color": "#000000",
+    "stroke": "#a4a4a4",
+    "stroke-width": "1px",
+    "relation-style": "-",
+    "entity": {
+        "fill": "#fffedf",
+        "shape": "([:])",
+        "relation-style": None,
+        "color": None,
+        "stroke": None,
+        "stroke-width": None
+    },
+    "activity": {
+        "fill": "#cfceff",
+        "shape": "[[:]]",
+        "relation-style": None,
+        "color": None,
+        "stroke": None,
+        "stroke-width": None
+    },
+    "agent": {
+        "fill": "#ffebc3",
+        "shape": "[/:\\]",
+        "relation-style": ".",
+        "color": None,
+        "stroke":  None,
+        "stroke-width": None
+    }
+}
+```
+
+__Reference Table__
+
+| keyword            | options                                     | explanation                                                                                                                                                                                                                                                          |
+|--------------------|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| revert-relations   | True \| False                               | Reverts the arrows and changes the labels accordingly. The reverted labels are not defined by PROV, and thus they are not compliant to the PROV model.                                                                                                               |
+| orientation        | "TD" \| "LR"                                | Top-down or left-right orientation of the graph (mermaid syntax).                                                                                                                                                                                                    |
+| included-relations | list of displayed relations                 | Defines which relations should be displayed. Per default "was_derived_by" and "was_informed_by" are excluded. Possible values are: "was_generated_by", was_derived_by", "was_attributed_to", "used", "was_informed_by", "was_associated_with", "acted_on_behalf_of". |
+| fill               | "\<#color-hex-code\>", e.g. "#fffedf" | Defines the color of the nodes.                                                                                                                                                                                                                                      |
+| shape              | "\<shape identifier\>", e.g. "[:]"            | Uses [mermaid shape syntax](https://mermaid-js.github.io/mermaid/#/flowchart?id=node-shapes). The colon separates the opening symbols from the closing symbols.                                                                                                      |
+| color              |  "\<#color-hex-code\>"                |  Defines the color of the nodes' texts.                                                                                                                                                                                                                              |
+|  stroke            |  "\<#color-hex-code\>"                |  Defines the color of the nodes' borders                                                                                                                                                                                                                             |
+|  stroke-width      |  "\<border width in px\>", e.g. "1px"         |  Defines the width of the nodes' borders.                                                                                                                                                                                                                            |
+| relation-style     | "-" (solid) \| "." (dashed)                 | Defines the style of the relations. Only two options are available.                                                                                                                                                                                                  |
+| entity             | dict                                        | Specify fill, shape, color, stroke, stroke-with and relation-style for entities. If any value is `None`, it falls back to the op level definitions                                                                                                                    |
+| activity           | dict                                        | see entity                                                                                                                                                                                                                                                           |
+| agent              | dict                                        | see entity                                                                                                                                                                                                                                                           |
+
+If further styling configuration is required, users have to interact directly with the resulting mermaid-md.
+
+
+## Comprehensive Examples
+
+Code to create the PROV-O [example 1](https://www.w3.org/TR/prov-o/#narrative-example-simple-1)
+
+```python
+from datetime import datetime
+
+from provo import ProvOntologyGraph
+from rdflib import FOAF, RDF, Literal, URIRef
+
+# create example from: https://www.w3.org/TR/prov-o/#narrative-example-simple-1
+
+
+# create graph
+prov_ontology_graph = ProvOntologyGraph(
+    namespace='http://example.org#',
+    namespace_abbreviation=""
+)
+
+# create entities
+crime_data = prov_ontology_graph.add_entity(
+    id='crimeData', 
+    label='Crime Data',
+    use_namespace=True)
+national_regions_list = prov_ontology_graph.add_entity(
+    id='nationalRegionsList', 
+    label='National Regions List',
+    use_namespace=True)
+aggregated_by_regions = prov_ontology_graph.add_entity(
+    id='aggregatedByRegions', 
+    label='Aggregated by Regions',
+    use_namespace=True)
+bar_chart = prov_ontology_graph.add_entity(
+    id='bar_chart', 
+    label='Bar Chart',
+    use_namespace=True)
+
+# create activities
+aggregation_activity = prov_ontology_graph.add_activity(
+    id='aggregationActivity', 
+    label='Aggregation Activity',
+    use_namespace=True)
+illustration_activity = prov_ontology_graph.add_activity(
+    id='illustrationActivity', 
+    label='Illustration Activity',
+    use_namespace=True)
+
+# create agents
+government = prov_ontology_graph.add_agent(
+    id='government', 
+    label='Government',
+    use_namespace=True)
+civil_action_group = prov_ontology_graph.add_agent(
+    id='civil_action_group', 
+    label='Civil Action Group',
+    use_namespace=True)
+national_newspaper_inc = prov_ontology_graph.add_agent(
+    id='national_newspaper_inc', 
+    label='National Newspaper Inc.',
+    use_namespace=True)
+derek = prov_ontology_graph.add_agent(
+    id='derek', 
+    label='Derek',
+    use_namespace=True)
+
+# build relations
+crime_data.was_attributed_to(government)
+national_regions_list.was_attributed_to(civil_action_group)
+
+aggregation_activity.used(crime_data)
+aggregation_activity.used(national_regions_list)
+aggregation_activity.started_at_time(datetime(2011, 7, 14, 1, 1, 1))
+aggregation_activity.ended_at_time(datetime(2011, 7, 14, 2, 2, 2))
+aggregation_activity.was_associated_with(derek)
+
+aggregated_by_regions.was_generated_by(aggregation_activity)
+aggregated_by_regions.was_attributed_to(derek)
+
+illustration_activity.was_informed_by(aggregation_activity)
+illustration_activity.used(aggregated_by_regions)
+illustration_activity.was_associated_with(derek)
+
+bar_chart.was_generated_by(illustration_activity)
+bar_chart.was_derived_from(aggregated_by_regions)
+bar_chart.was_attributed_to(derek)
+
+derek.acted_on_behalf_of(national_newspaper_inc)
+
+# print graph to terminal
+print(prov_ontology_graph)
+
+# use rdflib interface to add FOAF triples
+rdflib_graph = prov_ontology_graph.get_rdflib_graph()
+
+rdflib_graph.bind("foaf", FOAF)
+
+rdflib_graph.add((
+    URIRef(government.node_id),
+    RDF.type,
+    FOAF.Organization
+))
+
+rdflib_graph.add((
+    URIRef(civil_action_group.node_id),
+    RDF.type,
+    FOAF.Organization
+))
+
+rdflib_graph.add((
+    URIRef(national_newspaper_inc.node_id),
+    RDF.type,
+    FOAF.Organization
+))
+
+rdflib_graph.add((
+    URIRef(national_newspaper_inc.node_id),
+    FOAF.name,
+    Literal(national_newspaper_inc.label, lang="en")
+))
+
+rdflib_graph.add((
+    URIRef(derek.node_id),
+    RDF.type,
+    FOAF.Person
+))
+
+rdflib_graph.add((
+    URIRef(derek.node_id),
+    FOAF.givenName,
+    Literal(derek.label, lang="en")
+))
+
+rdflib_graph.add((
+    URIRef(derek.node_id),
+    FOAF.mbox,
+    URIRef("mailto:derek@example.org")
+))
+# serialize graph as rdf document
+rdflib_graph.serialize('examples/provenance_graph_example.ttl')
+
+
+
+# export mermaid-md with default_options
+prov_ontology_graph.export_as_mermaid_flowchart(file_name="examples/provenance_mermaid_default.md")
+
+# with adjusted options
+# prov_ontology_graph.export_as_mermaid_flowchart(
+#     file_name="examples/provenance_mermaid.md",
+#     user_options=options)
+
+```
+
+__Default mermaid graph:__
+```mermaid
+flowchart TD
+classDef entity fill:#fffedf
+classDef entity color:#000000
+classDef entity stroke:#a4a4a4
+classDef entity stroke-width:1px
+classDef activity fill:#cfceff
+classDef activity color:#000000
+classDef activity stroke:#a4a4a4
+classDef activity stroke-width:1px
+classDef agent fill:#ffebc3
+classDef agent color:#000000
+classDef agent stroke:#a4a4a4
+classDef agent stroke-width:1px
+http://example.org#crimeData([Crime Data]):::entity
+http://example.org#crimeData-. was attributed to .->http://example.org#government
+http://example.org#nationalRegionsList([National Regions List]):::entity
+http://example.org#nationalRegionsList-. was attributed to .->http://example.org#civil_action_group
+http://example.org#aggregatedByRegions([Aggregated by Regions]):::entity
+http://example.org#aggregatedByRegions-- was generated by -->http://example.org#aggregationActivity
+http://example.org#aggregatedByRegions-. was attributed to .->http://example.org#derek
+http://example.org#bar_chart([Bar Chart]):::entity
+http://example.org#bar_chart-- was generated by -->http://example.org#illustrationActivity
+http://example.org#bar_chart-. was attributed to .->http://example.org#derek
+http://example.org#aggregationActivity[[Aggregation Activity]]:::activity
+http://example.org#aggregationActivity-- used -->http://example.org#crimeData
+http://example.org#aggregationActivity-- used -->http://example.org#nationalRegionsList
+http://example.org#aggregationActivity-. was associated with .->http://example.org#derek
+http://example.org#illustrationActivity[[Illustration Activity]]:::activity
+http://example.org#illustrationActivity-- used -->http://example.org#aggregatedByRegions
+http://example.org#illustrationActivity-. was associated with .->http://example.org#derek
+http://example.org#government[/Government\]:::agent
+http://example.org#civil_action_group[/Civil Action Group\]:::agent
+http://example.org#national_newspaper_inc[/National Newspaper Inc.\]:::agent
+http://example.org#derek[/Derek\]:::agent
+http://example.org#derek-. acted on behalf of .->http://example.org#national_newspaper_inc
+```
+
+__User defined mermaid graph:__
+
+```python
+options = {
+    "revert-relations": True,
+    "entity": {
+        "shape": "[:]",
+        "fill": "#FC766AFF",
+        "stroke": "#FC766AFF",
+        "color": "333"
+    },
+    "agent": {
+        "shape": "[/:\\]",
+        "stroke":"#B0B8B4FF",
+        "fill": "#B0B8B4FF",               
+        "color": "333",
+        "relation-style": "."
+    },
+    "activity": {
+        "shape": "{{:}}",
+        "fill": "#184A45FF",
+        "stroke": "#184A45FF",
+        "color": "#eee"       
+    }
+}
+```
+
+```mermaid
+flowchart TD
+classDef entity fill:#FC766AFF
+classDef entity color:333
+classDef entity stroke:#FC766AFF
+classDef entity stroke-width:1px
+classDef activity fill:#184A45FF
+classDef activity color:#eee
+classDef activity stroke:#184A45FF
+classDef activity stroke-width:1px
+classDef agent fill:#B0B8B4FF
+classDef agent color:333
+classDef agent stroke:#B0B8B4FF
+classDef agent stroke-width:1px
+http://example.org#crimeData[Crime Data]:::entity
+http://example.org#government-. produced .->http://example.org#crimeData
+http://example.org#nationalRegionsList[National Regions List]:::entity
+http://example.org#civil_action_group-. produced .->http://example.org#nationalRegionsList
+http://example.org#aggregatedByRegions[Aggregated by Regions]:::entity
+http://example.org#aggregationActivity-- generated -->http://example.org#aggregatedByRegions
+http://example.org#derek-. produced .->http://example.org#aggregatedByRegions
+http://example.org#bar_chart[Bar Chart]:::entity
+http://example.org#illustrationActivity-- generated -->http://example.org#bar_chart
+http://example.org#derek-. produced .->http://example.org#bar_chart
+http://example.org#aggregationActivity{{Aggregation Activity}}:::activity
+http://example.org#crimeData-- was used by -->http://example.org#aggregationActivity
+http://example.org#nationalRegionsList-- was used by -->http://example.org#aggregationActivity
+http://example.org#derek-. initiated .->http://example.org#aggregationActivity
+http://example.org#illustrationActivity{{Illustration Activity}}:::activity
+http://example.org#aggregatedByRegions-- was used by -->http://example.org#illustrationActivity
+http://example.org#derek-. initiated .->http://example.org#illustrationActivity
+http://example.org#government[/Government\]:::agent
+http://example.org#civil_action_group[/Civil Action Group\]:::agent
+http://example.org#national_newspaper_inc[/National Newspaper Inc.\]:::agent
+http://example.org#derek[/Derek\]:::agent
+http://example.org#national_newspaper_inc-. instructed .->http://example.org#derek
+```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `provo-1.0.5/provo/provontologygraph.py` & `provo-1.1.0/provo/provontologygraph.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,560 +1,570 @@
-"""
-@author Arne Rümmler
-@contact arne.ruemmler@gmail.com
-
-@summary Implementation of a provenance graph
-    class that uses PROV-O terms
-"""
-
-
-from dataclasses import dataclass, field
-
-from rdflib import (
-    DC,
-    FOAF,
-    PROV,
-    RDF,
-    RDFS,
-    XSD,
-    Graph,  # type: ignore
-    Literal,
-    Namespace,
-    URIRef,
-)
-from validators import url
-
-from provo.idvault import IdVault
-from provo.startingpointclasses import Activity, Agent, Entity
-from provo.staticfunctions import update_dict
-
-
-@dataclass(frozen=True)
-class NamespaceMalformed(Exception):
-    """Raised when the namespace is not a valid URL."""
-
-    message: str
-
-
-@dataclass(frozen=True)
-class NamespaceHasNoEndSymbol(Exception):
-    """Raised if the namespace does not end with '/' or '#'."""
-
-    message: str
-
-
-@dataclass(frozen=True)
-class PrefixShorthandNotValid(Exception):
-    """Raised if the namespace abbreviation contains non-allowed characters."""
-
-    message: str
-
-
-@dataclass(frozen=True)
-class PrefixNotAllowed(Exception):
-    """Raised the namespace is not allowed."""
-
-    message: str
-
-
-@dataclass
-class ProvOntologyGraph:
-    """model that manages contents of a provenance graph
-    that adheres to the PROV-O provenance model."""
-
-    namespace: str = "https://provo-example.org/"
-    namespace_abbreviation: str = ""
-    lang: str = "en"
-    _entities: list[Entity] = field(init=False, default_factory=list)
-    _activities: list[Activity] = field(init=False, default_factory=list)
-    _agents: list[Agent] = field(init=False, default_factory=list)
-    _id_vault: IdVault = field(init=False, default_factory=IdVault)
-
-    def __post_init__(self):
-        """check validity of namespace and and namespace abbreviation"""
-
-        # validate namespace
-        # TODO rethink validation
-        if not url(self.namespace):  # type: ignore
-            raise NamespaceMalformed(
-                """
-            The provided namespace is not a valid URL!
-
-            See validators package (https://github.com/python-validators/validators),
-            validators.url() or https://gist.github.com/dperini/729294 for more
-            information on what qualifies a URL as valid.
-            
-            https://www.rfc-editor.org/rfc/rfc3986#section-3:
-            3.  Syntax Components
-
-            The generic URI syntax consists of a hierarchical sequence of
-            components referred to as the scheme, authority, path, query, and
-            fragment.
-
-                URI         = scheme ":" hier-part [ "?" query ] [ "#" fragment ]
-
-                hier-part   = "//" authority path-abempty
-                            / path-absolute
-                            / path-rootless
-                            / path-empty
-
-            The scheme and path components are required, though the path may be
-            empty (no characters).  When authority is present, the path must
-            either be empty or begin with a slash ("/") character.  When
-            authority is not present, the path cannot begin with two slash
-            characters ("//").  These restrictions result in five different ABNF
-            rules for a path (Section 3.3), only one of which will match any
-            given URI reference.
-
-            The following are two example URIs and their component parts:
-
-                    foo://example.com:8042/over/there?name=ferret#nose
-                    \_/   \______________/\_________/ \_________/ \__/
-                    |           |            |            |        |
-                scheme     authority       path        query   fragment
-                    |   _____________________|__
-                    / \ /                        \
-                    urn:example:animal:ferret:nose
-            """
-            )
-        end_symbol = self.namespace[-1]
-        if end_symbol not in ("/", "#"):
-            raise NamespaceHasNoEndSymbol(
-                "The provided Namespace has to end on a '/' or '#'!"
-            )
-
-        # validate namespace abbreviation
-        # TODO check what is actually allowed
-        allowed_symbols_for_prefix_shorthand = "abcdefghijklmnopqrstuvwxyz"
-
-        for symbol in self.namespace_abbreviation:
-            if symbol not in allowed_symbols_for_prefix_shorthand:
-                raise PrefixShorthandNotValid(
-                    f"""
-                    The provided namespace abbreviation is not valid.
-                    
-                    Character of the namespace have to be in "{allowed_symbols_for_prefix_shorthand}".
-                    """
-                )
-        # if self.namespace_abbreviation in forbidden_namespaces:
-        core_prefixes = ["owl", "rdf", "rdfs", "xsd", "xml"]
-        if self.namespace_abbreviation in core_prefixes:
-            raise PrefixNotAllowed(
-                f"""
-            The provided namespace abbreviation is a core prefix, 
-            and thus, prohibited from use.
-
-            Core prefixes are: {"".join([f"{k}, " if i != len(core_prefixes)-2 else f"{k} and " for i, k in enumerate(core_prefixes)])[:-2]}.
-            """
-            )
-
-    def __str__(self) -> str:
-        """prints the contents of the provenance graph in a nice format."""
-        contents = "Provenance Graph Contents:"
-        contents += "\n    ---"
-        contents += "\n    Entities:"
-        contents += "\n        ---\n"
-        for entity in self._entities:
-            lines = entity.__str__().splitlines()
-            for line in lines:
-                contents += f"        {line}\n"
-        contents += "    ---"
-        contents += "\n    Activities:"
-        contents += "\n        ---\n"
-        for activity in self._activities:
-            lines = activity.__str__().splitlines()
-            for line in lines:
-                contents += f"        {line}\n"
-        contents += "    ---"
-        contents += "\n    Agents:"
-        contents += "\n        ---\n"
-        for agent in self._agents:
-            lines = agent.__str__().splitlines()
-            for line in lines:
-                contents += f"        {line}\n"
-        contents += "    ---"
-
-        return contents
-
-    def _handle_id(self, namespace: str = "", id_string: str = "") -> str:
-        """checks whether the provided namespace-id combination is
-        already used for a node in the graph.
-        if no namespace is provided: default namespace is used,
-        if no id is provided: id get automatically generated."""
-
-        if not namespace:
-            namespace = self.namespace
-        if id_string:
-            node_id = self._id_vault.add_id(namespace, id_string)
-        else:
-            node_id = self._id_vault.generate(namespace)
-        return node_id
-
-    def add_entity(
-        self,
-        id_string: str = "",
-        label: str = "",
-        description: str = "",
-        namespace: str = "",
-    ) -> Entity:
-        """creates a new entity, adds it to the graph and returns it then"""
-
-        node_id = self._handle_id(namespace, id_string)
-        entity = Entity(node_id=node_id, label=label, description=description)
-        self._entities.append(entity)
-        return entity
-
-    def add_activity(
-        self,
-        id_string: str = "",
-        label: str = "",
-        description: str = "",
-        namespace: str = "",
-    ) -> Activity:
-        """creates a new activity, adds it to the graph and returns it then"""
-
-        node_id = self._handle_id(namespace, id_string)
-        activity = Activity(node_id=node_id, label=label, description=description)
-        self._activities.append(activity)
-        return activity
-
-    def add_agent(
-        self,
-        id_string: str = "",
-        label: str = "",
-        description: str = "",
-        namespace: str = "",
-    ) -> Agent:
-        """creates a new agent, adds it to the graph and returns it then"""
-
-        node_id = self._handle_id(namespace, id_string)
-        agent = Agent(node_id=node_id, label=label, description=description)
-        self._agents.append(agent)
-        return agent
-
-    # TODO
-    # def read_graph(self, file_path: str) -> None:
-    #     """reads the contents of an existing PROV-O provenance graph."""
-
-    #     pass
-
-    def get_rdflib_graph(self) -> Graph:
-        """returns the provenance graph as rdflib.Graph()."""
-
-        provenance_graph = Graph()
-        provenance_graph.bind("dc", DC)
-        provenance_graph.bind("foaf", FOAF)
-        provenance_graph.bind("rdf", RDF)
-        provenance_graph.bind("rdfs", RDFS)
-        provenance_graph.bind("prov", PROV)
-        provenance_graph.bind(self.namespace_abbreviation, Namespace(self.namespace))
-
-        for node in self._entities + self._activities + self._agents:
-            if node.label:
-                provenance_graph.add(
-                    (
-                        URIRef(node.node_id),
-                        RDFS.label,
-                        Literal(node.label, lang=self.lang),
-                    )
-                )
-            if node.description:
-                provenance_graph.add(
-                    (
-                        URIRef(node.node_id),
-                        RDFS.comment,
-                        Literal(node.description, lang=self.lang),
-                    )
-                )
-        for entity in self._entities:
-            provenance_graph.add((URIRef(entity.node_id), RDF.type, PROV.Entity))
-            for activity in entity._was_generated_by_activities:
-                provenance_graph.add(
-                    (
-                        URIRef(entity.node_id),
-                        PROV.wasGeneratedBy,
-                        URIRef(activity.node_id),
-                    )
-                )
-            for origin_entity in entity._was_derived_from_entities:
-                provenance_graph.add(
-                    (
-                        URIRef(entity.node_id),
-                        PROV.wasDerivedFrom,
-                        URIRef(origin_entity.node_id),
-                    )
-                )
-            for agent in entity._was_attributed_to_agents:
-                provenance_graph.add(
-                    (
-                        URIRef(entity.node_id),
-                        PROV.wasAttributedTo,
-                        URIRef(agent.node_id),
-                    )
-                )
-        for activity in self._activities:
-            provenance_graph.add((URIRef(activity.node_id), RDF.type, PROV.Activity))
-            if activity._start_time:
-                provenance_graph.add(
-                    (
-                        URIRef(activity.node_id),
-                        PROV.startedAtTime,
-                        Literal(activity._start_time, datatype=XSD.dateTime),
-                    )
-                )
-            if activity._end_time:
-                provenance_graph.add(
-                    (
-                        URIRef(activity.node_id),
-                        PROV.endedAtTime,
-                        Literal(activity._end_time, datatype=XSD.dateTime),
-                    )
-                )
-            for entity in activity._used_entities:
-                provenance_graph.add(
-                    (URIRef(activity.node_id), PROV.used, URIRef(entity.node_id))
-                )
-            for previous_activity in activity._was_informed_by_activities:
-                provenance_graph.add(
-                    (
-                        URIRef(activity.node_id),
-                        PROV.wasInformedBy,
-                        URIRef(previous_activity.node_id),
-                    )
-                )
-            for agent in activity._was_associated_with_agents:
-                provenance_graph.add(
-                    (
-                        URIRef(agent.node_id),
-                        PROV.wasAssociatedWith,
-                        URIRef(agent.node_id),
-                    )
-                )
-        for agent in self._agents:
-            provenance_graph.add((URIRef(agent.node_id), RDF.type, PROV.Agent))
-            for instructor in agent._acted_on_behalf_of_agents:
-                provenance_graph.add(
-                    (
-                        URIRef(agent.node_id),
-                        PROV.actedOnBehalfOf,
-                        URIRef(instructor.node_id),
-                    )
-                )
-
-        return provenance_graph
-
-    def serialize_as_rdf(self, file_name: str, export_format: str = "turtle") -> None:
-        """serializes the graph as rdf, available formats are:
-        "xml", "n3", "turtle", "nt", "pretty-xml", "trix", "trig", "nquads", "json-ld", "hext"
-        """
-        self.get_rdflib_graph().serialize(destination=file_name, format=export_format)
-
-    def export_as_mermaid_flowchart(
-        self, file_name: str, user_options: dict = {}
-    ) -> None:
-        """exports the contents of the graph as mermaid-md flowchart"""
-
-        # if possible the options use the mermaid terminology
-        options = {
-            "revert-relations": False,
-            "orientation": "TD",
-            "included-relations": [
-                "was_generated_by",
-                "was_attributed_to",
-                "used",
-                "was_associated_with",
-                "acted_on_behalf_of",
-            ],
-            "color": "#000000",
-            "stroke": "#a4a4a4",
-            "stroke-width": "1px",
-            "relation-style": "-",
-            "entity": {
-                "fill": "#fffedf",
-                "shape": "([:])",
-                "relation-style": None,
-                "color": None,
-                "stroke": None,
-                "stroke-width": None,
-            },
-            "activity": {
-                "fill": "#cfceff",
-                "shape": "[[:]]",
-                "relation-style": None,
-                "color": None,
-                "stroke": None,
-                "stroke-width": None,
-            },
-            "agent": {
-                "fill": "#ffebc3",
-                "shape": "[/:\\]",
-                "relation-style": ".",
-                "color": None,
-                "stroke": None,
-                "stroke-width": None,
-            },
-        }
-
-        options = update_dict(options, user_options)
-
-        text_color = options["color"]
-        stroke_color = options["stroke"]
-        stroke_width = options["stroke-width"]
-        stroke_style = options["relation-style"]
-
-        entity_text_color = options["entity"]["color"]
-        entity_stroke_color = options["entity"]["stroke"]
-        entity_stroke_width = options["entity"]["stroke-width"]
-        entity_stroke_style = options["entity"]["relation-style"]
-
-        activity_text_color = options["activity"]["color"]
-        activity_stroke_color = options["activity"]["stroke"]
-        activity_stroke_width = options["activity"]["stroke-width"]
-        activity_stroke_style = options["activity"]["relation-style"]
-
-        agent_text_color = options["agent"]["color"]
-        agent_stroke_color = options["agent"]["stroke"]
-        agent_stroke_width = options["agent"]["stroke-width"]
-        agent_stroke_style = options["agent"]["relation-style"]
-
-        lines = []
-        lines.append("```mermaid")
-        lines.append(f"flowchart {options['orientation']}")
-
-        lines.append(f"classDef entity fill:{options['entity']['fill']}")
-        if entity_text_color:
-            lines.append(f"classDef entity color:{options['entity']['color']}")
-        elif text_color:
-            lines.append(f"classDef entity color:{options['color']}")
-        if entity_stroke_color:
-            lines.append(f"classDef entity stroke:{options['entity']['stroke']}")
-        elif stroke_color:
-            lines.append(f"classDef entity stroke:{options['stroke']}")
-        if entity_stroke_width:
-            lines.append(
-                f"classDef entity stroke-width:{options['entity']['stroke-width']}"
-            )
-        elif stroke_width:
-            lines.append(f"classDef entity stroke-width:{options['stroke-width']}")
-
-        lines.append(f"classDef activity fill:{options['activity']['fill']}")
-        if activity_text_color:
-            lines.append(f"classDef activity color:{options['activity']['color']}")
-        elif text_color:
-            lines.append(f"classDef activity color:{options['color']}")
-        if activity_stroke_color:
-            lines.append(f"classDef activity stroke:{options['activity']['stroke']}")
-        elif stroke_color:
-            lines.append(f"classDef activity stroke:{options['stroke']}")
-        if activity_stroke_width:
-            lines.append(
-                f"classDef activity stroke-width:{options['activity']['stroke-width']}"
-            )
-        elif stroke_width:
-            lines.append(f"classDef activity stroke-width:{options['stroke-width']}")
-
-        lines.append(f"classDef agent fill:{options['agent']['fill']}")
-        if agent_text_color:
-            lines.append(f"classDef agent color:{options['agent']['color']}")
-        elif text_color:
-            lines.append(f"classDef agent color:{options['color']}")
-        if agent_stroke_color:
-            lines.append(f"classDef agent stroke:{options['agent']['stroke']}")
-        elif stroke_color:
-            lines.append(f"classDef agent stroke:{options['stroke']}")
-        if agent_stroke_width:
-            lines.append(
-                f"classDef agent stroke-width:{options['agent']['stroke-width']}"
-            )
-        elif stroke_width:
-            lines.append(f"classDef agent stroke-width:{options['stroke-width']}")
-
-        for entity in self._entities:
-            lines.append(
-                f'{entity.get_id()}{options["entity"]["shape"].split(":")[0]}<a style=color:inherit href={entity.get_id()}>{entity.get_label() if entity.get_label() else entity.get_id()}</a>{options["entity"]["shape"].split(":")[1]}:::entity'
-            )
-            if "was_derived_by" in options["included-relations"]:
-                for item in entity._was_derived_from_entities:
-                    if not options["revert-relations"]:
-                        lines.append(
-                            f"{entity.get_id()}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasDerivedFrom>was derived from</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{item.get_id()}"
-                        )
-                    else:
-                        lines.append(
-                            f"{item.get_id()}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasDerivedFrom>originated from</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{entity.get_id()}"
-                        )
-            if "was_generated_by" in options["included-relations"]:
-                for item in entity._was_generated_by_activities:
-                    if not options["revert-relations"]:
-                        lines.append(
-                            f"{entity.get_id()}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasGeneratedBy>was generated by</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{item.get_id()}"
-                        )
-                    else:
-                        lines.append(
-                            f"{item.get_id()}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasGeneratedBy>generated</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{entity.get_id()}"
-                        )
-            if "was_attributed_to" in options["included-relations"]:
-                for item in entity._was_attributed_to_agents:
-                    if not options["revert-relations"]:
-                        lines.append(
-                            f"{entity.get_id()}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAttributedTo>was attributed to</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.get_id()}"
-                        )
-                    else:
-                        lines.append(
-                            f"{item.get_id()}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAttributedTo>produced</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{entity.get_id()}"
-                        )
-
-        for activity in self._activities:
-            lines.append(
-                f"{activity.get_id()}{options['activity']['shape'].split(':')[0]}<a style=color:inherit href={activity.get_id()}>{activity.get_label() if activity.get_label() else activity.get_id()}</a>{options['activity']['shape'].split(':')[1]}:::activity"
-            )
-            if "was_informed_by" in options["included-relations"]:
-                for item in activity._was_informed_by_activities:
-                    if not options["revert-relations"]:
-                        lines.append(
-                            f"{activity.get_id()}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasInformedBy>was informed by</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{item.get_id()}"
-                        )
-                    else:
-                        lines.append(
-                            f"{item.get_id()}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasInformedBy>informed</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{activity.get_id()}"
-                        )
-            if "used" in options["included-relations"]:
-                for item in activity._used_entities:
-                    if not options["revert-relations"]:
-                        lines.append(
-                            f"{activity.get_id()}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#used>used</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{item.get_id()}"
-                        )
-                    else:
-                        lines.append(
-                            f"{item.get_id()}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#used>was used by</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{activity.get_id()}"
-                        )
-            if "was_associated_with" in options["included-relations"]:
-                for item in activity._was_associated_with_agents:
-                    if not options["revert-relations"]:
-                        lines.append(
-                            f"{activity.get_id()}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAssociatedWith>was associated with</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.get_id()}"
-                        )
-                    else:
-                        lines.append(
-                            f"{item.get_id()}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAssociatedWith>initiated</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{activity.get_id()}"
-                        )
-
-        for agent in self._agents:
-            lines.append(
-                f"{agent.get_id()}{options['agent']['shape'].split(':')[0]}<a style=color:inherit href={agent.get_id()}>{agent.get_label() if agent.get_label() else agent.get_id()}</a>{options['agent']['shape'].split(':')[1]}:::agent"
-            )
-            if "acted_on_behalf_of" in options["included-relations"]:
-                for item in agent._acted_on_behalf_of_agents:
-                    if not options["revert-relations"]:
-                        lines.append(
-                            f"{agent.get_id()}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#actedOnBehalfOf>acted on behalf of</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.get_id()}"
-                        )
-                    else:
-                        lines.append(
-                            f"{item.get_id()}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#actedOnBehalfOf>instructed</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{agent.get_id()}"
-                        )
-
-        lines.append("```")
-        lines = "\n".join(lines)
-
-        with open(file_name, "w") as f:
-            f.write(lines)
+"""
+@author Arne Rümmler
+@contact arne.ruemmler@gmail.com
+
+@summary Implementation of a provenance graph
+    class that uses PROV-O terms
+"""
+
+
+from dataclasses import dataclass, field
+
+from rdflib import (
+    DC,
+    FOAF,
+    PROV,
+    RDF,
+    RDFS,
+    XSD,
+    Graph,  # type: ignore
+    Literal,
+    Namespace,
+    URIRef,
+)
+from validators import url
+
+from provo.idvault import IdVault
+from provo.startingpointclasses import Activity, Agent, Entity
+from provo.staticfunctions import update_dict
+
+
+@dataclass(frozen=True)
+class NamespaceMalformed(Exception):
+    """Raised when the namespace is not a valid URL."""
+
+    message: str
+
+
+@dataclass(frozen=True)
+class NamespaceHasNoEndSymbol(Exception):
+    """Raised if the namespace does not end with '/' or '#'."""
+
+    message: str
+
+
+@dataclass(frozen=True)
+class PrefixShorthandNotValid(Exception):
+    """Raised if the namespace abbreviation contains non-allowed characters."""
+
+    message: str
+
+
+@dataclass(frozen=True)
+class PrefixNotAllowed(Exception):
+    """Raised the namespace is not allowed."""
+
+    message: str
+
+
+@dataclass
+class ProvOntologyGraph:
+    """model that manages contents of a provenance graph
+    that adheres to the PROV-O provenance model."""
+
+    namespace: str = "https://provo-example.org/"
+    namespace_abbreviation: str = ""
+    lang: str = "en"
+    _entities: list[Entity] = field(init=False, default_factory=list)
+    _activities: list[Activity] = field(init=False, default_factory=list)
+    _agents: list[Agent] = field(init=False, default_factory=list)
+    _id_vault: IdVault = field(init=False, default_factory=IdVault)
+
+    def __post_init__(self):
+        """check validity of namespace and and namespace abbreviation"""
+
+        # validate namespace
+        # TODO rethink validation, we technically want to validate an IRI
+        if not url(self.namespace):  # type: ignore
+            raise NamespaceMalformed(
+                """
+            The provided namespace is not a valid URL!
+
+            See validators package (https://github.com/python-validators/validators),
+            validators.url() or https://gist.github.com/dperini/729294 for more
+            information on what qualifies a URL as valid.
+            
+            https://www.rfc-editor.org/rfc/rfc3986#section-3:
+            3.  Syntax Components
+
+            The generic URI syntax consists of a hierarchical sequence of
+            components referred to as the scheme, authority, path, query, and
+            fragment.
+
+                URI         = scheme ":" hier-part [ "?" query ] [ "#" fragment ]
+
+                hier-part   = "//" authority path-abempty
+                            / path-absolute
+                            / path-rootless
+                            / path-empty
+
+            The scheme and path components are required, though the path may be
+            empty (no characters).  When authority is present, the path must
+            either be empty or begin with a slash ("/") character.  When
+            authority is not present, the path cannot begin with two slash
+            characters ("//").  These restrictions result in five different ABNF
+            rules for a path (Section 3.3), only one of which will match any
+            given URI reference.
+
+            The following are two example URIs and their component parts:
+
+                    foo://example.com:8042/over/there?name=ferret#nose
+                    \_/   \______________/\_________/ \_________/ \__/
+                    |           |            |            |        |
+                scheme     authority       path        query   fragment
+                    |   _____________________|__
+                    / \ /                        \
+                    urn:example:animal:ferret:nose
+            """
+            )
+        end_symbol = self.namespace[-1]
+        if end_symbol not in ("/", "#"):
+            raise NamespaceHasNoEndSymbol(
+                "The provided Namespace has to end on a '/' or '#'!"
+            )
+
+        # validate namespace abbreviation
+        # TODO check what is actually allowed
+        allowed_symbols_for_prefix_shorthand = "abcdefghijklmnopqrstuvwxyz"
+
+        for symbol in self.namespace_abbreviation:
+            if symbol not in allowed_symbols_for_prefix_shorthand:
+                raise PrefixShorthandNotValid(
+                    f"""
+                    The provided namespace abbreviation is not valid.
+                    
+                    Character of the namespace have to be in "{allowed_symbols_for_prefix_shorthand}".
+                    """
+                )
+        # if self.namespace_abbreviation in forbidden_namespaces:
+        core_prefixes = ["owl", "rdf", "rdfs", "xsd", "xml"]
+        if self.namespace_abbreviation in core_prefixes:
+            raise PrefixNotAllowed(
+                f"""
+            The provided namespace abbreviation is a core prefix, 
+            and thus, prohibited from use.
+
+            Core prefixes are: {"".join([f"{k}, " if i != len(core_prefixes)-2 else f"{k} and " for i, k in enumerate(core_prefixes)])[:-2]}.
+            """
+            )
+
+    def __str__(self) -> str:
+        """prints the contents of the provenance graph in a nice format."""
+        contents = "Provenance Graph Contents:"
+        contents += "\n    ---"
+        contents += "\n    Entities:"
+        contents += "\n        ---\n"
+        for entity in self._entities:
+            lines = entity.__str__().splitlines()
+            for line in lines:
+                contents += f"        {line}\n"
+        contents += "    ---"
+        contents += "\n    Activities:"
+        contents += "\n        ---\n"
+        for activity in self._activities:
+            lines = activity.__str__().splitlines()
+            for line in lines:
+                contents += f"        {line}\n"
+        contents += "    ---"
+        contents += "\n    Agents:"
+        contents += "\n        ---\n"
+        for agent in self._agents:
+            lines = agent.__str__().splitlines()
+            for line in lines:
+                contents += f"        {line}\n"
+        contents += "    ---"
+
+        return contents
+
+    def _handle_id(self, id: str = "", use_namespace: bool = False) -> str:
+        """checks whether the provided namespace-id combination is
+        already used for a node in the graph.
+        if no namespace is provided: default namespace is used,
+        if no id is provided: id get automatically generated."""
+
+        if use_namespace:
+            id = self.namespace + id
+        if id:
+            node_id = self._id_vault.add_id(id)
+        else:
+            node_id = self._id_vault.generate(self.namespace)
+        return node_id
+
+    def add_entity(
+        self,
+        id: str = "",
+        label: str = "",
+        description: str = "",
+        use_namespace: bool = False,
+    ) -> Entity:
+        """creates a new entity, adds it to the graph and returns it then"""
+
+        node_id = self._handle_id(id, use_namespace)
+        entity = Entity(node_id=node_id, label=label, description=description)
+        self._entities.append(entity)
+        return entity
+
+    def add_activity(
+        self,
+        id: str = "",
+        label: str = "",
+        description: str = "",
+        use_namespace: bool = False,
+    ) -> Activity:
+        """creates a new activity, adds it to the graph and returns it then"""
+
+        node_id = self._handle_id(id, use_namespace)
+        activity = Activity(node_id=node_id, label=label,
+                            description=description)
+        self._activities.append(activity)
+        return activity
+
+    def add_agent(
+        self,
+        id: str = "",
+        label: str = "",
+        description: str = "",
+        use_namespace: bool = False,
+    ) -> Agent:
+        """creates a new agent, adds it to the graph and returns it then"""
+
+        node_id = self._handle_id(id, use_namespace)
+        agent = Agent(node_id=node_id, label=label, description=description)
+        self._agents.append(agent)
+        return agent
+
+    # TODO
+    # def read_graph(self, file_path: str) -> None:
+    #     """reads the contents of an existing PROV-O provenance graph."""
+
+    #     pass
+
+    def get_rdflib_graph(self) -> Graph:
+        """returns the provenance graph as rdflib.Graph()."""
+
+        provenance_graph = Graph()
+        provenance_graph.bind("dc", DC)
+        provenance_graph.bind("foaf", FOAF)
+        provenance_graph.bind("rdf", RDF)
+        provenance_graph.bind("rdfs", RDFS)
+        provenance_graph.bind("prov", PROV)
+        provenance_graph.bind(self.namespace_abbreviation,
+                              Namespace(self.namespace))
+
+        for node in self._entities + self._activities + self._agents:
+            if node.label:
+                provenance_graph.add(
+                    (
+                        URIRef(node.node_id),
+                        RDFS.label,
+                        Literal(node.label, lang=self.lang),
+                    )
+                )
+            if node.description:
+                provenance_graph.add(
+                    (
+                        URIRef(node.node_id),
+                        RDFS.comment,
+                        Literal(node.description, lang=self.lang),
+                    )
+                )
+        for entity in self._entities:
+            provenance_graph.add(
+                (URIRef(entity.node_id), RDF.type, PROV.Entity))
+            for activity in entity._was_generated_by_activities:
+                provenance_graph.add(
+                    (
+                        URIRef(entity.node_id),
+                        PROV.wasGeneratedBy,
+                        URIRef(activity.node_id),
+                    )
+                )
+            for origin_entity in entity._was_derived_from_entities:
+                provenance_graph.add(
+                    (
+                        URIRef(entity.node_id),
+                        PROV.wasDerivedFrom,
+                        URIRef(origin_entity.node_id),
+                    )
+                )
+            for agent in entity._was_attributed_to_agents:
+                provenance_graph.add(
+                    (
+                        URIRef(entity.node_id),
+                        PROV.wasAttributedTo,
+                        URIRef(agent.node_id),
+                    )
+                )
+        for activity in self._activities:
+            provenance_graph.add(
+                (URIRef(activity.node_id), RDF.type, PROV.Activity))
+            if activity._start_time:
+                provenance_graph.add(
+                    (
+                        URIRef(activity.node_id),
+                        PROV.startedAtTime,
+                        Literal(activity._start_time, datatype=XSD.dateTime),
+                    )
+                )
+            if activity._end_time:
+                provenance_graph.add(
+                    (
+                        URIRef(activity.node_id),
+                        PROV.endedAtTime,
+                        Literal(activity._end_time, datatype=XSD.dateTime),
+                    )
+                )
+            for entity in activity._used_entities:
+                provenance_graph.add(
+                    (URIRef(activity.node_id), PROV.used, URIRef(entity.node_id))
+                )
+            for previous_activity in activity._was_informed_by_activities:
+                provenance_graph.add(
+                    (
+                        URIRef(activity.node_id),
+                        PROV.wasInformedBy,
+                        URIRef(previous_activity.node_id),
+                    )
+                )
+            for agent in activity._was_associated_with_agents:
+                provenance_graph.add(
+                    (
+                        URIRef(agent.node_id),
+                        PROV.wasAssociatedWith,
+                        URIRef(agent.node_id),
+                    )
+                )
+        for agent in self._agents:
+            provenance_graph.add((URIRef(agent.node_id), RDF.type, PROV.Agent))
+            for instructor in agent._acted_on_behalf_of_agents:
+                provenance_graph.add(
+                    (
+                        URIRef(agent.node_id),
+                        PROV.actedOnBehalfOf,
+                        URIRef(instructor.node_id),
+                    )
+                )
+
+        return provenance_graph
+
+    def serialize_as_rdf(self, file_name: str, export_format: str = "turtle") -> None:
+        """serializes the graph as rdf, available formats are:
+        "xml", "n3", "turtle", "nt", "pretty-xml", "trix", "trig", "nquads", "json-ld", "hext"
+        """
+        self.get_rdflib_graph().serialize(destination=file_name, format=export_format)
+
+    def export_as_mermaid_flowchart(
+        self, file_name: str, user_options: dict = {}
+    ) -> None:
+        """exports the contents of the graph as mermaid-md flowchart"""
+
+        # if possible the options use the mermaid terminology
+        options = {
+            "revert-relations": False,
+            "orientation": "TD",
+            "included-relations": [
+                "was_generated_by",
+                "was_attributed_to",
+                "used",
+                "was_associated_with",
+                "acted_on_behalf_of",
+            ],
+            "color": "#000000",
+            "stroke": "#a4a4a4",
+            "stroke-width": "1px",
+            "relation-style": "-",
+            "entity": {
+                "fill": "#fffedf",
+                "shape": "([:])",
+                "relation-style": None,
+                "color": None,
+                "stroke": None,
+                "stroke-width": None,
+            },
+            "activity": {
+                "fill": "#cfceff",
+                "shape": "[[:]]",
+                "relation-style": None,
+                "color": None,
+                "stroke": None,
+                "stroke-width": None,
+            },
+            "agent": {
+                "fill": "#ffebc3",
+                "shape": "[/:\\]",
+                "relation-style": ".",
+                "color": None,
+                "stroke": None,
+                "stroke-width": None,
+            },
+        }
+
+        options = update_dict(options, user_options)
+
+        text_color = options["color"]
+        stroke_color = options["stroke"]
+        stroke_width = options["stroke-width"]
+        stroke_style = options["relation-style"]
+
+        entity_text_color = options["entity"]["color"]
+        entity_stroke_color = options["entity"]["stroke"]
+        entity_stroke_width = options["entity"]["stroke-width"]
+        entity_stroke_style = options["entity"]["relation-style"]
+
+        activity_text_color = options["activity"]["color"]
+        activity_stroke_color = options["activity"]["stroke"]
+        activity_stroke_width = options["activity"]["stroke-width"]
+        activity_stroke_style = options["activity"]["relation-style"]
+
+        agent_text_color = options["agent"]["color"]
+        agent_stroke_color = options["agent"]["stroke"]
+        agent_stroke_width = options["agent"]["stroke-width"]
+        agent_stroke_style = options["agent"]["relation-style"]
+
+        lines = []
+        lines.append("```mermaid")
+        lines.append(f"flowchart {options['orientation']}")
+
+        lines.append(f"classDef entity fill:{options['entity']['fill']}")
+        if entity_text_color:
+            lines.append(f"classDef entity color:{options['entity']['color']}")
+        elif text_color:
+            lines.append(f"classDef entity color:{options['color']}")
+        if entity_stroke_color:
+            lines.append(
+                f"classDef entity stroke:{options['entity']['stroke']}")
+        elif stroke_color:
+            lines.append(f"classDef entity stroke:{options['stroke']}")
+        if entity_stroke_width:
+            lines.append(
+                f"classDef entity stroke-width:{options['entity']['stroke-width']}"
+            )
+        elif stroke_width:
+            lines.append(
+                f"classDef entity stroke-width:{options['stroke-width']}")
+
+        lines.append(f"classDef activity fill:{options['activity']['fill']}")
+        if activity_text_color:
+            lines.append(
+                f"classDef activity color:{options['activity']['color']}")
+        elif text_color:
+            lines.append(f"classDef activity color:{options['color']}")
+        if activity_stroke_color:
+            lines.append(
+                f"classDef activity stroke:{options['activity']['stroke']}")
+        elif stroke_color:
+            lines.append(f"classDef activity stroke:{options['stroke']}")
+        if activity_stroke_width:
+            lines.append(
+                f"classDef activity stroke-width:{options['activity']['stroke-width']}"
+            )
+        elif stroke_width:
+            lines.append(
+                f"classDef activity stroke-width:{options['stroke-width']}")
+
+        lines.append(f"classDef agent fill:{options['agent']['fill']}")
+        if agent_text_color:
+            lines.append(f"classDef agent color:{options['agent']['color']}")
+        elif text_color:
+            lines.append(f"classDef agent color:{options['color']}")
+        if agent_stroke_color:
+            lines.append(f"classDef agent stroke:{options['agent']['stroke']}")
+        elif stroke_color:
+            lines.append(f"classDef agent stroke:{options['stroke']}")
+        if agent_stroke_width:
+            lines.append(
+                f"classDef agent stroke-width:{options['agent']['stroke-width']}"
+            )
+        elif stroke_width:
+            lines.append(
+                f"classDef agent stroke-width:{options['stroke-width']}")
+
+        for entity in self._entities:
+            lines.append(
+                f'{entity.node_id}{options["entity"]["shape"].split(":")[0]}<a style=color:inherit href={entity.node_id}>{entity.label if entity.label else entity.node_id}</a>{options["entity"]["shape"].split(":")[1]}:::entity'
+            )
+            if "was_derived_by" in options["included-relations"]:
+                for item in entity._was_derived_from_entities:
+                    if not options["revert-relations"]:
+                        lines.append(
+                            f"{entity.node_id}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasDerivedFrom>was derived from</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{item.node_id}"
+                        )
+                    else:
+                        lines.append(
+                            f"{item.node_id}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasDerivedFrom>originated from</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{entity.node_id}"
+                        )
+            if "was_generated_by" in options["included-relations"]:
+                for item in entity._was_generated_by_activities:
+                    if not options["revert-relations"]:
+                        lines.append(
+                            f"{entity.node_id}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasGeneratedBy>was generated by</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{item.node_id}"
+                        )
+                    else:
+                        lines.append(
+                            f"{item.node_id}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasGeneratedBy>generated</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{entity.node_id}"
+                        )
+            if "was_attributed_to" in options["included-relations"]:
+                for item in entity._was_attributed_to_agents:
+                    if not options["revert-relations"]:
+                        lines.append(
+                            f"{entity.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAttributedTo>was attributed to</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.node_id}"
+                        )
+                    else:
+                        lines.append(
+                            f"{item.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAttributedTo>produced</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{entity.node_id}"
+                        )
+
+        for activity in self._activities:
+            lines.append(
+                f"{activity.node_id}{options['activity']['shape'].split(':')[0]}<a style=color:inherit href={activity.node_id}>{activity.label if activity.label else activity.node_id}</a>{options['activity']['shape'].split(':')[1]}:::activity"
+            )
+            if "was_informed_by" in options["included-relations"]:
+                for item in activity._was_informed_by_activities:
+                    if not options["revert-relations"]:
+                        lines.append(
+                            f"{activity.node_id}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasInformedBy>was informed by</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{item.node_id}"
+                        )
+                    else:
+                        lines.append(
+                            f"{item.node_id}-{entity_stroke_style if entity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasInformedBy>informed</a> {entity_stroke_style if entity_stroke_style else stroke_style}->{activity.node_id}"
+                        )
+            if "used" in options["included-relations"]:
+                for item in activity._used_entities:
+                    if not options["revert-relations"]:
+                        lines.append(
+                            f"{activity.node_id}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#used>used</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{item.node_id}"
+                        )
+                    else:
+                        lines.append(
+                            f"{item.node_id}-{activity_stroke_style if activity_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#used>was used by</a> {activity_stroke_style if activity_stroke_style else stroke_style}->{activity.node_id}"
+                        )
+            if "was_associated_with" in options["included-relations"]:
+                for item in activity._was_associated_with_agents:
+                    if not options["revert-relations"]:
+                        lines.append(
+                            f"{activity.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAssociatedWith>was associated with</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.node_id}"
+                        )
+                    else:
+                        lines.append(
+                            f"{item.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#wasAssociatedWith>initiated</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{activity.node_id}"
+                        )
+
+        for agent in self._agents:
+            lines.append(
+                f"{agent.node_id}{options['agent']['shape'].split(':')[0]}<a style=color:inherit href={agent.node_id}>{agent.label if agent.label else agent.node_id}</a>{options['agent']['shape'].split(':')[1]}:::agent"
+            )
+            if "acted_on_behalf_of" in options["included-relations"]:
+                for item in agent._acted_on_behalf_of_agents:
+                    if not options["revert-relations"]:
+                        lines.append(
+                            f"{agent.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#actedOnBehalfOf>acted on behalf of</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{item.node_id}"
+                        )
+                    else:
+                        lines.append(
+                            f"{item.node_id}-{agent_stroke_style if agent_stroke_style else stroke_style} <a style=color:inherit href=https://www.w3.org/TR/prov-o/#actedOnBehalfOf>instructed</a> {agent_stroke_style if agent_stroke_style else stroke_style}->{agent.node_id}"
+                        )
+
+        lines.append("```")
+        lines = "\n".join(lines)
+
+        with open(file_name, "w") as f:
+            f.write(lines)
```

### Comparing `provo-1.0.5/provo/startingpointclasses.py` & `provo-1.1.0/provo/startingpointclasses.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-"""
-@author Arne Rümmler
-@contact arne.ruemmler@gmail.com
-
-@summary Implementation of the starting term classes of
- PROV-O https://www.w3.org/TR/prov-o/ .
-"""
-
-
-from abc import ABC, abstractmethod
-from dataclasses import dataclass, field
-from datetime import datetime
-
-@dataclass(frozen=True)
-class NoStartTimeDefined(Exception):
-    """Raised if user user wants to access the start time of
-    an activity for which no start time was defined."""
-
-    message: str
-
-@dataclass(frozen=True)
-class NoEndTimeDefined(Exception):
-    """Raised if user user wants to access the end time of
-    an activity for which no end time was defined."""
-
-    message: str
-
-@dataclass(frozen=True)
-class InvalidProvClassForThisRelation(Exception):
-    """Raised when the wrong class is given as attribute
-    to one of the starting point property methods."""
-
-    message: str
-
-
-@dataclass(frozen=True)
-class NoDateTime(Exception):
-    """Raised when no datetime object is given as attribute."""
-
-    message: str
-
-
-@dataclass
-class Node(ABC):
-    """ Abstract parent class of Activity, Agent, and Entity. """
-
-    label: str = ""
-    description: str = ""
-    node_id: str = ""
-
-    @abstractmethod
-    def __str__(self) -> str:
-        """prints the node in a nice format"""
-        contents = f"id: {self.node_id}"
-        if self.label:
-            contents += f"\nlabel: {self.label}"
-        if self.description:
-            contents += f"\ndescription: {self.description}"
-        return contents
-
-    def get_id(self) -> str:
-        """returns the node's id"""
-
-        return self.node_id
-
-    def get_label(self) -> str:
-        """returns the node's label"""
-
-        return self.label
-
-    def get_description(self) -> str:
-        """returns the node's description"""
-
-        return self.description
-
-
-@dataclass
-class Entity(Node):
-    """ Class to create a PROV-O Entity object. 
-    https://www.w3.org/TR/prov-o/#Entity """
-
-    _was_derived_from_entities: list['Entity'] = field(init=False, default_factory=list)
-    _was_generated_by_activities: list['Activity'] = field(init=False, default_factory=list)
-    _was_attributed_to_agents: list['Agent'] = field(init=False, default_factory=list)
-
-    def __str__(self) -> str:
-        """prints the entity in a nice format."""
-        contents = super().__str__()
-        if self._was_derived_from_entities:
-            contents += f"\nwas derived from: {[item.label if item.label else item.node_id for item in self._was_derived_from_entities]}"
-        if self._was_generated_by_activities:
-            contents += f"\nwas generated by: {[item.label if item.label else item.node_id for item in self._was_generated_by_activities]}"
-        if self._was_attributed_to_agents:
-            contents += f"\nwas attributed to: {[item.label if item.label else item.node_id for item in self._was_attributed_to_agents]}"
-        contents += "\n---"
-        return contents
-
-    def was_derived_from(self, entity: 'Entity') -> None:
-        """ implements the wasDerivedFrom property of PROV-O
-        https://www.w3.org/TR/prov-o/#wasDerivedFrom """
-
-        if not isinstance(entity, Entity):
-            raise InvalidProvClassForThisRelation(
-                f"""The PROV relation "was derived from" refers to an Entity, thus the provided
-                attribute has to be of type <class 'provo.startingpointclasses.Entity'>. 
-                In contradiction to this, the provided attribute is of the type {type(entity)}."""
-            )
-        self._was_derived_from_entities.append(entity)
-
-    def was_generated_by(self, activity: 'Activity') -> None:
-        """ implements the wasGeneratedBy property of PROV-O
-        https://www.w3.org/TR/prov-o/#wasgeneratedBy """
-
-        if not isinstance(activity, Activity):
-            raise InvalidProvClassForThisRelation(
-                f"""The PROV relation "was generated by" refers to an Activity, thus the provided
-                attribute has to be of type <class 'provo.startingpointclasses.Activity'>. 
-                In contradiction to this, the provided attribute is of the type {type(activity)}."""
-            )
-        self._was_generated_by_activities.append(activity)
-
-    def was_attributed_to(self, agent: 'Agent') -> None:
-        """ implements the wasAttributedTo property of PROV-O
-        https://www.w3.org/TR/prov-o/#wasAttributedTo """
-
-        if not isinstance(agent, Agent):
-            raise InvalidProvClassForThisRelation(
-                f"""The PROV relation "was attributed to" refers to an Agent, thus the provided
-                attribute has to be of type <class 'provo.startingpointclasses.Agent'>. 
-                In contradiction to this, the provided attribute is of the type {type(agent)}."""
-            )
-        self._was_attributed_to_agents.append(agent)
-
-
-@dataclass
-class Activity(Node):
-    """ Class to create a PROV-O Activity object.
-    https://www.w3.org/TR/prov-o/#Activity """
-
-    _was_informed_by_activities: list['Activity'] = field(init=False, default_factory=list)
-    _used_entities: list['Entity'] = field(init=False, default_factory=list)
-    _was_associated_with_agents: list['Agent'] = field(init=False, default_factory=list)
-    _start_time: datetime = field(init=False, default_factory=lambda: None)  # type: ignore (there is no default date that resolves to False)
-    _end_time: datetime = field(init=False, default_factory=lambda: None)  # type: ignore
-
-    def __str__(self) -> str:
-        """prints the activity in a nice format."""
-        contents = super().__str__()
-        if self._start_time:
-            contents += f"\nstart time: {self._start_time}"
-        if self._end_time:
-            contents += f"\nend time: {self._end_time}"
-        if self._was_informed_by_activities:
-            contents += f"\nwas informed by: {[item.label if item.label else item.node_id for item in self._was_informed_by_activities]}"
-        if self._used_entities:
-            contents += f"\nused: {[item.label if item.label else item.node_id for item in self._used_entities]}"
-        if self._was_associated_with_agents:
-            contents += f"\nwas associated with: {[item.label if item.label else item.node_id for item in self._was_associated_with_agents]}"
-        contents += "\n---"
-        return contents
-
-    def get_start_time(self) -> datetime:
-        """returns the start time of the activity"""
-        if self._start_time:
-            return self._start_time
-        else:
-            raise NoStartTimeDefined(f"No start time defined for the activity {self.label if self.label else f'with the id <{self.node_id}>'}.")
-
-    def get_end_time(self):
-        """returns the end time of the activity"""
-        if self._end_time:
-            return self._end_time
-        else:
-            raise NoEndTimeDefined(f"No end time defined for the activity {self.label if self.label else f'with the id <{self.node_id}>'}.")
-
-    def was_informed_by(self, activity: 'Activity') -> None:
-        """ implements the wasInformedBy property of PROV-O
-        https://www.w3.org/TR/prov-o/#wasInformedBy """
-
-        if not isinstance(activity, Activity):
-            raise InvalidProvClassForThisRelation(
-                f"""The PROV relation "was informed by" refers to an Activity, thus the provided
-                attribute has to be of type <class 'provo.startingpointclasses.Activity'>. 
-                In contradiction to this, the provided attribute is of the type {type(activity)}."""
-            )
-        self._was_informed_by_activities.append(activity)
-
-    def used(self, entity: 'Entity') -> None:
-        """ implements the used property of PROV-O
-        https://www.w3.org/TR/prov-o/#used """
-
-        if not isinstance(entity, Entity):
-            raise InvalidProvClassForThisRelation(
-                f"""The PROV relation "used" refers to an Entity, thus the provided
-                attribute has to be of type <class 'provo.startingpointclasses.Entity'>. 
-                In contradiction to this, the provided attribute is of the type {type(entity)}."""
-            )
-        self._used_entities.append(entity)
-
-    def was_associated_with(self, agent: 'Agent') -> None:
-        """ implements the wasAssociatedWith property of PROV-O
-        https://www.w3.org/TR/prov-o/#wasAssociatedWith """
-
-        if not isinstance(agent, Agent):
-            raise InvalidProvClassForThisRelation(
-                f"""The PROV relation "was associated with" refers to an Agent, thus the provided
-                attribute has to be of type <class 'provo.startingpointclasses.Agent'>. 
-                In contradiction to this, the provided attribute is of the type {type(agent)}."""
-            )
-        self._was_associated_with_agents.append(agent)
-
-    def started_at_time(self, start_time: datetime) -> None:
-        """ implements the startedAtTime property of PROV-O
-        https://www.w3.org/TR/prov-o/#startedAtTime """
-
-        if not isinstance(start_time, datetime):
-            raise NoDateTime("The attribute `start_time` of the method `started_at_time` has to be a `datetime` object.")
-        self._start_time = start_time
-
-    def ended_at_time(self, end_time: datetime) -> None:
-        """ implements the endedAtTime property of PROV-O
-        https://www.w3.org/TR/prov-o/#endedAtTime """
-
-        if not isinstance(end_time, datetime):
-            raise NoDateTime("The attribute `end_time` of the method `ended_at_time` has to be a `datetime` object.")
-
-        self._end_time = end_time
-
-
-@dataclass
-class Agent(Node):
-    """ Class to create a PROV-O Agent object.
-    https://www.w3.org/TR/prov-o/#Agent """
-
-    _acted_on_behalf_of_agents: list['Agent'] = field(init=False, default_factory=list)
-
-    def __str__(self) -> str:
-        """prints the agent in a nice format."""
-        contents = super().__str__()
-        if self._acted_on_behalf_of_agents:
-            contents += f"\nacted on behalf of: {[item.label if item.label else item.node_id for item in self._acted_on_behalf_of_agents]}"
-        contents += "\n---"
-        return contents
-
-    def acted_on_behalf_of(self, agent: 'Agent') -> None:
-        """ implements the actedOnBehalfOf property of PROV-O
-        https://www.w3.org/TR/prov-o/#actedOnBehalfOf """
-
-        if not isinstance(agent, Agent):
-            raise InvalidProvClassForThisRelation(
-                f"""The PROV relation "acted on behalf of" refers to an Agent, thus the provided
-                attribute has to be of type <class 'provo.startingpointclasses.Agent'>. 
-                In contradiction to this, the provided attribute is of the type {type(agent)}."""
-            )
-        self._acted_on_behalf_of_agents.append(agent)
+"""
+@author Arne Rümmler
+@contact arne.ruemmler@gmail.com
+
+@summary Implementation of the starting term classes of
+ PROV-O https://www.w3.org/TR/prov-o/ .
+"""
+
+
+from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
+from datetime import datetime
+
+
+@dataclass(frozen=True)
+class NoStartTimeDefined(Exception):
+    """Raised if user user wants to access the start time of
+    an activity for which no start time was defined."""
+
+    message: str
+
+
+@dataclass(frozen=True)
+class NoEndTimeDefined(Exception):
+    """Raised if user user wants to access the end time of
+    an activity for which no end time was defined."""
+
+    message: str
+
+
+@dataclass(frozen=True)
+class InvalidProvClassForThisRelation(Exception):
+    """Raised when the wrong class is given as attribute
+    to one of the starting point property methods."""
+
+    message: str
+
+
+@dataclass(frozen=True)
+class NoDateTime(Exception):
+    """Raised when no datetime object is given as attribute."""
+
+    message: str
+
+
+@dataclass
+class Node(ABC):
+    """ Abstract parent class of Activity, Agent, and Entity. """
+
+    label: str = ""
+    description: str = ""
+    node_id: str = ""
+
+    @abstractmethod
+    def __str__(self) -> str:
+        """prints the node in a nice format"""
+        contents = f"id: {self.node_id}"
+        if self.label:
+            contents += f"\nlabel: {self.label}"
+        if self.description:
+            contents += f"\ndescription: {self.description}"
+        return contents
+
+
+@dataclass
+class Entity(Node):
+    """ Class to create a PROV-O Entity object. 
+    https://www.w3.org/TR/prov-o/#Entity """
+
+    _was_derived_from_entities: list['Entity'] = field(
+        init=False, default_factory=list)
+    _was_generated_by_activities: list['Activity'] = field(
+        init=False, default_factory=list)
+    _was_attributed_to_agents: list['Agent'] = field(
+        init=False, default_factory=list)
+
+    def __str__(self) -> str:
+        """prints the entity in a nice format."""
+        contents = super().__str__()
+        if self._was_derived_from_entities:
+            contents += f"\nwas derived from: {[item.label if item.label else item.node_id for item in self._was_derived_from_entities]}"
+        if self._was_generated_by_activities:
+            contents += f"\nwas generated by: {[item.label if item.label else item.node_id for item in self._was_generated_by_activities]}"
+        if self._was_attributed_to_agents:
+            contents += f"\nwas attributed to: {[item.label if item.label else item.node_id for item in self._was_attributed_to_agents]}"
+        contents += "\n---"
+        return contents
+
+    def was_derived_from(self, entity: 'Entity') -> None:
+        """ implements the wasDerivedFrom property of PROV-O
+        https://www.w3.org/TR/prov-o/#wasDerivedFrom """
+
+        if not isinstance(entity, Entity):
+            raise InvalidProvClassForThisRelation(
+                f"""The PROV relation "was derived from" refers to an Entity, thus the provided
+                attribute has to be of type <class 'provo.startingpointclasses.Entity'>. 
+                In contradiction to this, the provided attribute is of the type {type(entity)}."""
+            )
+        self._was_derived_from_entities.append(entity)
+
+    def was_generated_by(self, activity: 'Activity') -> None:
+        """ implements the wasGeneratedBy property of PROV-O
+        https://www.w3.org/TR/prov-o/#wasgeneratedBy """
+
+        if not isinstance(activity, Activity):
+            raise InvalidProvClassForThisRelation(
+                f"""The PROV relation "was generated by" refers to an Activity, thus the provided
+                attribute has to be of type <class 'provo.startingpointclasses.Activity'>. 
+                In contradiction to this, the provided attribute is of the type {type(activity)}."""
+            )
+        self._was_generated_by_activities.append(activity)
+
+    def was_attributed_to(self, agent: 'Agent') -> None:
+        """ implements the wasAttributedTo property of PROV-O
+        https://www.w3.org/TR/prov-o/#wasAttributedTo """
+
+        if not isinstance(agent, Agent):
+            raise InvalidProvClassForThisRelation(
+                f"""The PROV relation "was attributed to" refers to an Agent, thus the provided
+                attribute has to be of type <class 'provo.startingpointclasses.Agent'>. 
+                In contradiction to this, the provided attribute is of the type {type(agent)}."""
+            )
+        self._was_attributed_to_agents.append(agent)
+
+
+@dataclass
+class Activity(Node):
+    """ Class to create a PROV-O Activity object.
+    https://www.w3.org/TR/prov-o/#Activity """
+
+    _was_informed_by_activities: list['Activity'] = field(
+        init=False, default_factory=list)
+    _used_entities: list['Entity'] = field(init=False, default_factory=list)
+    _was_associated_with_agents: list['Agent'] = field(
+        init=False, default_factory=list)
+    # type: ignore (there is no default date that resolves to False)
+    _start_time: datetime = field(init=False, default_factory=lambda: None)
+    _end_time: datetime = field(
+        init=False, default_factory=lambda: None)  # type: ignore
+
+    def __str__(self) -> str:
+        """prints the activity in a nice format."""
+        contents = super().__str__()
+        if self._start_time:
+            contents += f"\nstart time: {self._start_time}"
+        if self._end_time:
+            contents += f"\nend time: {self._end_time}"
+        if self._was_informed_by_activities:
+            contents += f"\nwas informed by: {[item.label if item.label else item.node_id for item in self._was_informed_by_activities]}"
+        if self._used_entities:
+            contents += f"\nused: {[item.label if item.label else item.node_id for item in self._used_entities]}"
+        if self._was_associated_with_agents:
+            contents += f"\nwas associated with: {[item.label if item.label else item.node_id for item in self._was_associated_with_agents]}"
+        contents += "\n---"
+        return contents
+
+    def get_start_time(self) -> datetime:
+        """returns the start time of the activity"""
+        if self._start_time:
+            return self._start_time
+        else:
+            raise NoStartTimeDefined(
+                f"No start time defined for the activity {self.label if self.label else f'with the id <{self.node_id}>'}.")
+
+    def get_end_time(self):
+        """returns the end time of the activity"""
+        if self._end_time:
+            return self._end_time
+        else:
+            raise NoEndTimeDefined(
+                f"No end time defined for the activity {self.label if self.label else f'with the id <{self.node_id}>'}.")
+
+    def was_informed_by(self, activity: 'Activity') -> None:
+        """ implements the wasInformedBy property of PROV-O
+        https://www.w3.org/TR/prov-o/#wasInformedBy """
+
+        if not isinstance(activity, Activity):
+            raise InvalidProvClassForThisRelation(
+                f"""The PROV relation "was informed by" refers to an Activity, thus the provided
+                attribute has to be of type <class 'provo.startingpointclasses.Activity'>. 
+                In contradiction to this, the provided attribute is of the type {type(activity)}."""
+            )
+        self._was_informed_by_activities.append(activity)
+
+    def used(self, entity: 'Entity') -> None:
+        """ implements the used property of PROV-O
+        https://www.w3.org/TR/prov-o/#used """
+
+        if not isinstance(entity, Entity):
+            raise InvalidProvClassForThisRelation(
+                f"""The PROV relation "used" refers to an Entity, thus the provided
+                attribute has to be of type <class 'provo.startingpointclasses.Entity'>. 
+                In contradiction to this, the provided attribute is of the type {type(entity)}."""
+            )
+        self._used_entities.append(entity)
+
+    def was_associated_with(self, agent: 'Agent') -> None:
+        """ implements the wasAssociatedWith property of PROV-O
+        https://www.w3.org/TR/prov-o/#wasAssociatedWith """
+
+        if not isinstance(agent, Agent):
+            raise InvalidProvClassForThisRelation(
+                f"""The PROV relation "was associated with" refers to an Agent, thus the provided
+                attribute has to be of type <class 'provo.startingpointclasses.Agent'>. 
+                In contradiction to this, the provided attribute is of the type {type(agent)}."""
+            )
+        self._was_associated_with_agents.append(agent)
+
+    def started_at_time(self, start_time: datetime) -> None:
+        """ implements the startedAtTime property of PROV-O
+        https://www.w3.org/TR/prov-o/#startedAtTime """
+
+        if not isinstance(start_time, datetime):
+            raise NoDateTime(
+                "The attribute `start_time` of the method `started_at_time` has to be a `datetime` object.")
+        self._start_time = start_time
+
+    def ended_at_time(self, end_time: datetime) -> None:
+        """ implements the endedAtTime property of PROV-O
+        https://www.w3.org/TR/prov-o/#endedAtTime """
+
+        if not isinstance(end_time, datetime):
+            raise NoDateTime(
+                "The attribute `end_time` of the method `ended_at_time` has to be a `datetime` object.")
+
+        self._end_time = end_time
+
+
+@dataclass
+class Agent(Node):
+    """ Class to create a PROV-O Agent object.
+    https://www.w3.org/TR/prov-o/#Agent """
+
+    _acted_on_behalf_of_agents: list['Agent'] = field(
+        init=False, default_factory=list)
+
+    def __str__(self) -> str:
+        """prints the agent in a nice format."""
+        contents = super().__str__()
+        if self._acted_on_behalf_of_agents:
+            contents += f"\nacted on behalf of: {[item.label if item.label else item.node_id for item in self._acted_on_behalf_of_agents]}"
+        contents += "\n---"
+        return contents
+
+    def acted_on_behalf_of(self, agent: 'Agent') -> None:
+        """ implements the actedOnBehalfOf property of PROV-O
+        https://www.w3.org/TR/prov-o/#actedOnBehalfOf """
+
+        if not isinstance(agent, Agent):
+            raise InvalidProvClassForThisRelation(
+                f"""The PROV relation "acted on behalf of" refers to an Agent, thus the provided
+                attribute has to be of type <class 'provo.startingpointclasses.Agent'>. 
+                In contradiction to this, the provided attribute is of the type {type(agent)}."""
+            )
+        self._acted_on_behalf_of_agents.append(agent)
```

### Comparing `provo-1.0.5/provo/tests/test_provenance_graph.py` & `provo-1.1.0/provo/tests/test_provenance_graph.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-
-import pytest
-
-from provo.provontologygraph import (NamespaceHasNoEndSymbol,
-                                     NamespaceMalformed, PrefixNotAllowed,
-                                     PrefixShorthandNotValid,
-                                     ProvOntologyGraph)
-
-
-def test_graph_initialization():
-    """tests if namespace and namespace abbreviation (i.e., prefix) is valid"""
-    
-    ProvOntologyGraph()
-    ProvOntologyGraph(namespace="https://test.package/", namespace_abbreviation="")
-    ProvOntologyGraph(namespace="https://test.package#", namespace_abbreviation="")
-
-    malformed_namespaces = ["www.test.de", "https://test.package/ ",
-                            "test.org", " https://test.package/"]
-    for namespace in malformed_namespaces:
-        with pytest.raises(NamespaceMalformed):
-            ProvOntologyGraph(namespace=namespace)
-
-    with pytest.raises(NamespaceHasNoEndSymbol):
-        ProvOntologyGraph(namespace="https://test.package")
-
-    invalid_prefixes = [" ", ":", "test:"]
-    for prefix in invalid_prefixes:
-        with pytest.raises(PrefixShorthandNotValid):
-            ProvOntologyGraph(namespace_abbreviation=prefix)
-
-    core_prefixes = ["owl", "rdf", "rdfs", "xsd", "xml"]
-    for prefix in core_prefixes:
-        with pytest.raises(PrefixNotAllowed):
-            ProvOntologyGraph(namespace_abbreviation=prefix)
+
+import pytest
+
+from provo.provontologygraph import (NamespaceHasNoEndSymbol,
+                                     NamespaceMalformed, PrefixNotAllowed,
+                                     PrefixShorthandNotValid,
+                                     ProvOntologyGraph)
+
+
+def test_graph_initialization():
+    """tests if namespace and namespace abbreviation (i.e., prefix) is valid"""
+    
+    ProvOntologyGraph()
+    ProvOntologyGraph(namespace="https://test.package/", namespace_abbreviation="")
+    ProvOntologyGraph(namespace="https://test.package#", namespace_abbreviation="")
+
+    malformed_namespaces = ["www.test.de", "https://test.package/ ",
+                            "test.org", " https://test.package/"]
+    for namespace in malformed_namespaces:
+        with pytest.raises(NamespaceMalformed):
+            ProvOntologyGraph(namespace=namespace)
+
+    with pytest.raises(NamespaceHasNoEndSymbol):
+        ProvOntologyGraph(namespace="https://test.package")
+
+    invalid_prefixes = [" ", ":", "test:"]
+    for prefix in invalid_prefixes:
+        with pytest.raises(PrefixShorthandNotValid):
+            ProvOntologyGraph(namespace_abbreviation=prefix)
+
+    core_prefixes = ["owl", "rdf", "rdfs", "xsd", "xml"]
+    for prefix in core_prefixes:
+        with pytest.raises(PrefixNotAllowed):
+            ProvOntologyGraph(namespace_abbreviation=prefix)
```

### Comparing `provo-1.0.5/provo/tests/test_starting_point_classes.py` & `provo-1.1.0/provo/tests/test_starting_point_classes.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from datetime import datetime
-
-import pytest
-from provo.startingpointclasses import (Activity, Agent, Entity,
-                                        InvalidProvClassForThisRelation,
-                                        NoDateTime)
-
-entity = Entity(node_id='https://test.package/entity')
-activity = Activity(node_id='https://test.package/activity')
-agent = Agent(node_id='https://test.package/agent')
-
-
-def test_was_derived_from():
-    """tests was derived from method"""
-    entity.was_derived_from(entity)
-    with pytest.raises(InvalidProvClassForThisRelation):
-        entity.was_derived_from(activity)  # type: ignore
-    with pytest.raises(InvalidProvClassForThisRelation):
-        entity.was_derived_from(agent)  # type: ignore
-
-
-def test_was_generated_by():
-    """tests was generated by method"""
-    entity.was_generated_by(activity)
-    with pytest.raises(InvalidProvClassForThisRelation):
-        entity.was_generated_by(entity)  # type: ignore
-    with pytest.raises(InvalidProvClassForThisRelation):
-        entity.was_generated_by(agent)  # type: ignore
-
-
-def test_was_attributed_to():
-    """tests was attributed to method"""
-    entity.was_attributed_to(agent)
-    with pytest.raises(InvalidProvClassForThisRelation):
-        entity.was_attributed_to(activity)  # type: ignore
-    with pytest.raises(InvalidProvClassForThisRelation):
-        entity.was_attributed_to(entity)  # type: ignore
-
-
-def test_was_informed_by():
-    """tests was informed by method"""
-    activity.was_informed_by(activity)
-    with pytest.raises(InvalidProvClassForThisRelation):
-        activity.was_informed_by(entity)  # type: ignore
-    with pytest.raises(InvalidProvClassForThisRelation):
-        activity.was_informed_by(agent)  # type: ignore
-
-
-def test_was_associated_with():
-    """tests was associated with method"""
-    activity.was_associated_with(agent)
-    with pytest.raises(InvalidProvClassForThisRelation):
-        activity.was_associated_with(activity)  # type: ignore
-    with pytest.raises(InvalidProvClassForThisRelation):
-        activity.was_associated_with(entity)  # type: ignore
-
-
-def test_used():
-    """tests used method"""
-    activity.used(entity)
-    with pytest.raises(InvalidProvClassForThisRelation):
-        activity.used(activity)  # type: ignore
-    with pytest.raises(InvalidProvClassForThisRelation):
-        activity.used(agent)  # type: ignore
-
-
-def test_acted_on_behalf_of():
-    """tests acted on behalf of method"""
-    agent.acted_on_behalf_of(agent)
-    with pytest.raises(InvalidProvClassForThisRelation):
-        agent.acted_on_behalf_of(activity)  # type: ignore
-    with pytest.raises(InvalidProvClassForThisRelation):
-        agent.acted_on_behalf_of(entity)  # type: ignore
-
-
-def test_started_at_time():
-    """tests started at time method"""
-    activity.started_at_time(datetime(1980, 1, 1))
-    with pytest.raises(NoDateTime):
-        activity.started_at_time("01.01.1980")  # type: ignore
-    with pytest.raises(NoDateTime):
-        activity.started_at_time(1980)  # type: ignore
-
-
-def test_ended_at_time():
-    """tests ended at time method"""
-    activity.ended_at_time(datetime(1981, 1, 1))
-    with pytest.raises(NoDateTime):
-        activity.ended_at_time("01.01.1981")  # type: ignore
-    with pytest.raises(NoDateTime):
-        activity.ended_at_time(1981)  # type: ignore
+from datetime import datetime
+
+import pytest
+from provo.startingpointclasses import (Activity, Agent, Entity,
+                                        InvalidProvClassForThisRelation,
+                                        NoDateTime)
+
+entity = Entity(node_id='https://test.package/entity')
+activity = Activity(node_id='https://test.package/activity')
+agent = Agent(node_id='https://test.package/agent')
+
+
+def test_was_derived_from():
+    """tests was derived from method"""
+    entity.was_derived_from(entity)
+    with pytest.raises(InvalidProvClassForThisRelation):
+        entity.was_derived_from(activity)  # type: ignore
+    with pytest.raises(InvalidProvClassForThisRelation):
+        entity.was_derived_from(agent)  # type: ignore
+
+
+def test_was_generated_by():
+    """tests was generated by method"""
+    entity.was_generated_by(activity)
+    with pytest.raises(InvalidProvClassForThisRelation):
+        entity.was_generated_by(entity)  # type: ignore
+    with pytest.raises(InvalidProvClassForThisRelation):
+        entity.was_generated_by(agent)  # type: ignore
+
+
+def test_was_attributed_to():
+    """tests was attributed to method"""
+    entity.was_attributed_to(agent)
+    with pytest.raises(InvalidProvClassForThisRelation):
+        entity.was_attributed_to(activity)  # type: ignore
+    with pytest.raises(InvalidProvClassForThisRelation):
+        entity.was_attributed_to(entity)  # type: ignore
+
+
+def test_was_informed_by():
+    """tests was informed by method"""
+    activity.was_informed_by(activity)
+    with pytest.raises(InvalidProvClassForThisRelation):
+        activity.was_informed_by(entity)  # type: ignore
+    with pytest.raises(InvalidProvClassForThisRelation):
+        activity.was_informed_by(agent)  # type: ignore
+
+
+def test_was_associated_with():
+    """tests was associated with method"""
+    activity.was_associated_with(agent)
+    with pytest.raises(InvalidProvClassForThisRelation):
+        activity.was_associated_with(activity)  # type: ignore
+    with pytest.raises(InvalidProvClassForThisRelation):
+        activity.was_associated_with(entity)  # type: ignore
+
+
+def test_used():
+    """tests used method"""
+    activity.used(entity)
+    with pytest.raises(InvalidProvClassForThisRelation):
+        activity.used(activity)  # type: ignore
+    with pytest.raises(InvalidProvClassForThisRelation):
+        activity.used(agent)  # type: ignore
+
+
+def test_acted_on_behalf_of():
+    """tests acted on behalf of method"""
+    agent.acted_on_behalf_of(agent)
+    with pytest.raises(InvalidProvClassForThisRelation):
+        agent.acted_on_behalf_of(activity)  # type: ignore
+    with pytest.raises(InvalidProvClassForThisRelation):
+        agent.acted_on_behalf_of(entity)  # type: ignore
+
+
+def test_started_at_time():
+    """tests started at time method"""
+    activity.started_at_time(datetime(1980, 1, 1))
+    with pytest.raises(NoDateTime):
+        activity.started_at_time("01.01.1980")  # type: ignore
+    with pytest.raises(NoDateTime):
+        activity.started_at_time(1980)  # type: ignore
+
+
+def test_ended_at_time():
+    """tests ended at time method"""
+    activity.ended_at_time(datetime(1981, 1, 1))
+    with pytest.raises(NoDateTime):
+        activity.ended_at_time("01.01.1981")  # type: ignore
+    with pytest.raises(NoDateTime):
+        activity.ended_at_time(1981)  # type: ignore
```

### Comparing `provo-1.0.5/provo/tests/test_vault.py` & `provo-1.1.0/provo/tests/test_vault.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-import pytest
-from provo.idvault import IdAlreadyUsed, IdInvalid, IdVault
-from validators import url
-
-
-def test_generate():
-    """tests if the automatically generated id is a valid url"""
-
-    namespace = "https://test.package/"
-    vault = IdVault()
-    id = vault.generate(namespace=namespace)
-    # TODO rethink validation
-    assert url(id)  # type: ignore
-
-
-def test_no_id_duplication():
-    """tests if vault throws IdAlreadyUsed exception when an existing
-    id is added to the vault"""
-
-    namespace = "https://test.package/"
-    test_id = "test"
-    vault = IdVault()
-    vault.add_id(namespace=namespace, id_string=test_id)
-    with pytest.raises(IdAlreadyUsed):
-        vault.add_id(namespace=namespace, id_string=test_id)
-
-
-def test_id_validation():
-    """tests if vault throws IdInvalid exception if id contains one
-    of the invalid symbols"""
-
-    vault = IdVault()
-    invalid_symbols = '<>" {}|\\^`'
-
-    for symbol in invalid_symbols:
-        # test if error is thrown if namespace contains the symbol
-        namespace = f"https://t{symbol}est.package/"
-        test_id = "test"
-        with pytest.raises(IdInvalid):
-            vault._raise_exception_if_uri_invalid(namespace + test_id)
-
-        # test if error is thrown if id without namespace contains the symbol
-        namespace = "https://test.package/"
-        test_id = f"te{symbol}st"
-        with pytest.raises(IdInvalid):
-            vault._raise_exception_if_uri_invalid(namespace + test_id)
+import pytest
+from provo.idvault import IdAlreadyUsed, IdMalformed, IdVault
+from validators import url
+
+
+def test_generate():
+    """tests if the automatically generated id is a valid url"""
+
+    namespace = "https://test.package/"
+    vault = IdVault()
+    id = vault.generate(namespace=namespace)
+    # TODO rethink validation
+    assert url(id)  # type: ignore
+
+
+def test_no_id_duplication():
+    """tests if vault throws IdAlreadyUsed exception when an existing
+    id is added to the vault"""
+
+    test_id = "https://test.package/test"
+    vault = IdVault()
+    vault.add_id(node_id=test_id)
+    with pytest.raises(IdAlreadyUsed):
+        vault.add_id(node_id=test_id)
+
+
+def test_id_validation():
+    """tests if vault throws IdMalformed exception if id contains one
+    of the invalid symbols"""
+
+    vault = IdVault()
+    invalid_symbols = '<>" {}|\\^`'
+
+    for symbol in invalid_symbols:
+        # test if error is thrown if namespace contains the symbol
+        namespace = f"https://t{symbol}est.package/"
+        test_id = "test"
+        with pytest.raises(IdMalformed):
+            vault._raise_exception_if_uri_invalid(namespace + test_id)
+
+        # test if error is thrown if id without namespace contains the symbol
+        namespace = "https://test.package/"
+        test_id = f"te{symbol}st"
+        with pytest.raises(IdMalformed):
+            vault._raise_exception_if_uri_invalid(namespace + test_id)
```

