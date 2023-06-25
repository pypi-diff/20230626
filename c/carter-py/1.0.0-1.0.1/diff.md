# Comparing `tmp/carter_py-1.0.0-py3-none-any.whl.zip` & `tmp/carter_py-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8152 bytes, number of entries: 10
+Zip file size: 8208 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-15 11:17 carterpy/__init__.py
 -rw-rw-rw-  2.0 fat     3249 b- defN 23-Jun-10 19:44 carterpy/async_carter.py
 -rw-rw-rw-  2.0 fat     3161 b- defN 23-Jun-10 19:48 carterpy/carter.py
 -rw-rw-rw-  2.0 fat     2763 b- defN 23-Jun-10 19:49 carterpy/classes.py
--rw-rw-rw-  2.0 fat      481 b- defN 23-Jun-10 19:50 carterpy/utils.py
--rw-rw-rw-  2.0 fat     8818 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1075 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/license.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      779 b- defN 23-Jun-10 22:43 carter_py-1.0.0.dist-info/RECORD
-10 files, 20494 bytes uncompressed, 6828 bytes compressed:  66.7%
+-rw-rw-rw-  2.0 fat      466 b- defN 23-Jun-25 22:55 carterpy/utils.py
+-rw-rw-rw-  2.0 fat     8919 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1075 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/license.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      779 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/RECORD
+10 files, 20580 bytes uncompressed, 6884 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: carterpy/classes.py
 Comment: 
 
 Filename: carterpy/utils.py
 Comment: 
 
-Filename: carter_py-1.0.0.dist-info/METADATA
+Filename: carter_py-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: carter_py-1.0.0.dist-info/WHEEL
+Filename: carter_py-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: carter_py-1.0.0.dist-info/license.txt
+Filename: carter_py-1.0.1.dist-info/license.txt
 Comment: 
 
-Filename: carter_py-1.0.0.dist-info/top_level.txt
+Filename: carter_py-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: carter_py-1.0.0.dist-info/RECORD
+Filename: carter_py-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## carterpy/utils.py

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 URLS = {
-    "say": "https://unstable.carterlabs.ai/api/say",
-    "opener": "https://unstable.carterlabs.ai/api/opener",
-    "personalise": "https://unstable.carterlabs.ai/api/personalise",
+    "say": "https://api.carterlabs.ai/api/say",
+    "opener": "https://api.carterlabs.ai/api/opener",
+    "personalise": "https://api.carterlabs.ai/api/personalise",
 }
 
 def convert_to_string(variable_name, value):
     try:
         return str(value)
     except:
         raise TypeError(f"{variable_name} must be convertible to a string, received {type(value)}")
```

## Comparing `carter_py-1.0.0.dist-info/METADATA` & `carter_py-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carter-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: A wrapper for the Carter API
 Home-page: https://github.com/LazyLyrics/carter-py
 Author: LazyLyrics
 Author-email: lazylyrics@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -21,22 +21,24 @@
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: Requests (==2.28.2)
 Requires-Dist: responses (==0.23.1)
 Requires-Dist: setuptools (==65.5.0)
 
 # carter-py: A Python Wrapper for the Carter API
 
