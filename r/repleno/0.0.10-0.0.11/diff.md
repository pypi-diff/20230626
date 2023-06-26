# Comparing `tmp/repleno-0.0.10-py3-none-any.whl.zip` & `tmp/repleno-0.0.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 19935 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat    34250 b- defN 23-Jun-21 13:12 repleno/SKU.py
--rw-rw-rw-  2.0 fat      175 b- defN 23-Feb-28 13:50 repleno/__init__.py
--rw-rw-rw-  2.0 fat       96 b- defN 23-Jun-15 20:24 repleno/__main__.py
--rw-rw-rw-  2.0 fat    25702 b- defN 23-Jun-22 07:40 repleno/factory.py
--rw-rw-rw-  2.0 fat     2304 b- defN 23-Jun-20 20:17 repleno/order.py
--rw-rw-rw-  2.0 fat     9525 b- defN 23-Jun-20 19:10 repleno/utils.py
--rw-rw-rw-  2.0 fat     1316 b- defN 23-Jun-22 09:24 repleno-0.0.10.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 09:24 repleno-0.0.10.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-22 09:24 repleno-0.0.10.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      744 b- defN 23-Jun-22 09:24 repleno-0.0.10.dist-info/RECORD
-10 files, 74212 bytes uncompressed, 18685 bytes compressed:  74.8%
+Zip file size: 20275 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat    32772 b- defN 23-Jun-25 14:02 repleno/SKU.py
+-rw-rw-rw-  2.0 fat      519 b- defN 23-Jun-25 14:02 repleno/__init__.py
+-rw-rw-rw-  2.0 fat       96 b- defN 23-Jun-25 14:02 repleno/__main__.py
+-rw-rw-rw-  2.0 fat    24800 b- defN 23-Jun-26 12:01 repleno/factory.py
+-rw-rw-rw-  2.0 fat     2316 b- defN 23-Jun-25 14:02 repleno/order.py
+-rw-rw-rw-  2.0 fat     9539 b- defN 23-Jun-23 15:07 repleno/utils.py
+-rw-rw-rw-  2.0 fat     2680 b- defN 23-Jun-26 12:02 repleno-0.0.11.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 12:02 repleno-0.0.11.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-26 12:02 repleno-0.0.11.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      744 b- defN 23-Jun-26 12:02 repleno-0.0.11.dist-info/RECORD
+10 files, 73566 bytes uncompressed, 19025 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: repleno/order.py
 Comment: 
 
 Filename: repleno/utils.py
 Comment: 
 
-Filename: repleno-0.0.10.dist-info/METADATA
+Filename: repleno-0.0.11.dist-info/METADATA
 Comment: 
 
-Filename: repleno-0.0.10.dist-info/WHEEL
+Filename: repleno-0.0.11.dist-info/WHEEL
 Comment: 
 
-Filename: repleno-0.0.10.dist-info/top_level.txt
+Filename: repleno-0.0.11.dist-info/top_level.txt
 Comment: 
 
-Filename: repleno-0.0.10.dist-info/RECORD
+Filename: repleno-0.0.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## repleno/SKU.py

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 
 from enum import Enum
 from typing import List
 from repleno.utils import *
 import warnings
 from collections import deque
-import pptree
-import logging
 import hashlib
 
+import pptree
+import repleno
 
-class OutputFormatter:
+class _OutputFormatter:
     """
-    Makes things easier to store in a standard dictionary
+    Makes things easier to store in a standard dictionary.
     """
 
     def __init__(self, max_stack_size=None):
         self.records = {}
         self._skus = set()
         self._highest_level = None
         self._max_stack_size = max_stack_size
@@ -79,15 +79,15 @@
         if direction == "parents":
             if level > self.records[sku]["sku_level"]:
                 self.records[sku]["sku_level"] = level
 
     def get_output(self, skus_only=False, attributes=None, hash_keys=False):
         if skus_only:
             skus = self.records.keys()
-            return [(sku.item, sku.location) for sku in skus]
+            return { sku.item if not sku.location else (sku.item, sku.location) for sku in skus}
 
         f_result = deque()
         sku_id_pairs = {}
 
         for sku, val in self.records.items():
             SKUing = str(sku.location) + str(sku.item)
 
@@ -130,15 +130,15 @@
             else:
                 f_result.append(record)
 
         return list(f_result)
 
 
 
-class SKUType(Enum):
+class _SKUType(Enum):
     PARENT = "ultimate parent"
     INTERMEDIATE = "intermediate"
     CHILD = "ultimate child"
     UNDEFINED = "undefined"
 
 
 class _SKULink:
@@ -168,19 +168,32 @@
         if value <= 0:
             raise ValueError("Quantity must be a positive number.")
 
         self._qty = value
 
 
 class SKU:
-    """Any single article held in stock inside of the factory. It can be any
-    item finished good (FG), semi-assemblies or raw-materials.
     """
+    Class for keeping track of an item in inventory.
+
+    Stock keeping unit (SKU) is a unique combination of an item/part code in a
+    location.
 
