# Comparing `tmp/symbolic-9.2.0.zip` & `tmp/symbolic-9.2.1.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 2333268 bytes, number of entries: 19
-drwxr-xr-x  2.0 unx        0 b- stor 22-Sep-28 09:00 symbolic-9.2.0/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Sep-28 09:00 symbolic-9.2.0/symbolic/
--rw-r--r--  2.0 unx  2372941 b- defN 22-Sep-28 09:00 symbolic-9.2.0/rustsrc.zip
--rw-r--r--  2.0 unx        6 b- defN 22-Sep-28 09:00 symbolic-9.2.0/version.txt
--rw-r--r--  2.0 unx      365 b- defN 22-Sep-28 09:00 symbolic-9.2.0/PKG-INFO
--rw-r--r--  2.0 unx       87 b- defN 22-Sep-28 09:00 symbolic-9.2.0/README
--rw-r--r--  2.0 unx     2945 b- defN 22-Sep-28 09:00 symbolic-9.2.0/setup.py
--rw-r--r--  2.0 unx     2065 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/sourcemapcache.py
--rw-r--r--  2.0 unx     5643 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/sourcemap.py
--rw-r--r--  2.0 unx      599 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/_compat.py
--rw-r--r--  2.0 unx     4828 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/utils.py
--rw-r--r--  2.0 unx     2253 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/proguard.py
--rw-r--r--  2.0 unx     1583 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/common.py
--rw-r--r--  2.0 unx     8555 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/debuginfo.py
--rw-r--r--  2.0 unx     5033 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/symcache.py
--rw-r--r--  2.0 unx      575 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/__init__.py
--rw-r--r--  2.0 unx     1499 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/exceptions.py
--rw-r--r--  2.0 unx     1698 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/cfi.py
--rw-r--r--  2.0 unx      454 b- defN 22-Sep-28 09:00 symbolic-9.2.0/symbolic/demangle.py
-19 files, 2411129 bytes uncompressed, 2330648 bytes compressed:  3.3%
+Zip file size: 2333317 bytes, number of entries: 19
+drwxr-xr-x  2.0 unx        0 b- stor 22-Sep-29 10:39 symbolic-9.2.1/
+drwxr-xr-x  2.0 unx        0 b- stor 22-Sep-29 10:39 symbolic-9.2.1/symbolic/
+-rw-r--r--  2.0 unx  2372986 b- defN 22-Sep-29 10:39 symbolic-9.2.1/rustsrc.zip
+-rw-r--r--  2.0 unx        6 b- defN 22-Sep-29 10:39 symbolic-9.2.1/version.txt
+-rw-r--r--  2.0 unx      365 b- defN 22-Sep-29 10:39 symbolic-9.2.1/PKG-INFO
+-rw-r--r--  2.0 unx       87 b- defN 22-Sep-29 10:39 symbolic-9.2.1/README
+-rw-r--r--  2.0 unx     2945 b- defN 22-Sep-29 10:39 symbolic-9.2.1/setup.py
+-rw-r--r--  2.0 unx     2065 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/sourcemapcache.py
+-rw-r--r--  2.0 unx     5643 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/sourcemap.py
+-rw-r--r--  2.0 unx      599 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/_compat.py
+-rw-r--r--  2.0 unx     4828 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/utils.py
+-rw-r--r--  2.0 unx     2253 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/proguard.py
+-rw-r--r--  2.0 unx     1583 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/common.py
+-rw-r--r--  2.0 unx     8555 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/debuginfo.py
+-rw-r--r--  2.0 unx     5033 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/symcache.py
+-rw-r--r--  2.0 unx      575 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/__init__.py
+-rw-r--r--  2.0 unx     1499 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/exceptions.py
+-rw-r--r--  2.0 unx     1698 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/cfi.py
+-rw-r--r--  2.0 unx      454 b- defN 22-Sep-29 10:39 symbolic-9.2.1/symbolic/demangle.py
+19 files, 2411174 bytes uncompressed, 2330697 bytes compressed:  3.3%
```

## zipnote {}

```diff
@@ -1,58 +1,58 @@
-Filename: symbolic-9.2.0/
+Filename: symbolic-9.2.1/
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/
+Filename: symbolic-9.2.1/symbolic/
 Comment: 
 
-Filename: symbolic-9.2.0/rustsrc.zip
+Filename: symbolic-9.2.1/rustsrc.zip
 Comment: 
 
-Filename: symbolic-9.2.0/version.txt
+Filename: symbolic-9.2.1/version.txt
 Comment: 
 
-Filename: symbolic-9.2.0/PKG-INFO
+Filename: symbolic-9.2.1/PKG-INFO
 Comment: 
 
-Filename: symbolic-9.2.0/README
+Filename: symbolic-9.2.1/README
 Comment: 
 
-Filename: symbolic-9.2.0/setup.py
+Filename: symbolic-9.2.1/setup.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/sourcemapcache.py
+Filename: symbolic-9.2.1/symbolic/sourcemapcache.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/sourcemap.py
+Filename: symbolic-9.2.1/symbolic/sourcemap.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/_compat.py
+Filename: symbolic-9.2.1/symbolic/_compat.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/utils.py
+Filename: symbolic-9.2.1/symbolic/utils.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/proguard.py
+Filename: symbolic-9.2.1/symbolic/proguard.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/common.py
+Filename: symbolic-9.2.1/symbolic/common.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/debuginfo.py
+Filename: symbolic-9.2.1/symbolic/debuginfo.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/symcache.py
+Filename: symbolic-9.2.1/symbolic/symcache.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/__init__.py
+Filename: symbolic-9.2.1/symbolic/__init__.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/exceptions.py
+Filename: symbolic-9.2.1/symbolic/exceptions.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/cfi.py
+Filename: symbolic-9.2.1/symbolic/cfi.py
 Comment: 
 
-Filename: symbolic-9.2.0/symbolic/demangle.py
+Filename: symbolic-9.2.1/symbolic/demangle.py
 Comment: 
 
 Zip file comment:
```

## Comparing `symbolic-9.2.0/rustsrc.zip` & `symbolic-9.2.1/rustsrc.zip`

 * *Files 9% similar despite different names*

### zipinfo {}

```diff
@@ -1,322 +1,322 @@
-Zip file size: 2372941 bytes, number of entries: 320
--rw-r--r--  2.0 unx      176 b- defN 22-Sep-28 09:00 rustsrc/.clang-format
--rw-r--r--  2.0 unx      144 b- defN 22-Sep-28 09:00 rustsrc/.codecov.yml
--rw-r--r--  2.0 unx      593 b- defN 22-Sep-28 09:00 rustsrc/.craft.yml
--rw-r--r--  2.0 unx      256 b- defN 22-Sep-28 09:00 rustsrc/.editorconfig
--rw-r--r--  2.0 unx       33 b- defN 22-Sep-28 09:00 rustsrc/.github/CODEOWNERS
--rw-r--r--  2.0 unx     2255 b- defN 22-Sep-28 09:00 rustsrc/.github/workflows/build.yml
--rw-r--r--  2.0 unx     3922 b- defN 22-Sep-28 09:00 rustsrc/.github/workflows/ci.yml
--rw-r--r--  2.0 unx      368 b- defN 22-Sep-28 09:00 rustsrc/.github/workflows/enforce-license-compliance.yml
--rw-r--r--  2.0 unx      861 b- defN 22-Sep-28 09:00 rustsrc/.github/workflows/release.yml
--rw-r--r--  2.0 unx     1004 b- defN 22-Sep-28 09:00 rustsrc/.github/workflows/weekly.yml
--rw-r--r--  2.0 unx     3329 b- defN 22-Sep-28 09:00 rustsrc/.vscode/c_cpp_properties.json
--rw-r--r--  2.0 unx      496 b- defN 22-Sep-28 09:00 rustsrc/.vscode/extensions.json
--rw-r--r--  2.0 unx      695 b- defN 22-Sep-28 09:00 rustsrc/.vscode/launch.json
--rw-r--r--  2.0 unx     1498 b- defN 22-Sep-28 09:00 rustsrc/.vscode/settings.json
--rw-r--r--  2.0 unx     2193 b- defN 22-Sep-28 09:00 rustsrc/.vscode/tasks.json
--rw-r--r--  2.0 unx    32276 b- defN 22-Sep-28 09:00 rustsrc/CHANGELOG.md
--rw-r--r--  2.0 unx      149 b- defN 22-Sep-28 09:00 rustsrc/Cargo.toml
--rw-r--r--  2.0 unx     1120 b- defN 22-Sep-28 09:00 rustsrc/LICENSE
--rw-r--r--  2.0 unx     1987 b- defN 22-Sep-28 09:00 rustsrc/Makefile
--rw-r--r--  2.0 unx     6228 b- defN 22-Sep-28 09:00 rustsrc/README.md
--rw-r--r--  2.0 unx      339 b- defN 22-Sep-28 09:00 rustsrc/examples/addr2line/Cargo.toml
--rw-r--r--  2.0 unx     6781 b- defN 22-Sep-28 09:00 rustsrc/examples/addr2line/src/main.rs
--rw-r--r--  2.0 unx      333 b- defN 22-Sep-28 09:00 rustsrc/examples/dump_cfi/Cargo.toml
--rw-r--r--  2.0 unx     1405 b- defN 22-Sep-28 09:00 rustsrc/examples/dump_cfi/src/main.rs
--rw-r--r--  2.0 unx      299 b- defN 22-Sep-28 09:00 rustsrc/examples/dump_sources/Cargo.toml
--rw-r--r--  2.0 unx     2495 b- defN 22-Sep-28 09:00 rustsrc/examples/dump_sources/src/main.rs
--rw-r--r--  2.0 unx      569 b- defN 22-Sep-28 09:00 rustsrc/examples/minidump_stackwalk/Cargo.toml
--rw-r--r--  2.0 unx    23996 b- defN 22-Sep-28 09:00 rustsrc/examples/minidump_stackwalk/src/main.rs
--rw-r--r--  2.0 unx      299 b- defN 22-Sep-28 09:00 rustsrc/examples/object_debug/Cargo.toml
--rw-r--r--  2.0 unx     2509 b- defN 22-Sep-28 09:00 rustsrc/examples/object_debug/src/main.rs
--rw-r--r--  2.0 unx      339 b- defN 22-Sep-28 09:00 rustsrc/examples/sourcemapcache_debug/Cargo.toml
--rw-r--r--  2.0 unx     3412 b- defN 22-Sep-28 09:00 rustsrc/examples/sourcemapcache_debug/src/main.rs
--rw-r--r--  2.0 unx      366 b- defN 22-Sep-28 09:00 rustsrc/examples/symcache_debug/Cargo.toml
--rw-r--r--  2.0 unx     8981 b- defN 22-Sep-28 09:00 rustsrc/examples/symcache_debug/src/main.rs
--rw-r--r--  2.0 unx      329 b- defN 22-Sep-28 09:00 rustsrc/examples/unreal_engine_crash/Cargo.toml
--rw-r--r--  2.0 unx     1741 b- defN 22-Sep-28 09:00 rustsrc/examples/unreal_engine_crash/src/main.rs
--rwxr-xr-x  2.0 unx      395 b- defN 22-Sep-28 09:00 rustsrc/run
--rwxr-xr-x  2.0 unx      536 b- defN 22-Sep-28 09:00 rustsrc/scripts/bump-version
--rwxr-xr-x  2.0 unx    19164 b- defN 22-Sep-28 09:00 rustsrc/scripts/git-archive-all
--rw-r--r--  2.0 unx      762 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/Cargo.toml
--rw-r--r--  2.0 unx      750 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/Makefile
--rw-r--r--  2.0 unx     3773 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/README.md
--rw-r--r--  2.0 unx     1661 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/c-tests/common.c
--rwxr-xr-x  2.0 unx     8576 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/c-tests/demangle
--rw-r--r--  2.0 unx     1603 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/c-tests/demangle.c
--rw-r--r--  2.0 unx     1155 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/c-tests/object.c
--rw-r--r--  2.0 unx      343 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/cbindgen.toml
--rw-r--r--  2.0 unx    21766 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/include/symbolic.h
--rw-r--r--  2.0 unx     2146 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/cfi.rs
--rw-r--r--  2.0 unx      822 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/common.rs
--rw-r--r--  2.0 unx    11582 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/core.rs
--rw-r--r--  2.0 unx     6771 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/debuginfo.rs
--rw-r--r--  2.0 unx     1524 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/demangle.rs
--rw-r--r--  2.0 unx      472 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/lib.rs
--rw-r--r--  2.0 unx     4173 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/proguard.rs
--rw-r--r--  2.0 unx     9538 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/sourcemap.rs
--rw-r--r--  2.0 unx     6126 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/sourcemapcache.rs
--rw-r--r--  2.0 unx     6456 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/symcache.rs
--rw-r--r--  2.0 unx     3717 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cabi/src/utils.rs
--rw-r--r--  2.0 unx      742 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/Cargo.toml
--rw-r--r--  2.0 unx    56096 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/src/lib.rs
--rw-r--r--  2.0 unx    59446 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_elf.snap
--rw-r--r--  2.0 unx    21639 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_macho.snap
--rw-r--r--  2.0 unx    15120 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_pdb_windows.snap
--rw-r--r--  2.0 unx     3056 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_pe_windows.snap
--rw-r--r--  2.0 unx    61807 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_sym_linux.snap
--rw-r--r--  2.0 unx    10563 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_sym_macos.snap
--rw-r--r--  2.0 unx    15192 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_sym_windows.snap
--rw-r--r--  2.0 unx     3116 b- defN 22-Sep-28 09:00 rustsrc/symbolic-cfi/tests/test_cfi.rs
--rw-r--r--  2.0 unx     1058 b- defN 22-Sep-28 09:00 rustsrc/symbolic-common/Cargo.toml
--rw-r--r--  2.0 unx     1140 b- defN 22-Sep-28 09:00 rustsrc/symbolic-common/README.md
--rw-r--r--  2.0 unx     8533 b- defN 22-Sep-28 09:00 rustsrc/symbolic-common/src/byteview.rs
--rw-r--r--  2.0 unx    11432 b- defN 22-Sep-28 09:00 rustsrc/symbolic-common/src/cell.rs
--rw-r--r--  2.0 unx    15395 b- defN 22-Sep-28 09:00 rustsrc/symbolic-common/src/heuristics.rs
--rw-r--r--  2.0 unx     1150 b- defN 22-Sep-28 09:00 rustsrc/symbolic-common/src/lib.rs
--rw-r--r--  2.0 unx    25127 b- defN 22-Sep-28 09:00 rustsrc/symbolic-common/src/path.rs
--rw-r--r--  2.0 unx    26431 b- defN 22-Sep-28 09:00 rustsrc/symbolic-common/src/types.rs
--rw-r--r--  2.0 unx     3160 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/Cargo.toml
--rw-r--r--  2.0 unx     2596 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/benches/breakpad_parser.rs
--rw-r--r--  2.0 unx      426 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/fuzz/Cargo.toml
--rw-r--r--  2.0 unx     2746 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/fuzz/fuzz_targets/fuzz_objects.rs
--rw-r--r--  2.0 unx    28225 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/base.rs
--rw-r--r--  2.0 unx    82454 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/breakpad.rs
--rw-r--r--  2.0 unx    59962 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/dwarf.rs
--rw-r--r--  2.0 unx    37245 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/elf.rs
--rw-r--r--  2.0 unx    15427 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/function_builder.rs
--rw-r--r--  2.0 unx     2275 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/function_stack.rs
--rw-r--r--  2.0 unx     2857 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/lib.rs
--rw-r--r--  2.0 unx    16214 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/macho/bcsymbolmap.rs
--rw-r--r--  2.0 unx   144055 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/macho/compact.rs
--rw-r--r--  2.0 unx    34173 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/macho/mod.rs
--rw-r--r--  2.0 unx     1971 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/macho/mono_archive.rs
--rw-r--r--  2.0 unx    27017 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/object.rs
--rw-r--r--  2.0 unx    36700 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/pdb.rs
--rw-r--r--  2.0 unx    12931 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/pe.rs
--rw-r--r--  2.0 unx    38896 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/sourcebundle.rs
--rw-r--r--  2.0 unx     8028 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/wasm.rs
--rw-r--r--  2.0 unx     9940 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/src/wasm/parser.rs
--rw-r--r--  2.0 unx   414364 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/fixtures/2d10c42f-591d-3265-b147-78ba0868073f.dwarf-hidden
--rw-r--r--  2.0 unx      273 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/fixtures/2d10c42f-591d-3265-b147-78ba0868073f.plist
--rw-r--r--  2.0 unx   141461 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/fixtures/c8374b6d-6e96-34d8-ae38-efaa5fec424f.bcsymbolmap
--rw-r--r--  2.0 unx      549 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/fixtures/invalid-symbols.fuzzed
--rw-r--r--  2.0 unx     1086 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__breakpad_files.snap
--rw-r--r--  2.0 unx    13300 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__breakpad_functions.snap
--rw-r--r--  2.0 unx    14425 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__breakpad_functions_mac_with_inlines.snap
--rw-r--r--  2.0 unx     1297 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__breakpad_symbols.snap
--rw-r--r--  2.0 unx      577 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__elf_files.snap
--rw-r--r--  2.0 unx    54908 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__elf_functions.snap
--rw-r--r--  2.0 unx    12737 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__elf_symbols.snap
--rw-r--r--  2.0 unx      596 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__mach_files.snap
--rw-r--r--  2.0 unx    11222 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__mach_functions.snap
--rw-r--r--  2.0 unx    14983 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__mach_symbols.snap
--rw-r--r--  2.0 unx     1086 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__pdb_files.snap
--rw-r--r--  2.0 unx    47625 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__pdb_functions.snap
--rw-r--r--  2.0 unx     7065 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__pdb_symbols.snap
--rw-r--r--  2.0 unx      125 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__wasm_symbols.snap
--rw-r--r--  2.0 unx    16732 b- defN 22-Sep-28 09:00 rustsrc/symbolic-debuginfo/tests/test_objects.rs
--rw-r--r--  2.0 unx     1151 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/Cargo.toml
--rw-r--r--  2.0 unx     1027 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/README.md
--rw-r--r--  2.0 unx      970 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/build.rs
--rw-r--r--  2.0 unx    16380 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/src/lib.rs
--rw-r--r--  2.0 unx     1286 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/src/swiftdemangle.cpp
--rw-r--r--  2.0 unx    15194 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/tests/test_cpp.rs
--rw-r--r--  2.0 unx     2289 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/tests/test_detection.rs
--rw-r--r--  2.0 unx     1743 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/tests/test_msvc.rs
--rw-r--r--  2.0 unx     1855 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/tests/test_objcpp.rs
--rw-r--r--  2.0 unx    21637 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/tests/test_swift.rs
--rw-r--r--  2.0 unx      978 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/tests/utils/mod.rs
--rw-r--r--  2.0 unx     1807 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/1-arguments.patch
--rw-r--r--  2.0 unx    11751 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/LICENSE.txt
--rw-r--r--  2.0 unx     3192 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/LICENSE_LLVM.txt
--rw-r--r--  2.0 unx     2139 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/README.md
--rw-r--r--  2.0 unx     2956 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm-c/DataTypes.h
--rw-r--r--  2.0 unx    26508 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/Hashing.h
--rw-r--r--  2.0 unx      983 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/None.h
--rw-r--r--  2.0 unx    13251 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/Optional.h
--rw-r--r--  2.0 unx    75337 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/STLExtras.h
--rw-r--r--  2.0 unx     2754 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/STLForwardCompat.h
--rw-r--r--  2.0 unx    45144 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/SmallVector.h
--rw-r--r--  2.0 unx    34006 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/StringRef.h
--rw-r--r--  2.0 unx     6423 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/StringSwitch.h
--rw-r--r--  2.0 unx    13081 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/iterator.h
--rw-r--r--  2.0 unx     2252 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/iterator_range.h
--rw-r--r--  2.0 unx     2512 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Config/abi-breaking.h
--rw-r--r--  2.0 unx     3555 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Config/llvm-config.h
--rw-r--r--  2.0 unx    14249 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/Casting.h
--rw-r--r--  2.0 unx    19785 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/Compiler.h
--rw-r--r--  2.0 unx      878 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/DataTypes.h
--rw-r--r--  2.0 unx     6567 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/ErrorHandling.h
--rw-r--r--  2.0 unx     3291 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/MemAlloc.h
--rw-r--r--  2.0 unx     4942 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/SwapByteOrder.h
--rw-r--r--  2.0 unx    25919 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/raw_ostream.h
--rw-r--r--  2.0 unx     6912 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/type_traits.h
--rw-r--r--  2.0 unx     4918 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/AST/Ownership.h
--rw-r--r--  2.0 unx     7601 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/AST/ReferenceStorage.def
--rw-r--r--  2.0 unx     5362 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Basic/Compiler.h
--rw-r--r--  2.0 unx     6983 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Basic/InlineBitfield.h
--rw-r--r--  2.0 unx     3310 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Basic/LLVM.h
--rw-r--r--  2.0 unx    25080 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Basic/STLExtras.h
--rw-r--r--  2.0 unx    21991 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/Demangle.h
--rw-r--r--  2.0 unx     9564 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/DemangleNodes.def
--rw-r--r--  2.0 unx    21028 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/Demangler.h
--rw-r--r--  2.0 unx     2880 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/ManglingMacros.h
--rw-r--r--  2.0 unx    11779 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/ManglingUtils.h
--rw-r--r--  2.0 unx     1272 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/NamespaceMacros.h
--rw-r--r--  2.0 unx     2634 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/Punycode.h
--rw-r--r--  2.0 unx     4145 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/StandardTypesMangling.def
--rw-r--r--  2.0 unx     1607 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/ValueWitnessMangling.def
--rw-r--r--  2.0 unx     1364 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Runtime/BackDeployment.h
--rw-r--r--  2.0 unx      249 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Runtime/CMakeConfig.h
--rw-r--r--  2.0 unx    17169 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Runtime/Config.h
--rw-r--r--  2.0 unx     6806 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/include/swift/Strings.h
--rw-r--r--  2.0 unx      903 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/CMakeLists.txt
--rw-r--r--  2.0 unx     8396 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/Context.cpp
--rw-r--r--  2.0 unx   121687 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/Demangler.cpp
--rw-r--r--  2.0 unx     2458 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/ManglingUtils.cpp
--rw-r--r--  2.0 unx     2330 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/NodeDumper.cpp
--rw-r--r--  2.0 unx   104235 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/NodePrinter.cpp
--rw-r--r--  2.0 unx    76600 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/OldDemangler.cpp
--rw-r--r--  2.0 unx    66585 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/OldRemangler.cpp
--rw-r--r--  2.0 unx    10799 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/Punycode.cpp
--rw-r--r--  2.0 unx    84209 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/Remangler.cpp
--rw-r--r--  2.0 unx     4806 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/RemanglerBase.h
--rw-r--r--  2.0 unx     9651 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/stdlib/public/SwiftShims/Visibility.h
--rwxr-xr-x  2.0 unx     3963 b- defN 22-Sep-28 09:00 rustsrc/symbolic-demangle/vendor/swift/update.py
--rw-r--r--  2.0 unx      546 b- defN 22-Sep-28 09:00 rustsrc/symbolic-il2cpp/Cargo.toml
--rw-r--r--  2.0 unx      321 b- defN 22-Sep-28 09:00 rustsrc/symbolic-il2cpp/src/lib.rs
--rw-r--r--  2.0 unx     8773 b- defN 22-Sep-28 09:00 rustsrc/symbolic-il2cpp/src/line_mapping/from_object.rs
--rw-r--r--  2.0 unx     4646 b- defN 22-Sep-28 09:00 rustsrc/symbolic-il2cpp/src/line_mapping/mod.rs
--rw-r--r--  2.0 unx      715 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/Cargo.toml
--rw-r--r--  2.0 unx      410 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/fuzz/Cargo.toml
--rw-r--r--  2.0 unx      900 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/fuzz/fuzz_targets/fuzz_ppdb.rs
--rw-r--r--  2.0 unx     2664 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/cache/lookup.rs
--rw-r--r--  2.0 unx     7593 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/cache/mod.rs
--rw-r--r--  2.0 unx     2833 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/cache/raw.rs
--rw-r--r--  2.0 unx     3850 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/cache/writer.rs
--rw-r--r--  2.0 unx    26510 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/format/metadata.rs
--rw-r--r--  2.0 unx    12054 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/format/mod.rs
--rw-r--r--  2.0 unx     2865 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/format/raw.rs
--rw-r--r--  2.0 unx     9457 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/format/sequence_points.rs
--rw-r--r--  2.0 unx     4116 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/format/streams.rs
--rw-r--r--  2.0 unx     4080 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/format/utils.rs
--rw-r--r--  2.0 unx     2859 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/src/lib.rs
--rw-r--r--  2.0 unx      772 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/tests/fixtures/Async.pdbx
--rw-r--r--  2.0 unx     3128 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/tests/fixtures/Documents.pdbx
--rw-r--r--  2.0 unx     1132 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/tests/fixtures/EmbeddedSource.pdbx
--rw-r--r--  2.0 unx     1016 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/tests/fixtures/MethodBoundaries.pdbx
--rw-r--r--  2.0 unx     1740 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/tests/fixtures/Scopes.pdbx
--rw-r--r--  2.0 unx      876 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/tests/fixtures/SourceLink.pdbx
--rw-r--r--  2.0 unx    10880 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/tests/fixtures/integration.pdb
--rw-r--r--  2.0 unx     2534 b- defN 22-Sep-28 09:00 rustsrc/symbolic-ppdb/tests/test_caches.rs
--rw-r--r--  2.0 unx      629 b- defN 22-Sep-28 09:00 rustsrc/symbolic-sourcemapcache/Cargo.toml
--rw-r--r--  2.0 unx      280 b- defN 22-Sep-28 09:00 rustsrc/symbolic-sourcemapcache/src/lib.rs
--rw-r--r--  2.0 unx    11209 b- defN 22-Sep-28 09:00 rustsrc/symbolic-sourcemapcache/src/lookup.rs
--rw-r--r--  2.0 unx     3780 b- defN 22-Sep-28 09:00 rustsrc/symbolic-sourcemapcache/src/raw.rs
--rw-r--r--  2.0 unx    12462 b- defN 22-Sep-28 09:00 rustsrc/symbolic-sourcemapcache/src/writer.rs
--rw-r--r--  2.0 unx    10051 b- defN 22-Sep-28 09:00 rustsrc/symbolic-sourcemapcache/tests/integration.rs
--rw-r--r--  2.0 unx     1213 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/Cargo.toml
--rw-r--r--  2.0 unx     1984 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/benches/bench_writer.rs
--rw-r--r--  2.0 unx     3169 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/src/error.rs
--rw-r--r--  2.0 unx     9621 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/src/lib.rs
--rw-r--r--  2.0 unx     9010 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/src/lookup.rs
--rw-r--r--  2.0 unx     4924 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/src/raw.rs
--rw-r--r--  2.0 unx     1603 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/src/transform/bcsymbolmap.rs
--rw-r--r--  2.0 unx     1401 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/src/transform/il2cpp.rs
--rw-r--r--  2.0 unx     2060 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/src/transform/mod.rs
--rw-r--r--  2.0 unx    21727 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/src/writer.rs
--rw-r--r--  2.0 unx     4937 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/breakpad.rs
--rw-r--r--  2.0 unx    12687 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/snapshots/test_cache__functions_linux.snap
--rw-r--r--  2.0 unx    14934 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/snapshots/test_cache__functions_macos.snap
--rw-r--r--  2.0 unx      754 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/snapshots/test_cache__lookup.snap
--rw-r--r--  2.0 unx    12688 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/snapshots/test_writer__functions_linux.snap
--rw-r--r--  2.0 unx    14935 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/snapshots/test_writer__functions_macos.snap
--rw-r--r--  2.0 unx      262 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/snapshots/test_writer__overlapping_funcs.snap
--rw-r--r--  2.0 unx     2396 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/test_cache.rs
--rw-r--r--  2.0 unx     1235 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/test_transformers.rs
--rw-r--r--  2.0 unx    12141 b- defN 22-Sep-28 09:00 rustsrc/symbolic-symcache/tests/test_writer.rs
--rw-r--r--  2.0 unx      169 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/Cargo.toml
--rw-r--r--  2.0 unx      168 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/libgallium_dri.sym
--rwxr-xr-x  2.0 unx   138024 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/crash
--rwxr-xr-x  2.0 unx  1450496 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/crash.debug
--rw-r--r--  2.0 unx    78235 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/crash.sym
--rw-r--r--  2.0 unx        9 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/debug_info.txt.crc
--rwxr-xr-x  2.0 unx    16000 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with123_debuglink
--rwxr-xr-x  2.0 unx    16000 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with12_debuglink
--rwxr-xr-x  2.0 unx    15992 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with1_debuglink
--rwxr-xr-x  2.0 unx    16032 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with_compressed_debuglink
--rwxr-xr-x  2.0 unx    15992 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with_debuglink
--rwxr-xr-x  2.0 unx    15896 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_without_debuglink
--rwxr-xr-x  2.0 unx     1736 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/generate_elf_debug_link.sh
--rw-r--r--  2.0 unx      648 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/Example.framework.dSYM/Contents/Info.plist
--rw-r--r--  2.0 unx    19320 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/Example.framework.dSYM/Contents/Resources/DWARF/Example
--rwxr-xr-x  2.0 unx   139580 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/crash
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/crash.app.dSYM/Contents/Resources/DWARF/crash
--rw-r--r--  2.0 unx      634 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/crash.dSYM/Contents/Info.plist
--rw-r--r--  2.0 unx   650058 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/crash.dSYM/Contents/Resources/DWARF/crash
--rw-r--r--  2.0 unx       57 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/crash.dSYM/Contents/Resources/DWARF/invalid
--rw-r--r--  2.0 unx   183389 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/crash.inlines.sym
--rw-r--r--  2.0 unx   111874 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/crash.sym
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/other.dSYM/Contents/Resources/DWARF/invalid
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/other.dmp.dSYM/Contents/Resources/DWARF/invalid
--rw-r--r--  2.0 unx     9680 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/macos/overlapping_funcs.dSYM/Contents/Resources/DWARF/overlapping_funcs
--rw-r--r--  2.0 unx   155342 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/regression/large_symbol.sym
--rw-r--r--  2.0 unx      242 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/README.md
--rw-r--r--  2.0 unx    64749 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/hermes-metro/react-native-hermes.map
--rw-r--r--  2.0 unx     9168 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/hermes-metro/react-native-metro.js
--rw-r--r--  2.0 unx    64417 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/hermes-metro/react-native-metro.js.map
--rw-r--r--  2.0 unx      208 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/inlining/module.js
--rw-r--r--  2.0 unx      873 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/inlining/module.js.map
--rw-r--r--  2.0 unx      294 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/nofiles.js
--rw-r--r--  2.0 unx      645 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/nofiles.js.map
--rw-r--r--  2.0 unx     1022 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/old-logs/simple.chrome.log
--rw-r--r--  2.0 unx     2172 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/old-logs/simple.firefox.log
--rw-r--r--  2.0 unx     3161 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/old-logs/simple.node.log
--rw-r--r--  2.0 unx     2855 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/old-logs/simple.safari.log
--rw-r--r--  2.0 unx    16183 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/preact-missing-source-contents.module.js.map
--rw-r--r--  2.0 unx    10031 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/preact.module.js
--rw-r--r--  2.0 unx    68935 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/preact.module.js.map
--rw-r--r--  2.0 unx       31 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/simple/minified.js
--rw-r--r--  2.0 unx      318 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/simple/minified.js.map
--rw-r--r--  2.0 unx      184 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/simple/original.js
--rw-r--r--  2.0 unx      747 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/async.mjs
--rw-r--r--  2.0 unx      114 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/shared.mjs
--rw-r--r--  2.0 unx     1473 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/sync.mjs
--rw-r--r--  2.0 unx       66 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/trace.html
--rw-r--r--  2.0 unx      408 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/trace.mjs
--rw-r--r--  2.0 unx      300 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/webpack/bundle.js
--rw-r--r--  2.0 unx     1716 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/sourcemapcache/webpack/bundle.js.map
--rw-r--r--  2.0 unx   121355 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/symcache/compat/v1.symc
--rw-r--r--  2.0 unx   222900 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/symcache/current/linux.symc
--rw-r--r--  2.0 unx   168461 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/symcache/current/macos.symc
--rw-r--r--  2.0 unx    42896 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/unreal/unreal_crash
--rw-r--r--  2.0 unx    33249 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/unreal/unreal_crash_apple
--rwxr-xr-x  2.0 unx     4293 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/wasm/simple.wasm
--rwxr-xr-x  2.0 unx    12800 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/windows/CrashWithException.exe
--rwxr-xr-x  2.0 unx   610304 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/windows/CrashWithException.pdb
--rwxr-xr-x  2.0 unx    20620 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/windows/CrashWithException.pdb.sym
--rwxr-xr-x  2.0 unx    19968 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/windows/crash.exe
--rwxr-xr-x  2.0 unx  1019904 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/windows/crash.pdb
--rwxr-xr-x  2.0 unx    46361 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/windows/crash.sym
--rw-r--r--  2.0 unx      254 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/xul.sym
--rw-r--r--  2.0 unx      422 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/fixtures/xul2.sym
--rw-r--r--  2.0 unx      367 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/overlapping_funcs/build.sh
--rw-r--r--  2.0 unx      101 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/overlapping_funcs/main.c
--rw-r--r--  2.0 unx      105 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/overlapping_funcs/testachio.c
--rw-r--r--  2.0 unx       52 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/overlapping_funcs/testachio.h
--rw-r--r--  2.0 unx      104 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/overlapping_funcs/testaroni.c
--rw-r--r--  2.0 unx       51 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/overlapping_funcs/testaroni.h
--rw-r--r--  2.0 unx      768 b- defN 22-Sep-28 09:00 rustsrc/symbolic-testutils/src/lib.rs
--rw-r--r--  2.0 unx     1248 b- defN 22-Sep-28 09:00 rustsrc/symbolic-unreal/Cargo.toml
--rw-r--r--  2.0 unx    14050 b- defN 22-Sep-28 09:00 rustsrc/symbolic-unreal/src/container.rs
--rw-r--r--  2.0 unx    26736 b- defN 22-Sep-28 09:00 rustsrc/symbolic-unreal/src/context.rs
--rw-r--r--  2.0 unx     2411 b- defN 22-Sep-28 09:00 rustsrc/symbolic-unreal/src/error.rs
--rw-r--r--  2.0 unx      195 b- defN 22-Sep-28 09:00 rustsrc/symbolic-unreal/src/lib.rs
--rw-r--r--  2.0 unx     6078 b- defN 22-Sep-28 09:00 rustsrc/symbolic-unreal/src/logs.rs
--rw-r--r--  2.0 unx     5302 b- defN 22-Sep-28 09:00 rustsrc/symbolic-unreal/tests/snapshots/test_unreal_crash_parse__contexts_runtime_properties.snap
--rw-r--r--  2.0 unx     6134 b- defN 22-Sep-28 09:00 rustsrc/symbolic-unreal/tests/test_unreal_crash_parse.rs
--rw-r--r--  2.0 unx     1876 b- defN 22-Sep-28 09:00 rustsrc/symbolic/Cargo.toml
--rw-r--r--  2.0 unx     2937 b- defN 22-Sep-28 09:00 rustsrc/symbolic/README.md
--rw-r--r--  2.0 unx     3229 b- defN 22-Sep-28 09:00 rustsrc/symbolic/src/lib.rs
-320 files, 8903943 bytes uncompressed, 2313755 bytes compressed:  74.0%
+Zip file size: 2372986 bytes, number of entries: 320
+-rw-r--r--  2.0 unx      176 b- defN 22-Sep-29 10:39 rustsrc/.clang-format
+-rw-r--r--  2.0 unx      144 b- defN 22-Sep-29 10:39 rustsrc/.codecov.yml
+-rw-r--r--  2.0 unx      593 b- defN 22-Sep-29 10:39 rustsrc/.craft.yml
+-rw-r--r--  2.0 unx      256 b- defN 22-Sep-29 10:39 rustsrc/.editorconfig
+-rw-r--r--  2.0 unx       33 b- defN 22-Sep-29 10:39 rustsrc/.github/CODEOWNERS
+-rw-r--r--  2.0 unx     2255 b- defN 22-Sep-29 10:39 rustsrc/.github/workflows/build.yml
+-rw-r--r--  2.0 unx     3922 b- defN 22-Sep-29 10:39 rustsrc/.github/workflows/ci.yml
+-rw-r--r--  2.0 unx      368 b- defN 22-Sep-29 10:39 rustsrc/.github/workflows/enforce-license-compliance.yml
+-rw-r--r--  2.0 unx      861 b- defN 22-Sep-29 10:39 rustsrc/.github/workflows/release.yml
+-rw-r--r--  2.0 unx     1004 b- defN 22-Sep-29 10:39 rustsrc/.github/workflows/weekly.yml
+-rw-r--r--  2.0 unx     3329 b- defN 22-Sep-29 10:39 rustsrc/.vscode/c_cpp_properties.json
+-rw-r--r--  2.0 unx      496 b- defN 22-Sep-29 10:39 rustsrc/.vscode/extensions.json
+-rw-r--r--  2.0 unx      695 b- defN 22-Sep-29 10:39 rustsrc/.vscode/launch.json
+-rw-r--r--  2.0 unx     1498 b- defN 22-Sep-29 10:39 rustsrc/.vscode/settings.json
+-rw-r--r--  2.0 unx     2193 b- defN 22-Sep-29 10:39 rustsrc/.vscode/tasks.json
+-rw-r--r--  2.0 unx    32435 b- defN 22-Sep-29 10:39 rustsrc/CHANGELOG.md
+-rw-r--r--  2.0 unx      149 b- defN 22-Sep-29 10:39 rustsrc/Cargo.toml
+-rw-r--r--  2.0 unx     1120 b- defN 22-Sep-29 10:39 rustsrc/LICENSE
+-rw-r--r--  2.0 unx     1987 b- defN 22-Sep-29 10:39 rustsrc/Makefile
+-rw-r--r--  2.0 unx     6228 b- defN 22-Sep-29 10:39 rustsrc/README.md
+-rw-r--r--  2.0 unx      339 b- defN 22-Sep-29 10:39 rustsrc/examples/addr2line/Cargo.toml
+-rw-r--r--  2.0 unx     6781 b- defN 22-Sep-29 10:39 rustsrc/examples/addr2line/src/main.rs
+-rw-r--r--  2.0 unx      333 b- defN 22-Sep-29 10:39 rustsrc/examples/dump_cfi/Cargo.toml
+-rw-r--r--  2.0 unx     1405 b- defN 22-Sep-29 10:39 rustsrc/examples/dump_cfi/src/main.rs
+-rw-r--r--  2.0 unx      299 b- defN 22-Sep-29 10:39 rustsrc/examples/dump_sources/Cargo.toml
+-rw-r--r--  2.0 unx     2495 b- defN 22-Sep-29 10:39 rustsrc/examples/dump_sources/src/main.rs
+-rw-r--r--  2.0 unx      569 b- defN 22-Sep-29 10:39 rustsrc/examples/minidump_stackwalk/Cargo.toml
+-rw-r--r--  2.0 unx    23996 b- defN 22-Sep-29 10:39 rustsrc/examples/minidump_stackwalk/src/main.rs
+-rw-r--r--  2.0 unx      299 b- defN 22-Sep-29 10:39 rustsrc/examples/object_debug/Cargo.toml
+-rw-r--r--  2.0 unx     2509 b- defN 22-Sep-29 10:39 rustsrc/examples/object_debug/src/main.rs
+-rw-r--r--  2.0 unx      339 b- defN 22-Sep-29 10:39 rustsrc/examples/sourcemapcache_debug/Cargo.toml
+-rw-r--r--  2.0 unx     3412 b- defN 22-Sep-29 10:39 rustsrc/examples/sourcemapcache_debug/src/main.rs
+-rw-r--r--  2.0 unx      366 b- defN 22-Sep-29 10:39 rustsrc/examples/symcache_debug/Cargo.toml
+-rw-r--r--  2.0 unx     8981 b- defN 22-Sep-29 10:39 rustsrc/examples/symcache_debug/src/main.rs
+-rw-r--r--  2.0 unx      329 b- defN 22-Sep-29 10:39 rustsrc/examples/unreal_engine_crash/Cargo.toml
+-rw-r--r--  2.0 unx     1741 b- defN 22-Sep-29 10:39 rustsrc/examples/unreal_engine_crash/src/main.rs
+-rwxr-xr-x  2.0 unx      395 b- defN 22-Sep-29 10:39 rustsrc/run
+-rwxr-xr-x  2.0 unx      536 b- defN 22-Sep-29 10:39 rustsrc/scripts/bump-version
+-rwxr-xr-x  2.0 unx    19164 b- defN 22-Sep-29 10:39 rustsrc/scripts/git-archive-all
+-rw-r--r--  2.0 unx      762 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/Cargo.toml
+-rw-r--r--  2.0 unx      750 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/Makefile
+-rw-r--r--  2.0 unx     3773 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/README.md
+-rw-r--r--  2.0 unx     1661 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/c-tests/common.c
+-rwxr-xr-x  2.0 unx     8576 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/c-tests/demangle
+-rw-r--r--  2.0 unx     1603 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/c-tests/demangle.c
+-rw-r--r--  2.0 unx     1155 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/c-tests/object.c
+-rw-r--r--  2.0 unx      343 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/cbindgen.toml
+-rw-r--r--  2.0 unx    21766 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/include/symbolic.h
+-rw-r--r--  2.0 unx     2146 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/cfi.rs
+-rw-r--r--  2.0 unx      822 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/common.rs
+-rw-r--r--  2.0 unx    11582 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/core.rs
+-rw-r--r--  2.0 unx     6771 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/debuginfo.rs
+-rw-r--r--  2.0 unx     1524 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/demangle.rs
+-rw-r--r--  2.0 unx      472 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/lib.rs
+-rw-r--r--  2.0 unx     4173 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/proguard.rs
+-rw-r--r--  2.0 unx     9538 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/sourcemap.rs
+-rw-r--r--  2.0 unx     6126 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/sourcemapcache.rs
+-rw-r--r--  2.0 unx     6456 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/symcache.rs
+-rw-r--r--  2.0 unx     3717 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cabi/src/utils.rs
+-rw-r--r--  2.0 unx      742 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/Cargo.toml
+-rw-r--r--  2.0 unx    56096 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/src/lib.rs
+-rw-r--r--  2.0 unx    59446 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_elf.snap
+-rw-r--r--  2.0 unx    21639 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_macho.snap
+-rw-r--r--  2.0 unx    15120 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_pdb_windows.snap
+-rw-r--r--  2.0 unx     3056 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_pe_windows.snap
+-rw-r--r--  2.0 unx    61807 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_sym_linux.snap
+-rw-r--r--  2.0 unx    10563 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_sym_macos.snap
+-rw-r--r--  2.0 unx    15192 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/tests/snapshots/test_cfi__cfi_sym_windows.snap
+-rw-r--r--  2.0 unx     3116 b- defN 22-Sep-29 10:39 rustsrc/symbolic-cfi/tests/test_cfi.rs
+-rw-r--r--  2.0 unx     1058 b- defN 22-Sep-29 10:39 rustsrc/symbolic-common/Cargo.toml
+-rw-r--r--  2.0 unx     1140 b- defN 22-Sep-29 10:39 rustsrc/symbolic-common/README.md
+-rw-r--r--  2.0 unx     8533 b- defN 22-Sep-29 10:39 rustsrc/symbolic-common/src/byteview.rs
+-rw-r--r--  2.0 unx    11432 b- defN 22-Sep-29 10:39 rustsrc/symbolic-common/src/cell.rs
+-rw-r--r--  2.0 unx    15395 b- defN 22-Sep-29 10:39 rustsrc/symbolic-common/src/heuristics.rs
+-rw-r--r--  2.0 unx     1150 b- defN 22-Sep-29 10:39 rustsrc/symbolic-common/src/lib.rs
+-rw-r--r--  2.0 unx    25127 b- defN 22-Sep-29 10:39 rustsrc/symbolic-common/src/path.rs
+-rw-r--r--  2.0 unx    26431 b- defN 22-Sep-29 10:39 rustsrc/symbolic-common/src/types.rs
+-rw-r--r--  2.0 unx     3160 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/Cargo.toml
+-rw-r--r--  2.0 unx     2596 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/benches/breakpad_parser.rs
+-rw-r--r--  2.0 unx      426 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/fuzz/Cargo.toml
+-rw-r--r--  2.0 unx     2746 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/fuzz/fuzz_targets/fuzz_objects.rs
+-rw-r--r--  2.0 unx    28225 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/base.rs
+-rw-r--r--  2.0 unx    82454 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/breakpad.rs
+-rw-r--r--  2.0 unx    59962 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/dwarf.rs
+-rw-r--r--  2.0 unx    37245 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/elf.rs
+-rw-r--r--  2.0 unx    15427 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/function_builder.rs
+-rw-r--r--  2.0 unx     2275 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/function_stack.rs
+-rw-r--r--  2.0 unx     2857 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/lib.rs
+-rw-r--r--  2.0 unx    16214 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/macho/bcsymbolmap.rs
+-rw-r--r--  2.0 unx   144055 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/macho/compact.rs
+-rw-r--r--  2.0 unx    34173 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/macho/mod.rs
+-rw-r--r--  2.0 unx     1971 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/macho/mono_archive.rs
+-rw-r--r--  2.0 unx    27017 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/object.rs
+-rw-r--r--  2.0 unx    36700 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/pdb.rs
+-rw-r--r--  2.0 unx    12931 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/pe.rs
+-rw-r--r--  2.0 unx    38896 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/sourcebundle.rs
+-rw-r--r--  2.0 unx     8028 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/wasm.rs
+-rw-r--r--  2.0 unx     9940 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/src/wasm/parser.rs
+-rw-r--r--  2.0 unx   414364 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/fixtures/2d10c42f-591d-3265-b147-78ba0868073f.dwarf-hidden
+-rw-r--r--  2.0 unx      273 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/fixtures/2d10c42f-591d-3265-b147-78ba0868073f.plist
+-rw-r--r--  2.0 unx   141461 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/fixtures/c8374b6d-6e96-34d8-ae38-efaa5fec424f.bcsymbolmap
+-rw-r--r--  2.0 unx      549 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/fixtures/invalid-symbols.fuzzed
+-rw-r--r--  2.0 unx     1086 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__breakpad_files.snap
+-rw-r--r--  2.0 unx    13300 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__breakpad_functions.snap
+-rw-r--r--  2.0 unx    14425 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__breakpad_functions_mac_with_inlines.snap
+-rw-r--r--  2.0 unx     1297 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__breakpad_symbols.snap
+-rw-r--r--  2.0 unx      577 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__elf_files.snap
+-rw-r--r--  2.0 unx    54908 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__elf_functions.snap
+-rw-r--r--  2.0 unx    12737 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__elf_symbols.snap
+-rw-r--r--  2.0 unx      596 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__mach_files.snap
+-rw-r--r--  2.0 unx    11222 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__mach_functions.snap
+-rw-r--r--  2.0 unx    14983 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__mach_symbols.snap
+-rw-r--r--  2.0 unx     1086 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__pdb_files.snap
+-rw-r--r--  2.0 unx    47625 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__pdb_functions.snap
+-rw-r--r--  2.0 unx     7065 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__pdb_symbols.snap
+-rw-r--r--  2.0 unx      125 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/snapshots/test_objects__wasm_symbols.snap
+-rw-r--r--  2.0 unx    16732 b- defN 22-Sep-29 10:39 rustsrc/symbolic-debuginfo/tests/test_objects.rs
+-rw-r--r--  2.0 unx     1151 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/Cargo.toml
+-rw-r--r--  2.0 unx     1027 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/README.md
+-rw-r--r--  2.0 unx      970 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/build.rs
+-rw-r--r--  2.0 unx    16380 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/src/lib.rs
+-rw-r--r--  2.0 unx     1286 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/src/swiftdemangle.cpp
+-rw-r--r--  2.0 unx    15194 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/tests/test_cpp.rs
+-rw-r--r--  2.0 unx     2289 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/tests/test_detection.rs
+-rw-r--r--  2.0 unx     1743 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/tests/test_msvc.rs
+-rw-r--r--  2.0 unx     1855 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/tests/test_objcpp.rs
+-rw-r--r--  2.0 unx    21637 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/tests/test_swift.rs
+-rw-r--r--  2.0 unx      978 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/tests/utils/mod.rs
+-rw-r--r--  2.0 unx     1807 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/1-arguments.patch
+-rw-r--r--  2.0 unx    11751 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/LICENSE.txt
+-rw-r--r--  2.0 unx     3192 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/LICENSE_LLVM.txt
+-rw-r--r--  2.0 unx     2139 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/README.md
+-rw-r--r--  2.0 unx     2956 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm-c/DataTypes.h
+-rw-r--r--  2.0 unx    26508 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/Hashing.h
+-rw-r--r--  2.0 unx      983 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/None.h
+-rw-r--r--  2.0 unx    13251 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/Optional.h
+-rw-r--r--  2.0 unx    75337 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/STLExtras.h
+-rw-r--r--  2.0 unx     2754 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/STLForwardCompat.h
+-rw-r--r--  2.0 unx    45144 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/SmallVector.h
+-rw-r--r--  2.0 unx    34006 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/StringRef.h
+-rw-r--r--  2.0 unx     6423 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/StringSwitch.h
+-rw-r--r--  2.0 unx    13081 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/iterator.h
+-rw-r--r--  2.0 unx     2252 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/ADT/iterator_range.h
+-rw-r--r--  2.0 unx     2512 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Config/abi-breaking.h
+-rw-r--r--  2.0 unx     3555 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Config/llvm-config.h
+-rw-r--r--  2.0 unx    14249 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/Casting.h
+-rw-r--r--  2.0 unx    19785 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/Compiler.h
+-rw-r--r--  2.0 unx      878 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/DataTypes.h
+-rw-r--r--  2.0 unx     6567 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/ErrorHandling.h
+-rw-r--r--  2.0 unx     3291 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/MemAlloc.h
+-rw-r--r--  2.0 unx     4942 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/SwapByteOrder.h
+-rw-r--r--  2.0 unx    25919 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/raw_ostream.h
+-rw-r--r--  2.0 unx     6912 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/llvm/Support/type_traits.h
+-rw-r--r--  2.0 unx     4918 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/AST/Ownership.h
+-rw-r--r--  2.0 unx     7601 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/AST/ReferenceStorage.def
+-rw-r--r--  2.0 unx     5362 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Basic/Compiler.h
+-rw-r--r--  2.0 unx     6983 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Basic/InlineBitfield.h
+-rw-r--r--  2.0 unx     3310 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Basic/LLVM.h
+-rw-r--r--  2.0 unx    25080 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Basic/STLExtras.h
+-rw-r--r--  2.0 unx    21991 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/Demangle.h
+-rw-r--r--  2.0 unx     9564 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/DemangleNodes.def
+-rw-r--r--  2.0 unx    21028 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/Demangler.h
+-rw-r--r--  2.0 unx     2880 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/ManglingMacros.h
+-rw-r--r--  2.0 unx    11779 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/ManglingUtils.h
+-rw-r--r--  2.0 unx     1272 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/NamespaceMacros.h
+-rw-r--r--  2.0 unx     2634 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/Punycode.h
+-rw-r--r--  2.0 unx     4145 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/StandardTypesMangling.def
+-rw-r--r--  2.0 unx     1607 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Demangling/ValueWitnessMangling.def
+-rw-r--r--  2.0 unx     1364 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Runtime/BackDeployment.h
+-rw-r--r--  2.0 unx      249 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Runtime/CMakeConfig.h
+-rw-r--r--  2.0 unx    17169 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Runtime/Config.h
+-rw-r--r--  2.0 unx     6806 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/include/swift/Strings.h
+-rw-r--r--  2.0 unx      903 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/CMakeLists.txt
+-rw-r--r--  2.0 unx     8396 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/Context.cpp
+-rw-r--r--  2.0 unx   121687 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/Demangler.cpp
+-rw-r--r--  2.0 unx     2458 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/ManglingUtils.cpp
+-rw-r--r--  2.0 unx     2330 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/NodeDumper.cpp
+-rw-r--r--  2.0 unx   104235 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/NodePrinter.cpp
+-rw-r--r--  2.0 unx    76600 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/OldDemangler.cpp
+-rw-r--r--  2.0 unx    66585 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/OldRemangler.cpp
+-rw-r--r--  2.0 unx    10799 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/Punycode.cpp
+-rw-r--r--  2.0 unx    84209 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/Remangler.cpp
+-rw-r--r--  2.0 unx     4806 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/lib/Demangling/RemanglerBase.h
+-rw-r--r--  2.0 unx     9651 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/stdlib/public/SwiftShims/Visibility.h
+-rwxr-xr-x  2.0 unx     3963 b- defN 22-Sep-29 10:39 rustsrc/symbolic-demangle/vendor/swift/update.py
+-rw-r--r--  2.0 unx      546 b- defN 22-Sep-29 10:39 rustsrc/symbolic-il2cpp/Cargo.toml
+-rw-r--r--  2.0 unx      321 b- defN 22-Sep-29 10:39 rustsrc/symbolic-il2cpp/src/lib.rs
+-rw-r--r--  2.0 unx     8773 b- defN 22-Sep-29 10:39 rustsrc/symbolic-il2cpp/src/line_mapping/from_object.rs
+-rw-r--r--  2.0 unx     4646 b- defN 22-Sep-29 10:39 rustsrc/symbolic-il2cpp/src/line_mapping/mod.rs
+-rw-r--r--  2.0 unx      715 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/Cargo.toml
+-rw-r--r--  2.0 unx      410 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/fuzz/Cargo.toml
+-rw-r--r--  2.0 unx      900 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/fuzz/fuzz_targets/fuzz_ppdb.rs
+-rw-r--r--  2.0 unx     2664 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/cache/lookup.rs
+-rw-r--r--  2.0 unx     7593 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/cache/mod.rs
+-rw-r--r--  2.0 unx     2833 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/cache/raw.rs
+-rw-r--r--  2.0 unx     3850 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/cache/writer.rs
+-rw-r--r--  2.0 unx    26510 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/format/metadata.rs
+-rw-r--r--  2.0 unx    12054 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/format/mod.rs
+-rw-r--r--  2.0 unx     2865 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/format/raw.rs
+-rw-r--r--  2.0 unx     9457 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/format/sequence_points.rs
+-rw-r--r--  2.0 unx     4116 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/format/streams.rs
+-rw-r--r--  2.0 unx     4080 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/format/utils.rs
+-rw-r--r--  2.0 unx     2859 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/src/lib.rs
+-rw-r--r--  2.0 unx      772 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/tests/fixtures/Async.pdbx
+-rw-r--r--  2.0 unx     3128 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/tests/fixtures/Documents.pdbx
+-rw-r--r--  2.0 unx     1132 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/tests/fixtures/EmbeddedSource.pdbx
+-rw-r--r--  2.0 unx     1016 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/tests/fixtures/MethodBoundaries.pdbx
+-rw-r--r--  2.0 unx     1740 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/tests/fixtures/Scopes.pdbx
+-rw-r--r--  2.0 unx      876 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/tests/fixtures/SourceLink.pdbx
+-rw-r--r--  2.0 unx    10880 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/tests/fixtures/integration.pdb
+-rw-r--r--  2.0 unx     2534 b- defN 22-Sep-29 10:39 rustsrc/symbolic-ppdb/tests/test_caches.rs
+-rw-r--r--  2.0 unx      629 b- defN 22-Sep-29 10:39 rustsrc/symbolic-sourcemapcache/Cargo.toml
+-rw-r--r--  2.0 unx      280 b- defN 22-Sep-29 10:39 rustsrc/symbolic-sourcemapcache/src/lib.rs
+-rw-r--r--  2.0 unx    11209 b- defN 22-Sep-29 10:39 rustsrc/symbolic-sourcemapcache/src/lookup.rs
+-rw-r--r--  2.0 unx     3780 b- defN 22-Sep-29 10:39 rustsrc/symbolic-sourcemapcache/src/raw.rs
+-rw-r--r--  2.0 unx    12462 b- defN 22-Sep-29 10:39 rustsrc/symbolic-sourcemapcache/src/writer.rs
+-rw-r--r--  2.0 unx    10051 b- defN 22-Sep-29 10:39 rustsrc/symbolic-sourcemapcache/tests/integration.rs
+-rw-r--r--  2.0 unx     1213 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/Cargo.toml
+-rw-r--r--  2.0 unx     1984 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/benches/bench_writer.rs
+-rw-r--r--  2.0 unx     3169 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/src/error.rs
+-rw-r--r--  2.0 unx     9621 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/src/lib.rs
+-rw-r--r--  2.0 unx     9010 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/src/lookup.rs
+-rw-r--r--  2.0 unx     4924 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/src/raw.rs
+-rw-r--r--  2.0 unx     1603 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/src/transform/bcsymbolmap.rs
+-rw-r--r--  2.0 unx     1401 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/src/transform/il2cpp.rs
+-rw-r--r--  2.0 unx     2060 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/src/transform/mod.rs
+-rw-r--r--  2.0 unx    21727 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/src/writer.rs
+-rw-r--r--  2.0 unx     4937 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/breakpad.rs
+-rw-r--r--  2.0 unx    12687 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/snapshots/test_cache__functions_linux.snap
+-rw-r--r--  2.0 unx    14934 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/snapshots/test_cache__functions_macos.snap
+-rw-r--r--  2.0 unx      754 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/snapshots/test_cache__lookup.snap
+-rw-r--r--  2.0 unx    12688 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/snapshots/test_writer__functions_linux.snap
+-rw-r--r--  2.0 unx    14935 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/snapshots/test_writer__functions_macos.snap
+-rw-r--r--  2.0 unx      262 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/snapshots/test_writer__overlapping_funcs.snap
+-rw-r--r--  2.0 unx     2396 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/test_cache.rs
+-rw-r--r--  2.0 unx     1235 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/test_transformers.rs
+-rw-r--r--  2.0 unx    12141 b- defN 22-Sep-29 10:39 rustsrc/symbolic-symcache/tests/test_writer.rs
+-rw-r--r--  2.0 unx      169 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/Cargo.toml
+-rw-r--r--  2.0 unx      168 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/libgallium_dri.sym
+-rwxr-xr-x  2.0 unx   138024 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/crash
+-rwxr-xr-x  2.0 unx  1450496 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/crash.debug
+-rw-r--r--  2.0 unx    78235 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/crash.sym
+-rw-r--r--  2.0 unx        9 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/debug_info.txt.crc
+-rwxr-xr-x  2.0 unx    16000 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with123_debuglink
+-rwxr-xr-x  2.0 unx    16000 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with12_debuglink
+-rwxr-xr-x  2.0 unx    15992 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with1_debuglink
+-rwxr-xr-x  2.0 unx    16032 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with_compressed_debuglink
+-rwxr-xr-x  2.0 unx    15992 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_with_debuglink
+-rwxr-xr-x  2.0 unx    15896 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/gen/elf_without_debuglink
+-rwxr-xr-x  2.0 unx     1736 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/linux/elf_debuglink/generate_elf_debug_link.sh
+-rw-r--r--  2.0 unx      648 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/Example.framework.dSYM/Contents/Info.plist
+-rw-r--r--  2.0 unx    19320 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/Example.framework.dSYM/Contents/Resources/DWARF/Example
+-rwxr-xr-x  2.0 unx   139580 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/crash
+-rw-r--r--  2.0 unx        0 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/crash.app.dSYM/Contents/Resources/DWARF/crash
+-rw-r--r--  2.0 unx      634 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/crash.dSYM/Contents/Info.plist
+-rw-r--r--  2.0 unx   650058 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/crash.dSYM/Contents/Resources/DWARF/crash
+-rw-r--r--  2.0 unx       57 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/crash.dSYM/Contents/Resources/DWARF/invalid
+-rw-r--r--  2.0 unx   183389 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/crash.inlines.sym
+-rw-r--r--  2.0 unx   111874 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/crash.sym
+-rw-r--r--  2.0 unx        0 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/other.dSYM/Contents/Resources/DWARF/invalid
+-rw-r--r--  2.0 unx        0 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/other.dmp.dSYM/Contents/Resources/DWARF/invalid
+-rw-r--r--  2.0 unx     9680 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/macos/overlapping_funcs.dSYM/Contents/Resources/DWARF/overlapping_funcs
+-rw-r--r--  2.0 unx   155342 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/regression/large_symbol.sym
+-rw-r--r--  2.0 unx      242 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/README.md
+-rw-r--r--  2.0 unx    64749 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/hermes-metro/react-native-hermes.map
+-rw-r--r--  2.0 unx     9168 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/hermes-metro/react-native-metro.js
+-rw-r--r--  2.0 unx    64417 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/hermes-metro/react-native-metro.js.map
+-rw-r--r--  2.0 unx      208 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/inlining/module.js
+-rw-r--r--  2.0 unx      873 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/inlining/module.js.map
+-rw-r--r--  2.0 unx      294 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/nofiles.js
+-rw-r--r--  2.0 unx      645 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/nofiles.js.map
+-rw-r--r--  2.0 unx     1022 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/old-logs/simple.chrome.log
+-rw-r--r--  2.0 unx     2172 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/old-logs/simple.firefox.log
+-rw-r--r--  2.0 unx     3161 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/old-logs/simple.node.log
+-rw-r--r--  2.0 unx     2855 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/old-logs/simple.safari.log
+-rw-r--r--  2.0 unx    16183 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/preact-missing-source-contents.module.js.map
+-rw-r--r--  2.0 unx    10031 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/preact.module.js
+-rw-r--r--  2.0 unx    68935 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/preact.module.js.map
+-rw-r--r--  2.0 unx       31 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/simple/minified.js
+-rw-r--r--  2.0 unx      318 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/simple/minified.js.map
+-rw-r--r--  2.0 unx      184 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/simple/original.js
+-rw-r--r--  2.0 unx      747 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/async.mjs
+-rw-r--r--  2.0 unx      114 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/shared.mjs
+-rw-r--r--  2.0 unx     1473 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/sync.mjs
+-rw-r--r--  2.0 unx       66 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/trace.html
+-rw-r--r--  2.0 unx      408 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/trace/trace.mjs
+-rw-r--r--  2.0 unx      300 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/webpack/bundle.js
+-rw-r--r--  2.0 unx     1716 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/sourcemapcache/webpack/bundle.js.map
+-rw-r--r--  2.0 unx   121355 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/symcache/compat/v1.symc
+-rw-r--r--  2.0 unx   222900 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/symcache/current/linux.symc
+-rw-r--r--  2.0 unx   168461 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/symcache/current/macos.symc
+-rw-r--r--  2.0 unx    42896 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/unreal/unreal_crash
+-rw-r--r--  2.0 unx    33249 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/unreal/unreal_crash_apple
+-rwxr-xr-x  2.0 unx     4293 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/wasm/simple.wasm
+-rwxr-xr-x  2.0 unx    12800 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/windows/CrashWithException.exe
+-rwxr-xr-x  2.0 unx   610304 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/windows/CrashWithException.pdb
+-rwxr-xr-x  2.0 unx    20620 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/windows/CrashWithException.pdb.sym
+-rwxr-xr-x  2.0 unx    19968 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/windows/crash.exe
+-rwxr-xr-x  2.0 unx  1019904 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/windows/crash.pdb
+-rwxr-xr-x  2.0 unx    46361 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/windows/crash.sym
+-rw-r--r--  2.0 unx      254 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/xul.sym
+-rw-r--r--  2.0 unx      422 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/fixtures/xul2.sym
+-rw-r--r--  2.0 unx      367 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/overlapping_funcs/build.sh
+-rw-r--r--  2.0 unx      101 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/overlapping_funcs/main.c
+-rw-r--r--  2.0 unx      105 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/overlapping_funcs/testachio.c
+-rw-r--r--  2.0 unx       52 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/overlapping_funcs/testachio.h
+-rw-r--r--  2.0 unx      104 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/overlapping_funcs/testaroni.c
+-rw-r--r--  2.0 unx       51 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/overlapping_funcs/testaroni.h
+-rw-r--r--  2.0 unx      768 b- defN 22-Sep-29 10:39 rustsrc/symbolic-testutils/src/lib.rs
+-rw-r--r--  2.0 unx     1248 b- defN 22-Sep-29 10:39 rustsrc/symbolic-unreal/Cargo.toml
+-rw-r--r--  2.0 unx    14050 b- defN 22-Sep-29 10:39 rustsrc/symbolic-unreal/src/container.rs
+-rw-r--r--  2.0 unx    26736 b- defN 22-Sep-29 10:39 rustsrc/symbolic-unreal/src/context.rs
+-rw-r--r--  2.0 unx     2411 b- defN 22-Sep-29 10:39 rustsrc/symbolic-unreal/src/error.rs
+-rw-r--r--  2.0 unx      195 b- defN 22-Sep-29 10:39 rustsrc/symbolic-unreal/src/lib.rs
+-rw-r--r--  2.0 unx     6078 b- defN 22-Sep-29 10:39 rustsrc/symbolic-unreal/src/logs.rs
+-rw-r--r--  2.0 unx     5302 b- defN 22-Sep-29 10:39 rustsrc/symbolic-unreal/tests/snapshots/test_unreal_crash_parse__contexts_runtime_properties.snap
+-rw-r--r--  2.0 unx     6134 b- defN 22-Sep-29 10:39 rustsrc/symbolic-unreal/tests/test_unreal_crash_parse.rs
+-rw-r--r--  2.0 unx     1876 b- defN 22-Sep-29 10:39 rustsrc/symbolic/Cargo.toml
+-rw-r--r--  2.0 unx     2937 b- defN 22-Sep-29 10:39 rustsrc/symbolic/README.md
+-rw-r--r--  2.0 unx     3229 b- defN 22-Sep-29 10:39 rustsrc/symbolic/src/lib.rs
+320 files, 8904102 bytes uncompressed, 2313800 bytes compressed:  74.0%
```

### rustsrc/CHANGELOG.md

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 9.2.1
+
+**Fixes**:
+- Fixed a bug in Unreal Engine log parsing by updating the `anylog` dependency. ([#695](https://github.com/getsentry/symbolic/pull/695))
+
 ## 9.2.0
 
 **Features**:
 
 - Added a new sub-crate for working with JavaScript SourceMaps: `symbolic-sourcemapcache`. ([#688](https://github.com/getsentry/symbolic/pull/688))
 - This new sourcemap handling is also exposed via the symbolic Python bindings.
 - The new version 8 of the symcache format saves strings slightly more compactly. Reading of version 7 is still supported. ([#670](https://github.com/getsentry/symbolic/pull/670))
```

