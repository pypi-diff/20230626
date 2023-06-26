# Comparing `tmp/rabeffi-0.1.0.tar.gz` & `tmp/rabeffi-0.1.1.tar.gz`

## Comparing `rabeffi-0.1.0.tar` & `rabeffi-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 rabeffi-0.1.0/Cargo.toml
--rw-r--r--   0     1008     1001     1152 2023-06-26 05:02:46.000000 rabeffi-0.1.0/.github/workflows/rabe-actions.yml
--rwxr-xr-x   0     1008     1001       42 2023-06-26 05:09:09.000000 rabeffi-0.1.0/.gitignore
--rw-r--r--   0     1008     1001      791 2023-06-26 05:02:46.000000 rabeffi-0.1.0/README.md
--rwxr-xr-x   0     1008     1001      411 2023-06-26 05:02:46.000000 rabeffi-0.1.0/build.rs
--rw-r--r--   0     1008     1001      315 2023-06-26 05:04:18.000000 rabeffi-0.1.0/pyproject.toml
--rw-r--r--   0     1008     1001    16171 2023-06-26 05:12:56.000000 rabeffi-0.1.0/rabe.h
--rw-r--r--   0     1008     1001      101 2023-06-26 05:06:23.000000 rabeffi-0.1.0/rabeffi.pyi
--rwxr-xr-x   0     1008     1001     3684 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/common.rs
--rw-r--r--   0     1008     1001     6271 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/cp_abe/ac17.rs
--rw-r--r--   0     1008     1001     8661 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/cp_abe/aw11.rs
--rw-r--r--   0     1008     1001    16317 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/cp_abe/bdabe.rs
--rw-r--r--   0     1008     1001     6748 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/cp_abe/bsw.rs
--rw-r--r--   0     1008     1001    16461 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/cp_abe/mke08.rs
--rwxr-xr-x   0     1008     1001       86 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/cp_abe/mod.rs
--rw-r--r--   0     1008     1001     5806 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/kp_abe/ac17.rs
--rw-r--r--   0     1008     1001     6688 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/kp_abe/lsw.rs
--rwxr-xr-x   0     1008     1001       42 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/kp_abe/mod.rs
--rw-r--r--   0     1008     1001     7017 2023-06-26 05:02:46.000000 rabeffi-0.1.0/src/kp_abe/yct14.rs
--rwxr-xr-x   0     1008     1001      105 2023-06-26 05:03:49.000000 rabeffi-0.1.0/src/lib.rs
--rw-r--r--   0     1008     1001      536 2023-06-26 05:06:21.000000 rabeffi-0.1.0/src/py_module.rs
--rw-r--r--   0     1008     1001       51 2023-06-26 05:07:57.000000 rabeffi-0.1.0/test.py
--rw-r--r--   0     1008     1001    24850 2023-06-26 05:04:40.000000 rabeffi-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 rabeffi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 rabeffi-0.1.1/Cargo.toml
+-rw-r--r--   0     1008     1001     1152 2023-06-26 05:02:46.000000 rabeffi-0.1.1/.github/workflows/rabe-actions.yml
+-rwxr-xr-x   0     1008     1001       42 2023-06-26 05:09:09.000000 rabeffi-0.1.1/.gitignore
+-rw-r--r--   0     1008     1001      791 2023-06-26 05:02:46.000000 rabeffi-0.1.1/README.md
+-rwxr-xr-x   0     1008     1001      411 2023-06-26 05:02:46.000000 rabeffi-0.1.1/build.rs
+-rw-r--r--   0     1008     1001      315 2023-06-26 05:20:19.000000 rabeffi-0.1.1/pyproject.toml
+-rw-r--r--   0     1008     1001     8225 2023-06-26 05:17:57.000000 rabeffi-0.1.1/rabe.h
+-rw-r--r--   0     1008     1001      101 2023-06-26 05:06:23.000000 rabeffi-0.1.1/rabeffi.pyi
+-rwxr-xr-x   0     1008     1001     3684 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/common.rs
+-rw-r--r--   0     1008     1001     6271 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/cp_abe/ac17.rs
+-rw-r--r--   0     1008     1001     8661 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/cp_abe/aw11.rs
+-rw-r--r--   0     1008     1001    16317 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/cp_abe/bdabe.rs
+-rw-r--r--   0     1008     1001     6748 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/cp_abe/bsw.rs
+-rw-r--r--   0     1008     1001    16461 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/cp_abe/mke08.rs
+-rwxr-xr-x   0     1008     1001       86 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/cp_abe/mod.rs
+-rw-r--r--   0     1008     1001     5806 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/kp_abe/ac17.rs
+-rw-r--r--   0     1008     1001     6688 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/kp_abe/lsw.rs
+-rwxr-xr-x   0     1008     1001       42 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/kp_abe/mod.rs
+-rw-r--r--   0     1008     1001     7017 2023-06-26 05:02:46.000000 rabeffi-0.1.1/src/kp_abe/yct14.rs
+-rwxr-xr-x   0     1008     1001      105 2023-06-26 05:03:49.000000 rabeffi-0.1.1/src/lib.rs
+-rw-r--r--   0     1008     1001      536 2023-06-26 05:06:21.000000 rabeffi-0.1.1/src/py_module.rs
+-rw-r--r--   0     1008     1001       51 2023-06-26 05:07:57.000000 rabeffi-0.1.1/test.py
+-rw-r--r--   0     1008     1001    24849 2023-06-26 05:20:16.000000 rabeffi-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 rabeffi-0.1.1/PKG-INFO
```

### Comparing `rabeffi-0.1.0/Cargo.toml` & `rabeffi-0.1.1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
-name = "rabe-ffi"
-version = "0.1.0"
+name = "rabeffi"
+version = "0.1.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 crate-type = ["cdylib","staticlib"]
```

### Comparing `rabeffi-0.1.0/.github/workflows/rabe-actions.yml` & `rabeffi-0.1.1/.github/workflows/rabe-actions.yml`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/README.md` & `rabeffi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/common.rs` & `rabeffi-0.1.1/src/common.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/cp_abe/ac17.rs` & `rabeffi-0.1.1/src/cp_abe/ac17.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/cp_abe/aw11.rs` & `rabeffi-0.1.1/src/cp_abe/aw11.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/cp_abe/bdabe.rs` & `rabeffi-0.1.1/src/cp_abe/bdabe.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/cp_abe/bsw.rs` & `rabeffi-0.1.1/src/cp_abe/bsw.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/cp_abe/mke08.rs` & `rabeffi-0.1.1/src/cp_abe/mke08.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/kp_abe/ac17.rs` & `rabeffi-0.1.1/src/kp_abe/ac17.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/kp_abe/lsw.rs` & `rabeffi-0.1.1/src/kp_abe/lsw.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/kp_abe/yct14.rs` & `rabeffi-0.1.1/src/kp_abe/yct14.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/src/py_module.rs` & `rabeffi-0.1.1/src/py_module.rs`

 * *Files identical despite different names*

### Comparing `rabeffi-0.1.0/Cargo.lock` & `rabeffi-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -595,16 +595,16 @@
 dependencies = [
  "byteorder",
  "rand",
  "serde",
 ]
 
 [[package]]
-name = "rabe-ffi"
-version = "0.1.0"
+name = "rabeffi"
+version = "0.1.1"
 dependencies = [
  "cbindgen",
  "libc",
  "pyo3",
  "rabe",
  "serde",
  "serde_json",
```

### Comparing `rabeffi-0.1.0/PKG-INFO` & `rabeffi-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabeffi
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # Rabe-ffi
```

