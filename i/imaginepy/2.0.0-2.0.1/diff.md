# Comparing `tmp/imaginepy-2.0.0.tar.gz` & `tmp/imaginepy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imaginepy-2.0.0.tar", last modified: Mon Jun 26 00:36:50 2023, max compression
+gzip compressed data, was "imaginepy-2.0.1.tar", last modified: Mon Jun 26 01:28:19 2023, max compression
```

## Comparing `imaginepy-2.0.0.tar` & `imaginepy-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 00:36:50.949813 imaginepy-2.0.0/
--rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     5376 2023-06-26 00:36:50.949313 imaginepy-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4510 2023-06-26 00:35:21.000000 imaginepy-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 00:36:50.933788 imaginepy-2.0.0/imaginepy/
--rw-rw-rw-   0        0        0      146 2023-06-25 23:44:15.000000 imaginepy-2.0.0/imaginepy/__init__.py
--rw-rw-rw-   0        0        0    11029 2023-06-26 00:08:10.000000 imaginepy-2.0.0/imaginepy/async_imagine.py
--rw-rw-rw-   0        0        0    44101 2023-06-25 23:52:33.000000 imaginepy-2.0.0/imaginepy/constants.py
--rw-rw-rw-   0        0        0      326 2023-06-25 22:17:39.000000 imaginepy-2.0.0/imaginepy/exceptions.py
--rw-rw-rw-   0        0        0    10572 2023-06-26 00:10:58.000000 imaginepy-2.0.0/imaginepy/sync_imagine.py
--rw-rw-rw-   0        0        0     1615 2023-06-25 22:15:48.000000 imaginepy-2.0.0/imaginepy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 00:36:50.948313 imaginepy-2.0.0/imaginepy.egg-info/
--rw-rw-rw-   0        0        0     5376 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-26 00:36:50.000000 imaginepy-2.0.0/imaginepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 00:36:50.950314 imaginepy-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-06-26 00:15:09.000000 imaginepy-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 01:28:19.820451 imaginepy-2.0.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-14 17:40:10.000000 imaginepy-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     5643 2023-06-26 01:28:19.819949 imaginepy-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4777 2023-06-26 01:24:09.000000 imaginepy-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 01:28:19.812937 imaginepy-2.0.1/imaginepy/
+-rw-rw-rw-   0        0        0      146 2023-06-25 23:44:15.000000 imaginepy-2.0.1/imaginepy/__init__.py
+-rw-rw-rw-   0        0        0    11138 2023-06-26 01:23:47.000000 imaginepy-2.0.1/imaginepy/async_imagine.py
+-rw-rw-rw-   0        0        0    44101 2023-06-25 23:52:33.000000 imaginepy-2.0.1/imaginepy/constants.py
+-rw-rw-rw-   0        0        0      326 2023-06-25 22:17:39.000000 imaginepy-2.0.1/imaginepy/exceptions.py
+-rw-rw-rw-   0        0        0    10572 2023-06-26 00:10:58.000000 imaginepy-2.0.1/imaginepy/sync_imagine.py
+-rw-rw-rw-   0        0        0     1615 2023-06-25 22:15:48.000000 imaginepy-2.0.1/imaginepy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-26 01:28:19.818949 imaginepy-2.0.1/imaginepy.egg-info/
+-rw-rw-rw-   0        0        0     5643 2023-06-26 01:28:19.000000 imaginepy-2.0.1/imaginepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-06-26 01:28:19.000000 imaginepy-2.0.1/imaginepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 01:28:19.000000 imaginepy-2.0.1/imaginepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-26 01:28:19.000000 imaginepy-2.0.1/imaginepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-26 01:28:19.000000 imaginepy-2.0.1/imaginepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-26 01:28:19.820451 imaginepy-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1251 2023-06-26 01:28:09.000000 imaginepy-2.0.1/setup.py
```

### Comparing `imaginepy-2.0.0/LICENSE` & `imaginepy-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imaginepy-2.0.0/PKG-INFO` & `imaginepy-2.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaginepy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python library to create Art with AI.
 Home-page: https://github.com/ItsCEED/imaginepy
 Author: CEED
 Author-email: 
 License: GPL-3.0-only
 Keywords: art,image,ai,stable-diffusion
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,17 +19,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-<b>>PyPi IS NOT UPDATE! PLEASE INSTALL FROM THE REPO!</b>
-<br>
-  
 <img src="https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/docs/imagine_logo.gif" width="10%">
 
 **ImaginePy**
 <br>
 <a href="https://discord.gg/axfkjqWR5E" target="_blank">
   <img src="https://discordapp.com/api/guilds/1110314971012808774/widget.png?style=banner4" alt="Discord Banner 4">
 </a>
