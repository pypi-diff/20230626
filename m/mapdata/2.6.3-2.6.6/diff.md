# Comparing `tmp/mapdata-2.6.3.tar.gz` & `tmp/mapdata-2.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.6.3.tar", last modified: Sat Jun 24 22:29:17 2023, max compression
+gzip compressed data, was "mapdata-2.6.6.tar", last modified: Mon Jun 26 00:24:46 2023, max compression
```

## Comparing `mapdata-2.6.3.tar` & `mapdata-2.6.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-24 22:29:17.748690 mapdata-2.6.3/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.6.3/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.6.3/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4019 2023-06-24 22:29:17.748690 mapdata-2.6.3/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2821 2023-06-23 20:29:24.000000 mapdata-2.6.3/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-24 22:29:17.744690 mapdata-2.6.3/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   328878 2023-06-24 21:57:48.000000 mapdata-2.6.3/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-24 22:29:17.748690 mapdata-2.6.3/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4019 2023-06-24 22:29:17.000000 mapdata-2.6.3/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-24 22:29:17.000000 mapdata-2.6.3/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-24 22:29:17.000000 mapdata-2.6.3/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-24 22:29:17.000000 mapdata-2.6.3/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-24 22:29:17.748690 mapdata-2.6.3/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-24 22:15:50.000000 mapdata-2.6.3/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-26 00:24:46.342885 mapdata-2.6.6/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.6.6/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.6.6/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3962 2023-06-26 00:24:46.342885 mapdata-2.6.6/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2738 2023-06-26 00:24:30.000000 mapdata-2.6.6/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-26 00:24:46.342885 mapdata-2.6.6/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   331077 2023-06-26 00:16:11.000000 mapdata-2.6.6/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-26 00:24:46.342885 mapdata-2.6.6/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     3962 2023-06-26 00:24:46.000000 mapdata-2.6.6/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-26 00:24:46.000000 mapdata-2.6.6/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-26 00:24:46.000000 mapdata-2.6.6/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-26 00:24:46.000000 mapdata-2.6.6/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-26 00:24:46.342885 mapdata-2.6.6/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1339 2023-06-26 00:17:02.000000 mapdata-2.6.6/setup.py
```

### Comparing `mapdata-2.6.3/LICENSE.txt` & `mapdata-2.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.6.3/PKG-INFO` & `mapdata-2.6.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.6.3
-Summary: An interactive map and table explorer for geographic coordinates in a CSV file
+Version: 2.6.6
+Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,15 +35,14 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
-![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png){width=50%}
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
```

### Comparing `mapdata-2.6.3/README.md` & `mapdata-2.6.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
-![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png){width=50%}
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
```

### Comparing `mapdata-2.6.3/mapdata/mapdata.py` & `mapdata-2.6.6/mapdata/mapdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "2.6.3"
-vdate = "2023-06-24"
+version = "2.6.6"
+vdate = "2023-06-25"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -579,14 +579,27 @@
 		return rv
 	except:
 		return None
 
 def isboolean(v):
 	return parse_boolean(v) is not None
 
+def conv_datetime(v):
+	if v is None or (type(v) is str and v.strip() == ''):
+		return None
+	try:
+		rv = parse_datetime(v)
+	except:
+		try:
+			d = parse_date(v)
+			rv = datetime.datetime.combine(d, datetime.datetime.min.time())
+		except:
+			return None
+	return rv
+
 
 def dt_type(v):
 	# Type of date/time: timestamp, date, or None
 	if type(v) is str and v.strip() == '':
 		v = None
 	if parse_date(v):
 		return "date"
@@ -594,15 +607,15 @@
 		return "timestamp"
 	if parse_datetimetz(v):
 		return "timestamptz"
 	return None
 
 def data_type(v):
 	# Characterizes the value v as one of a simple set of data types.
-	# Returns "timestamp", "date", "int", "float", or "string"
+	# Returns "timestamp", "date", "timestamptz", "int", "float", "boolean", or "string"
 	if v is None or (type(v) is str and v == ''):
 		return None
 	if isint(v):
 		return "int"
 	if isfloat(v):
 		return "float"
 	dt = dt_type(v)
@@ -612,17 +625,17 @@
 		return "boolean"
 	return "string"
 
 def data_type_cast_fn(data_type_str):
 	if data_type_str == "string":
 		return str
 	elif data_type_str == "date":
-		return datetime.date
+		return parse_date
 	elif data_type_str == "timestamp":
