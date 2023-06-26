# Comparing `tmp/sunspot-0.0.1.tar.gz` & `tmp/sunspot-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunspot-0.0.1.tar", last modified: Sun May 28 15:05:17 2023, max compression
+gzip compressed data, was "sunspot-0.6.tar", last modified: Mon Jun 26 12:10:47 2023, max compression
```

## Comparing `sunspot-0.0.1.tar` & `sunspot-0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-05-28 15:05:17.906365 sunspot-0.0.1/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      266 2023-05-28 15:05:17.906224 sunspot-0.0.1/PKG-INFO
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      367 2023-05-28 14:56:59.000000 sunspot-0.0.1/pyproject.toml
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       38 2023-05-28 15:05:17.906402 sunspot-0.0.1/setup.cfg
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-05-28 15:05:17.905578 sunspot-0.0.1/src/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      238 2023-05-03 00:20:45.000000 sunspot-0.0.1/src/foobar.py
-drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-05-28 15:05:17.906082 sunspot-0.0.1/src/sunspot.egg-info/
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      266 2023-05-28 15:05:17.000000 sunspot-0.0.1/src/sunspot.egg-info/PKG-INFO
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      195 2023-05-28 15:05:17.000000 sunspot-0.0.1/src/sunspot.egg-info/SOURCES.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)        1 2023-05-28 15:05:17.000000 sunspot-0.0.1/src/sunspot.egg-info/dependency_links.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       20 2023-05-28 15:05:17.000000 sunspot-0.0.1/src/sunspot.egg-info/top_level.txt
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    14867 2023-05-28 14:56:59.000000 sunspot-0.0.1/src/sunspot.py
--rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     8529 2023-05-28 14:56:59.000000 sunspot-0.0.1/src/test.py
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-26 12:10:47.769705 sunspot-0.6/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12028 2023-06-26 12:10:47.769430 sunspot-0.6/PKG-INFO
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    10997 2023-06-25 19:24:10.000000 sunspot-0.6/README.md
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     1104 2023-06-26 12:10:32.000000 sunspot-0.6/pyproject.toml
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       38 2023-06-26 12:10:47.769750 sunspot-0.6/setup.cfg
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-26 12:10:47.768523 sunspot-0.6/src/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      868 2023-06-22 01:07:07.000000 sunspot-0.6/src/foobar.py
+drwxr-xr-x   0 phillipcurtsmith   (501) staff       (20)        0 2023-06-26 12:10:47.769247 sunspot-0.6/src/sunspot.egg-info/
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    12028 2023-06-26 12:10:47.000000 sunspot-0.6/src/sunspot.egg-info/PKG-INFO
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)      205 2023-06-26 12:10:47.000000 sunspot-0.6/src/sunspot.egg-info/SOURCES.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)        1 2023-06-26 12:10:47.000000 sunspot-0.6/src/sunspot.egg-info/dependency_links.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)       20 2023-06-26 12:10:47.000000 sunspot-0.6/src/sunspot.egg-info/top_level.txt
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)    18189 2023-06-25 15:03:29.000000 sunspot-0.6/src/sunspot.py
+-rw-r--r--   0 phillipcurtsmith   (501) staff       (20)     8456 2023-06-25 00:40:27.000000 sunspot-0.6/src/test.py
```

### Comparing `sunspot-0.0.1/src/sunspot.py` & `sunspot-0.6/src/sunspot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
-Sunspot: Simple and light-weight ephemeris engine for automated telescope guidance and astronomical observation.
+Sunspot: Simple and light-weight JPL ephemeris parser and tracking engine for astronomy and telescope guidance. Provides simple lists of ephemeris data for any Target Body available through the JPL Horizons App. Also provides real-time tracking of those data for the duration of an ephemeris.
 
 Powered by NASA/JPL Horizons Ephemeris API, which is not affiliated with Sunspot.
 For NASA/JPL information, see: https://ssd.jpl.nasa.gov/horizons/manual.html#center
 
 __author__ = "Phillip Curtsmith"
 __copyright__ = "Copyright 2023, Phillip Curtsmith"
 