@@ -92,81 +89,96 @@
 
 ## Usage
 
 The following is a minimal example of using ImaginePy in a script. It gets the generated image
 from the text and increases the quality.
 
 ```python
-from imaginepy import Imagine, Style, Ratio
+from imaginepy import Imagine
+from imaginepy.constants import *
+
 
 def main():
-    imagine = Imagine(style=Style.ANIME_V2)
+    imagine = Imagine()
 
     img_data = imagine.sdprem(
         prompt="Woman sitting on a table, looking at the sky, seen from behind",
-        style=Style.ANIME_V2,
-        ratio=Ratio.RATIO_16X9
+        style=Style.NO_STYLE,
+        ratio=Ratio.RATIO_16X9,
+        negative="",
+        seed=1000,
+        cfg=16,
+        model=Model.REALISTIC,
+        asbase64=False  # default is false, putting it here as presentation.
     )
 
     if img_data is None:
         print("An error occurred while generating the image.")
         return
 
-    img_data = imagine.upscale(image=img_data)
+    img_data = imagine.upscale(img_data)
 
     if img_data is None:
         print("An error occurred while upscaling the image.")
         return
 
     try:
         with open("example.jpeg", mode="wb") as img_file:
             img_file.write(img_data)
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
+
 if __name__ == "__main__":
     main()
 ```
 
 Async version
 
 ```python
 import asyncio
-from imaginepy import AsyncImagine, Style, Ratio
+from imaginepy import AsyncImagine
+from imaginepy.constants import *
 
 
 async def main():
-    imagine = AsyncImagine(style=Style.ANIME_V2)
-
-    img_data = await imagine.sdprem(
+    imagine = AsyncImagine()
+    img_data = imagine.sdprem(
         prompt="Woman sitting on a table, looking at the sky, seen from behind",
-        style=Style.ANIME_V2,
-        ratio=Ratio.RATIO_16X9
+        style=Style.NO_STYLE,
+        ratio=Ratio.RATIO_16X9,
+        negative="",
+        seed=1000,
+        cfg=16,
+        model=Model.REALISTIC,
+        asbase64=False  # default is false, putting it here as presentation.
     )
 
     if img_data is None:
         print("An error occurred while generating the image.")
         return
 
     img_data = await imagine.upscale(image=img_data)
 
     if img_data is None:
         print("An error occurred while upscaling the image.")
         return
 
-    await imagine.close()
     try:
         with open("example.png", mode="wb") as img_file:
             img_file.write(img_data)
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
+    await imagine.close()
+
 
 if __name__ == "__main__":
     asyncio.run(main())
+
 ```
 
 ## Credit
 
 - Imagine Icon &copy; Vyro AI & API
 - Original reverse and version by: [hyugogirubato]
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: imaginepy Version: 2.0.0 Summary: Python library to
+Metadata-Version: 2.1 Name: imaginepy Version: 2.0.1 Summary: Python library to
 create Art with AI. Home-page: https://github.com/ItsCEED/imaginepy Author:
 CEED Author-email: License: GPL-3.0-only Keywords: art,image,ai,stable-
 diffusion Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Utilities Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
-              >PyPi IS NOT UPDATE! PLEASE INSTALL FROM THE REPO!
  [https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/
                      docs/imagine_logo.gif] **ImaginePy**
                               [Discord_Banner_4]
                      [Python version] [Release] [Version]
 ## Features - ð¨ Turn words into art - ð Choose from an array of art
 styles - ð§ Adjust your masterpiece with creative controls! - ð¦ Stay ahead
 of the game with the ever-growing art library! - ð Generate wallpapers -
