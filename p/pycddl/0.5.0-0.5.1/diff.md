# Comparing `tmp/pycddl-0.5.0.tar.gz` & `tmp/pycddl-0.5.1.tar.gz`

## Comparing `pycddl-0.5.0.tar` & `pycddl-0.5.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 pycddl-0.5.0/Cargo.toml
--rw-rw-rw-   0        0        0      239 2023-06-13 21:10:07.000000 pycddl-0.5.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0       46 2023-06-13 21:10:07.000000 pycddl-0.5.0/.dir-locals.el
--rw-rw-rw-   0        0        0       50 2023-06-13 21:10:07.000000 pycddl-0.5.0/.flake8
--rw-rw-rw-   0        0        0       31 2023-06-13 21:10:07.000000 pycddl-0.5.0/.gitignore
--rw-rw-rw-   0        0        0     2457 2023-06-13 21:10:07.000000 pycddl-0.5.0/.gitlab-ci.yml
--rw-rw-rw-   0        0        0     1079 2023-06-13 21:10:07.000000 pycddl-0.5.0/LICENSE
--rw-rw-rw-   0        0        0       58 2023-06-13 21:10:07.000000 pycddl-0.5.0/Makefile
--rw-rw-rw-   0        0        0     2223 2023-06-13 21:10:07.000000 pycddl-0.5.0/README.md
--rw-rw-rw-   0        0        0      795 2023-06-13 21:10:07.000000 pycddl-0.5.0/RELEASE.md
--rw-rw-rw-   0        0        0      116 2023-06-13 21:10:07.000000 pycddl-0.5.0/build.rs
--rw-rw-rw-   0        0        0     1352 2023-06-13 21:10:07.000000 pycddl-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      773 2023-06-13 21:10:07.000000 pycddl-0.5.0/pysrc/pycddl/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-13 21:10:07.000000 pycddl-0.5.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       63 2023-06-13 21:10:07.000000 pycddl-0.5.0/rust-toolchain.toml
--rw-rw-rw-   0        0        0     3735 2023-06-13 21:10:07.000000 pycddl-0.5.0/src/lib.rs
--rw-rw-rw-   0        0        0        0 2023-06-13 21:10:07.000000 pycddl-0.5.0/tests/__init__.py
--rw-rw-rw-   0        0        0      616 2023-06-13 21:10:07.000000 pycddl-0.5.0/tests/test_benchmarks.py
--rw-rw-rw-   0        0        0     6456 2023-06-13 21:10:07.000000 pycddl-0.5.0/tests/test_cddl.py
--rw-rw-rw-   0        0        0      820 2023-06-13 21:10:07.000000 pycddl-0.5.0/tests/utils.py
--rw-rw-rw-   0        0        0    32557 2023-06-13 21:10:07.000000 pycddl-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 pycddl-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 pycddl-0.5.1/Cargo.toml
+-rw-rw-rw-   0        0        0      239 2023-06-26 21:06:01.000000 pycddl-0.5.1/.bumpversion.cfg
+-rw-rw-rw-   0        0        0       46 2023-06-26 21:06:01.000000 pycddl-0.5.1/.dir-locals.el
+-rw-rw-rw-   0        0        0       50 2023-06-26 21:06:01.000000 pycddl-0.5.1/.flake8
+-rw-rw-rw-   0        0        0       31 2023-06-26 21:06:01.000000 pycddl-0.5.1/.gitignore
+-rw-rw-rw-   0        0        0     2457 2023-06-26 21:06:01.000000 pycddl-0.5.1/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     1079 2023-06-26 21:06:01.000000 pycddl-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-06-26 21:06:01.000000 pycddl-0.5.1/Makefile
+-rw-rw-rw-   0        0        0     2297 2023-06-26 21:06:01.000000 pycddl-0.5.1/README.md
+-rw-rw-rw-   0        0        0      800 2023-06-26 21:06:01.000000 pycddl-0.5.1/RELEASE.md
+-rw-rw-rw-   0        0        0      116 2023-06-26 21:06:01.000000 pycddl-0.5.1/build.rs
+-rw-rw-rw-   0        0        0     1352 2023-06-26 21:06:01.000000 pycddl-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0      773 2023-06-26 21:06:01.000000 pycddl-0.5.1/pysrc/pycddl/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-26 21:06:01.000000 pycddl-0.5.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       63 2023-06-26 21:06:01.000000 pycddl-0.5.1/rust-toolchain.toml
+-rw-rw-rw-   0        0        0     3735 2023-06-26 21:06:01.000000 pycddl-0.5.1/src/lib.rs
+-rw-rw-rw-   0        0        0        0 2023-06-26 21:06:01.000000 pycddl-0.5.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      616 2023-06-26 21:06:01.000000 pycddl-0.5.1/tests/test_benchmarks.py
+-rw-rw-rw-   0        0        0     6456 2023-06-26 21:06:01.000000 pycddl-0.5.1/tests/test_cddl.py
+-rw-rw-rw-   0        0        0      820 2023-06-26 21:06:01.000000 pycddl-0.5.1/tests/utils.py
+-rw-rw-rw-   0        0        0    33437 2023-06-26 21:06:37.000000 pycddl-0.5.1/Cargo.lock
+-rw-r--r--   0        0        0     2610 1970-01-01 00:00:00.000000 pycddl-0.5.1/PKG-INFO
```

### Comparing `pycddl-0.5.0/Cargo.toml` & `pycddl-0.5.1/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [package]
 name = "pycddl"