-__license__ = "MIT"
-__version__ = "1.0.1"
 __maintainer__ = "Phillip Curtsmith"
 __email__ = "phillip.curtsmith@gmail.com"
 """
 
 DATA_FORMAT = "%Y-%m-%d %H:%M:%S"
 DEFAULT_EPHEMERIS_QUANTITIES = '1,2,4'
 SOLAR_AND_LUNAR_PRESENCE_SYMBOLS = [ 'C', 'm', 'N', 'A', '*', '' ]
@@ -24,14 +22,15 @@
     def __init__( self, start_time: str, stop_time: str, observer_location: str, step_size: str, target_body: str, quantities: str = DEFAULT_EPHEMERIS_QUANTITIES ):
         """
         :param start_time: 'YYYY-MM-DD HH:MM:SS'
         :param stop_time: 'YYYY-MM-DD HH:MM:SS'
         :param observer_location: '00,00,00' as 'latitude [fractional degrees], longitude [fractional degrees], elevation [kilometers]'
         :param step_size: 'n t', where 1 <= n <= 90024 (the maximum number of entries) and t is a unit of time, e.g., 'minute', 'hour', 'day', 'month', 'year'
         :param target_body: observable target from JPL index, here: https://ssd.jpl.nasa.gov/horizons/app.html#/
+        :param quantities: observer quantities from JPL index, here: https://ssd.jpl.nasa.gov/horizons/app.html#/ . Default includes right ascension, declination, and altitude/azimuth
         """
         self.RAW_DATA = get_jpl_ephemeris( start_time, stop_time, observer_location, step_size, target_body, quantities )
         self.DATA_ENTRIES_RAW, self.DATA_ENTRIES, self.DATA_TITLES = self.clean_ephemeris_data()
         self.PARSED_DATA = self.parse_ephemeris_data()
 
     def clean_ephemeris_data( self ) -> list:
         """
@@ -45,26 +44,38 @@
         return data_entries_raw, data_entries, data_titles
 
     def parse_ephemeris_data( self ) -> dict:
         """
         :return: A dictionary of ephemeris data, where keys are data column titles and each value is a list of data corresponding to that title. Entries in each list are in chronological order.
         """
         from collections import defaultdict
+        from datetime import datetime
         ephemeris = defaultdict( list )
         for row in self.DATA_ENTRIES:
             row_items = row.split( ',' )
             row_items = [ i.strip(' ') for i in row_items ]
             row_items = [ i for i in row_items if i not in SOLAR_AND_LUNAR_PRESENCE_SYMBOLS ]
             for column in range( len(self.DATA_TITLES) ):
                 ephemeris[ self.DATA_TITLES[column] ].append( row_items[column] )
+        # Scrub dates to include numeric months rather than strings, e.g., 'Feb' becomes '02'
+        dates = ephemeris.get( self.DATA_TITLES[0] )
+        for k, entry in enumerate( dates ):
+            dates[k] = convert_numeric_month( entry )
+        # JPL omits 'seconds' unit completely if user enters HH:MM:SS where SS=00. If present, fix.
+        try:
+            datetime.strptime( dates[0], DATA_FORMAT )
+        except ValueError:
+            zeros = ":00"
+            for k, entry in enumerate( dates ):
+                dates[k] = entry + zeros
         return ephemeris
 
     def get_ephemeris_data( self, column_title: str ) -> list:
         """
-        :param column_title: String title corresponding to a column of ephemeris data, e.g., "Date__(UT)__HR:MN:SS"
+        :param column_title: String title corresponding to a column of ephemeris data, e.g., "Date__(UT)__HR:MN:SS" or Ephemeris.DATA_TITLES[n] where n is a valid index.
         :return: A list of data corresponding to an ephemeris data column title. Entries in this list are in chronological order.
         """
         if not self.DATA_TITLES.__contains__( column_title ):
             raise SystemError( "'" + column_title + "'" + " is not a valid ephemeris data column title." )
         return self.PARSED_DATA.get( column_title )
 
     def dates( self ) -> list:
@@ -91,67 +102,132 @@
         for i in range( len(target_data) ):
             if source_data[i] == source_data_point:
                 h.append( target_data[i] )
         return h
 
 
 class Tracker:
