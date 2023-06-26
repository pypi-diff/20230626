# Comparing `tmp/pix_framework-0.8.9.tar.gz` & `tmp/pix_framework-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pix_framework-0.8.9.tar", max compression
+gzip compressed data, was "pix_framework-0.9.0.tar", max compression
```

## Comparing `pix_framework-0.8.9.tar` & `pix_framework-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-06-08 15:10:45.934945 pix_framework-0.8.9/LICENSE
--rw-r--r--   0        0        0      549 2023-06-08 15:10:45.934945 pix_framework-0.8.9/README.md
--rw-r--r--   0        0        0      799 2023-06-08 15:10:45.934945 pix_framework-0.8.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/__init__.py
--rw-r--r--   0        0        0       32 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/calendar/__init__.py
--rw-r--r--   0        0        0     7524 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/calendar/availability.py
--rw-r--r--   0        0        0    31886 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/calendar/resource_calendar.py
--rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/__init__.py
--rw-r--r--   0        0        0     5835 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/calendar_factory.py
--rw-r--r--   0        0        0     6967 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/case_arrival.py
--rw-r--r--   0        0        0     4903 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/gateway_probabilities.py
--rw-r--r--   0        0        0     5621 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/discovery/resource_pools.py
--rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/enhancement/__init__.py
--rw-r--r--   0        0        0     5444 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/enhancement/multitasking.py
--rw-r--r--   0        0        0       27 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/filesystem/__init__.py
--rw-r--r--   0        0        0     1088 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/filesystem/file_manager.py
--rw-r--r--   0        0        0     2498 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/input.py
--rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/io/__init__.py
--rw-r--r--   0        0        0    38326 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/io/bpm_graph.py
--rw-r--r--   0        0        0     2284 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/log_ids.py
--rw-r--r--   0        0        0        0 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/log_split/__init__.py
--rw-r--r--   0        0        0     4414 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/log_split/log_split.py
--rw-r--r--   0        0        0       27 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/statistics/__init__.py
--rw-r--r--   0        0        0    13047 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/statistics/distribution.py
--rw-r--r--   0        0        0      970 2023-06-08 15:10:45.934945 pix_framework-0.8.9/src/pix_framework/statistics/utils.py
--rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 pix_framework-0.8.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 09:23:27.785219 pix_framework-0.9.0/LICENSE
+-rw-r--r--   0        0        0      549 2023-06-09 09:23:27.785219 pix_framework-0.9.0/README.md
+-rw-r--r--   0        0        0      799 2023-06-09 09:23:27.785219 pix_framework-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/__init__.py
+-rw-r--r--   0        0        0       32 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/calendar/__init__.py
+-rw-r--r--   0        0        0     7396 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/calendar/availability.py
+-rw-r--r--   0        0        0    30618 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/calendar/resource_calendar.py
+-rw-r--r--   0        0        0        0 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/discovery/__init__.py
+-rw-r--r--   0        0        0     5455 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/discovery/calendar_factory.py
+-rw-r--r--   0        0        0     6883 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/discovery/case_arrival.py
+-rw-r--r--   0        0        0     4771 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/discovery/gateway_probabilities.py
+-rw-r--r--   0        0        0     5557 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/discovery/resource_pools.py
+-rw-r--r--   0        0        0        0 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/enhancement/__init__.py
+-rw-r--r--   0        0        0     5404 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/enhancement/multitasking.py
+-rw-r--r--   0        0        0       27 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/filesystem/__init__.py
+-rw-r--r--   0        0        0     1088 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/filesystem/file_manager.py
+-rw-r--r--   0        0        0     2388 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/input.py
+-rw-r--r--   0        0        0        0 2023-06-09 09:23:27.785219 pix_framework-0.9.0/src/pix_framework/io/__init__.py
+-rw-r--r--   0        0        0    36970 2023-06-09 09:23:27.789219 pix_framework-0.9.0/src/pix_framework/io/bpm_graph.py
+-rw-r--r--   0        0        0     2268 2023-06-09 09:23:27.789219 pix_framework-0.9.0/src/pix_framework/log_ids.py
+-rw-r--r--   0        0        0        0 2023-06-09 09:23:27.789219 pix_framework-0.9.0/src/pix_framework/log_split/__init__.py
+-rw-r--r--   0        0        0     4256 2023-06-09 09:23:27.789219 pix_framework-0.9.0/src/pix_framework/log_split/log_split.py
+-rw-r--r--   0        0        0       27 2023-06-09 09:23:27.789219 pix_framework-0.9.0/src/pix_framework/statistics/__init__.py
+-rw-r--r--   0        0        0    15518 2023-06-09 09:23:27.789219 pix_framework-0.9.0/src/pix_framework/statistics/distribution.py
+-rw-r--r--   0        0        0      970 2023-06-09 09:23:27.789219 pix_framework-0.9.0/src/pix_framework/statistics/utils.py
+-rw-r--r--   0        0        0     1257 1970-01-01 00:00:00.000000 pix_framework-0.9.0/PKG-INFO
```

### Comparing `pix_framework-0.8.9/LICENSE` & `pix_framework-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.9/README.md` & `pix_framework-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.9/pyproject.toml` & `pix_framework-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pix-framework"
-version = "0.8.9"
+version = "0.9.0"
 description = "Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project."
 authors = [
     "David Chapela de la Campa <david.chapela.delacampa@gmail.com>",
     "Ihar Suvorau <ihar.suvorau@gmail.com>",
 ]
 readme = "README.md"
 packages = [{ include = "pix_framework", from = "src" }]
```

### Comparing `pix_framework-0.8.9/src/pix_framework/calendar/availability.py` & `pix_framework-0.9.0/src/pix_framework/calendar/availability.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 
 import pandas as pd
 import pytz
 
 from pix_framework.calendar.resource_calendar import RCalendar, Interval
 
 
