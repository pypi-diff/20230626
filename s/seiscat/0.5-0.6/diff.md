# Comparing `tmp/seiscat-0.5.tar.gz` & `tmp/seiscat-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seiscat-0.5.tar", last modified: Thu Jun 22 15:36:04 2023, max compression
+gzip compressed data, was "seiscat-0.6.tar", last modified: Mon Jun 26 08:42:21 2023, max compression
```

## Comparing `seiscat-0.5.tar` & `seiscat-0.6.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-22 15:35:56.000000 seiscat-0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 15:35:56.000000 seiscat-0.5/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 15:35:56.000000 seiscat-0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 15:35:56.000000 seiscat-0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-22 15:36:04.985955 seiscat-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-22 15:35:56.000000 seiscat-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.989955 seiscat-0.5/seiscat/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-22 15:36:04.989955 seiscat-0.5/seiscat/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/seiscat/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/conf/configspec.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/seiscat/configobj/
--rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/configobj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/configobj/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/configobj/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9117 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/fdsnws.py
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/seiscat/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/scripts/seiscat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-22 15:35:56.000000 seiscat-0.5/seiscat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:36:04.985955 seiscat-0.5/seiscat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 15:36:04.000000 seiscat-0.5/seiscat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-22 15:36:04.985955 seiscat-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-22 15:35:56.000000 seiscat-0.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-22 15:35:56.000000 seiscat-0.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:42:21.119385 seiscat-0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-26 08:42:11.000000 seiscat-0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 08:42:11.000000 seiscat-0.6/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-26 08:42:11.000000 seiscat-0.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-26 08:42:11.000000 seiscat-0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-26 08:42:21.119385 seiscat-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-06-26 08:42:11.000000 seiscat-0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:42:21.119385 seiscat-0.6/seiscat/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-26 08:42:21.119385 seiscat-0.6/seiscat/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:42:21.119385 seiscat-0.6/seiscat/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/conf/configspec.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:42:21.119385 seiscat-0.6/seiscat/configobj/
+-rw-r--r--   0 runner    (1001) docker     (123)    88030 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/configobj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/configobj/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/configobj/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/download_and_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/editdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/fdsnws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/parse_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:42:21.119385 seiscat-0.6/seiscat/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/scripts/seiscat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-26 08:42:11.000000 seiscat-0.6/seiscat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:42:21.119385 seiscat-0.6/seiscat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-26 08:42:21.000000 seiscat-0.6/seiscat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-26 08:42:21.000000 seiscat-0.6/seiscat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:42:21.000000 seiscat-0.6/seiscat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 08:42:21.000000 seiscat-0.6/seiscat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-26 08:42:21.000000 seiscat-0.6/seiscat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 08:42:21.000000 seiscat-0.6/seiscat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-26 08:42:21.119385 seiscat-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-26 08:42:11.000000 seiscat-0.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-26 08:42:11.000000 seiscat-0.6/versioneer.py
```

### Comparing `seiscat-0.5/LICENSE.txt` & `seiscat-0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seiscat-0.5/PKG-INFO` & `seiscat-0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.5
+Version: 0.6
 Summary: Keep a local seismic catalog
 Home-page: https://seiscat.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://seiscat.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/seiscat
@@ -69,14 +69,18 @@
 To keep the database updated, run on a regular basis:
 
     seiscat updatedb
 
 (This will use the configuration parameter `recheck_period` to recheck the
 last *n* days or hours).
 
+You can edit the attributes of specific events in the database using:
+
+    seiscat editdb
+
 You can print the catalog to screen:
 
     seiscat print
 
 Or plot it:
 
     seiscat plot