-		return parse_datetime
+		return conv_datetime
 	elif data_type_str == "timestamptz":
 		return parse_datetimetz
 	elif data_type_str == "int":
 		return conv_int
 	elif data_type_str == "float":
 		return conv_float
 	elif data_type_str == "boolean":
@@ -645,28 +658,38 @@
 			if 'int' in uq_types and 'float' in uq_types:
 				return 'float'
 			else:
 				return "string"
 		else:
 			return "string"
 
-def set_data_types(headers, rows, data_type_list):
-	return_queue = queue.Queue()
-	def eval_columns(headers, rows, return_queue):
-		coltypes = []
-		for i, colname in enumerate(headers):
-			datavals = [row[i] for row in rows]
-			non_null = [d for d in datavals if d is not None and not (type(d) is str and d.strip() == '')]
-			nullcount = len(datavals) - len(non_null)
-			uniquevals = len(set(non_null))
-			coltypes.append((colname, common_data_type(datavals), nullcount, uniquevals))
-		return_queue.put(coltypes)
-	t = threading.Thread(target=eval_columns, args=(headers, rows, return_queue))
-	t.start()
-	return (t, return_queue)
+#def set_data_types(headers, rows):
+#	return_queue = queue.Queue()
+#	def eval_columns(headers, rows, return_queue):
+#		coltypes = []
+#		for i, colname in enumerate(headers):
+#			datavals = [row[i] for row in rows]
+#			non_null = [d for d in datavals if d is not None and not (type(d) is str and d.strip() == '')]
+#			nullcount = len(datavals) - len(non_null)
+#			uniquevals = len(set(non_null))
+#			coltypes.append((colname, common_data_type(datavals), nullcount, uniquevals))
+#		return_queue.put(coltypes)
+#	t = threading.Thread(target=eval_columns, args=(headers, rows, return_queue))
+#	t.start()
+#	return (t, return_queue)
+
+def set_data_types(headers, rows):
+	coltypes = []
+	for i, colname in enumerate(headers):
+		datavals = [row[i] for row in rows]
+		non_null = [d for d in datavals if d is not None and not (type(d) is str and d.strip() == '')]
+		nullcount = len(datavals) - len(non_null)
+		uniquevals = len(set(non_null))
+		coltypes.append((colname, common_data_type(datavals), nullcount, uniquevals))
+	return coltypes
 
 # Translations to SQLite type affinity names
 sqlite_type_x = {'int': 'INTEGER', 'float': 'REAL', 'string': 'TEXT', 'timestamptz': 'TEXT',
 		'timestamp': 'TEXT', 'date': 'TEXT', 'boolean': 'INTEGER'}
 
 def center_window(win):
 	win.update_idletasks()
@@ -687,58 +710,72 @@
 
 
 class MapUI(object):
 	def __init__(self, src_name, message, lat_col, lon_col, crs=4326, sheet=None,
 			label_col=None, symbol_col=None, color_col=None,
 			map_export_file=None, export_time_sec=10):
 		self.win = tk.Tk()
+		self.win.withdraw()
+		self.loading_dlg = LoadingDialog(self.win)
 		if src_name is None:
-			self.win._root().withdraw()
 			sdsd = SelDataSrcDialog()
 			src_name, label_col, lat_col, lon_col, crs, symbol_col, color_col, message, headers, rows = sdsd.select()
 			if src_name is None:
 				self.cancel()
-			self.win._root().deiconify()
 		else:
 			# src_name is a filename, either CSV or spreadsheet
+			self.loading_dlg.display("Loading data")
 			fn, ext = os.path.splitext(src_name)
 			if ext.lower() == ".csv":
 				try:
 					headers, rows = file_data(src_name, 0)
 				except:
-					self.win._root().withdraw()
 					fatal_error("Could not read data from %s" % src_data, kwargs={'parent': self.win})
 			else:
 				if sheet is None:
-					self.win._root().withdraw()
 					fatal_error("A sheet name must be specified for spreadsheets", kwargs={'parent': self.win})
 				try:
 					if ext.lower() == '.ods':
 						headers, rows = ods_data(src_name, sheet, 0)
 					else:
 						headers, rows = xls_data(src_name, sheet, 0)
 				except:
-					self.win._root().withdraw()
 					fatal_error("Could not read table from %s, sheet %s" % (src_name, sheet), kwargs={'parent': self.win})