-def get_last_available_timestamp(
-    start: pd.Timestamp, end: pd.Timestamp, schedule: RCalendar
-) -> pd.Timestamp:
+def get_last_available_timestamp(start: pd.Timestamp, end: pd.Timestamp, schedule: RCalendar) -> pd.Timestamp:
     """
     Get the timestamp [last_available] within the interval from [start] to [end] (i.e. [start] <= [last_available] <= [end]) such that
     the interval from [last_available] to [end] is the largest and all of it is in the working hours in the calendar [schedule].
 
     For example, for [start] = 09:30, [end] = 14:00, and a [schedule] of every week day from 06:00 to 09:00, and from 10:00 to 16:00. The
     [last_available] would be 10:00.
 
@@ -72,17 +70,15 @@
                 last_available = last_available.replace(
                     hour=interval_start.hour,
                     minute=interval_start.minute,
                     second=interval_start.second,
                     microsecond=interval_start.microsecond,
                 )
         if not found:
-            start_of_day = last_available.replace(
-                hour=00, minute=00, second=00, microsecond=0
-            )
+            start_of_day = last_available.replace(hour=00, minute=00, second=00, microsecond=0)
             if (last_available - start_of_day) > pd.Timedelta(seconds=2):
                 # Non-working interval between last_available and the start of the day
                 found = True
             else:
                 # Move to previous day at 23:59:59.999999
                 last_available = (last_available - pd.Timedelta(days=1)).replace(
                     hour=23, minute=59, second=59, microsecond=999999
@@ -129,25 +125,21 @@
                     month=current_instant.month,
                     year=current_instant.year,
                     tzinfo=pytz.timezone("UTC"),
                 )
                 if current_instant < interval_end:
                     if current_instant < interval_start:
                         # Non-working time gap between [current_instant] and the start of the current working interval, save it
-                        non_working_intervals += [
-                            Interval(current_instant, min(interval_start, end))
-                        ]
+                        non_working_intervals += [Interval(current_instant, min(interval_start, end))]
                     # Advance [current_instant] to the end of the working interval
                     current_instant = min(interval_end, end)
             # Current day finished, add non-working interval from current instant to end of day and advance
-            end_of_day = current_instant.replace(
-                hour=23, minute=59, second=59, microsecond=0
-            ) + pd.Timedelta(microseconds=999999)
+            end_of_day = current_instant.replace(hour=23, minute=59, second=59, microsecond=0) + pd.Timedelta(
+                microseconds=999999
+            )
             if current_instant < end:
-                non_working_intervals += [
-                    Interval(current_instant, min(end_of_day, end))
-                ]
+                non_working_intervals += [Interval(current_instant, min(end_of_day, end))]
                 current_instant = (current_instant + pd.Timedelta(days=1)).replace(
                     hour=0, minute=0, second=0, microsecond=0
                 )
     # Return found non-working intervals
     return non_working_intervals
```

### Comparing `pix_framework-0.8.9/src/pix_framework/calendar/resource_calendar.py` & `pix_framework-0.9.0/src/pix_framework/calendar/resource_calendar.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,21 +114,16 @@
             self.resource_task_freq[r_name][t_name] = 0
             self.active_res_task_weekdays[r_name][t_name] = {}
             self.active_res_task_weekdays_granules[r_name][t_name] = {}
             self.res_task_weekdays_granules_freq[r_name][t_name] = {}
         if weekday not in self.active_res_task_weekdays[r_name][t_name]:
             self.active_res_task_weekdays[r_name][t_name][weekday] = set()
             self.active_res_task_weekdays_granules[r_name][t_name][weekday] = {}
-        if (
-            g_index
-            not in self.active_res_task_weekdays_granules[r_name][t_name][weekday]
-        ):
-            self.active_res_task_weekdays_granules[r_name][t_name][weekday][
-                g_index
-            ] = set()
+        if g_index not in self.active_res_task_weekdays_granules[r_name][t_name][weekday]:
+            self.active_res_task_weekdays_granules[r_name][t_name][weekday][g_index] = set()
         if g_index not in self.res_task_weekdays_granules_freq[r_name][t_name]:
             self.res_task_weekdays_granules_freq[r_name][t_name][g_index] = {}
         if weekday not in self.res_task_weekdays_granules_freq[r_name][t_name][g_index]:
             self.res_task_weekdays_granules_freq[r_name][t_name][g_index][weekday] = 0
         if weekday not in self.res_active_weekdays[r_name]:
             self.res_active_weekdays[r_name][weekday] = set()
         if g_index not in self.res_active_granules_weekdays[r_name]:
@@ -143,34 +138,30 @@
             self.observed_weekdays[weekday] = set()
 
         # Updating the weekdays and granules the resource was observed working
         self.res_active_weekdays[r_name][weekday].add(str_date)
         self.res_active_granules_weekdays[r_name][g_index][weekday].add(str_date)
         self.res_granules_frequency[r_name][g_index][weekday] += 1
 
-        self.active_res_task_weekdays_granules[r_name][t_name][weekday][g_index].add(
-            str_date
-        )
+        self.active_res_task_weekdays_granules[r_name][t_name][weekday][g_index].add(str_date)
         self.active_res_task_weekdays[r_name][t_name][weekday].add(str_date)
 
         self.resource_freq[r_name] += 1
         self.resource_task_freq[r_name][t_name] += 1
         self.res_count_events_in_log[r_name] += 1
         self.shared_task_granules[r_name][g_index][weekday].add(t_name)
         self.res_task_weekdays_granules_freq[r_name][t_name][g_index][weekday] += 1
 
         if not is_joint:
             self.max_resource_task_freq[t_name] = max(
                 self.max_resource_task_freq[t_name],
                 self.resource_task_freq[r_name][t_name],
             )
             self.observed_weekdays[weekday].add(str_date)
-            self.max_resource_freq = max(
-                self.max_resource_freq, self.resource_freq[r_name]
-            )
+            self.max_resource_freq = max(self.max_resource_freq, self.resource_freq[r_name])
             self.task_events_count[t_name] += 1
             self.total_events_in_log += 1
 
     def register_task_enablement(self, trace_events):
         self.res_enabled_task_granules = None
         for e_info in trace_events:
             t_name = e_info.task_name
@@ -197,30 +188,21 @@
             joint_granules = {}
             for t_name in self.resource_task_freq[r_name]:
                 for g_index in self.task_enabled_in_granule[t_name]:
                     if g_index not in self.res_enabled_task_granules[r_name]:
                         joint_granules[g_index] = {}
                         self.res_enabled_task_granules[r_name][g_index] = {}
                     for weekday in self.task_enabled_in_granule[t_name][g_index]:
-                        if (
-                            weekday
-                            not in self.res_enabled_task_granules[r_name][g_index]
-                        ):
-                            self.res_enabled_task_granules[r_name][g_index][
-                                weekday
-                            ] = set()
+                        if weekday not in self.res_enabled_task_granules[r_name][g_index]:
+                            self.res_enabled_task_granules[r_name][g_index][weekday] = set()
                             joint_granules[g_index][weekday] = set()
-                        joint_granules[g_index][
-                            weekday
-                        ] |= self.task_enabled_in_granule[t_name][g_index][weekday]
+                        joint_granules[g_index][weekday] |= self.task_enabled_in_granule[t_name][g_index][weekday]
             for g_index in joint_granules:
                 for weekday in joint_granules[g_index]:
-                    self.res_enabled_task_granules[r_name][g_index][weekday] = len(
-                        joint_granules[g_index][weekday]
-                    )
+                    self.res_enabled_task_granules[r_name][g_index][weekday] = len(joint_granules[g_index][weekday])
 
     def enablement_confidence(self, r_name, weekday, g_index):
         if self.res_enabled_task_granules is None:
             self.compute_resource_task_granule_enablement()
         return (
             len(self.res_active_granules_weekdays[r_name][g_index][weekday])
             / self.res_enabled_task_granules[r_name][g_index][weekday]
@@ -245,43 +227,34 @@
         for t_name in self.resource_task_freq[r_name]:
             total_res += self.resource_task_freq[r_name][t_name]
             total_max += self.max_resource_task_freq[t_name]
         return total_res / total_max if total_max > 0 else 0
 
     def resource_task_participation_ratio(self, r_name, t_name):
         if self.max_resource_task_freq[t_name] > 0:
-            return (
-                self.resource_task_freq[r_name][t_name]
-                / self.max_resource_task_freq[t_name]
-            )
+            return self.resource_task_freq[r_name][t_name] / self.max_resource_task_freq[t_name]
         return 0
 
     # From all the WeekDays the resource was active, in which ration they were in the given granule
     def confidence(self, r_name, weekday, g_index):
         return len(self.res_active_granules_weekdays[r_name][g_index][weekday]) / len(
             self.res_active_weekdays[r_name][weekday]
         )
 
     def support(self, r_name, weekday, g_index):
-        return len(self.res_active_granules_weekdays[r_name][g_index][weekday]) / len(
-            self.observed_weekdays[weekday]
-        )
+        return len(self.res_active_granules_weekdays[r_name][g_index][weekday]) / len(self.observed_weekdays[weekday])
 
     def weekday_support(self, r_name, weekday):
-        return len(self.res_active_weekdays[r_name][weekday]) / len(
-            self.observed_weekdays[weekday]
-        )
+        return len(self.res_active_weekdays[r_name][weekday]) / len(self.observed_weekdays[weekday])
 
     def task_coverage(self, t_name):
         return self.task_events_in_calendar[t_name] / self.task_events_count[t_name]
 
     def can_improve_support(self, r_name, weekday, g_index):
-        best_task, confidence_values = self.task_cond_confidence(
-            r_name, weekday, g_index
-        )
+        best_task, confidence_values = self.task_cond_confidence(r_name, weekday, g_index)
 
         return best_task
 
     def reset_calendar_info(self):
         self.total_events_in_calendar = 0
         for t_name in self.task_events_count:
             self.task_events_in_calendar[t_name] = 0
@@ -289,39 +262,29 @@
             self.res_count_events_in_calendar[r_name] = 0
             self.active_granules_in_calendar[r_name] = set()
             self.active_weekdays_in_calendar[r_name] = set()
             self.g_discarded[r_name] = []
             self.confidence_numerator_sum[r_name] = 0
             self.confidence_denominator_sum[r_name] = 0
 
-    def check_accepted_granule(
-        self, r_name, weekday, g_index, best_task
-    ):  # TODO: what does it check?
-        self.res_count_events_in_calendar[r_name] += self.res_granules_frequency[
-            r_name
-        ][g_index][weekday]
-        self.total_events_in_calendar += self.res_granules_frequency[r_name][g_index][
-            weekday
-        ]
+    def check_accepted_granule(self, r_name, weekday, g_index, best_task):  # TODO: what does it check?
+        self.res_count_events_in_calendar[r_name] += self.res_granules_frequency[r_name][g_index][weekday]
+        self.total_events_in_calendar += self.res_granules_frequency[r_name][g_index][weekday]
         self.confidence_numerator_sum[r_name] += len(
             self.active_res_task_weekdays_granules[r_name][best_task][weekday][g_index]
         )
-        self.confidence_denominator_sum[r_name] += len(
-            self.active_res_task_weekdays[r_name][best_task][weekday]
-        )
-        self.active_granules_in_calendar[
-            r_name
-        ] |= self.active_res_task_weekdays_granules[r_name][best_task][weekday][g_index]
-        self.active_weekdays_in_calendar[r_name] |= self.active_res_task_weekdays[
-            r_name
-        ][best_task][weekday]
+        self.confidence_denominator_sum[r_name] += len(self.active_res_task_weekdays[r_name][best_task][weekday])
+        self.active_granules_in_calendar[r_name] |= self.active_res_task_weekdays_granules[r_name][best_task][weekday][
+            g_index
+        ]
+        self.active_weekdays_in_calendar[r_name] |= self.active_res_task_weekdays[r_name][best_task][weekday]
         for t_name in self.shared_task_granules[r_name][g_index][weekday]:
-            self.task_events_in_calendar[
-                t_name
-            ] += self.res_task_weekdays_granules_freq[r_name][t_name][g_index][weekday]
+            self.task_events_in_calendar[t_name] += self.res_task_weekdays_granules_freq[r_name][t_name][g_index][
+                weekday
+            ]
 
     def check_discarded_granule(self, r_name, weekday, g_index):
         if r_name not in self.g_discarded:
             self.g_discarded[r_name] = []
         self.g_discarded[r_name].append(GranuleInfo(weekday, g_index))
 
     def update_discarded_granules_list(self, r_name, accepted_indexes):
@@ -348,34 +311,29 @@
         if (
             r_name not in self.active_weekdays_in_calendar
             or len(self.active_weekdays_in_calendar[r_name]) == 0
             or self.res_count_events_in_log[r_name] == 0
         ):
             return 0, 0
         return (
-            self.confidence_numerator_sum[r_name]
-            / self.confidence_denominator_sum[r_name],
-            self.res_count_events_in_calendar[r_name]
-            / self.res_count_events_in_log[r_name],
+            self.confidence_numerator_sum[r_name] / self.confidence_denominator_sum[r_name],
+            self.res_count_events_in_calendar[r_name] / self.res_count_events_in_log[r_name],
         )
 
 
 class IntervalPoint:
     def __init__(self, date_time, week_day, index, to_start_dist, to_end_dist):
         self.date_time = date_time
         self.week_day = week_day
         self.index = index
         self.to_start_dist = to_start_dist
         self.to_end_dist = to_end_dist
 
     def in_same_interval(self, another_point):
-        return (
-            self.week_day == another_point.week_day
-            and self.index == another_point.index
-        )
+        return self.week_day == another_point.week_day and self.index == another_point.index
 
 
 @dataclass
 class Interval:
     start: datetime.datetime
     end: datetime.datetime
     duration: float
@@ -409,82 +367,62 @@
 
     def is_after(self, c_date):
         return c_date <= self.start
 
     def intersection(self, interval):
         if interval is None:
             return None
-        [first_i, second_i] = (
-            [self, interval] if self.start <= interval.start else [interval, self]
-        )
+        [first_i, second_i] = [self, interval] if self.start <= interval.start else [interval, self]
         if second_i.start < first_i.end:
-            return Interval(
-                max(first_i.start, second_i.start), min(first_i.end, second_i.end)
-            )
+            return Interval(max(first_i.start, second_i.start), min(first_i.end, second_i.end))
         return None
 
 
 class CalendarIterator:
     def __init__(self, start_date: datetime, calendar_info):
         self.start_date = start_date
 
         self.calendar = calendar_info
 
         self.c_day = start_date.date().weekday()
 
-        c_date = datetime.datetime.combine(
-            calendar_info.default_date, start_date.time()
-        )
+        c_date = datetime.datetime.combine(calendar_info.default_date, start_date.time())
         c_interval = calendar_info.work_intervals[self.c_day][0]
         self.c_index = -1
-        while (
-            c_interval.end < c_date
-            and self.c_index < len(calendar_info.work_intervals[self.c_day]) - 1
-        ):
+        while c_interval.end < c_date and self.c_index < len(calendar_info.work_intervals[self.c_day]) - 1:
             self.c_index += 1
             c_interval = calendar_info.work_intervals[self.c_day][self.c_index]
 
         self.c_interval = Interval(
             self.start_date,
-            self.start_date
-            + timedelta(seconds=(c_interval.end - c_date).total_seconds()),
+            self.start_date + timedelta(seconds=(c_interval.end - c_date).total_seconds()),
         )
 
     def next_working_interval(self):
         res_interval = self.c_interval
         day_intervals = self.calendar.work_intervals[self.c_day]
         p_duration = 0
 
         self.c_index += 1
         if self.c_index >= len(day_intervals):
-            p_duration += (
-                86400
-                - (
-                    day_intervals[self.c_index - 1].end - self.calendar.new_day
-                ).total_seconds()
-            )
+            p_duration += 86400 - (day_intervals[self.c_index - 1].end - self.calendar.new_day).total_seconds()
             while True:
                 self.c_day = (self.c_day + 1) % 7
                 day_intervals = self.calendar.work_intervals[self.c_day]
                 if len(day_intervals) > 0:
-                    p_duration += (
-                        day_intervals[0].start - self.calendar.new_day
-                    ).total_seconds()
+                    p_duration += (day_intervals[0].start - self.calendar.new_day).total_seconds()
                     break
                 else:
                     p_duration += 86400
             self.c_index = 0
         elif self.c_index > 0:
-            p_duration += (
-                day_intervals[self.c_index].start - day_intervals[self.c_index - 1].end
-            ).total_seconds()
+            p_duration += (day_intervals[self.c_index].start - day_intervals[self.c_index - 1].end).total_seconds()
         self.c_interval = Interval(
             res_interval.end + timedelta(seconds=p_duration),
-            res_interval.end
-            + timedelta(seconds=p_duration + day_intervals[self.c_index].duration),
+            res_interval.end + timedelta(seconds=p_duration + day_intervals[self.c_index].duration),
         )
         return res_interval
 
 
 class RCalendar:  # AvailabilityCalendar
     def __init__(self, calendar_id):
         self.calendar_id = calendar_id
@@ -540,28 +478,24 @@
                     self.add_calendar_item(
                         int_week_days[i],
                         int_week_days[i],
                         str(interval.start.time()),
                         str(interval.end.time()),
                     )
 
-    def add_calendar_item(
-        self, from_day: str, to_day: str, begin_time: str, end_time: str
-    ):
+    def add_calendar_item(self, from_day: str, to_day: str, begin_time: str, end_time: str):
         if from_day.upper() in str_week_days and to_day.upper() in str_week_days:
             try:
                 t_interval = Interval(
                     start=pd.Timestamp(begin_time).to_pydatetime(),
                     end=pd.Timestamp(end_time).to_pydatetime(),
                 )
                 if self.default_date is None:
                     self.default_date = t_interval.start.date()
-                    self.new_day = datetime.datetime.combine(
-                        self.default_date, datetime.time()
-                    )
+                    self.new_day = datetime.datetime.combine(self.default_date, datetime.time())
                 d_s = str_week_days[from_day]
                 d_e = str_week_days[to_day]
                 while True:
                     self._add_interval(d_s % 7, t_interval)
                     if d_s % 7 == d_e:
                         break
                     d_s += 1
@@ -628,32 +562,28 @@
         if duration > self.total_weekly_work:
             real_duration += to_seconds(int(duration / self.total_weekly_work), "WEEKS")
             pending_duration %= self.total_weekly_work
         # Addressing the first day as an special case
         c_day = requested_date.date().weekday()
         c_date = datetime.datetime.combine(self.default_date, requested_date.time())
 
-        worked_time, total_time = self._find_time_starting(
-            pending_duration, c_day, c_date
-        )
+        worked_time, total_time = self._find_time_starting(pending_duration, c_day, c_date)
         if worked_time > total_time and worked_time - total_time < 0.001:
             total_time = worked_time
         pending_duration -= worked_time
         real_duration += total_time
         c_date = self.new_day
         while pending_duration > 0:
             c_day += 1
             r_d = c_day % 7
             if pending_duration > self.work_rest_count[r_d][0]:
                 pending_duration -= self.work_rest_count[r_d][0]
                 real_duration += 86400
             else:
-                real_duration += self._find_time_completion(
-                    pending_duration, self.work_rest_count[r_d][0], r_d, c_date
-                )
+                real_duration += self._find_time_completion(pending_duration, self.work_rest_count[r_d][0], r_d, c_date)
                 break
         return real_duration
 
     def next_available_time(self, requested_date):
         """
         Validates whether the 'requested_date' is located in the arrival time calendar.
         Valid = complies with the provided time periods of the arrival calendar.