-    __slot__ = ["item", "location", "sellable", "phantom", "obsolete", "_type", "status", "_abc_classifications", "abc_classification", "safety_stock_qty", "lead_time", "inventory_qty", "minimum_order_qty", "batch_qty", "_child_links", "_parent_links", "_pptree_parents", "_pptree_children"]
+    It's covers products to costumers, assemblies and purchased
+    materials.
+
+    Note
+    ----
+    Current location is always in the output of properties and functions.
+    Because sometimes different factories have the same item/part code.    
+
+    """
+
+
+    __slot__ = ["item", "location", "sellable", "phantom", "obsolete", "_type", "status", "_abc_classifications", "abc_classification", "safety_stock_qty", "lead_time", "inventory_qty", "minimum_order_qty", "batch_size", "_child_links", "_parent_links", "_pptree_parents", "_pptree_children"]
 
     classification_rank = {
         "AX": 90,
         "AY": 80,
         "AZ": 70,
         "BX": 60,
         "BY": 50,
@@ -190,69 +203,85 @@
         "CZ": 10,
         "NA": 00,
     }
 
     def __init__(
         self,
         item,
-        location,
+        location: str = None,
         inventory_qty: float = 0,
-        minimum_order_qty: float = 1,
-        batch_qty: float = 0,
+        minimum_order_qty: float = 0,
+        batch_size: float = 0,
         safety_stock_qty: float = 0,
         lead_time: int = 0,
         abc_classification="NA",
         sellable=False,
         phantom=False,
         obsolete=False,
         status=None,
     ):
         # Keys
-        self.item = item
+        if not isinstance(item, str):
+            raise TypeError(f"Bad type for '{item}': item must be a string, not a {type(item)}")
+        if not item:
+            raise ValueError(f"Item '{item}' must be a non-empty string.")
+        self.item = item.strip().upper()
+
+        if location is not None:
+            if not isinstance(location, str):
+                raise TypeError(f"Bad type for: '{location}': location must be a string, not a {type(location)}")
+            if not location:
+                raise ValueError(f"Location '{location}' must be a non-empty string.")
+            location = location.strip().upper()
         self.location = location
 
         # Qualitative fields
         self.sellable = sellable
         self.phantom = phantom
         self.obsolete = obsolete
-        self._type = SKUType.UNDEFINED
+        self._type = _SKUType.UNDEFINED
         self.status = status 
         # Classification: necessary if setter gets classification before assigning a classification
         self._abc_classification = "NA"
         self.abc_classification = abc_classification
 
         # Numerical fields
         self.safety_stock_qty = safety_stock_qty
         self.lead_time = lead_time
         self.inventory_qty = inventory_qty
         self.minimum_order_qty = minimum_order_qty
-        self.batch_qty = batch_qty
+        self.batch_size = batch_size
 
         # Links between the items
         self._child_links: List[_SKULink] = []
         self._parent_links: List[_SKULink] = []
 
         # Links between the items (only for pptree library)
         self._pptree_parents: List[SKU] = []
         self._pptree_children: List[SKU] = []
 
     def __repr__(self):
         return f"SKU(location={self.location}, item={self.item})"
 
     def __str__(self):
-        return f"{self.item}"
+        output = f"{self.item}"
+        if self.location:
+            output + f" at {self.location}"
+
+        return output
 
     def __eq__(self, other):
         if isinstance(other, SKU):
             return (self.location, self.item) == (other.location, other.item)
         return False
 
     def __hash__(self):
         return hash((self.location, self.item))
 
+
     # Children
     # ========================
 
     @property
     def children(self):
         """Returns all the immediate child items."""
         output = set()
@@ -360,37 +389,37 @@
         """Set the value of minimum order qty."""
         try:
             value = float(value)
         except TypeError:
             print("minimum order qty must be an integer or a float.")
             raise
 
-        if value <= 0:
+        if value < 0:
             raise ValueError(f"minimum order qty must be a positive number.")
 
         self._minimum_order_qty = float(value)
 
     @property
-    def batch_qty(self):
+    def batch_size(self):
         """Get the value of rounding value qty."""
-        return self._batch_qty
+        return self._batch_size
 
-    @batch_qty.setter
-    def batch_qty(self, value):
+    @batch_size.setter
+    def batch_size(self, value):
         """Set the value of rounding value qty."""
         try:
             value = float(value)
         except TypeError:
             print("rounding value qty must be an integer or a float.")
             raise
 
         if value < 0:
             raise ValueError(f"rounding value qty must be a positive number.")
 
-        self._batch_qty = float(value)
+        self._batch_size = float(value)
 
     @property
     def safety_stock_qty(self):
         """Get the value of safety stock qty."""
         return self._safety_stock_qty
 
     @safety_stock_qty.setter
@@ -428,38 +457,38 @@
 
     @property
     def type(self):
         return self._type.value
 
     @type.setter
     def type(self, value):
-        if not isinstance(value, SKUType):
+        if not isinstance(value, _SKUType):
             raise TypeError(
                 f"Argument must be of type NodeType.\nYour value is:{value} and type: {type(value)}"
             )
 
-        if value == SKUType.INTERMEDIATE:
+        if value == _SKUType.INTERMEDIATE:
             raise ValueError(
                 f"You can only assign the values: PARENT and CHILD.\nYour value is: {value.name}"
             )
 
         # current   new     result
         # ===========================
         # None      parent  parent
         # None      child   child
         # child     parent  intermediate
         # child     child   child
         # parent    parent  parent
         # parent    child   intermediate
 
         if value != self._type:
-            if self._type == SKUType.UNDEFINED:
+            if self._type == _SKUType.UNDEFINED:
                 self._type = value
             else:
-                self._type = SKUType.INTERMEDIATE
+                self._type = _SKUType.INTERMEDIATE
 
 
     def _level_order_traverse(self, direction):
         # try to get the attribute
         if getattr(self, direction) is None:
             raise AttributeError(
                 f"Attribute {direction} not found in class {self.__class__.__name__}"
@@ -487,15 +516,16 @@
         root_nodes = []
 
         while stack:
             node = stack.pop()
             if len(getattr(node, direction)) == 0:
                 root_nodes.append(node)
             else:
-                stack += getattr(node, direction)
+                for sku in getattr(node, direction):
+                    stack.add(sku)
 
         return root_nodes
 
 
     @property
     def abc_classification(self):
         return self._abc_classification
@@ -567,53 +597,65 @@
             return self.safety_stock_qty
 
         if self.inventory_qty < self.safety_stock_qty:
             return self.safety_stock_qty - self.inventory_qty
         else:
             return 0
 
-    def lot_size(self, order_qty):
-        """Rounds the order quantity to the nearest multiple of the minimum order quantity.
-
-        If a rounding order quantity is specified, the rounded value will be a multiple
-        of the rounding value that is higher than the minimum order quantity.
+    def _adjust_qty_to_moq_and_batch(self, order_qty: int | float) -> repleno._Order:
+        """
+        Rounds the quantity according to the minimum order qty and batch size of the SKU.
 
-        Args:
-            order_qty (float): The order quantity to round.
-
-        Returns:
-            float: The rounded order quantity.
+        Parameters
+        ----------
+        order_qty : int | float
+            Quantity to be lot sized.
+
+        Returns
+        -------
+        _Order
+            Order with the adjusted quantity
 
         """
