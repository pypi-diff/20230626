# Comparing `tmp/BlaApi-1.4.tar.gz` & `tmp/BlaApi-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\BlaApi-1.4.tar", last modified: Wed Jun  7 22:55:22 2023, max compression
+gzip compressed data, was "BlaApi-1.5.tar", last modified: Mon Jun 26 11:39:50 2023, max compression
```

## Comparing `BlaApi-1.4.tar` & `BlaApi-1.5.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 22:55:22.000000 BlaApi-1.4/
-drwxrwxrwx   0        0        0        0 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi/
--rw-rw-rw-   0        0        0        0 2023-06-07 22:15:05.000000 BlaApi-1.4/BlaApi/__init__.py
--rw-rw-rw-   0        0        0     4024 2023-06-07 22:31:28.000000 BlaApi-1.4/BlaApi/client.py
--rw-rw-rw-   0        0        0     3857 2023-06-07 22:15:05.000000 BlaApi-1.4/BlaApi/diary.py
-drwxrwxrwx   0        0        0        0 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/
--rw-rw-rw-   0        0        0     6133 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 22:55:22.000000 BlaApi-1.4/BlaApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-07 22:15:05.000000 BlaApi-1.4/LICENSE
--rw-rw-rw-   0        0        0     6133 2023-06-07 22:55:22.000000 BlaApi-1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5480 2023-06-07 22:16:04.000000 BlaApi-1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 22:55:22.000000 BlaApi-1.4/setup.cfg
--rw-rw-rw-   0        0        0     3708 2023-06-07 22:42:26.000000 BlaApi-1.4/setup.py
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-06-26 11:39:50.371933 BlaApi-1.5/
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-06-26 11:39:50.367933 BlaApi-1.5/BlaApi/
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       26 2023-06-24 11:54:49.000000 BlaApi-1.5/BlaApi/__init__.py
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     7825 2023-06-26 11:15:42.000000 BlaApi-1.5/BlaApi/client.py
+drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-06-26 11:39:50.370932 BlaApi-1.5/BlaApi.egg-info/
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-06-26 11:39:49.000000 BlaApi-1.5/BlaApi.egg-info/PKG-INFO
+-rw-r--r--   0 muddi     (1000) muddi     (1001)      211 2023-06-26 11:39:50.000000 BlaApi-1.5/BlaApi.egg-info/SOURCES.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)        1 2023-06-26 11:39:49.000000 BlaApi-1.5/BlaApi.egg-info/dependency_links.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       21 2023-06-26 11:39:49.000000 BlaApi-1.5/BlaApi.egg-info/requires.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)        7 2023-06-26 11:39:49.000000 BlaApi-1.5/BlaApi.egg-info/top_level.txt
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     1669 2023-06-22 17:58:15.000000 BlaApi-1.5/LICENSE
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-06-26 11:39:50.370932 BlaApi-1.5/PKG-INFO
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     4851 2023-06-26 11:18:41.000000 BlaApi-1.5/README.md
+-rw-r--r--   0 muddi     (1000) muddi     (1001)       38 2023-06-26 11:39:50.371933 BlaApi-1.5/setup.cfg
+-rw-r--r--   0 muddi     (1000) muddi     (1001)     3583 2023-06-26 11:39:28.000000 BlaApi-1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BlaApi-1.4/BlaApi.egg-info/PKG-INFO` & `BlaApi-1.5/BlaApi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,171 +1,169 @@
-Metadata-Version: 2.1
-Name: BlaApi
-Version: 1.4
-Summary: A wrapper for the beacon light api.
-Home-page: https://github.com/me/myproject
-Author: Omer-Farooqui
-Author-email: deaddogfuneral@gmail.com
-License: BSD-4
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# BLA-API-Wrapper.
-
-## Description
-
-##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
-
-### Table of Contents
-
-- [Installation](#Installation)
-
-
-
-- [Quick-Start](#Quick-Start)
-
-
-
-- [Documentation](#Documentation)
-
-
-
-- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
-
-
-- Useful Links:
-  
-  - [PyPI](https://pypi.org/project/BlaApi/)
-  
-  - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
-
-## Installation
-
-The library is available on [PyPI](https://pypi.org/project/BlaApi/), install using pip.
-
-```shell
-pip install BlaApi
-```
-
-Or update it.
-
-```shell
-pip install BlaApi --upgrade
-```
-
-## Quick Start
-
-The code below returns a list of **'notification_ids'** The date needs to be in the format; **'Abbreviated_Day, DD/MM/YYYY'**
-
-```python
-from BlaApi.diary import Diary
-username = # Bla username
-password = # Bla password
-
-d = Diary(username=username, password=password)
-notification_ids = d.search_by_date("Thu, 13/04/2023")
-print(notification_ids)
-```
-
-###### Output:
-
-```shell
-['3049357', '3049213', '3038795', '3038038', '3036497', '3036305']
-```
-
-We can use **'notification ids'** to make api calls and retrieve useful information.
-
-```python
-#from BlaApi.client import Client
-#c = Client(username, password)
-c = d.client
-diary_data = c.get_diary_data(notification_ids)
-print(diary_data)
-```
-
-The output consists of a list of dictionaries which contain details for the corresponding notification id.
-
-###### Output:
-
-```python
-[{
-        "studentId": "8326",
-        "id": "3049213",
-        "appDiaryId": "64980",
-        "title": "Class work - 13th April",
-        "details": "<p><strong>Book: TBS</strong></p><p><strong>Unit 06: Setting up a company</strong></p><p><strong>Chapter 01: Gathering information</strong></p><p>Chapter completed; discussed all activities. 'Sharpen your skills' also covered. </p><p><br></p>",
-        "bRead": "1",
-        "created": "2023-04-13 10:05:25",
-        "diaryType": "cw",
-        "dateDue": None,
-        "attachment": None,
-        "attachment2": None,
-        "dateSubmitted": None,
-        "subject": "ENGLISH LANGUAGE",
-        "currentTimestamp": "2023-04-15 15:25:21",
-        "assignmentId": "64980",
-        "gr_no": "12266",
-        "comments": [],
-},
-]
-```
-
-*Currently, there is no built-in way to parse this output, but I might add it in the future if needed. Check out some [examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples) or read the [documentation.](#Documentation)*
-
-## Documentation
-
-This is some boilerplate code you should be familiar with.
-
-```python
-from BlaApi.client import Client
-from BlaApi.diary import Diary
-username = #bla username
-password = #bla password
-
-c = Client(username, password)
-d = Diary(username, password)
-```
-
-> Whenever I mention **'Client'**, or **'Diary'**, it means that i'm talking about the files [client.py](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/blob/master/BlaApi/client.py), and [diary.py](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/blob/master/BlaApi/diary.py). Also keep in mind that In the api, the 'notificationId' and 'id' variables are used interchangeably.
-
-The **'login()'** method from **'Client'** allows you to retrieve information such as: auth token, student names, student ids .
-
-The **'get_diary_list()'** method from **'Client'**  will return a list of all the diaries available in the app's database, which allows you to retrieve information such as: date posted, subject name, assignment id, notification id (id), title, description, diary type (cw/hw), if the diary has been read (bRead) and the student id which the diary corresponds to.
-
-The **'get_diary_data()'** method from **'Client'** allows you to get the content of the diary itself, by passing a list of notification ids. it has options such as: student id, app diary id (assignment id), attachment id, comments and the rest is the same as **get_diary_list()**
-
-The **'Diary'** class contains many methods to parse and sort through the diary list, and return notification ids for the entries. The methods inside it also allow you to also pass in a list of notification ids as a second argument using its **'passthru'** variable.
-
-The **'get_current_date()'** method from **'Diary'** returns today's date in a format that the api needs to function. (Abbreviated_Day, DD/MM/YYYY)
-
-The **'search_by_student'** method from **'Diary'** returns the notification_ids for one of the students registered on your account. By default it sets student_number = 0, meaning it will return diaries for the first student by default.
-
-The other methods from **'Diary'** are: **'search_by_date(date)'**, and **'search_been_read(True/False)'**. They are self explanatory.
-
-## To-Do
-
-- [ ] Add some way to parse the diary data
-  
-  - [ ] Comments
-  
-  - [ ] Description
-  
-  - [ ] Attachments
-
-- [ ] Make better doccumentation
-
-### My motivation to create this
-
-Simply put, I found my school's app to be subpar, so I'm attempting to create a better one. *(It's also an excuse to learn new skills)*
-
-
-
-
-Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you want to send hate comments, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you don't 👉👈.
+Metadata-Version: 2.1
+Name: BlaApi
+Version: 1.5
+Summary: A wrapper for the beacon light api.
+Home-page: https://github.com/me/myproject
+Author: Omer-Farooqui
+Author-email: deaddogfuneral@gmail.com
+License: BSD-4
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# BLA-API-Wrapper.
+
+## Description
+
+##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
+
+### Table of Contents
+
+- [Installation](#Installation)
+
+
+
+- [Quick-Start](#Quick-Start)
+
+
+
+- [Documentation](#Documentation)
+
+
+
+- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
+
+
+- Useful Links:
+  
+  - [PyPI](https://pypi.org/project/BlaApi/)
+  
+  - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
+
+## Installation
+
+The library is available on [PyPI](https://pypi.org/project/BlaApi/), install using pip.
+
+```shell
+pip install BlaApi
+```
+
+Or update it.
+
+```shell
+pip install BlaApi --upgrade
+```
+
+## Quick Start
+
+The code below returns a list of **'notification_ids'** The date needs to be in the format; **'Abbreviated_Day, DD/MM/YYYY'**
+
+```python
+from BlaApi import Client
+username = 'my username'
+password = 'my password'
+
+notification_ids = c.search_by_date("Thu, 13/04/2023")
+print(notification_ids)
+```
+
+###### Output:
+
+```shell
+['3049357', '3049213', '3038795', '3038038', '3036497', '3036305']
+```
+
+We can use **'notification ids'** to make api calls and retrieve useful information.
+
+```python
+from BlaApi import Client
+c = Client(username, password)
+diary_data = c.get_diary_data(notification_ids)
+print(diary_data)
+```
+
+The output consists of a list of dictionaries which contain details for the corresponding notification id.
+
+###### Output:
+
+```python
+[{
+        "studentId": "8326",
+        "id": "3049213",
+        "appDiaryId": "64980",
+        "title": "Class work - 13th April",
+        "details": "<p><strong>Book: TBS</strong></p><p><strong>Unit 06: Setting up a company</strong></p><p><strong>Chapter 01: Gathering information</strong></p><p>Chapter completed; discussed all activities. 'Sharpen your skills' also covered. </p><p><br></p>",
+        "bRead": "1",
+        "created": "2023-04-13 10:05:25",
+        "diaryType": "cw",
+        "dateDue": None,
+        "attachment": None,
+        "attachment2": None,
+        "dateSubmitted": None,
+        "subject": "ENGLISH LANGUAGE",
+        "currentTimestamp": "2023-04-15 15:25:21",
+        "assignmentId": "64980",
+        "gr_no": "12266",
+        "comments": [],
+},
+]
+```
+
+*Currently, there is no built-in way to parse this output, but I might add it in the future if needed. Check out some [examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples) or read the [documentation.](#Documentation)*
+
+## Documentation
+
+This is some boilerplate code you should be familiar with.
+
+```python
+from BlaApi import Client
+username = 'my username'
+password = 'my password'
+
+c = Client(username, password)
+```
+
+> Keep in mind that In the api, the 'notificationId' and 'id' variables are used interchangeably.
+
+The **'login()'** method allows you to retrieve information such as: auth token and student information such as class, section student_name, gr_number, student_id.
+
+The **'get_diary_list()'** method will return a list of all the diaries available in the app's database, which allows you to retrieve information such as: date posted, subject name, assignment id, notification id (id), title, description, diary type (cw/hw), if the diary has been read (bRead) and the student id which the diary corresponds to.
+
+The **'get_diary_data()'** method allows you to get the content of the diary itself, by passing a list of notification ids. it has options such as: student id, app diary id (assignment id), attachment id, comments and the rest is the same as **get_diary_list()**
+
+The there are methods to parse and sort through the diary list, and return notification ids for the entries. The methods inside it also allow you to also pass in a list of notification ids as a second argument using its **'passthru'** variable.
+
+The **'get_current_date()'** method from **'Diary'** returns today's date in a format that the api needs to function. (Abbreviated_Day, DD/MM/YYYY)
+
+The **'search_by_student'** method from **'Diary'** returns the notification_ids for one of the students registered on your account. By default it sets student_number = 0, meaning it will return diaries for the first student by default.
+
+The other methods from **'Diary'** are: **'search_by_date(date)'**, and **'search_been_read(True/False)'**. They are self explanatory.
+
+## To-Do
+
+- [ ] Add methods for interacting with more features
+  
+  - [ ] Comments
+  
+  - [ ] Description
+
+  - [ ] Student info
+  
+  - [ ] Attachments
+
+- [ ] Make better doccumentation
+
+### My motivation to create this
+
+Simply put, I found my school's app to be subpar, so I'm attempting to create a better one.
+
+
+
+
+Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you have any questions, and star the [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you're cool
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `BlaApi-1.4/PKG-INFO` & `BlaApi-1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,171 +1,169 @@
-Metadata-Version: 2.1
-Name: BlaApi
-Version: 1.4
-Summary: A wrapper for the beacon light api.
-Home-page: https://github.com/me/myproject
-Author: Omer-Farooqui
-Author-email: deaddogfuneral@gmail.com
-License: BSD-4
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# BLA-API-Wrapper.
-
-## Description
-
-##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
-
-### Table of Contents
-
-- [Installation](#Installation)
-
-
-
-- [Quick-Start](#Quick-Start)
-
-
-
-- [Documentation](#Documentation)
-
-
-
-- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
-
-
-- Useful Links:
-  
-  - [PyPI](https://pypi.org/project/BlaApi/)
-  
-  - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
-
-## Installation
-
-The library is available on [PyPI](https://pypi.org/project/BlaApi/), install using pip.
-
-```shell
-pip install BlaApi
-```
-
-Or update it.
-
-```shell
-pip install BlaApi --upgrade
-```
-
-## Quick Start
-
-The code below returns a list of **'notification_ids'** The date needs to be in the format; **'Abbreviated_Day, DD/MM/YYYY'**
-
-```python
-from BlaApi.diary import Diary
-username = # Bla username
-password = # Bla password
-
-d = Diary(username=username, password=password)
-notification_ids = d.search_by_date("Thu, 13/04/2023")
-print(notification_ids)
-```
-
-###### Output:
-
-```shell
-['3049357', '3049213', '3038795', '3038038', '3036497', '3036305']
-```
-
-We can use **'notification ids'** to make api calls and retrieve useful information.
-
-```python
-#from BlaApi.client import Client
-#c = Client(username, password)
-c = d.client
-diary_data = c.get_diary_data(notification_ids)
-print(diary_data)
-```
-
-The output consists of a list of dictionaries which contain details for the corresponding notification id.
-
-###### Output:
-
-```python
-[{
-        "studentId": "8326",
-        "id": "3049213",
-        "appDiaryId": "64980",
-        "title": "Class work - 13th April",
-        "details": "<p><strong>Book: TBS</strong></p><p><strong>Unit 06: Setting up a company</strong></p><p><strong>Chapter 01: Gathering information</strong></p><p>Chapter completed; discussed all activities. 'Sharpen your skills' also covered. </p><p><br></p>",
-        "bRead": "1",
-        "created": "2023-04-13 10:05:25",
-        "diaryType": "cw",
-        "dateDue": None,
-        "attachment": None,
-        "attachment2": None,
-        "dateSubmitted": None,
-        "subject": "ENGLISH LANGUAGE",
-        "currentTimestamp": "2023-04-15 15:25:21",
-        "assignmentId": "64980",
-        "gr_no": "12266",
-        "comments": [],
-},
-]
-```
-
-*Currently, there is no built-in way to parse this output, but I might add it in the future if needed. Check out some [examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples) or read the [documentation.](#Documentation)*
-
-## Documentation
-
-This is some boilerplate code you should be familiar with.
-
-```python
-from BlaApi.client import Client
-from BlaApi.diary import Diary
-username = #bla username
-password = #bla password
-
-c = Client(username, password)
-d = Diary(username, password)
-```
-
-> Whenever I mention **'Client'**, or **'Diary'**, it means that i'm talking about the files [client.py](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/blob/master/BlaApi/client.py), and [diary.py](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/blob/master/BlaApi/diary.py). Also keep in mind that In the api, the 'notificationId' and 'id' variables are used interchangeably.
-
-The **'login()'** method from **'Client'** allows you to retrieve information such as: auth token, student names, student ids .
-
-The **'get_diary_list()'** method from **'Client'**  will return a list of all the diaries available in the app's database, which allows you to retrieve information such as: date posted, subject name, assignment id, notification id (id), title, description, diary type (cw/hw), if the diary has been read (bRead) and the student id which the diary corresponds to.
-
-The **'get_diary_data()'** method from **'Client'** allows you to get the content of the diary itself, by passing a list of notification ids. it has options such as: student id, app diary id (assignment id), attachment id, comments and the rest is the same as **get_diary_list()**
-
-The **'Diary'** class contains many methods to parse and sort through the diary list, and return notification ids for the entries. The methods inside it also allow you to also pass in a list of notification ids as a second argument using its **'passthru'** variable.
-
-The **'get_current_date()'** method from **'Diary'** returns today's date in a format that the api needs to function. (Abbreviated_Day, DD/MM/YYYY)
-
-The **'search_by_student'** method from **'Diary'** returns the notification_ids for one of the students registered on your account. By default it sets student_number = 0, meaning it will return diaries for the first student by default.
-
-The other methods from **'Diary'** are: **'search_by_date(date)'**, and **'search_been_read(True/False)'**. They are self explanatory.
-
-## To-Do
-
-- [ ] Add some way to parse the diary data
-  
-  - [ ] Comments
-  
-  - [ ] Description
-  
-  - [ ] Attachments
-
-- [ ] Make better doccumentation
-
-### My motivation to create this
-
-Simply put, I found my school's app to be subpar, so I'm attempting to create a better one. *(It's also an excuse to learn new skills)*
-
-
-
-
-Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you want to send hate comments, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you don't 👉👈.
+Metadata-Version: 2.1
+Name: BlaApi
+Version: 1.5
+Summary: A wrapper for the beacon light api.
+Home-page: https://github.com/me/myproject
+Author: Omer-Farooqui
+Author-email: deaddogfuneral@gmail.com
+License: BSD-4
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=3.7.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# BLA-API-Wrapper.
+
+## Description
+
+##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
+
+### Table of Contents
+
+- [Installation](#Installation)
+
+
+
+- [Quick-Start](#Quick-Start)
+
+
+
+- [Documentation](#Documentation)
+
+
+
+- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
+
+
+- Useful Links:
+  
+  - [PyPI](https://pypi.org/project/BlaApi/)
+  
+  - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
+
+## Installation
+
+The library is available on [PyPI](https://pypi.org/project/BlaApi/), install using pip.
+
+```shell
+pip install BlaApi
+```
+
+Or update it.
+
+```shell
+pip install BlaApi --upgrade
+```
+
+## Quick Start
+
+The code below returns a list of **'notification_ids'** The date needs to be in the format; **'Abbreviated_Day, DD/MM/YYYY'**
+
+```python
+from BlaApi import Client
+username = 'my username'
+password = 'my password'
+
+notification_ids = c.search_by_date("Thu, 13/04/2023")
+print(notification_ids)
+```
+
+###### Output:
+
+```shell
+['3049357', '3049213', '3038795', '3038038', '3036497', '3036305']
+```
+
+We can use **'notification ids'** to make api calls and retrieve useful information.
+
+```python
+from BlaApi import Client
+c = Client(username, password)
+diary_data = c.get_diary_data(notification_ids)
+print(diary_data)
+```
+
+The output consists of a list of dictionaries which contain details for the corresponding notification id.
+
+###### Output:
+
+```python
+[{
+        "studentId": "8326",
+        "id": "3049213",
+        "appDiaryId": "64980",
+        "title": "Class work - 13th April",
+        "details": "<p><strong>Book: TBS</strong></p><p><strong>Unit 06: Setting up a company</strong></p><p><strong>Chapter 01: Gathering information</strong></p><p>Chapter completed; discussed all activities. 'Sharpen your skills' also covered. </p><p><br></p>",
+        "bRead": "1",
+        "created": "2023-04-13 10:05:25",
+        "diaryType": "cw",
+        "dateDue": None,
+        "attachment": None,
+        "attachment2": None,
+        "dateSubmitted": None,
+        "subject": "ENGLISH LANGUAGE",
+        "currentTimestamp": "2023-04-15 15:25:21",
+        "assignmentId": "64980",
+        "gr_no": "12266",
+        "comments": [],
+},
+]
+```
+
+*Currently, there is no built-in way to parse this output, but I might add it in the future if needed. Check out some [examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples) or read the [documentation.](#Documentation)*
+
+## Documentation
+
+This is some boilerplate code you should be familiar with.
+
+```python
+from BlaApi import Client
+username = 'my username'
+password = 'my password'
+
+c = Client(username, password)
+```
+
+> Keep in mind that In the api, the 'notificationId' and 'id' variables are used interchangeably.
+
+The **'login()'** method allows you to retrieve information such as: auth token and student information such as class, section student_name, gr_number, student_id.
+
+The **'get_diary_list()'** method will return a list of all the diaries available in the app's database, which allows you to retrieve information such as: date posted, subject name, assignment id, notification id (id), title, description, diary type (cw/hw), if the diary has been read (bRead) and the student id which the diary corresponds to.
+
+The **'get_diary_data()'** method allows you to get the content of the diary itself, by passing a list of notification ids. it has options such as: student id, app diary id (assignment id), attachment id, comments and the rest is the same as **get_diary_list()**
+
+The there are methods to parse and sort through the diary list, and return notification ids for the entries. The methods inside it also allow you to also pass in a list of notification ids as a second argument using its **'passthru'** variable.
+
+The **'get_current_date()'** method from **'Diary'** returns today's date in a format that the api needs to function. (Abbreviated_Day, DD/MM/YYYY)
+
+The **'search_by_student'** method from **'Diary'** returns the notification_ids for one of the students registered on your account. By default it sets student_number = 0, meaning it will return diaries for the first student by default.
+
+The other methods from **'Diary'** are: **'search_by_date(date)'**, and **'search_been_read(True/False)'**. They are self explanatory.
+
+## To-Do
+
+- [ ] Add methods for interacting with more features
+  
+  - [ ] Comments
+  
+  - [ ] Description
+
+  - [ ] Student info
+  
+  - [ ] Attachments
+
+- [ ] Make better doccumentation
+
+### My motivation to create this
+
+Simply put, I found my school's app to be subpar, so I'm attempting to create a better one.
+
+
+
+
+Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you have any questions, and star the [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you're cool
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `BlaApi-1.4/README.md` & `BlaApi-1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,152 +1,150 @@
-# BLA-API-Wrapper.
-
-## Description
-
-##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
-
-### Table of Contents
-
-- [Installation](#Installation)
-
-
-
-- [Quick-Start](#Quick-Start)
-
-
-
-- [Documentation](#Documentation)
-
-
-
-- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
-
-
-- Useful Links:
-  
-  - [PyPI](https://pypi.org/project/BlaApi/)
-  
-  - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
-
-## Installation
-
-The library is available on [PyPI](https://pypi.org/project/BlaApi/), install using pip.
-
-```shell
-pip install BlaApi
-```
-
-Or update it.
-
-```shell
-pip install BlaApi --upgrade
-```
-
-## Quick Start
-
-The code below returns a list of **'notification_ids'** The date needs to be in the format; **'Abbreviated_Day, DD/MM/YYYY'**
-
-```python
-from BlaApi.diary import Diary
-username = # Bla username
-password = # Bla password
-
-d = Diary(username=username, password=password)
-notification_ids = d.search_by_date("Thu, 13/04/2023")
-print(notification_ids)
-```
-
-###### Output:
-
-```shell
-['3049357', '3049213', '3038795', '3038038', '3036497', '3036305']
-```
-
-We can use **'notification ids'** to make api calls and retrieve useful information.
-
-```python
-#from BlaApi.client import Client
-#c = Client(username, password)
-c = d.client
-diary_data = c.get_diary_data(notification_ids)
-print(diary_data)
-```
-
-The output consists of a list of dictionaries which contain details for the corresponding notification id.
-
-###### Output:
-
-```python
-[{
-        "studentId": "8326",
-        "id": "3049213",
-        "appDiaryId": "64980",
-        "title": "Class work - 13th April",
-        "details": "<p><strong>Book: TBS</strong></p><p><strong>Unit 06: Setting up a company</strong></p><p><strong>Chapter 01: Gathering information</strong></p><p>Chapter completed; discussed all activities. 'Sharpen your skills' also covered. </p><p><br></p>",
-        "bRead": "1",
-        "created": "2023-04-13 10:05:25",
-        "diaryType": "cw",
-        "dateDue": None,
-        "attachment": None,
-        "attachment2": None,
-        "dateSubmitted": None,
-        "subject": "ENGLISH LANGUAGE",
-        "currentTimestamp": "2023-04-15 15:25:21",
-        "assignmentId": "64980",
-        "gr_no": "12266",
-        "comments": [],
-},
-]
-```
-
-*Currently, there is no built-in way to parse this output, but I might add it in the future if needed. Check out some [examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples) or read the [documentation.](#Documentation)*
-
-## Documentation
-
-This is some boilerplate code you should be familiar with.
-
-```python
-from BlaApi.client import Client
-from BlaApi.diary import Diary
-username = #bla username
-password = #bla password
-
-c = Client(username, password)
-d = Diary(username, password)
-```
-
-> Whenever I mention **'Client'**, or **'Diary'**, it means that i'm talking about the files [client.py](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/blob/master/BlaApi/client.py), and [diary.py](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/blob/master/BlaApi/diary.py). Also keep in mind that In the api, the 'notificationId' and 'id' variables are used interchangeably.
-
-The **'login()'** method from **'Client'** allows you to retrieve information such as: auth token, student names, student ids .
-
-The **'get_diary_list()'** method from **'Client'**  will return a list of all the diaries available in the app's database, which allows you to retrieve information such as: date posted, subject name, assignment id, notification id (id), title, description, diary type (cw/hw), if the diary has been read (bRead) and the student id which the diary corresponds to.
-
-The **'get_diary_data()'** method from **'Client'** allows you to get the content of the diary itself, by passing a list of notification ids. it has options such as: student id, app diary id (assignment id), attachment id, comments and the rest is the same as **get_diary_list()**
-
-The **'Diary'** class contains many methods to parse and sort through the diary list, and return notification ids for the entries. The methods inside it also allow you to also pass in a list of notification ids as a second argument using its **'passthru'** variable.
-
-The **'get_current_date()'** method from **'Diary'** returns today's date in a format that the api needs to function. (Abbreviated_Day, DD/MM/YYYY)
-
-The **'search_by_student'** method from **'Diary'** returns the notification_ids for one of the students registered on your account. By default it sets student_number = 0, meaning it will return diaries for the first student by default.
-
-The other methods from **'Diary'** are: **'search_by_date(date)'**, and **'search_been_read(True/False)'**. They are self explanatory.
-
-## To-Do
-
-- [ ] Add some way to parse the diary data
-  
-  - [ ] Comments
-  
-  - [ ] Description
-  
-  - [ ] Attachments
-
-- [ ] Make better doccumentation
-
-### My motivation to create this
-
-Simply put, I found my school's app to be subpar, so I'm attempting to create a better one. *(It's also an excuse to learn new skills)*
-
-
-
-
-Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you want to send hate comments, and star my [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you don't 👉👈.
+# BLA-API-Wrapper.
+
+## Description
+
+##### Reverse engineering of [Beacon Light Academy's Homework App.](https://beaconlightacademy.edu.pk/app/)
+
+### Table of Contents
+
+- [Installation](#Installation)
+
+
+
+- [Quick-Start](#Quick-Start)
+
+
+
+- [Documentation](#Documentation)
+
+
+
+- [Examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples)
+
+
+- Useful Links:
+  
+  - [PyPI](https://pypi.org/project/BlaApi/)
+  
+  - [Github Repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper)
+
+## Installation
+
+The library is available on [PyPI](https://pypi.org/project/BlaApi/), install using pip.
+
+```shell
+pip install BlaApi
+```
+
+Or update it.
+
+```shell
+pip install BlaApi --upgrade
+```
+
+## Quick Start
+
+The code below returns a list of **'notification_ids'** The date needs to be in the format; **'Abbreviated_Day, DD/MM/YYYY'**
+
+```python
+from BlaApi import Client
+username = 'my username'
+password = 'my password'
+
+notification_ids = c.search_by_date("Thu, 13/04/2023")
+print(notification_ids)
+```
+
+###### Output:
+
+```shell
+['3049357', '3049213', '3038795', '3038038', '3036497', '3036305']
+```
+
+We can use **'notification ids'** to make api calls and retrieve useful information.
+
+```python
+from BlaApi import Client
+c = Client(username, password)
+diary_data = c.get_diary_data(notification_ids)
+print(diary_data)
+```
+
+The output consists of a list of dictionaries which contain details for the corresponding notification id.
+
+###### Output:
+
+```python
+[{
+        "studentId": "8326",
+        "id": "3049213",
+        "appDiaryId": "64980",
+        "title": "Class work - 13th April",
+        "details": "<p><strong>Book: TBS</strong></p><p><strong>Unit 06: Setting up a company</strong></p><p><strong>Chapter 01: Gathering information</strong></p><p>Chapter completed; discussed all activities. 'Sharpen your skills' also covered. </p><p><br></p>",
+        "bRead": "1",
+        "created": "2023-04-13 10:05:25",
+        "diaryType": "cw",
+        "dateDue": None,
+        "attachment": None,
+        "attachment2": None,
+        "dateSubmitted": None,
+        "subject": "ENGLISH LANGUAGE",
+        "currentTimestamp": "2023-04-15 15:25:21",
+        "assignmentId": "64980",
+        "gr_no": "12266",
+        "comments": [],
+},
+]
+```
+
+*Currently, there is no built-in way to parse this output, but I might add it in the future if needed. Check out some [examples](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/tree/master/examples) or read the [documentation.](#Documentation)*
+
+## Documentation
+
+This is some boilerplate code you should be familiar with.
+
+```python
+from BlaApi import Client
+username = 'my username'
+password = 'my password'
+
+c = Client(username, password)
+```
+
+> Keep in mind that In the api, the 'notificationId' and 'id' variables are used interchangeably.
+
+The **'login()'** method allows you to retrieve information such as: auth token and student information such as class, section student_name, gr_number, student_id.
+
+The **'get_diary_list()'** method will return a list of all the diaries available in the app's database, which allows you to retrieve information such as: date posted, subject name, assignment id, notification id (id), title, description, diary type (cw/hw), if the diary has been read (bRead) and the student id which the diary corresponds to.
+
+The **'get_diary_data()'** method allows you to get the content of the diary itself, by passing a list of notification ids. it has options such as: student id, app diary id (assignment id), attachment id, comments and the rest is the same as **get_diary_list()**
+
+The there are methods to parse and sort through the diary list, and return notification ids for the entries. The methods inside it also allow you to also pass in a list of notification ids as a second argument using its **'passthru'** variable.
+
+The **'get_current_date()'** method from **'Diary'** returns today's date in a format that the api needs to function. (Abbreviated_Day, DD/MM/YYYY)
+
+The **'search_by_student'** method from **'Diary'** returns the notification_ids for one of the students registered on your account. By default it sets student_number = 0, meaning it will return diaries for the first student by default.
+
+The other methods from **'Diary'** are: **'search_by_date(date)'**, and **'search_been_read(True/False)'**. They are self explanatory.
+
+## To-Do
+
+- [ ] Add methods for interacting with more features
+  
+  - [ ] Comments
+  
+  - [ ] Description
+
+  - [ ] Student info
+  
+  - [ ] Attachments
+
+- [ ] Make better doccumentation
+
+### My motivation to create this
+
+Simply put, I found my school's app to be subpar, so I'm attempting to create a better one.
+
+
+
+
+Feel free to open an [issue](https://github.com/Omer-Farooqui/BLA-Api-Wrapper/issues) if you have any questions, and star the [repo](https://github.com/Omer-Farooqui/BLA-Api-Wrapper) if you're cool
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `BlaApi-1.4/setup.py` & `BlaApi-1.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = 'BlaApi'
-DESCRIPTION = 'A wrapper for the beacon light api.'
-URL = 'https://github.com/me/myproject'
-EMAIL = 'deaddogfuneral@gmail.com'
-AUTHOR = 'Omer-Farooqui'
-REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.4'
-
-# What packages are required for this module to be executed?
-REQUIRED = [
-     'httpx', 'fake_useragent',
-]
-
-# What packages are optional?
-EXTRAS = {
-    # 'fancy feature': ['django'],
-}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, '__version__.py')) as f:
-        exec(f.read(), about)
-else:
-    about['__version__'] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = 'Build and publish the package.'
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print('\033[1m{0}\033[0m'.format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status('Removing previous builds…')
-            rmtree(os.path.join(here, 'dist'))
-        except OSError:
-            pass
-
-        self.status('Building Source and Wheel (universal) distribution…')
-        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
-
-        self.status('Uploading the package to PyPI via Twine…')
-        os.system('twine upload dist/*')
-
-        self.status('Pushing git tags…')
-        os.system('git tag v{0}'.format(about['__version__']))
-        os.system('git push --tags')
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about['__version__'],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(),
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['mypackage'],
-
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license='BSD-4',
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy'
-    ],
-    # $ setup.py publish support.
-    cmdclass={
-        'upload': UploadCommand,
-    },
-)
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = 'BlaApi'
+DESCRIPTION = 'A wrapper for the beacon light api.'
+URL = 'https://github.com/me/myproject'
+EMAIL = 'deaddogfuneral@gmail.com'
+AUTHOR = 'Omer-Farooqui'
+REQUIRES_PYTHON = '>=3.7.0'
+VERSION = '1.5'
+
+# What packages are required for this module to be executed?
+REQUIRED = [
+     'httpx', 'fake_useragent',
+]
+
+# What packages are optional?
+EXTRAS = {
+    # 'fancy feature': ['django'],
+}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, '__version__.py')) as f:
+        exec(f.read(), about)
+else:
+    about['__version__'] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = 'Build and publish the package.'
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print('\033[1m{0}\033[0m'.format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status('Removing previous builds…')
+            rmtree(os.path.join(here, 'dist'))
+        except OSError:
+            pass
+
+        self.status('Building Source and Wheel (universal) distribution…')
+        os.system('{0} setup.py sdist bdist_wheel --universal'.format(sys.executable))
+
+        self.status('Uploading the package to PyPI via Twine…')
+        os.system('twine upload dist/*')
+
+        self.status('Pushing git tags…')
+        os.system('git tag v{0}'.format(about['__version__']))
+        os.system('git push --tags')
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about['__version__'],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(),
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['mypackage'],
+
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license='BSD-4',
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        'License :: OSI Approved :: BSD License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy'
+    ],
+    # $ setup.py publish support.
+    cmdclass={
+        'upload': UploadCommand,
+    },
+)
```