### rustsrc/examples/addr2line/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "addr2line"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Jan Michael Auer <mail@jauer.org>"]
 edition = "2021"
 publish = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### rustsrc/examples/dump_cfi/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dump_cfi"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Jan Michael Auer <mail@jauer.org>"]
 edition = "2021"
 publish = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### rustsrc/examples/dump_sources/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "dump_sources"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Jan Michael Auer <mail@jauer.org>"]
 edition = "2021"
 publish = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### rustsrc/examples/minidump_stackwalk/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "minidump_stackwalk"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Jan Michael Auer <mail@jauer.org>"]
 edition = "2021"
 publish = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### rustsrc/examples/object_debug/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "object_debug"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Jan Michael Auer <mail@jauer.org>"]
 edition = "2021"
 publish = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### rustsrc/examples/sourcemapcache_debug/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "sourcemapcache_debug"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Sentry <hello@sentry.io>"]
 edition = "2021"
 publish = false
 
 [dependencies]
 anyhow = "1.0.32"
 clap = "3.1.0"
```

### rustsrc/examples/symcache_debug/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symcache_debug"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Jan Michael Auer <mail@jauer.org>"]
 edition = "2021"
 publish = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### rustsrc/examples/unreal_engine_crash/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "unreal_engine_crash"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Jan Michael Auer <mail@jauer.org>"]
 edition = "2021"
 publish = false
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
```