-    # High level internal summary.
-    # A user can spawn any number of Tracker objects, where a Tracker can track any number of Ephemeris data types.
-    # User can specify a start_time. If left None, start time is the start time for Ephemeris.
-    # User MUST specify a client-side user_method
-    # TODO concurrency, async, or schedule at fixed rate?
-    # TODO start time is now or some specific future time?
-    # TODO add a feature where the method is called in lead-up to that time, or exactly at that time. Lead-up mode is useful for telescope move operations, where the telescope should be in position already for subsequent method calls.
-
-
-    def __init__( self, e: Ephemeris, data_titles, user_method, start_time=None ):
-        self.tracked_data = data_titles
-        self.t = None
-        if not type( data_titles ) is list:
-            raise SystemError( "'data_titles' argument must be a list of strings, where each entry is a column of ephemeris data. If you wish to track only a single data title, 'data_titles' should be a list of length 1." )
-        for i in data_titles:
-            if i not in e.DATA_TITLES:
-                raise SystemError( "Entries in 'data_titles' must be members of Epehmeris.DATA_TITLES." )
-        if start_time is None:
-            starting_index = self.next_event_index( e )
-        else:
-            starting_index = self.known_event_index( e )
+
+    def __init__( self, e: Ephemeris,
+                  track_before_method: callable( list ) = None,
+                  track_on_time_method: callable( list ) = None,
+                  track_after_method: callable( list ) = None,
+                  verbose: bool = False ):
+        """
+        Create Tracker object. Tracking begins automatically upon object creation. Tracker objects will automatically track beginning with the next-soonest date. If no next-soonest date, e.g., all dates are in past, SystemError results.
+        :param e: Ephemeris object.
+        :param track_before_method: User-defined method. Must accept list of strings corresponding to Ephemeris _Observer Quantities_. Optional argument.
+        :param track_on_time_method: User-defined method. Must accept list of strings corresponding to Ephemeris _Observer Quantities_. Optional argument.
+        :param track_after_method: User-defined method. Must accept list of strings corresponding to Ephemeris _Observer Quantities_. Optional argument.
+        :param verbose: If True, prints method execution time stamps to terminal.
+        """
+        self.verbose = verbose
+        self.ephemeris = e
+        starting_index = self.next_event_index( e )
         if starting_index is None:
-            raise SystemError( "Tracker initiated for past event. Tracker can only track current event." )
+            raise SystemError( "All Ephemeris entries are in the past! One cannot track past events." )
+        if self.verbose:
+            print( "First scheduled tracking event: [" + e.dates()[starting_index] + "]" )
+
+        # Start tracking thread
         import threading
-        # TODO how to update method args (3rd parameter) for each call to timer?
-        # TODO how to force this to trigger at the correct start time?
-        # TODO Does this trigger at _interval_ since last trigger, or _interval_ since user_method completes?
-        self.t = threading.Timer( 30.0, user_method, [] )
+        import signal
+        self.exit_event_trigger = threading.Event()
+        signal.signal( signal.SIGINT, self.terminate_tracking )
+        self.c = threading.Thread( target = self.track, args = [ track_before_method,
+                                                                 track_on_time_method,
+                                                                 track_after_method,
+                                                                 starting_index ] )
+        self.c.start()
+
+    def terminate_tracking( self ) -> None:
+        """
+        Terminate tracking for a current Tracker object.
+        :return: None
+        """
+        self.exit_event_trigger.set()
+
+    def user_cancelled_tracking( self ) -> bool:
+        if not self.exit_event_trigger:
+            if self.verbose:
+                print( "SUNSPOT#TRACKER: Tracking cancelled by user." )
+            return True
+        return False
 
-    def known_event_index( self, e: Ephemeris ):
-        pass
+    def track( self, before_method, on_time_method, after_method, starting_index ):
+        from datetime import datetime
+        count = starting_index
+        dates = self.ephemeris.dates()
+        for i in range( starting_index, len( dates ) ):
+            method_arguments = self.collate_arguments( count )
+            #
+            # CALL BEFORE_METHOD
+            #
+            if self.user_cancelled_tracking():
+                break
+            if before_method is not None:
+                if self.verbose:
+                    print( "SUNSPOT#TRACKER#CALL-BEFORE: Scheduled event [" + dates[count] + "] executed at [" + f'{datetime.now():%Y-%m-%d %H:%M:%S%z}' + "]." )
+                before_method( method_arguments )
+            #
+            # DELAY
+            #
+            if self.exit_event_trigger.wait( timeout = sleep_time( dates[count] ) ):
+                if self.verbose:
+                    print( "SUNSPOT#TRACKER: Tracking cancelled by user." )
+                break
+            #
+            # CALL ON_TIME_METHOD
+            #
+            if self.user_cancelled_tracking():
+                break
+            if on_time_method is not None:
+                if self.verbose:
+                    print( "SUNSPOT#TRACKER#CALL-ON-TIME: Scheduled event [" + dates[count] + "] executed at [" + f'{datetime.now():%Y-%m-%d %H:%M:%S%z}' + "]." )
+                on_time_method( method_arguments )
+            #
+            # CALL AFTER_METHOD
+            #
+            if self.user_cancelled_tracking():
+                break
+            if after_method is not None:
+                if self.verbose:
+                    print( "SUNSPOT#TRACKER#CALL-AFTER: Scheduled event [" + dates[count] + "] executed at [" + f'{datetime.now():%Y-%m-%d %H:%M:%S%z}' + "]." )
+                after_method( method_arguments )
+            #
+            count = count + 1
+        if not self.exit_event_trigger.is_set():
+            if self.verbose:
+                print( "SUNSPOT#TRACKER: Ephemeris tracking completed normally at [" + f'{datetime.now():%Y-%m-%d %H:%M:%S%z}' + "]." )
+
+    def collate_arguments( self, count ) -> list:
+        args = []
+        for i in self.ephemeris.DATA_TITLES:
+            args.append( self.ephemeris.get_ephemeris_data(i)[ count ] )
+        return args
 
     def next_event_index( self, e: Ephemeris ):
         from datetime import datetime