+
         if order_qty == 0:
             return 0
 
-        if self.batch_qty:
-            min_qty = self.minimum_order_qty or 0
-            order_qty = max(order_qty, min_qty)
-            return get_next_multiple(order_qty, self.batch_qty)
-
-        if self.minimum_order_qty:
-            return max(order_qty, self.minimum_order_qty)
-
-    def _link_both_skus(self, child_sku, qty):
-        """
-        Note: this is an internal method that can be used externally only by the
-        Factory class. This is because the Factory needs to register it to keep
-        track of all the items.
+        if order_qty <= self.minimum_order_qty:
+            return self.minimum_order_qty
+
+        if not self.batch_size:
+            return order_qty
+
+        order_qty_diff = order_qty - self.minimum_order_qty  
+        above_moq_qty = math.ceil(order_qty_diff / self.batch_size) * self.batch_size
+
+        return self.minimum_order_qty + above_moq_qty
 
+
+    def _link_child(self, child_sku, qty=1):
+        """
+        Internal Method to be used exclusively by the Factory class. This is
+        because the Factory needs to register it to keep track of all the
+        items.
         """
+
         if not isinstance(child_sku, SKU):
-            raise TypeError("child_node argument must be of type Item.")
+            raise TypeError(f"Bad type: child_sku argument must be {type(SKU)}")
 
         if self.item == child_sku.item and self.location == child_sku.location:
-            warnings.warn(
-                f"parent and child skus cannot be the same.\n{child_sku.item} is parent and child at the same time"
-            )
-        
+            warnings.warn(f"SKU cannot be linked to itself.")
+            return 
+
+        try:
+            qty = convert_to_float(qty)
+        except Exception as e:
+            print(f"'{qty}' was not able to be converted to a float number.")
+            raise
+ 
         self._check_for_recursion(child_sku)
         self._update_types(child_sku)
         self._update_sellable_flag(child_sku)
         self._add_child_for_pptree_visualisation(child_sku)
 
         # Link both ways: parent > child and child > parent
         if not isinstance(qty, (float, int)):
@@ -622,171 +664,51 @@
         self._child_links.append(_SKULink(child_sku, qty))
         child_sku._parent_links.append(_SKULink(self, 0 if qty == 0 else 1 / qty))
 
 
     def _check_for_recursion(self, child_node):
         if child_node in self.all_parents:
             raise ValueError(
-                f"Linking the parent-child relationship ('{self.item}'>>'{child_node.code}') resulted in recursion."
+                f"Linking the child '{child_node.item}' to the parent '{self.item}' resulted in recursion."
             )
 
     def _update_types(self, child_node):
-        self.type = SKUType.PARENT
-        child_node.type = SKUType.CHILD
+        # NOTE: the property type must be used for validation, not "_type"
+        self.type = _SKUType.PARENT  
+        child_node.type = _SKUType.CHILD 
 
     def _update_sellable_flag(self, child_node):
-        if self.type == SKUType.PARENT:
+        if self._type == _SKUType.PARENT:
             self.sellable = True
 
-        if child_node.type == SKUType.PARENT:
+        if child_node._type == _SKUType.PARENT:
             self.sellable = True
 
     def _add_child_for_pptree_visualisation(self, child_node):
         child_node._pptree_parents.append(self)
         self._pptree_children.append(child_node)
 
     def show(self, direction="children"):
         if direction not in ["children", "parents"]:
             raise ValueError('direction arg must be "children" or "parents"')
         else:
             # second argument is property name of Node that holds next node
             pptree.print_tree(self, childattr="_pptree_" + direction)
 
-    def get_phaseout_collaterals(self, tree=False):
-        """
-        Returns all items that should be phased out together
-
-        Args:
-            tree (bool, optional): If true, it returns the same item with the
-            prefix "po_" and linked to this item are the item collaterals.
-            Defaults to False and returns only a list of item codes that are
-            collaterals.
-
-        Returns:
-            list or Item: returns a list if tree is False, otherwise it returns
-            an Item.
-        """
-        logging.debug(f"Getting collaterals for {self.item}")
-
-        po_self = SKU(self.item)
-
-        parent_collat, po_self = self._link_parents_to_po_item(po_self)
-        child_collat, po_self = self._link_child_to_po_item(parent_collat, po_self)
-
-        all_collaterals = set()
-        all_collaterals.update(parent_collat)
-        all_collaterals.update(child_collat)
-        all_collaterals.discard(self.item)
-
-        if tree:
-            return po_self
-        else:
-            return all_collaterals
-
-    def _link_parents_to_po_item(self, po_self):
-        """
-        Check if parent items should be part of collaterals when self is being
-        obsoleted
-        """
-        if po_self is not None and not isinstance(po_self, SKU):
-            raise TypeError(
-                f"input is an instance of {type(po_self)}, it must be of type Item."
-            )
-
-        logging.debug(f"traversing {len(self.parents)} parents for item {self.item}")
-
-        # Insert None so the new tree can be linked to po_self
-        stack = [(parent, None) for parent in self.parents]
-        collat_list = set()
-
-        while stack:
-            parent, child = stack.pop()
-
-            # === for tree ===
-            if child is None:
-                po_child = po_self
-            else:
-                po_child = SKU(child.code)
-
-            po_parent = SKU(parent.code)
-            po_parent._link_both_skus(po_child)
-
-            # === for list ===
-            collat_list.add(parent.code)
-            collaterals, po_parent = parent._link_child_to_po_item(
-                collat_list, po_parent
-            )
-            collat_list.update(collaterals)
-
-            # === traversal ===
-            child = parent
-            for p in child.parents[::-1]:
-                if p.code is not collaterals:
-                    stack.append((p, child))
-
-        return collat_list, po_self
-
-    def _link_child_to_po_item(self, collaterals, po_self):
-        """
-        Check if child items should be part of collaterals when self is being
-        obsoleted
-        """
-        if po_self is not None and not isinstance(po_self, SKU):
-            raise TypeError(
-                f"input is an instance of {type(po_self)}, it must be of type Item."
-            )
-
-        stack = [(None, child) for child in self.children]
-        result = set()
-
-        while stack:
-            parent, child = stack.pop()
-
-            po_child = SKU(child.code)
-            if parent is None:
-                po_parent = po_self
-            else:
-                po_parent = SKU(parent.code)
-
-            not_sellable_single_parent = len(child.parents) <= 1 and not child.sellable
-
-            parents_code = [i.code for i in child.parents]
-            all_parents_in_collaterals = not bool(set(parents_code) - collaterals)
-            not_sellable_all_parents_in_collaterals = (
-                len(child.parents) > 1
-                and all_parents_in_collaterals
-                and not child.sellable
-            )
-
-            if not_sellable_single_parent or not_sellable_all_parents_in_collaterals:
-                # for tree
-                child_codes = [i.code for i in po_parent.children]
-                if po_child.item not in child_codes:
-                    po_parent._link_both_skus(po_child)
-
-                # for list
-                result.add(child.code)
-
-                parent = child
-                for c in parent.children[::-1]:
-                    if c.code is not collaterals:
-                        stack.append((parent, c))
-
-        return result, po_self
 
     def _are_levels_equal(self, node, direction, past_node=None):
         anti_direction = "parents" if direction == "children" else "children"
 
         if not self and not node:
             # both nodes are empty, so they're equal
             return True
         elif not self or not node:
             # one node is empty and the other is not, so they're not equal
             return False
-        elif self.item != node.code:
+        elif self.item != node.item:
             # the nodes have different values, so the trees are not equal
             return False
         elif len(getattr(self, direction)) != len(getattr(node, direction)):
             # the nodes have different numbers of children, so the trees are not equal
             return False
         elif past_node is not None and len(getattr(self, anti_direction)) > 1:
             # recursively check the children of the parents or the parents of the children
@@ -858,88 +780,122 @@
             "stocking_type": the stocking type,
             "level": starts at 0 with root items and increases by +1,
         }
 
         The parents list contains only items that have id's
         """
 