### rustsrc/symbolic-cabi/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-cabi"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Armin Ronacher <armin.ronacher@active-4.com>",
     "Jan Michael Auer <mail@jauer.org>",
 ]
 homepage = "https://github.com/getsentry/symbolic"
 repository = "https://github.com/getsentry/symbolic"
@@ -18,8 +18,8 @@
 
 [lib]
 crate-type = ["cdylib"]
 
 [dependencies]
 proguard = { version = "5.0.0", features = ["uuid"] }
 sourcemap = "6.0.2"
-symbolic = { version = "9.2.0", path = "../symbolic", features = ["cfi", "debuginfo", "demangle", "sourcemapcache", "symcache"] }
+symbolic = { version = "9.2.1", path = "../symbolic", features = ["cfi", "debuginfo", "demangle", "sourcemapcache", "symcache"] }
```

### rustsrc/symbolic-cfi/Cargo.toml

```diff
@@ -1,25 +1,25 @@
 [package]
 name = "symbolic-cfi"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Armin Ronacher <armin.ronacher@active-4.com>",
     "Jan Michael Auer <mail@jauer.org>",
 ]
 documentation = "https://docs.rs/symbolic-cfi"
 homepage = "https://github.com/getsentry/symbolic"
 repository = "https://github.com/getsentry/symbolic"
 description = """
 A library to process call frame information
 """
 edition = "2021"
 
 [dependencies]
