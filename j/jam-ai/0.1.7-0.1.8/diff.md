# Comparing `tmp/jam_ai-0.1.7.tar.gz` & `tmp/jam_ai-0.1.8.tar.gz`

## Comparing `jam_ai-0.1.7.tar` & `jam_ai-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,46 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/cmd/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.7/cmd/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/albert-einstein.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/homer-simpson.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/marie-curie.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/walter-white.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/base.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/core.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/version.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/instrument/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/instrument/base.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/instrument/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/instrument/text.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/__init__.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/base.py
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/openai.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/stability_ai.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/writesonic.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/__init__.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/base.py
--rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/memory.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/model.py
--rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/sqlite.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/personnel/__init__.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/personnel/base.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/personnel/personnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/util/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/util/generate.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/util/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/instrument/__init__.py
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/instrument/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/interface/__init__.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/interface/test_base.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.7/LICENSE
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 jam_ai-0.1.7/README.md
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 jam_ai-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    16417 2020-02-02 00:00:00.000000 jam_ai-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/cmd/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.8/cmd/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/albert-einstein.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/homer-simpson.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/marie-curie.json
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.8/example/personnel/walter-white.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/base.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/core.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/version.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/base.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/instrument/text.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/base.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/openai.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/stability_ai.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/interface/writesonic.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/__init__.py
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/base.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/memory.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/model.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/mysql.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/postgres.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/persistence/sqlite.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/__init__.py
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/base.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/personnel/personnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/generate.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.8/jam/util/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/instrument/__init__.py
+-rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/instrument/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/interface/__init__.py
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/interface/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/test_persistence/__init__.py
+-rw-r--r--   0        0        0     6328 2020-02-02 00:00:00.000000 jam_ai-0.1.8/tests/test_persistence/test_base.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 jam_ai-0.1.8/README.md
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 jam_ai-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    16352 2020-02-02 00:00:00.000000 jam_ai-0.1.8/PKG-INFO
```

### Comparing `jam_ai-0.1.7/cmd/main.py` & `jam_ai-0.1.8/cmd/main.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/example/personnel/albert-einstein.json` & `jam_ai-0.1.8/example/personnel/albert-einstein.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/example/personnel/homer-simpson.json` & `jam_ai-0.1.8/example/personnel/homer-simpson.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/example/personnel/marie-curie.json` & `jam_ai-0.1.8/example/personnel/marie-curie.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/example/personnel/walter-white.json` & `jam_ai-0.1.8/example/personnel/walter-white.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/base.py` & `jam_ai-0.1.8/jam/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/core.py` & `jam_ai-0.1.8/jam/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,9 +56,10 @@
                 self._assign(member, message)
         return self.cache_output
 
     def history(self):
         result = self.persistence.all()
         return result
 
-    def clear(self):
+    def clear(self, key: str = None,  value: List[str] = None):
+        self.persistence.clear(key, value)
         return
```

### Comparing `jam_ai-0.1.7/jam/instrument/base.py` & `jam_ai-0.1.8/jam/instrument/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/instrument/image.py` & `jam_ai-0.1.8/jam/instrument/image.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/interface/base.py` & `jam_ai-0.1.8/jam/interface/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/interface/openai.py` & `jam_ai-0.1.8/jam/interface/openai.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/interface/stability_ai.py` & `jam_ai-0.1.8/jam/interface/stability_ai.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/interface/writesonic.py` & `jam_ai-0.1.8/jam/interface/writesonic.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/persistence/base.py` & `jam_ai-0.1.8/jam/persistence/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from datetime import datetime
-from typing import Dict, AnyStr
+from typing import Dict, AnyStr, List
 
 
 class BasePersistence(object):
 
     def __init__(self):
         pass
 
     @staticmethod
     def transform(data: Dict) -> Dict:
         return {}
 
-    def save(self, role: str, author: str, content: str):
-        pass
+    def save(self,
+             role: str,
+             author: str,
+             content: str,
+             mentions: List[str] = None,
+             function: str = None,
+             success: bool = True):
+        return []
 
     def find(self, key: str, value: str = None, limit: int = 5):
         return []
 
     def all(self):
         return []
```

### Comparing `jam_ai-0.1.7/jam/persistence/memory.py` & `jam_ai-0.1.8/jam/persistence/memory.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/persistence/model.py` & `jam_ai-0.1.8/jam/persistence/model.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/persistence/sqlite.py` & `jam_ai-0.1.8/jam/persistence/sqlite.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/jam/personnel/base.py` & `jam_ai-0.1.8/jam/personnel/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/tests/instrument/test_base.py` & `jam_ai-0.1.8/tests/instrument/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/tests/interface/test_base.py` & `jam_ai-0.1.8/tests/interface/test_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,25 +38,25 @@
         self.assertEqual(self.ji_2.success, True)
         self.assertEqual(self.ji_3.success, False)
 
     def tearDown(self) -> None:
         pass
 
 
-class BaseInterfaceAlter(BaseInterface):
+class AlterInterface(BaseInterface):
 
     def call(self, x: AnyStr = None) -> JIOutput:
         return JIOutput(output=x, success=False)
 
 
 class TestBaseInterface(unittest.TestCase):
 
     def setUp(self) -> None:
         self.bi_1 = BaseInterface()
-        self.bi_2 = BaseInterface()
+        self.bi_2 = AlterInterface()
 
     def test_class_identity(self):
         self.assertIsInstance(self.bi_1, BaseInterface)
         self.assertIsInstance(self.bi_2, BaseInterface)
 
     def test_class_method_call(self):
         self.assertIsInstance(self.bi_1.call(), JIOutput)