-        output = OutputFormatter(max_stack_size=max_stack_size)
+        # Breadth-first traversal (BFS) is used because it's easier to think
+        # about the logic by levels
+        
+        output = _OutputFormatter(max_stack_size=max_stack_size)
 
         # add current items and iterate over the children
         # ===============================================
         if not include_obsoletes and self.obsolete:
             return []
 
-        parent_skus = self.parents if include_obsoletes else self.active_parents
-        queue = [(parent_skus, self, 0)]  # (previous_sku, current_sku, level)
+        selected_parents = self.parents if include_obsoletes else self.active_parents
+        queue = [(selected_parents, self, 0)]  # (previous_sku, current_sku, level)
         while queue:
             for _ in range(len(queue)):
                 sku_ancestor, sku, level = queue.pop(0)
 
-                child_skus = sku.child_skus if include_obsoletes else sku.active_children
+                selected_children = sku.child_skus if include_obsoletes else sku.active_children
 
                 output.store(
                     sku=sku,
                     parent_skus=sku_ancestor,
-                    child_skus=child_skus,
+                    child_skus=selected_children,
                     level=level,
                     direction="children",
                 )
 
-                for child_sku in sku.child_skus:
-                    queue.append((sku, child_sku, level - 1))
+                for c_sku in selected_children:
+                    queue.append((sku, c_sku, level - 1))
 
         # iterate over the parents
         # ==========================
         # get parent nodes from node
 
-        child_skus = self.child_skus if include_obsoletes else self.active_children
-        queue = [(child_skus, self, 0)]
+        selected_children = self.child_skus if include_obsoletes else self.active_children
+        queue = [(selected_children, self, 0)]
         while queue:
             for _ in range(len(queue)):
                 sku_ancestor, sku, level = queue.pop(0)
 
-                parent_skus = sku.parents if include_obsoletes else sku.active_parents
+                selected_parents = sku.parents if include_obsoletes else sku.active_parents
 
                 output.store(
                     sku=sku,
-                    parent_skus=parent_skus,
+                    parent_skus=selected_parents,
                     child_skus=sku_ancestor,
                     level=level,
                     direction="parents",
                 )
 
-                for parent_sku in sku.parents:
-                    queue.append((sku, parent_sku, level + 1))
+                for p_sku in selected_parents:
+                    queue.append((sku, p_sku, level + 1))
 
         return output.get_output(attributes=attributes)
 
 
     def get_collaterals(
         self,
         include_obsoletes=False,
-        max_stack_size=None,
-        attributes=None,
         skus_only=False,
+        attributes=None,
+        max_stack_size=None,
     ):
         """
+        # TODO: complete docstring
+
+        It returns a list of dictionaries with the following keys:
+
         It generates a list of all items that meet the following criteria:
             1. Items that use item_code as input material for their produciton;
             2. Items that are used as input material for item_code's production;
             3. Any indirect items that satisfy the point 1 or 2.
 
-        It returns a list of dictionaries with the following keys:
-
-            TODO: complete doscstring
+        Parameters
+        ----------
+        include_obsoletes : bool, optional
+            Obsolete items are not considered when gathering the collaterals, by
+            default False
+            
+        skus_only : bool, optional
+            It return a set with the SKU's that are collaterals, by default False
+
+        attributes : _type_, optional
+            Returns the list of dictionaries including the SKU attributes
+            specified here. The attributes here must match the SKU attribute
+            names, by default None
+            
+        max_stack_size : int, optional
+            It throws an error if the amount of collaterals collected exceeds
+            the stack size, by default None
+            
+        Returns
+        -------
+        list
+            If skus_only = True, it returns a list with the skus. 
+            Otherwise, it returns a list of dictionaries with the following
+            keys:
+            - # TODO: complete list
+            - + attributes (if specified)
 
         """