-symbolic-common = { version = "9.2.0", path = "../symbolic-common" }
-symbolic-debuginfo = { version = "9.2.0", path = "../symbolic-debuginfo" }
+symbolic-common = { version = "9.2.1", path = "../symbolic-common" }
+symbolic-debuginfo = { version = "9.2.1", path = "../symbolic-debuginfo" }
 thiserror = "1.0.20"
 
 [dev-dependencies]
 insta = { version = "1.18.0", features = ["yaml"] }
 symbolic-testutils = { path = "../symbolic-testutils" }
 similar-asserts = "1.0.0"
```

### rustsrc/symbolic-common/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-common"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Armin Ronacher <armin.ronacher@active-4.com>",
     "Jan Michael Auer <mail@jauer.org>",
 ]
 documentation = "https://docs.rs/symbolic-common"
 homepage = "https://github.com/getsentry/symbolic"
```

### rustsrc/symbolic-debuginfo/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-debuginfo"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Armin Ronacher <armin.ronacher@active-4.com>",
     "Jan Michael Auer <mail@jauer.org>",
 ]
 documentation = "https://docs.rs/symbolic-debuginfo"
 homepage = "https://github.com/getsentry/symbolic"
@@ -92,15 +92,15 @@
 pdb-addr2line = { version = "0.10.2", optional = true }
 regex = { version = "1.3.5", optional = true }
 # keep this in sync with whatever version `goblin` uses
 scroll = { version = "0.11", optional = true }
 serde = { version = "1.0.94", features = ["derive"] }
 serde_json = { version = "1.0.40", optional = true }
 smallvec = { version = "1.2.0", optional = true }