@@ -64,14 +64,14 @@
 
         bi_1_call = self.bi_1.call()
         self.assertEqual(bi_1_call.out_type, JIOutput.JIO_TEXT)
         self.assertEqual(bi_1_call.output, '')
         self.assertEqual(bi_1_call.function, None)
         self.assertEqual(bi_1_call.success, True)
 
-        bi_2_call = self.bi_2.call()
+        bi_2_call = self.bi_2.call(x='Hello')
         self.assertEqual(bi_2_call.out_type, JIOutput.JIO_TEXT)
-        self.assertEqual(bi_2_call.output, '')
+        self.assertEqual(bi_2_call.output, 'Hello')
         self.assertEqual(bi_2_call.function, None)
-        self.assertEqual(bi_2_call.success, True)
+        self.assertEqual(bi_2_call.success, False)
```

### Comparing `jam_ai-0.1.7/.gitignore` & `jam_ai-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/LICENSE` & `jam_ai-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.7/README.md` & `jam_ai-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,25 +10,21 @@
 
 ## Quick Start
 
 ```python
 from jam import Jam
 from jam.personnel import BasicPersonnel
 from jam.instrument import PromptPainter
-from jam.persistence import SQLitePersistence
 
 jam_room = Jam(
     members=[
-        BasicPersonnel.from_json('example/personnel/albert-einstein.json'),
-        BasicPersonnel.from_json('example/personnel/stephen-hawking.json')
+        BasicPersonnel.from_json('albert-einstein.json'),
+        BasicPersonnel.from_json('stephen-hawking.json')
     ],
-    instruments=[
-        PromptPainter()
-    ],
-    persistence=SQLitePersistence()
+    instruments=[PromptPainter()]
 )
 
 prompt = jam_room.compose(
     message='Give me a question',
     multi=True
 )
 
@@ -47,19 +43,21 @@
 pip install jam-ai --upgrade
 ```
 You need to use Pip to install jam. Conda package is currently unavailable.
 
 ### Requirements
 * Python >= 3.8
 * OpenAI
+* Requests
+* Pillow
 
 Extra Requirements for Function Calls
-* Requests
+* Psycopg2
+* PyMySQL
 * Stability SDK
-* Pillow
 
 ### Extension
 
 For the use of other libraries, please consider to always feed in your API Keys respectively. See below for example.
 
 ```bash
 export STABILITY_KEY=YOUR_STABILITY_AI_KEY # If you are using Stability SDK
```

### Comparing `jam_ai-0.1.7/pyproject.toml` & `jam_ai-0.1.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jam-ai"
-version = "0.1.7"
+version = "0.1.8"
 version_pattern = "MAJOR.MINOR.PATCH"
 authors = [
   { name="Abhishta Gatya", email="abhishtagatya@yahoo.com" },
 ]
 description = "Engaging with Multiple AI Agents with Jam."
 keywords = ["openai", "multi agent", "chat engine", "collaboration", "machine learning", "data science"]
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     'openai',
     'Pillow',
     'requests',
     'SQLAlchemy',
+    'psycopg2',
+    'pymysql',
     'stability-sdk',
     'rich',
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
     'Development Status :: 3 - Alpha',
     # 'Development Status :: 4 - Beta',
```

### Comparing `jam_ai-0.1.7/PKG-INFO` & `jam_ai-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jam-ai
-Version: 0.1.7
+Version: 0.1.8
 Summary: Engaging with Multiple AI Agents with Jam.
 Project-URL: homepage, https://github.com/abhishtagatya/jam
 Project-URL: documentation, https://github.com/abhishtagatya/jam
 Project-URL: changelog, https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md
 Author-email: Abhishta Gatya <abhishtagatya@yahoo.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -227,14 +227,16 @@
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Requires-Dist: openai
 Requires-Dist: pillow
+Requires-Dist: psycopg2
+Requires-Dist: pymysql
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: sqlalchemy
 Requires-Dist: stability-sdk
 Description-Content-Type: text/markdown
 
 # Jam.AI
@@ -249,25 +251,21 @@
 
 ## Quick Start
 
 ```python
 from jam import Jam
 from jam.personnel import BasicPersonnel
 from jam.instrument import PromptPainter
-from jam.persistence import SQLitePersistence
 
 jam_room = Jam(
     members=[
-        BasicPersonnel.from_json('example/personnel/albert-einstein.json'),
-        BasicPersonnel.from_json('example/personnel/stephen-hawking.json')
+        BasicPersonnel.from_json('albert-einstein.json'),
+        BasicPersonnel.from_json('stephen-hawking.json')
     ],
-    instruments=[
-        PromptPainter()
-    ],
-    persistence=SQLitePersistence()
+    instruments=[PromptPainter()]
 )
 
 prompt = jam_room.compose(
     message='Give me a question',
     multi=True
 )
 
@@ -286,19 +284,21 @@
 pip install jam-ai --upgrade
 ```
 You need to use Pip to install jam. Conda package is currently unavailable.
 
 ### Requirements
 * Python >= 3.8
 * OpenAI
+* Requests
+* Pillow
 
 Extra Requirements for Function Calls
-* Requests
+* Psycopg2
+* PyMySQL
 * Stability SDK
-* Pillow
 
 ### Extension
 
 For the use of other libraries, please consider to always feed in your API Keys respectively. See below for example.
 
 ```bash
 export STABILITY_KEY=YOUR_STABILITY_AI_KEY # If you are using Stability SDK
```