-[GitHub](https://github.com/LazyLyrics/carter-py) | [PyPI](https://pypi.org/project/carter-py/) | [Change Log](https://github.com/LazyLyrics/carter-py/blob/main/CHANGELOG.md)| [Docs](https://lazylyrics.gitbook.io/carter-py/)
+[GitHub](https://github.com/LazyLyrics/carter-py) | [PyPI](https://pypi.org/project/carter-py/) | [Change Log](https://github.com/LazyLyrics/carter-py/blob/main/CHANGELOG.md)| [Docs](https://lazylyrics.gitbook.io/carter-py-v1/)
 
 `carter-py` is a Python package that provides a simple wrapper for the Carter API. It allows you to easily send text messages to the API and receive responses with minimal setup, and with the ability to add more complex functionality in upcoming releases.
 
 Please note that this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). As carter-py is built around an API which is still in beta, breaking changes may be introduced indirectly in minor releases. Major releases will be reserved for breaking changes to the way in carter-py is used. IE. function names, parameter depreciations etc. Where a breaking change is made on the API side, carter-py will be updated to reflect this change.
 
 I will continue to build carter-py with the intention of maintaining backwards compatibility, but this is not guaranteed. Previous versions of carter-py are always likely to be outdated as the API progresses. Please consult the changelog for any breaking changes and try to use the latest version of carter-py.
 
+For support and general chit chat, join the [discord](https://discord.gg/4w2Hs9QU)!
+
 ## Installation
 
 ```bash
 pip install `carter-py`
 ```
 
 This will install the latest version of `carter-py` and its dependencies.
@@ -62,15 +64,15 @@
 
 # Print the response text
 
 print(response.output_text)
 
 ```
 
-`carter.say()` returns an instance of the Interaction class, which contains the response text and other information about the interaction. It takes input text, and optionally a player ID, as arguments. If you don't specify a player ID, it will use a random one. Both must be strings or convertible to strings.
+`carter.say()` returns an instance of the Interaction class, which contains the response text and other information about the interaction. It takes input text, and optionally a user_id, as arguments. If you don't specify a player ID, it will use a random one. Both must be strings or convertible to strings.
 
 ### Opener
 
 Make use of the `/opener` endpoint to get a random opener from the Carter API. This is useful for when you want to start a conversation with a player.
 
 ```python
 # with carter object already created
@@ -82,15 +84,15 @@
 ### Personalise
 
 Make use of the `/personalise` endpoint to personalise any text in the style of your Carter character.
 
 ```python
 # with carter object already created
 
-interaction = carter.personalise("Hello, world!")
+interaction = carter.personalise("Hello, world!", "player_id")
 print(interaction.output_text)
 ```
 
 ### Speak
 
 When using any of the methods above, the output audio will **not** be returned by default as this currently introduces significant latency on the API end. If you want to receive the audio you have two options. You can set the `speak` parameter to `True` when creating the Carter object, or you can set it to `True` when calling the method. When calling a function `carter-py` will check to see if you have provided a speak parameter, if you have then it will override the default on the class. If you have not provided a speak parameter, then it will use the default on the class. Here's an example:
```

## Comparing `carter_py-1.0.0.dist-info/license.txt` & `carter_py-1.0.1.dist-info/license.txt`

 * *Files identical despite different names*

## Comparing `carter_py-1.0.0.dist-info/RECORD` & `carter_py-1.0.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 carterpy/__init__.py,sha256=SWOh6maoMonoFWKkqj5S42uK47hk7OgGgWjymXeXuZ4,67
 carterpy/async_carter.py,sha256=dYBI0cTpz9iEybofgJ4eeE-qZ6dcB0U5aB5YhzEF9rs,3249
 carterpy/carter.py,sha256=RQE1kLH3J6dJHf4z7acoaSpV3MoekSehVFDoIMt_xlc,3161
 carterpy/classes.py,sha256=pICxet4VQ8tqEQE8ZukpTdi9tS193pXySAJHgU1Adp8,2763
-carterpy/utils.py,sha256=Ff6AzmCPIrvDHGF887ms1Zb6Jm69Sg3KjXzsMt8RNQ0,481
-carter_py-1.0.0.dist-info/METADATA,sha256=MPbWApEU_6H0UbxR1H_oesfiuVfhzSLzxvtId0-00vg,8818
-carter_py-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-carter_py-1.0.0.dist-info/license.txt,sha256=ufmiTBS0Q6R8mZXaRjKpnIqT9NafpZYq9DoCZ_oGYBA,1075
-carter_py-1.0.0.dist-info/top_level.txt,sha256=l8aBC3U-dSDPJ4ZDLx8cpzscw9PFaB7vu3pA5WhXa4I,9
-carter_py-1.0.0.dist-info/RECORD,,
+carterpy/utils.py,sha256=d2ZPAGt1JXW2EqK4khkiJERIMy-P-V5hhQzIIFSetcw,466
+carter_py-1.0.1.dist-info/METADATA,sha256=k5Tg8ffGaeVoNaE9nz7b-jyKZCJfL1IKGqkndzVkg4o,8919
+carter_py-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+carter_py-1.0.1.dist-info/license.txt,sha256=ufmiTBS0Q6R8mZXaRjKpnIqT9NafpZYq9DoCZ_oGYBA,1075
+carter_py-1.0.1.dist-info/top_level.txt,sha256=l8aBC3U-dSDPJ4ZDLx8cpzscw9PFaB7vu3pA5WhXa4I,9
+carter_py-1.0.1.dist-info/RECORD,,
```

