# Comparing `tmp/testflows.asserts-6.5.230616.1120952.tar.gz` & `tmp/testflows.asserts-6.5.230626.1133416.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.asserts-6.5.230616.1120952.tar", last modified: Fri Jun 16 12:09:53 2023, max compression
+gzip compressed data, was "testflows.asserts-6.5.230626.1133416.tar", last modified: Mon Jun 26 13:34:17 2023, max compression
```

## Comparing `testflows.asserts-6.5.230616.1120952.tar` & `testflows.asserts-6.5.230626.1133416.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230616.1120952/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       16 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230616.1120952/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     7427 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     6852 2023-03-13 19:57:54.000000 testflows.asserts-6.5.230616.1120952/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1597 2023-06-16 12:09:52.000000 testflows.asserts-6.5.230616.1120952/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.187473 testflows.asserts-6.5.230616.1120952/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/testflows/asserts/
--rw-rw-r--   0 user      (1000) user      (1000)     1470 2023-06-16 12:09:52.000000 testflows.asserts-6.5.230616.1120952/testflows/asserts/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    25290 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230616.1120952/testflows/asserts/asserts.py
--rw-rw-r--   0 user      (1000) user      (1000)     6161 2023-06-15 01:11:04.000000 testflows.asserts-6.5.230616.1120952/testflows/asserts/helpers.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/
--rwxrwxr-x   0 user      (1000) user      (1000)     7427 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/PKG-INFO
--rwxrwxr-x   0 user      (1000) user      (1000)      386 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/SOURCES.txt
--rwxrwxr-x   0 user      (1000) user      (1000)        1 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/dependency_links.txt
--rwxrwxr-x   0 user      (1000) user      (1000)        1 2022-12-23 06:55:07.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/not-zip-safe
--rwxrwxr-x   0 user      (1000) user      (1000)       27 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/requires.txt
--rwxrwxr-x   0 user      (1000) user      (1000)       10 2023-06-16 12:09:53.000000 testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-16 12:09:53.191473 testflows.asserts-6.5.230616.1120952/tests/
--rw-rw-r--   0 user      (1000) user      (1000)    28026 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230616.1120952/tests/tests.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-26 13:34:16.999604 testflows.asserts-6.5.230626.1133416/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230626.1133416/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2023-03-13 19:56:48.000000 testflows.asserts-6.5.230626.1133416/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     7427 2023-06-26 13:34:16.999604 testflows.asserts-6.5.230626.1133416/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     6852 2023-03-13 19:57:54.000000 testflows.asserts-6.5.230626.1133416/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-26 13:34:16.999604 testflows.asserts-6.5.230626.1133416/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1557 2023-06-26 13:34:16.000000 testflows.asserts-6.5.230626.1133416/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-26 13:34:16.999604 testflows.asserts-6.5.230626.1133416/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-26 13:34:16.999604 testflows.asserts-6.5.230626.1133416/testflows/asserts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1470 2023-06-26 13:34:16.000000 testflows.asserts-6.5.230626.1133416/testflows/asserts/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25290 2023-06-19 12:01:44.000000 testflows.asserts-6.5.230626.1133416/testflows/asserts/asserts.py
+-rw-rw-r--   0 user      (1000) user      (1000)     6364 2023-06-26 13:32:40.000000 testflows.asserts-6.5.230626.1133416/testflows/asserts/helpers.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-26 13:34:16.999604 testflows.asserts-6.5.230626.1133416/testflows.asserts.egg-info/
+-rwxrwxr-x   0 user      (1000) user      (1000)     7427 2023-06-26 13:34:16.000000 testflows.asserts-6.5.230626.1133416/testflows.asserts.egg-info/PKG-INFO
+-rwxrwxr-x   0 user      (1000) user      (1000)      386 2023-06-26 13:34:16.000000 testflows.asserts-6.5.230626.1133416/testflows.asserts.egg-info/SOURCES.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)        1 2023-06-26 13:34:16.000000 testflows.asserts-6.5.230626.1133416/testflows.asserts.egg-info/dependency_links.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)        1 2022-12-23 06:55:07.000000 testflows.asserts-6.5.230626.1133416/testflows.asserts.egg-info/not-zip-safe
+-rwxrwxr-x   0 user      (1000) user      (1000)       27 2023-06-26 13:34:16.000000 testflows.asserts-6.5.230626.1133416/testflows.asserts.egg-info/requires.txt
+-rwxrwxr-x   0 user      (1000) user      (1000)       10 2023-06-26 13:34:16.000000 testflows.asserts-6.5.230626.1133416/testflows.asserts.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-26 13:34:16.999604 testflows.asserts-6.5.230626.1133416/tests/
+-rw-rw-r--   0 user      (1000) user      (1000)    33406 2023-06-26 13:32:40.000000 testflows.asserts-6.5.230626.1133416/tests/tests.py
```

### Comparing `testflows.asserts-6.5.230616.1120952/LICENSE` & `testflows.asserts-6.5.230626.1133416/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.asserts-6.5.230616.1120952/PKG-INFO` & `testflows.asserts-6.5.230626.1133416/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.asserts
-Version: 6.5.230616.1120952
+Version: 6.5.230626.1133416
 Summary: TestFlows - Asserts Assertion Library
 Home-page: https://github.com/testflows/testflows-asserts
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.asserts-6.5.230616.1120952/README.rst` & `testflows.asserts-6.5.230626.1133416/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.asserts-6.5.230616.1120952/setup.py` & `testflows.asserts-6.5.230626.1133416/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,34 +15,29 @@
 from setuptools import setup
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setup(
     name="testflows.asserts",
-    version="6.5.230616.1120952",
+    version="6.5.230626.1133416",
     description="TestFlows - Asserts Assertion Library",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/testflows-asserts",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
     ],
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     license="Apache-2.0",
     packages=[
         "testflows.asserts",
     ],
     zip_safe=False,
