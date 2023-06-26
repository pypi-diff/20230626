# Comparing `tmp/python-bale-bot-2.4.5.tar.gz` & `tmp/python-bale-bot-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bale-bot-2.4.5.tar", last modified: Fri Apr 21 07:00:33 2023, max compression
+gzip compressed data, was "python-bale-bot-2.4.6.tar", last modified: Mon Jun 26 09:34:53 2023, max compression
```

## Comparing `python-bale-bot-2.4.5.tar` & `python-bale-bot-2.4.6.tar`

### file list

```diff
@@ -1,44 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.569614 python-bale-bot-2.4.5/
--rw-rw-rw-   0        0        0     1091 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/LICENSE
--rw-rw-rw-   0        0        0     3052 2023-04-21 07:00:33.566612 python-bale-bot-2.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.483621 python-bale-bot-2.4.5/bale/
--rw-rw-rw-   0        0        0     1983 2023-04-13 11:25:40.000000 python-bale-bot-2.4.5/bale/__init__.py
--rw-rw-rw-   0        0        0      243 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.505619 python-bale-bot-2.4.5/bale/attachments/
--rw-rw-rw-   0        0        0      179 2023-04-11 12:58:39.000000 python-bale-bot-2.4.5/bale/attachments/__init__.py
--rw-rw-rw-   0        0        0     2586 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/attachments/audio.py
--rw-rw-rw-   0        0        0     1973 2023-04-11 13:00:45.000000 python-bale-bot-2.4.5/bale/attachments/contact.py
--rw-rw-rw-   0        0        0     3366 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/attachments/document.py
--rw-rw-rw-   0        0        0     1991 2023-04-11 13:00:45.000000 python-bale-bot-2.4.5/bale/attachments/location.py
--rw-rw-rw-   0        0        0     1995 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/attachments/photo.py
--rw-rw-rw-   0        0        0     2382 2023-04-11 12:52:46.000000 python-bale-bot-2.4.5/bale/attachments/video.py
--rw-rw-rw-   0        0        0    40598 2023-04-13 11:25:40.000000 python-bale-bot-2.4.5/bale/bot.py
--rw-rw-rw-   0        0        0     3777 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/callbackquery.py
--rw-rw-rw-   0        0        0    10832 2023-04-18 18:41:38.000000 python-bale-bot-2.4.5/bale/chat.py
--rw-rw-rw-   0        0        0     3934 2023-04-13 11:25:40.000000 python-bale-bot-2.4.5/bale/chatmember.py
--rw-rw-rw-   0        0        0     7595 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/components.py
--rw-rw-rw-   0        0        0     3740 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/error.py
--rw-rw-rw-   0        0        0    14455 2023-04-13 11:01:04.000000 python-bale-bot-2.4.5/bale/message.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.514618 python-bale-bot-2.4.5/bale/payments/
--rw-rw-rw-   0        0        0       56 2023-04-11 12:58:40.000000 python-bale-bot-2.4.5/bale/payments/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/payments/invoice.py
--rw-rw-rw-   0        0        0     1733 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/payments/price.py
--rw-rw-rw-   0        0        0     4402 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/permissions.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.523617 python-bale-bot-2.4.5/bale/request/
--rw-rw-rw-   0        0        0      201 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/request/__init__.py
--rw-rw-rw-   0        0        0    12113 2023-04-11 12:44:43.000000 python-bale-bot-2.4.5/bale/request/http.py
--rw-rw-rw-   0        0        0     1371 2023-04-11 12:44:43.000000 python-bale-bot-2.4.5/bale/request/parser.py
--rw-rw-rw-   0        0        0      123 2023-04-09 22:53:13.000000 python-bale-bot-2.4.5/bale/request/utils.py
--rw-rw-rw-   0        0        0     6631 2023-04-11 17:56:28.000000 python-bale-bot-2.4.5/bale/update.py
--rw-rw-rw-   0        0        0     5285 2023-04-13 11:33:59.000000 python-bale-bot-2.4.5/bale/updater.py
--rw-rw-rw-   0        0        0     6176 2023-04-13 11:29:15.000000 python-bale-bot-2.4.5/bale/user.py
--rw-rw-rw-   0        0        0      145 2023-04-21 06:51:10.000000 python-bale-bot-2.4.5/bale/version.py
-drwxrwxrwx   0        0        0        0 2023-04-21 07:00:33.564611 python-bale-bot-2.4.5/python_bale_bot.egg-info/
--rw-rw-rw-   0        0        0     3052 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      807 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-21 07:00:33.000000 python-bale-bot-2.4.5/python_bale_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 07:00:33.569614 python-bale-bot-2.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1698 2023-04-21 06:51:10.000000 python-bale-bot-2.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.341871 python-bale-bot-2.4.6/
+-rw-rw-rw-   0        0        0    15402 2023-05-07 15:38:30.000000 python-bale-bot-2.4.6/LICENSE
+-rw-rw-rw-   0        0        0     3057 2023-06-26 09:34:53.341208 python-bale-bot-2.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2341 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.133652 python-bale-bot-2.4.6/bale/
+-rw-rw-rw-   0        0        0     2072 2023-06-20 15:49:07.000000 python-bale-bot-2.4.6/bale/__init__.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.158670 python-bale-bot-2.4.6/bale/attachments/
+-rw-rw-rw-   0        0        0      203 2023-06-20 14:42:57.000000 python-bale-bot-2.4.6/bale/attachments/__init__.py
+-rw-rw-rw-   0        0        0     2452 2023-06-26 08:09:14.000000 python-bale-bot-2.4.6/bale/attachments/audio.py
+-rw-rw-rw-   0        0        0     2323 2023-06-26 08:48:02.000000 python-bale-bot-2.4.6/bale/attachments/contact.py
+-rw-rw-rw-   0        0        0     2307 2023-06-26 08:10:29.000000 python-bale-bot-2.4.6/bale/attachments/document.py
+-rw-rw-rw-   0        0        0     4004 2023-06-26 08:40:10.000000 python-bale-bot-2.4.6/bale/attachments/file.py
+-rw-rw-rw-   0        0        0     2323 2023-06-26 08:48:02.000000 python-bale-bot-2.4.6/bale/attachments/location.py
+-rw-rw-rw-   0        0        0     2269 2023-06-26 08:10:29.000000 python-bale-bot-2.4.6/bale/attachments/photo.py
+-rw-rw-rw-   0        0        0     2650 2023-06-26 08:10:29.000000 python-bale-bot-2.4.6/bale/attachments/video.py
+-rw-rw-rw-   0        0        0    43778 2023-06-25 18:25:53.000000 python-bale-bot-2.4.6/bale/bot.py
+-rw-rw-rw-   0        0        0     3964 2023-05-07 15:38:31.000000 python-bale-bot-2.4.6/bale/callbackquery.py
+-rw-rw-rw-   0        0        0    11048 2023-06-20 16:33:57.000000 python-bale-bot-2.4.6/bale/chat.py
+-rw-rw-rw-   0        0        0     3934 2023-04-13 11:25:40.000000 python-bale-bot-2.4.6/bale/chatmember.py
+-rw-rw-rw-   0        0        0     3740 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/error.py
+-rw-rw-rw-   0        0        0    15334 2023-06-26 08:04:21.000000 python-bale-bot-2.4.6/bale/message.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.203717 python-bale-bot-2.4.6/bale/payments/
+-rw-rw-rw-   0        0        0       56 2023-04-11 12:58:40.000000 python-bale-bot-2.4.6/bale/payments/__init__.py
+-rw-rw-rw-   0        0        0     2131 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/payments/invoice.py
+-rw-rw-rw-   0        0        0     1733 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/payments/price.py
+-rw-rw-rw-   0        0        0     4402 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/permissions.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.263710 python-bale-bot-2.4.6/bale/request/
+-rw-rw-rw-   0        0        0      201 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/request/__init__.py
+-rw-rw-rw-   0        0        0    10708 2023-05-17 19:07:05.000000 python-bale-bot-2.4.6/bale/request/http.py
+-rw-rw-rw-   0        0        0     1371 2023-04-11 12:44:43.000000 python-bale-bot-2.4.6/bale/request/parser.py
+-rw-rw-rw-   0        0        0      123 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/request/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.276879 python-bale-bot-2.4.6/bale/ui/
+-rw-rw-rw-   0        0        0      167 2023-06-26 08:08:10.000000 python-bale-bot-2.4.6/bale/ui/__init__.py
+-rw-rw-rw-   0        0        0     4820 2023-06-26 08:20:23.000000 python-bale-bot-2.4.6/bale/ui/components.py
+-rw-rw-rw-   0        0        0     2923 2023-06-20 15:49:07.000000 python-bale-bot-2.4.6/bale/ui/inline_keyboard.py
+-rw-rw-rw-   0        0        0     1739 2023-06-26 08:24:36.000000 python-bale-bot-2.4.6/bale/ui/menu_keyboard.py
+-rw-rw-rw-   0        0        0     6631 2023-04-11 17:56:28.000000 python-bale-bot-2.4.6/bale/update.py
+-rw-rw-rw-   0        0        0     5356 2023-04-29 18:54:30.000000 python-bale-bot-2.4.6/bale/updater.py
+-rw-rw-rw-   0        0        0     6782 2023-06-20 16:33:57.000000 python-bale-bot-2.4.6/bale/user.py
+-rw-rw-rw-   0        0        0      328 2023-05-07 15:38:31.000000 python-bale-bot-2.4.6/bale/utils.py
+-rw-rw-rw-   0        0        0      145 2023-06-20 14:42:57.000000 python-bale-bot-2.4.6/bale/version.py
+drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.338870 python-bale-bot-2.4.6/python_bale_bot.egg-info/
+-rw-rw-rw-   0        0        0     3057 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      921 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 09:34:53.341871 python-bale-bot-2.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1672 2023-06-20 14:42:57.000000 python-bale-bot-2.4.6/setup.py
```

### Comparing `python-bale-bot-2.4.5/PKG-INFO` & `python-bale-bot-2.4.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: python-bale-bot
-Version: 2.4.5
+Version: 2.4.6
 Summary: An API wrapper for Bale written in Python
 Home-page: https://github.com/python-bale-bot/python-bale-bot/
 Author: Kian Ahmadian
 License: MIT License
 Project-URL: Documentation, https://docs.python-bale-bot.ir/en/master/