+			self.loading_dlg.hide()
+		self.win.deiconify()
+
+
+		# Size and position window.
+		self.win.geometry("1200x1000")
+		self.win.update_idletasks()
+		m = re.match(r"(\d+)x(\d+)\+(-?\d+)\+(-?\d+)", self.win.geometry())
+		if m is not None:
+			wwd = int(m.group(1))
+			wht = int(m.group(2))
+			swd = self.win.winfo_screenwidth()
+			sht = self.win.winfo_screenheight()
+			xpos = (swd/2) - (wwd/2)
+			ypos = (sht/2) - (wht/2)
+			self.win.geometry("%dx%d+%d+%d" % (wwd, wht, xpos, ypos))
+
+		self.loading_dlg.display("Preparing map")
+
 		self.win.protocol("WM_DELETE_WINDOW", self.cancel)
 		self.data_src_name = src_name
 		self.win.title("Map of %s" % src_name)
 		# Patch ImageTk.PhotoImage.__del__ 
 		ImageTk.PhotoImage.__del__ = new_img_del
 		# Set the font
 		self.mapfont = self.makefont()
 		# Set the application window icon
 		#win_icon = tk.BitmapImage(data=win_icon_xbm, foreground="black", background="tan")
 		#self.win.iconbitmap(win_icon)
 		# Source and possibly un-projected crs
 		self.src_crs = crs
 		self.crs = crs
-		# Created column names for un-projected coordinates
-		self.lat_4326_col = None
-		self.lon_4326_col = None
 		# The markers for all the locations in the data table
 		self.loc_map_markers = []
 		# The markers for the selected location(s)
 		self.sel_map_markers = []
 		# The number of table rows without coordinates
 		self.missing_latlon = 0
 		# Map bounds
@@ -845,34 +882,23 @@
 		self.set_tbl_selectmode()
 		self.set_status()
 		# Add menu
 		self.add_menu(table_object = self.tbl, column_headers=headers)
 		self.tbl.bind('<ButtonRelease-1>', self.mark_map)
 		# Other key bindings
 		self.win.protocol("WM_DELETE_WINDOW", self.cancel)
-		# Size and position window.
-		self.win.geometry("1200x1000")
-		self.win.update_idletasks()
-		m = re.match(r"(\d+)x(\d+)\+(-?\d+)\+(-?\d+)", self.win.geometry())
-		if m is not None:
-			wwd = int(m.group(1))
-			wht = int(m.group(2))
-			swd = self.win.winfo_screenwidth()
-			sht = self.win.winfo_screenheight()
-			xpos = (swd/2) - (wwd/2)
-			ypos = (sht/2) - (wht/2)
-			self.win.geometry("%dx%d+%d+%d" % (wwd, wht, xpos, ypos))
 		# Limit resizing
 		self.win.minsize(width=860, height=640)
 		# Set table status message
 		self.set_status()
 		# Just export the map and quit?
 		if map_export_file is not None:
 			self.imageoutputfile = map_export_file
 			self.win.after(export_time_sec * 1000, self.export_map_and_quit)
+		self.loading_dlg.hide()
 	def makefont(self):
 		global label_font, label_size, label_bold
 		fams = tkfont.families()
 		if not label_font in fams:
 			alt_fonts = ["Liberation Sans", "Arial", "Helvetica", "Nimbus Sans", "Liberation Sans", "Trebuchet MS", "Tahoma", "DejaVu Sans", "Bitstream Vera Sans", "Open Sans"]
 			font_found = False
 			for f in alt_fonts:
@@ -951,20 +977,23 @@
 	def set_get_loc_marker(self):
 		mkr_key = "%s %s" % (location_color, location_marker)
 		if mkr_key not in custom_icons:
 			custom_icons[mkr_key] = tk.BitmapImage(data=icon_xbm[location_marker], foreground=location_color)
 		return custom_icons[mkr_key]
 	def redraw_loc_markers(self, tdata):
 		# tdata is the treeview control containing the data table.
+		self.loading_dlg.display("Redrawing markers")
 		while len(self.loc_map_markers) > 0:
 			self.loc_map_markers.pop().delete()
 		self.draw_loc_markers(tdata)
+		self.loading_dlg.hide()
 	def draw_loc_markers(self, tdata):
 		# tdata is the treeview control containing the data table.
 		# Also set the number of rows missing coordinates and the bounding box.
+		self.loading_dlg.display("Preparing map")
 		self.missing_latlon = 0
 		for row_id in tdata.get_children():
 			rowdata = tdata.item(row_id)["values"]
 			try:
 				lat_val = float(rowdata[self.lat_index])
 			except:
 				lat_val = None