-    install_requires=[
-    ],
-    extras_require={
-        "dev": [
-            "testflows.core>=1.6"
-        ]
-    }
+    install_requires=[],
+    extras_require={"dev": ["testflows.core>=1.6"]},
 )
```

### Comparing `testflows.asserts-6.5.230616.1120952/testflows/asserts/__init__.py` & `testflows.asserts-6.5.230626.1133416/testflows/asserts/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "6.5.230616.1120952"
+__version__ = "6.5.230626.1133416"
 __license__ = f"""
 Copyright 2019 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.asserts-6.5.230616.1120952/testflows/asserts/asserts.py` & `testflows.asserts-6.5.230626.1133416/testflows/asserts/asserts.py`

 * *Files identical despite different names*

### Comparing `testflows.asserts-6.5.230616.1120952/testflows/asserts/helpers.py` & `testflows.asserts-6.5.230626.1133416/testflows/asserts/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,15 +75,17 @@
                     frame_info=self.frame_info,
                     nodes=[],
                 )
             )
         return True
 
 
-def snapshot(value, id=None, output=None, path=None, name="snapshot", encoder=repr, comment=None):
+def snapshot(
+    value, id=None, output=None, path=None, name="snapshot", encoder=repr, comment=None
+):
     """Compare value representation to a stored snapshot.
     If snapshot does not exist, assertion passes else
     representation of the value is compared to the stored snapshot.
 
     Snapshot files have format:
 
         <test file name>[.<id>].snapshot
@@ -95,15 +97,17 @@
     :param name: name of the snapshot value inside the snapshots file, default: `snapshot`
     :param encoder: custom snapshot encoder, default: `repr`
     :param comment: optional comment to be added at the end of the snapshot value
     """
     name = varname(name) if name != "snapshot" else name
 
     class SnapshotError(object):
-        def __init__(self, filename, name, snapshot_value, actual_value, comment=None, diff=None):
+        def __init__(
+            self, filename, name, snapshot_value, actual_value, comment=None, diff=None
+        ):
             self.snapshot_value = snapshot_value
             self.actual_value = actual_value
             self.diff = diff
             self.filename = str(filename)
             self.name = str(name)
             self.comment = str(comment) if comment is not None else None
 
@@ -165,20 +169,25 @@
 
     if os.path.exists(filename):
         module_name = f"snapshot_{hashlib.sha1(os.path.abspath(filename).encode('utf-8')).hexdigest()}"
         snapshot_module = SourceFileLoader(module_name, filename).load_module()
         if hasattr(snapshot_module, name):
             snapshot_value = getattr(snapshot_module, name)
             if not (snapshot_value == repr_value):
-                return SnapshotError(filename, name, snapshot_value, repr_value, comment)
+                return SnapshotError(
+                    filename, name, snapshot_value, repr_value, comment
+                )
             return True
 
     # no snapshot, so just store the representation
     with open(filename, "a") as fd:
         repr_value = repr_value.replace('"""', '""" + \'"""\' + r"""')
         if comment is not None:
             comment = f" # {comment}"
         else:
             comment = ""
