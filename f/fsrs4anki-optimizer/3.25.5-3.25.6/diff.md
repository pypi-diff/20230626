# Comparing `tmp/fsrs4anki_optimizer-3.25.5.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.5.tar", last modified: Thu Jun 22 07:08:36 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.6.tar", last modified: Mon Jun 26 09:54:05 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.5.tar` & `fsrs4anki_optimizer-3.25.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44545 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44569 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 09:54:04.000000 fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 09:54:05.000004 fsrs4anki_optimizer-3.25.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 09:53:52.000000 fsrs4anki_optimizer-3.25.6/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.6/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
         df.drop(df[df['review_date'].dt.year < 2006].index, inplace=True)
         df.sort_values(by=['cid', 'id'], inplace=True, ignore_index=True)
         self.type_sequence = np.array(df['type'])
         self.time_sequence = np.array(df['time'])
         df.to_csv("revlog.csv", index=False)
         print("revlog.csv saved.")
 
-        df = df[df['type'] != 3].copy()
+        df = df[(df['type'] != 3) | (df['factor'] != 0)].copy()
         df['real_days'] = df['review_date'] - timedelta(hours=int(next_day_starts_at))
         df['real_days'] = pd.DatetimeIndex(df['real_days'].dt.floor('D', ambiguous='infer', nonexistent='shift_forward')).to_julian_date()
         df.drop_duplicates(['cid', 'real_days'], keep='first', inplace=True)
         df['delta_t'] = df.real_days.diff()
         df.dropna(inplace=True)
         df['i'] = df.groupby('cid').cumcount() + 1
         df.loc[df['i'] == 1, 'delta_t'] = 0
```