@@ -1008,32 +1037,36 @@
 					self.loc_map_markers.append(mkr)
 				else:
 					mkr = self.map_widget.set_marker(lat_val, lon_val, icon=marker_icon, command=self.map_sel_table)
 					self.loc_map_markers.append(mkr)
 			else:
 				self.missing_latlon += 1
 		self.update_plot_data()
+		self.loading_dlg.hide()
 	def add_data(self, rows, headers, lat_col, lon_col, label_col, symbol_col, color_col):
 		# Re-set all data-specific variables and widgets
 		self.headers = headers
 		self.rows = rows
 		self.lat_col = lat_col
 		self.lon_col = lon_col
 		self.src_lat_col = lat_col
 		self.src_lon_col = lon_col
+		self.lat_4326_col = None
+		self.lon_4326_col = None
 		self.label_col = label_col
 		self.symbol_col = symbol_col
 		self.color_col = color_col
 		self.lat_index = headers.index(lat_col)
 		self.lon_index = headers.index(lon_col)
 		self.src_lat_index = headers.index(lat_col)
 		self.src_lon_index = headers.index(lon_col)
 		self.label_index = headers.index(label_col) if label_col is not None and label_col != '' else None
 		self.symbol_index = headers.index(symbol_col) if symbol_col is not None and symbol_col != '' else None
 		self.color_index = headers.index(color_col) if color_col is not None and color_col != '' else None
+
 		if self.crs != 4326:
 			try:
 				from pyproj import CRS, Transformer
 			except:
 				fatal_error("The pyproj library is required to re-project spatial coordinates")
 			try:
 				crs_proj = CRS(self.crs)
@@ -1071,16 +1104,17 @@
 					newy = None
 				if len(r) < len(headers):
 					r.extend([newy, newx])
 				else:
 					r[self.lat_index] = newy
 					r[self.lon_index] = newx
 		# Launch separate process to determine data types
+		import timeit
 		self.data_types = []
-		(dt_thread, dt_queue) = set_data_types(headers, rows, self.data_types)
+
 		# Populate the treeview
 		tframe, tdata = treeview_table(self.tblframe, rows, headers, "browse")
 		self.table_row_count = len(tdata.get_children())
 		# Scan the table, put points on the map, and find the map extent.
 		self.min_lat = self.max_lat = self.min_lon = self.max_lon = None
 		self.sel_map_markers = []
 		self.missing_latlon = 0
@@ -1104,24 +1138,26 @@
 		cur = self.db.cursor()
 		colnames = db_colnames(headers)
 		colnames.append("treeviewid")
 		cur.execute("create table mapdata (%s);" % ",".join(colnames))
 		tbldata = []
 		for row_id in tdata.get_children():
 			row_vals = tdata.item(row_id)["values"]
+			row_vals = [None if isinstance(x, str) and x.strip() == '' else x for x in row_vals]
 			row_vals.append(row_id)
 			tbldata.append(row_vals)
 		params = ",".join(['?'] * len(colnames))
 		cur.executemany("insert into mapdata values (%s)" % params, tbldata)
 		cur.close()
 		# Initial value for user-entered WHERE clause
 		self.whereclause = ""
+
 		# Save data types for use in column selection for plotting
-		dt_thread.join()
-		self.data_types = dt_queue.get(block=True)
+		self.data_types = set_data_types(headers, rows)
+
 		# Return frame and data table
 		return tframe, tdata
 	def remove_data(self):
 		while len(self.sel_map_markers) > 0:
 			self.sel_map_markers.pop().delete()
 		while len(self.loc_map_markers) > 0:
 			self.loc_map_markers.pop().delete()
@@ -1559,15 +1595,15 @@
 					global multiselect
 					multiselect = "1"
 					self.multiselect_var.set("1")
 					self.tbl.configure(selectmode = tk.EXTENDED)
 					if action == "Replace":
 						# Remove any existing selections
 						self.unselect_map()
-						self.tbl.selection_set(tuple(id_list))
+						self.tbl.selection_set(list(id_list))
 					elif action == "Add":
 						# Add new selections
 						all_selections = tuple(set(self.tbl.selection()) | set(id_list))
 						self.tbl.selection_set(all_selections)
 					else:
 						# Remove
 						diff_selections = tuple(set(self.tbl.selection()) - set(id_list))
@@ -1638,14 +1674,60 @@
 		plot_menu.add_command(label="Close all", command = self.close_all_plots, underline=0)
 		help_menu.add_command(label="Online help", command = online_help, underline=7)
 		help_menu.add_command(label="Config files", command = show_config_files, underline=0)
 		help_menu.add_command(label="About", command = show_about, underline=0)
 
 
 