-        fd.write(f'''{name} = r"""{repr_value}"""{comment}\n\n''')
+        if repr_value.endswith('"'):
+            fd.write(f'''{name} = r"""{repr_value[:-1]}""" + '"'{comment}\n\n''')
+        else:
+            fd.write(f'''{name} = r"""{repr_value}"""{comment}\n\n''')
 
     return True
```

### Comparing `testflows.asserts-6.5.230616.1120952/testflows.asserts.egg-info/PKG-INFO` & `testflows.asserts-6.5.230626.1133416/testflows.asserts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.asserts
-Version: 6.5.230616.1120952
+Version: 6.5.230626.1133416
 Summary: TestFlows - Asserts Assertion Library
 Home-page: https://github.com/testflows/testflows-asserts
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.asserts-6.5.230616.1120952/tests/tests.py` & `testflows.asserts-6.5.230626.1133416/tests/tests.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import random
 import tempfile
 
 from testflows.core import main, note
 from testflows.core import TestModule, Module, Test, Suite, xfail
 from testflows.asserts import error, errors, values, raises, snapshot
 
+
 def snap(value):
     """Take a snapshot of the value. If the value is an
     AssertionError with an error object then do not
     include the "where section".
     """
     if isinstance(value, AssertionError) and value.args:
         if isinstance(value.args[0], error):
@@ -33,32 +34,34 @@
             return err.generate_message()
         if isinstance(value.args[0], errors):
             err = value.args[0]
             err.where_section = False
             return str(err)
     return repr(value)
 
+
 @TestModule
 def regression(self):
-    """TestFlows - Asserts regression suite.
-    """
+    """TestFlows - Asserts regression suite."""
     with Suite("errors"):
         with Test("errors no fails"):
             with errors():
                 assert True
                 assert 1 == 1
 
         with Test("errors"):
             with raises(AssertionError) as e:
                 with errors():
                     assert True
                     assert False, "boo"
             note(e.exception)
             with values() as that:
-                assert that(snapshot(e.exception, "errors-errors", encoder=snap)), error()
+                assert that(
+                    snapshot(e.exception, "errors-errors", encoder=snap)
+                ), error()
 
         with Test("soft error no fails"):
             with errors() as soft:
                 with soft.error():
                     assert True
                 with soft.error():
                     assert 1 == 1
@@ -69,15 +72,17 @@
                     with soft.error():
                         assert False, "boo"
                     with soft.error():
                         assert False, "boo2"
                     assert True
             note(e.exception)
             with values() as that:
-                assert that(snapshot(e.exception, "errors-soft-errors", encoder=snap)), error()
+                assert that(
+                    snapshot(e.exception, "errors-soft-errors", encoder=snap)
+                ), error()
 
         with Test("mixed errors no fails"):
             with errors() as soft:
                 assert True
                 with soft.error():
                     assert True
                 assert "a" == "a"
@@ -89,567 +94,791 @@
                 with errors() as soft:
                     with soft.error():
                         assert False, "boo"
                     assert True
                     assert False, "boo2"
                     # should not get here as the assertion above
                     # should cause an exception
-                    assert 1/0
+                    assert 1 / 0
             note(e.exception)
             with values() as that:
-                assert that(snapshot(e.exception, "errors-mixed-errors", encoder=snap)), error()
+                assert that(
+                    snapshot(e.exception, "errors-mixed-errors", encoder=snap)
+                ), error()
 
     with Suite("helpers"):
         with Test("snapshot"):
             with Test("triple quotes"):
                 with values() as that:
-                    assert that(snapshot('"""hello"""there"""""foo""boo', "snapshot-triple-quotes", encoder=snap)), error()
+                    assert that(
+                        snapshot(
+                            '"""hello"""there"""""foo""boo',
+                            "snapshot-triple-quotes",
+                            encoder=snap,
+                        )
+                    ), error()
 
             with Test("multiple snapshots in the same file"):
                 with values() as that:
-                    assert that(snapshot("first", "snapshot-multiple-snapshots-in-the-same-file", name="first", encoder=snap)), error()
-                    assert that(snapshot("second", "snapshot-multiple-snapshots-in-the-same-file", name="second", encoder=snap)), error()
+                    assert that(
+                        snapshot(
+                            "first",
+                            "snapshot-multiple-snapshots-in-the-same-file",
+                            name="first",
+                            encoder=snap,
+                        )
+                    ), error()
+                    assert that(
+                        snapshot(
+                            "second",
+                            "snapshot-multiple-snapshots-in-the-same-file",
+                            name="second",
+                            encoder=snap,
+                        )
+                    ), error()
+
+            with Test("value that ends with double quotes"):
+                s = "1,'home'"
+                with values() as that:
+                    assert that(
+                        snapshot(
+                            s,
+                            "snapshot-value-ends-with-double-quotes",
+                            name="third",
+                            encoder=repr,
+                        )
+                    ), error()
 
         with Test("raises"):
             with Test("not raised"):
                 with raises(AssertionError) as e:
                     with raises(AssertionError):
                         pass
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "raises-not-raised", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "raises-not-raised", encoder=snap)
+                    ), error()
 
             with Test("unexpected exception"):
                 with raises(AssertionError) as e:
                     with raises(AssertionError):
                         raise ValueError("error")
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "raises-unexpected-exception", encoder=snap)), error()
+                    assert that(
+                        snapshot(
+                            e.exception, "raises-unexpected-exception", encoder=snap
+                        )
+                    ), error()
 
             with Test("ok"):
                 with raises(ValueError) as e:
                     raise ValueError("error")
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "raised-ok", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "raised-ok", encoder=snap)
+                    ), error()
 
     with Suite("assertions"):
         with Test("multiline"):
             with Test("implicit"):
                 with raises(AssertionError) as e:
-                    assert (1,
-                            2) is False, error()
+                    assert (1, 2) is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "multiline-implicit", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "multiline-implicit", encoder=snap)
+                    ), error()
 
             with Test("explicit"):
                 with raises(AssertionError) as e:
-                    assert "hello" == "foo bar"\
-                        and 3 == 3\
-                        and 1 > 1 or 1>1 or 3>3 or 4>+4, error()
+                    assert (
+                        "hello" == "foo bar"
+                        and 3 == 3
+                        and 1 > 1
+                        or 1 > 1
+                        or 3 > 3
+                        or 4 > +4
+                    ), error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "multiline-explicit", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "multiline-explicit", encoder=snap)
+                    ), error()
 
         with Test("values"):
             with Test("assert with file read"):
                 with tempfile.TemporaryFile("w+") as fp:
                     fp.write("hello")
                     fp.seek(0)
                     with raises(AssertionError) as e, values() as that:
                         assert not that(fp.read()), error()
                     note(e.exception)
                     with values() as that:
-                        assert that(snapshot(e.exception, "values-assert_with_file_read", encoder=snap)), error()
+                        assert that(
+                            snapshot(
+                                e.exception,
+                                "values-assert_with_file_read",
+                                encoder=snap,
+                            )
+                        ), error()
 
             with Test("assert with list append"):
                 some_list = []
                 with raises(AssertionError) as e, values() as that:
                     assert that(some_list.append(2)) == [1], error()
                 note(e.exception)
                 with Test("assert that list did not change"):
                     assert some_list == [2], error()
                 with values() as that:
-                    assert that(snapshot(e.exception, "values-assert_with_list_append", encoder=snap)), error()
+                    assert that(
+                        snapshot(
+                            e.exception, "values-assert_with_list_append", encoder=snap
+                        )
+                    ), error()
 
         with Suite("func"):
             with Test("args"):
                 vs = []