@@ -671,20 +601,15 @@
                 return (interval.start - c_date).total_seconds()
             if interval.contains(c_date):
                 return 0
         duration = 86400 - (c_date - self.new_day).total_seconds()
         for i in range(c_day + 1, c_day + 8):
             r_day = i % 7
             if self.work_rest_count[r_day][0] > 0:
-                return (
-                    duration
-                    + (
-                        self.work_intervals[r_day][0].start - self.new_day
-                    ).total_seconds()
-                )
+                return duration + (self.work_intervals[r_day][0].start - self.new_day).total_seconds()
             duration += 86400
         return duration
 
     def find_working_time(self, start_date, end_date):
         pending_duration = (end_date - start_date).total_seconds()
         worked_hours = 0
 
@@ -725,39 +650,33 @@
         available_duration = self._calculate_available_duration(c_day, from_date)
         if available_duration <= pending_duration:
             return (
                 available_duration,
                 86400 - (from_date - self.new_day).total_seconds(),
             )
         else:
-            return pending_duration, self._find_time_completion(
-                pending_duration, available_duration, c_day, from_date
-            )
+            return pending_duration, self._find_time_completion(pending_duration, available_duration, c_day, from_date)
 
     def _calculate_available_duration(self, c_day, from_date):
         i = -1
         passed_duration = 0
         for t_interval in self.work_intervals[c_day]:
             i += 1
             if t_interval.is_before(from_date):
                 passed_duration += t_interval.duration
                 continue
             if t_interval.is_after(from_date):
                 break
             if t_interval.contains(from_date):
-                passed_duration += (
-                    from_date - self.work_intervals[c_day][i].start
-                ).total_seconds()
+                passed_duration += (from_date - self.work_intervals[c_day][i].start).total_seconds()
                 break
 
         return self.work_rest_count[c_day][0] - passed_duration
 
-    def _find_time_completion(
-        self, pending_duration, total_duration, c_day, from_datetime
-    ):
+    def _find_time_completion(self, pending_duration, total_duration, c_day, from_datetime):
         i = len(self.work_intervals[c_day]) - 1
         while total_duration > pending_duration:
             total_duration -= self.work_intervals[c_day][i].duration
             i -= 1
         if total_duration < pending_duration:
             to_datetime = self.work_intervals[c_day][i + 1].start + timedelta(
                 seconds=(pending_duration - total_duration)
@@ -784,16 +703,14 @@
                     )
 
 
 def build_full_time_calendar(calendar_id) -> RCalendar:
     r_calendar = RCalendar(calendar_id)
     for i in range(0, 7):
         str_weekday = int_week_days[i]
-        r_calendar.add_calendar_item(
-            str_weekday, str_weekday, "00:00:00.000", "23:59:59.999"
-        )
+        r_calendar.add_calendar_item(str_weekday, str_weekday, "00:00:00.000", "23:59:59.999")
     return r_calendar
 
 
 def to_seconds(value, from_unit):
     u_from = from_unit.upper()
     return value * conversion_table[u_from] if u_from in conversion_table else value