-symbolic-common = { version = "9.2.0", path = "../symbolic-common" }
+symbolic-common = { version = "9.2.1", path = "../symbolic-common" }
 thiserror = "1.0.20"
 wasmparser = { version = "0.90.0", optional = true }
 zip = { version = "0.6.2", optional = true, default-features = false, features = [
     "deflate",
 ] }
 
 [dev-dependencies]
```

### rustsrc/symbolic-debuginfo/fuzz/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-debuginfo-fuzz"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Automatically generated"]
 publish = false
 edition = "2021"
 
 [package.metadata]
 cargo-fuzz = true
```

### rustsrc/symbolic-demangle/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-demangle"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Armin Ronacher <armin.ronacher@active-4.com>",
     "Jan Michael Auer <mail@jauer.org>",
 ]
 documentation = "https://docs.rs/symbolic-demangle"
 homepage = "https://github.com/getsentry/symbolic"
@@ -30,15 +30,15 @@
 rust = ["rustc-demangle"]
 swift = ["cc"]
 
 [dependencies]
 cpp_demangle = { version = "0.3.2", optional = true }
 msvc-demangler = { version = "0.9.0", optional = true }
 rustc-demangle = { version = "0.1.16", optional = true }
-symbolic-common = { version = "9.2.0", path = "../symbolic-common" }
+symbolic-common = { version = "9.2.1", path = "../symbolic-common" }
 
 [build-dependencies]
 cc = { version = "1.0.50", optional = true }
 
 [badges]
 travis-ci = { repository = "getsentry/symbolic", branch = "master" }
