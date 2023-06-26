# Comparing `tmp/chainner_ext-0.0.0.tar.gz` & `tmp/chainner_ext-0.1.0.tar.gz`

## Comparing `chainner_ext-0.0.0.tar` & `chainner_ext-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,37 @@
--rw-r--r--   0        0        0      158 1970-01-01 00:00:00.000000 chainner_ext-0.0.0/local_dependencies/image-core/Cargo.toml
--rw-r--r--   0     1001      123     3497 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-core/src/image.rs
--rw-r--r--   0     1001      123       71 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-core/src/lib.rs
--rw-r--r--   0     1001      123     2020 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-core/src/ndim.rs
--rw-r--r--   0     1001      123     5326 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-core/src/util.rs
--rw-r--r--   0        0        0      285 1970-01-01 00:00:00.000000 chainner_ext-0.0.0/local_dependencies/image-ops/Cargo.toml
--rw-r--r--   0     1001      123   715105 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fill_alpha_color.png
--rw-r--r--   0     1001      123   686932 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fill_alpha_nearest.png
--rw-r--r--   0     1001      123   948084 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fill_alpha_texture.png
--rw-r--r--   0     1001      123   368895 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fragment_blur.png
--rw-r--r--   0     1001      123   885535 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fragment_blur_alpha-1.png
--rw-r--r--   0     1001      123  1325732 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fragment_blur_alpha-2.png
--rw-r--r--   0     1001      123   101770 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/nearest_neighbor_200.png
--rw-r--r--   0     1001      123   630755 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/nearest_neighbor_4x.png
--rw-r--r--   0     1001      123  1482001 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/overlay_mut.png
--rw-r--r--   0     1001      123  1482001 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/overlay_self_mut.png
--rw-r--r--   0     1001      123     1860 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/benches/my_benchmark.rs
--rw-r--r--   0     1001      123     1682 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/blend.rs
--rw-r--r--   0     1001      123    12620 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/fill_alpha.rs
--rw-r--r--   0     1001      123     5446 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/fragment_blur.rs
--rw-r--r--   0     1001      123       83 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/lib.rs
--rw-r--r--   0     1001      123     2372 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/scale.rs
--rw-r--r--   0     1001      123     3342 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/util/bits.rs
--rw-r--r--   0     1001      123     6946 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/util/grid.rs
--rw-r--r--   0     1001      123     1747 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/util/image.rs
--rw-r--r--   0     1001      123      917 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/local_dependencies/image-ops/src/util/mod.rs
--rw-r--r--   0        0        0      417 1970-01-01 00:00:00.000000 chainner_ext-0.0.0/Cargo.toml
--rw-r--r--   0     1001      123      361 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/chainner_ext.pyi
--rw-r--r--   0     1001      123      775 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/pyproject.toml
--rw-r--r--   0     1001      123     5439 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/src/convert.rs
--rw-r--r--   0     1001      123     4088 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/src/lib.rs
--rw-r--r--   0     1001      123    32276 2023-06-14 09:27:29.000000 chainner_ext-0.0.0/Cargo.lock
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 chainner_ext-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0      285 1970-01-01 00:00:00.000000 chainner_ext-0.1.0/local_dependencies/image-ops/Cargo.toml
+-rw-r--r--   0     1001      123   715105 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fill_alpha_color.png
+-rw-r--r--   0     1001      123   686932 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fill_alpha_nearest.png
+-rw-r--r--   0     1001      123   948084 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fill_alpha_texture.png
+-rw-r--r--   0     1001      123   368895 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fragment_blur.png
+-rw-r--r--   0     1001      123   885535 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fragment_blur_alpha-1.png
+-rw-r--r--   0     1001      123  1325732 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fragment_blur_alpha-2.png
+-rw-r--r--   0     1001      123   101770 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/nearest_neighbor_200.png
+-rw-r--r--   0     1001      123   630755 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/nearest_neighbor_4x.png
+-rw-r--r--   0     1001      123  1482001 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/overlay_mut.png
+-rw-r--r--   0     1001      123  1482001 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/overlay_self_mut.png
+-rw-r--r--   0     1001      123     1860 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/benches/my_benchmark.rs
+-rw-r--r--   0     1001      123     1682 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/blend.rs
+-rw-r--r--   0     1001      123    12620 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/fill_alpha.rs
+-rw-r--r--   0     1001      123     5446 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/fragment_blur.rs
+-rw-r--r--   0     1001      123       83 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/lib.rs
+-rw-r--r--   0     1001      123     2372 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/scale.rs
+-rw-r--r--   0     1001      123     3342 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/util/bits.rs
+-rw-r--r--   0     1001      123     6946 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/util/grid.rs
+-rw-r--r--   0     1001      123     1747 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/util/image.rs
+-rw-r--r--   0     1001      123      917 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-ops/src/util/mod.rs
+-rw-r--r--   0        0        0      158 1970-01-01 00:00:00.000000 chainner_ext-0.1.0/local_dependencies/image-core/Cargo.toml
+-rw-r--r--   0     1001      123     3497 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-core/src/image.rs
+-rw-r--r--   0     1001      123       71 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-core/src/lib.rs
+-rw-r--r--   0     1001      123     2020 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-core/src/ndim.rs
+-rw-r--r--   0     1001      123     5326 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/image-core/src/util.rs
+-rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 chainner_ext-0.1.0/local_dependencies/regex-py/Cargo.toml
+-rw-r--r--   0     1001      123     4739 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/regex-py/src/lib.rs
+-rw-r--r--   0     1001      123     1538 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/local_dependencies/regex-py/src/position.rs
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 chainner_ext-0.1.0/Cargo.toml
+-rw-r--r--   0     1001      123     1451 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/chainner_ext.pyi
+-rw-r--r--   0     1001      123      775 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/pyproject.toml
+-rw-r--r--   0     1001      123     5439 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/src/convert.rs
+-rw-r--r--   0     1001      123     4222 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/src/lib.rs
+-rw-r--r--   0     1001      123     2444 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/src/regex.rs
+-rw-r--r--   0     1001      123    32810 2023-06-26 12:19:29.000000 chainner_ext-0.1.0/Cargo.lock
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 chainner_ext-0.1.0/PKG-INFO
```

### Comparing `chainner_ext-0.0.0/local_dependencies/image-core/src/image.rs` & `chainner_ext-0.1.0/local_dependencies/image-core/src/image.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-core/src/ndim.rs` & `chainner_ext-0.1.0/local_dependencies/image-core/src/ndim.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-core/src/util.rs` & `chainner_ext-0.1.0/local_dependencies/image-core/src/util.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fill_alpha_color.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fill_alpha_color.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fill_alpha_nearest.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fill_alpha_nearest.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fill_alpha_texture.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fill_alpha_texture.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fragment_blur.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fragment_blur.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fragment_blur_alpha-1.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fragment_blur_alpha-1.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/fragment_blur_alpha-2.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/fragment_blur_alpha-2.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/nearest_neighbor_200.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/nearest_neighbor_200.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/nearest_neighbor_4x.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/nearest_neighbor_4x.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/overlay_mut.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/overlay_mut.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/__snapshots/overlay_self_mut.png` & `chainner_ext-0.1.0/local_dependencies/image-ops/__snapshots/overlay_self_mut.png`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/benches/my_benchmark.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/benches/my_benchmark.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/src/blend.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/src/blend.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/src/fill_alpha.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/src/fill_alpha.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/src/fragment_blur.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/src/fragment_blur.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/src/scale.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/src/scale.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/src/util/bits.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/src/util/bits.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/src/util/grid.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/src/util/grid.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/src/util/image.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/src/util/image.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/local_dependencies/image-ops/src/util/mod.rs` & `chainner_ext-0.1.0/local_dependencies/image-ops/src/util/mod.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/pyproject.toml` & `chainner_ext-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "chainner_ext"
-version = "0.0.0"
+version = "0.1.0"
 description = "Rust implementation of functionality used in chaiNNer"
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `chainner_ext-0.0.0/src/convert.rs` & `chainner_ext-0.1.0/src/convert.rs`

 * *Files identical despite different names*

### Comparing `chainner_ext-0.0.0/src/lib.rs` & `chainner_ext-0.1.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 mod convert;
+mod regex;
 
 use glam::Vec4;
 use image_core::{Image, Size};
 use image_ops::{
     fill_alpha::{fill_alpha, FillMode},
     scale::nearest_neighbor,
 };