```

### Comparing `pix_framework-0.8.9/src/pix_framework/discovery/calendar_factory.py` & `pix_framework-0.9.0/src/pix_framework/discovery/calendar_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,91 +21,70 @@
         self.kpi_calendar = CalendarKPIInfoFactory(minutes_x_granule)
         self.minutes_x_granule = minutes_x_granule
 
         self.from_datetime = datetime.datetime(9999, 12, 31, tzinfo=pytz.UTC)
         self.to_datetime = datetime.datetime(1, 1, 1, tzinfo=pytz.UTC)
 
     def check_date_time(self, resource_name, activity_name, timestamp, is_joint=False):
-        self.kpi_calendar.register_resource_timestamp(
-            resource_name, activity_name, timestamp, is_joint
-        )
+        self.kpi_calendar.register_resource_timestamp(resource_name, activity_name, timestamp, is_joint)
 
         self.from_datetime = min(self.from_datetime, timestamp)
         self.to_datetime = max(self.to_datetime, timestamp)
 
-    def build_weekly_calendars(
-        self, min_confidence, desired_support, min_participation
-    ) -> Dict[str, RCalendar]:
+    def build_weekly_calendars(self, min_confidence, desired_support, min_participation) -> Dict[str, RCalendar]:
         """
         Builds a calendar for each resource in the KPI calendar, using the given parameters.
         Returns a dictionary with the resource name as key and its calendar as value.
         """
 
         self.kpi_calendar.reset_calendar_info()
 
         r_calendars = {}
 
         for r_name in self.kpi_calendar.shared_task_granules:
-            if (
-                self.kpi_calendar.resource_participation_ratio(r_name)
-                >= min_participation
-            ):
-                r_calendars[r_name] = self._build_resource_calendar(
-                    r_name, min_confidence, desired_support
-                )
+            if self.kpi_calendar.resource_participation_ratio(r_name) >= min_participation:
+                r_calendars[r_name] = self._build_resource_calendar(r_name, min_confidence, desired_support)
             else:
                 r_calendars[r_name] = None
 
         return r_calendars
 
-    def _build_resource_calendar(
-        self, r_name, min_confidence, desired_support
-    ) -> RCalendar:
+    def _build_resource_calendar(self, r_name, min_confidence, desired_support) -> RCalendar:
         kpi_c = self.kpi_calendar
         r_calendar = RCalendar("%s_Schedule" % r_name)
 
         count = 0
         for g_index in kpi_c.shared_task_granules[r_name]:
             for weekday in kpi_c.shared_task_granules[r_name][g_index]:
-                best_task, conf_values = kpi_c.task_cond_confidence(
-                    r_name, weekday, g_index
-                )
+                best_task, conf_values = kpi_c.task_cond_confidence(r_name, weekday, g_index)
                 if min_confidence <= conf_values[best_task]:
                     kpi_c.check_accepted_granule(r_name, weekday, g_index, best_task)
                     self._add_calendar_item(weekday, g_index, r_calendar)
                 else:
                     count += 1
                     kpi_c.g_discarded[r_name].append(GranuleInfo(weekday, g_index))
 
         # TODO: part below looks like a special case which can be handled in a separate function
 
         confidence, support = kpi_c.compute_confidence_support(r_name)
 
         if confidence > 0 and support < desired_support:
             kpi_c.g_discarded[r_name].sort(
-                key=lambda x: kpi_c.res_granules_frequency[r_name][x.granule_index][
-                    x.week_day
-                ],
+                key=lambda x: kpi_c.res_granules_frequency[r_name][x.granule_index][x.week_day],
                 reverse=True,
             )
 
             accepted_indexes = []
             i = 0
             for g_info in kpi_c.g_discarded[r_name]:
-                best_task = kpi_c.can_improve_support(
-                    r_name, g_info.week_day, g_info.granule_index
-                )
+                best_task = kpi_c.can_improve_support(r_name, g_info.week_day, g_info.granule_index)
 
                 if best_task is not None:
-                    self._add_calendar_item(
-                        g_info.week_day, g_info.granule_index, r_calendar
-                    )
-                    kpi_c.check_accepted_granule(
-                        r_name, g_info.week_day, g_info.granule_index, best_task
-                    )
+                    self._add_calendar_item(g_info.week_day, g_info.granule_index, r_calendar)
+                    kpi_c.check_accepted_granule(r_name, g_info.week_day, g_info.granule_index, best_task)
                     accepted_indexes.append(i)
                 _, support = kpi_c.compute_confidence_support(r_name)
 
                 if support >= desired_support:
                     break
 
                 i += 1
@@ -120,17 +99,15 @@
         str_wday = int_week_days[week_day]
         hour = (g_index * self.minutes_x_granule) // 60
         from_min = (g_index * self.minutes_x_granule) % 60
         to_min = from_min + self.minutes_x_granule
 
         if to_min >= 60:
             if hour == 23:
-                r_calendar.add_calendar_item(
-                    str_wday, str_wday, "%d:%d:%d" % (hour, from_min, 0), "23:59:59.999"
-                )
+                r_calendar.add_calendar_item(str_wday, str_wday, "%d:%d:%d" % (hour, from_min, 0), "23:59:59.999")
             else:
                 r_calendar.add_calendar_item(
                     str_wday,
                     str_wday,
                     "%d:%d:%d" % (hour, from_min, 0),
                     "%d:%d:%d" % (hour + 1, 0, 0),
                 )
```

### Comparing `pix_framework-0.8.9/src/pix_framework/discovery/case_arrival.py` & `pix_framework-0.9.0/src/pix_framework/discovery/case_arrival.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,26 +59,20 @@
     :param granularity: number of minutes to take as minimum available interval surrounding each
                         observed arrival for the calendar.
     :param filter_outliers: flag to remove outlier in the inter-arrival time discovery.
 
     :return: case arrival model.
     """
     return CaseArrivalModel(
-        case_arrival_calendar=discover_case_arrival_calendar(
-            event_log, log_ids, granularity
-        ),
-        inter_arrival_times=discover_inter_arrival_distribution(
-            event_log, log_ids, filter_outliers
-        ),
+        case_arrival_calendar=discover_case_arrival_calendar(event_log, log_ids, granularity),
+        inter_arrival_times=discover_inter_arrival_distribution(event_log, log_ids, filter_outliers),
     )
 
 
-def discover_case_arrival_calendar(
-    event_log: pd.DataFrame, log_ids: EventLogIDs, granularity=60
-) -> RCalendar:
+def discover_case_arrival_calendar(event_log: pd.DataFrame, log_ids: EventLogIDs, granularity=60) -> RCalendar:
     """
     Discover weekly calendar for the arrival of new cases, i.e., the periods of times in each day when
     new cases arrive to the system.
 
     :param event_log: event log to model the case arrivals from.
     :param log_ids: Event log column IDs.
     :param granularity: number of minutes to take as minimum available interval surrounding each
@@ -95,17 +89,15 @@
     for case_id, events in event_log.groupby(by=log_ids.case):
         resource = "system"  # Assign all arrivals to the same resource
         activity = "case_arrival"  # Assign same activity label to all arrivals
         case_arrival = events[log_ids.start_time].min()
         calendar_factory.check_date_time(resource, activity, case_arrival)
 
     # Discover calendar for the case arrivals
