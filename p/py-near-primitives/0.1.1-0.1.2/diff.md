# Comparing `tmp/py_near_primitives-0.1.1.tar.gz` & `tmp/py_near_primitives-0.1.2.tar.gz`

## Comparing `py_near_primitives-0.1.1.tar` & `py_near_primitives-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 py_near_primitives-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123    11357 2023-06-25 09:39:13.000000 py_near_primitives-0.1.1/LICENSE
--rw-r--r--   0     1001      123      579 2023-06-25 09:39:13.000000 py_near_primitives-0.1.1/README.md
--rw-r--r--   0     1001      123     1195 2023-06-25 09:39:13.000000 py_near_primitives-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123    17770 2023-06-25 09:39:13.000000 py_near_primitives-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123    69227 2023-06-25 09:39:37.000000 py_near_primitives-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 py_near_primitives-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      765 1970-01-01 00:00:00.000000 py_near_primitives-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123    11357 2023-06-26 03:15:27.000000 py_near_primitives-0.1.2/LICENSE
+-rw-r--r--   0     1001      123      579 2023-06-26 03:15:27.000000 py_near_primitives-0.1.2/README.md
+-rw-r--r--   0     1001      123     1195 2023-06-26 03:15:27.000000 py_near_primitives-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123    17770 2023-06-26 03:15:27.000000 py_near_primitives-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123    69227 2023-06-26 03:15:52.000000 py_near_primitives-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 py_near_primitives-0.1.2/PKG-INFO
```

### Comparing `py_near_primitives-0.1.1/Cargo.toml` & `py_near_primitives-0.1.2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_near_primitives-0.1.1/LICENSE` & `py_near_primitives-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `py_near_primitives-0.1.1/README.md` & `py_near_primitives-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `py_near_primitives-0.1.1/pyproject.toml` & `py_near_primitives-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py_near_primitives"
-version = "0.1.0"
+version = "0.1.2"
 description = "Python bindings for NEAR Rust primitives."
 authors = ["pvolnov <notanemail@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
@@ -21,15 +21,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 
 [project]
 name = "py_near_primitives"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python bindings for NEAR Rust primitives."
 authors = [ {name = "pvolnov", email = "notanemail@gmail.com"} ]
 license = {file = "LICENSE"} # relative to the package/ directory
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `py_near_primitives-0.1.1/src/lib.rs` & `py_near_primitives-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_near_primitives-0.1.1/Cargo.lock` & `py_near_primitives-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1113,17 +1113,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "libsecp256k1"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c9d220bc1feda2ac231cb78c3d26f27676b8cf82c96971f7aeef3d0cf2797c73"
 dependencies = [
```

### Comparing `py_near_primitives-0.1.1/PKG-INFO` & `py_near_primitives-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_near_primitives
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python bindings for NEAR Rust primitives.
 Author-email: pvolnov <notanemail@gmail.com>
 License: MIT
```