-                def foo(x,y,z):
-                    vs.append((x,y,z))
-                    return x,y,z
+
+                def foo(x, y, z):
+                    vs.append((x, y, z))
+                    return x, y, z
+
                 with raises(AssertionError) as e:
-                    assert foo(1,2,3) is False, error()
+                    assert foo(1, 2, 3) is False, error()
                 note(e.exception)
                 with Test("assert that args are the same"):
                     assert vs[0] == vs[1], error()
                 with Test("assert exception snapshot value"):
                     with values() as that:
-                        assert that(snapshot(e.exception, "func-args", encoder=snap)), error()
+                        assert that(
+                            snapshot(e.exception, "func-args", encoder=snap)
+                        ), error()
 
             with Test("*vargs"):
                 vs = []
+
                 def foo(*x):
                     note(x)
                     vs.append(x)
                     return x
+
                 with raises(AssertionError) as e:
-                    assert foo(*[1,2]) is False, error()
+                    assert foo(*[1, 2]) is False, error()
                 note(e.exception)
                 with Test("assert *vargs are the same"):
                     assert vs[0] == vs[1]
                 with values() as that:
-                    assert that(snapshot(e.exception, "func-vargs", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "func-vargs", encoder=snap)
+                    ), error()
 
             with Test("**kwargs"):
                 vs = []
+
                 def foo(**x):
                     note(x)
                     vs.append(x)
                     return x
+
                 with raises(AssertionError) as e:
-                    assert foo(x=1,y=2) is False, error()
+                    assert foo(x=1, y=2) is False, error()
                 note(e.exception)
                 with Test("assert **kwargs are the same"):
                     assert vs[0] == vs[1]
                 with values() as that:
-                    assert that(snapshot(e.exception, "func-kwargs", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "func-kwargs", encoder=snap)
+                    ), error()
 
             with Test("args *vargs **kwargs"):
                 vs = []
-                def foo(x,*y,**z):
+
+                def foo(x, *y, **z):
                     note((x, y, z))
                     vs.append((x, y, z))
                     return x, y, z
+
                 with raises(AssertionError) as e:
-                    assert foo(1,*[2],z=3) is False, error()
+                    assert foo(1, *[2], z=3) is False, error()
                 note(e.exception)
                 with Test("assert args, *vargs, **kwargs are the same"):
                     assert vs[0] == vs[1]
                 with values() as that:
-                    assert that(snapshot(e.exception, "func-args_vargs_kwargs", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "func-args_vargs_kwargs", encoder=snap)
+                    ), error()
 
         with Suite("boolean ops"):
             with Test("and"):
                 with raises(AssertionError) as e:
                     assert 1 and 0, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "boolean-ops-and", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "boolean-ops-and", encoder=snap)
+                    ), error()
 
             with Test("multiple and"):
                 with raises(AssertionError) as e:
                     assert 1 and 2 and 3 and 0, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "boolean-ops-multiple-and", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "boolean-ops-multiple-and", encoder=snap)
+                    ), error()
 
             with Test("or"):
                 with raises(AssertionError) as e:
-                    assert 0 or '', error()
+                    assert 0 or "", error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "boolean-ops-or", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "boolean-ops-or", encoder=snap)
+                    ), error()
 
             with Test("multiple or"):
                 with raises(AssertionError) as e:
-                    assert 0 or '' or False or None, error()
+                    assert 0 or "" or False or None, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "boolean-ops-multiple-or", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "boolean-ops-multiple-or", encoder=snap)
+                    ), error()
 
         with Suite("binary ops"):
             with Test("add"):
                 with raises(AssertionError) as e:
                     assert 1 + 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-add", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-add", encoder=snap)
+                    ), error()
 
             with Test("sub"):
                 with raises(AssertionError) as e:
                     assert 1 - 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-sub", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-sub", encoder=snap)
+                    ), error()
 
             with Test("mul"):
                 with raises(AssertionError) as e:
                     assert 1 * 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-mul", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-mul", encoder=snap)