@@ -33,28 +32,31 @@
 running the `imaginepy` executable is somewhat different to a normal PIP
 installation. See [Venv's Docs] on various ways of making calls under the
 virtual-environment. [Python]: https://python.org [Venv's]: https://
 docs.python.org/3/tutorial/venv.html [Venv's Docs]: https://docs.python.org/3/
 library/venv.html [hyugogirubato]: https://github.com/hyugogirubato/pyImagine
 ## Usage The following is a minimal example of using ImaginePy in a script. It
 gets the generated image from the text and increases the quality. ```python
-from imaginepy import Imagine, Style, Ratio def main(): imagine = Imagine
-(style=Style.ANIME_V2) img_data = imagine.sdprem( prompt="Woman sitting on a
-table, looking at the sky, seen from behind", style=Style.ANIME_V2,
-ratio=Ratio.RATIO_16X9 ) if img_data is None: print("An error occurred while
-generating the image.") return img_data = imagine.upscale(image=img_data) if
-img_data is None: print("An error occurred while upscaling the image.") return
-try: with open("example.jpeg", mode="wb") as img_file: img_file.write(img_data)
-except Exception as e: print(f"An error occurred while writing the image to
-file: {e}") if __name__ == "__main__": main() ``` Async version ```python
-import asyncio from imaginepy import AsyncImagine, Style, Ratio async def main
-(): imagine = AsyncImagine(style=Style.ANIME_V2) img_data = await
-imagine.sdprem( prompt="Woman sitting on a table, looking at the sky, seen from
-behind", style=Style.ANIME_V2, ratio=Ratio.RATIO_16X9 ) if img_data is None:
-print("An error occurred while generating the image.") return img_data = await
-imagine.upscale(image=img_data) if img_data is None: print("An error occurred
-while upscaling the image.") return await imagine.close() try: with open
+from imaginepy import Imagine from imaginepy.constants import * def main():
+imagine = Imagine() img_data = imagine.sdprem( prompt="Woman sitting on a
+table, looking at the sky, seen from behind", style=Style.NO_STYLE,
+ratio=Ratio.RATIO_16X9, negative="", seed=1000, cfg=16, model=Model.REALISTIC,
+asbase64=False # default is false, putting it here as presentation. ) if
+img_data is None: print("An error occurred while generating the image.") return
+img_data = imagine.upscale(img_data) if img_data is None: print("An error
+occurred while upscaling the image.") return try: with open("example.jpeg",
+mode="wb") as img_file: img_file.write(img_data) except Exception as e: print
+(f"An error occurred while writing the image to file: {e}") if __name__ ==
+"__main__": main() ``` Async version ```python import asyncio from imaginepy
+import AsyncImagine from imaginepy.constants import * async def main(): imagine
+= AsyncImagine() img_data = imagine.sdprem( prompt="Woman sitting on a table,
+looking at the sky, seen from behind", style=Style.NO_STYLE,
+ratio=Ratio.RATIO_16X9, negative="", seed=1000, cfg=16, model=Model.REALISTIC,
+asbase64=False # default is false, putting it here as presentation. ) if
+img_data is None: print("An error occurred while generating the image.") return
+img_data = await imagine.upscale(image=img_data) if img_data is None: print("An
+error occurred while upscaling the image.") return try: with open
 ("example.png", mode="wb") as img_file: img_file.write(img_data) except
 Exception as e: print(f"An error occurred while writing the image to file:
-{e}") if __name__ == "__main__": asyncio.run(main()) ``` ## Credit - Imagine
-Icon © Vyro AI & API - Original reverse and version by: [hyugogirubato] ##
-License [GNU General Public License, Version 3.0](LICENSE)
+{e}") await imagine.close() if __name__ == "__main__": asyncio.run(main()) ```
+## Credit - Imagine Icon © Vyro AI & API - Original reverse and version by:
+[hyugogirubato] ## License [GNU General Public License, Version 3.0](LICENSE)
```

### Comparing `imaginepy-2.0.0/README.md` & `imaginepy-2.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 <div align="center">
-<b>>PyPi IS NOT UPDATE! PLEASE INSTALL FROM THE REPO!</b>
-<br>
-  
 <img src="https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/docs/imagine_logo.gif" width="10%">
 
 **ImaginePy**
 <br>
 <a href="https://discord.gg/axfkjqWR5E" target="_blank">
   <img src="https://discordapp.com/api/guilds/1110314971012808774/widget.png?style=banner4" alt="Discord Banner 4">
 </a>
@@ -68,81 +65,96 @@
 
 ## Usage
 
 The following is a minimal example of using ImaginePy in a script. It gets the generated image
 from the text and increases the quality.
 
 ```python
-from imaginepy import Imagine, Style, Ratio
+from imaginepy import Imagine
+from imaginepy.constants import *
+
 
 def main():
-    imagine = Imagine(style=Style.ANIME_V2)
+    imagine = Imagine()
 
     img_data = imagine.sdprem(
         prompt="Woman sitting on a table, looking at the sky, seen from behind",
-        style=Style.ANIME_V2,
-        ratio=Ratio.RATIO_16X9
+        style=Style.NO_STYLE,
+        ratio=Ratio.RATIO_16X9,
+        negative="",
+        seed=1000,
+        cfg=16,
+        model=Model.REALISTIC,
+        asbase64=False  # default is false, putting it here as presentation.
     )
 
     if img_data is None:
         print("An error occurred while generating the image.")
         return
 
-    img_data = imagine.upscale(image=img_data)
+    img_data = imagine.upscale(img_data)
 
     if img_data is None:
         print("An error occurred while upscaling the image.")
         return
 
     try:
         with open("example.jpeg", mode="wb") as img_file:
             img_file.write(img_data)
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
+
 if __name__ == "__main__":
     main()
 ```
 
 Async version
 
 ```python
 import asyncio
-from imaginepy import AsyncImagine, Style, Ratio
+from imaginepy import AsyncImagine
+from imaginepy.constants import *
 
 
 async def main():
-    imagine = AsyncImagine(style=Style.ANIME_V2)
-
-    img_data = await imagine.sdprem(
+    imagine = AsyncImagine()
+    img_data = imagine.sdprem(
         prompt="Woman sitting on a table, looking at the sky, seen from behind",
-        style=Style.ANIME_V2,
-        ratio=Ratio.RATIO_16X9
+        style=Style.NO_STYLE,
+        ratio=Ratio.RATIO_16X9,
+        negative="",
+        seed=1000,
+        cfg=16,
+        model=Model.REALISTIC,
+        asbase64=False  # default is false, putting it here as presentation.
     )
 
     if img_data is None:
         print("An error occurred while generating the image.")
         return
 
     img_data = await imagine.upscale(image=img_data)
 
     if img_data is None:
         print("An error occurred while upscaling the image.")
         return
 
-    await imagine.close()
     try:
         with open("example.png", mode="wb") as img_file:
             img_file.write(img_data)
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
+    await imagine.close()
+
 
 if __name__ == "__main__":
     asyncio.run(main())
+
 ```
 
 ## Credit
 
 - Imagine Icon &copy; Vyro AI & API
 - Original reverse and version by: [hyugogirubato]
```

### Comparing `imaginepy-2.0.0/imaginepy/async_imagine.py` & `imaginepy-2.0.1/imaginepy/async_imagine.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 class AsyncImagine:
 
     def __init__(self, restricted: bool = True):
         self.restricted = restricted
         self.api = "https://inferenceengine.vyro.ai"
         self.cdn = "https://1966211409.rsc.cdn77.org/appStuff/imagine-fncisndcubnsduigfuds"
         self.version = 1
+        self.client = httpx.AsyncClient()
+
+    async def close(self):
+        await self.client.aclose()
 
     async def _request(self, **kwargs) -> Response:
         headers = {"accept": "*/*", "user-agent": "okhttp/4.10.0"}
         headers.update(kwargs.get("headers") or {})
 
         data = clear_dict(kwargs.get("data"))
         if data:
```

### Comparing `imaginepy-2.0.0/imaginepy/constants.py` & `imaginepy-2.0.1/imaginepy/constants.py`

 * *Files identical despite different names*

### Comparing `imaginepy-2.0.0/imaginepy/sync_imagine.py` & `imaginepy-2.0.1/imaginepy/sync_imagine.py`

 * *Files identical despite different names*

### Comparing `imaginepy-2.0.0/imaginepy/utils.py` & `imaginepy-2.0.1/imaginepy/utils.py`

 * *Files identical despite different names*

### Comparing `imaginepy-2.0.0/imaginepy.egg-info/PKG-INFO` & `imaginepy-2.0.1/imaginepy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imaginepy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Python library to create Art with AI.
 Home-page: https://github.com/ItsCEED/imaginepy
 Author: CEED
 Author-email: 
 License: GPL-3.0-only
 Keywords: art,image,ai,stable-diffusion
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,17 +19,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
-<b>>PyPi IS NOT UPDATE! PLEASE INSTALL FROM THE REPO!</b>
-<br>
-  
 <img src="https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/docs/imagine_logo.gif" width="10%">
 
 **ImaginePy**
 <br>
 <a href="https://discord.gg/axfkjqWR5E" target="_blank">
   <img src="https://discordapp.com/api/guilds/1110314971012808774/widget.png?style=banner4" alt="Discord Banner 4">
 </a>
@@ -92,81 +89,96 @@
 
 ## Usage
 
 The following is a minimal example of using ImaginePy in a script. It gets the generated image
 from the text and increases the quality.
 
 ```python
-from imaginepy import Imagine, Style, Ratio
+from imaginepy import Imagine
+from imaginepy.constants import *
+
 
 def main():
-    imagine = Imagine(style=Style.ANIME_V2)
+    imagine = Imagine()
 
     img_data = imagine.sdprem(
         prompt="Woman sitting on a table, looking at the sky, seen from behind",
-        style=Style.ANIME_V2,
-        ratio=Ratio.RATIO_16X9
+        style=Style.NO_STYLE,
+        ratio=Ratio.RATIO_16X9,
+        negative="",
+        seed=1000,
+        cfg=16,
+        model=Model.REALISTIC,
+        asbase64=False  # default is false, putting it here as presentation.
     )
 
     if img_data is None:
         print("An error occurred while generating the image.")
         return
 
-    img_data = imagine.upscale(image=img_data)
+    img_data = imagine.upscale(img_data)
 
     if img_data is None:
         print("An error occurred while upscaling the image.")
         return
 
     try:
         with open("example.jpeg", mode="wb") as img_file:
             img_file.write(img_data)
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
+
 if __name__ == "__main__":
     main()
 ```
 
 Async version
 
 ```python
 import asyncio
-from imaginepy import AsyncImagine, Style, Ratio
+from imaginepy import AsyncImagine
+from imaginepy.constants import *
 
 
 async def main():
-    imagine = AsyncImagine(style=Style.ANIME_V2)
-
-    img_data = await imagine.sdprem(
+    imagine = AsyncImagine()
+    img_data = imagine.sdprem(
         prompt="Woman sitting on a table, looking at the sky, seen from behind",
-        style=Style.ANIME_V2,
-        ratio=Ratio.RATIO_16X9
+        style=Style.NO_STYLE,
+        ratio=Ratio.RATIO_16X9,
+        negative="",
+        seed=1000,
+        cfg=16,
+        model=Model.REALISTIC,
+        asbase64=False  # default is false, putting it here as presentation.
     )
 
     if img_data is None:
         print("An error occurred while generating the image.")
         return
 
     img_data = await imagine.upscale(image=img_data)
 
     if img_data is None:
         print("An error occurred while upscaling the image.")
         return
 
-    await imagine.close()
     try:
         with open("example.png", mode="wb") as img_file:
             img_file.write(img_data)
     except Exception as e:
         print(f"An error occurred while writing the image to file: {e}")
 
+    await imagine.close()
+
 
 if __name__ == "__main__":
     asyncio.run(main())
+
 ```
 
 ## Credit
 
 - Imagine Icon &copy; Vyro AI & API
 - Original reverse and version by: [hyugogirubato]
```

#### html2text {}

```diff
@@ -1,19 +1,18 @@
-Metadata-Version: 2.1 Name: imaginepy Version: 2.0.0 Summary: Python library to
+Metadata-Version: 2.1 Name: imaginepy Version: 2.0.1 Summary: Python library to
 create Art with AI. Home-page: https://github.com/ItsCEED/imaginepy Author:
 CEED Author-email: License: GPL-3.0-only Keywords: art,image,ai,stable-
 diffusion Classifier: Development Status :: 5 - Production/Stable Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Utilities Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE
-              >PyPi IS NOT UPDATE! PLEASE INSTALL FROM THE REPO!
  [https://github.com/ItsCEED/ImaginePy-Midjourney-Free-Alternative/blob/main/
                      docs/imagine_logo.gif] **ImaginePy**
                               [Discord_Banner_4]
                      [Python version] [Release] [Version]
 ## Features - ð¨ Turn words into art - ð Choose from an array of art
 styles - ð§ Adjust your masterpiece with creative controls! - ð¦ Stay ahead
 of the game with the ever-growing art library! - ð Generate wallpapers -
@@ -33,28 +32,31 @@
 running the `imaginepy` executable is somewhat different to a normal PIP
 installation. See [Venv's Docs] on various ways of making calls under the
 virtual-environment. [Python]: https://python.org [Venv's]: https://
 docs.python.org/3/tutorial/venv.html [Venv's Docs]: https://docs.python.org/3/
 library/venv.html [hyugogirubato]: https://github.com/hyugogirubato/pyImagine
 ## Usage The following is a minimal example of using ImaginePy in a script. It
 gets the generated image from the text and increases the quality. ```python
-from imaginepy import Imagine, Style, Ratio def main(): imagine = Imagine
-(style=Style.ANIME_V2) img_data = imagine.sdprem( prompt="Woman sitting on a
-table, looking at the sky, seen from behind", style=Style.ANIME_V2,
-ratio=Ratio.RATIO_16X9 ) if img_data is None: print("An error occurred while
-generating the image.") return img_data = imagine.upscale(image=img_data) if
-img_data is None: print("An error occurred while upscaling the image.") return
-try: with open("example.jpeg", mode="wb") as img_file: img_file.write(img_data)
-except Exception as e: print(f"An error occurred while writing the image to
-file: {e}") if __name__ == "__main__": main() ``` Async version ```python
-import asyncio from imaginepy import AsyncImagine, Style, Ratio async def main
-(): imagine = AsyncImagine(style=Style.ANIME_V2) img_data = await
-imagine.sdprem( prompt="Woman sitting on a table, looking at the sky, seen from
-behind", style=Style.ANIME_V2, ratio=Ratio.RATIO_16X9 ) if img_data is None:
-print("An error occurred while generating the image.") return img_data = await
-imagine.upscale(image=img_data) if img_data is None: print("An error occurred
-while upscaling the image.") return await imagine.close() try: with open
+from imaginepy import Imagine from imaginepy.constants import * def main():
+imagine = Imagine() img_data = imagine.sdprem( prompt="Woman sitting on a
+table, looking at the sky, seen from behind", style=Style.NO_STYLE,
+ratio=Ratio.RATIO_16X9, negative="", seed=1000, cfg=16, model=Model.REALISTIC,
+asbase64=False # default is false, putting it here as presentation. ) if
+img_data is None: print("An error occurred while generating the image.") return
+img_data = imagine.upscale(img_data) if img_data is None: print("An error
+occurred while upscaling the image.") return try: with open("example.jpeg",
+mode="wb") as img_file: img_file.write(img_data) except Exception as e: print
+(f"An error occurred while writing the image to file: {e}") if __name__ ==
+"__main__": main() ``` Async version ```python import asyncio from imaginepy
+import AsyncImagine from imaginepy.constants import * async def main(): imagine
+= AsyncImagine() img_data = imagine.sdprem( prompt="Woman sitting on a table,
+looking at the sky, seen from behind", style=Style.NO_STYLE,
+ratio=Ratio.RATIO_16X9, negative="", seed=1000, cfg=16, model=Model.REALISTIC,
+asbase64=False # default is false, putting it here as presentation. ) if
+img_data is None: print("An error occurred while generating the image.") return
+img_data = await imagine.upscale(image=img_data) if img_data is None: print("An
+error occurred while upscaling the image.") return try: with open
 ("example.png", mode="wb") as img_file: img_file.write(img_data) except
 Exception as e: print(f"An error occurred while writing the image to file:
-{e}") if __name__ == "__main__": asyncio.run(main()) ``` ## Credit - Imagine
-Icon © Vyro AI & API - Original reverse and version by: [hyugogirubato] ##
-License [GNU General Public License, Version 3.0](LICENSE)
+{e}") await imagine.close() if __name__ == "__main__": asyncio.run(main()) ```
+## Credit - Imagine Icon © Vyro AI & API - Original reverse and version by:
+[hyugogirubato] ## License [GNU General Public License, Version 3.0](LICENSE)
```

### Comparing `imaginepy-2.0.0/setup.py` & `imaginepy-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='imaginepy',
-    version='2.0.0',
+    version='2.0.1',
     author='CEED',
     author_email='',
     description='Python library to create Art with AI.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/ItsCEED/imaginepy',
     license="GPL-3.0-only",
@@ -36,8 +36,8 @@
     python_requires='>=3.7',
     install_requires=[
         'aiohttp',
         'requests_toolbelt',
         'langdetect',
         'pybase64'
     ],
-)
+)
```