-    calendars = calendar_factory.build_weekly_calendars(
-        min_confidence=0.1, desired_support=0.7, min_participation=0.4
-    )
+    calendars = calendar_factory.build_weekly_calendars(min_confidence=0.1, desired_support=0.7, min_participation=0.4)
 
     calendar = calendars["system"]
     return calendar
 
 
 def discover_inter_arrival_distribution(
     event_log: pd.DataFrame, log_ids: EventLogIDs, filter_outliers: bool = True
@@ -117,17 +109,15 @@
     :param log_ids: Event log column IDs.
     :param filter_outliers: flag to remove outlier inter-arrival times.
     :return: Duration distribution for the inter-arrival times.
     """
     # Get the durations between each two consecutive arrivals
     inter_arrival_durations = _get_inter_arrival_times(event_log, log_ids)
     # Get the best distribution fitting the inter-arrival durations
-    arrival_distribution = get_best_fitting_distribution(
-        data=inter_arrival_durations, filter_outliers=filter_outliers
-    )
+    arrival_distribution = get_best_fitting_distribution(data=inter_arrival_durations, filter_outliers=filter_outliers)
     # Return it
     return arrival_distribution.to_prosimos_distribution()
 
 
 def get_observed_inter_arrival_distribution(
     event_log: pd.DataFrame,
     log_ids: EventLogIDs,
@@ -149,17 +139,15 @@
     arrival_distribution = get_observations_histogram(
         data=inter_arrival_durations, num_bins=num_bins, filter_outliers=filter_outliers
     )
     # Return custom histogram distribution
     return arrival_distribution
 
 
-def _get_inter_arrival_times(
-    event_log: pd.DataFrame, log_ids: EventLogIDs
-) -> List[float]:
+def _get_inter_arrival_times(event_log: pd.DataFrame, log_ids: EventLogIDs) -> List[float]:
     # Get the arrival times from the event log
     arrival_times = []
     for case_id, events in event_log.groupby(by=log_ids.case):
         arrival_times += [events[log_ids.start_time].min()]
     # Sort them
     arrival_times.sort()
     # Compute durations between one arrival and the next one (inter-arrival durations)
```

### Comparing `pix_framework-0.8.9/src/pix_framework/discovery/gateway_probabilities.py` & `pix_framework-0.9.0/src/pix_framework/discovery/gateway_probabilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,18 +65,15 @@
 
     DISCOVERY = "discovery"
     EQUIPROBABLE = "equiprobable"
 
     @classmethod
     def from_str(
         cls, value: Union[str, List[str]]
-    ) -> Union[
-        "GatewayProbabilitiesDiscoveryMethod",
-        List["GatewayProbabilitiesDiscoveryMethod"],
-    ]:
+    ) -> Union["GatewayProbabilitiesDiscoveryMethod", List["GatewayProbabilitiesDiscoveryMethod"],]:
         if isinstance(value, str):
             return GatewayProbabilitiesDiscoveryMethod._from_str(value)
         elif isinstance(value, list):
             return [GatewayProbabilitiesDiscoveryMethod._from_str(v) for v in value]
 
     @classmethod
     def _from_str(cls, value: str) -> "GatewayProbabilitiesDiscoveryMethod":
@@ -103,54 +100,44 @@
 ) -> List[GatewayProbabilities]:
     """
     Compute the gateway probabilities for a given event log and BPMN model.
     """
     if discovery_method is GatewayProbabilitiesDiscoveryMethod.EQUIPROBABLE:
         gateway_probabilities = bpmn_graph.compute_equiprobable_gateway_probabilities()
     elif discovery_method is GatewayProbabilitiesDiscoveryMethod.DISCOVERY:
-        gateway_probabilities = discover_gateway_probabilities(
-            bpmn_graph, event_log, log_ids
-        )
+        gateway_probabilities = discover_gateway_probabilities(bpmn_graph, event_log, log_ids)
     else:
-        raise ValueError(
-            f"Unknown gateway probabilities discovery method: {discovery_method}"
-        )
+        raise ValueError(f"Unknown gateway probabilities discovery method: {discovery_method}")
 
     return _translate_to_prosimos_format(gateway_probabilities)
 
 
-def discover_gateway_probabilities(
-    bpmn_graph: BPMNGraph, event_log: pd.DataFrame, log_ids: EventLogIDs
-):
+def discover_gateway_probabilities(bpmn_graph: BPMNGraph, event_log: pd.DataFrame, log_ids: EventLogIDs):
     """
     Discover the frequency of each gateway branch with replay.
     """
 
     arcs_frequencies = {}
 
     for _, events in event_log.groupby(log_ids.case):
-        trace = events.sort_values([log_ids.start_time, log_ids.end_time])[
-            log_ids.activity
-        ].tolist()
+        trace = events.sort_values([log_ids.start_time, log_ids.end_time])[log_ids.activity].tolist()
 
         bpmn_graph.replay_trace(trace, arcs_frequencies)
 
     gateway_probabilities = bpmn_graph.discover_gateway_probabilities(arcs_frequencies)
 
     return gateway_probabilities
 
 
 def _translate_to_prosimos_format(gateway_probabilities) -> List[GatewayProbabilities]:
     prosimos_gateway_probabilities = [
         GatewayProbabilities(
             gateway_id,
             [
-                PathProbability(
-                    outgoing_node, gateway_probabilities[gateway_id][outgoing_node]
-                )
+                PathProbability(outgoing_node, gateway_probabilities[gateway_id][outgoing_node])
                 for outgoing_node in gateway_probabilities[gateway_id]
             ],
         )
         for gateway_id in gateway_probabilities
     ]
 
     return prosimos_gateway_probabilities
```

### Comparing `pix_framework-0.8.9/src/pix_framework/discovery/resource_pools.py` & `pix_framework-0.9.0/src/pix_framework/discovery/resource_pools.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,17 @@
         self._activity_key = activity_key
         self._resource_key = resource_key
         self._drawing = drawing
         self._sim_threshold = sim_threshold
 
         self._log = self._filter_log(log)
 
-        self.tasks = {
-            val: i for i, val in enumerate(self._log[self._activity_key].unique())
-        }
-
-        self.users = {
-            val: i for i, val in enumerate(self._log[self._resource_key].unique())
-        }
+        self.tasks = {val: i for i, val in enumerate(self._log[self._activity_key].unique())}
+
+        self.users = {val: i for i, val in enumerate(self._log[self._resource_key].unique())}
 
         self.roles, self.resource_table = self._discover_roles()
 
     def _filter_log(self, log: pd.DataFrame):
         filtered_list = log[[self._activity_key, self._resource_key]]
         return filtered_list
 
@@ -142,20 +138,16 @@
         resource_table = []
         for record in records:
             for member in record["members"]:
                 resource_table.append({"role": record["role"], "resource": member})
         return records, resource_table
 
 
-def discover_resource_pools(
-    log: pd.DataFrame, log_ids: EventLogIDs
-) -> dict[str, list[str]]:
+def discover_resource_pools(log: pd.DataFrame, log_ids: EventLogIDs) -> dict[str, list[str]]:
     """
     Discover resource pools from an event log.
 
     Returns a dictionary mapping role names (pools) to lists of resource names.
     """
-    discoverer = _ResourcePoolDiscoverer(
-        log, activity_key=log_ids.activity, resource_key=log_ids.resource
-    )
+    discoverer = _ResourcePoolDiscoverer(log, activity_key=log_ids.activity, resource_key=log_ids.resource)
     df = pd.DataFrame(discoverer.resource_table)
     return df.groupby("role")["resource"].apply(list).to_dict()
```

### Comparing `pix_framework-0.8.9/src/pix_framework/enhancement/multitasking.py` & `pix_framework-0.9.0/src/pix_framework/enhancement/multitasking.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,32 +69,28 @@
         end_timestamps = events[log_ids.end_time]
         start_timestamps = events[log_ids.start_time]
         result = ((end_timestamps - start_timestamps) / (max_end - min_start)).sum()
         utilization[resource] = result
     return {"utilization": utilization, "number_of_events": number_of_events}
 
 
-def _adjust_duration_for_resource(
-    log: pd.DataFrame, log_ids: EventLogIDs, resource: str
-):
+def _adjust_duration_for_resource(log: pd.DataFrame, log_ids: EventLogIDs, resource: str):
     resource_events = log[log[log_ids.resource] == resource]
     data = _make_custom_records(resource_events, log, log_ids)
     aux_log = _make_auxiliary_log(data)
     _update_end_timestamps(aux_log, log, log_ids)
 
 
 def _make_aux_log(log, log_ids, resource):
     resource_events = log[log[log_ids.resource] == resource]
     data = _make_custom_records(resource_events, log, log_ids)
     return _make_auxiliary_log(data)
 
 
-def _make_custom_records(
-    resource_events: pd.DataFrame, log: pd.DataFrame, log_ids: EventLogIDs
-):
+def _make_custom_records(resource_events: pd.DataFrame, log: pd.DataFrame, log_ids: EventLogIDs):
     """
     Prepares records for the Sweep Line algorithm.
     """
     data = []
 
     for i, event in resource_events.iterrows():
         start_timestamp = event[log_ids.start_time]
@@ -148,23 +144,19 @@
             active_set[record.event_id] = record
         else:
             del active_set[record.event_id]
 
     return aux_log
 
 
-def _update_end_timestamps(
-    records: List[_AuxiliaryLogRecord], log: pd.DataFrame, log_ids: EventLogIDs
-) -> pd.DataFrame:
+def _update_end_timestamps(records: List[_AuxiliaryLogRecord], log: pd.DataFrame, log_ids: EventLogIDs) -> pd.DataFrame:
     """
     Modifies end timestamp according to the adjusted durations.
     """
     # group-by below works only on sorted data
     records = sorted(records, key=lambda record: record.event_id)
 
     for event_id, group in groupby(records, lambda record: record.event_id):
         duration = sum(map(lambda record: record.adjusted_duration_s, group))
-        log.at[event_id, log_ids.end_time] = log.loc[event_id][
-            log_ids.start_time
-        ] + pd.Timedelta(duration, unit="s")
+        log.at[event_id, log_ids.end_time] = log.loc[event_id][log_ids.start_time] + pd.Timedelta(duration, unit="s")
 
     return log
```

### Comparing `pix_framework-0.8.9/src/pix_framework/filesystem/file_manager.py` & `pix_framework-0.9.0/src/pix_framework/filesystem/file_manager.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.9/src/pix_framework/input.py` & `pix_framework-0.9.0/src/pix_framework/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,20 @@
             event_log[log_ids.resource].fillna(missing_resource, inplace=True)
     # Set resource type to string if numeric
     if log_ids.resource in event_log.columns:
         event_log[log_ids.resource] = event_log[log_ids.resource].apply(str)
     # Convert timestamp value to pd.Timestamp (setting timezone to UTC)
     event_log[log_ids.end_time] = pd.to_datetime(event_log[log_ids.end_time], utc=True)
     if log_ids.start_time in event_log.columns:
-        event_log[log_ids.start_time] = pd.to_datetime(
-            event_log[log_ids.start_time], utc=True
-        )
+        event_log[log_ids.start_time] = pd.to_datetime(event_log[log_ids.start_time], utc=True)
     if log_ids.enabled_time in event_log.columns:
-        event_log[log_ids.enabled_time] = pd.to_datetime(
-            event_log[log_ids.enabled_time], utc=True
-        )
+        event_log[log_ids.enabled_time] = pd.to_datetime(event_log[log_ids.enabled_time], utc=True)
     # Sort by end time
     if sort:
-        if (
-            log_ids.start_time in event_log.columns
-            and log_ids.enabled_time in event_log.columns
-        ):
-            event_log = event_log.sort_values(
-                [log_ids.start_time, log_ids.end_time, log_ids.enabled_time]
-            )
+        if log_ids.start_time in event_log.columns and log_ids.enabled_time in event_log.columns:
+            event_log = event_log.sort_values([log_ids.start_time, log_ids.end_time, log_ids.enabled_time])
         elif log_ids.start_time in event_log.columns:
             event_log = event_log.sort_values([log_ids.start_time, log_ids.end_time])
         else:
             event_log = event_log.sort_values(log_ids.end_time)
     # Return parsed event log
     return event_log
```

### Comparing `pix_framework-0.8.9/src/pix_framework/io/bpm_graph.py` & `pix_framework-0.9.0/src/pix_framework/io/bpm_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         self.end_event = None
         self.element_info = dict()
         self.from_name = dict()
         self.flow_arcs = dict()
         self.concurrent_enablers = dict()
         self.nodes_bitset = dict()
         self.arcs_bitset = dict()
-        self.or_join_pred = (
-            dict()
-        )  # or_id -> [0 = node predecesors bitset, 1 = predecesors flow arcs]
+        self.or_join_pred = dict()  # or_id -> [0 = node predecesors bitset, 1 = predecesors flow arcs]
         self.or_join_conflicting_pred = dict()
         self.decision_successors = dict()
         self.element_probability = None
         self.task_resource_probability = None
         self.closest_distance = None
         self.decision_flows_sortest_path = None
 
@@ -114,23 +112,20 @@
 
         bpmn_graph = BPMNGraph()
         for process in root.findall("xmlns:process", bpmn_element_ns):
             for xmlns_key in to_extract:
                 for bpmn_element in process.findall(xmlns_key, bpmn_element_ns):
                     name = (
                         bpmn_element.attrib["name"]
-                        if "name" in bpmn_element.attrib
-                        and len(bpmn_element.attrib["name"]) > 0
+                        if "name" in bpmn_element.attrib and len(bpmn_element.attrib["name"]) > 0
                         else bpmn_element.attrib["id"]
                     )
                     bpmn_graph.add_bpmn_element(
                         bpmn_element.attrib["id"],
-                        ElementInfo(
-                            to_extract[xmlns_key], bpmn_element.attrib["id"], name
-                        ),
+                        ElementInfo(to_extract[xmlns_key], bpmn_element.attrib["id"], name),
                     )
             for flow_arc in process.findall("xmlns:sequenceFlow", bpmn_element_ns):
                 bpmn_graph.add_flow_arc(
                     flow_arc.attrib["id"],
                     flow_arc.attrib["sourceRef"],
                     flow_arc.attrib["targetRef"],
                 )
@@ -150,17 +145,15 @@
         self.element_info[element_id] = element_info
         self.from_name[element_info.name] = element_id
         self.nodes_bitset[element_id] = 1 << len(self.element_info)
 
     def add_flow_arc(self, flow_id, source_id, target_id):
         for node_id in [source_id, target_id]:
             if node_id not in self.element_info:
-                self.element_info[node_id] = ElementInfo(
-                    BPMNNodeType.UNDEFINED, node_id, node_id
-                )
+                self.element_info[node_id] = ElementInfo(BPMNNodeType.UNDEFINED, node_id, node_id)
         self.element_info[source_id].outgoing_flows.append(flow_id)
         self.element_info[target_id].incoming_flows.append(flow_id)
         self.flow_arcs[flow_id] = [source_id, target_id]
         self.arcs_bitset[flow_id] = 1 << len(self.flow_arcs)
 
     def encode_or_join_predecessors(self):
         for e_id in self.element_info:
@@ -174,19 +167,15 @@
                     for flow_id in element.incoming_flows:
                         prev_id = self.flow_arcs[flow_id][0]
                         if self.or_join_pred[e_id][0] & self.nodes_bitset[prev_id] == 0:
                             pred_queue.append(prev_id)
                         self.or_join_pred[e_id][0] |= self.nodes_bitset[prev_id]
                         if self.flow_arcs[flow_id][1] != e_id:
                             self.or_join_pred[e_id][1] |= self.arcs_bitset[flow_id]
-            if (
-                element.type
-                in [BPMNNodeType.EXCLUSIVE_GATEWAY, BPMNNodeType.INCLUSIVE_GATEWAY]
-                and element.is_split()
-            ):
+            if element.type in [BPMNNodeType.EXCLUSIVE_GATEWAY, BPMNNodeType.INCLUSIVE_GATEWAY] and element.is_split():
                 self._find_decision_successors(element)
 
     def _find_decision_successors(self, split_info):
         self.decision_successors[split_info.id] = set()
         visited = {split_info.id}
         suc_queue = deque([split_info])
         while suc_queue:
@@ -201,25 +190,19 @@
                     elif next_info.is_gateway():
                         suc_queue.append(next_info)
 
     def _find_or_conflicting_predecessors(self, or_join_id):
         visited = {or_join_id}
         self.or_join_conflicting_pred[or_join_id] = set()
         for in_flow in self.element_info[or_join_id].incoming_flows:
-            self._dfs_from_or_join(
-                or_join_id, in_flow, self._get_predecessor(in_flow), visited
-            )
+            self._dfs_from_or_join(or_join_id, in_flow, self._get_predecessor(in_flow), visited)
 
     def _dfs_from_or_join(self, or_id, flow_id, e_info, visited):
         visited.add(e_info.id)
-        if (
-            e_info.type
-            in [BPMNNodeType.INCLUSIVE_GATEWAY, BPMNNodeType.EXCLUSIVE_GATEWAY]
-            and e_info.is_split()
-        ):
+        if e_info.type in [BPMNNodeType.INCLUSIVE_GATEWAY, BPMNNodeType.EXCLUSIVE_GATEWAY] and e_info.is_split():
             self.or_join_conflicting_pred[or_id].add(e_info.id)
         for in_flow in e_info.incoming_flows:
             prev_info = self._get_predecessor(in_flow)
             if prev_info.id not in visited and prev_info.is_gateway():
                 self._dfs_from_or_join(or_id, flow_id, prev_info, visited)
 
     def _is_enabled(self, e_id, p_state):
@@ -253,18 +236,15 @@
             else:
                 count_tokens = 0
                 for flow_id in e_info.incoming_flows:
                     if p_state.tokens[flow_id] > 0:
                         count_tokens += 1
                 if count_tokens == len(e_info.incoming_flows):
                     return True
-                if (
-                    count_tokens > 0
-                    and self.or_join_pred[e_id][1] & p_state.state_mask == 0
-                ):
+                if count_tokens > 0 and self.or_join_pred[e_id][1] & p_state.state_mask == 0:
                     return True
                 return False
         return False
 
     def update_process_state(self, e_id, p_state):
         if not self._is_enabled(e_id, p_state):
             return []
@@ -285,17 +265,15 @@
                     if e_info.type in [
                         BPMNNodeType.TASK,
                         BPMNNodeType.PARALLEL_GATEWAY,
                         BPMNNodeType.START_EVENT,
                     ]:
                         f_arcs = copy.deepcopy(e_info.outgoing_flows)
                     elif e_info.type is BPMNNodeType.INCLUSIVE_GATEWAY:
-                        f_arcs = self.element_probability[
-                            e_info.id
-                        ].get_multiple_flows()
+                        f_arcs = self.element_probability[e_info.id].get_multiple_flows()
                 random.shuffle(f_arcs)
             for f_arc in f_arcs:
                 self._find_next(f_arc, p_state, enabled_tasks, to_execute)
             current += 1
         if len(enabled_tasks) > 1:
             random.shuffle(enabled_tasks)
         return enabled_tasks
@@ -363,36 +341,27 @@
                 break
 
         self.check_unfired_or_splits(fired_or_splits, f_arcs_frequency, p_state)
         if post_p:
             self.postprocess_unfired_tasks(task_sequence, fired_tasks, f_arcs_frequency)
         return is_correct, fired_tasks, p_state.pending_tokens()
 
-    def postprocess_unfired_tasks(
-        self, task_sequence: list, fired_tasks: list, f_arcs_frequency: dict
-    ):
+    def postprocess_unfired_tasks(self, task_sequence: list, fired_tasks: list, f_arcs_frequency: dict):
         if self.closest_distance is None:
             self._sort_by_closest_predecesors()
         for i in range(0, len(fired_tasks)):
-            if (
-                not fired_tasks[i]
-                and task_sequence[i] is not None
-                and self.from_name.get(task_sequence[i])
-            ):
+            if not fired_tasks[i] and task_sequence[i] is not None and self.from_name.get(task_sequence[i]):
                 e_info = self.element_info[self.from_name.get(task_sequence[i])]
                 fix_from = [
                     self.starting_event,
                     self.closest_distance[e_info.id][self.starting_event],
                 ]
                 j = i - 1
                 while j >= 0:
-                    if (
-                        task_sequence[j] is None
-                        or self.from_name.get(task_sequence[j]) is None
-                    ):
+                    if task_sequence[j] is None or self.from_name.get(task_sequence[j]) is None:
                         j -= 1
                         continue
                     p_info = self.element_info[self.from_name.get(task_sequence[j])]
                     if (
                         p_info.id in self.closest_distance[e_info.id]
                         and self.closest_distance[e_info.id][p_info.id] < fix_from[1]
                     ):
@@ -400,17 +369,15 @@
                             p_info.id,
                             self.closest_distance[e_info.id][p_info.id],
                         ]
                         if fix_from[1] == 1:
                             break
                     j -= 1
                 if fix_from[0] is not None:
-                    for flow_id in self.decision_flows_sortest_path[e_info.id][
-                        fix_from[0]
-                    ]:
+                    for flow_id in self.decision_flows_sortest_path[e_info.id][fix_from[0]]:
                         if flow_id not in f_arcs_frequency:
                             f_arcs_frequency[flow_id] = 0
                         f_arcs_frequency[flow_id] += 1
 
     def _sort_by_closest_predecesors(self):
         self.closest_distance = dict()
         self.decision_flows_sortest_path = dict()
@@ -444,17 +411,15 @@
                             p_info.type
                             in [
                                 BPMNNodeType.INCLUSIVE_GATEWAY,
                                 BPMNNodeType.EXCLUSIVE_GATEWAY,
                             ]
                             and p_info.is_split()
                         ):
-                            self.decision_flows_sortest_path[e_id][p_id].append(
-                                pred_seq[p_info.id]
-                            )
+                            self.decision_flows_sortest_path[e_id][p_id].append(pred_seq[p_info.id])
                         p_info = self._get_successor(pred_seq[p_info.id])
 
     def try_firing(
         self,
         task_index,
         from_index,
         task_sequence,
@@ -462,20 +427,16 @@
         pending_tasks,
         p_state,
         f_arcs_frequency,
         fired_or_splits,
     ):
         task_info = self.element_info[self.from_name[task_sequence[task_index]]]
         if not p_state.has_token(task_info.incoming_flows[0]):
-            enabled_pred, or_fired, path_decisions = self._find_enabled_predecessors(
-                task_info, p_state
-            )
-            firing_index = self.find_firing_index(
-                task_index, from_index, task_sequence, path_decisions, enabled_pred
-            )
+            enabled_pred, or_fired, path_decisions = self._find_enabled_predecessors(task_info, p_state)
+            firing_index = self.find_firing_index(task_index, from_index, task_sequence, path_decisions, enabled_pred)
             if firing_index == from_index:
                 self._fire_enabled_predecessors(
                     enabled_pred,
                     p_state,
                     or_fired,
                     path_decisions,
                     f_arcs_frequency,
@@ -501,20 +462,16 @@
         fired_or_splits,
     ):
         el_id = self.from_name.get(task_sequence[task_index])
         if el_id is None:
             return
         task_info = self.element_info[el_id]
         if not p_state.has_token(task_info.incoming_flows[0]):
-            enabled_pred, or_fired, path_decisions = self._find_enabled_predecessors(
-                task_info, p_state
-            )
-            firing_index = self.find_firing_index(
-                task_index, from_index, task_sequence, path_decisions, enabled_pred
-            )
+            enabled_pred, or_fired, path_decisions = self._find_enabled_predecessors(task_info, p_state)
+            firing_index = self.find_firing_index(task_index, from_index, task_sequence, path_decisions, enabled_pred)
             if firing_index == from_index:
                 self._fire_enabled_predecessors(
                     enabled_pred,
                     p_state,
                     or_fired,
                     path_decisions,
                     f_arcs_frequency,
@@ -622,20 +579,16 @@
         enabled_pred = deque()
         for i in range(0, max_dist[0] + 1):
             if i in closer_pred[1]:
                 for pred_id in closer_pred[1][i]:
                     enabled_pred.appendleft(pred_id)
         return enabled_pred, closer_pred[2], closer_pred[3]
 
-    def find_firing_index(
-        self, task_index, from_index, task_sequence, path_decisions, enabled_pred
-    ):
-        is_conflicting, conflicting_gateways = self.is_conflicting_task(
-            path_decisions, enabled_pred
-        )
+    def find_firing_index(self, task_index, from_index, task_sequence, path_decisions, enabled_pred):
+        is_conflicting, conflicting_gateways = self.is_conflicting_task(path_decisions, enabled_pred)
         if is_conflicting:
             firing_index = from_index
             for i in range(from_index + 1, len(task_sequence)):
                 if task_sequence[i] != task_sequence[task_index]:
                     for or_id in conflicting_gateways:
                         for split_id in conflicting_gateways[or_id]:
                             t_id = self.from_name[task_sequence[i]]
@@ -644,18 +597,15 @@
             return firing_index
         return from_index
 
     def is_conflicting_task(self, path_decisions, enabled_pred):
         conflicting_gateways = dict()
         is_conflicting = False
         for or_id in path_decisions:
-            if (
-                self.element_info[or_id].type is BPMNNodeType.INCLUSIVE_GATEWAY
-                and self.element_info[or_id].is_join()
-            ):
+            if self.element_info[or_id].type is BPMNNodeType.INCLUSIVE_GATEWAY and self.element_info[or_id].is_join():
                 conflicting_gateways[or_id] = set()
                 for enabled in enabled_pred:
                     e_info = enabled[0]
                     if e_info.id in self.or_join_conflicting_pred[or_id]:
                         conflicting_gateways[or_id].add(e_info.id)
                     if len(conflicting_gateways[or_id]) > 1:
                         is_conflicting = True
@@ -668,17 +618,15 @@
         or_firing,
         path_decisions,
         f_arcs_frequency,
         fired_or_split,
     ):
         visited_elements = set()
         if not enabled_pred:
-            self.try_firing_or_join(
-                enabled_pred, p_state, or_firing, path_decisions, f_arcs_frequency
-            )
+            self.try_firing_or_join(enabled_pred, p_state, or_firing, path_decisions, f_arcs_frequency)
         while enabled_pred:
             [e_info, e_flow] = enabled_pred.popleft()
             if self._is_enabled(e_info.id, p_state):
                 visited_elements.add(e_info.id)
                 if e_info.type is BPMNNodeType.PARALLEL_GATEWAY:
                     for out_flow in e_info.outgoing_flows:
                         self._update_next(
@@ -718,21 +666,17 @@
                                     or_firing,
                                     path_decisions,
                                     f_arcs_frequency,
                                     True,
                                 )
             for in_flow in e_info.incoming_flows:
                 p_state.remove_token(in_flow)
-            self.try_firing_or_join(
-                enabled_pred, p_state, or_firing, path_decisions, f_arcs_frequency
-            )
+            self.try_firing_or_join(enabled_pred, p_state, or_firing, path_decisions, f_arcs_frequency)
 
-    def try_firing_or_join(
-        self, enabled_pred, p_state, or_firing, path_decisions, f_arcs_frequency
-    ):
+    def try_firing_or_join(self, enabled_pred, p_state, or_firing, path_decisions, f_arcs_frequency):
         fired = set()
         or_firing_list = list()
         for or_join_id in or_firing:
             or_firing_list.append(or_join_id)
         for or_join_id in or_firing_list:
             if self._is_enabled(or_join_id, p_state) or not enabled_pred:
                 fired.add(or_join_id)
@@ -776,24 +720,20 @@
         if flow_id not in f_arcs_frequency:
             f_arcs_frequency[flow_id] = 1
         else:
             f_arcs_frequency[flow_id] += 1
         p_state.add_token(flow_id)
         if not from_or:
             next_info = self._get_successor(flow_id)
-            if next_info.type is BPMNNodeType.PARALLEL_GATEWAY and self._is_enabled(
-                next_info.id, p_state
-            ):
+            if next_info.type is BPMNNodeType.PARALLEL_GATEWAY and self._is_enabled(next_info.id, p_state):
                 enabled_pred.appendleft([next_info, None])
             elif next_info.id in path_decisions:
                 if next_info.type is BPMNNodeType.INCLUSIVE_GATEWAY:
                     if next_info.is_split():
-                        enabled_pred.appendleft(
-                            [next_info, path_decisions[next_info.id]]
-                        )
+                        enabled_pred.appendleft([next_info, path_decisions[next_info.id]])
                     else:
                         if next_info.id not in or_firing:
                             or_firing[next_info.id] = 1
                 else:
                     enabled_pred.appendleft([next_info, path_decisions[next_info.id]])
 
     def _get_predecessor(self, flow_id):
@@ -802,115 +742,94 @@
     def _get_successor(self, flow_id):
         return self.element_info[self.flow_arcs[flow_id][1]]
 
     def compute_branching_probability(self, flow_arcs_frequency):
         gateways_branching = dict()
         for e_id in self.element_info:
             if (
-                self.element_info[e_id].type
-                in [BPMNNodeType.EXCLUSIVE_GATEWAY, BPMNNodeType.INCLUSIVE_GATEWAY]
+                self.element_info[e_id].type in [BPMNNodeType.EXCLUSIVE_GATEWAY, BPMNNodeType.INCLUSIVE_GATEWAY]
                 and len(self.element_info[e_id].outgoing_flows) > 1
             ):
                 total_frequency = 0
                 for flow_id in self.element_info[e_id].outgoing_flows:
                     if flow_id not in flow_arcs_frequency:
                         flow_arcs_frequency[flow_id] = 0
                     total_frequency += flow_arcs_frequency[flow_id]
                 flow_arc_probability = dict()
                 for flow_id in self.element_info[e_id].outgoing_flows:
                     flow_arc_probability[flow_id] = (
-                        flow_arcs_frequency[flow_id] / total_frequency
-                        if total_frequency > 0
-                        else 0
+                        flow_arcs_frequency[flow_id] / total_frequency if total_frequency > 0 else 0
                     )
                 gateways_branching[e_id] = flow_arc_probability
         return gateways_branching
 
     def discover_gateway_probabilities(self, flow_arcs_frequency):
         gateways_branching = dict()
         for e_id in self.element_info:
             if (
-                self.element_info[e_id].type
-                in [BPMNNodeType.EXCLUSIVE_GATEWAY, BPMNNodeType.INCLUSIVE_GATEWAY]
+                self.element_info[e_id].type in [BPMNNodeType.EXCLUSIVE_GATEWAY, BPMNNodeType.INCLUSIVE_GATEWAY]
                 and len(self.element_info[e_id].outgoing_flows) > 1
             ):
                 (
                     flow_arcs_probability,
                     total_frequency,
                 ) = self._calculate_arcs_probabilities(e_id, flow_arcs_frequency)
                 # recalculate not only pure zeros, but also low probabilities
                 if min(flow_arcs_probability.values()) <= 0.005:
-                    self._recalculate_arcs_probabilities(
-                        flow_arcs_frequency, flow_arcs_probability, total_frequency
-                    )
+                    self._recalculate_arcs_probabilities(flow_arcs_frequency, flow_arcs_probability, total_frequency)
                 self._check_probabilities(flow_arcs_probability)
                 gateways_branching[e_id] = flow_arcs_probability
         return gateways_branching
 
     def compute_equiprobable_gateway_probabilities(self):
         gateways_branching = dict()
         for e_id in self.element_info:
             if (
-                self.element_info[e_id].type
-                in [BPMNNodeType.EXCLUSIVE_GATEWAY, BPMNNodeType.INCLUSIVE_GATEWAY]
+                self.element_info[e_id].type in [BPMNNodeType.EXCLUSIVE_GATEWAY, BPMNNodeType.INCLUSIVE_GATEWAY]
                 and len(self.element_info[e_id].outgoing_flows) > 1
             ):
                 average_probability = 1.0 / len(self.element_info[e_id].outgoing_flows)
                 probabilities = dict()
                 for flow_id in self.element_info[e_id].outgoing_flows:
                     probabilities[flow_id] = average_probability
                 gateways_branching[e_id] = probabilities
         return gateways_branching
 
     @staticmethod
-    def _recalculate_arcs_probabilities(
-        flow_arcs_frequency, flow_arcs_probability, total_frequency
-    ):
+    def _recalculate_arcs_probabilities(flow_arcs_frequency, flow_arcs_probability, total_frequency):
         # recalculating probabilities because of missing arcs or very small probabilities for them
         arcs_probabilities = np.array(list(flow_arcs_probability.values()))
         valid_probability_threshold = 0.005
         min_probability = 0.01
-        number_of_invalid_arcs = (
-            arcs_probabilities <= valid_probability_threshold
-        ).sum()
+        number_of_invalid_arcs = (arcs_probabilities <= valid_probability_threshold).sum()
         number_of_valid_arcs = len(flow_arcs_probability) - number_of_invalid_arcs
-        if (
-            number_of_valid_arcs == 0
-        ):  # if all arcs are missing, we make the probability equiprobable
+        if number_of_valid_arcs == 0:  # if all arcs are missing, we make the probability equiprobable
             probability = 1.0 / float(number_of_invalid_arcs)
             for flow_id in flow_arcs_probability:
                 flow_arcs_probability[flow_id] = probability
         else:  # otherwise, we set min_probability instead of zero and balance probabilities for valid arcs
-            valid_probabilities = arcs_probabilities[
-                arcs_probabilities > valid_probability_threshold
-            ].sum()
-            extra_probability = (number_of_invalid_arcs * min_probability) - (
-                1.0 - valid_probabilities
-            )
+            valid_probabilities = arcs_probabilities[arcs_probabilities > valid_probability_threshold].sum()
+            extra_probability = (number_of_invalid_arcs * min_probability) - (1.0 - valid_probabilities)
             extra_probability_per_valid_arc = extra_probability / number_of_valid_arcs
             for flow_id in flow_arcs_probability:
                 if flow_arcs_probability[flow_id] <= valid_probability_threshold:
                     # enforcing the minimum possible probability
                     probability = min_probability
                 else:
                     # balancing valid probabilities
-                    probability = (
-                        flow_arcs_probability[flow_id] - extra_probability_per_valid_arc
-                    )
+                    probability = flow_arcs_probability[flow_id] - extra_probability_per_valid_arc
                 flow_arcs_probability[flow_id] = probability
 
     @staticmethod
     def _check_probabilities(flow_arcs_probability):
         # checking probabilities sum up to 1.0
         tolerance = 0.001
         probabilities_sum = sum(flow_arcs_probability.values())
         if 1.0 - probabilities_sum >= tolerance:
-            logger.warning(
-                f"Sum of outgoing flow arcs does not sum up to {1.0 - tolerance}: {probabilities_sum}"
-            )
+            logger.warning(f"Sum of outgoing flow arcs does not sum up to {1.0 - tolerance}: {probabilities_sum}")
 
     def _calculate_arcs_probabilities(self, e_id, flow_arcs_frequency):
         total_frequency = 0
         for flow_id in self.element_info[e_id].outgoing_flows:
             frequency = flow_arcs_frequency.get(flow_id)
             total_frequency += frequency if frequency else 0
         flow_arcs_probability = dict()
```

### Comparing `pix_framework-0.8.9/src/pix_framework/log_ids.py` & `pix_framework-0.9.0/src/pix_framework/log_ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,21 +7,19 @@
     case: str = "case"  # Case ID
     activity: str = "activity"  # Activity label
     resource: str = "resource"  # Resource who performed this activity instance
     start_time: str = "start_time"  # Start time of the activity instance
     end_time: str = "end_time"  # End time of the activity instance
     # Start time estimator
     enabled_time: str = "enabled_time"  # Enablement time of the activity instance
-    enabling_activity: str = (
-        "enabling_activity"  # Label of the activity instance enabling the current one
-    )
-    available_time: str = "available_time"  # Last availability time of the resource who performed this activity instance
-    estimated_start_time: str = (
-        "estimated_start_time"  # Estimated start time of the activity instance
+    enabling_activity: str = "enabling_activity"  # Label of the activity instance enabling the current one
+    available_time: str = (
+        "available_time"  # Last availability time of the resource who performed this activity instance
     )
+    estimated_start_time: str = "estimated_start_time"  # Estimated start time of the activity instance
     batch_id: str = "batch_instance_id"  # ID of the batch instance this activity instance belongs to, if any
     batch_type: str = "batch_instance_type"  # Type of the batch instance this activity instance belongs to, if any
 
     @staticmethod
     def from_dict(config: dict) -> "EventLogIDs":
         return EventLogIDs(**config)
```

### Comparing `pix_framework-0.8.9/src/pix_framework/log_split/log_split.py` & `pix_framework-0.9.0/src/pix_framework/log_split/log_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     training_case_ids = []
     training_full = False
     # Go over the case IDs (sorted by start and end time of its events)
     for case_id in sorted_event_log[log_ids.case].unique():
         # The first traces until the size limit is met goes to the training set
         if not training_full:
             training_case_ids += [case_id]
-            training_full = len(
-                event_log[event_log[log_ids.case].isin(training_case_ids)]
-            ) >= (training_percentage * total_events)
+            training_full = len(event_log[event_log[log_ids.case].isin(training_case_ids)]) >= (
+                training_percentage * total_events
+            )
     # Return the two splits
     return (
         event_log[event_log[log_ids.case].isin(training_case_ids)],
         event_log[~event_log[log_ids.case].isin(training_case_ids)],
     )
 
 
@@ -55,41 +55,27 @@
     :param remove_partial_traces_from_validation    if true, remove from validation set the traces that has been split being some event in
                                                     training and some events in validation.
 
     :return: a tuple with two datasets, the training and the validation ones.
     """
     # Sort if needed
     if sort:
-        keys = (
-            [log_ids.start_time, log_ids.end_time]
-            if log_ids.start_time in event_log.columns
-            else [log_ids.end_time]
-        )
+        keys = [log_ids.start_time, log_ids.end_time] if log_ids.start_time in event_log.columns else [log_ids.end_time]
         sorted_event_log = event_log.sort_values(keys)
     else:
         sorted_event_log = event_log
     # Get the event splitting train and validation
     num_train_events = int(len(event_log) * training_percentage)
     last_training_event = sorted_event_log.head(num_train_events).iloc[-1]
     # Split the log based on the timestamp of the splitting event
     if log_ids.start_time in event_log.columns:
-        training_log = event_log[
-            event_log[log_ids.start_time] <= last_training_event[log_ids.start_time]
-        ]
-        validation_log = event_log[
-            event_log[log_ids.start_time] > last_training_event[log_ids.start_time]
-        ]
+        training_log = event_log[event_log[log_ids.start_time] <= last_training_event[log_ids.start_time]]
+        validation_log = event_log[event_log[log_ids.start_time] > last_training_event[log_ids.start_time]]
     else:
-        training_log = event_log[
-            event_log[log_ids.end_time] <= last_training_event[log_ids.end_time]
-        ]
-        validation_log = event_log[
-            event_log[log_ids.end_time] > last_training_event[log_ids.end_time]
-        ]
+        training_log = event_log[event_log[log_ids.end_time] <= last_training_event[log_ids.end_time]]
+        validation_log = event_log[event_log[log_ids.end_time] > last_training_event[log_ids.end_time]]
     # Remove from validation incomplete traces if needed
     if remove_partial_traces_from_validation:
         training_cases = training_log[log_ids.case].unique()
-        validation_log = validation_log[
-            ~validation_log[log_ids.case].isin(training_cases)
-        ]
+        validation_log = validation_log[~validation_log[log_ids.case].isin(training_cases)]
     # Return the two splits
     return training_log, validation_log
```

### Comparing `pix_framework-0.8.9/src/pix_framework/statistics/utils.py` & `pix_framework-0.9.0/src/pix_framework/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `pix_framework-0.8.9/PKG-INFO` & `pix_framework-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pix-framework
-Version: 0.8.9
+Version: 0.9.0
 Summary: Process Improvement Explorer Framework contains process discovery and improvement modules of the Process Improvement Explorer project.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