@@ -84,16 +88,21 @@
 Each of the above commands can have its own options.
 As an example, to discover the options for the `plot` command, try:
 
     seiscat plot -h
 
 SeisCat supports command line tab completion for arguments, thanks to
 [argcomplete](https://kislyuk.github.io/argcomplete/).
-To enable command line tab completion, add the following line to your `.bashrc`
-or `.zshrc`:
+To enable command line tab completion run:
+
+    activate-global-python-argcomplete
+
+(This is a one-time command that needs to be run only once).
+
+Or, alternatively, add the following line to your `.bashrc` or `.zshrc`:
 
     eval "$(register-python-argcomplete seiscat)"
 
 ## Installation
 
 ### Installing the latest release
```

### Comparing `seiscat-0.5/README.md` & `seiscat-0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 To keep the database updated, run on a regular basis:
 
     seiscat updatedb
 
 (This will use the configuration parameter `recheck_period` to recheck the
 last *n* days or hours).
 
+You can edit the attributes of specific events in the database using:
+
+    seiscat editdb
+
 You can print the catalog to screen:
 
     seiscat print
 
 Or plot it:
 
     seiscat plot
@@ -55,16 +59,21 @@
 Each of the above commands can have its own options.
 As an example, to discover the options for the `plot` command, try:
 
     seiscat plot -h
 
 SeisCat supports command line tab completion for arguments, thanks to
 [argcomplete](https://kislyuk.github.io/argcomplete/).
-To enable command line tab completion, add the following line to your `.bashrc`
-or `.zshrc`:
+To enable command line tab completion run:
+
+    activate-global-python-argcomplete
+
+(This is a one-time command that needs to be run only once).
+
+Or, alternatively, add the following line to your `.bashrc` or `.zshrc`:
 
     eval "$(register-python-argcomplete seiscat)"
 
 ## Installation
 
 ### Installing the latest release
```

### Comparing `seiscat-0.5/seiscat/conf/configspec.conf` & `seiscat-0.6/seiscat/conf/configspec.conf`

 * *Files identical despite different names*

### Comparing `seiscat-0.5/seiscat/configobj/__init__.py` & `seiscat-0.6/seiscat/configobj/__init__.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.5/seiscat/configobj/validate.py` & `seiscat-0.6/seiscat/configobj/validate.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.5/seiscat/db.py` & `seiscat-0.6/seiscat/db.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,14 +16,32 @@
 from .utils import err_exit
 
 # Current supported DB version
 # Increment this number when changing the DB schema
 DB_VERSION = 1
 
 
+def _get_db_connection(config, initdb=False):
+    """
+    Get database connection.
+
+    :param config: config object
+    :return: database connection
+    """
+    db_file = config.get('db_file', None)
+    if db_file is None:
+        err_exit('db_file not set in config file')
+    if not initdb:
+        try:
+            open(db_file, 'r')
+        except FileNotFoundError:
+            err_exit(f'Database file "{db_file}" not found.')
+    return sqlite3.connect(db_file)
+
+
 def _check_db_version(cursor, config):
     """
     Check if database version is compatible with current version.
 
     :param cursor: database cursor
     :param config: config object
     """
@@ -75,34 +93,56 @@
     if not initdb and not os.path.exists(db_file):
         err_exit(
             f'Database file "{db_file}" does not exist.\n'
             'Run "seiscat initdb" first.'
         )
 
 
-def _same_values(event1, event2):
+def _same_values(values1, values2, skip_begin=0, skip_end=0):
     """
-    Check if two events have the same values.
+    Check if two lists of values have the same values.
 
     :param event1: first event
     :param event2: second event
-    :returns: True if events have the same values, False otherwise
+    :param skip_begin: number of fields to skip at the beginning of values
+    :param skip_end: number of fields to skip at the end of values
+    :returns: True if the two lists have the same values, False otherwise
     """
-    for idx in range(2, len(event1)):
+    for idx in range(skip_begin, len(values1)-skip_end):
         try:
             # Use np.isclose() for numbers
-            match = np.isclose(event1[idx], event2[idx])
+            match = np.isclose(values1[idx], values2[idx])
         except TypeError:
             # Use == for strings
-            match = event1[idx] == event2[idx]
+            match = values1[idx] == values2[idx]
         if not match:
             return False
     return True
 
 
+def _event_exists(cursor, values, skip_begin=0, skip_end=0):
+    """
+    Check if an event exists in the database, based on values.
+
+    :param cursor: database cursor
+    :param values: list of values
+    :param skip_begin: number of fields to skip at the beginning of values
+    :param skip_end: number of fields to skip at the end of values
+    :returns: True if event exists, False otherwise
+    """
+    evid = values[0]
+    cursor.execute('SELECT * FROM events WHERE evid = ?', (evid,))
+    rows = cursor.fetchall()
+    rows_with_same_values = [
+        row for row in rows
+        if _same_values(values, row, skip_begin, skip_end)
+    ]
+    return len(rows_with_same_values) > 0
+
+
 def _get_evid(resource_id):
     """
     Get evid from resource_id.
 
     :param resource_id: resource_id string
     :returns: evid string
     """
@@ -119,33 +159,34 @@
 
 
 def _get_db_field_definitions(config):
     """
     Get a list of database fields.
 
     :param config: config object
-    :returns: list of fields
+    :returns: list of field definitions, number of extra fields
     """
-    fields = [
+    field_definitions = [
         'evid TEXT',
         'ver INTEGER',
         'time TEXT',
         'lat REAL',
         'lon REAL',
         'depth REAL',
         'mag REAL',
         'mag_type TEXT',
         'event_type TEXT',
     ]
     extra_field_names = config['extra_field_names'] or []
     extra_field_types = config['extra_field_types'] or []
-    fields.extend(
+    n_extra_fields = len(extra_field_names)
+    field_definitions.extend(
         f'{name} {dbtype}' for name, dbtype
         in zip(extra_field_names, extra_field_types))
-    return fields
+    return field_definitions, n_extra_fields
 
 
 def _get_db_values_from_event(ev, config):
     """
     Get a list of values from an obspy event object.
 
     :param ev: obspy event object
@@ -175,98 +216,180 @@
     """
     Write catalog to database.
 
     :param cat: obspy Catalog object
     :param config: config object
     :param initdb: if True, create new database file
     """
-    # open database connection
-    conn = sqlite3.connect(config['db_file'])
+    conn = _get_db_connection(config, initdb)
     c = conn.cursor()
     if initdb:
         _set_db_version(c)
     else:
         _check_db_version(c, config)
-    field_definitions = _get_db_field_definitions(config)
+    field_definitions, n_extra_fields = _get_db_field_definitions(config)
     # create table if it doesn't exist, use evid and ver as primary key
     c.execute(
         'CREATE TABLE IF NOT EXISTS events '
         f'({", ".join(field_definitions)}, PRIMARY KEY (evid, ver))')
     events_written = 0
     for ev in cat:
         values = _get_db_values_from_event(ev, config)
         if initdb or config['overwrite_updated_events']:
             # add events to table, replace events that already exist
             c.execute(
                 'INSERT OR REPLACE INTO events VALUES '
                 f'({", ".join("?" * len(values))})', values)
-        else:
-            # check if an event with the same values already exists
-            evid = values[0]
-            c.execute(
-                'SELECT * FROM events WHERE evid = ?', (evid,))
-            rows = c.fetchall()
-            rows_with_different_values = [
-                row for row in rows if not _same_values(values, row)]
-            try:
-                max_version = max(row[1] for row in rows_with_different_values)
-            except ValueError:
-                # rows_with_different_values is empty
-                max_version = 0
-            values[1] = max_version + 1
-            # add events to table, ignore events that have same evid and vers
-            # (i.e., the same primary keys)
-            c.execute(
-                'INSERT OR IGNORE INTO events VALUES '
-                f'({", ".join("?" * len(values))})', values)
-        events_written += c.rowcount
+            events_written += c.rowcount
+        elif not _event_exists(
+                c, values, skip_begin=2, skip_end=n_extra_fields):
+            while True:
+                try:
+                    c.execute(
+                        'INSERT INTO events VALUES '
+                        f'({", ".join("?" * len(values))})', values)
+                    events_written += c.rowcount
+                    break
+                except sqlite3.IntegrityError:
+                    # evid and ver already exist, increment ver
+                    values[1] += 1
     # close database connection
     conn.commit()
     print(f'Wrote {events_written} events to database "{config["db_file"]}"')
 
 
-def read_fields_and_rows_from_db(config):
+def read_fields_and_rows_from_db(config, eventid=None, version=None):
     """
     Read fields and rows from database. Return a list of fields and a list of
     rows.
 
     :param config: config object
+    :param eventid: limit to events with this evid
+    :param version: limit to events with this version
+                    (ignored if eventid is None)
     :returns: list of fields, list of rows
     """
-    db_file = config.get('db_file', None)
-    if db_file is None:
-        err_exit('db_file not set in config file')
-    try:
-        open(db_file, 'r')
-    except FileNotFoundError:
-        err_exit(f'Database file "{db_file}" not found.')
-    conn = sqlite3.connect(db_file)
+    conn = _get_db_connection(config)
     c = conn.cursor()
     # read field names
     c.execute('PRAGMA table_info(events)')
     # we just need the field names, which are in the second column
     fields = [f[1] for f in c.fetchall()]
     # read events
-    c.execute('SELECT * FROM events')
+    if eventid is not None and version is not None:
+        c.execute(
+            'SELECT * FROM events WHERE evid = ? AND ver = ?',
+            (eventid, version))
+    elif eventid is not None:
+        c.execute('SELECT * FROM events WHERE evid = ?', (eventid,))
+    else:
+        c.execute('SELECT * FROM events')
+    try:
+        allversions = config['args'].allversions
+    except AttributeError:
+        allversions = True
     rows = c.fetchall()
-    allversions = config['args'].allversions
     if not allversions:
         # keep only the latest version of each event
         evids = set()
         rows_to_keep = []
         for row in sorted(rows, key=lambda r: r[:2], reverse=True):
             evid = row[0]
             if evid not in evids:
                 rows_to_keep.append(row)
                 evids.add(evid)
         rows = rows_to_keep
     conn.close()
     return fields, rows
 
 
+def replicate_event_in_db(config, eventid, version=1):
+    """
+    Replicate an event in the database. The new event will have the same
+    evid as the original event, but a different version.
+
+    :param config: config object
+    :param eventid: event id of the original event
+    :param version: version of the original event
+    """
+    fields, rows = read_fields_and_rows_from_db(
+        config, eventid=eventid, version=version)
+    if not rows:
+        err_exit(f'Event {eventid} version {version} not found in database')
+    row = list(rows[0])
+    # increment version
+    ver_index = fields.index('ver')
+    row[ver_index] += 1
+    conn = _get_db_connection(config)
+    c = conn.cursor()
+    while True:
+        try:
+            c.execute(
+                'INSERT INTO events VALUES '
+                f'({", ".join("?" * len(row))})', row)
+            break
+        except sqlite3.IntegrityError:
+            # version already exists, increment version and try again
+            row[ver_index] += 1
+    # close database connection
+    conn.commit()
+    print(f'Added event {eventid} version {row[ver_index]} to database')
+
+
+def delete_event_from_db(config, eventid, version=None):
+    """
+    Delete an event from the database.
+
+    :param config: config object
+    :param eventid: event id of the event to delete
+    :param version: version of the event to delete
+                    (if None, delete all versions of the event)
+    """
+    conn = _get_db_connection(config)
+    c = conn.cursor()
+    if version is not None:
+        c.execute(
+            'DELETE FROM events WHERE evid = ? AND ver = ?',
+            (eventid, version))
+    else:
+        c.execute('DELETE FROM events WHERE evid = ?', (eventid,))
+    # close database connection
+    conn.commit()
+    if version is None:
+        msg = f'Event {eventid} deleted from database'
+    else:
+        msg = f'Event {eventid} version {version} deleted from database'
+    print(msg)
+
+
+def update_event_in_db(config, eventid, version, field, value):
+    """
+    Update an event in the database.
+
+    :param config: config object
+    :param eventid: event id of the event to update
+    :param version: version of the event to update
+    :param field: field to update
+    :param value: new value
+    """
+    conn = _get_db_connection(config)
+    c = conn.cursor()
+    try:
+        c.execute(
+            f'UPDATE events SET {field} = ? WHERE evid = ? AND ver = ?',
+            (value, eventid, version))
+    except sqlite3.OperationalError:
+        err_exit(f'Field "{field}" not found in database')
+    # close database connection
+    conn.commit()
+    print(
+        f'Updated field "{field}={value}" '
+        f'for event {eventid} version {version}')
+
+
 def read_events_from_db(config):
     """
     Read events from database. Return a list of events.
 
     :param config: config object
     :returns: list of events, each event is a dictionary
     """
```

### Comparing `seiscat-0.5/seiscat/fdsnws.py` & `seiscat-0.6/seiscat/fdsnws.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.5/seiscat/plot.py` & `seiscat-0.6/seiscat/plot.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.5/seiscat/print.py` & `seiscat-0.6/seiscat/print.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     Print catalog statistics.
 
     :param config: config object
     """
     print(get_catalog_stats(config))
 
 
-def print_catalog_table(config):
+def print_catalog_table(config, eventid=None, version=None):
     """
     Pretty-print the catalog as a table.
 
     :param config: config object
     """
-    fields, rows = read_fields_and_rows_from_db(config)
+    fields, rows = read_fields_and_rows_from_db(config, eventid, version)
     if len(rows) == 0:
         print('No events in catalog')
         return
     # get max length of each field
     max_len = [len(f) for f in fields]
     for row in rows:
         for i, val in enumerate(row):
@@ -55,13 +55,14 @@
 
 def print_catalog(config):
     """
     Print catalog.
 
     :param config: config object
     """
-    if config['args'].format == 'stats':
+    args = config['args']
+    if args.format == 'stats':
         print_catalog_stats(config)
-    elif config['args'].format == 'table':
-        print_catalog_table(config)
+    elif args.format == 'table':
+        print_catalog_table(config, eventid=args.eventid)
     else:
-        err_exit(f'Unknown format "{config["args"].format}"')
+        err_exit(f'Unknown format "{args.format}"')
```

### Comparing `seiscat-0.5/seiscat/utils.py` & `seiscat-0.6/seiscat/utils.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.5/seiscat.egg-info/PKG-INFO` & `seiscat-0.6/seiscat.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seiscat
-Version: 0.5
+Version: 0.6
 Summary: Keep a local seismic catalog
 Home-page: https://seiscat.seismicsource.org
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://seiscat.seismicsource.org
 Project-URL: Source, https://github.com/SeismicSource/seiscat
@@ -69,14 +69,18 @@
 To keep the database updated, run on a regular basis:
 
     seiscat updatedb
 
 (This will use the configuration parameter `recheck_period` to recheck the
 last *n* days or hours).
 
+You can edit the attributes of specific events in the database using:
+
+    seiscat editdb
+
 You can print the catalog to screen:
 
     seiscat print
 
 Or plot it:
 
     seiscat plot
@@ -84,16 +88,21 @@
 Each of the above commands can have its own options.
 As an example, to discover the options for the `plot` command, try:
 
     seiscat plot -h
 
 SeisCat supports command line tab completion for arguments, thanks to
 [argcomplete](https://kislyuk.github.io/argcomplete/).
-To enable command line tab completion, add the following line to your `.bashrc`
-or `.zshrc`:
+To enable command line tab completion run:
+
+    activate-global-python-argcomplete
+
+(This is a one-time command that needs to be run only once).
+
+Or, alternatively, add the following line to your `.bashrc` or `.zshrc`:
 
     eval "$(register-python-argcomplete seiscat)"
 
 ## Installation
 
 ### Installing the latest release
```

### Comparing `seiscat-0.5/seiscat.egg-info/SOURCES.txt` & `seiscat-0.6/seiscat.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 README.md
 setup.cfg
 setup.py
 versioneer.py
 seiscat/__init__.py
 seiscat/_version.py
 seiscat/db.py
+seiscat/download_and_store.py
+seiscat/editdb.py
 seiscat/fdsnws.py
+seiscat/parse_arguments.py
 seiscat/plot.py
 seiscat/print.py
 seiscat/utils.py
 seiscat.egg-info/PKG-INFO
 seiscat.egg-info/SOURCES.txt
 seiscat.egg-info/dependency_links.txt
 seiscat.egg-info/entry_points.txt
```

### Comparing `seiscat-0.5/setup.py` & `seiscat-0.6/setup.py`

 * *Files identical despite different names*

### Comparing `seiscat-0.5/versioneer.py` & `seiscat-0.6/versioneer.py`

 * *Files identical despite different names*