+class LoadingDialog(object):
+	def __init__(self, parent):
+		self.parent = parent
+		self.dlg = tk.Toplevel(parent)
+		self.dlg.title("MapData")
+		#self.dlg.geometry("150x50")
+		center_window(self.dlg)
+		self.dlg.update_idletasks()
+		self.dlg.withdraw()
+		self.dlg.wm_overrideredirect(True)
+		self.dlg.configure(bg="Gold")
+		self.messages = []
+		self.var_lbl = tk.StringVar(self.dlg, "")
+		self.lbl_loading = tk.Label(self.dlg, bg="Gold", textvariable=self.var_lbl)
+		self.lbl_loading.place(relx=0.5, rely=0.5, anchor="center")
+		self.dlg.update()
+		self.dots = 3
+	def update_lbl(self):
+		if len(self.messages) > 0:
+			self.dots = self.dots % 3 + 1
+			lbl = self.messages[0] + '.' * self.dots
+			self.var_lbl.set(lbl)
+			self.dlg.update()
+			self.after_id = self.dlg.after(250, self.update_lbl)
+	def display(self, message):
+		self.messages.append(message)
+		self.var_lbl.set(message)
+		self.dlg.deiconify()
+		raise_window(self.dlg)
+		self.dlg.update()
+		self.dlg.focus_force()
+		#self.after_id = self.dlg.after(250, self.update_lbl)
+	def hide(self):
+		self.var_lbl.set("")
+		#self.dlg.after_cancel(self.after_id)
+		do_withdraw = True
+		if len(self.messages) > 0:
+			self.messages.pop(-1)
+			if len(self.messages) > 0:
+				self.var_lbl.set(self.messages[0])
+				do_withdraw = False
+		if do_withdraw:
+			self.dlg.withdraw()
+
+
+
 class LabelDialog(object):
 	def __init__(self, parent, column_list, label_col):
 		columns = ['']
 		columns.extend(column_list)
 		label_col = '' if label_col is None else label_col
 		self.dlg = tk.Toplevel()
 		self.dlg.title("Change Labeling")
@@ -2387,15 +2469,15 @@
 		query_frame.columnconfigure(0, weight=1)
 		query_frame.columnconfigure(1, weight=1)
 		sql_frame = tk.Frame(query_frame)
 		sql_frame.grid(row=0, column=0, sticky=tk.NSEW, padx=(3,3), pady=(3,3))
 		sql_frame.rowconfigure(0, weight=1)
 		sql_frame.columnconfigure(0, weight=1)
 		col_frame = tk.Frame(query_frame)
-		col_frame.grid(row=0, column=1, sticky=tk.NS, padx=(3,3), pady=(3,3))
+		col_frame.grid(row=0, column=1, rowspan=2, sticky=tk.NS, padx=(3,3), pady=(3,3))
 		col_frame.rowconfigure(0, weight=1)
 		act_frame = tk.Frame(query_frame)
 		act_frame.grid(row=1, column=0, sticky=tk.EW, padx=(3,3), pady=(3,3))
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.grid(row=2, column=0, sticky=tk.EW, pady=(3,3))
 		btn_frame.columnconfigure(0, weight=1)
 		# Prompt
```

### Comparing `mapdata-2.6.3/mapdata.egg-info/PKG-INFO` & `mapdata-2.6.6/mapdata.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.6.3
-Summary: An interactive map and table explorer for geographic coordinates in a CSV file
+Version: 2.6.6
+Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -35,15 +35,14 @@
 
 *mapdata.py* is a viewer for geographic coordinate data read from a CSV file, spreadsheet,
 or database.  Both a map and a data
 table are displayed.  When a location is selected on the map, the same location is highlighted in the
 table, and *vice-versa*.  Single or multiple selections may be enabled.  Locations may also
 be selected and highlighted by writing a query expression to select rows of the data table.
 
-![MapData illustration](https://mapdata.osdn.io/_images/mapdata_ui.png){width=50%}
 
 Coordinates should be in decimal degrees, in WGS84 (coordinate reference system [CRS] 4326), however,
 coordinates in other CRSs can be converted to 4326.
 
 The map display can be customized in several ways:
 
   * Different raster tile servers may be used for the basemap.  The default is
```

### Comparing `mapdata-2.6.3/setup.py` & `mapdata-2.6.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.6.3',
-	description="An interactive map and table explorer for geographic coordinates in a CSV file",
+	version='2.6.6',
+	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
 	python_requires = '>=3.8',
```