-Project-URL: Changelog, https://python-bale-bot.rtfd.io/en/master/whats_new.html
+Project-URL: Changelog, https:///docs.python-bale-bot.ir/en/master/whats_new.html
 Project-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
 Keywords: bale,bale-bot,framework,bot
 Platform: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
@@ -55,7 +55,9 @@
 <p><b>The <a href="https://python-bale-bot.readthedocs.io/en/master">package documentation</a> is the technical reference for python-bale-bot. It contains descriptions of all available classes, modules, methods and arguments as well as the changelog.</b></p>
 
 
 ## Contact to Developers
 [![Email](https://img.shields.io/badge/Email-python--bale--bot@googlegroups.com-green?logo=Gmail&logoColor=white)](mailto:python-bale-bot@googlegroups.com)
 [![Discord](https://img.shields.io/badge/Support_Server-bYHEzyDe2j-green?logo=Discord&logoColor=white)](https://discord.gg/bYHEzyDe2j)
 [![Our Site](https://img.shields.io/badge/Our_site-python--bale--bot.ir-green?logo=GitHub&logoColor=white)](https://python-bale-bot.ir)
+
+
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.5 Summary: An API
+Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.6 Summary: An API
 wrapper for Bale written in Python Home-page: https://github.com/python-bale-
 bot/python-bale-bot/ Author: Kian Ahmadian License: MIT License Project-URL:
 Documentation, https://docs.python-bale-bot.ir/en/master/ Project-URL:
-Changelog, https://python-bale-bot.rtfd.io/en/master/whats_new.html Project-
+Changelog, https:///docs.python-bale-bot.ir/en/master/whats_new.html Project-
 URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
 Keywords: bale,bale-bot,framework,bot Platform: Windows Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: docs License-File:
 LICENSE # python-bale-bot
                            [python-bale-bot image]
                   An API wrapper for Bale written in Python.
```

### Comparing `python-bale-bot-2.4.5/README.md` & `python-bale-bot-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.5/bale/__init__.py` & `python-bale-bot-2.4.6/bale/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from .version import __version__
 from .request import HTTPClient, Route, ResponseStatusCode, ResponseParser
-from .components import Components, RemoveComponents, InlineKeyboard, Keyboard
-from .attachments import *
-from .payments import *
+from .ui import InlineKeyboard, MenuKeyboard, RemoveMenuKeyboard, Components
+from .attachments import File, Audio, ContactMessage, Location, Photo, Document, Video
 from .payments import Price, Invoice
 from .user import User
 from .attachments.contact import ContactMessage
 from .chat import Chat, ChatType
 from .message import Message
 from .permissions import Permissions
 from .chatmember import ChatMember, ChatMemberStatus
@@ -37,8 +36,9 @@
 from .update import Update, UpdateType
 from .updater import Updater, EventType
 from .error import BaleError, APIError, NetworkError, HTTPException, TimeOut, NotFound, Forbidden, HTTPClientError, InvalidToken, RateLimited
 from .bot import Bot
 
 __title__ = "python-bale-bot"
 __author__ = "Kian Ahmadian"
+__copyright__ = 'Copyright 2021-present Kian Ahmadian'
 __license__ = 'MIT'
```

### Comparing `python-bale-bot-2.4.5/bale/attachments/audio.py` & `python-bale-bot-2.4.6/bale/attachments/video.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,53 +17,58 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-class Audio:
-    """This object shows a waist.
+from typing import TYPE_CHECKING
+
+from .file import File
+if TYPE_CHECKING:
+    from bale import Bot
+
+
+class Video(File):
+    """This object shows a Video.
 
     Attributes
     ----------
         file_id: str
-            Audio ID
-        duration: int
-            Audio duration
+            Identifier for this file, which can be used to download or reuse the file.
+        width: int
+            Video width as defined by sender.
         file_size: int
-            Audio Size.
-        mime_type: Optional[:class:`str`]
-            Audio Mime type.
-        title: Optional[:class:`str`]
-            Audio Title.
+            File size in bytes.
+        height: str
+            Video height as defined by sender.
+        duration: int
+            Duration of the video in seconds as defined by sender.
+        mime_type: :class:`str`
+           MIME type of file as defined by sender.
     """
-    __slots__ = (
-        "file_id",
-        "duration",
-        "title",
-        "file_size",
-        "mime_type",
-        "bot"
+    __FILE_TYPE__ = "VIDEO"
+    __slots__ = File.__slots__ + (
+        "width",
+        "height",
+        "duration"
     )
 
-    def __init__(self, file_id: str, duration: int, file_size: int = None, mime_type: str = None, title: str = None):
-        self.file_id = file_id
-        self.duration = duration
+    def __init__(self, file_id: str, mime_type: str, width: int, height: int, file_size: int, duration: int, bot: "Bot"):
+        super().__init__(self.__FILE_TYPE__, file_id, file_size, mime_type, bot, duration = duration, width = width, height = height)
 
-        self.title = title
-        self.file_size = file_size
-        self.mime_type = mime_type
+        self.width = width
+        self.height = height
+        self.duration = duration
 
     @classmethod
-    def from_dict(cls, data):
-        return cls(file_id=data["file_id"], duration=data["duration"], file_size=data["file_size"], title=data["title"],
-                   mime_type=data["mime_type"])
-
-    def to_dict(self):
-        data = {"file_id": self.file_id if self.file_id is not None else None,
-                "duration": self.duration if self.duration is not None else None,
-                "title": self.title if self.title is not None else None,
-                "file_size": self.file_size if self.file_size is not None else None,
-                "mime_type": self.mime_type if self.mime_type is not None else None}
+    def from_dict(cls, data: dict, bot: "Bot"):
+        return cls(
+            file_id=data.get("file_id"),
+            width=data.get("width"),
+            height=data.get("height"),
+            file_size=data.get("file_size"),
+            duration=data.get("duration"),
+            mime_type=data.get("mime_type"),
+            bot=bot
+        )
 
-        return data
```

### Comparing `python-bale-bot-2.4.5/bale/attachments/contact.py` & `python-bale-bot-2.4.6/bale/attachments/contact.py`

 * *Files 25% similar despite different names*

```diff
@@ -48,7 +48,16 @@
     def from_dict(cls, data: dict):
         return cls(first_name=data["first_name"], last_name=data["last_name"], phone_number=data["phone_number"])
 
     def to_dict(self):
         data = {"phone_number": self.phone_number, "first_name": self.first_name, "last_name": self.last_name}
 
         return data
+
+    def __eq__(self, other):
+        return isinstance(other, ContactMessage) and self.phone_number == other.phone_number
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __repr__(self):
+        return f"<ContactMessage phone_number={self.phone_number} first_name={self.first_name} last_name={self.last_name} >"
```

### Comparing `python-bale-bot-2.4.5/bale/attachments/location.py` & `python-bale-bot-2.4.6/bale/attachments/location.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,30 +28,39 @@
 
     Attributes
     ----------
         longitude: int
             Location longitude
         latitude: int
             Location latitude
-        link: str
     """
     __slots__ = (
         "longitude",
         "latitude"
     )
 
     def __init__(self, longitude: int, latitude: int):
         self.longitude = longitude
         self.latitude = latitude
 
     @property
-    def link(self):
+    def link(self) -> str:
+        """:class:`str`: export location link from map"""
         return f"https://maps.google.com/maps?q=loc:{self.longitude},{self.latitude}"
 
     @classmethod
     def from_dict(cls, data):
         return cls(longitude=data["longitude"], latitude=data["latitude"])
 
     def to_dict(self):
         data = {"longitude": self.longitude if self.longitude is not None else None,
                 "latitude": self.latitude if self.latitude is not None else None}
         return data
+
+    def __eq__(self, other):
+        return isinstance(other, Location) and self.link == other.link
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
+    def __repr__(self):
+        return f"<Location longitude={self.longitude} latitude={self.latitude} >"
```

### Comparing `python-bale-bot-2.4.5/bale/attachments/video.py` & `python-bale-bot-2.4.6/bale/attachments/photo.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,60 +17,48 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+from typing import TYPE_CHECKING
 
+from .file import File
+if TYPE_CHECKING:
+    from bale import Bot
 
-class Video:
-    """This object shows a Video.
+
+class Photo(File):
+    """This object shows a Photo.
 
     Attributes
     ----------
         file_id: str
-            Video ID
+            Identifier for this file, which can be used to download or reuse the file.
         width: int
-            Video width
-        file_size: int
-            Video Size.
+            Photo width as defined by sender.
         height: str
-            Video height.
-        duration: int
-            Video duration.
-
+            Photo height as defined by sender.
+        file_size: int
+            File size in bytes.
     """
-    __slots__ = (
-        "file_id",
+    __FILE_TYPE__ = "PHOTO"
+    __slots__ = File.__slots__ + (
         "width",
-        "height",
-        "file_size",
-        "duration"
+        "height"
     )
+    def __init__(self, file_id: str, width: int, height: int, file_size: int, bot: "Bot"):
+        super().__init__(self.__FILE_TYPE__, file_id, file_size, "jpg", bot, width = width, height = height)
 
-    def __init__(self, file_id: str, width: int, height: int, file_size: int, duration: int):
-        self.file_id = file_id
         self.width = width
         self.height = height
-        self.file_size = file_size
-        self.duration = duration
 
     @classmethod
-    def from_dict(cls, data: dict):
+    def from_dict(cls, data: dict, bot: "Bot"):
         return cls(
             file_id=data.get("file_id"),
             width=data.get("width"),
             height=data.get("height"),
             file_size=data.get("file_size"),
-            duration=data.get("duration")
+            bot=bot
         )
-
-    def to_dict(self):
-        data = {
-            "file_id": self.file_id,
-            "width": self.width,
-            "height": self.height,
-            "file_size": self.file_size,
-            "duration": self.duration
-        }
-        return data
```

### Comparing `python-bale-bot-2.4.5/bale/bot.py` & `python-bale-bot-2.4.6/bale/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 SOFTWARE.
 """
 from __future__ import annotations
 import asyncio
 from typing import Callable, Dict, Tuple, List, Optional
 from builtins import enumerate, reversed
 from .error import NotFound, InvalidToken
-from bale import (Message, Update, User, Components, RemoveComponents, Chat, Price, ChatMember, HTTPClient, Updater,
-                  Photo, Document, Location, ContactMessage, Video)
+from bale import (Message, Update, User, Components, RemoveMenuKeyboard, Chat, Price, ChatMember, HTTPClient, Updater,
+                  Photo, Document, Location, ContactMessage, Video, Audio)
 
 __all__ = (
     "Bot"
 )
 
 
 class _Loop:
@@ -51,15 +51,14 @@
     """This object represents a Bale Bot.
 
     Parameters
     ----------
         token: str 
             Bot Token
         updater: Optional[:class:`bale.Updater`]
-        base_url: Optional[:class:`str`]
 
     .. note::
         When you create bot and run for first-step, use :meth:`bale.Bot.delete_webhook` method in `on_ready` event.
     """
     __slots__ = (
         "loop",
         "token",
@@ -73,15 +72,15 @@
     )
 
     def __init__(self, token: str, **kwargs):
         if not isinstance(token, str):
             raise InvalidToken("token must be type of the str")
         self.loop = _loop
         self.token = token
-        self.http: HTTPClient = HTTPClient(self.loop, token, kwargs.get("base_url"))
+        self.http: HTTPClient = HTTPClient(self.loop, token)
         self._user = None
         self.events: Dict[str, List[Callable]] = {}
         self.listeners: Dict[str, List[Tuple[asyncio.Future, Callable[..., bool]]]] = {}
         self._closed = False
 
         self.updater: Updater = kwargs.get("updater", Updater)(self)
 
@@ -163,15 +162,15 @@
             await core(*args, **kwargs)
         except Exception as ext:
             await self.on_error(event_name, ext)
 
     def call_to_run_event(self, core, event_name, *args, **kwargs):
         task = self.run_event(core, event_name, *args, **kwargs)
         self.loop: asyncio.AbstractEventLoop
-        return self.loop.create_task(task, name=event_name)
+        return self.loop.create_task(task, name=f"python-bale-bot: {event_name}")
 
     def dispatch(self, event_name, /, *args, **kwargs):
         method = "on_" + event_name
         listeners = self.listeners.get(event_name)
         if listeners:
             removed = []
             for index, (future, check) in enumerate(listeners):
@@ -209,15 +208,15 @@
         print("error", event_name, error)
 
     async def get_bot(self) -> User:
         """Get bot information
 
         Returns
         -------
-            :class:`Bale.User` :
+            :class:`bale.User` :
                 Bot User information.
         Raises
         ------
             APIError
                 Get bot Failed.
         """
         response = await self.http.get_bot()
@@ -237,15 +236,15 @@
             APIError
                 Delete webhook Failed.
         """
         response = await self.http.delete_webhook()
         return response.result or False
 
     async def send_message(self, chat_id: str | int, text: str, *,
-                           components: Optional["Components" | "RemoveComponents"] = None,
+                           components: Optional["Components" | "RemoveMenuKeyboard"] = None,
                            reply_to_message_id: Optional[str | int] = None) -> "Message":
         """This service is used to send text messages.
 
         Parameters
         ----------
             chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
@@ -270,15 +269,15 @@
         """
         if not isinstance(chat_id, (str, int)):
             raise TypeError(
                 "chat_id param must be type of str or int"
             )
 
         if components:
-            if not isinstance(components, (Components, RemoveComponents)):
+            if not isinstance(components, (Components, RemoveMenuKeyboard)):
                 raise TypeError(
                     "components param must be type of Components or RemoveComponents"
                 )
             components = components.to_dict()
 
         if reply_to_message_id and not isinstance(reply_to_message_id, (int, str)):
             raise TypeError(
@@ -295,15 +294,15 @@
         Parameters
         ----------
             chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             from_chat_id: :class:`str` | :class:`int`
                 the chat where the original message was sent (or channel username in the format @channelusername).
             message_id: :class:`int` | :class:`str`
-                Message in the chat specified in :param:`from_chat_id`.
+                Message in the chat specified in ``from_chat_id``.
         Returns
         -------
             :class:`bale.Message`
                 The Message
         Raises
         ------
             NotFound
@@ -337,15 +336,15 @@
         """This service is used to send document.
 
         Parameters
         ----------
         chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
         document: :class:`bytes` | :class:`str` | :class:`bale.Document`
-            File to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one.
+            File to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
         caption: Optional[:class:`str`]
             Document caption.
         reply_to_message_id: Optional[:class:`str` | :class:`int`]
                 Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
@@ -388,15 +387,15 @@
         """This service is used to send photo.
 
         Parameters
         ----------
             chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             photo: :class:`bytes` | :class:`str` | :class:`bale.Photo`
-                Photo to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one.
+                Photo to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
             caption: Optional[:class:`str`]
                 Photo caption.
             reply_to_message_id: Optional[:class:`str` | :class:`int`]
                 Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
@@ -435,24 +434,80 @@
                 "caption param must be type of str"
             )
 
         response = await self.http.send_photo(str(chat_id), photo, caption=caption,
                                               reply_to_message_id=reply_to_message_id)
         return Message.from_dict(data=response.result, bot=self)
 
+    async def send_audio(self, chat_id: str | int, audio: bytes | str | "Audio", *, caption: Optional[str] = None,
+                         reply_to_message_id: Optional[str | int] = None) -> "Message":
+        """This service is used to send Audio.
+
+        Parameters
+        ----------
+            chat_id: :class:`str` | :class:`int`
+                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            audio: :class:`bytes` | :class:`str` | :class:`bale.Audio`
+                Audio file to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
+            caption: Optional[:class:`str`]
+                Audio caption.
+            reply_to_message_id: Optional[:class:`str` | :class:`int`]
+                Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
+
+        Returns
+        --------
+            :class:`bale.Message`
+                The Message.
+
+        Raises
+        ------
+            NotFound
+                Invalid Chat ID.
+            Forbidden
+                You do not have permission to Send Audio to chat.
+            APIError
+                Send Audio Failed.
+        """
+        if not isinstance(chat_id, (str, int)):
+            raise TypeError(
+                "chat_id param must be type of str or int"
+            )
+
+        if not isinstance(audio, (bytes, str, Audio)):
+            raise TypeError(
+                "audio param must be type of bytes, str or Audio"
+            )
+
+        if isinstance(audio, Audio):
+            audio = audio.file_id
+
+        if reply_to_message_id and not isinstance(reply_to_message_id, (str, int)):
+            raise TypeError(
+                "reply_to_message_id param must be type of str or int"
+            )
+
+        if caption and not isinstance(caption, str):
+            raise TypeError(
+                "caption param must be type of str"
+            )
+
+        response = await self.http.send_audio(str(chat_id), audio, caption=caption,
+                                              reply_to_message_id=reply_to_message_id)
+        return Message.from_dict(data=response.result, bot=self)
+
     async def send_video(self, chat_id: str | int, video: bytes | str | "Photo", *, caption: Optional[str] = None,
                          reply_to_message_id: Optional[str | int] = None) -> "Message":
         """This service is used to send Video.
 
         Parameters
         ----------
             chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             video: :class:`bytes` | :class:`str` | :class:`bale.Photo`
-                Video to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Telegram to get a file from the Internet, or upload a new one.
+                Video to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
             caption: Optional[:class:`str`]
                 Video caption.
             reply_to_message_id: Optional[:class:`str` | :class:`int`]
                 Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
@@ -496,18 +551,18 @@
         return Message.from_dict(data=response.result, bot=self)
 
     async def send_location(self, chat_id: str | int, location: "Location") -> "Message":
         """Use this method to send point on the map.
 
         Parameters
         ----------
-        chat_id: :class:`str` | :class:`int`
+            chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
-        location: :class:`bale.Location`
-            The Location.
+            location: :class:`bale.Location`
+                The Location.
 
         Returns
         --------
             :class:`bale.Message`
                 The Message.
 
         Raises
@@ -533,18 +588,18 @@
         return Message.from_dict(data=response.result, bot=self)
 
     async def send_contact(self, chat_id: str | int, contact: "ContactMessage") -> "Message":
         """This service is used to send contact.
 
         Parameters
         ----------
-        chat_id: :class:`str` | :class:`int`
-                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
-        contact: :class:`bale.ContactMessage`
-            The Contact.
+            chat_id: :class:`str` | :class:`int`
+                    Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            contact: :class:`bale.ContactMessage`
+                The Contact.
 
         Returns
         --------
             :class:`bale.Message`
                 The Message.
 
         Raises
@@ -576,36 +631,36 @@
                            need_phone_number: Optional[bool] = False,
                            need_email: Optional[bool] = False, need_shipping_address: Optional[bool] = False,
                            is_flexible: Optional[bool] = True) -> Message:
         """You can use this service to send money request messages.
 
         Parameters
         ----------
-        chat_id: :class:`str` | :class:`int`
-                Unique identifier for the target chat or username of the target channel (in the format @channelusername).
-        title: str
-            Product name. 1- 32 characters.
-        description: str
-            Product description. 1- 255 characters.
-        provider_token: str
-            You can use 3 methods to receive money: 1.Card number 2. Port number and acceptor number 3. Wallet number "Bale"
-        prices: List[:class:`bale.Price`]
-            A list of prices.
-        photo_url: Optional[:class:`str`]
-            URL of the product photo for the invoice. Can be a photo of the goods or a marketing image for a service. People like it better when they see what they are paying for.
-        need_name: Optional[bool]
-            Pass True, if you require the user’s full name to complete the order.
-        need_phone_number: Optional[bool]
-            Pass True, if you require the user’s phone number to complete the order.
-        need_email: Optional[bool]
-            Pass True, if you require the user’s email to complete the order.
-        need_shipping_address: Optional[bool]
-            Pass True, if you require the user’s shipping address to complete the order.
-        is_flexible: Optional[bool]
-            Pass True, if the final price depends on the shipping method.
+            chat_id: :class:`str` | :class:`int`
+                    Unique identifier for the target chat or username of the target channel (in the format @channelusername).
+            title: str
+                Product name. 1- 32 characters.
+            description: str
+                Product description. 1- 255 characters.
+            provider_token: str
+                You can use 3 methods to receive money: 1.Card number 2. Port number and acceptor number 3. Wallet number "Bale"
+            prices: List[:class:`bale.Price`]
+                A list of prices.
+            photo_url: Optional[:class:`str`]
+                URL of the product photo for the invoice. Can be a photo of the goods or a marketing image for a service. People like it better when they see what they are paying for.
+            need_name: Optional[bool]
+                Pass True, if you require the user’s full name to complete the order.
+            need_phone_number: Optional[bool]
+                Pass True, if you require the user’s phone number to complete the order.
+            need_email: Optional[bool]
+                Pass True, if you require the user’s email to complete the order.
+            need_shipping_address: Optional[bool]
+                Pass True, if you require the user’s shipping address to complete the order.
+            is_flexible: Optional[bool]
+                Pass True, if the final price depends on the shipping method.
 
         Returns
         -------
             :class:`bale.Message`
             
         Raises
         ------
@@ -617,52 +672,67 @@
                 Send Invoice Failed.  
         """
         if not isinstance(chat_id, (str, int)):
             raise TypeError(
                 "chat param must be type of str or int"
             )
 
-        if not isinstance(photo_url, str):
+        if not isinstance(title, str):
+            raise TypeError(
+                "title param must be type of str"
+            )
+
+        if not isinstance(provider_token, str):
+            raise TypeError(
+                "provider_token param must be type of str"
+            )
+
+        if not isinstance(prices, list):
+            raise TypeError(
+                "prices must param must be type of list"
+            )
+
+        if photo_url and not isinstance(photo_url, str):
             raise TypeError(
                 "photo_url param must be type of str"
             )
 
-        if not isinstance(need_name, bool):
+        if need_name is not None and not isinstance(need_name, bool):
             raise TypeError(
                 "need_name param must be type of boolean"
             )
 
-        if not isinstance(need_phone_number, bool):
+        if need_phone_number is not None and not isinstance(need_phone_number, bool):
             raise TypeError(
                 "need_phone_number param must be type of boolean"
             )
 
-        if not isinstance(need_email, bool):
+        if need_email is not None and not isinstance(need_email, bool):
             raise TypeError(
                 "need_email param must be type of boolean"
             )
 
-        if not isinstance(need_shipping_address, bool):
+        if need_shipping_address is not None and not isinstance(need_shipping_address, bool):
             raise TypeError(
                 "need_shipping_address param must be type of boolean"
             )
 
-        if not isinstance(is_flexible, bool):
+        if is_flexible is not None and not isinstance(is_flexible, bool):
             raise TypeError(
                 "is_flexible param must be type of boolean"
             )
 
         prices = [price.to_dict() for price in prices if isinstance(price, Price)]
         response = await self.http.send_invoice(str(chat_id), title, description, provider_token, prices, photo_url,
                                                 need_name,
                                                 need_phone_number, need_email, need_shipping_address, is_flexible)
         return Message.from_dict(data=response.result, bot=self)
 
     async def edit_message(self, chat_id: str | int, message_id: str | int, text: str, *,
-                           components: Optional["Components" | "RemoveComponents"] = None) -> "Message":
+                           components: Optional["Components" | "RemoveMenuKeyboard"] = None) -> "Message":
         """You can use this service to edit text messages that you have already sent through the arm.
 
         Parameters
         ----------
             chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             message_id: :class:`str` | :class:`int`
@@ -686,15 +756,15 @@
             )
 
         if not isinstance(message_id, (str, int)):
             raise TypeError(
                 "message_id param must be type of str or int"
             )
 
-        if components and not isinstance(components, (Components, RemoveComponents)):
+        if components and not isinstance(components, (Components, RemoveMenuKeyboard)):
             raise TypeError(
                 "components param must be type of Components or RemoveComponents"
             )
 
         if components:
             components = components.to_dict()
 
@@ -1024,16 +1094,16 @@
 
         if limit and not isinstance(limit, int):
             raise TypeError(
                 "limit param must be int"
             )
 
         response = await self.http.get_updates(offset, limit)
-        return [Update.from_dict(data=update_payload, bot=self) for update_payload in response.result or list()
-                if not offset or (offset and update_payload.get("update_id") > offset)]
+        return [Update.from_dict(data=update_payload, bot=self) for update_payload in response.result
+                if not offset or (offset and update_payload.get("update_id") > offset)] if response.result else None
 
     async def connect(self, sleep_after_every_get_updates):
         self._user = await self.get_bot()
         await self.updater.start(sleep_after_every_get_updates=sleep_after_every_get_updates)
 
     def run(self, sleep_after_every_get_updates=None):
         """Run bot and https"""
@@ -1042,7 +1112,9 @@
             async with self:
                 await self.connect(sleep_after_every_get_updates=sleep_after_every_get_updates)
 
         try:
             asyncio.run(main())
         except KeyboardInterrupt:  # Control-C
             pass
+        except SystemExit:
+            pass
```

### Comparing `python-bale-bot-2.4.5/bale/callbackquery.py` & `python-bale-bot-2.4.6/bale/callbackquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         "from_user",
         "message",
         "inline_message_id",
         "data",
         "bot"
     )
 
-    def __init__(self, callback_id: int = None, data: str = None, message: "Message" = None,
+    def __init__(self, callback_id: int, data: str = None, message: "Message" = None,
                  inline_message_id: str = None, from_user: "User" = None, bot: "Bot" = None):
         self.callback_id = callback_id
         self.data = data
         self.message = message
         self.inline_message_id = inline_message_id
         self.from_user = from_user
         self.bot = bot
@@ -90,9 +90,15 @@
         if self.message:
             data["message"] = self.message.to_dict()
         if self.from_user:
             data["from_user"] = self.from_user.to_dict()
 
         return data
 
+    def __eq__(self, other):
+        return isinstance(other, CallbackQuery) and self.callback_id == other.callback_id
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
+
     def __repr__(self):
         return f"<CallbackQuery inline_message_id={self.inline_message_id} message={self.message} from_user={self.from_user} data={self.data}>"
```

### Comparing `python-bale-bot-2.4.5/bale/chat.py` & `python-bale-bot-2.4.6/bale/chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from __future__ import annotations
 from bale import User
 from typing import TYPE_CHECKING, Optional, List
 if TYPE_CHECKING:
-    from bale import Bot, Message, User, Photo, Document, Components, RemoveComponents, Price, Location, ContactMessage, Video
+    from bale import Bot, Message, User, Photo, Document, Components, RemoveMenuKeyboard, Price, Location, ContactMessage, Video, Audio
 
 
 __all__ = (
     "Chat",
     "ChatType"
 )
 
@@ -138,37 +138,43 @@
         self.bot = bot
 
     @property
     def mention(self) -> str | None:
         """Optional[:class:`str`]"""
         return ("@" + self.username) if self.username else None
 
-    async def send(self, text: str, components: Optional["Components" | "RemoveComponents"] = None):
+    async def send(self, text: str, components: Optional["Components" | "RemoveMenuKeyboard"] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_message`.
         """
         return await self.bot.send_message(self.chat_id, text, components=components)
 
     async def send_document(self, document: bytes | str | "Document", *, caption: Optional[str] = None):
         """
-        For the documentation of the arguments, please see :meth:`bale.Bot.send_photo`.
+        For the documentation of the arguments, please see :meth:`bale.Bot.send_document`.
         """
         return await self.bot.send_document(self.chat_id, document, caption=caption)
 
     async def send_photo(self, photo: bytes | str | "Photo", *, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_photo`.
         """
         return await self.bot.send_photo(self.chat_id, photo, caption=caption)
 
-    async def send_video(self, photo: bytes | str | "Video", *, caption: Optional[str] = None):
+    async def send_video(self, video: bytes | str | "Video", *, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_video`.
         """
-        return await self.bot.send_video(self.chat_id, photo, caption=caption)
+        return await self.bot.send_video(self.chat_id, video, caption=caption)
+
+    async def send_audio(self, audio: bytes | str | "Audio", *, caption: Optional[str] = None):
+        """
+        For the documentation of the arguments, please see :meth:`bale.Bot.send_audio`.
+        """
+        return await self.bot.send_audio(self.chat_id, audio, caption=caption)
 
     async def send_location(self, location: "Location"):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_location`.
         """
         return await self.bot.send_location(self.chat_id, location)
 
@@ -192,15 +198,15 @@
         """
         For the documentation of the method, please see :meth:`bale.Bot.leave_chat`.
         """
         await self.bot.leave_chat(self.chat_id)
 
     async def add_user(self, user: "User"):
         """
-        For the documentation of the arguments, please see :meth:`bale.Bot.invite_to_chat`.
+        For the documentation of the arguments, please see :meth:`bale.Bot.invite_user`.
         """
         await self.bot.invite_user(self.chat_id, user.chat_id)
 
     async def get_chat_member(self, user: "User" | str):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.get_chat_member`.
         """
@@ -253,16 +259,15 @@
             "first_name": self.first_name,
             "last_name": self.last_name
         }
 
         return data
 
     def __str__(self):
-        return (str(self.username) + "#" + str(self.chat_id) if self.username else str(self.first_name) + " " + str(
-            self.last_name))
+        return str(self.first_name) + str(self.last_name)
 
     def __eq__(self, other):
         return isinstance(other, Chat) and self.chat_id == other.chat_id
 
     def __ne__(self, other):
         return not self.__eq__(other)
```

### Comparing `python-bale-bot-2.4.5/bale/chatmember.py` & `python-bale-bot-2.4.6/bale/chatmember.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.5/bale/error.py` & `python-bale-bot-2.4.6/bale/error.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.5/bale/message.py` & `python-bale-bot-2.4.6/bale/message.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,132 +20,150 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from __future__ import annotations
 
 from datetime import datetime
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, List, Optional, NoReturn
 
 if TYPE_CHECKING:
     from bale import Bot
 
-from bale import (Chat, User, Document, ContactMessage, Location, Photo, Invoice, Components, RemoveComponents, Price,
-                  Video)
+from bale import (Chat, User, Document, ContactMessage, Location, Photo, Invoice, Components, RemoveMenuKeyboard,
+                  Video, Audio, File)
 
 
 class Message:
     """This object shows a message.
 
     Attributes
     ----------
         message_id: str
             Unique message identifier inside this chat.
         from_user: Optional[:class:`bale.User`]
-            Sender of the message; empty for messages sent to channels. For backward compatibility, this will contain a fake sender user in non-channel chats, if the message was sent on behalf of a chat.
+            Sender of the message; empty for messages sent to channels. For backward compatibility, this will contain a
+            fake sender user in non-channel chats, if the message was sent on behalf of a chat.
         chat: :class:`bale.Chat`
             Conversation the message belongs to.
         date: :class:`datetime.datetime`
             Date the message was sent in Unix time.
         text: Optional[:class:`str`]
             Message Content
         caption: Optional[:class:`str`]
             Caption for the animation, audio, document, photo, video or voice.
         forward_from: Optional[:class:`bale.User`]
             For forwarded messages, sender of the original message.
         forward_from_chat: Optional[:class:`bale.Chat`]
             For messages forwarded from channels or from anonymous administrators, information about the original sender chat.
         reply_to_message: Optional[:class:`bale.Message`]
-            For replies, the original message. Note that the Message object in this field will not contain further reply_to_message fields even if it itself is a reply.
+            For replies, the original message. Note that the Message object in this field will not contain further
+            reply_to_message fields even if it itself is a reply.
         contact: Optional[:class:`bale.ContactMessage`]
             Message is a shared contact, information about the contact.
         location: Optional[:class:`bale.Location`]
             Message is a shared location, information about the location.
         document: Optional[:class:`bale.Document`]
             Message is a general file, information about the file.
+        video: Optional[:class:`bale.Video`]
+            Message is a video, information about the video.
+        audio: Optional[:class:`bale.Audio`]
+            Message is an audio, information about the Audio.
         new_chat_members: Optional[List[:class:`bale.User`]]
-            New members that were added to the group or supergroup and information about them (the bot itself may be one of these members). This list is empty if the message does not contain new chat members.
+            New members that were added to the group or supergroup and information about them (the bot itself may be
+            one of these members). This list is empty if the message does not contain new chat members.
         left_chat_member: Optional[:class:`bale.User`]
             A member was removed from the group, information about them (this member may be the bot itself).
         invoice: Optional[:class:`bale.Invoice`]
             Message is an invoice for a payment, information about the invoice.
     """
     __slots__ = (
         "text", "caption", "from_user", "_author", "contact", "location", "chat", "message_id", "forward_from",
         "forward_from_chat", "forward_from_message_id", "date_code", "date",
-        "edit_date", "audio", "document", "photos", "voice", "location", "invoice", "new_chat_members",
+        "edit_date", "audio", "document", "video", "photos", "location", "invoice", "new_chat_members",
         "left_chat_member", "reply_to_message",
         "invoice", "bot"
     )
 
     def __init__(self, message_id: str, date: datetime, text: Optional[str] = None, caption: Optional[str] = None,
                  forward_from: Optional["User"] = None, forward_from_chat: Optional["Chat"] = None,
                  forward_from_message_id: Optional[str] = None, from_user: Optional["User"] = None,
                  document: Optional["Document"] = None,
                  contact: Optional["ContactMessage"] = None, location: Optional["Location"] = None,
-                 chat: Optional["Chat"] = None, photos: Optional[List["Photo"]] = None,
-                 reply_to_message: Optional["Message"] = None, invoice: Optional["Invoice"] = None,
+                 chat: Optional["Chat"] = None, video: Optional["Video"] = None,
+                 photos: Optional[List["Photo"]] = None, reply_to_message: Optional["Message"] = None,
+                 invoice: Optional["Invoice"] = None, audio: Optional["Audio"] = None,
                  bot: 'Bot' = None, **options):
         self.message_id: str = message_id if message_id is not None else None
         self.date = date if date is not None else None
 
         self.text: str | None = text if text is not None else None
         self.chat: Chat | None = chat if chat is not None else None
         self.reply_to_message: Message | None = reply_to_message if reply_to_message is not None else reply_to_message
         self.from_user: User | None = from_user if from_user is not None else None
         self.forward_from: User | None = forward_from if forward_from is not None else None
         self.forward_from_message_id: str = forward_from_message_id if forward_from_message_id is not None else None
         self.forward_from_chat: Chat | None = forward_from_chat if forward_from_chat is not None else None
         self.caption: str | None = caption if caption is not None else None
         self.document = document if document is not None else None
+        self.video = video if video is not None else None
+        self.audio = audio if audio is not None else None
         self.photos = photos if photos is not None else None
         self.contact: ContactMessage | None = contact if contact is not None else None
         self.location: Location | None = location if location is not None else None
         self.new_chat_members: List[User] | None = options.get("new_chat_members")
         self.left_chat_member: User | None = options.get("left_chat_member")
         self.invoice = invoice
         self.bot: Bot = bot if bot is not None else None
 
     @property
     def author(self):
         """An alias for :attr:`from_user`"""
         return self.from_user
 
     @property
-    def content(self):
+    def attachment(self) -> Optional["File"]:
+        """Optional[:class:`bale.File`]: Represents the message attachment. ``None`` if the message don't have any attachments"""
+        attachment = self.video or self.photos or self.audio or self.document
+        if not attachment:
+            return
+
+        if isinstance(attachment, list):
+            attachment = attachment[0]
+
+        return attachment.base_file
+
+    @property
+    def content(self) -> Optional[str]:
+        """Optional[:class:`str`]: Represents the message content. ``None`` if the message don't have text or caption"""
         return self.caption or self.text
 
     @content.setter
-    def content(self, _value):
+    def content(self, _value: str) -> NoReturn:
         if not isinstance(_value, str):
             raise TypeError("content must be type of str")
+
         if self.caption:
             self.caption = _value
         elif self.text:
             self.text = _value
 
     @property
-    def chat_id(self):
-        if self.chat:
-            return self.chat.chat_id
-        return None
+    def chat_id(self) -> Optional[str | int]:
+        """:class:`str` | :class:`int`: Represents the Unique identifier of Conversation the message belongs to."""
+        return self.chat.chat_id
 
     @property
-    def reply_to_message_id(self):
-        if self.reply_to_message:
-            return self.reply_to_message.message_id
-        return None
-
-    @reply_to_message_id.setter
-    def reply_to_message_id(self, _value):
-        if not isinstance(_value, int):
-            raise TypeError("_value must be type of int")
+    def reply_to_message_id(self) -> Optional[str]:
+        """Optional[:class:`str`]: Represents the Unique identifier of Original message, if the message has been replied. ``None`` If the message is not replied"""
+        if not self.reply_to_message:
+            return
+
+        return self.reply_to_message.message_id
 
-        if self.reply_to_message:
-            self.reply_to_message.message_id = _value
 
     @classmethod
     def from_dict(cls, data: dict, bot):
         options = {}
         if data.get("new_chat_members"):
             options["new_chat_members"] = [User.from_dict(bot=bot, data=i) for i in data.get("new_chat_members")]
         if data.get("left_chat_member"):
@@ -163,16 +181,17 @@
                    forward_from_chat=Chat.from_dict(bot=bot, data=data.get("forward_from_chat")) if data.get(
                        "forward_from_chat") else None,
                    forward_from_message_id=str(data.get("forward_from_message_id")) if data.get(
                        "forward_from_message_id") else None,
                    document=Document.from_dict(bot=bot, data=data.get("document")) if data.get("document") else None,
                    contact=ContactMessage.from_dict(data=data.get("contact")) if data.get("contact") else None,
                    location=Location.from_dict(data=data.get("location")) if data.get("location") else None,
-                   photos=[Photo.from_dict(data=photo_payload) for photo_payload in data.get("photo")] if data.get(
-                       "photo") else None,
+                   audio=Audio.from_dict(data=data.get("audio"), bot=bot) if data.get("audio") else None,
+                   photos=[Photo.from_dict(data=photo_payload, bot=bot) for photo_payload in data.get("photo")] if data.get(
+                       "photo") else None, video=Video.from_dict(data=data.get("video"), bot=bot) if data.get("video") else None,
                    invoice=Invoice.from_dict(data=data.get("invoice")) if data.get("invoice") else None, **options)
 
     def to_dict(self):
         data = {"message_id": self.message_id, "date": self.date, "text": self.text}
 
         if self.chat:
             data["chat"] = self.chat.to_dict()
@@ -180,14 +199,18 @@
             data["from"] = self.from_user.to_dict()
         if self.caption:
             data["caption"] = self.caption
         if self.document:
             data["document"] = self.document.to_dict()
         if self.photos:
             data["photo"] = [photo.to_dict() for photo in self.photos]
+        if self.video:
+            data["video"] = self.video.to_dict()
+        if self.audio:
+            data["audio"] = self.audio.to_dict()
         if self.contact:
             data["contact"] = self.contact.to_dict()
         if self.location:
             data["location"] = self.location.to_dict()
         if self.new_chat_members:
             data["new_chat_members"] = self.new_chat_members
         if self.forward_from:
@@ -197,15 +220,15 @@
         if self.left_chat_member:
             data["left_chat_member"] = self.left_chat_member.to_dict()
         if self.reply_to_message_id:
             data["reply_to_message_id"] = self.reply_to_message_id
 
         return data
 
-    async def reply(self, text: str, *, components: Optional[Components | RemoveComponents] = None):
+    async def reply(self, text: str, *, components: Optional[Components | RemoveMenuKeyboard] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_message`.
         """
         return await self.bot.send_message(self.chat_id, text, components=components,
                                            reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
     async def forward(self, chat_id: str | int):
@@ -231,28 +254,22 @@
     async def reply_video(self, video: bytes | str | "Video", *, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_video`.
         """
         return await self.bot.send_video(self.chat_id, video, caption=caption,
                                          reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-    async def reply_invoice(self, title: str, description: str, provider_token: str, prices: List["Price"], *,
-                            photo_url: Optional[str] = None,
-                            need_name: Optional[bool] = False, need_phone_number: Optional[bool] = False,
-                            need_email: Optional[bool] = False,
-                            need_shipping_address: Optional[bool] = False, is_flexible: Optional[bool] = True):
-        """
-        For the documentation of the arguments, please see :meth:`bale.Bot.send_invoice`
-        """
-        return await self.bot.send_invoice(self.chat_id, title, description, provider_token, prices,
-                                           photo_url=photo_url, need_name=need_name, need_email=need_email,
-                                           need_phone_number=need_phone_number,
-                                           need_shipping_address=need_shipping_address, is_flexible=is_flexible)
+    async def reply_audio(self, audio: bytes | str | "Audio", *, caption: Optional[str] = None):
+        """
+        For the documentation of the arguments, please see :meth:`bale.Bot.send_audio`.
+        """
+        return await self.bot.send_video(self.chat_id, audio, caption=caption,
+                                         reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-    async def edit(self, text: str, *, components: "Components" | "RemoveComponents" = None) -> Message:
+    async def edit(self, text: str, *, components: "Components" | "RemoveMenuKeyboard" = None) -> Message:
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.edit_message`
         """
         return await self.bot.edit_message(self.chat_id, self.message_id, text, components=components)
 
     async def delete(self):
         """
```

### Comparing `python-bale-bot-2.4.5/bale/payments/invoice.py` & `python-bale-bot-2.4.6/bale/payments/invoice.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.5/bale/payments/price.py` & `python-bale-bot-2.4.6/bale/payments/price.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.5/bale/permissions.py` & `python-bale-bot-2.4.6/bale/permissions.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.5/bale/request/http.py` & `python-bale-bot-2.4.6/bale/request/http.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,195 +23,123 @@
 """
 from bale.version import BALE_API_BASE_URL, BALE_API_FILE_URL
 import asyncio
 import aiohttp
 from ..error import (NetworkError, TimeOut, NotFound, Forbidden, APIError, BaleError, HTTPClientError, RateLimited, HTTPException)
 from .parser import ResponseParser
 from .utils import ResponseStatusCode
-from collections import deque
 
 __all__ = ("HTTPClient", "Route")
 
-
-class RateLimit:
-	__slots__ = (
-		"_loop",
-		"_requests",
-		"_has_rate_limit"
-	)
-	def __init__(self, loop):
-		self._has_rate_limit = False
-		self._requests = deque()
-		self._loop = loop
-
-	def enable(self):
-		self._has_rate_limit = True
-
-	def _next(self):
-		while self._requests:
-			future = self._requests.popleft()
-
-			if not future.done():
-				future.set_result(None)
-				break
-
-	def _wake(self):
-		while self._requests:
-			future = self._requests.popleft()
-			if not future.done():
-				future.set_result(None)
-
-	async def new_request(self):
-		if self._has_rate_limit:
-			future = self._loop.create_future()
-			self._requests.append(future)
-
-			try:
-				await future
-			except:
-				future.cancel()
-				if not self._has_rate_limit:
-					self._next()
-				raise
-
-	async def __aenter__(self):
-		await self.new_request()
-		return self
-
-	async def __aexit__(self, exc_type, exc_val, exc_tb):
-		if len(self._requests) > 0:
-			self._next()
-		else:
-			self._has_rate_limit = False
-
-	def __bool__(self):
-		return self._has_rate_limit
-
 class Route:
 	"""Route Class for http"""
 	__slots__ = (
 		"method",
-		"path",
-		"token",
-		"_base"
+		"endpoint",
+		"token"
 	)
 
-	def __init__(self, method: str, path: str, token: str):
+	def __init__(self, method: str, endpoint: str, token: str):
 		if not isinstance(token, str):
 			raise TypeError("token param must be str.")
 		self.method = method
-		self.path = path
+		self.endpoint = endpoint
 		self.token = token
-		self._base = BALE_API_BASE_URL
 
 	@property
 	def url(self):
-		"""finally url"""
-		return self._base + "bot" + self.token + "/" + self.path
-
-	def set_base(self, _value):
-		"""Set base url for route"""
-		self._base = _value
+		"""export url for request"""
+		return "{base_url}bot{token}/{endpoint}".format(base_url = BALE_API_BASE_URL, token = self.token, endpoint = self.endpoint)
 
 class HTTPClient:
 	"""Send a Request to BALE API Server"""
 
 	__slots__ = (
 		"_loop",
 		"token",
-		"__session",
-		"rate_limit",
-		"base_url"
+		"__session"
 	)
 
-	def __init__(self, loop, token=None, base_url = None):
+	def __init__(self, loop, token):
 		self.__session = None
 		self._loop: asyncio.AbstractEventLoop = loop
 		self.token = token
-		self.rate_limit = RateLimit(self.loop)
-		self.base_url: str = base_url
 
 	def is_closed(self):
 		return self.__session is None
 
 	@property
 	def loop(self):
 		return self._loop
 
 	@loop.setter
 	def loop(self, _value):
 		self._loop = _value
-		self.rate_limit._loop = _value
 
 	def reload_session(self):
 		"""Reset Session"""
 		if self.__session and self.__session.closed:
 			self.__session = aiohttp.ClientSession(loop=self.loop, connector=aiohttp.TCPConnector(keepalive_timeout=20.0))
 
 	async def start(self):
 		"""Start Http client"""
+		if self.__session:
+			raise RuntimeError("HTTPClient started ")
 		self.__session = aiohttp.ClientSession(loop=self.loop, connector=aiohttp.TCPConnector(keepalive_timeout=20.0))
 
 	async def close(self):
 		"""Close Session connection"""
 		if self.__session:
 			await self.__session.close()
 			self.__session = None
 
 	async def request(self, route: Route, **kwargs):
-		if self.base_url:
-			route.set_base(self.base_url)
 		url = route.url
 		method = route.method
-		async with self.rate_limit:
-			for tries in range(5):
-				try:
-					async with self.__session.request(method=method, url=url, **kwargs) as response:
-						response: aiohttp.ClientResponse = response
-						parsed_response = await ResponseParser.from_response(response)
-						if response.status == ResponseStatusCode.OK:
-							return parsed_response
-						elif response.status == ResponseStatusCode.NOT_FOUND:
-							raise NotFound(parsed_response.description)
-						elif response.status == ResponseStatusCode.PERMISSION_DENIED:
+		for tries in range(5):
+			try:
+				async with self.__session.request(method=method, url=url, **kwargs) as response:
+					response: aiohttp.ClientResponse = response
+					parsed_response = await ResponseParser.from_response(response)
+					if response.status == ResponseStatusCode.OK:
+						return parsed_response
+					elif response.status == ResponseStatusCode.NOT_FOUND:
+						raise NotFound(parsed_response.description)
+					elif response.status == ResponseStatusCode.PERMISSION_DENIED:
+						raise Forbidden()
+					elif not parsed_response.ok or response.status in (ResponseStatusCode.NOT_INCORRECT, ResponseStatusCode.RATE_LIMIT):
+						if parsed_response.description == HTTPClientError.USER_OR_CHAT_NOT_FOUND:
+							raise NotFound("User or Chat not Found")
+						elif response.status == ResponseStatusCode.RATE_LIMIT or parsed_response.description in (HTTPClientError.RATE_LIMIT, HTTPClientError.LOCAL_RATE_LIMIT):
+							if tries >= 4:
+								raise RateLimited()
+
+							await asyncio.sleep((1 + tries) * 2)
+							continue
+						elif parsed_response.description == HTTPClientError.PERMISSION_DENIED:
 							raise Forbidden()
-						elif not parsed_response.ok or response.status in (ResponseStatusCode.NOT_INCORRECT, ResponseStatusCode.RATE_LIMIT):
-							if parsed_response.description == HTTPClientError.USER_OR_CHAT_NOT_FOUND:
-								raise NotFound("User or Chat not Found")
-							elif response.status == ResponseStatusCode.RATE_LIMIT or parsed_response.description in (HTTPClientError.RATE_LIMIT, HTTPClientError.LOCAL_RATE_LIMIT):
-								if tries >= 4:
-									raise RateLimited()
-
-								if bool(self.rate_limit):
-									await self.rate_limit.new_request()
-								else:
-									self.rate_limit.enable()
-									await asyncio.sleep(tries * 2 + 1)
-								continue
-							elif parsed_response.description == HTTPClientError.PERMISSION_DENIED:
-								raise Forbidden()
-
-							raise APIError(
-									str(parsed_response.error_code), parsed_response.description
-								)
-				except aiohttp.ClientConnectorError as error:
-					raise NetworkError(str(error))
-				except aiohttp.ServerTimeoutError:
-					raise TimeOut()
-				except aiohttp.ClientOSError as error:
-					raise BaleError(str(error))
-				except Exception as error:
-					raise HTTPException(error)
+
+						raise APIError(
+								str(parsed_response.error_code), parsed_response.description
+							)
+			except aiohttp.ClientConnectorError as error:
+				raise NetworkError(str(error))
+			except aiohttp.ServerTimeoutError:
+				raise TimeOut()
+			except aiohttp.ClientOSError as error:
+				raise BaleError(str(error))
+			except Exception as error:
+				raise HTTPException(error)
 
 	async def get_file(self, file_id):
-		async with self.__session.get(BALE_API_FILE_URL + "/" + "bot" + self.token + "/" + file_id) as response:
+		async with self.__session.get("{base_file_url}/bot{token}/{file_id}".format(base_file_url = BALE_API_FILE_URL, token = self.token, file_id = file_id)) as response:
 			if response.status == ResponseStatusCode.OK:
 				return await response.read()
-			elif response.status == ResponseStatusCode.NOT_FOUND:
-				raise NotFound("Document is not Found")
+			elif response.status in (ResponseStatusCode.NOT_INCORRECT, ResponseStatusCode.NOT_FOUND):
+				raise NotFound("File is not Found")
 			elif response.status == ResponseStatusCode.PERMISSION_DENIED:
 				raise Forbidden()
 			else:
 				error_payload = await response.json()
 				raise APIError(0, "UNKNOWN ERROR: {}".format(error_payload))
 
 		raise RuntimeError("failed to get file")
```

### Comparing `python-bale-bot-2.4.5/bale/request/parser.py` & `python-bale-bot-2.4.6/bale/request/parser.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.5/bale/update.py` & `python-bale-bot-2.4.6/bale/update.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.5/bale/updater.py` & `python-bale-bot-2.4.6/bale/updater.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,35 +109,38 @@
         self.bot.dispatch("ready")
         await self.action_getupdates()
 
     async def action_getupdates(self):
         while self._is_running:
             try:
                 updates = await self.bot.get_updates(offset=self._last_offset)
-                for update in updates:
-                    await self.call_to_dispatch(update)
+            except Exception as exc:
+                await self.bot.on_error("getUpdates", exc)
+            else:
+                if updates:
+                    for update in updates:
+                        await self.call_to_dispatch(update)
 
-                self._last_offset = updates[-1].update_id if bool(updates) else self._last_offset
+                    self._last_offset = updates[-1].update_id
                 if self.interval:
                     await asyncio.sleep(self.interval)
-            except Exception as exc:
-                await self.bot.on_error("getUpdates", exc)
 
     async def call_to_dispatch(self, update: "Update"):
         self.bot.dispatch("update", update)
         if update.type.is_callback_update():
             self.bot.dispatch("callback", update.callback_query)
         elif update.type.is_message_update():
             self.bot.dispatch("message", update.message)
             if update.message.left_chat_member:
                 self.bot.dispatch("member_chat_leave", update.message, update.message.chat, update.message.left_chat_member)
             for user in update.message.new_chat_members or []:
                 self.bot.dispatch("member_chat_join", update.message, update.message.chat, user)
         elif update.type.is_edited_message():
             self.bot.dispatch("edited_message", update.edited_message)
 
-    def stop(self):
+    async def stop(self):
         """Stop running and Stop `poll_event` loop"""
-        if not self._is_running:
-            raise RuntimeError("Updater is not running")
+        async with self.__lock:
+            if not self._is_running:
+                raise RuntimeError("Updater is not running")
 
-        self._is_running = False
+            self._is_running = False
```

### Comparing `python-bale-bot-2.4.5/bale/user.py` & `python-bale-bot-2.4.6/bale/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, List
 if TYPE_CHECKING:
-    from bale import Bot, Photo, Document, Components, RemoveComponents, Price, Location, ContactMessage
+    from bale import Bot, Photo, Document, Components, RemoveMenuKeyboard, Price, Location, ContactMessage, Video, Audio
 
 
 class User:
     """This object represents a Bale user or bot.
 
     Attributes
     ----------
@@ -67,15 +67,15 @@
         return f"@{self.username}" if self.username else None
 
     @property
     def chat_id(self) -> str:
         """:class:`str`"""
         return str(self.user_id)
 
-    async def send(self, text: str, components: Optional["Components" | "RemoveComponents"] =None):
+    async def send(self, text: str, components: Optional["Components" | "RemoveMenuKeyboard"] =None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_message`.
         """
         return await self.bot.send_message(self.chat_id, text, components=components)
 
     async def send_document(self, document: bytes | str | "Document", *, caption: Optional[str] = None):
         """
@@ -85,14 +85,26 @@
 
     async def send_photo(self, photo: bytes | str | "Photo", *, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_photo`.
         """
         return await self.bot.send_photo(self.chat_id, photo, caption=caption)
 
+    async def send_video(self, video: bytes | str | "Video", *, caption: Optional[str] = None):
+        """
+        For the documentation of the arguments, please see :meth:`bale.Bot.send_video`.
+        """
+        return await self.bot.send_video(self.chat_id, video, caption=caption)
+
+    async def send_audio(self, audio: bytes | str | "Audio", *, caption: Optional[str] = None):
+        """
+        For the documentation of the arguments, please see :meth:`bale.Bot.send_audio`.
+        """
+        return await self.bot.send_audio(self.chat_id, audio, caption=caption)
+
     async def send_location(self, location: "Location"):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_location`.
         """
         return await self.bot.send_location(self.chat_id, location)
 
     async def send_contact(self, contact: "ContactMessage"):
```

### Comparing `python-bale-bot-2.4.5/python_bale_bot.egg-info/PKG-INFO` & `python-bale-bot-2.4.6/python_bale_bot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: python-bale-bot
-Version: 2.4.5
+Version: 2.4.6
 Summary: An API wrapper for Bale written in Python
 Home-page: https://github.com/python-bale-bot/python-bale-bot/
 Author: Kian Ahmadian
 License: MIT License
 Project-URL: Documentation, https://docs.python-bale-bot.ir/en/master/
-Project-URL: Changelog, https://python-bale-bot.rtfd.io/en/master/whats_new.html
+Project-URL: Changelog, https:///docs.python-bale-bot.ir/en/master/whats_new.html
 Project-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
 Keywords: bale,bale-bot,framework,bot
 Platform: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
@@ -55,7 +55,9 @@
 <p><b>The <a href="https://python-bale-bot.readthedocs.io/en/master">package documentation</a> is the technical reference for python-bale-bot. It contains descriptions of all available classes, modules, methods and arguments as well as the changelog.</b></p>
 
 
 ## Contact to Developers
 [![Email](https://img.shields.io/badge/Email-python--bale--bot@googlegroups.com-green?logo=Gmail&logoColor=white)](mailto:python-bale-bot@googlegroups.com)
 [![Discord](https://img.shields.io/badge/Support_Server-bYHEzyDe2j-green?logo=Discord&logoColor=white)](https://discord.gg/bYHEzyDe2j)
 [![Our Site](https://img.shields.io/badge/Our_site-python--bale--bot.ir-green?logo=GitHub&logoColor=white)](https://python-bale-bot.ir)
+
+
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.5 Summary: An API
+Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.6 Summary: An API
 wrapper for Bale written in Python Home-page: https://github.com/python-bale-
 bot/python-bale-bot/ Author: Kian Ahmadian License: MIT License Project-URL:
 Documentation, https://docs.python-bale-bot.ir/en/master/ Project-URL:
-Changelog, https://python-bale-bot.rtfd.io/en/master/whats_new.html Project-
+Changelog, https:///docs.python-bale-bot.ir/en/master/whats_new.html Project-
 URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
 Keywords: bale,bale-bot,framework,bot Platform: Windows Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: docs License-File:
 LICENSE # python-bale-bot
                            [python-bale-bot image]
                   An API wrapper for Bale written in Python.
```

### Comparing `python-bale-bot-2.4.5/python_bale_bot.egg-info/SOURCES.txt` & `python-bale-bot-2.4.6/python_bale_bot.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,34 +3,39 @@
 setup.py
 bale/__init__.py
 bale/__main__.py
 bale/bot.py
 bale/callbackquery.py
 bale/chat.py
 bale/chatmember.py
-bale/components.py
 bale/error.py
 bale/message.py
 bale/permissions.py
 bale/update.py
 bale/updater.py
 bale/user.py
+bale/utils.py
 bale/version.py
 bale/attachments/__init__.py
 bale/attachments/audio.py
 bale/attachments/contact.py
 bale/attachments/document.py
+bale/attachments/file.py
 bale/attachments/location.py
 bale/attachments/photo.py
 bale/attachments/video.py
 bale/payments/__init__.py
 bale/payments/invoice.py
 bale/payments/price.py
 bale/request/__init__.py
 bale/request/http.py
 bale/request/parser.py
 bale/request/utils.py
+bale/ui/__init__.py
+bale/ui/components.py
+bale/ui/inline_keyboard.py
+bale/ui/menu_keyboard.py
 python_bale_bot.egg-info/PKG-INFO
 python_bale_bot.egg-info/SOURCES.txt
 python_bale_bot.egg-info/dependency_links.txt
 python_bale_bot.egg-info/requires.txt
 python_bale_bot.egg-info/top_level.txt
```

### Comparing `python-bale-bot-2.4.5/setup.py` & `python-bale-bot-2.4.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from setuptools import setup, find_packages
 
 def get_readme_file() -> str:
-    """Get Readme File"""
     with open("README.md", encoding="utf-8") as f:
         readme_file = f.read()
     return readme_file
 
 extras_require = {
     'docs': [
         'sphinx==4.4.0',
@@ -14,23 +13,23 @@
         'typing-extensions>=4.3,<5',
     ]
 }
 
 if __name__ == "__main__":
     setup(
         name="python-bale-bot",
-        version="2.4.5",
+        version="2.4.6",
         platforms=["Windows", ],
         fullname="python-bale-bot",
         description="An API wrapper for Bale written in Python",
         author="Kian Ahmadian",
         license="MIT License",
         project_urls={
             "Documentation": "https://docs.python-bale-bot.ir/en/master/",
-            "Changelog": "https://python-bale-bot.rtfd.io/en/master/whats_new.html",
+            "Changelog": "https:///docs.python-bale-bot.ir/en/master/whats_new.html",
             "Bug Tracker": "https://github.com/python-bale-bot/python-bale-bot/issues",
             "Source Code": "https://github.com/python-bale-bot/python-bale-bot/"
         },
         keywords=["bale", "bale-bot", "framework", "bot"],
         python_requires='>=3.8',
         extras_require=extras_require,
         include_package_data=True,
```