+
+        # Breadth-first traversal (BFS) is used because it's easier to think
+        # about the logic by levels
+
         if not include_obsoletes and self.obsolete:
             return []
 
-        output = OutputFormatter(max_stack_size=max_stack_size)
+        output = _OutputFormatter(max_stack_size=max_stack_size)
 
         output = self._scan_this_and_parents(
             collaterals=output,
             include_obsoletes=include_obsoletes,
         )
         output = self._scan_children(
             collaterals=output,
@@ -948,75 +904,76 @@
         )
 
         return output.get_output(skus_only, attributes, skus_only)
 
     def _scan_this_and_parents(self, collaterals, include_obsoletes):
         p_collaterals = collaterals
 
-        child_skus = self.children if include_obsoletes else self.active_children
+        child_skus = self.children if include_obsoletes else self.active_children  # just to record previous skus
         queue = [(child_skus, self, 0)]  # (previous_sku, current_sku, level)
         while queue:
             for _ in range(len(queue)):
                 sku_ancestor, sku, level = queue.pop(0)
 
                 # Scan the children and add the result to p_collaterals
-                p_collaterals = sku._scan_children(collaterals=p_collaterals, level=level, include_obsoletes=include_obsoletes)
+                if self != sku:
+                    p_collaterals = sku._scan_children(collaterals=p_collaterals, level=level, include_obsoletes=include_obsoletes)
 
                 # Filter out obsoletes if needed
-                parent_skus = sku.parents if include_obsoletes else sku.active_parents
+                selected_parents = sku.parents if include_obsoletes else sku.active_parents
 
                 # Add parent to collaterals
                 p_collaterals.store(
                     sku=sku,
-                    parent_skus=parent_skus,
+                    parent_skus=selected_parents,
                     child_skus=sku_ancestor,
                     level=level,
                     direction="parents",
                 )
 
-                for parent_node in sku.parents:
+                for parent_node in selected_parents:
                     queue.append((sku, parent_node, level + 1))
 
         return p_collaterals
 
     def _scan_children(self, collaterals, level, include_obsoletes):
         """
         Check if child items should be part of collaterals when self is being
         obsoleted
         """
 
         # Start from the children
-        mod_children = self.children if include_obsoletes else self.active_children
+        selected_children = self.children if include_obsoletes else self.active_children
         # Remove any SKU that is already in collaterals
-        mod_children = mod_children - collaterals._skus        
+        selected_children = selected_children - collaterals._skus        
 
-        queue = [(self, sku, level - 1) for sku in mod_children]
+        queue = [(self, sku, level - 1) for sku in selected_children]
         while queue:
             for _ in range(len(queue)):
                 sku_ancestor, sku, level = queue.pop(0)
 
                 # Logic to see if child should be added
                 unique_parent = len(sku.parents) <= 1
                 all_parents_in_collaterals = not bool(set(sku.parents) - collaterals._skus)
 
-                add_children = unique_parent and not sku.sellable or all_parents_in_collaterals
+                add_children = (unique_parent or all_parents_in_collaterals) and not sku.sellable
 
                 if add_children:
                     # Filter out obsoletes if needed
-                    mod_children = sku.children if include_obsoletes else sku.active_children
-                    mod_children = mod_children - collaterals._skus
+                    selected_children = sku.children if include_obsoletes else sku.active_children
+                    selected_children = selected_children - collaterals._skus
 
                     # Add child to collaterals
                     collaterals.store(
                         sku=sku,
                         parent_skus=sku_ancestor,
-                        child_skus=mod_children,
+                        child_skus=selected_children,
                         level=level,
                         direction="children",
                     )
 
                     # Move to next children
-                    for child_node in mod_children:
+                    for child_node in selected_children:
                         if not collaterals.records.get(child_node):
                             queue.append((sku, child_node, level - 1))
         
         return collaterals
```

## repleno/__init__.py

```diff
@@ -1,5 +1,21 @@
 # Set default logging handler to avoid "No handler found" warnings.
 import logging
 from logging import NullHandler
 
 logging.getLogger(__name__).addHandler(NullHandler())
+
+
+from repleno.factory import Factory
+from repleno.order import _Order
+from repleno.SKU import SKU
+from repleno.SKU import _SKUType
+from repleno.order import _OrderType
+
+# Use __all__ to let type checkers know what is part of the public API.
+__all__ = [
+    "Factory",
+    "_Order",
+    "SKU",
+    "_SKUType",
+    "_OrderType",
+]
```

## repleno/factory.py

```diff
@@ -1,86 +1,66 @@
 from __future__ import annotations
 from datetime import datetime
 from repleno.utils import *
-from repleno.order import Order
-from repleno.SKU import SKU
-from repleno.SKU import SKUType
-from repleno.order import OrderType
 
 import warnings
-
-
-# future improvements
-# todo: in factory, develop mrp that is focused on obsoletion, covering the 3 scenarios (scrap everything, produce and scrap, produce everything)
-# todo: method for flushing any general label from root to child nodes.
-# todo: when parameters are being loaded and column is not perfectly what's in the file, no warning is issue! Or if column is not found.
-# todo: if one component goes out of stock, what's the impact on the finished goods in units?
-# todo: during MRP, if an order is issued to a specific item and the long time of this item is longer than the sales lead time, issue a warning (?)
-# todo: add average sales as property to the item class and flush down a category (VS and sub-VS)
-# todo: consider the different UoM's
-# todo: per component, shows how much of its demand impact finished goods. If 1 component goes into only 1 FG, then 100%
-# todo: allow user to specify date formatting
+import repleno as repl
 
 
 class Factory:
-    """
-    The factory class stores all the SKU's created.
-    """
 
     def __init__(self, bom=None, bom_mapping = None, parameters=None, parameters_mapping=None):
         self._skus = {}
 
         if bom:
             self.load_bom(bom, bom_mapping)
 
         if parameters:
             self.load_parameters(parameters, parameters_mapping)
 
         self._cache = {}  # don't use @lru_cache because of memory leak
 
     @property
-    def items_mapping(self):
-        return self._skus
+    def all_item_location_pairs(self) -> set:
+        return {key for key in self._skus.keys()}
 
     @property
-    def skus(self):
-        # if no location available, return only item
-        return [item_loc if item_loc[0] else item_loc[1] for item_loc in self._skus.keys()]
-
+    def all_skus(self) -> set:
+        return {key for key in self._skus.values()}
 
     @property
-    def item_codes(self):
-        output_list = [item[0] for item in self._skus.items()]
-
-        return output_list
+    def all_items(self) -> set:
+        # if no location available, return only item
+        return {item_loc[0] for item_loc in self._skus.keys()}
 
     @property
-    def abc_classifications(self):
+    def abc_classifications(self) -> dict:
         result = {}
-        for item in self.skus:
-            result[item.code] = item.abc_classification
+        for sku in self.skus:
+            result[(sku.item, sku.location)] = sku.abc_classification
 
         return result
 
-    def get_sku(self, item, location=None):
+    def get_sku(self, item: str, location: str = None) -> repl.SKU:
+        # TODO: accept a tuple as well, it should be easy to query the fact.skus, select one and use the get_skus()
         item_fmt = str(item).strip().upper()
 
         if not location:
             return self._skus.get((item_fmt, None))
         
         location_fmt = str(location).strip().upper()
         return self._skus.get((item_fmt, location_fmt))
 
     def load_bom(
         self,
         data: str | list[dict],
         mapping: list[dict] = None,
     ):
         """
-        Load the bill of materials (BOM) into the model.
+        Load bill of materials into the model.
  
         Parameters
         ----------
         data : str | list[dict]
             A CSV filename or a list of dictionaries with the following
             keys/column names: 
 
@@ -144,35 +124,29 @@
         self,
         item,
         child_item,
         qty=1,
         location=None,
         child_location=None,
     ):
-        # Validate/transform inputs
-        try:
-            qty = convert_to_float(qty)
-        except Exception as e:
-            print(f"'{qty}' was not able to be converted to a float number.")
-            raise
-
+        # Format items and locations in the same way that SKU will do for
+        # consistency when using get_sku()
         item = item.strip().upper()
+        child_item = child_item.strip().upper()
+
         if location:
             location = location.strip().upper()
 
-        child_item = child_item.strip().upper()
         if child_location:
             child_location = child_location.strip().upper()
 
         # Get or register SKUs in factory
-        sku = self._skus.setdefault((item, location), SKU(item=item, location=location))
-        child_sku = self._skus.setdefault((child_item, child_location), SKU(item=child_item, location=child_location))
-
-        # Link SKUs both ways
-        sku._link_both_skus(child_sku, qty)
+        sku = self._skus.setdefault((item, location), repl.SKU(item=item, location=location))
+        child_sku = self._skus.setdefault((child_item, child_location), repl.SKU(item=child_item, location=child_location))
+        sku._link_child(child_sku, qty)
 
 
     def load_parameters(self, data: str | list, mapping: list = None, sellable_true_value: str = None, phantom_true_value: str = None, obsolete_true_value: str = None) -> None:
         """
         Load parameters into the model.
 
         data : str | list
@@ -186,15 +160,15 @@
             - "obsolete": bool, 
             - "status": str,
             - "abc_classification": str, 
             - "safety_stock_qty": int | float, 
             - "lead_time": int | float,
             - "inventory_qty": int | float, 
             - "minimum_order_qty"; int | float,
-            - "batch_qty": int | float 
+            - "batch_size": int | float 
  
         mapping : list, optional
             Remap the keys or column names if data does not have the expected
             ones. Keys are the expected keys (above) and values are the new
             names in your dictionaries or columns.
             If mapping is specified, all keys/column names are considered
             mandatory and error is raised if they are not found.
@@ -215,15 +189,15 @@
         
         # the fields "sellable", "phantom" and obsolete must be booleans. 
         # If the input data is not boolean, the truth values can be defined by passing a string 
         # that represents the truth values to the parameters: `sellable_true_value` and `phantom_true_value`, correspondingly.
         # 
 
         mandatory_keys = ["item"]
-        optional_keys = ["location", "sellable", "phantom", "obsolete", "status", "abc_classification", "safety_stock_qty", "lead_time", "inventory_qty", "minimum_order_qty", "batch_qty"]
+        optional_keys = ["location", "sellable", "phantom", "obsolete", "status", "abc_classification", "safety_stock_qty", "lead_time", "inventory_qty", "minimum_order_qty", "batch_size"]
         data = extract_and_transform_data(data, mandatory_keys, optional_keys, mapping)
 
         if isinstance(data, list) and data:
             for record in data:
                 try:
                     item_code = record["item"]
                     location = record.get("location", None)
@@ -281,17 +255,17 @@
                     if inventory_qty_data:
                         sku.inventory_qty = inventory_qty_data
                     
                     minimum_order_qty_data = record.get("minimum_order_qty", None)
                     if minimum_order_qty_data:
                         sku.minimum_order_qty = minimum_order_qty_data
 
-                    batch_qty_data = record.get("batch_qty", None)
-                    if batch_qty_data:
-                        sku.batch_qty = batch_qty_data
+                    batch_size_data = record.get("batch_size", None)
+                    if batch_size_data:
+                        sku.batch_size = batch_size_data
 
                 except KeyError:
                     print(f"Bad key/column name: make sure the following are in the file: {[key for key in mandatory_keys.keys()]}")
                     raise
 
             return
 
@@ -337,15 +311,15 @@
                         f"No MRP ran for '{i['item']}', as no BOM found for it.",
                         UserWarning,
                         stacklevel=2,
                     )
                     continue
 
                 try:
-                    order = Order(
+                    order = repl._Order(
                         item,
                         datetime.strptime(i["due_date"], date_format),
                         convert_to_float(i["qty"]),
                     )
 
                     output.append(order)
 
@@ -360,37 +334,36 @@
         )
 
     def run_mrp(self, mps, date_format="%Y-%m-%d", mapping=None, output=""):
         # Attention, calling this function alters the Factory object state
         # (inventories will be decreased or increased depending on the
         # requirements generated by the MPS.)
         
-        result_orders = self._get_mps_orders(mps, mapping, date_format)
-
-        if not result_orders:
+        mps_orders = self._get_mps_orders(mps, mapping, date_format)
+        if not mps_orders:
             return []
 
-        final_orders = []
-        for order in result_orders:
-            result_orders = self._compute_child_requirements(order)
-            final_orders += result_orders
+        purchased_orders = []
+        for order in mps_orders:
+            exploded_order = self._explode_orders(order)
+            purchased_orders += exploded_order
 
-        final_orders = self._populate_order_type(final_orders)
+        purchased_orders = self._populate_order_type(purchased_orders)
 
         result = []
-        for order in final_orders:
+        for order in purchased_orders:
             result.append(order.to_dict())
 
         if output:
-            to_csv(result, output)
+            to_csv(result, output, date_keys=["due_date"])
         else:
             return result
 
 
-    def _compute_child_requirements(self, top_order):
+    def _explode_orders(self, top_order):
         """Breaks down the top level order into dependent orders for individual
         subassemblies, component parts and raw materials that are required to
         produce the top level order.
 
         # TODO: transform into examples with >>> 3x not 2x
         >> ord = Order(Order('20220101', Bicycle, 2)) # 2 Bikes for 01/01/22
         >> explode_bom(ord)
@@ -409,82 +382,77 @@
         # gross_order                                          -6  -3  -3
         # new_inventory_qty                                        -4   2   0
         # net_order (to replenish inventory_qty)                    4   -   -
         # net_order_rounded (according to lot size)             5   -   -
         # final_inventory_qty (net_order_rounded - gross_order)     1   -   -
         # ----------------------------------------------------------------
 
-        if not isinstance(top_order, Order):
+        # Depth-first traversal (DFS) is used because it's easier when
+        # debugging. Because each branch is exploded at the time, so there's
+        # less skip steps when debugging.
+        # Pre-order traversal because root node should be visited and have its
+        # calculations first, beforemoving to the child nodes.
+        
+        if not isinstance(top_order, repl._Order):
             raise AttributeError("work_orders must be instance of WorkOrder.")
 
         result = []
-        queue = []
-
-        queue.append(top_order)
-
-        while len(queue) != 0:
-            # Get last order added on the queue and get the net of it
-            gross_order = queue.pop()
-            net_order = self._get_net_workorder(gross_order)
-
-            # adjust inventories acc. to new order
-            sku = gross_order.sku
-            inventory_qty_net_gross_diff = net_order.qty - gross_order.qty
-            sku.inventory_qty += inventory_qty_net_gross_diff
-
-            if net_order.qty != 0:
+        stack = [top_order]
+        while stack:
+                # Get last order added on the queue and get the net of it
+                current_order = stack.pop()
+                sku = current_order.sku
+
+                net_order = self._get_net_workorder(current_order)
+
+                # adjust inventories acc. to new order
+                qty_left_for_inventory = net_order.qty - current_order.qty
+                sku.inventory_qty += qty_left_for_inventory
+
+                # register order, if needed
+                if net_order.qty == 0:
+                    continue   
                 result.append(net_order)
 
                 # adjust the lead time
-                gross_order.due_date = remove_business_days(
-                    gross_order.due_date, sku.lead_time
+                current_order.due_date = remove_business_days(
+                    current_order.due_date, sku.lead_time
                 )
 
-                # get gross order for child and add it to the queue
-                top_order = gross_order
-                for child_link in sku.child_links:
-                    gross_req_qty = net_order.qty * child_link.qty
+                for child_link in reversed(sku.child_links):
+                    exploded_qty = net_order.qty * child_link.qty
 
-                    queue.append(
-                        Order(child_link.sku, top_order.due_date, gross_req_qty)
+                    stack.append(
+                        repl._Order(child_link.sku, current_order.due_date, exploded_qty)
                     )
 
         return result
 
-    def _get_net_workorder(self, order: Order) -> Order:
+    def _get_net_workorder(self, order: repl._Order) -> repl._Order:
         """Subtracts the order qty from the inventory_qty balance for this
         stock unit and if inventory_qty falls below zero returns an order with the
         net requirements lot sized.
 
         """
-        net_quantity = order.qty
+        reorder_qty = (order.qty + order.sku.safety_stock_qty) - order.sku.inventory_qty
 
-        # account for inventory_qty on hand or backorder
-        net_quantity -= order.sku.inventory_qty
-
-        # account for safety stock
-        net_quantity += order.sku.get_missing_safety_stock_qty()
-
-        if net_quantity > 0:
-            net_qty_rounded = order.sku.lot_size(net_quantity)
-            return Order(order.sku, order.due_date, net_qty_rounded)
+        if reorder_qty > 0:
+            net_qty_rounded = order.sku._adjust_qty_to_moq_and_batch(reorder_qty)
+            return repl._Order(order.sku, order.due_date, net_qty_rounded)
         else:
-            return Order(order.sku, order.due_date, 0)
+            return repl._Order(order.sku, order.due_date, 0)
 
-    def _populate_order_type(self, orders: List[Order]):
-        """Populate the type property of Order instances
 