```

### rustsrc/symbolic-il2cpp/Cargo.toml

```diff
@@ -1,18 +1,18 @@
 [package]
 name = "symbolic-il2cpp"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = ["Sentry <hello@sentry.io>"]
 documentation = "https://docs.rs/symbolic-il2cpp"
 homepage = "https://github.com/getsentry/symbolic"
 repository = "https://github.com/getsentry/symbolic"
 description = """
 A library for parsing il2cpp line mappings.
 """
 edition = "2021"
 
 [dependencies]
 indexmap = "1.8.0"
 serde_json = "1.0.79"
-symbolic-common = { version = "9.2.0", path = "../symbolic-common" }
-symbolic-debuginfo = { version = "9.2.0", path = "../symbolic-debuginfo" }
+symbolic-common = { version = "9.2.1", path = "../symbolic-common" }
+symbolic-debuginfo = { version = "9.2.1", path = "../symbolic-debuginfo" }
```

### rustsrc/symbolic-ppdb/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-ppdb"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Sebastian Zivota <sebastian.zivota@sentry.io>",
     "Arpad Borsos <arpad.borsos@sentry.io>"
 ]
 documentation = "https://docs.rs/symbolic-ppdb"
 homepage = "https://github.com/getsentry/symbolic"
@@ -17,11 +17,11 @@
 exclude = ["tests/**/*"]
 
 [package.metadata.docs.rs]
 all-features = true
 
 [dependencies]
 indexmap = "1.9.1"
-symbolic-common = { version = "9.2.0", path = "../symbolic-common" }
+symbolic-common = { version = "9.2.1", path = "../symbolic-common" }
 watto = { version = "0.1.0", features = ["writer", "strings"] }
 thiserror = "1.0.31"
 uuid = "1.0.0"
```

