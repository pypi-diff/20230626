# Comparing `tmp/odoo13_addon_gestion_editorial-13.0.0.3.0-py3-none-any.whl.zip` & `tmp/odoo13_addon_gestion_editorial-13.0.0.3.1.dev3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,18 @@
-Zip file size: 1418 bytes, number of entries: 4
--rw-r--r--  2.0 unx      503 b- defN 23-May-22 16:05 odoo13_addon_gestion_editorial-13.0.0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 16:05 odoo13_addon_gestion_editorial-13.0.0.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-22 16:05 odoo13_addon_gestion_editorial-13.0.0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      408 b- defN 23-May-22 16:05 odoo13_addon_gestion_editorial-13.0.0.3.0.dist-info/RECORD
-4 files, 1008 bytes uncompressed, 612 bytes compressed:  39.3%
+Zip file size: 14391 bytes, number of entries: 16
+-rw-r--r--  2.0 unx       68 b- defN 23-Jun-26 17:44 gestion_editorial/__init__.py
+-rw-r--r--  2.0 unx     1538 b- defN 23-Jun-26 17:44 gestion_editorial/__manifest__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-Jun-26 17:44 gestion_editorial/models/__init__.py
+-rw-r--r--  2.0 unx    14028 b- defN 23-Jun-26 17:52 gestion_editorial/models/liquidacion_descontrol.py
+-rw-r--r--  2.0 unx     5085 b- defN 23-Jun-26 17:44 gestion_editorial/models/product_descontrol.py
+-rw-r--r--  2.0 unx      400 b- defN 23-Jun-26 17:44 gestion_editorial/models/purchase_order_descontrol.py
+-rw-r--r--  2.0 unx      738 b- defN 23-Jun-26 17:44 gestion_editorial/models/res_partner_descontrol.py
+-rw-r--r--  2.0 unx     2785 b- defN 23-Jun-26 17:44 gestion_editorial/models/sale_order_descontrol.py
+-rw-r--r--  2.0 unx     6376 b- defN 23-Jun-26 17:44 gestion_editorial/models/stock_picking_descontrol.py
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-26 17:44 gestion_editorial/wizards/__init__.py
+-rw-r--r--  2.0 unx       44 b- defN 23-Jun-26 17:44 gestion_editorial/wizards/liquidacion_lineas_pendientes/__init__.py
+-rw-r--r--  2.0 unx     6000 b- defN 23-Jun-26 17:44 gestion_editorial/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.py
+-rw-r--r--  2.0 unx      508 b- defN 23-Jun-26 17:52 odoo13_addon_gestion_editorial-13.0.0.3.1.dev3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-26 17:52 odoo13_addon_gestion_editorial-13.0.0.3.1.dev3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-26 17:52 odoo13_addon_gestion_editorial-13.0.0.3.1.dev3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1695 b- defN 23-Jun-26 17:52 odoo13_addon_gestion_editorial-13.0.0.3.1.dev3.dist-info/RECORD
+16 files, 39671 bytes uncompressed, 11453 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -1,13 +1,49 @@
-Filename: odoo13_addon_gestion_editorial-13.0.0.3.0.dist-info/METADATA
+Filename: gestion_editorial/__init__.py
 Comment: 
 
-Filename: odoo13_addon_gestion_editorial-13.0.0.3.0.dist-info/WHEEL
+Filename: gestion_editorial/__manifest__.py
 Comment: 
 
-Filename: odoo13_addon_gestion_editorial-13.0.0.3.0.dist-info/top_level.txt
+Filename: gestion_editorial/models/__init__.py
 Comment: 
 
-Filename: odoo13_addon_gestion_editorial-13.0.0.3.0.dist-info/RECORD
+Filename: gestion_editorial/models/liquidacion_descontrol.py
+Comment: 
+
+Filename: gestion_editorial/models/product_descontrol.py
+Comment: 
+
+Filename: gestion_editorial/models/purchase_order_descontrol.py
+Comment: 
+
+Filename: gestion_editorial/models/res_partner_descontrol.py
+Comment: 
+
+Filename: gestion_editorial/models/sale_order_descontrol.py
+Comment: 
+
+Filename: gestion_editorial/models/stock_picking_descontrol.py
+Comment: 
+
+Filename: gestion_editorial/wizards/__init__.py
+Comment: 
+
+Filename: gestion_editorial/wizards/liquidacion_lineas_pendientes/__init__.py
+Comment: 
+
+Filename: gestion_editorial/wizards/liquidacion_lineas_pendientes/liquidacion_lineas_pendientes.py
+Comment: 
+
+Filename: odoo13_addon_gestion_editorial-13.0.0.3.1.dev3.dist-info/METADATA
+Comment: 
+
+Filename: odoo13_addon_gestion_editorial-13.0.0.3.1.dev3.dist-info/WHEEL
+Comment: 
+
+Filename: odoo13_addon_gestion_editorial-13.0.0.3.1.dev3.dist-info/top_level.txt
+Comment: 
+
+Filename: odoo13_addon_gestion_editorial-13.0.0.3.1.dev3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