+                    ), error()
 
             with Test("div"):
                 with raises(AssertionError) as e:
                     assert 1 / 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-div", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-div", encoder=snap)
+                    ), error()
 
             with Test("mod"):
                 with raises(AssertionError) as e:
                     assert 1 % 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-mod", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-mod", encoder=snap)
+                    ), error()
 
             with Test("pow"):
                 with raises(AssertionError) as e:
-                    assert 1 ** 3 is False, error()
+                    assert 1**3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-pow", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-pow", encoder=snap)
+                    ), error()
 
             with Test("lshift"):
                 with raises(AssertionError) as e:
                     assert 1 << 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-lshift", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-lshift", encoder=snap)
+                    ), error()
 
             with Test("rshift"):
                 with raises(AssertionError) as e:
                     assert 1 >> 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-rshift", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-rshift", encoder=snap)
+                    ), error()
 
             with Test("bitOr"):
                 with raises(AssertionError) as e:
                     assert 1 | 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-bitOr", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-bitOr", encoder=snap)
+                    ), error()
 
             with Test("bitXor"):
                 with raises(AssertionError) as e:
                     assert 1 ^ 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-bitXor", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-bitXor", encoder=snap)
+                    ), error()
 
             with Test("bitAnd"):
                 with raises(AssertionError) as e:
                     assert 1 & 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-bitAnd", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-bitAnd", encoder=snap)
+                    ), error()
 
             with Test("floor div"):
                 with raises(AssertionError) as e:
                     assert 1 // 3 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-floor-div", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-floor-div", encoder=snap)
+                    ), error()
 
             with Test("mixed ops"):
                 with raises(AssertionError) as e:
-                    assert 1 + 3 - 4 * 5 ** 1 >> 1 << 3 % 5 | 2 ^ 5 & 6 // 3 is False, error()
+                    assert (
+                        1 + 3 - 4 * 5**1 >> 1 << 3 % 5 | 2 ^ 5 & 6 // 3 is False
+                    ), error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "binary-ops-mixed-ops", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "binary-ops-mixed-ops", encoder=snap)
+                    ), error()
 
         with Suite("unary ops"):
             with Test("invert"):
                 with raises(AssertionError) as e:
                     assert ~4 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "unary-ops-invert", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "unary-ops-invert", encoder=snap)
+                    ), error()
 
             with Test("not"):
                 with raises(AssertionError) as e:
                     assert not 4 is 4, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "unary-ops-not", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "unary-ops-not", encoder=snap)
+                    ), error()
 
             with Test("uadd"):
                 with raises(AssertionError) as e:
                     assert +4 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "unary-ops-uadd", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "unary-ops-uadd", encoder=snap)
+                    ), error()
 
             with Test("usub"):
                 with raises(AssertionError) as e:
                     assert -4 is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "unary-ops-usub", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "unary-ops-usub", encoder=snap)
+                    ), error()
 
         with Suite("compare ops"):
             with Test("eq"):
                 with raises(AssertionError) as e:
                     assert 1 == 2, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-eq", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-eq", encoder=snap)
+                    ), error()
 
             with Test("eq str"):
                 with raises(AssertionError) as e:
                     assert "1:a\n2:a\n3:c" == "1:a\n2:b\n3:c", error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-eq-str", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-eq-str", encoder=snap)
+                    ), error()
 
             with Test("eq tuple"):
                 with raises(AssertionError) as e:
-                    assert (1,2,3) == (1,1,3), error()
+                    assert (1, 2, 3) == (1, 1, 3), error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-eq-tuple", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-eq-tuple", encoder=snap)
+                    ), error()
 
             with Test("eq list"):
                 with raises(AssertionError) as e:
-                    assert [1,2,3] == [1,1,3], error()
+                    assert [1, 2, 3] == [1, 1, 3], error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-eq-list", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-eq-list", encoder=snap)
+                    ), error()
 
             with Test("eq set"):
                 with raises(AssertionError) as e:
-                    assert {1,2,3} == {1,2,3,4}, error()
+                    assert {1, 2, 3} == {1, 2, 3, 4}, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-eq-set", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-eq-set", encoder=snap)
+                    ), error()
 
             with Test("eq dict"):
                 with raises(AssertionError) as e:
-                    assert {1:"a", 2:"a", 3:"c"} == {1:"a", 2:"b", 3:"c"}, error()
+                    assert {1: "a", 2: "a", 3: "c"} == {1: "a", 2: "b", 3: "c"}, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-eq-dict", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-eq-dict", encoder=snap)
+                    ), error()
 
             with Test("ne"):
                 with raises(AssertionError) as e:
                     assert 1 != 1, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-ne", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-ne", encoder=snap)
+                    ), error()
 
             with Test("lt"):
                 with raises(AssertionError) as e:
                     assert 1 < 1, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-lt", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-lt", encoder=snap)
+                    ), error()
 
             with Test("le"):
                 with raises(AssertionError) as e:
                     assert 1 <= 0, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-le", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-le", encoder=snap)
+                    ), error()
 
             with Test("gt"):
                 with raises(AssertionError) as e:
                     assert 1 > 1, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-gt", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-gt", encoder=snap)
+                    ), error()
 
             with Test("ge"):
                 with raises(AssertionError) as e:
                     assert 1 >= 2, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-ge", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-ge", encoder=snap)
+                    ), error()
 
             with Test("is"):
                 with raises(AssertionError) as e:
                     assert 1 is 2, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-is", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-is", encoder=snap)
+                    ), error()
 
             with Test("is not"):
                 with raises(AssertionError) as e:
                     assert 1 is not 1, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-is-not", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-is-not", encoder=snap)
+                    ), error()
 
             with Test("in"):
                 with raises(AssertionError) as e:
                     assert 1 in [2], error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-in", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-in", encoder=snap)
+                    ), error()
 
             with Test("not in"):
                 with raises(AssertionError) as e:
                     assert 1 not in [1], error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "compare-ops-not-in", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "compare-ops-not-in", encoder=snap)
+                    ), error()
 
         with Suite("common types"):
             with Test("str"):
                 with raises(AssertionError) as e:
                     assert "hello" is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-types-str", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-types-str", encoder=snap)
+                    ), error()
 
             with Test("list"):
                 with raises(AssertionError) as e:
                     assert [1] is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-types-list", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-types-list", encoder=snap)
+                    ), error()
 
             with Test("tuple"):
                 with raises(AssertionError) as e:
                     assert (1,) is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-types-tuple", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-types-tuple", encoder=snap)
+                    ), error()
 
             with Test("dict"):
                 with raises(AssertionError) as e:
-                    assert {'a':1} is False, error()
+                    assert {"a": 1} is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-types-dict", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-types-dict", encoder=snap)
+                    ), error()
 
             with Test("object type"):
                 with raises(AssertionError) as e:
                     assert object is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-types-object-type", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-types-object-type", encoder=snap)
+                    ), error()
 
             with Test("object"):
                 with raises(AssertionError) as e:
                     assert object() is False, error()
                 note(e.exception)
 
             with Test("bytes"):
                 with raises(AssertionError) as e:
-                    assert b'hello' is False, error()
+                    assert b"hello" is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-types-bytes", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-types-bytes", encoder=snap)
+                    ), error()
 
             with Test("unicode"):
                 with raises(AssertionError) as e:
-                    assert u'hello' is False, error()
+                    assert "hello" is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-types-unicode", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-types-unicode", encoder=snap)
+                    ), error()
 
         with Suite("common idioms"):
             with Test("if/else"):
                 with raises(AssertionError) as e:
                     assert (1 if 1 else 2) is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-if-else", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-idioms-if-else", encoder=snap)
+                    ), error()
 
             with Test("ellipsis"):
                 with raises(AssertionError) as e:
                     assert ... is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-ellipsis", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-idioms-ellipsis", encoder=snap)
+                    ), error()
 
             with Test("assignment"):
+
                 def foo(x):
                     return x
+
                 with raises(AssertionError) as e:
-                    assert foo(x = 1) is False, error()
+                    assert foo(x=1) is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-assignment", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-idioms-assignment", encoder=snap)
+                    ), error()
 
             with Test("subscript"):
                 with raises(AssertionError) as e:
-                    assert [1,2,3][1:] is False, error()
+                    assert [1, 2, 3][1:] is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-subscript", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-idioms-subscript", encoder=snap)
+                    ), error()
 
             with Test("attr access"):
                 with raises(AssertionError) as e:
                     assert object().__class__ is False, error()
                 note(e.exception)
 
             with Test("attribute function call"):
                 with raises(AssertionError) as e:
-                    assert "hello".join([' ', 'there']) is False, error()
+                    assert "hello".join([" ", "there"]) is False, error()
                 note(e.exception)
 
             with Test("lambda name"):
                 with raises(AssertionError) as e:
                     assert (lambda x: x)(1) is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-lambda-name", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-idioms-lambda-name", encoder=snap)
+                    ), error()
 
             with Test("lambda expr"):
                 with raises(AssertionError) as e:
-                    assert (lambda x: x+1)(1) is False, error()
+                    assert (lambda x: x + 1)(1) is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-lambda-expr", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-idioms-lambda-expr", encoder=snap)
+                    ), error()
 
             with Test("getitem"):
                 with raises(AssertionError) as e:
-                    assert {'a':1}['a'] is False, error()
+                    assert {"a": 1}["a"] is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-getitem", encoder=snap)), error()
+                    assert that(
+                        snapshot(e.exception, "common-idioms-getitem", encoder=snap)
+                    ), error()
 
             with Test("generator expression"):
+
                 def foo(x):
                     return x
+
                 with raises(AssertionError) as e:
-                    assert foo(x*x for x in range(2)) is False, error()
+                    assert foo(x * x for x in range(2)) is False, error()
                 note(e.exception)
 
             with Test("list comprehension"):
+
                 def foo(x):
                     return x
+
                 with raises(AssertionError) as e:
-                    assert foo([y*x for x in [[1],[2]] if len(x) > 0 for y in x if y > 0]) is False, error()
-                note(e.exception)
-                with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-list-comprehension", encoder=snap)), error()
+                    assert (
+                        foo(
+                            [
+                                y * x
+                                for x in [[1], [2]]
+                                if len(x) > 0
+                                for y in x
+                                if y > 0
+                            ]
+                        )
+                        is False
+                    ), error()
+                note(e.exception)
+                with values() as that:
+                    assert that(
+                        snapshot(
+                            e.exception,
+                            "common-idioms-list-comprehension",
+                            encoder=snap,
+                        )
+                    ), error()
 
             with Test("set comprehension"):
                 with raises(AssertionError) as e, values() as that:
                     f = 5
                     assert {that(x) for x in range(f)} is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-set-comprehension", encoder=snap)), error()
+                    assert that(
+                        snapshot(
+                            e.exception, "common-idioms-set-comprehension", encoder=snap
+                        )
+                    ), error()
 
             with Test("dict comprehension"):
                 with raises(AssertionError) as e, values() as that:
                     f, g = 2, 3
-                    assert {that(x): x*f for x in range(g)} is False, error()
+                    assert {that(x): x * f for x in range(g)} is False, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-dict-comprehension", encoder=snap)), error()
+                    assert that(
+                        snapshot(
+                            e.exception,
+                            "common-idioms-dict-comprehension",
+                            encoder=snap,
+                        )
+                    ), error()
 
             with Test("chained comparison"):
                 with raises(AssertionError) as e:
                     x = 2
                     assert 1 >= x <= 3 <= 10, error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-chained-comparison", encoder=snap)), error()
+                    assert that(
+                        snapshot(
+                            e.exception,
+                            "common-idioms-chained-comparison",
+                            encoder=snap,
+                        )
+                    ), error()
 
             with Test("chained str comparison"):
                 with raises(AssertionError) as e:
                     x = "bbb"
                     assert "a" == x <= "ccc" <= "ddd", error()
                 note(e.exception)
                 with values() as that:
-                    assert that(snapshot(e.exception, "common-idioms-chained-str-comparison", encoder=snap)), error()
+                    assert that(
+                        snapshot(
+                            e.exception,
+                            "common-idioms-chained-str-comparison",
+                            encoder=snap,
+                        )
+                    ), error()
+
 
 if main():
     Module(run=regression)
```