-        Args:
-            orders (List[_Order]): list of Order instances
-        """
+    def _populate_order_type(self, orders: List[repl._Order]):
+        """Populate the type property of Order instances """
         for order in orders:
-            if order.sku.type == SKUType.CHILD:
-                order.type = OrderType.PURCHASE_ORDER
+            if order.sku._type == repl._SKUType.CHILD:
+                order._type = repl._OrderType.PURCHASE_ORDER
             else:
-                order.type = OrderType.WORK_ORDER
+                order._type = repl._OrderType.WORK_ORDER
 
         return orders
 
 
     def export_abc_classifications(self, csv_path):
         to_csv(
             self._format_abc_classification_for_csv(self.abc_classifications), csv_path
@@ -504,24 +472,24 @@
         open_orders_hashed = hash_dicts_list(open_orders)
 
         if (required_orders_hashed, open_orders_hashed) in self._cache:
             return self._cache[(required_orders_hashed, open_orders_hashed)]
 
         # Convert dictionaries of Order objects
         required_orders_fmt = [
-            Order(
-                SKU(o["item_code"]),
+            repl._Order(
+                repl.SKU(o["item_code"]),
                 datetime.strptime(o["due_date"], "%Y-%m-%d").date(),
                 o["qty"],
             )
             for o in required_orders
         ]
         open_orders_fmt = [
-            Order(
-                SKU(o["item_code"]),
+            repl._Order(
+                repl.SKU(o["item_code"]),
                 datetime.strptime(o["due_date"], "%Y-%m-%d").date(),
                 o["qty"],
             )
             for o in open_orders
         ]
 
         # Use a dictionary to keep track of dates and quantities for each item_code.
@@ -550,24 +518,24 @@
         for item in quantities:
             quantities[item].sort(key=lambda x: x[0])
 
         self._cache[(required_orders_hashed, open_orders_hashed)] = quantities
         return quantities
 
     # todo: rename qty to quantity and adjust this as well all over the project
-    def get_inventory_qty_over_time(
+    def get_inventory_over_time(
         self,
         required_orders,
         open_orders,
         item_codes=[],
         shortages_only=False,
         required_orders_field_mapping={},
         open_orders_field_mapping={},
         to_csv_path=None,
-    ): 
+    ):
         """
         Calculates the difference in quantities across time for each item_code in the
         required_orders and open_orders lists.
 
         Args:
             - required_orders (List[Dict[str, any]]): A list of dictionaries
             representing required orders.  Each dictionary contains the
```

## repleno/order.py

```diff
@@ -1,40 +1,40 @@
 from __future__ import annotations
 
-from repleno.SKU import SKU
 from datetime import datetime, date
 from enum import Enum
 
+import repleno as repleno
 
-class OrderType(Enum):
+class _OrderType(Enum):
     WORK_ORDER = "Work Order"
     PURCHASE_ORDER = "Purchase Order"
     NOT_SET = "Not set"
 
 
-class Order:
+class _Order:
     __slot__ = ["_sku", "due_date", "qty", "type"]
 
-    def __init__(self, sku, due_date, qty, type=OrderType.NOT_SET):
-        if not isinstance(sku, SKU):
+    def __init__(self, sku, due_date, qty, type=_OrderType.NOT_SET):
+        if not isinstance(sku, repleno.SKU):
             raise TypeError("sku must be of SKU type")
 
         self._sku = sku
         self.due_date = due_date
         self.qty = qty
         self.type = type
 
     def __repr__(self) -> str:
         return f"Order(sku=SKU({self._sku}), due_date={self._due_date:%Y-%m-%d}, qty={self._qty}, type={self._type})"
 
     def __str__(self) -> str:
         return f"{self._qty} of {self._sku} on {self._due_date:%Y-%m-%d}"
 
-    def __eq__(self, other: Order) -> bool:
-        if isinstance(other, Order):
+    def __eq__(self, other: _Order) -> bool:
+        if isinstance(other, _Order):
             return (
                 self.sku == other.sku
                 and self.due_date == other.due_date
                 and self.qty == other.qty
             )
         return False
 
@@ -71,15 +71,15 @@
 
     @property
     def type(self):
         return self._type
 
     @type.setter
     def type(self, value):
-        if not isinstance(value, OrderType):
+        if not isinstance(value, _OrderType):
             raise TypeError("Value must be of type OrderType.")
 
         self._type = value
 
 
     def to_dict(self):
         return {"location": self.sku.location, "item": self.sku.item, "due_date": self.due_date, "qty": self.qty, "order_type": self.type.value}
```

## repleno/utils.py

```diff
@@ -176,15 +176,15 @@
         if pval_ratio > suggested_word_ratio and (0.6 < pval_ratio < 1.0):
             suggested_word = possible_val
             suggested_word_ratio = pval_ratio
 
     return suggested_word
 
 
-def to_csv(dictionaries, file_path: str):
+def to_csv(dictionaries, file_path: str, date_keys: list = None):
     """Print data in a csv file"""
 
     if not is_valid_dir(file_path):
         raise NotADirectoryError("Directory does not exist: ", file_path)
 
     if not is_valid_csv(file_path):
         raise AttributeError("Path must have csv extension: ", file_path)
@@ -195,16 +195,18 @@
     with open(file_path, "w", newline="") as file:
         file.write(f"sep={separator}\n")
 
         writer = csv.DictWriter(file, delimiter=separator, fieldnames=fieldnames)
 
         writer.writeheader()
 
-        # write the rest of the data
         for row in dictionaries:
+            if date_keys:
+                for key in date_keys:
+                    row[key] = row[key].strftime("%Y-%m-%d")
             writer.writerow(row)
 
 
 def is_valid_dir(path):
     # remove the base name, if any
     only_path = os.path.split(path)[0]
     print(only_path)
@@ -230,19 +232,14 @@
             return 1
 
         return float(input)
     except ValueError:
         print(f"{input} could not be converted into a float number.")
         raise
 
-
-def get_next_multiple(number, multiple):
-    return math.ceil(number / multiple) * multiple
-
-
 def hash_dicts_list(list_dict):
     result_json = json.dumps(list_dict, sort_keys=True)
 
     return hashlib.sha3_256(result_json.encode()).hexdigest()
 
 
 def _get_key(dict, value):
```