@@ -34,14 +35,18 @@
         }
     };
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn chainner_ext(_py: Python, m: &PyModule) -> PyResult<()> {
+    m.add_class::<regex::RustRegex>()?;
+    m.add_class::<regex::MatchGroup>()?;
+    m.add_class::<regex::RegexMatch>()?;
+
     /// Test function
     #[pyfn(m)]
     fn test_invert<'py>(
         py: Python<'py>,
         img: PyReadonlyArrayDyn<f32>,
     ) -> PyResult<&'py PyArray3<f32>> {
         let img = load_image!(img);
```

### Comparing `chainner_ext-0.0.0/Cargo.lock` & `chainner_ext-0.1.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "aho-corasick"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "atomic-polyfill"
@@ -45,14 +54,15 @@
 version = "0.0.0"
 dependencies = [
  "glam",
  "image-core",
  "image-ops",
  "numpy",
  "pyo3",
+ "regex-py",
 ]
 
 [[package]]
 name = "bit_field"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc827186963e592360843fb5ba4b973e145841266c1357f7180c43526f2e5b61"
@@ -526,14 +536,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
 dependencies = [
  "rawpointer",
 ]
 
 [[package]]
+name = "memchr"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
+
+[[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
@@ -857,32 +873,41 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.2"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cce168fea28d3e05f158bda4576cf0c844d5045bc2cc3620fa0292ed5bb5814c"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
+ "aho-corasick",
+ "memchr",
  "regex-syntax",
 ]
 
 [[package]]
+name = "regex-py"
+version = "0.0.0"
+dependencies = [
+ "regex",
+]
+
+[[package]]
 name = "regex-syntax"
-version = "0.6.29"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "rstar"
-version = "0.10.0"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f39465655a1e3d8ae79c6d9e007f4953bfc5d55297602df9dc38f9ae9f1359a"
+checksum = "73111312eb7a2287d229f06c00ff35b51ddee180f017ab6dec1f69d62ac098d6"
 dependencies = [
  "heapless",
  "num-traits",
  "smallvec",
 ]
 
 [[package]]
```

### Comparing `chainner_ext-0.0.0/PKG-INFO` & `chainner_ext-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainner_ext
-Version: 0.0.0
+Version: 0.1.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Dist: numpy >=1.16.0
```

