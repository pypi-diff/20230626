# Comparing `tmp/mighty_logger-0.6.1.tar.gz` & `tmp/mighty_logger-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mighty_logger-0.6.1.tar", last modified: Sun Jun 18 13:45:38 2023, max compression
+gzip compressed data, was "mighty_logger-0.7.0.tar", last modified: Mon Jun 26 14:26:27 2023, max compression
```

## Comparing `mighty_logger-0.6.1.tar` & `mighty_logger-0.7.0.tar`

### file list

```diff
@@ -1,34 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.626365 mighty_logger-0.6.1/
--rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.6.1/LICENSE
--rw-rw-rw-   0        0        0    10797 2023-06-18 13:45:38.645888 mighty_logger-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     9824 2023-06-18 13:24:38.000000 mighty_logger-0.6.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.537706 mighty_logger-0.6.1/mighty_logger/
--rw-rw-rw-   0        0        0      823 2023-06-18 13:45:30.000000 mighty_logger-0.6.1/mighty_logger/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.582361 mighty_logger-0.6.1/mighty_logger/basic/
--rw-rw-rw-   0        0        0      857 2023-04-11 08:43:49.000000 mighty_logger-0.6.1/mighty_logger/basic/__init__.py
--rw-rw-rw-   0        0        0     5371 2023-06-12 12:55:27.000000 mighty_logger-0.6.1/mighty_logger/basic/basic_logger.py
--rw-rw-rw-   0        0        0     1325 2023-04-12 11:19:28.000000 mighty_logger-0.6.1/mighty_logger/basic/exceptions.py
--rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.6.1/mighty_logger/basic/patterns.py
--rw-rw-rw-   0        0        0     4009 2023-06-12 12:55:27.000000 mighty_logger-0.6.1/mighty_logger/basic/text_buffer_type.py
--rw-rw-rw-   0        0        0    80755 2023-06-18 13:42:58.000000 mighty_logger-0.6.1/mighty_logger/powerful_logger.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.604562 mighty_logger-0.6.1/mighty_logger/src/
--rw-rw-rw-   0        0        0      943 2023-06-11 13:34:59.000000 mighty_logger-0.6.1/mighty_logger/src/__init__.py
--rw-rw-rw-   0        0        0     4572 2023-06-11 16:58:31.000000 mighty_logger-0.6.1/mighty_logger/src/ansi_format.py
--rw-rw-rw-   0        0        0     8659 2023-06-11 16:58:31.000000 mighty_logger-0.6.1/mighty_logger/src/color_picker.py
--rw-rw-rw-   0        0        0     1376 2023-06-18 11:06:25.000000 mighty_logger-0.6.1/mighty_logger/src/log_enums.py
--rw-rw-rw-   0        0        0     5647 2023-06-11 16:58:31.000000 mighty_logger-0.6.1/mighty_logger/src/status_variables.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.615562 mighty_logger-0.6.1/mighty_logger/text/
--rw-rw-rw-   0        0        0      853 2023-06-10 14:12:03.000000 mighty_logger-0.6.1/mighty_logger/text/__init__.py
--rw-rw-rw-   0        0        0    10316 2023-06-18 13:17:24.000000 mighty_logger-0.6.1/mighty_logger/text/animation.py
--rw-rw-rw-   0        0        0     3180 2023-06-18 10:25:46.000000 mighty_logger-0.6.1/mighty_logger/text/icon_set.py
--rw-rw-rw-   0        0        0     6042 2023-06-17 14:04:56.000000 mighty_logger-0.6.1/mighty_logger/text/text_buffer.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.542708 mighty_logger-0.6.1/mighty_logger.egg-info/
--rw-rw-rw-   0        0        0    10797 2023-06-18 13:45:38.000000 mighty_logger-0.6.1/mighty_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      750 2023-06-18 13:45:38.000000 mighty_logger-0.6.1/mighty_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 13:45:38.000000 mighty_logger-0.6.1/mighty_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-18 13:45:38.000000 mighty_logger-0.6.1/mighty_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 13:45:38.646888 mighty_logger-0.6.1/setup.cfg
--rw-rw-rw-   0        0        0     2796 2023-06-18 13:45:30.000000 mighty_logger-0.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 13:45:38.625364 mighty_logger-0.6.1/test/
--rw-rw-rw-   0        0        0     2483 2023-06-18 13:19:47.000000 mighty_logger-0.6.1/test/test_console.py
--rw-rw-rw-   0        0        0     2508 2023-06-18 11:18:04.000000 mighty_logger-0.6.1/test/test_html.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:26:27.352771 mighty_logger-0.7.0/
+-rw-rw-rw-   0        0        0    11357 2023-04-10 16:24:05.000000 mighty_logger-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0    10783 2023-06-26 14:26:27.352771 mighty_logger-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9841 2023-06-26 14:22:34.000000 mighty_logger-0.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 14:26:27.267418 mighty_logger-0.7.0/mighty_logger/
+-rw-rw-rw-   0        0        0      863 2023-06-24 13:25:16.000000 mighty_logger-0.7.0/mighty_logger/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:26:27.300465 mighty_logger-0.7.0/mighty_logger/basic/
+-rw-rw-rw-   0        0        0      789 2023-06-26 10:51:25.000000 mighty_logger-0.7.0/mighty_logger/basic/__init__.py
+-rw-rw-rw-   0        0        0     8304 2023-06-25 13:09:47.000000 mighty_logger-0.7.0/mighty_logger/basic/basic_logger.py
+-rw-rw-rw-   0        0        0     1499 2023-06-26 10:49:56.000000 mighty_logger-0.7.0/mighty_logger/basic/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:26:27.319235 mighty_logger-0.7.0/mighty_logger/basic/lib_types/
+-rw-rw-rw-   0        0        0      875 2023-06-25 13:20:13.000000 mighty_logger-0.7.0/mighty_logger/basic/lib_types/__init__.py
+-rw-rw-rw-   0        0        0     1086 2023-06-25 13:07:43.000000 mighty_logger-0.7.0/mighty_logger/basic/lib_types/animation_type.py
+-rw-rw-rw-   0        0        0     1848 2023-06-25 13:06:36.000000 mighty_logger-0.7.0/mighty_logger/basic/lib_types/entry_type.py
+-rw-rw-rw-   0        0        0     1297 2023-06-26 11:32:43.000000 mighty_logger-0.7.0/mighty_logger/basic/lib_types/environment_type.py
+-rw-rw-rw-   0        0        0      874 2023-06-25 13:06:36.000000 mighty_logger-0.7.0/mighty_logger/basic/lib_types/status_message_type.py
+-rw-rw-rw-   0        0        0     4317 2023-06-26 11:33:46.000000 mighty_logger-0.7.0/mighty_logger/basic/lib_types/text_buffer_type.py
+-rw-rw-rw-   0        0        0      823 2023-04-11 10:58:04.000000 mighty_logger-0.7.0/mighty_logger/basic/patterns.py
+-rw-rw-rw-   0        0        0    27826 2023-06-26 11:10:15.000000 mighty_logger-0.7.0/mighty_logger/powerful_logger.py
+-rw-rw-rw-   0        0        0     7054 2023-06-26 11:10:15.000000 mighty_logger-0.7.0/mighty_logger/simple_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:26:27.348772 mighty_logger-0.7.0/mighty_logger/src/
+-rw-rw-rw-   0        0        0     1110 2023-06-24 13:02:04.000000 mighty_logger-0.7.0/mighty_logger/src/__init__.py
+-rw-rw-rw-   0        0        0     9975 2023-06-25 13:20:13.000000 mighty_logger-0.7.0/mighty_logger/src/animation.py
+-rw-rw-rw-   0        0        0     4572 2023-06-11 16:58:31.000000 mighty_logger-0.7.0/mighty_logger/src/ansi_format.py
+-rw-rw-rw-   0        0        0     8659 2023-06-11 16:58:31.000000 mighty_logger-0.7.0/mighty_logger/src/color_picker.py
+-rw-rw-rw-   0        0        0    38487 2023-06-25 13:20:13.000000 mighty_logger-0.7.0/mighty_logger/src/entry_types.py
+-rw-rw-rw-   0        0        0     1140 2023-06-25 13:20:13.000000 mighty_logger-0.7.0/mighty_logger/src/environments.py
+-rw-rw-rw-   0        0        0     5473 2023-06-25 13:20:13.000000 mighty_logger-0.7.0/mighty_logger/src/status_variables.py
+-rw-rw-rw-   0        0        0    10787 2023-06-26 11:01:56.000000 mighty_logger-0.7.0/mighty_logger/src/text_buffer.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:26:27.272243 mighty_logger-0.7.0/mighty_logger.egg-info/
+-rw-rw-rw-   0        0        0    10783 2023-06-26 14:26:27.000000 mighty_logger-0.7.0/mighty_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      994 2023-06-26 14:26:27.000000 mighty_logger-0.7.0/mighty_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 14:26:27.000000 mighty_logger-0.7.0/mighty_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-26 14:26:27.000000 mighty_logger-0.7.0/mighty_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 14:26:27.353772 mighty_logger-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1707 2023-06-25 13:24:09.000000 mighty_logger-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 14:26:27.350771 mighty_logger-0.7.0/test/
+-rw-rw-rw-   0        0        0     2626 2023-06-25 14:48:08.000000 mighty_logger-0.7.0/test/test.py
+-rw-rw-rw-   0        0        0      837 2023-06-26 10:38:49.000000 mighty_logger-0.7.0/test/test_simple.py
```

### Comparing `mighty_logger-0.6.1/LICENSE` & `mighty_logger-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.1/PKG-INFO` & `mighty_logger-0.7.0/mighty_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: mighty_logger
-Version: 0.6.1
-Summary: Powerful functional logger with support for qt programming
+Name: mighty-logger
+Version: 0.7.0
+Summary: Powerful functional logger
 Home-page: https://github.com/Nakama3942/mighty_logger
 Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -103,17 +103,16 @@
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
-- [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
-- [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
-- [ ] v0.7.2 - Search update (added search by log entry types)
+- [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
+- [ ] v0.7.1 - Search update (added search by log entry types)
 - [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
 - [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
@@ -147,14 +146,16 @@
 
 ```sh
 pip install mighty_logger
 ```
 
 ## Usage
 
+ATTENTION!!! OUTDATED MATERIAL! RELEVANCE - v0.6.1! WILL BE OVERWRITTEN IN v0.9.1!
+
 This is the simplest example of using the library:
 
 ```python
 from mighty_logger import Logger
 from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
```

### Comparing `mighty_logger-0.6.1/README.md` & `mighty_logger-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,17 +84,16 @@
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
-- [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
-- [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
-- [ ] v0.7.2 - Search update (added search by log entry types)
+- [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
+- [ ] v0.7.1 - Search update (added search by log entry types)
 - [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
 - [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
@@ -128,14 +127,16 @@
 
 ```sh
 pip install mighty_logger
 ```
 
 ## Usage
 
+ATTENTION!!! OUTDATED MATERIAL! RELEVANCE - v0.6.1! WILL BE OVERWRITTEN IN v0.9.1!
+
 This is the simplest example of using the library:
 
 ```python
 from mighty_logger import Logger
 from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
```

### Comparing `mighty_logger-0.6.1/mighty_logger/__init__.py` & `mighty_logger-0.7.0/mighty_logger/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,11 +13,12 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from .powerful_logger import Logger
+from .simple_logger import SimpleLogger
 
 __authot__ = "Kalynovsky 'Nakamura Akira' Valentin"
-__version__ = "0.6.1"
+__version__ = "0.7.0"
 __email__ = "nakama3942@gmail.com"
```

### Comparing `mighty_logger-0.6.1/mighty_logger/basic/exceptions.py` & `mighty_logger-0.7.0/mighty_logger/basic/exceptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,26 +22,36 @@
 	"""
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
 
-class CombinationException(BaseException):
+class ReCreationException(BaseException):
 	"""
-	An exception that is thrown when composing impossible combinations of boolean flags.
+	The exception that is thrown when an object of the Singleton class is re-created.
 	"""
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
 
-class ReCreationException(BaseException):
+class EnvironmentException(BaseException):
 	"""
-	The exception that is thrown when an object of the Singleton class is re-created.
+	The exception that is thrown when on environmental errors.
+	"""
+	def __init__(self, message):
+		self.message = message
+
+	def __str__(self):
+		return self.message
+
+class InitException(BaseException):
+	"""
+	The exception thrown on errors during initialization.
 	"""
 	def __init__(self, message):
 		self.message = message
 
 	def __str__(self):
 		return self.message
```

### Comparing `mighty_logger-0.6.1/mighty_logger/basic/patterns.py` & `mighty_logger-0.7.0/mighty_logger/basic/patterns.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.1/mighty_logger/basic/text_buffer_type.py` & `mighty_logger-0.7.0/mighty_logger/basic/lib_types/text_buffer_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,111 +12,122 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-from abc import ABC, abstractmethod
+from mighty_logger.basic.lib_types.environment_type import EnvironmentType
 
-class TextBufferType(ABC):
-	def __init__(self) -> None:
+class TextBufferType:
+	def __init__(self, env: EnvironmentType) -> None:
 		self._text_buffer: list[str] = []
+		self._environment: EnvironmentType = env
 
 	def __lshift__(self, entry: str) -> None:
 		"""
 		Used to add a string to the end of the buffer.
 
 		:param entry: The line to be added
 		"""
-		self.append(f"{entry}")
+		self.append(entry)
 
 	def __rshift__(self, entry: str) -> None:
 		"""
 		Used to save a buffer to the file.
 
 		:param entry: The name of the file where you want to save the buffer
 		"""
-		self.save(entry)
+		self.save(entry, True)
 
 	def get_data(self) -> list:
 		"""
 		Returns a list of strings from a text buffer.
 
 		:return: a list of text buffer lines
 		"""
 		return self._text_buffer
 
-	@abstractmethod
 	def append(self, message: str) -> None:
 		"""
 		Adds a string to the end of the text buffer.
 
 		:param message: The string to be added to the buffer
 		"""
 		raise NotImplementedError("Method append() is not implemented in the base class.")
 
-	@abstractmethod
 	def insert(self, number_string: int, message: str) -> None:
 		"""
 		Adds a string to the middle of the text buffer at the specified position.
 
 		:param number_string: Position (number) of the line to which you need to add a string
 		:param message: The string to be placed on the position
 		"""
 		raise NotImplementedError("Method insert() is not implemented in the base class.")
 
-	@abstractmethod
 	def replace(self, number_string: int, message: str) -> None:
 		"""
 		Replaces a specific string in a text buffer. If there is no such string, the method
 		fills the list with empty strings up to the required position and *adds* the string.
 
 		:param number_string: Position (number) of the string to be replaced (added)
 		:param message: A string that will replace the previous one by position
 		"""
 		raise NotImplementedError("Method replace() is not implemented in the base class.")
 
-	@abstractmethod
 	def pop(self, number_string: int = -1) -> str:
 		"""
 		Removes and returns the specified string from the buffer.
 
 		:param number_string: The string to be removed from the buffer
 		"""
-		raise NotImplementedError("Method remove() is not implemented in the base class.")
+		raise NotImplementedError("Method pop() is not implemented in the base class.")
 
-	@abstractmethod
 	def remove(self, number_string: int = -1) -> None:
 		"""
 		Deletes without returning the specified string from the buffer.
 
 		:param number_string: The string to be removed from the buffer
 		"""
 		raise NotImplementedError("Method remove() is not implemented in the base class.")
 
-	@abstractmethod
-	def save(self, name_file: str = "buffer", clean: bool = True) -> None:
+	def clear(self) -> None:
+		"""
+		...
+		"""
+		raise NotImplementedError("Method clear() is not implemented in the base class.")
+
+	def save(self, name_file: str, clean: bool) -> None:
 		"""
 		Saves the text of the buffer to a file.
 
 		:param name_file: The name of the file where the buffer will be saved
 		:param clean: Saving should be done in Plain text?
 		"""
 		raise NotImplementedError("Method save() is not implemented in the base class.")
 
-	@abstractmethod
+	def load(self, name_file: str) -> None:
+		"""
+		...
+		"""
+		raise NotImplementedError("Method load() is not implemented in the base class.")
+
+	def input(self, input_text: str) -> str:
+		"""
+		...
+
+		:param input_text:
+		"""
+		raise NotImplementedError("Method input() is not implemented in the base class.")
+
 	def update_console(self) -> None:
 		"""
 		Refreshes the console, erasing output text and outputting an updated buffer.
 		"""
 		raise NotImplementedError("Method update_console() is not implemented in the base class.")
 
-	@abstractmethod
 	def update_entry(self) -> None:
 		"""
 		Rewrites the last line of output after updating the last line of the buffer.
 		Used (mostly) by the Progress bar (that is Progress string).
 		"""
 		raise NotImplementedError("Method update_entry() is not implemented in the base class.")
-
-	# todo v0.7.0 abstractmethod remove(), clear(), -open_save() or load()-
```

### Comparing `mighty_logger-0.6.1/mighty_logger/src/__init__.py` & `mighty_logger-0.7.0/mighty_logger/src/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
+from .animation import IndefiniteAnimations, DefiniteAnimations
 from .ansi_format import GetAnsiFormat
 from .color_picker import DecColor,\
 	HexColor,\
 	AnsiColor,\
 	Dec2Hex,\
 	Dec2Ansi,\
 	Hex2Dec,\
 	Hex2Ansi,\
 	Ansi2Dec,\
 	Ansi2Hex
-from .log_enums import LogEnvironments, TypesEntries
+from .entry_types import LoggerEntryTypes, ProcessEntryTypes
+from .environments import LogEnvironments
 from .status_variables import StatusMessagePatterns
+from .text_buffer import BasicTextBuffer, TextBuffer
```

### Comparing `mighty_logger-0.6.1/mighty_logger/src/ansi_format.py` & `mighty_logger-0.7.0/mighty_logger/src/ansi_format.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.1/mighty_logger/src/color_picker.py` & `mighty_logger-0.7.0/mighty_logger/src/color_picker.py`

 * *Files identical despite different names*

### Comparing `mighty_logger-0.6.1/mighty_logger/src/status_variables.py` & `mighty_logger-0.7.0/mighty_logger/src/status_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-class StatusMessageType:
-	"""
-	Wrapper class for status message.
-	"""
-	def __init__(self, message: str):
-		self.__current_status_message: str = message
-
-	@property
-	def current_status_message(self) -> str:
-		return self.__current_status_message
+from mighty_logger.basic.lib_types.status_message_type import StatusMessageType
 
 class StatusMessagePatterns:
 	"""
 	A class that emits the desired status message templates.
 	"""
 	@staticmethod
 	def completed() -> StatusMessageType:
```

### Comparing `mighty_logger-0.6.1/mighty_logger/text/__init__.py` & `mighty_logger-0.7.0/mighty_logger/basic/lib_types/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-"""
-A package with the implementation of text formats.
-\n
-Copyright © 2023 Kalynovsky Valentin. All rights reserved.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
-"""
-
-from .animation import IndefiniteAnimations, DefiniteAnimations
-from .icon_set import IconSetType, EmptyIconSet, IconSet1, IconSet2, IconSet3, IconSet4
-from .text_buffer import BasicTextBuffer, TextBuffer
+"""
+...
+\n
+Copyright © 2023 Kalynovsky Valentin. All rights reserved.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+from .animation_type import IndefiniteAnimationType, DefiniteAnimationType
+from .entry_type import EntryType
+from .environment_type import EnvironmentType
+from .status_message_type import StatusMessageType
+from .text_buffer_type import TextBufferType
```

### Comparing `mighty_logger-0.6.1/mighty_logger/text/animation.py` & `mighty_logger-0.7.0/mighty_logger/src/animation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,15 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
-class BasicAnimationType:
-	"""
-	Basic wrapper class for animations type.
-	"""
-	def __init__(self, animation: list):
-		self.__animation: list = animation
-
-	@property
-	def animation(self) -> list:
-		return self.__animation
-
-class IndefiniteAnimationType(BasicAnimationType):
-	"""
-	Wrapper class for indefinite animations type.
-	"""
-	...
-
-class DefiniteAnimationType(BasicAnimationType):
-	"""
-	Wrapper class for definite animations type.
-	"""
-	...
+from mighty_logger.basic.lib_types.animation_type import IndefiniteAnimationType, DefiniteAnimationType
 
 class IndefiniteAnimations:
 	"""
 	The class with sets indefinite animations.
 	"""
 	Dots = IndefiniteAnimationType([
 		'.       ',
```

### Comparing `mighty_logger-0.6.1/mighty_logger.egg-info/PKG-INFO` & `mighty_logger-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: mighty-logger
-Version: 0.6.1
-Summary: Powerful functional logger with support for qt programming
+Name: mighty_logger
+Version: 0.7.0
+Summary: Powerful functional logger
 Home-page: https://github.com/Nakama3942/mighty_logger
 Author: Kalynovsky 'Nakamura Akira' Valentin
 Author-email: nakama3942@gmail.com
 License: Apache License, Version 2.0, see LICENSE file
 Project-URL: Releases, https://github.com/Nakama3942/mighty_logger/releases
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -103,17 +103,16 @@
 - [x] v0.2.0 - Structural update (added basic console logger with HTML base)
 - [x] v0.3.0 - Background update (added background for log entries)
 - [x] v0.4.0 - Buffer update (added text buffer)
 - [x] v0.5.0 - Unifying update (console and HTML are combined into one class)
 - [x] v0.5.1 - Hints update (added status message templates and hint symbols (icons) near log entries status)
 - [x] v0.6.0 - Progress update (added start of some log entries in threads (process))
 - [x] v0.6.1 - Animation update (added animations in processes)
-- [ ] v0.7.0 - "Buffer improvement" update (added buffer clearing and loading)
-- [ ] v0.7.1 - Conversion update (added conversion from Console type to HTML and vice versa)
-- [ ] v0.7.2 - Search update (added search by log entry types)
+- [x] v0.7.0 - "Buffer improvement" update (buffer development completed and entry type system reworked)
+- [ ] v0.7.1 - Search update (added search by log entry types)
 - [ ] v0.8.0 - Export update (added conversion to different types, such as csv, pdf, etc.)
 - [ ] v0.9.0 - Extension update (made wheel format and instruction of toml)
 - [ ] v0.9.1 - Documenting update (all updates since v0.7.0 are documented; updated old documentation; documentation site generation added)
 - [ ] v1.0.0 - Completion of logger development (logger development completed)
 - [ ] v1.1.0 - Font update (added a class that formats text outside the logger)
 
 </details>
@@ -147,14 +146,16 @@
 
 ```sh
 pip install mighty_logger
 ```
 
 ## Usage
 
+ATTENTION!!! OUTDATED MATERIAL! RELEVANCE - v0.6.1! WILL BE OVERWRITTEN IN v0.9.1!
+
 This is the simplest example of using the library:
 
 ```python
 from mighty_logger import Logger
 from mighty_logger.src import StatusMessagePatterns
 
 if __name__ == "__main__":
```

### Comparing `mighty_logger-0.6.1/mighty_logger.egg-info/SOURCES.txt` & `mighty_logger-0.7.0/mighty_logger.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 mighty_logger/__init__.py
 mighty_logger/powerful_logger.py
+mighty_logger/simple_logger.py
 mighty_logger.egg-info/PKG-INFO
 mighty_logger.egg-info/SOURCES.txt
 mighty_logger.egg-info/dependency_links.txt
 mighty_logger.egg-info/top_level.txt
 mighty_logger/basic/__init__.py
 mighty_logger/basic/basic_logger.py
 mighty_logger/basic/exceptions.py
 mighty_logger/basic/patterns.py
-mighty_logger/basic/text_buffer_type.py
+mighty_logger/basic/lib_types/__init__.py
+mighty_logger/basic/lib_types/animation_type.py
+mighty_logger/basic/lib_types/entry_type.py
+mighty_logger/basic/lib_types/environment_type.py
+mighty_logger/basic/lib_types/status_message_type.py
+mighty_logger/basic/lib_types/text_buffer_type.py
 mighty_logger/src/__init__.py
+mighty_logger/src/animation.py
 mighty_logger/src/ansi_format.py
 mighty_logger/src/color_picker.py
-mighty_logger/src/log_enums.py
+mighty_logger/src/entry_types.py
+mighty_logger/src/environments.py
 mighty_logger/src/status_variables.py
-mighty_logger/text/__init__.py
-mighty_logger/text/animation.py
-mighty_logger/text/icon_set.py
-mighty_logger/text/text_buffer.py
-test/test_console.py
-test/test_html.py
+mighty_logger/src/text_buffer.py
+test/test.py
+test/test_simple.py
```

### Comparing `mighty_logger-0.6.1/test/test_console.py` & `mighty_logger-0.7.0/test/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from time import sleep
 
 from mighty_logger import Logger
-from mighty_logger.src import TypesEntries
-from mighty_logger.text import IndefiniteAnimations, DefiniteAnimations
+from mighty_logger.src import LoggerEntryTypes, ProcessEntryTypes, LogEnvironments, IndefiniteAnimations, DefiniteAnimations
 
 if __name__ == "__main__":
-	logger = Logger(program_name="Installer", console_width=115, status_message_global_entry=False)
+	logger = Logger(program_name="Installer", log_environment=LogEnvironments.CONSOLE, console_width=115, status_message_global_entry=False)
+	logger.publish_author()
 
-	logger.message(message_text="Program installation started")
 	logger.start_timer(message_text="Timer started")
+	logger.entry(entry_type=LoggerEntryTypes.message, message_text="Program installation started")
 
 	sleep(1)
 	logger.start_indefinite_process(animation=IndefiniteAnimations.SuperSpace, message_text="File upload")
 	sleep(2)
-	logger.note_process(entry_type=TypesEntries.ACHIEVEMENT, message_text="Files downloaded")
+	logger.note_process(entry_type=ProcessEntryTypes.achievement, message_text="Files downloaded")
 	sleep(3)
 	logger.progress_rise(100)
 	logger.stop_process(message_text="Files unzipped")
 
-	logger.warning(message_text="Newer version found")
-	logger.timer_mark(message_text="Timer mark", local_background=False)
+	logger.entry(entry_type=LoggerEntryTypes.warning, message_text="Newer version found")
+	logger.timer_mark(message_text="Timer mark")
+
+	logger.separator()
+
+	data = logger.getty("Enter password: ")
 
 	sleep(1)
 	logger.start_definite_process(progress_bar=DefiniteAnimations.Arrow, message_text="Installing files")
 	sleep(0.6)
 	logger.progress_rise(3)
 	sleep(0.4)
 	logger.progress_rise(7)
@@ -39,32 +43,31 @@
 	logger.progress_rise(35)
 	sleep(1.4)
 	logger.progress_rise(45)
 	sleep(1.6)
 	logger.progress_rise(46)
 	sleep(1.1)
 	logger.progress_rise(47)
-	logger.note_process(entry_type=TypesEntries.MILESTONE, message_text="Files prepared")
+	logger.note_process(entry_type=ProcessEntryTypes.milestone, message_text="Files prepared")
 	sleep(3.7)
 	logger.progress_rise(76)
-	logger.note_process(entry_type=TypesEntries.TIMER_MARK, message_text="Timer mark")
 	sleep(1.5)
 	logger.progress_rise(77)
 	sleep(1.4)
 	logger.progress_rise(79)
 	sleep(1.1)
 	logger.progress_rise(81)
 	sleep(1.2)
 	logger.progress_rise(82)
 	sleep(1.3)
 	logger.progress_rise(85)
 	sleep(0.8)
-	logger.note_process(entry_type=TypesEntries.ERROR, message_text="Incompatibility found")
+	logger.note_process(entry_type=LoggerEntryTypes.error, message_text="Incompatibility found")
 	sleep(1.3)
-	logger.note_process(entry_type=TypesEntries.RESOLVED, message_text="Incompatibility eliminated")
+	logger.note_process(entry_type=LoggerEntryTypes.resolved, message_text="Incompatibility eliminated")
 	sleep(1.1)
 	logger.progress_rise(86)
 	sleep(0.6)
 	logger.progress_rise(87)
 	sleep(0.9)
 	logger.progress_rise(88)
 	sleep(0.9)
@@ -77,9 +80,10 @@
 	logger.progress_rise(97)
 	sleep(1.5)
 	logger.progress_rise(100)
 	sleep(1.3)
 	logger.stop_process(message_text="Program installed")
 
 	logger.stop_timer(message_text="Timer completed")
+	logger.empty(entry=data)
 
-	logger.buffer().save("log.txt")
+	logger.savy("log", False)
```