### rustsrc/symbolic-ppdb/fuzz/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-ppdb-fuzz"
-version = "9.2.0"
+version = "9.2.1"
 authors = ["Automatically generated"]
 publish = false
 edition = "2021"
 
 [package.metadata]
 cargo-fuzz = true
```

### rustsrc/symbolic-sourcemapcache/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-sourcemapcache"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = ["Sentry <hello@sentry.io>"]
 documentation = "https://docs.rs/symbolic-sourcemapcache"
 homepage = "https://github.com/getsentry/symbolic"
 repository = "https://github.com/getsentry/symbolic"
 description = """
 A fast lookup cache for JavaScript Source Maps.
```

### rustsrc/symbolic-symcache/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-symcache"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Armin Ronacher <armin.ronacher@active-4.com>",
     "Jan Michael Auer <mail@jauer.org>",
 ]
 documentation = "https://docs.rs/symbolic-symcache"
 homepage = "https://github.com/getsentry/symbolic"
@@ -19,17 +19,17 @@
     "tests/**/*",
 ]
 
 [package.metadata.docs.rs]
 all-features = true
 
 [dependencies]
-symbolic-common = { version = "9.2.0", path = "../symbolic-common" }
-symbolic-debuginfo = { version = "9.2.0", path = "../symbolic-debuginfo" }
-symbolic-il2cpp = { version = "9.2.0", path = "../symbolic-il2cpp", optional = true }
+symbolic-common = { version = "9.2.1", path = "../symbolic-common" }
+symbolic-debuginfo = { version = "9.2.1", path = "../symbolic-debuginfo" }
+symbolic-il2cpp = { version = "9.2.1", path = "../symbolic-il2cpp", optional = true }
 thiserror = "1.0.20"
 indexmap = "1.7.0"
 tracing = "0.1.35"
 watto = { version = "0.1.0", features = ["writer", "strings"] }
 
 [dev-dependencies]
 insta = { version = "1.18.0", features = ["yaml"] }
```

### rustsrc/symbolic-testutils/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-testutils"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 edition = "2021"
 publish = false
 
 [package.metadata.docs.rs]
 all-features = true
```

### rustsrc/symbolic-unreal/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic-unreal"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Armin Ronacher <armin.ronacher@active-4.com>",
     "Jan Michael Auer <mail@jauer.org>",
     "Bruno Garcia <bruno@brunogarcia.com>",
 ]
 documentation = "https://docs.rs/symbolic-unreal"
@@ -22,15 +22,15 @@
 [package.metadata.docs.rs]
 all-features = true
 
 [features]
 serde = ["serde_", "chrono/serde"]
 
 [dependencies]
-anylog = "0.6.1"
+anylog = "0.6.2"
 bytes = "1.1.0"
 # this is still used for compatibility with `anylog`
 chrono = "0.4.7"
 elementtree = "1.2.2"
 flate2 = { version = "1.0.13", features = ["rust_backend"], default-features = false }
 lazy_static = "1.4.0"
 regex = "1.3.5"
```

### rustsrc/symbolic/Cargo.toml

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "symbolic"
-version = "9.2.0"
+version = "9.2.1"
 license = "MIT"
 authors = [
     "Armin Ronacher <armin.ronacher@active-4.com>",
     "Jan Michael Auer <mail@jauer.org>",
 ]
 documentation = "https://docs.rs/symbolic"
 homepage = "https://github.com/getsentry/symbolic"
@@ -30,16 +30,16 @@
 ppdb = ["symbolic-ppdb"]
 sourcemapcache = ["symbolic-sourcemapcache"]
 symcache = ["symbolic-symcache", "debuginfo"]
 unreal = ["symbolic-unreal"]
 unreal-serde = ["unreal", "common-serde", "symbolic-unreal/serde"]
 
 [dependencies]
-symbolic-cfi = { version = "9.2.0", path = "../symbolic-cfi", optional = true }
-symbolic-common = { version = "9.2.0", path = "../symbolic-common" }
-symbolic-debuginfo = { version = "9.2.0", path = "../symbolic-debuginfo", optional = true }
-symbolic-demangle = { version = "9.2.0", path = "../symbolic-demangle", optional = true }
-symbolic-il2cpp = { version = "9.2.0", path = "../symbolic-il2cpp", optional = true }
-symbolic-ppdb = { version = "9.2.0", path = "../symbolic-ppdb", optional = true }
-symbolic-sourcemapcache = { version = "9.2.0", path = "../symbolic-sourcemapcache", optional = true }
-symbolic-symcache = { version = "9.2.0", path = "../symbolic-symcache", optional = true }
-symbolic-unreal = { version = "9.2.0", path = "../symbolic-unreal", optional = true }
+symbolic-cfi = { version = "9.2.1", path = "../symbolic-cfi", optional = true }
+symbolic-common = { version = "9.2.1", path = "../symbolic-common" }
+symbolic-debuginfo = { version = "9.2.1", path = "../symbolic-debuginfo", optional = true }
+symbolic-demangle = { version = "9.2.1", path = "../symbolic-demangle", optional = true }
+symbolic-il2cpp = { version = "9.2.1", path = "../symbolic-il2cpp", optional = true }
+symbolic-ppdb = { version = "9.2.1", path = "../symbolic-ppdb", optional = true }
+symbolic-sourcemapcache = { version = "9.2.1", path = "../symbolic-sourcemapcache", optional = true }
+symbolic-symcache = { version = "9.2.1", path = "../symbolic-symcache", optional = true }
+symbolic-unreal = { version = "9.2.1", path = "../symbolic-unreal", optional = true }
```

## Comparing `symbolic-9.2.0/setup.py` & `symbolic-9.2.1/setup.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/sourcemapcache.py` & `symbolic-9.2.1/symbolic/sourcemapcache.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/sourcemap.py` & `symbolic-9.2.1/symbolic/sourcemap.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/_compat.py` & `symbolic-9.2.1/symbolic/_compat.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/utils.py` & `symbolic-9.2.1/symbolic/utils.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/proguard.py` & `symbolic-9.2.1/symbolic/proguard.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/common.py` & `symbolic-9.2.1/symbolic/common.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/debuginfo.py` & `symbolic-9.2.1/symbolic/debuginfo.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/symcache.py` & `symbolic-9.2.1/symbolic/symcache.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/__init__.py` & `symbolic-9.2.1/symbolic/__init__.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/exceptions.py` & `symbolic-9.2.1/symbolic/exceptions.py`

 * *Files identical despite different names*

## Comparing `symbolic-9.2.0/symbolic/cfi.py` & `symbolic-9.2.1/symbolic/cfi.py`

 * *Files identical despite different names*

