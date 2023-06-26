# Comparing `tmp/aiogram3b8_calendar-0.0.1.tar.gz` & `tmp/aiogram3b8_calendar-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3b8_calendar-0.0.1.tar", last modified: Mon Jun 19 12:33:30 2023, max compression
+gzip compressed data, was "aiogram3b8_calendar-0.0.2.tar", last modified: Mon Jun 26 15:56:52 2023, max compression
```

## Comparing `aiogram3b8_calendar-0.0.1.tar` & `aiogram3b8_calendar-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 12:33:30.263634 aiogram3b8_calendar-0.0.1/
--rw-rw-rw-   0        0        0     1076 2023-06-19 08:09:16.000000 aiogram3b8_calendar-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1795 2023-06-19 12:33:30.264632 aiogram3b8_calendar-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-06-19 12:29:05.000000 aiogram3b8_calendar-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 12:33:29.567387 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar/
--rw-rw-rw-   0        0        0      222 2023-06-19 11:51:04.000000 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar/__init__.py
--rw-rw-rw-   0        0        0     5638 2023-06-19 10:16:37.000000 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar/dialog_calendar.py
--rw-rw-rw-   0        0        0     5619 2023-06-19 10:09:43.000000 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar/simple_calendar.py
-drwxrwxrwx   0        0        0        0 2023-06-19 12:33:30.261636 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-06-19 12:33:28.000000 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-06-19 12:33:28.000000 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 12:33:28.000000 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-19 12:33:28.000000 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-19 12:33:28.000000 aiogram3b8_calendar-0.0.1/aiogram3b8_calendar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 12:33:30.708200 aiogram3b8_calendar-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1103 2023-06-19 12:24:45.000000 aiogram3b8_calendar-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:56:52.643751 aiogram3b8_calendar-0.0.2/
+-rw-rw-rw-   0        0        0     1076 2023-06-26 09:06:42.000000 aiogram3b8_calendar-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1795 2023-06-26 15:56:52.680429 aiogram3b8_calendar-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-06-26 09:06:42.000000 aiogram3b8_calendar-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 15:56:52.390451 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar/
+-rw-rw-rw-   0        0        0      222 2023-06-26 15:09:48.000000 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar/__init__.py
+-rw-rw-rw-   0        0        0     5870 2023-06-26 15:51:37.000000 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar/dialog_calendar.py
+-rw-rw-rw-   0        0        0     5482 2023-06-26 15:51:31.000000 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar/simple_calendar.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:56:52.624747 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-06-26 15:56:47.000000 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-06-26 15:56:47.000000 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:56:47.000000 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-26 15:56:47.000000 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-26 15:56:47.000000 aiogram3b8_calendar-0.0.2/aiogram3b8_calendar.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-26 15:56:52.710426 aiogram3b8_calendar-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1103 2023-06-26 14:14:27.000000 aiogram3b8_calendar-0.0.2/setup.py
```

### Comparing `aiogram3b8_calendar-0.0.1/LICENSE.txt` & `aiogram3b8_calendar-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiogram3b8_calendar-0.0.1/PKG-INFO` & `aiogram3b8_calendar-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3b8_calendar
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Inline Calendar & Date Selection tool for Aiogram Telegram bots
 Home-page: https://github.com/yoworu/aiogram3.0.0b8_calendar/
 Download-URL: https://github.com/yoworu/aiogram3.0.0b8_calendar.git
 Author: Andrew Nikolabay
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,Calendar
```

### Comparing `aiogram3b8_calendar-0.0.1/README.md` & `aiogram3b8_calendar-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3b8_calendar-0.0.1/aiogram3b8_calendar/dialog_calendar.py` & `aiogram3b8_calendar-0.0.2/aiogram3b8_calendar/dialog_calendar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import calendar
-from datetime import datetime
+from datetime import date
+
 
 from aiogram.types import InlineKeyboardMarkup, InlineKeyboardButton
 from aiogram.filters.callback_data import CallbackData
 from aiogram.types import CallbackQuery
 from aiogram.utils.keyboard import InlineKeyboardBuilder
 
 