-version = "0.5.0"  # pycddl version, for bumpversion
+version = "0.5.1"  # pycddl version, for bumpversion
 edition = "2021"
 license = "MIT"
 authors = ["Tahoe-LAFS project"]
 description = "Validate CBOR documents using CDDL schema language"
 homepage = "https://gitlab.com/tahoe-lafs/pycddl"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "pycddl"
 crate-type = ["cdylib"]
 
 [dependencies]
-cddl = "0.9"
+cddl = {git = "https://github.com/anweiss/cddl.git"}
 ciborium = "0.2"
 self_cell = "1.0"
 pyo3 = { version = "0.19", features = ["extension-module"] }
 
 [build-dependencies]
 pyo3-build-config = { version = "0.19", features = ["resolve-config"] }
```

### Comparing `pycddl-0.5.0/.gitlab-ci.yml` & `pycddl-0.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pycddl-0.5.0/LICENSE` & `pycddl-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycddl-0.5.0/README.md` & `pycddl-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 In order to reduce memory usage, you can pass in any Python object that implements the buffer API and stores bytes, e.g. a `memoryview()` or a `mmap` object.
 
 **The passed-in object must be read-only, and the data must not change during validation!**
 If you mutate the data while validation is happening the result can be memory corruption or other [undefined behavior](https://stackoverflow.com/questions/18506029/can-undefined-behavior-erase-the-hard-drive#comment27209771_18506029).
 
 ## Release notes
 
+### 0.5.1
+
+* Upgrade to newer `cddl` crate, fixing some validation bugs.
+
 ### 0.5.0
 
 * Support for ARM macOS.
 * Dropped Python 3.7 support.
 
 ### 0.4.1
```

### Comparing `pycddl-0.5.0/RELEASE.md` & `pycddl-0.5.1/RELEASE.md`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## How it works
 
 GitLab CI automation will automatically upload wheels to PyPI on tagged versions.
 So we need to do a Git tag.
 At the same time, the wheel versions come out of `Cargo.toml` (via the [Maturin packaging tool](https://maturin.rs/)).
 
-So we use [bump2version](https://github.com/c4urself/bump2version/) to both update `Cargo.toml` and add a matching Git tag at the same time.
+So we use [bump2version](https://github.com/c4urself/bump2version/) to update `Cargo.toml`, and then separately add a matching Git tag in GitLab.
 
 ## How to do it
 
 1. `pip install bump2version`
 2. Make sure you're on `main` git branch, or in PR that will get merged soon.
 3. `bump2version --no-tag --no-commit --current-version 0.x.y minor` (or `patch`, depending)
 4. Rebuild.
```

### Comparing `pycddl-0.5.0/pyproject.toml` & `pycddl-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycddl-0.5.0/pysrc/pycddl/__init__.py` & `pycddl-0.5.1/pysrc/pycddl/__init__.py`

 * *Files identical despite different names*

### Comparing `pycddl-0.5.0/src/lib.rs` & `pycddl-0.5.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pycddl-0.5.0/tests/test_benchmarks.py` & `pycddl-0.5.1/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pycddl-0.5.0/tests/test_cddl.py` & `pycddl-0.5.1/tests/test_cddl.py`

 * *Files identical despite different names*

### Comparing `pycddl-0.5.0/tests/utils.py` & `pycddl-0.5.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pycddl-0.5.0/Cargo.lock` & `pycddl-0.5.1/Cargo.lock`

 * *Files 5% similar despite different names*

```diff
@@ -75,23 +75,23 @@
 name = "base16"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d27c3610c36aee21ce8ac510e6224498de4228ad772a171ed65643a24693a5a8"
 
 [[package]]
 name = "base64"
-version = "0.13.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "base64-url"
-version = "1.4.13"
+version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67a99c239d0c7e77c85dddfa9cebce48704b3c49550fcd3b84dd637e4484899f"
+checksum = "9c5b0a88aa36e9f095ee2e2b13fb8c5e4313e022783aedacc123328c0084916d"
 dependencies = [
  "base64",
 ]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
@@ -118,36 +118,35 @@
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cddl"
 version = "0.9.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "286a21bdd91f4cab45c26ae7310f73aedf1e8f6fe21e210d220c449991c7fcf4"
+source = "git+https://github.com/anweiss/cddl.git#4cf8dd2dd810e55fafa76e176275c53485cccd24"
 dependencies = [
  "abnf_to_pest",
  "base16",
- "base64",
  "base64-url",
  "chrono",
  "ciborium",
  "clap",
  "codespan-reporting",
  "console_error_panic_hook",
  "crossterm",
+ "data-encoding",
  "displaydoc",
  "hexf-parse",
  "itertools",
  "lexical-core",
  "log",
  "pest_meta",
  "pest_vm",
  "regex",
- "regex-syntax 0.6.29",
+ "regex-syntax",
  "serde",
  "serde-wasm-bindgen",
  "serde_json",
  "simplelog",
  "uriparse",
  "wasm-bindgen",
 ]
@@ -164,15 +163,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
- "time",
+ "time 0.1.45",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "ciborium"
 version = "0.2.1"
@@ -263,26 +262,26 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.7"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crossterm"
-version = "0.25.0"
+version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e64e6c0fbe2c17357405f7c758c1ef960fce08bdfb2c03d88d2a18d7e09c4b67"
+checksum = "a84cda67535339806297f1b331d6dd6320470d2a0fe65381e79ee9e156dd3d13"
 dependencies = [
  "bitflags",
  "crossterm_winapi",
  "libc",
  "mio",
  "parking_lot",
  "signal-hook",
@@ -306,14 +305,20 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
+name = "data-encoding"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
+
+[[package]]
 name = "digest"
 version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
@@ -323,15 +328,15 @@
 name = "displaydoc"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
@@ -516,17 +521,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.146"
+version = "0.2.147"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
 
 [[package]]
 name = "lock_api"
 version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
@@ -589,14 +594,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "num_threads"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "os_str_bytes"
@@ -625,38 +639,38 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "pest"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
+checksum = "f73935e4d55e2abf7f130186537b19e7a4abc886a0252380b59248af473a3fc9"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
+checksum = "a01f71cb40bd8bb94232df14b946909e14660e33fc05db3e50ae2a82d7ea0ca0"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
 name = "pest_vm"
-version = "2.6.0"
+version = "2.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "910fc201ae72f3391e17ef56d12d95d7d537d68bdf572758edaca76c9349624f"
+checksum = "674aab48b903ab99b2557d34744ba69f7c108ab37eaf3b9a732ba136c84a3454"
 dependencies = [
  "pest",
  "pest_meta",
 ]
 
 [[package]]
 name = "pretty"
@@ -692,24 +706,24 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.60"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pycddl"
-version = "0.5.0"
+version = "0.5.1"
 dependencies = [
  "cddl",
  "ciborium",
  "pyo3",
  "pyo3-build-config",
  "self_cell",
 ]
@@ -794,25 +808,19 @@
 
 [[package]]
 name = "regex"
 version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
- "regex-syntax 0.7.2",
+ "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.29"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
-
-[[package]]
-name = "regex-syntax"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "ryu"
 version = "1.0.13"
@@ -823,65 +831,65 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "self_cell"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a3926e239738d36060909ffe6f511502f92149a45a1fade7fe031cb2d33e88b"
+checksum = "4c309e515543e67811222dbc9e3dd7e1056279b782e1dacffe4242b718734fb6"
 
 [[package]]
 name = "serde"
 version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
-version = "0.4.5"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3b4c031cd0d9014307d82b8abf653c0290fbdaeb4c02d00c63cf52f728628bf"
+checksum = "f3b143e2833c57ab9ad3ea280d21fd34e285a42837aeb0ee301f4f41890fa00e"
 dependencies = [
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
 version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.96"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -912,21 +920,21 @@
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simplelog"
-version = "0.11.2"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1348164456f72ca0116e4538bdaabb0ddb622c7d9f16387c725af3e96d6001c"
+checksum = "acee08041c5de3d5048c8b3f6f13fafb3026b24ba43c6a695a0c76179b844369"
 dependencies = [
- "chrono",
  "log",
  "termcolor",
+ "time 0.3.22",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
@@ -952,28 +960,28 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "2efbeae7acf4eabd6bcdcbd11c92f45231ddda7539edc7806bd1a04a03b24616"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.7"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "termcolor"
 version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
 dependencies = [
@@ -999,29 +1007,58 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
 dependencies = [
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
+name = "time"
+version = "0.3.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
+dependencies = [
+ "itoa",
+ "libc",
+ "num_threads",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+
+[[package]]
+name = "time-macros"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+dependencies = [
+ "time-core",
+]
+
+[[package]]
 name = "typed-arena"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typenum"
@@ -1104,15 +1141,15 @@
 checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1126,15 +1163,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.22",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.87"
```

### Comparing `pycddl-0.5.0/PKG-INFO` & `pycddl-0.5.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycddl
-Version: 0.5.0
+Version: 0.5.1
 License-File: LICENSE
 Summary: Validate CBOR documents using CDDL schema language
 Home-Page: https://gitlab.com/tahoe-lafs/pycddl
 Author: Tahoe-LAFS project
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -36,14 +36,18 @@
 In order to reduce memory usage, you can pass in any Python object that implements the buffer API and stores bytes, e.g. a `memoryview()` or a `mmap` object.
 
 **The passed-in object must be read-only, and the data must not change during validation!**
 If you mutate the data while validation is happening the result can be memory corruption or other [undefined behavior](https://stackoverflow.com/questions/18506029/can-undefined-behavior-erase-the-hard-drive#comment27209771_18506029).
 
 ## Release notes
 
+### 0.5.1
+
+* Upgrade to newer `cddl` crate, fixing some validation bugs.
+
 ### 0.5.0
 
 * Support for ARM macOS.
 * Dropped Python 3.7 support.
 
 ### 0.4.1
```