-        dates = e.PARSED_DATA.get( e.DATA_TITLES[0] )
-        for i in range( 0, len( dates ) - 2 ):
-            if datetime.now().timestamp() < datetime.strptime( dates[i], DATA_FORMAT ).timestamp() and datetime.now().timestamp() >= datetime.strptime( dates[i+1], DATA_FORMAT ).timestamp():
-                return i
+        dates = e.dates()
+        for i in dates:
+            if datetime.now().timestamp() < datetime.strptime( i, DATA_FORMAT ).timestamp():
+                return dates.index( i )
         return None
 
-    def terminate_tracking( self, terminated_data=None ):
-        '''
-        Data_title is a list of str corresponding to the data objects which will no longer be tracked. If None, cancel all tracking activity
-        If data_title is a subset of tracked_data, cancel tracking only for those items.
-        :param terminated_data:
-        :return:
-        '''
-        if not type( terminated_data ) is list:
-            raise SystemError( "'data_title' argument must be a list of strings, where each entry is a column of ephemeris data." )
-        if terminated_data is None or terminated_data is self.tracked_data:
-            self.t.cancel()
-            return
-        self.tracked_data = [ x for x in self.tracked_data if x not in terminated_data ]
+
+def sleep_time( future ) -> float:
+    """
+    :return: The difference, in seconds, between the moment this function is called and the (future) datetime passed as argument.
+    If return value is negative (e.g., an event presumed to be in the future is actually in the past), throws exception.
+    """
+    from datetime import datetime
+    delay = datetime.strptime( future, DATA_FORMAT ).timestamp() - datetime.now().timestamp()
+    if delay < 0:
+        raise SystemError( "Tracker timing error: attempting to track object at time [" + future + "] indicates this time has already passed. Possibly the result of a long-running user process delaying thread execution." )
+    return delay
 
 
 def convert_numeric_month( r ) -> str:
     return r.replace( "Jan", "01" ).replace( "Feb", "02" ).replace( "Mar", "03" ).replace( "Apr", "04" ).replace( "May", "05" ).replace( "Jun", "06" ).replace( "Jul", "07" ).replace( "Aug", "08" ).replace( "Sep", "09" ).replace( "Oct", "10" ).replace( "Nov", "11" ).replace( "Dec", "12" )
 
 
 def get_jpl_ephemeris(  start_time: str,
@@ -219,15 +295,15 @@
     if "$$SOE" not in response:
         raise SystemError( "NASA/JPL Horizons API response invalid. Check src.Ephemeris argument format." )
 
 
 def validate_jpl_ephemeris_date(t):
     from datetime import datetime
     try:
-        d = datetime.strptime( convert_numeric_month(t), DATA_FORMAT )
+        d = datetime.strptime( t, DATA_FORMAT )
     except ValueError as e:
         raise SystemError( "Invalid date format! Dates must be in format YYYY-MM-DD HH:MM:SS as 24h clock." ) from e
     if d.timestamp() < datetime.strptime( '1599-12-10 23:59:00', DATA_FORMAT ).timestamp():
         raise SystemError( "Earliest accessible JPL Ephemeris date is 1599-12-10 23:59:00." )
     if d.timestamp() > datetime.strptime( '2500-12-31 23:58:00', DATA_FORMAT ).timestamp():
         raise SystemError( "Most distant accessible JPL Ephemeris date is 2500-12-31 23:58:00." )
 
@@ -235,16 +311,7 @@
 def validate_jpl_ephemeris_step_unit( u ):
     error = "Invalid step unit label. Check Check step_size argument format."
     try:
         if not VALID_STEP_LABELS.__contains__( u.split( ' ' )[1] ):
             raise SystemError( error )
     except IndexError:
         raise SystemError( error )
-
-
-def fixture() -> Ephemeris:
-    return Ephemeris( '1988-12-08 01:02:03', '1990-04-22 04:05:06', '-71.332597,42.458790,0.041', '1 day', '10' )
-
-
-def terminal_print( e = fixture() ):
-    for i in e.DATA_ENTRIES_RAW:
-        print( i )
```

### Comparing `sunspot-0.0.1/src/test.py` & `sunspot-0.6/src/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,18 +65,17 @@
     # 3/3: Only a single '83.979965' value found in vector 'Sky_mot_PA'. Confirm #find_corresponding_data returns str rather than list.
     dates = e.find_corresponding_data(  e.DATA_TITLES[0], 'Sky_mot_PA', '83.979965' )
     assert( type( dates ) == str )
 
 
 def verify_chronology( dates ):
     from datetime import datetime
-    dates = [sunspot.convert_numeric_month(item) for item in dates]
-    now = datetime.strptime(dates[0],sunspot.DATA_FORMAT)
+    now = datetime.strptime( dates[0], sunspot.DATA_FORMAT )
     for index in range( len(dates) - 1 ):
-        then = datetime.strptime(dates[index+1],sunspot.DATA_FORMAT)
+        then = datetime.strptime( dates[index+1], sunspot.DATA_FORMAT )
         assert ( then.timestamp() > now.timestamp() )
         now = then
 
 
 @pytest.mark.parametrize( 'fixture', FIXTURE_LIST_ALL )
 def test_corresponding_data_missing_target( fixture, request ):
     """
@@ -134,28 +133,28 @@
     """
     from datetime import datetime
     e = request.getfixturevalue( fixture )
     dates_index = 0
     for title_index in range( 1, len( e.DATA_TITLES ) ):
         for date_index in range( -1, len( e.dates() ) - 2 ):
             now = e.find_corresponding_data( e.DATA_TITLES[dates_index], e.DATA_TITLES[title_index], e.get_ephemeris_data( e.DATA_TITLES[title_index] )[date_index+1] )
-            now = datetime.strptime(sunspot.convert_numeric_month(now),sunspot.DATA_FORMAT)
+            now = datetime.strptime( now, sunspot.DATA_FORMAT )
             then = e.find_corresponding_data( e.DATA_TITLES[dates_index], e.DATA_TITLES[title_index], e.get_ephemeris_data( e.DATA_TITLES[title_index] )[date_index+2] )
-            then = datetime.strptime(sunspot.convert_numeric_month(then),sunspot.DATA_FORMAT)
+            then = datetime.strptime( then, sunspot.DATA_FORMAT )
             assert( then.timestamp() > now.timestamp() )
 
 
 @pytest.fixture
 def fixture_default_args() -> sunspot.Ephemeris:
     """
     :return: Ephemeris recovers data vectors for a default set of args, e.g., no 5th arg to src.Ephemeris()
     """
     return sunspot.Ephemeris('1988-12-08 01:02:03',
                                 '1990-04-22 04:05:06',
-                                '-71.332597,42.458790,0.041',
+                                '-71.332597, 42.458790, 0.041',
                                 '1 day',
                                 '10')
 
 
 @pytest.fixture
 def fixture_1_args() -> sunspot.Ephemeris:
     """
@@ -168,30 +167,30 @@
                                 '10',
                                 '1')
 
 
 @pytest.fixture
 def fixture_2_args() -> sunspot.Ephemeris:
     """
-    :return: Ephemeris recovers two data vectors (4 and 2)
+    :return: Ephemeris recovers two data vectors (2 and 4)
     """
     return sunspot.Ephemeris('1988-12-08 01:02:03',
                                 '1990-04-22 04:05:06',
                                 '-71.332597,42.458790,0.041',
                                 '1 day',
                                 '10',
                                 '2,4')
 
 
 @pytest.fixture
 def fixture_2_args_reversed() -> sunspot.Ephemeris:
     """
-    :return: Ephemeris recovers two data vectors (4 and 2)
+    :return: Ephemeris recovers two data vectors (4 and 2). Start time HH:MM:SS is such that SS = 00.
     """
-    return sunspot.Ephemeris('1988-12-08 01:02:03',
+    return sunspot.Ephemeris('1988-12-08 01:02:00',
                                 '1990-04-22 04:05:06',
                                 '-71.332597,42.458790,0.041',
                                 '1 day',
                                 '10',
                                 '4,2')
```