@@ -16,21 +17,18 @@
 
 ignore_callback = CalendarCallback(act="IGNORE", year=-1, month=-1, day=-1).pack()  # for buttons with no answer
 
 
 class DialogCalendar:
     months = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"]
 
-    def __init__(self, year: int = datetime.now().year, month: int = datetime.now().month):
-        self.year = year
-        self.month = month
-
-    async def start_calendar(
-        self,
-        year: int = datetime.now().year
+
+    @staticmethod
+    def start_calendar(
+        year: int = date.today().year
     ) -> InlineKeyboardMarkup:
         inline_kb = InlineKeyboardBuilder()
         
         # first row - years
         years = []
         for value in range(year - 2, year + 3):
             years.append(InlineKeyboardButton(
@@ -49,53 +47,55 @@
                 callback_data=CalendarCallback(act="NEXT-YEARS", year=year, month=-1, day=-1).pack()
             ),
             width=2
         )
 
         return inline_kb.as_markup()
 
-    async def _get_month_kb(self, year: int):
+    @classmethod
+    def _get_month_kb(cls, year: int):
         inline_kb = InlineKeyboardBuilder()
         
         # first row with year button
         inline_kb.row(
             InlineKeyboardButton(text=" ", callback_data=ignore_callback),
             InlineKeyboardButton(
                 text=year,
                 callback_data=CalendarCallback(act="START", year=year, month=-1, day=-1).pack()
             ),
             InlineKeyboardButton(text=" ", callback_data=ignore_callback)
         )
         # two rows with 6 months buttons
         months_1 = []
-        for month in self.months[0:6]:
+        for month in cls.months[0:6]:
             months_1.append(InlineKeyboardButton(
                 text=month,
-                callback_data=CalendarCallback(act="SET-MONTH", year=year, month=self.months.index(month)+1, day=-1).pack()
+                callback_data=CalendarCallback(act="SET-MONTH", year=year, month=cls.months.index(month)+1, day=-1).pack()
             ))
         inline_kb.row(*months_1, width=6)
         months_2 = []
-        for month in self.months[6:12]:
+        for month in cls.months[6:12]:
             months_2.append(InlineKeyboardButton(
                 text=month,
-                callback_data=CalendarCallback(act="SET-MONTH", year=year, month=self.months.index(month)+1, day=-1).pack()
+                callback_data=CalendarCallback(act="SET-MONTH", year=year, month=cls.months.index(month)+1, day=-1).pack()
             ))
         inline_kb.row(*months_2, width=6)
         return inline_kb.as_markup()
 
-    async def _get_days_kb(self, year: int, month: int):
+    @classmethod
+    def _get_days_kb(cls, year: int, month: int):
         inline_kb = InlineKeyboardBuilder()
         
         inline_kb.row(
             InlineKeyboardButton(
                 text=year,
                 callback_data=CalendarCallback(act="START", year=year, month=-1, day=-1).pack()
             ),
             InlineKeyboardButton(
-                text=self.months[month - 1],
+                text=cls.months[month - 1],
                 callback_data=CalendarCallback(act="SET-YEAR", year=year, month=-1, day=-1).pack()
             ),
         )
         days = []
         for day in ["Mo", "Tu", "We", "Th", "Fr", "Sa", "Su"]:
             days.append(InlineKeyboardButton(text=day, callback_data=ignore_callback))
         inline_kb.row(*days, width=7)
@@ -108,27 +108,35 @@
                     continue
                 days.append(InlineKeyboardButton(
                     text=str(day), callback_data=CalendarCallback(act="SET-DAY", year=year, month=month, day=day).pack()
                 ))
             inline_kb.row(*days, width=7)
         return inline_kb.as_markup()
 
-    async def process_selection(self, query: CallbackQuery, data: CalendarCallback) -> tuple:
-        return_data = (False, None)
+    @classmethod
+    async def process_selection(cls, query: CallbackQuery, data: CalendarCallback) -> date | None:
+        """
+        Process the callback_query. This method generates a new calendar if forward or
+        backward is pressed. This method should be called inside a CallbackQueryHandler.
+        :param query: callback_query, as provided by the CallbackQueryHandler
+        :param data: callback_data, dictionary, set by calendar_callback
+        :return: Returns a date or None.
+        """
+        return_data = None
         if data.act == "IGNORE":
             await query.answer(cache_time=60)
         if data.act == "SET-YEAR":
-            await query.message.edit_reply_markup(reply_markup=await self._get_month_kb(int(data.year)))
+            await query.message.edit_reply_markup(reply_markup=cls._get_month_kb(int(data.year)))
         if data.act == "PREV-YEARS":
             new_year = int(data.year) - 5
-            await query.message.edit_reply_markup(reply_markup=await self.start_calendar(new_year))
+            await query.message.edit_reply_markup(reply_markup=cls.start_calendar(new_year))
         if data.act == "NEXT-YEARS":
             new_year = int(data.year) + 5
-            await query.message.edit_reply_markup(reply_markup=await self.start_calendar(new_year))
+            await query.message.edit_reply_markup(reply_markup=cls.start_calendar(new_year))
         if data.act == "START":
-            await query.message.edit_reply_markup(reply_markup=await self.start_calendar(int(data.year)))
+            await query.message.edit_reply_markup(reply_markup=cls.start_calendar(int(data.year)))
         if data.act == "SET-MONTH":
-            await query.message.edit_reply_markup(reply_markup=await self._get_days_kb(int(data.year), int(data.month)))
+            await query.message.edit_reply_markup(reply_markup=cls._get_days_kb(int(data.year), int(data.month)))
         if data.act == "SET-DAY":
             await query.message.delete_reply_markup()   # removing inline keyboard
-            return_data = True, datetime(int(data.year), int(data.month), int(data.day))
+            return_data = date(int(data.year), int(data.month), int(data.day))
         return return_data
```

### Comparing `aiogram3b8_calendar-0.0.1/aiogram3b8_calendar/simple_calendar.py` & `aiogram3b8_calendar-0.0.2/aiogram3b8_calendar/simple_calendar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import calendar
-from datetime import datetime, timedelta
+from datetime import timedelta, date
+
 
 from aiogram.types import InlineKeyboardMarkup, InlineKeyboardButton
 from aiogram.filters.callback_data import CallbackData
 from aiogram.types import CallbackQuery
 from aiogram.utils.keyboard import InlineKeyboardBuilder
 
-
 # setting callback_data prefix and parts
 class CalendarCallback(CallbackData, prefix='simple_calendar'):
     act: str
     year: int
     month: int
     day: int
     
 
 class SimpleCalendar:
 
-    async def start_calendar(
-        self,
-        year: int = datetime.now().year,
-        month: int = datetime.now().month
+    @staticmethod
+    def start_calendar(
+        year: int = date.today().year,
+        month: int = date.today().month
     ) -> InlineKeyboardMarkup:
         """
         Creates an inline keyboard with the provided year and month
         :param int year: Year to use in the calendar, if None the current year is used.
         :param int month: Month to use in the calendar, if None the current month is used.
         :return: Returns InlineKeyboardMarkup object with the calendar.
         """
@@ -54,15 +54,15 @@
         inline_kb.row(*second_row, width=7)
         
         # Calendar rows - Days of month
         month_calendar = calendar.monthcalendar(year, month)
         for week in month_calendar:
             calendar_rows = []
             for day in week:
-                if (day == 0):
+                if (day == 0): 
                     calendar_rows.append(InlineKeyboardButton(text=" ", callback_data=ignore_callback))
                     continue
                 calendar_rows.append(InlineKeyboardButton(
                     text=str(day), callback_data=CalendarCallback(act="DAY", year=year, month=month, day=day).pack()
                 ))
             inline_kb.row(*calendar_rows, width=7)
 
@@ -74,44 +74,44 @@
             InlineKeyboardButton(text=" ", callback_data=ignore_callback),
             InlineKeyboardButton(
                 text=">", callback_data=CalendarCallback(act="NEXT-MONTH", year=year, month=month, day=day).pack()
             )
         )
 
         return inline_kb.as_markup()
-
-    async def process_selection(self, query: CallbackQuery, data: CalendarCallback) -> tuple:
+    
+    @classmethod
+    async def process_selection(cls, query: CallbackQuery, data: CalendarCallback) -> date | None:
         """
         Process the callback_query. This method generates a new calendar if forward or
         backward is pressed. This method should be called inside a CallbackQueryHandler.
         :param query: callback_query, as provided by the CallbackQueryHandler
         :param data: callback_data, dictionary, set by calendar_callback
-        :return: Returns a tuple (Boolean,datetime), indicating if a date is selected
-                    and returning the date if so.
+        :return: Returns a date or None.
         """
-        return_data = (False, None)
-        temp_date = datetime(int(data.year), int(data.month), 1)
+        return_data = None
+        temp_date = date(int(data.year), int(data.month), 1)
         # processing empty buttons, answering with no action
         if data.act == "IGNORE":
             await query.answer(cache_time=60)
         # user picked a day button, return date
         if data.act == "DAY":
             await query.message.delete_reply_markup()   # removing inline keyboard
-            return_data = True, datetime(int(data.year), int(data.month), int(data.day))
+            return_data = date(int(data.year), int(data.month), int(data.day))
         # user navigates to previous year, editing message with new calendar
         if data.act == "PREV-YEAR":
-            prev_date = datetime(int(data.year) - 1, int(data.month), 1)
-            await query.message.edit_reply_markup(reply_markup=await self.start_calendar(int(prev_date.year), int(prev_date.month)))
+            prev_date = date(int(data.year) - 1, int(data.month), 1)
+            await query.message.edit_reply_markup(reply_markup=cls.start_calendar(int(prev_date.year), int(prev_date.month)))
         # user navigates to next year, editing message with new calendar
         if data.act == "NEXT-YEAR":
-            next_date = datetime(int(data.year) + 1, int(data.month), 1)
-            await query.message.edit_reply_markup(reply_markup=await self.start_calendar(int(next_date.year), int(next_date.month)))
+            next_date = date(int(data.year) + 1, int(data.month), 1)
+            await query.message.edit_reply_markup(reply_markup=cls.start_calendar(int(next_date.year), int(next_date.month)))
         # user navigates to previous month, editing message with new calendar
         if data.act == "PREV-MONTH":
             prev_date = temp_date - timedelta(days=1)
-            await query.message.edit_reply_markup(reply_markup=await self.start_calendar(int(prev_date.year), int(prev_date.month)))
+            await query.message.edit_reply_markup(reply_markup=cls.start_calendar(int(prev_date.year), int(prev_date.month)))
         # user navigates to next month, editing message with new calendar
         if data.act == "NEXT-MONTH":
             next_date = temp_date + timedelta(days=31)
-            await query.message.edit_reply_markup(reply_markup=await self.start_calendar(int(next_date.year), int(next_date.month)))
+            await query.message.edit_reply_markup(reply_markup=cls.start_calendar(int(next_date.year), int(next_date.month)))
         # at some point user clicks DAY button, returning date
         return return_data
```

### Comparing `aiogram3b8_calendar-0.0.1/aiogram3b8_calendar.egg-info/PKG-INFO` & `aiogram3b8_calendar-0.0.2/aiogram3b8_calendar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3b8-calendar
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Inline Calendar & Date Selection tool for Aiogram Telegram bots
 Home-page: https://github.com/yoworu/aiogram3.0.0b8_calendar/
 Download-URL: https://github.com/yoworu/aiogram3.0.0b8_calendar.git
 Author: Andrew Nikolabay
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,Calendar
```

### Comparing `aiogram3b8_calendar-0.0.1/setup.py` & `aiogram3b8_calendar-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
   name='aiogram3b8_calendar',
   packages=['aiogram3b8_calendar'],
-  version='0.0.1',
+  version='0.0.2',
   license='MIT',
   description='Simple Inline Calendar & Date Selection tool for Aiogram Telegram bots',
   long_description=long_description,
   author='Andrew Nikolabay',
   author_email='',
   url='https://github.com/yoworu/aiogram3.0.0b8_calendar/',
   download_url='https://github.com/yoworu/aiogram3.0.0b8_calendar.git',
```

