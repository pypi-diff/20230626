# Comparing `tmp/cpdb-protein-0.1.0.tar.gz` & `tmp/cpdb-protein-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpdb-protein-0.1.0.tar", last modified: Tue Jun 13 20:31:22 2023, max compression
+gzip compressed data, was "cpdb-protein-0.2.0.tar", last modified: Mon Jun 26 17:00:18 2023, max compression
```

## Comparing `cpdb-protein-0.1.0.tar` & `cpdb-protein-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 jamasba    (501) staff       (20)        0 2023-06-13 20:31:22.935613 cpdb-protein-0.1.0/
--rw-rw-r--   0 jamasba    (501) staff       (20)     1069 2023-06-13 13:11:32.000000 cpdb-protein-0.1.0/LICENSE
--rw-rw-r--   0 jamasba    (501) staff       (20)       37 2023-06-13 20:26:30.000000 cpdb-protein-0.1.0/MANIFEST.in
--rw-r--r--   0 jamasba    (501) staff       (20)      183 2023-06-13 20:31:22.935433 cpdb-protein-0.1.0/PKG-INFO
--rw-r--r--   0 jamasba    (501) staff       (20)     3740 2023-06-13 15:09:49.000000 cpdb-protein-0.1.0/README.md
-drwxr-xr-x   0 jamasba    (501) staff       (20)        0 2023-06-13 20:31:22.933829 cpdb-protein-0.1.0/cpdb/
--rw-rw-r--   0 jamasba    (501) staff       (20)      255 2023-06-13 14:50:01.000000 cpdb-protein-0.1.0/cpdb/__init__.py
--rw-r--r--   0 jamasba    (501) staff       (20)   369822 2023-06-13 20:26:01.000000 cpdb-protein-0.1.0/cpdb/parser.c
--rw-r--r--   0 jamasba    (501) staff       (20)     6343 2023-06-13 15:09:49.000000 cpdb-protein-0.1.0/cpdb/parser.pyx
-drwxr-xr-x   0 jamasba    (501) staff       (20)        0 2023-06-13 20:31:22.934737 cpdb-protein-0.1.0/cpdb_protein.egg-info/
--rw-r--r--   0 jamasba    (501) staff       (20)      183 2023-06-13 20:31:22.000000 cpdb-protein-0.1.0/cpdb_protein.egg-info/PKG-INFO
--rw-r--r--   0 jamasba    (501) staff       (20)      302 2023-06-13 20:31:22.000000 cpdb-protein-0.1.0/cpdb_protein.egg-info/SOURCES.txt
--rw-r--r--   0 jamasba    (501) staff       (20)        1 2023-06-13 20:31:22.000000 cpdb-protein-0.1.0/cpdb_protein.egg-info/dependency_links.txt
--rw-r--r--   0 jamasba    (501) staff       (20)       13 2023-06-13 20:31:22.000000 cpdb-protein-0.1.0/cpdb_protein.egg-info/requires.txt
--rw-r--r--   0 jamasba    (501) staff       (20)        5 2023-06-13 20:31:22.000000 cpdb-protein-0.1.0/cpdb_protein.egg-info/top_level.txt
--rw-r--r--   0 jamasba    (501) staff       (20)       38 2023-06-13 20:31:22.935668 cpdb-protein-0.1.0/setup.cfg
--rw-r--r--   0 jamasba    (501) staff       (20)      512 2023-06-13 20:31:00.000000 cpdb-protein-0.1.0/setup.py
-drwxr-xr-x   0 jamasba    (501) staff       (20)        0 2023-06-13 20:31:22.934894 cpdb-protein-0.1.0/tests/
--rw-r--r--   0 jamasba    (501) staff       (20)     1620 2023-06-13 15:09:49.000000 cpdb-protein-0.1.0/tests/test_similarity_to_biopandas.py
+drwxr-xr-x   0 jamasba    (501) staff       (20)        0 2023-06-26 17:00:18.543398 cpdb-protein-0.2.0/
+-rw-rw-r--   0 jamasba    (501) staff       (20)     1069 2023-06-13 13:11:32.000000 cpdb-protein-0.2.0/LICENSE
+-rw-rw-r--   0 jamasba    (501) staff       (20)       37 2023-06-13 20:26:30.000000 cpdb-protein-0.2.0/MANIFEST.in
+-rw-r--r--   0 jamasba    (501) staff       (20)      183 2023-06-26 17:00:18.543221 cpdb-protein-0.2.0/PKG-INFO
+-rw-r--r--   0 jamasba    (501) staff       (20)     4731 2023-06-26 15:25:54.000000 cpdb-protein-0.2.0/README.md
+drwxr-xr-x   0 jamasba    (501) staff       (20)        0 2023-06-26 17:00:18.541764 cpdb-protein-0.2.0/cpdb/
+-rw-rw-r--   0 jamasba    (501) staff       (20)     2351 2023-06-26 15:25:27.000000 cpdb-protein-0.2.0/cpdb/__init__.py
+-rw-r--r--   0 jamasba    (501) staff       (20)   488463 2023-06-26 17:00:18.000000 cpdb-protein-0.2.0/cpdb/parser.c
+-rw-r--r--   0 jamasba    (501) staff       (20)    11943 2023-06-26 14:53:15.000000 cpdb-protein-0.2.0/cpdb/parser.pyx
+drwxr-xr-x   0 jamasba    (501) staff       (20)        0 2023-06-26 17:00:18.542591 cpdb-protein-0.2.0/cpdb_protein.egg-info/
+-rw-r--r--   0 jamasba    (501) staff       (20)      183 2023-06-26 17:00:18.000000 cpdb-protein-0.2.0/cpdb_protein.egg-info/PKG-INFO
+-rw-r--r--   0 jamasba    (501) staff       (20)      317 2023-06-26 17:00:18.000000 cpdb-protein-0.2.0/cpdb_protein.egg-info/SOURCES.txt
+-rw-r--r--   0 jamasba    (501) staff       (20)        1 2023-06-26 17:00:18.000000 cpdb-protein-0.2.0/cpdb_protein.egg-info/dependency_links.txt
+-rw-r--r--   0 jamasba    (501) staff       (20)       20 2023-06-26 17:00:18.000000 cpdb-protein-0.2.0/cpdb_protein.egg-info/requires.txt
+-rw-r--r--   0 jamasba    (501) staff       (20)        5 2023-06-26 17:00:18.000000 cpdb-protein-0.2.0/cpdb_protein.egg-info/top_level.txt
+-rw-r--r--   0 jamasba    (501) staff       (20)       82 2023-06-26 16:02:53.000000 cpdb-protein-0.2.0/pyproject.toml
+-rw-r--r--   0 jamasba    (501) staff       (20)       38 2023-06-26 17:00:18.543466 cpdb-protein-0.2.0/setup.cfg
+-rw-r--r--   0 jamasba    (501) staff       (20)      562 2023-06-26 16:00:26.000000 cpdb-protein-0.2.0/setup.py
+drwxr-xr-x   0 jamasba    (501) staff       (20)        0 2023-06-26 17:00:18.542853 cpdb-protein-0.2.0/tests/
+-rw-r--r--   0 jamasba    (501) staff       (20)     1612 2023-06-26 16:10:15.000000 cpdb-protein-0.2.0/tests/test_similarity_to_biopandas.py
```

### Comparing `cpdb-protein-0.1.0/LICENSE` & `cpdb-protein-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpdb-protein-0.1.0/cpdb/parser.c` & `cpdb-protein-0.2.0/cpdb/parser.c`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "cpdb.parser",
         "sources": [
-            "cpdb_protein/cpdb/parser.pyx"
+            "cpdb/parser.pyx"
         ]
     },
     "module_name": "cpdb.parser"
 }
 END: Cython Metadata */
 
 #ifndef PY_SSIZE_T_CLEAN
@@ -764,16 +764,16 @@
 #include "numpy/ndarrayobject.h"
 #include "numpy/ndarraytypes.h"
 #include "numpy/arrayscalars.h"
 #include "numpy/ufuncobject.h"
 
     /* NumPy API declarations from "numpy/__init__.pxd" */
     
-#include <stdlib.h>
 #include <stdint.h>
+#include <stdlib.h>
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
@@ -997,15 +997,15 @@
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
 
 static const char *__pyx_f[] = {
-  "cpdb_protein/cpdb/parser.pyx",
+  "cpdb/parser.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 /* BufferFormatStructs.proto */
 #define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
@@ -1038,195 +1038,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1253,52 +1235,52 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 struct __pyx_t_4cpdb_6parser_AtomData;
 
-/* "cpdb/parser.pyx":11
+/* "cpdb/parser.pyx":12
  * 
  * 
  * cdef struct AtomData:             # <<<<<<<<<<<<<<
  *     char[7] record_type
  *     int atom_serial
  */
 struct __pyx_t_4cpdb_6parser_AtomData {
@@ -1602,14 +1584,25 @@
 
 /* decode_c_string.proto */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1880,18 +1873,18 @@
 static PyTypeObject *__pyx_ptype_5numpy_inexact = 0;
 static PyTypeObject *__pyx_ptype_5numpy_floating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_complexfloating = 0;
 static PyTypeObject *__pyx_ptype_5numpy_flexible = 0;
 static PyTypeObject *__pyx_ptype_5numpy_character = 0;
 static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
 
-/* Module declarations from 'libc.stdlib' */
-
 /* Module declarations from 'libc.stdint' */
 
+/* Module declarations from 'libc.stdlib' */
+
 /* Module declarations from 'cpdb.parser' */
 static __Pyx_TypeInfo __Pyx_TypeInfo_float = { "float", NULL, sizeof(float), { 0 }, 0, 'R', 0, 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_int = { "int", NULL, sizeof(int), { 0 }, 0, IS_UNSIGNED(int) ? 'U' : 'I', IS_UNSIGNED(int), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_object = { "Python object", NULL, sizeof(PyObject *), { 0 }, 0, 'O', 0, 0 };
 #define __Pyx_MODULE_NAME "cpdb.parser"
 extern int __pyx_module_is_main_cpdb__parser;
 int __pyx_module_is_main_cpdb__parser = 0;
@@ -1908,14 +1901,15 @@
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_ascii[] = "ascii";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_int32[] = "int32";
+static const char __pyx_k_lines[] = "lines";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_strip[] = "strip";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_ENDMDL[] = "ENDMDL";
 static const char __pyx_k_HETATM[] = "HETATM";
 static const char __pyx_k_charge[] = "charge";
@@ -1932,37 +1926,41 @@
 static const char __pyx_k_replace[] = "replace";
 static const char __pyx_k_x_coord[] = "x_coord";
 static const char __pyx_k_y_coord[] = "y_coord";
 static const char __pyx_k_z_coord[] = "z_coord";
 static const char __pyx_k_b_factor[] = "b_factor";
 static const char __pyx_k_chain_id[] = "chain_id";
 static const char __pyx_k_filename[] = "filename";
+static const char __pyx_k_py_bytes[] = "py_bytes";
 static const char __pyx_k_x_coords[] = "x_coords";
 static const char __pyx_k_y_coords[] = "y_coords";
 static const char __pyx_k_z_coords[] = "z_coords";
 static const char __pyx_k_atom_data[] = "atom_data";
 static const char __pyx_k_atom_name[] = "atom_name";
 static const char __pyx_k_b_factors[] = "b_factors";
+static const char __pyx_k_input_str[] = "input_str";
 static const char __pyx_k_insertion[] = "insertion";
 static const char __pyx_k_max_atoms[] = "max_atoms";
 static const char __pyx_k_model_idx[] = "model_idx";
 static const char __pyx_k_occupancy[] = "occupancy";
-static const char __pyx_k_parse_pdb[] = "parse_pdb";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_atom_number[] = "atom_number";
 static const char __pyx_k_cpdb_parser[] = "cpdb.parser";
 static const char __pyx_k_occupancies[] = "occupancies";
+static const char __pyx_k_python_line[] = "python_line";
 static const char __pyx_k_record_name[] = "record_name";
 static const char __pyx_k_residue_name[] = "residue_name";
 static const char __pyx_k_element_symbol[] = "element_symbol";
+static const char __pyx_k_parse_pdb_file[] = "parse_pdb_file";
 static const char __pyx_k_residue_number[] = "residue_number";
+static const char __pyx_k_cpdb_parser_pyx[] = "cpdb/parser.pyx";
+static const char __pyx_k_parse_pdb_string[] = "parse_pdb_string";
 static const char __pyx_k_FileNotFoundError[] = "FileNotFoundError";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Could_not_open_file[] = "Could not open file";
-static const char __pyx_k_cpdb_protein_cpdb_parser_pyx[] = "cpdb_protein/cpdb/parser.pyx";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static PyObject *__pyx_n_b_ATOM;
 static PyObject *__pyx_kp_u_Could_not_open_file;
 static PyObject *__pyx_n_b_ENDMDL;
 static PyObject *__pyx_n_s_FileNotFoundError;
 static PyObject *__pyx_n_b_HETATM;
@@ -1979,46 +1977,51 @@
 static PyObject *__pyx_n_s_b_factors;
 static PyObject *__pyx_n_s_chain_id;
 static PyObject *__pyx_n_u_chain_id;
 static PyObject *__pyx_n_s_charge;
 static PyObject *__pyx_n_u_charge;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_cpdb_parser;
-static PyObject *__pyx_kp_s_cpdb_protein_cpdb_parser_pyx;
+static PyObject *__pyx_kp_s_cpdb_parser_pyx;
 static PyObject *__pyx_n_s_decode;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_element_symbol;
 static PyObject *__pyx_n_u_element_symbol;
 static PyObject *__pyx_n_s_empty;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_errors;
 static PyObject *__pyx_n_s_filename;
 static PyObject *__pyx_n_s_float32;
 static PyObject *__pyx_n_s_fp;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
+static PyObject *__pyx_n_s_input_str;
 static PyObject *__pyx_n_s_insertion;
 static PyObject *__pyx_n_u_insertion;
 static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_s_line;
+static PyObject *__pyx_n_s_lines;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_max_atoms;
 static PyObject *__pyx_n_s_model_idx;
 static PyObject *__pyx_n_u_model_idx;
 static PyObject *__pyx_n_s_n_atoms;
 static PyObject *__pyx_n_s_n_model;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_object;
 static PyObject *__pyx_n_s_occupancies;
 static PyObject *__pyx_n_u_occupancy;
-static PyObject *__pyx_n_s_parse_pdb;
+static PyObject *__pyx_n_s_parse_pdb_file;
+static PyObject *__pyx_n_s_parse_pdb_string;
+static PyObject *__pyx_n_s_py_bytes;
+static PyObject *__pyx_n_s_python_line;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_record_name;
 static PyObject *__pyx_n_u_record_name;
 static PyObject *__pyx_n_u_replace;
 static PyObject *__pyx_n_s_residue_name;
 static PyObject *__pyx_n_u_residue_name;
 static PyObject *__pyx_n_s_residue_number;
@@ -2029,44 +2032,47 @@
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_u_x_coord;
 static PyObject *__pyx_n_s_x_coords;
 static PyObject *__pyx_n_u_y_coord;
 static PyObject *__pyx_n_s_y_coords;
 static PyObject *__pyx_n_u_z_coord;
 static PyObject *__pyx_n_s_z_coords;
-static PyObject *__pyx_pf_4cpdb_6parser_parse_pdb(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, int __pyx_v_max_atoms); /* proto */
+static PyObject *__pyx_pf_4cpdb_6parser_parse_pdb_file(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, int __pyx_v_max_atoms); /* proto */
+static PyObject *__pyx_pf_4cpdb_6parser_2parse_pdb_string(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_str, int __pyx_v_max_atoms); /* proto */
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
+static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_codeobj__7;
+static PyObject *__pyx_codeobj__9;
 /* Late includes */
 
-/* "cpdb/parser.pyx":33
+/* "cpdb/parser.pyx":34
  * @cython.wraparound(False)
  * @cython.nonecheck(False)
- * def parse_pdb(filename, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
+ * def parse_pdb_file(filename, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
  *     cdef FILE *fp = NULL
  *     cdef char *line = NULL
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4cpdb_6parser_1parse_pdb(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_4cpdb_6parser_1parse_pdb = {"parse_pdb", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4cpdb_6parser_1parse_pdb, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_4cpdb_6parser_1parse_pdb(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_4cpdb_6parser_1parse_pdb_file(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_4cpdb_6parser_1parse_pdb_file = {"parse_pdb_file", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4cpdb_6parser_1parse_pdb_file, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4cpdb_6parser_1parse_pdb_file(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_filename = 0;
   int __pyx_v_max_atoms;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("parse_pdb (wrapper)", 0);
+  __Pyx_RefNannySetupContext("parse_pdb_file (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_filename,&__pyx_n_s_max_atoms,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
@@ -2086,48 +2092,48 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_atoms);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse_pdb") < 0)) __PYX_ERR(0, 33, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse_pdb_file") < 0)) __PYX_ERR(0, 34, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_filename = values[0];
     if (values[1]) {
-      __pyx_v_max_atoms = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_max_atoms == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 33, __pyx_L3_error)
+      __pyx_v_max_atoms = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_max_atoms == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
     } else {
       __pyx_v_max_atoms = ((int)0xF4240);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("parse_pdb", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 33, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("parse_pdb_file", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 34, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("cpdb.parser.parse_pdb", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("cpdb.parser.parse_pdb_file", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4cpdb_6parser_parse_pdb(__pyx_self, __pyx_v_filename, __pyx_v_max_atoms);
+  __pyx_r = __pyx_pf_4cpdb_6parser_parse_pdb_file(__pyx_self, __pyx_v_filename, __pyx_v_max_atoms);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4cpdb_6parser_parse_pdb(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, int __pyx_v_max_atoms) {
+static PyObject *__pyx_pf_4cpdb_6parser_parse_pdb_file(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_filename, int __pyx_v_max_atoms) {
   FILE *__pyx_v_fp;
   char *__pyx_v_line;
   int __pyx_v_n_atoms;
   int __pyx_v_i;
   int __pyx_v_n_model;
   struct __pyx_t_4cpdb_6parser_AtomData *__pyx_v_atom_data;
   PyArrayObject *__pyx_v_x_coords = 0;
@@ -2215,15 +2221,15 @@
   float __pyx_t_32;
   Py_ssize_t __pyx_t_33;
   int __pyx_t_34;
   PyObject **__pyx_t_35;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("parse_pdb", 0);
+  __Pyx_RefNannySetupContext("parse_pdb_file", 0);
   __pyx_pybuffer_x_coords.pybuffer.buf = NULL;
   __pyx_pybuffer_x_coords.refcount = 0;
   __pyx_pybuffernd_x_coords.data = NULL;
   __pyx_pybuffernd_x_coords.rcbuffer = &__pyx_pybuffer_x_coords;
   __pyx_pybuffer_y_coords.pybuffer.buf = NULL;
   __pyx_pybuffer_y_coords.refcount = 0;
   __pyx_pybuffernd_y_coords.data = NULL;
@@ -2281,1846 +2287,1848 @@
   __pyx_pybuffernd_element_symbol.data = NULL;
   __pyx_pybuffernd_element_symbol.rcbuffer = &__pyx_pybuffer_element_symbol;
   __pyx_pybuffer_charge.pybuffer.buf = NULL;
   __pyx_pybuffer_charge.refcount = 0;
   __pyx_pybuffernd_charge.data = NULL;
   __pyx_pybuffernd_charge.rcbuffer = &__pyx_pybuffer_charge;
 
-  /* "cpdb/parser.pyx":34
+  /* "cpdb/parser.pyx":35
  * @cython.nonecheck(False)
- * def parse_pdb(filename, int max_atoms=1000000) -> object:
+ * def parse_pdb_file(filename, int max_atoms=1000000) -> object:
  *     cdef FILE *fp = NULL             # <<<<<<<<<<<<<<
  *     cdef char *line = NULL
  *     cdef int n_atoms = 0
  */
   __pyx_v_fp = NULL;
 
-  /* "cpdb/parser.pyx":35
- * def parse_pdb(filename, int max_atoms=1000000) -> object:
+  /* "cpdb/parser.pyx":36
+ * def parse_pdb_file(filename, int max_atoms=1000000) -> object:
  *     cdef FILE *fp = NULL
  *     cdef char *line = NULL             # <<<<<<<<<<<<<<
  *     cdef int n_atoms = 0
  *     cdef int i = 0
  */
   __pyx_v_line = NULL;
 
-  /* "cpdb/parser.pyx":36
+  /* "cpdb/parser.pyx":37
  *     cdef FILE *fp = NULL
  *     cdef char *line = NULL
  *     cdef int n_atoms = 0             # <<<<<<<<<<<<<<
  *     cdef int i = 0
  *     cdef int n_model =1
  */
   __pyx_v_n_atoms = 0;
 
-  /* "cpdb/parser.pyx":37
+  /* "cpdb/parser.pyx":38
  *     cdef char *line = NULL
  *     cdef int n_atoms = 0
  *     cdef int i = 0             # <<<<<<<<<<<<<<
  *     cdef int n_model =1
  * 
  */
   __pyx_v_i = 0;
 
-  /* "cpdb/parser.pyx":38
+  /* "cpdb/parser.pyx":39
  *     cdef int n_atoms = 0
  *     cdef int i = 0
  *     cdef int n_model =1             # <<<<<<<<<<<<<<
  * 
  *     cdef AtomData *atom_data = <AtomData *> malloc(max_atoms * cython.sizeof(AtomData))
  */
   __pyx_v_n_model = 1;
 
-  /* "cpdb/parser.pyx":40
+  /* "cpdb/parser.pyx":41
  *     cdef int n_model =1
  * 
  *     cdef AtomData *atom_data = <AtomData *> malloc(max_atoms * cython.sizeof(AtomData))             # <<<<<<<<<<<<<<
  * 
  *     line = <char *> malloc(82 * cython.sizeof(char))  # 82 chars to include newline and null terminator
  */
   __pyx_v_atom_data = ((struct __pyx_t_4cpdb_6parser_AtomData *)malloc((__pyx_v_max_atoms * (sizeof(struct __pyx_t_4cpdb_6parser_AtomData)))));
 
-  /* "cpdb/parser.pyx":42
+  /* "cpdb/parser.pyx":43
  *     cdef AtomData *atom_data = <AtomData *> malloc(max_atoms * cython.sizeof(AtomData))
  * 
  *     line = <char *> malloc(82 * cython.sizeof(char))  # 82 chars to include newline and null terminator             # <<<<<<<<<<<<<<
  *     fp = fopen(filename.encode('utf-8'), "r, ccs=UTF-8")
  *     if fp == NULL:
  */
   __pyx_v_line = ((char *)malloc((82 * (sizeof(char)))));
 
-  /* "cpdb/parser.pyx":43
+  /* "cpdb/parser.pyx":44
  * 
  *     line = <char *> malloc(82 * cython.sizeof(char))  # 82 chars to include newline and null terminator
  *     fp = fopen(filename.encode('utf-8'), "r, ccs=UTF-8")             # <<<<<<<<<<<<<<
  *     if fp == NULL:
  *         raise FileNotFoundError("Could not open file")
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_filename, __pyx_n_s_encode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_utf_8);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_AsString(__pyx_t_1); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(0, 44, __pyx_L1_error)
   __pyx_v_fp = fopen(__pyx_t_4, ((char const *)"r, ccs=UTF-8"));
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpdb/parser.pyx":44
+  /* "cpdb/parser.pyx":45
  *     line = <char *> malloc(82 * cython.sizeof(char))  # 82 chars to include newline and null terminator
  *     fp = fopen(filename.encode('utf-8'), "r, ccs=UTF-8")
  *     if fp == NULL:             # <<<<<<<<<<<<<<
  *         raise FileNotFoundError("Could not open file")
  * 
  */
   __pyx_t_5 = ((__pyx_v_fp == NULL) != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "cpdb/parser.pyx":45
+    /* "cpdb/parser.pyx":46
  *     fp = fopen(filename.encode('utf-8'), "r, ccs=UTF-8")
  *     if fp == NULL:
  *         raise FileNotFoundError("Could not open file")             # <<<<<<<<<<<<<<
  * 
  *     while fgets(line, 82, fp) != NULL: # 82
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FileNotFoundError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FileNotFoundError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 45, __pyx_L1_error)
+    __PYX_ERR(0, 46, __pyx_L1_error)
 
-    /* "cpdb/parser.pyx":44
+    /* "cpdb/parser.pyx":45
  *     line = <char *> malloc(82 * cython.sizeof(char))  # 82 chars to include newline and null terminator
  *     fp = fopen(filename.encode('utf-8'), "r, ccs=UTF-8")
  *     if fp == NULL:             # <<<<<<<<<<<<<<
  *         raise FileNotFoundError("Could not open file")
  * 
  */
   }
 
-  /* "cpdb/parser.pyx":47
+  /* "cpdb/parser.pyx":48
  *         raise FileNotFoundError("Could not open file")
  * 
  *     while fgets(line, 82, fp) != NULL: # 82             # <<<<<<<<<<<<<<
  *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':
  *             strncpy(atom_data[n_atoms].record_type, line, 6)
  */
   while (1) {
     __pyx_t_5 = ((fgets(__pyx_v_line, 82, __pyx_v_fp) != NULL) != 0);
     if (!__pyx_t_5) break;
 
-    /* "cpdb/parser.pyx":48
+    /* "cpdb/parser.pyx":49
  * 
  *     while fgets(line, 82, fp) != NULL: # 82
  *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':             # <<<<<<<<<<<<<<
  *             strncpy(atom_data[n_atoms].record_type, line, 6)
  *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 4 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 4 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_n_b_ATOM, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_6 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_n_b_ATOM, Py_EQ)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_7 = (__pyx_t_6 != 0);
     if (!__pyx_t_7) {
     } else {
       __pyx_t_5 = __pyx_t_7;
       goto __pyx_L7_bool_binop_done;
     }
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 6 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 6 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_n_b_HETATM, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 48, __pyx_L1_error)
+    __pyx_t_7 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_n_b_HETATM, Py_EQ)); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 49, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_6 = (__pyx_t_7 != 0);
     __pyx_t_5 = __pyx_t_6;
     __pyx_L7_bool_binop_done:;
     if (__pyx_t_5) {
 
-      /* "cpdb/parser.pyx":49
+      /* "cpdb/parser.pyx":50
  *     while fgets(line, 82, fp) != NULL: # 82
  *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':
  *             strncpy(atom_data[n_atoms].record_type, line, 6)             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
  * 
  */
       (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).record_type, __pyx_v_line, 6));
 
-      /* "cpdb/parser.pyx":50
+      /* "cpdb/parser.pyx":51
  *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':
  *             strncpy(atom_data[n_atoms].record_type, line, 6)
  *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator             # <<<<<<<<<<<<<<
  * 
  *             atom_data[n_atoms].atom_serial = atoi(line[6:11])
  */
       ((__pyx_v_atom_data[__pyx_v_n_atoms]).record_type[6]) = '\x00';
 
-      /* "cpdb/parser.pyx":52
+      /* "cpdb/parser.pyx":53
  *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
  * 
  *             atom_data[n_atoms].atom_serial = atoi(line[6:11])             # <<<<<<<<<<<<<<
  * 
  *             strncpy(atom_data[n_atoms].atom_name, line[12:16], 4)
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 6, 11 - 6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 52, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 6, 11 - 6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_8 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L1_error)
       (__pyx_v_atom_data[__pyx_v_n_atoms]).atom_serial = atoi(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":54
+      /* "cpdb/parser.pyx":55
  *             atom_data[n_atoms].atom_serial = atoi(line[6:11])
  * 
  *             strncpy(atom_data[n_atoms].atom_name, line[12:16], 4)             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].atom_name[4] = b'\0'
  * 
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 12, 16 - 12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 12, 16 - 12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 55, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L1_error)
       (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).atom_name, __pyx_t_9, 4));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":55
+      /* "cpdb/parser.pyx":56
  * 
  *             strncpy(atom_data[n_atoms].atom_name, line[12:16], 4)
  *             atom_data[n_atoms].atom_name[4] = b'\0'             # <<<<<<<<<<<<<<
  * 
  *             strncpy(atom_data[n_atoms].alt_loc, line[16:17], 1)
  */
       ((__pyx_v_atom_data[__pyx_v_n_atoms]).atom_name[4]) = '\x00';
 
-      /* "cpdb/parser.pyx":57
+      /* "cpdb/parser.pyx":58
  *             atom_data[n_atoms].atom_name[4] = b'\0'
  * 
  *             strncpy(atom_data[n_atoms].alt_loc, line[16:17], 1)             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].alt_loc[1] = b'\0'
  * 
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 16, 17 - 16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 16, 17 - 16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 58, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 57, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 58, __pyx_L1_error)
       (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).alt_loc, __pyx_t_9, 1));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":58
+      /* "cpdb/parser.pyx":59
  * 
  *             strncpy(atom_data[n_atoms].alt_loc, line[16:17], 1)
  *             atom_data[n_atoms].alt_loc[1] = b'\0'             # <<<<<<<<<<<<<<
  * 
  *             strncpy(atom_data[n_atoms].residue_name, line[17:20], 3)
  */
       ((__pyx_v_atom_data[__pyx_v_n_atoms]).alt_loc[1]) = '\x00';
 
-      /* "cpdb/parser.pyx":60
+      /* "cpdb/parser.pyx":61
  *             atom_data[n_atoms].alt_loc[1] = b'\0'
  * 
  *             strncpy(atom_data[n_atoms].residue_name, line[17:20], 3)             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].residue_name[3] = b'\0'
  * 
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 17, 20 - 17); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 60, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 17, 20 - 17); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 61, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 60, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 61, __pyx_L1_error)
       (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).residue_name, __pyx_t_9, 3));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":61
+      /* "cpdb/parser.pyx":62
  * 
  *             strncpy(atom_data[n_atoms].residue_name, line[17:20], 3)
  *             atom_data[n_atoms].residue_name[3] = b'\0'             # <<<<<<<<<<<<<<
  * 
  *             strncpy(atom_data[n_atoms].chain_id, line[21:22], 1)
  */
       ((__pyx_v_atom_data[__pyx_v_n_atoms]).residue_name[3]) = '\x00';
 
-      /* "cpdb/parser.pyx":63
+      /* "cpdb/parser.pyx":64
  *             atom_data[n_atoms].residue_name[3] = b'\0'
  * 
  *             strncpy(atom_data[n_atoms].chain_id, line[21:22], 1)             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].chain_id[1] = b'\0'
  * 
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 21, 22 - 21); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 21, 22 - 21); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 63, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L1_error)
       (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).chain_id, __pyx_t_9, 1));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":64
+      /* "cpdb/parser.pyx":65
  * 
  *             strncpy(atom_data[n_atoms].chain_id, line[21:22], 1)
  *             atom_data[n_atoms].chain_id[1] = b'\0'             # <<<<<<<<<<<<<<
  * 
  *             atom_data[n_atoms].res_num = atoi(line[22:26])
  */
       ((__pyx_v_atom_data[__pyx_v_n_atoms]).chain_id[1]) = '\x00';
 
-      /* "cpdb/parser.pyx":66
+      /* "cpdb/parser.pyx":67
  *             atom_data[n_atoms].chain_id[1] = b'\0'
  * 
  *             atom_data[n_atoms].res_num = atoi(line[22:26])             # <<<<<<<<<<<<<<
  * 
  *             strncpy(atom_data[n_atoms].iCode, line[26:27], 1)
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 22, 26 - 22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 66, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 22, 26 - 22); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_8 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 66, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L1_error)
       (__pyx_v_atom_data[__pyx_v_n_atoms]).res_num = atoi(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":68
+      /* "cpdb/parser.pyx":69
  *             atom_data[n_atoms].res_num = atoi(line[22:26])
  * 
  *             strncpy(atom_data[n_atoms].iCode, line[26:27], 1)             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].iCode[1] = b'\0'
  * 
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 26, 27 - 26); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 26, 27 - 26); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 69, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 69, __pyx_L1_error)
       (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).iCode, __pyx_t_9, 1));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":69
+      /* "cpdb/parser.pyx":70
  * 
  *             strncpy(atom_data[n_atoms].iCode, line[26:27], 1)
  *             atom_data[n_atoms].iCode[1] = b'\0'             # <<<<<<<<<<<<<<
  * 
  *             atom_data[n_atoms].x = atof(line[30:38])
  */
       ((__pyx_v_atom_data[__pyx_v_n_atoms]).iCode[1]) = '\x00';
 
-      /* "cpdb/parser.pyx":71
+      /* "cpdb/parser.pyx":72
  *             atom_data[n_atoms].iCode[1] = b'\0'
  * 
  *             atom_data[n_atoms].x = atof(line[30:38])             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].y = atof(line[38:46])
  *             atom_data[n_atoms].z = atof(line[46:54])
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 30, 38 - 30); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 71, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 30, 38 - 30); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 71, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L1_error)
       (__pyx_v_atom_data[__pyx_v_n_atoms]).x = atof(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":72
+      /* "cpdb/parser.pyx":73
  * 
  *             atom_data[n_atoms].x = atof(line[30:38])
  *             atom_data[n_atoms].y = atof(line[38:46])             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].z = atof(line[46:54])
  * 
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 38, 46 - 38); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 38, 46 - 38); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 72, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L1_error)
       (__pyx_v_atom_data[__pyx_v_n_atoms]).y = atof(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":73
+      /* "cpdb/parser.pyx":74
  *             atom_data[n_atoms].x = atof(line[30:38])
  *             atom_data[n_atoms].y = atof(line[38:46])
  *             atom_data[n_atoms].z = atof(line[46:54])             # <<<<<<<<<<<<<<
  * 
  *             atom_data[n_atoms].occupancy = atof(line[54:60])
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 46, 54 - 46); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 73, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 46, 54 - 46); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 74, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 73, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 74, __pyx_L1_error)
       (__pyx_v_atom_data[__pyx_v_n_atoms]).z = atof(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":75
+      /* "cpdb/parser.pyx":76
  *             atom_data[n_atoms].z = atof(line[46:54])
  * 
  *             atom_data[n_atoms].occupancy = atof(line[54:60])             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].temp_factor = atof(line[60:66])
  * 
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 54, 60 - 54); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 54, 60 - 54); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
       (__pyx_v_atom_data[__pyx_v_n_atoms]).occupancy = atof(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":76
+      /* "cpdb/parser.pyx":77
  * 
  *             atom_data[n_atoms].occupancy = atof(line[54:60])
  *             atom_data[n_atoms].temp_factor = atof(line[60:66])             # <<<<<<<<<<<<<<
  * 
  *             strncpy(atom_data[n_atoms].element_symbol, line[76:78], 2)
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 60, 66 - 60); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 60, 66 - 60); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 77, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 77, __pyx_L1_error)
       (__pyx_v_atom_data[__pyx_v_n_atoms]).temp_factor = atof(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":78
+      /* "cpdb/parser.pyx":79
  *             atom_data[n_atoms].temp_factor = atof(line[60:66])
  * 
  *             strncpy(atom_data[n_atoms].element_symbol, line[76:78], 2)             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].element_symbol[2] = b'\0'
  * 
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 76, 78 - 76); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 78, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 76, 78 - 76); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 79, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 78, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 79, __pyx_L1_error)
       (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).element_symbol, __pyx_t_9, 2));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":79
+      /* "cpdb/parser.pyx":80
  * 
  *             strncpy(atom_data[n_atoms].element_symbol, line[76:78], 2)
  *             atom_data[n_atoms].element_symbol[2] = b'\0'             # <<<<<<<<<<<<<<
  * 
  *             strncpy(atom_data[n_atoms].charge, line[78:79], 2)
  */
       ((__pyx_v_atom_data[__pyx_v_n_atoms]).element_symbol[2]) = '\x00';
 
-      /* "cpdb/parser.pyx":81
+      /* "cpdb/parser.pyx":82
  *             atom_data[n_atoms].element_symbol[2] = b'\0'
  * 
  *             strncpy(atom_data[n_atoms].charge, line[78:79], 2)             # <<<<<<<<<<<<<<
  *             atom_data[n_atoms].model_idx = n_model
  *             n_atoms += 1
  */
-      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 78, 79 - 78); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 78, 79 - 78); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 81, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyBytes_AsString(__pyx_t_2); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 82, __pyx_L1_error)
       (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).charge, __pyx_t_9, 2));
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "cpdb/parser.pyx":82
+      /* "cpdb/parser.pyx":83
  * 
  *             strncpy(atom_data[n_atoms].charge, line[78:79], 2)
  *             atom_data[n_atoms].model_idx = n_model             # <<<<<<<<<<<<<<
  *             n_atoms += 1
  * 
  */
       (__pyx_v_atom_data[__pyx_v_n_atoms]).model_idx = __pyx_v_n_model;
 
-      /* "cpdb/parser.pyx":83
+      /* "cpdb/parser.pyx":84
  *             strncpy(atom_data[n_atoms].charge, line[78:79], 2)
  *             atom_data[n_atoms].model_idx = n_model
  *             n_atoms += 1             # <<<<<<<<<<<<<<
  * 
  *             if n_atoms >= max_atoms:
  */
       __pyx_v_n_atoms = (__pyx_v_n_atoms + 1);
 
-      /* "cpdb/parser.pyx":85
+      /* "cpdb/parser.pyx":86
  *             n_atoms += 1
  * 
  *             if n_atoms >= max_atoms:             # <<<<<<<<<<<<<<
  *                 break
  *         elif line[:6] == b'ENDMDL':
  */
       __pyx_t_5 = ((__pyx_v_n_atoms >= __pyx_v_max_atoms) != 0);
       if (__pyx_t_5) {
 
-        /* "cpdb/parser.pyx":86
+        /* "cpdb/parser.pyx":87
  * 
  *             if n_atoms >= max_atoms:
  *                 break             # <<<<<<<<<<<<<<
  *         elif line[:6] == b'ENDMDL':
  *             n_model += 1
  */
         goto __pyx_L5_break;
 
-        /* "cpdb/parser.pyx":85
+        /* "cpdb/parser.pyx":86
  *             n_atoms += 1
  * 
  *             if n_atoms >= max_atoms:             # <<<<<<<<<<<<<<
  *                 break
  *         elif line[:6] == b'ENDMDL':
  */
       }
 
-      /* "cpdb/parser.pyx":48
+      /* "cpdb/parser.pyx":49
  * 
  *     while fgets(line, 82, fp) != NULL: # 82
  *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':             # <<<<<<<<<<<<<<
  *             strncpy(atom_data[n_atoms].record_type, line, 6)
  *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
  */
       goto __pyx_L6;
     }
 
-    /* "cpdb/parser.pyx":87
+    /* "cpdb/parser.pyx":88
  *             if n_atoms >= max_atoms:
  *                 break
  *         elif line[:6] == b'ENDMDL':             # <<<<<<<<<<<<<<
  *             n_model += 1
  * 
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 6 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 6 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_n_b_ENDMDL, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyBytes_Equals(__pyx_t_2, __pyx_n_b_ENDMDL, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_6 = (__pyx_t_5 != 0);
     if (__pyx_t_6) {
 
-      /* "cpdb/parser.pyx":88
+      /* "cpdb/parser.pyx":89
  *                 break
  *         elif line[:6] == b'ENDMDL':
  *             n_model += 1             # <<<<<<<<<<<<<<
  * 
  *     fclose(fp)
  */
       __pyx_v_n_model = (__pyx_v_n_model + 1);
 
-      /* "cpdb/parser.pyx":87
+      /* "cpdb/parser.pyx":88
  *             if n_atoms >= max_atoms:
  *                 break
  *         elif line[:6] == b'ENDMDL':             # <<<<<<<<<<<<<<
  *             n_model += 1
  * 
  */
     }
     __pyx_L6:;
   }
   __pyx_L5_break:;
 
-  /* "cpdb/parser.pyx":90
+  /* "cpdb/parser.pyx":91
  *             n_model += 1
  * 
  *     fclose(fp)             # <<<<<<<<<<<<<<
  *     free(line)
  * 
  */
   (void)(fclose(__pyx_v_fp));
 
-  /* "cpdb/parser.pyx":91
+  /* "cpdb/parser.pyx":92
  * 
  *     fclose(fp)
  *     free(line)             # <<<<<<<<<<<<<<
  * 
  *     # Create memory view arrays
  */
   free(__pyx_v_line);
 
-  /* "cpdb/parser.pyx":94
+  /* "cpdb/parser.pyx":95
  * 
  *     # Create memory view arrays
  *     cdef cnp.ndarray[float, ndim=1] x_coords = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_float32); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_float32); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 94, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 95, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 94, __pyx_L1_error)
+  if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 95, __pyx_L1_error)
   __pyx_t_13 = ((PyArrayObject *)__pyx_t_12);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_coords.rcbuffer->pybuffer, (PyObject*)__pyx_t_13, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_x_coords = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_x_coords.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 94, __pyx_L1_error)
+      __PYX_ERR(0, 95, __pyx_L1_error)
     } else {__pyx_pybuffernd_x_coords.diminfo[0].strides = __pyx_pybuffernd_x_coords.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_coords.diminfo[0].shape = __pyx_pybuffernd_x_coords.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_13 = 0;
   __pyx_v_x_coords = ((PyArrayObject *)__pyx_t_12);
   __pyx_t_12 = 0;
 
-  /* "cpdb/parser.pyx":95
+  /* "cpdb/parser.pyx":96
  *     # Create memory view arrays
  *     cdef cnp.ndarray[float, ndim=1] x_coords = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_12);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_12);
   __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float32); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float32); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_11) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_11) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 95, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 96, __pyx_L1_error)
   __pyx_t_14 = ((PyArrayObject *)__pyx_t_11);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_coords.rcbuffer->pybuffer, (PyObject*)__pyx_t_14, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_y_coords = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_y_coords.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 95, __pyx_L1_error)
+      __PYX_ERR(0, 96, __pyx_L1_error)
     } else {__pyx_pybuffernd_y_coords.diminfo[0].strides = __pyx_pybuffernd_y_coords.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_coords.diminfo[0].shape = __pyx_pybuffernd_y_coords.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_14 = 0;
   __pyx_v_y_coords = ((PyArrayObject *)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "cpdb/parser.pyx":96
+  /* "cpdb/parser.pyx":97
  *     cdef cnp.ndarray[float, ndim=1] x_coords = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_11);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_11);
   __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 96, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 97, __pyx_L1_error)
   __pyx_t_15 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_z_coords.rcbuffer->pybuffer, (PyObject*)__pyx_t_15, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_z_coords = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_z_coords.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 96, __pyx_L1_error)
+      __PYX_ERR(0, 97, __pyx_L1_error)
     } else {__pyx_pybuffernd_z_coords.diminfo[0].strides = __pyx_pybuffernd_z_coords.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_z_coords.diminfo[0].shape = __pyx_pybuffernd_z_coords.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_15 = 0;
   __pyx_v_z_coords = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cpdb/parser.pyx":97
+  /* "cpdb/parser.pyx":98
  *     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_float32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 98, __pyx_L1_error)
   __pyx_t_16 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_occupancies.rcbuffer->pybuffer, (PyObject*)__pyx_t_16, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_occupancies = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_occupancies.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 97, __pyx_L1_error)
+      __PYX_ERR(0, 98, __pyx_L1_error)
     } else {__pyx_pybuffernd_occupancies.diminfo[0].strides = __pyx_pybuffernd_occupancies.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_occupancies.diminfo[0].shape = __pyx_pybuffernd_occupancies.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_16 = 0;
   __pyx_v_occupancies = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cpdb/parser.pyx":98
+  /* "cpdb/parser.pyx":99
  *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
  *     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_float32); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_float32); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_t_12) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 98, __pyx_L1_error)
+  if (!(likely(((__pyx_t_12) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_12, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 99, __pyx_L1_error)
   __pyx_t_17 = ((PyArrayObject *)__pyx_t_12);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_b_factors.rcbuffer->pybuffer, (PyObject*)__pyx_t_17, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_b_factors = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_b_factors.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 98, __pyx_L1_error)
+      __PYX_ERR(0, 99, __pyx_L1_error)
     } else {__pyx_pybuffernd_b_factors.diminfo[0].strides = __pyx_pybuffernd_b_factors.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_b_factors.diminfo[0].shape = __pyx_pybuffernd_b_factors.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_17 = 0;
   __pyx_v_b_factors = ((PyArrayObject *)__pyx_t_12);
   __pyx_t_12 = 0;
 
-  /* "cpdb/parser.pyx":99
+  /* "cpdb/parser.pyx":100
  *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)
  *     cdef cnp.ndarray[int, ndim=1] model_idx = np.empty(n_atoms, dtype=np.int32)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_12);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_12);
   __pyx_t_12 = 0;
-  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_11) < 0) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_12, __pyx_n_s_dtype, __pyx_t_11) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 99, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_12); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 99, __pyx_L1_error)
+  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 100, __pyx_L1_error)
   __pyx_t_18 = ((PyArrayObject *)__pyx_t_11);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_atom_number.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_atom_number = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_atom_number.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 99, __pyx_L1_error)
+      __PYX_ERR(0, 100, __pyx_L1_error)
     } else {__pyx_pybuffernd_atom_number.diminfo[0].strides = __pyx_pybuffernd_atom_number.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_atom_number.diminfo[0].shape = __pyx_pybuffernd_atom_number.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_18 = 0;
   __pyx_v_atom_number = ((PyArrayObject *)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "cpdb/parser.pyx":100
+  /* "cpdb/parser.pyx":101
  *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
  *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
  *     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[int, ndim=1] model_idx = np.empty(n_atoms, dtype=np.int32)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_11);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_11);
   __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 101, __pyx_L1_error)
   __pyx_t_19 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_residue_number.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_residue_number = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_residue_number.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 100, __pyx_L1_error)
+      __PYX_ERR(0, 101, __pyx_L1_error)
     } else {__pyx_pybuffernd_residue_number.diminfo[0].strides = __pyx_pybuffernd_residue_number.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_residue_number.diminfo[0].shape = __pyx_pybuffernd_residue_number.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_19 = 0;
   __pyx_v_residue_number = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cpdb/parser.pyx":101
+  /* "cpdb/parser.pyx":102
  *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
  *     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)
  *     cdef cnp.ndarray[int, ndim=1] model_idx = np.empty(n_atoms, dtype=np.int32)             # <<<<<<<<<<<<<<
  * 
  *     # Create NumPy arrays for string columns
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_np); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_int32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_int32); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_2) < 0) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 101, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 102, __pyx_L1_error)
   __pyx_t_20 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_model_idx.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_model_idx = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_model_idx.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 101, __pyx_L1_error)
+      __PYX_ERR(0, 102, __pyx_L1_error)
     } else {__pyx_pybuffernd_model_idx.diminfo[0].strides = __pyx_pybuffernd_model_idx.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_model_idx.diminfo[0].shape = __pyx_pybuffernd_model_idx.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_20 = 0;
   __pyx_v_model_idx = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cpdb/parser.pyx":104
+  /* "cpdb/parser.pyx":105
  * 
  *     # Create NumPy arrays for string columns
  *     cdef cnp.ndarray[object, ndim=1] record_name = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 104, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 104, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 105, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 104, __pyx_L1_error)
+  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 105, __pyx_L1_error)
   __pyx_t_21 = ((PyArrayObject *)__pyx_t_11);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_record_name.rcbuffer->pybuffer, (PyObject*)__pyx_t_21, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_record_name = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_record_name.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 104, __pyx_L1_error)
+      __PYX_ERR(0, 105, __pyx_L1_error)
     } else {__pyx_pybuffernd_record_name.diminfo[0].strides = __pyx_pybuffernd_record_name.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_record_name.diminfo[0].shape = __pyx_pybuffernd_record_name.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_21 = 0;
   __pyx_v_record_name = ((PyArrayObject *)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "cpdb/parser.pyx":105
+  /* "cpdb/parser.pyx":106
  *     # Create NumPy arrays for string columns
  *     cdef cnp.ndarray[object, ndim=1] record_name = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_11);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_11);
   __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 105, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 106, __pyx_L1_error)
   __pyx_t_22 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_atom_name.rcbuffer->pybuffer, (PyObject*)__pyx_t_22, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_atom_name = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_atom_name.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 105, __pyx_L1_error)
+      __PYX_ERR(0, 106, __pyx_L1_error)
     } else {__pyx_pybuffernd_atom_name.diminfo[0].strides = __pyx_pybuffernd_atom_name.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_atom_name.diminfo[0].shape = __pyx_pybuffernd_atom_name.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_22 = 0;
   __pyx_v_atom_name = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cpdb/parser.pyx":106
+  /* "cpdb/parser.pyx":107
  *     cdef cnp.ndarray[object, ndim=1] record_name = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 106, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 107, __pyx_L1_error)
   __pyx_t_23 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_alt_loc.rcbuffer->pybuffer, (PyObject*)__pyx_t_23, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_alt_loc = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_alt_loc.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 106, __pyx_L1_error)
+      __PYX_ERR(0, 107, __pyx_L1_error)
     } else {__pyx_pybuffernd_alt_loc.diminfo[0].strides = __pyx_pybuffernd_alt_loc.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_alt_loc.diminfo[0].shape = __pyx_pybuffernd_alt_loc.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_23 = 0;
   __pyx_v_alt_loc = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cpdb/parser.pyx":107
+  /* "cpdb/parser.pyx":108
  *     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 107, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 108, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 107, __pyx_L1_error)
+  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 108, __pyx_L1_error)
   __pyx_t_24 = ((PyArrayObject *)__pyx_t_11);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_residue_name.rcbuffer->pybuffer, (PyObject*)__pyx_t_24, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_residue_name = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_residue_name.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 107, __pyx_L1_error)
+      __PYX_ERR(0, 108, __pyx_L1_error)
     } else {__pyx_pybuffernd_residue_name.diminfo[0].strides = __pyx_pybuffernd_residue_name.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_residue_name.diminfo[0].shape = __pyx_pybuffernd_residue_name.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_24 = 0;
   __pyx_v_residue_name = ((PyArrayObject *)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "cpdb/parser.pyx":108
+  /* "cpdb/parser.pyx":109
  *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_11);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_11);
   __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 108, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 108, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 108, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 109, __pyx_L1_error)
   __pyx_t_25 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_chain_id.rcbuffer->pybuffer, (PyObject*)__pyx_t_25, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_chain_id = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_chain_id.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 108, __pyx_L1_error)
+      __PYX_ERR(0, 109, __pyx_L1_error)
     } else {__pyx_pybuffernd_chain_id.diminfo[0].strides = __pyx_pybuffernd_chain_id.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_chain_id.diminfo[0].shape = __pyx_pybuffernd_chain_id.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_25 = 0;
   __pyx_v_chain_id = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cpdb/parser.pyx":109
+  /* "cpdb/parser.pyx":110
  *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] charge = np.empty(n_atoms, dtype=object)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 109, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 109, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_11, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 109, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 110, __pyx_L1_error)
   __pyx_t_26 = ((PyArrayObject *)__pyx_t_2);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_insertion.rcbuffer->pybuffer, (PyObject*)__pyx_t_26, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_insertion = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_insertion.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 109, __pyx_L1_error)
+      __PYX_ERR(0, 110, __pyx_L1_error)
     } else {__pyx_pybuffernd_insertion.diminfo[0].strides = __pyx_pybuffernd_insertion.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_insertion.diminfo[0].shape = __pyx_pybuffernd_insertion.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_26 = 0;
   __pyx_v_insertion = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "cpdb/parser.pyx":110
+  /* "cpdb/parser.pyx":111
  *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
  *     cdef cnp.ndarray[object, ndim=1] charge = np.empty(n_atoms, dtype=object)
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 110, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 110, __pyx_L1_error)
-  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 110, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 110, __pyx_L1_error)
+  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 111, __pyx_L1_error)
   __pyx_t_27 = ((PyArrayObject *)__pyx_t_11);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_element_symbol.rcbuffer->pybuffer, (PyObject*)__pyx_t_27, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_element_symbol = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_element_symbol.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 110, __pyx_L1_error)
+      __PYX_ERR(0, 111, __pyx_L1_error)
     } else {__pyx_pybuffernd_element_symbol.diminfo[0].strides = __pyx_pybuffernd_element_symbol.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_element_symbol.diminfo[0].shape = __pyx_pybuffernd_element_symbol.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_27 = 0;
   __pyx_v_element_symbol = ((PyArrayObject *)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "cpdb/parser.pyx":111
+  /* "cpdb/parser.pyx":112
  *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)
  *     cdef cnp.ndarray[object, ndim=1] charge = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
  * 
  *     # Fill memory view arrays
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_11, __pyx_n_s_np); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_11);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_11);
   __pyx_t_11 = 0;
-  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 111, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
-  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 112, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_11); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 111, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 112, __pyx_L1_error)
   __pyx_t_28 = ((PyArrayObject *)__pyx_t_1);
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_charge.rcbuffer->pybuffer, (PyObject*)__pyx_t_28, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
       __pyx_v_charge = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_charge.rcbuffer->pybuffer.buf = NULL;
-      __PYX_ERR(0, 111, __pyx_L1_error)
+      __PYX_ERR(0, 112, __pyx_L1_error)
     } else {__pyx_pybuffernd_charge.diminfo[0].strides = __pyx_pybuffernd_charge.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_charge.diminfo[0].shape = __pyx_pybuffernd_charge.rcbuffer->pybuffer.shape[0];
     }
   }
   __pyx_t_28 = 0;
   __pyx_v_charge = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cpdb/parser.pyx":114
+  /* "cpdb/parser.pyx":115
  * 
  *     # Fill memory view arrays
  *     for i in range(n_atoms):             # <<<<<<<<<<<<<<
  *         x_coords[i] = atom_data[i].x
  *         y_coords[i] = atom_data[i].y
  */
   __pyx_t_29 = __pyx_v_n_atoms;
   __pyx_t_30 = __pyx_t_29;
   for (__pyx_t_31 = 0; __pyx_t_31 < __pyx_t_30; __pyx_t_31+=1) {
     __pyx_v_i = __pyx_t_31;
 
-    /* "cpdb/parser.pyx":115
+    /* "cpdb/parser.pyx":116
  *     # Fill memory view arrays
  *     for i in range(n_atoms):
  *         x_coords[i] = atom_data[i].x             # <<<<<<<<<<<<<<
  *         y_coords[i] = atom_data[i].y
  *         z_coords[i] = atom_data[i].z
  */
     __pyx_t_32 = (__pyx_v_atom_data[__pyx_v_i]).x;
     __pyx_t_33 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_x_coords.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_x_coords.diminfo[0].strides) = __pyx_t_32;
 
-    /* "cpdb/parser.pyx":116
+    /* "cpdb/parser.pyx":117
  *     for i in range(n_atoms):
  *         x_coords[i] = atom_data[i].x
  *         y_coords[i] = atom_data[i].y             # <<<<<<<<<<<<<<
  *         z_coords[i] = atom_data[i].z
  *         occupancies[i] = atom_data[i].occupancy
  */
     __pyx_t_32 = (__pyx_v_atom_data[__pyx_v_i]).y;
     __pyx_t_33 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_y_coords.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_y_coords.diminfo[0].strides) = __pyx_t_32;
 
-    /* "cpdb/parser.pyx":117
+    /* "cpdb/parser.pyx":118
  *         x_coords[i] = atom_data[i].x
  *         y_coords[i] = atom_data[i].y
  *         z_coords[i] = atom_data[i].z             # <<<<<<<<<<<<<<
  *         occupancies[i] = atom_data[i].occupancy
  *         b_factors[i] = atom_data[i].temp_factor
  */
     __pyx_t_32 = (__pyx_v_atom_data[__pyx_v_i]).z;
     __pyx_t_33 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_z_coords.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_z_coords.diminfo[0].strides) = __pyx_t_32;
 
-    /* "cpdb/parser.pyx":118
+    /* "cpdb/parser.pyx":119
  *         y_coords[i] = atom_data[i].y
  *         z_coords[i] = atom_data[i].z
  *         occupancies[i] = atom_data[i].occupancy             # <<<<<<<<<<<<<<
  *         b_factors[i] = atom_data[i].temp_factor
  *         model_idx[i] = atom_data[i].model_idx
  */
     __pyx_t_32 = (__pyx_v_atom_data[__pyx_v_i]).occupancy;
     __pyx_t_33 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_occupancies.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_occupancies.diminfo[0].strides) = __pyx_t_32;
 
-    /* "cpdb/parser.pyx":119
+    /* "cpdb/parser.pyx":120
  *         z_coords[i] = atom_data[i].z
  *         occupancies[i] = atom_data[i].occupancy
  *         b_factors[i] = atom_data[i].temp_factor             # <<<<<<<<<<<<<<
  *         model_idx[i] = atom_data[i].model_idx
  *         atom_number[i] = atom_data[i].atom_serial
  */
     __pyx_t_32 = (__pyx_v_atom_data[__pyx_v_i]).temp_factor;
     __pyx_t_33 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_b_factors.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_b_factors.diminfo[0].strides) = __pyx_t_32;
 
-    /* "cpdb/parser.pyx":120
+    /* "cpdb/parser.pyx":121
  *         occupancies[i] = atom_data[i].occupancy
  *         b_factors[i] = atom_data[i].temp_factor
  *         model_idx[i] = atom_data[i].model_idx             # <<<<<<<<<<<<<<
  *         atom_number[i] = atom_data[i].atom_serial
  *         residue_number[i] = atom_data[i].res_num
  */
     __pyx_t_34 = (__pyx_v_atom_data[__pyx_v_i]).model_idx;
     __pyx_t_33 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_model_idx.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_model_idx.diminfo[0].strides) = __pyx_t_34;
 
-    /* "cpdb/parser.pyx":121
+    /* "cpdb/parser.pyx":122
  *         b_factors[i] = atom_data[i].temp_factor
  *         model_idx[i] = atom_data[i].model_idx
  *         atom_number[i] = atom_data[i].atom_serial             # <<<<<<<<<<<<<<
  *         residue_number[i] = atom_data[i].res_num
  * 
  */
     __pyx_t_34 = (__pyx_v_atom_data[__pyx_v_i]).atom_serial;
     __pyx_t_33 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_atom_number.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_atom_number.diminfo[0].strides) = __pyx_t_34;
 
-    /* "cpdb/parser.pyx":122
+    /* "cpdb/parser.pyx":123
  *         model_idx[i] = atom_data[i].model_idx
  *         atom_number[i] = atom_data[i].atom_serial
  *         residue_number[i] = atom_data[i].res_num             # <<<<<<<<<<<<<<
  * 
  *         # Fill NumPy arrays for string columns
  */
     __pyx_t_34 = (__pyx_v_atom_data[__pyx_v_i]).res_num;
     __pyx_t_33 = __pyx_v_i;
     *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_residue_number.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_residue_number.diminfo[0].strides) = __pyx_t_34;
 
-    /* "cpdb/parser.pyx":125
+    /* "cpdb/parser.pyx":126
  * 
  *         # Fill NumPy arrays for string columns
  *         record_name[i] = atom_data[i].record_type[:strlen(atom_data[i].record_type)].decode('ascii', errors='replace').strip()             # <<<<<<<<<<<<<<
  *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
  *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
  */
-    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).record_type) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).record_type) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).record_type) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).record_type) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__2, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_11, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_33 = __pyx_v_i;
     __pyx_t_35 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_record_name.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_record_name.diminfo[0].strides);
     __Pyx_XGOTREF(*__pyx_t_35);
     __Pyx_INCREF(__pyx_t_1); __Pyx_XDECREF(*__pyx_t_35);
     *__pyx_t_35 = __pyx_t_1;
     __Pyx_XGIVEREF(*__pyx_t_35);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpdb/parser.pyx":126
+    /* "cpdb/parser.pyx":127
  *         # Fill NumPy arrays for string columns
  *         record_name[i] = atom_data[i].record_type[:strlen(atom_data[i].record_type)].decode('ascii', errors='replace').strip()
  *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()             # <<<<<<<<<<<<<<
  *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
  *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
  */
-    __pyx_t_11 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).atom_name, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).atom_name), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).atom_name, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).atom_name), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 127, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_strip); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_strip); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_11 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_11)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_11);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_33 = __pyx_v_i;
     __pyx_t_35 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_atom_name.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_atom_name.diminfo[0].strides);
     __Pyx_XGOTREF(*__pyx_t_35);
     __Pyx_INCREF(__pyx_t_1); __Pyx_XDECREF(*__pyx_t_35);
     *__pyx_t_35 = __pyx_t_1;
     __Pyx_XGIVEREF(*__pyx_t_35);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpdb/parser.pyx":127
+    /* "cpdb/parser.pyx":128
  *         record_name[i] = atom_data[i].record_type[:strlen(atom_data[i].record_type)].decode('ascii', errors='replace').strip()
  *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
  *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()             # <<<<<<<<<<<<<<
  *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
  *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
  */
-    __pyx_t_2 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).alt_loc, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).alt_loc), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).alt_loc, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).alt_loc), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_11, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_33 = __pyx_v_i;
     __pyx_t_35 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_alt_loc.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_alt_loc.diminfo[0].strides);
     __Pyx_XGOTREF(*__pyx_t_35);
     __Pyx_INCREF(__pyx_t_1); __Pyx_XDECREF(*__pyx_t_35);
     *__pyx_t_35 = __pyx_t_1;
     __Pyx_XGIVEREF(*__pyx_t_35);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpdb/parser.pyx":128
+    /* "cpdb/parser.pyx":129
  *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
  *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
  *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
  *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
  *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
  */
-    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).residue_name) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).residue_name) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).residue_name) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).residue_name) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 128, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, __pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 128, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, __pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_11, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_33 = __pyx_v_i;
     __pyx_t_35 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_residue_name.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_residue_name.diminfo[0].strides);
     __Pyx_XGOTREF(*__pyx_t_35);
     __Pyx_INCREF(__pyx_t_1); __Pyx_XDECREF(*__pyx_t_35);
     *__pyx_t_35 = __pyx_t_1;
     __Pyx_XGIVEREF(*__pyx_t_35);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpdb/parser.pyx":129
+    /* "cpdb/parser.pyx":130
  *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
  *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
  *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
  *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
  *         element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()
  */
-    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).chain_id) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).chain_id) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).chain_id) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).chain_id) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_11, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_33 = __pyx_v_i;
     __pyx_t_35 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_chain_id.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_chain_id.diminfo[0].strides);
     __Pyx_XGOTREF(*__pyx_t_35);
     __Pyx_INCREF(__pyx_t_1); __Pyx_XDECREF(*__pyx_t_35);
     *__pyx_t_35 = __pyx_t_1;
     __Pyx_XGIVEREF(*__pyx_t_35);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpdb/parser.pyx":130
+    /* "cpdb/parser.pyx":131
  *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
  *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
  *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
  *         element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()
  *         charge[i] = atom_data[i].charge[:strlen(atom_data[i].charge)].decode('utf-8').strip()
  */
-    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).iCode) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).iCode) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).iCode) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).iCode) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, __pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_tuple__3, __pyx_t_11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_11, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_33 = __pyx_v_i;
     __pyx_t_35 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_insertion.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_insertion.diminfo[0].strides);
     __Pyx_XGOTREF(*__pyx_t_35);
     __Pyx_INCREF(__pyx_t_1); __Pyx_XDECREF(*__pyx_t_35);
     *__pyx_t_35 = __pyx_t_1;
     __Pyx_XGIVEREF(*__pyx_t_35);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpdb/parser.pyx":131
+    /* "cpdb/parser.pyx":132
  *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
  *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
  *         element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
  *         charge[i] = atom_data[i].charge[:strlen(atom_data[i].charge)].decode('utf-8').strip()
  * 
  */
-    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).element_symbol) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).element_symbol) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).element_symbol) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).element_symbol) - 0); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_decode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_11, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_tuple__3, __pyx_t_11); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_strip); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_11);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_11, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_11);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_33 = __pyx_v_i;
     __pyx_t_35 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_element_symbol.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_element_symbol.diminfo[0].strides);
     __Pyx_XGOTREF(*__pyx_t_35);
     __Pyx_INCREF(__pyx_t_1); __Pyx_XDECREF(*__pyx_t_35);
     *__pyx_t_35 = __pyx_t_1;
     __Pyx_XGIVEREF(*__pyx_t_35);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "cpdb/parser.pyx":132
+    /* "cpdb/parser.pyx":133
  *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
  *         element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()
  *         charge[i] = atom_data[i].charge[:strlen(atom_data[i].charge)].decode('utf-8').strip()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_11 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).charge, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).charge), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).charge, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).charge), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_strip); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_11, __pyx_n_s_strip); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
     __pyx_t_11 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_11 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_11)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_11);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_11) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_33 = __pyx_v_i;
     __pyx_t_35 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_charge.rcbuffer->pybuffer.buf, __pyx_t_33, __pyx_pybuffernd_charge.diminfo[0].strides);
     __Pyx_XGOTREF(*__pyx_t_35);
     __Pyx_INCREF(__pyx_t_1); __Pyx_XDECREF(*__pyx_t_35);
     *__pyx_t_35 = __pyx_t_1;
     __Pyx_XGIVEREF(*__pyx_t_35);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "cpdb/parser.pyx":137
+  /* "cpdb/parser.pyx":138
  *     # Convert the C struct data to Python objects and return
  *     result = {
  *         'record_name': record_name,             # <<<<<<<<<<<<<<
  *         'atom_number': atom_number,
  *         'atom_name': atom_name,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_record_name, ((PyObject *)__pyx_v_record_name)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_record_name, ((PyObject *)__pyx_v_record_name)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":138
+  /* "cpdb/parser.pyx":139
  *     result = {
  *         'record_name': record_name,
  *         'atom_number': atom_number,             # <<<<<<<<<<<<<<
  *         'atom_name': atom_name,
  *         'alt_loc': alt_loc,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_atom_number, ((PyObject *)__pyx_v_atom_number)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_atom_number, ((PyObject *)__pyx_v_atom_number)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":139
+  /* "cpdb/parser.pyx":140
  *         'record_name': record_name,
  *         'atom_number': atom_number,
  *         'atom_name': atom_name,             # <<<<<<<<<<<<<<
  *         'alt_loc': alt_loc,
  *         'residue_name': residue_name,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_atom_name, ((PyObject *)__pyx_v_atom_name)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_atom_name, ((PyObject *)__pyx_v_atom_name)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":140
+  /* "cpdb/parser.pyx":141
  *         'atom_number': atom_number,
  *         'atom_name': atom_name,
  *         'alt_loc': alt_loc,             # <<<<<<<<<<<<<<
  *         'residue_name': residue_name,
  *         'chain_id': chain_id,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_alt_loc, ((PyObject *)__pyx_v_alt_loc)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_alt_loc, ((PyObject *)__pyx_v_alt_loc)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":141
+  /* "cpdb/parser.pyx":142
  *         'atom_name': atom_name,
  *         'alt_loc': alt_loc,
  *         'residue_name': residue_name,             # <<<<<<<<<<<<<<
  *         'chain_id': chain_id,
  *         'residue_number': residue_number,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_residue_name, ((PyObject *)__pyx_v_residue_name)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_residue_name, ((PyObject *)__pyx_v_residue_name)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":142
+  /* "cpdb/parser.pyx":143
  *         'alt_loc': alt_loc,
  *         'residue_name': residue_name,
  *         'chain_id': chain_id,             # <<<<<<<<<<<<<<
  *         'residue_number': residue_number,
  *         "insertion": insertion,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_chain_id, ((PyObject *)__pyx_v_chain_id)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_chain_id, ((PyObject *)__pyx_v_chain_id)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":143
+  /* "cpdb/parser.pyx":144
  *         'residue_name': residue_name,
  *         'chain_id': chain_id,
  *         'residue_number': residue_number,             # <<<<<<<<<<<<<<
  *         "insertion": insertion,
  *         'x_coord': x_coords,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_residue_number, ((PyObject *)__pyx_v_residue_number)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_residue_number, ((PyObject *)__pyx_v_residue_number)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":144
+  /* "cpdb/parser.pyx":145
  *         'chain_id': chain_id,
  *         'residue_number': residue_number,
  *         "insertion": insertion,             # <<<<<<<<<<<<<<
  *         'x_coord': x_coords,
  *         'y_coord': y_coords,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_insertion, ((PyObject *)__pyx_v_insertion)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_insertion, ((PyObject *)__pyx_v_insertion)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":145
+  /* "cpdb/parser.pyx":146
  *         'residue_number': residue_number,
  *         "insertion": insertion,
  *         'x_coord': x_coords,             # <<<<<<<<<<<<<<
  *         'y_coord': y_coords,
  *         'z_coord': z_coords,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_x_coord, ((PyObject *)__pyx_v_x_coords)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_x_coord, ((PyObject *)__pyx_v_x_coords)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":146
+  /* "cpdb/parser.pyx":147
  *         "insertion": insertion,
  *         'x_coord': x_coords,
  *         'y_coord': y_coords,             # <<<<<<<<<<<<<<
  *         'z_coord': z_coords,
  *         'occupancy': occupancies,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_y_coord, ((PyObject *)__pyx_v_y_coords)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_y_coord, ((PyObject *)__pyx_v_y_coords)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":147
+  /* "cpdb/parser.pyx":148
  *         'x_coord': x_coords,
  *         'y_coord': y_coords,
  *         'z_coord': z_coords,             # <<<<<<<<<<<<<<
  *         'occupancy': occupancies,
  *         'b_factor': b_factors,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_z_coord, ((PyObject *)__pyx_v_z_coords)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_z_coord, ((PyObject *)__pyx_v_z_coords)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":148
+  /* "cpdb/parser.pyx":149
  *         'y_coord': y_coords,
  *         'z_coord': z_coords,
  *         'occupancy': occupancies,             # <<<<<<<<<<<<<<
  *         'b_factor': b_factors,
  *         'element_symbol': element_symbol,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_occupancy, ((PyObject *)__pyx_v_occupancies)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_occupancy, ((PyObject *)__pyx_v_occupancies)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":149
+  /* "cpdb/parser.pyx":150
  *         'z_coord': z_coords,
  *         'occupancy': occupancies,
  *         'b_factor': b_factors,             # <<<<<<<<<<<<<<
  *         'element_symbol': element_symbol,
  *         'charge': charge,
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_b_factor, ((PyObject *)__pyx_v_b_factors)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_b_factor, ((PyObject *)__pyx_v_b_factors)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":150
+  /* "cpdb/parser.pyx":151
  *         'occupancy': occupancies,
  *         'b_factor': b_factors,
  *         'element_symbol': element_symbol,             # <<<<<<<<<<<<<<
  *         'charge': charge,
  *         'model_idx': model_idx
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_element_symbol, ((PyObject *)__pyx_v_element_symbol)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_element_symbol, ((PyObject *)__pyx_v_element_symbol)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":151
+  /* "cpdb/parser.pyx":152
  *         'b_factor': b_factors,
  *         'element_symbol': element_symbol,
  *         'charge': charge,             # <<<<<<<<<<<<<<
  *         'model_idx': model_idx
  *     }
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_charge, ((PyObject *)__pyx_v_charge)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_charge, ((PyObject *)__pyx_v_charge)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
 
-  /* "cpdb/parser.pyx":152
+  /* "cpdb/parser.pyx":153
  *         'element_symbol': element_symbol,
  *         'charge': charge,
  *         'model_idx': model_idx             # <<<<<<<<<<<<<<
  *     }
  * 
  */
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_model_idx, ((PyObject *)__pyx_v_model_idx)) < 0) __PYX_ERR(0, 137, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_u_model_idx, ((PyObject *)__pyx_v_model_idx)) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "cpdb/parser.pyx":156
+  /* "cpdb/parser.pyx":157
  * 
  *     # Free the allocated memory for the atom_data array
  *     free(atom_data)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   free(__pyx_v_atom_data);
 
-  /* "cpdb/parser.pyx":158
+  /* "cpdb/parser.pyx":159
  *     free(atom_data)
  * 
  *     return result             # <<<<<<<<<<<<<<
+ * 
+ * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "cpdb/parser.pyx":33
+  /* "cpdb/parser.pyx":34
  * @cython.wraparound(False)
  * @cython.nonecheck(False)
- * def parse_pdb(filename, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
+ * def parse_pdb_file(filename, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
  *     cdef FILE *fp = NULL
  *     cdef char *line = NULL
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
@@ -4145,15 +4153,2179 @@
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_record_name.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_residue_name.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_residue_number.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_coords.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_y_coords.rcbuffer->pybuffer);
     __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z_coords.rcbuffer->pybuffer);
   __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
-  __Pyx_AddTraceback("cpdb.parser.parse_pdb", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("cpdb.parser.parse_pdb_file", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_alt_loc.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_atom_name.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_atom_number.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_b_factors.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_chain_id.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_charge.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_element_symbol.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_insertion.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_model_idx.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_occupancies.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_record_name.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_residue_name.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_residue_number.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_coords.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_y_coords.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z_coords.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_x_coords);
+  __Pyx_XDECREF((PyObject *)__pyx_v_y_coords);
+  __Pyx_XDECREF((PyObject *)__pyx_v_z_coords);
+  __Pyx_XDECREF((PyObject *)__pyx_v_occupancies);
+  __Pyx_XDECREF((PyObject *)__pyx_v_b_factors);
+  __Pyx_XDECREF((PyObject *)__pyx_v_atom_number);
+  __Pyx_XDECREF((PyObject *)__pyx_v_residue_number);
+  __Pyx_XDECREF((PyObject *)__pyx_v_model_idx);
+  __Pyx_XDECREF((PyObject *)__pyx_v_record_name);
+  __Pyx_XDECREF((PyObject *)__pyx_v_atom_name);
+  __Pyx_XDECREF((PyObject *)__pyx_v_alt_loc);
+  __Pyx_XDECREF((PyObject *)__pyx_v_residue_name);
+  __Pyx_XDECREF((PyObject *)__pyx_v_chain_id);
+  __Pyx_XDECREF((PyObject *)__pyx_v_insertion);
+  __Pyx_XDECREF((PyObject *)__pyx_v_element_symbol);
+  __Pyx_XDECREF((PyObject *)__pyx_v_charge);
+  __Pyx_XDECREF(__pyx_v_result);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "cpdb/parser.pyx":164
+ * @cython.wraparound(False)
+ * @cython.nonecheck(False)
+ * def parse_pdb_string(cnp.str input_str, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
+ *     cdef char *line = NULL
+ *     cdef int n_atoms = 0
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4cpdb_6parser_3parse_pdb_string(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_4cpdb_6parser_3parse_pdb_string = {"parse_pdb_string", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_4cpdb_6parser_3parse_pdb_string, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4cpdb_6parser_3parse_pdb_string(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_input_str = 0;
+  int __pyx_v_max_atoms;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("parse_pdb_string (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_input_str,&__pyx_n_s_max_atoms,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_input_str)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_max_atoms);
+          if (value) { values[1] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "parse_pdb_string") < 0)) __PYX_ERR(0, 164, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_input_str = ((PyObject*)values[0]);
+    if (values[1]) {
+      __pyx_v_max_atoms = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_max_atoms == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
+    } else {
+      __pyx_v_max_atoms = ((int)0xF4240);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("parse_pdb_string", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 164, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("cpdb.parser.parse_pdb_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_input_str), (&PyUnicode_Type), 1, "input_str", 1))) __PYX_ERR(0, 164, __pyx_L1_error)
+  __pyx_r = __pyx_pf_4cpdb_6parser_2parse_pdb_string(__pyx_self, __pyx_v_input_str, __pyx_v_max_atoms);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4cpdb_6parser_2parse_pdb_string(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_str, int __pyx_v_max_atoms) {
+  char *__pyx_v_line;
+  int __pyx_v_n_atoms;
+  int __pyx_v_i;
+  int __pyx_v_n_model;
+  PyObject *__pyx_v_py_bytes = 0;
+  struct __pyx_t_4cpdb_6parser_AtomData *__pyx_v_atom_data;
+  PyObject *__pyx_v_lines = NULL;
+  PyObject *__pyx_v_python_line = NULL;
+  PyArrayObject *__pyx_v_x_coords = 0;
+  PyArrayObject *__pyx_v_y_coords = 0;
+  PyArrayObject *__pyx_v_z_coords = 0;
+  PyArrayObject *__pyx_v_occupancies = 0;
+  PyArrayObject *__pyx_v_b_factors = 0;
+  PyArrayObject *__pyx_v_atom_number = 0;
+  PyArrayObject *__pyx_v_residue_number = 0;
+  PyArrayObject *__pyx_v_model_idx = 0;
+  PyArrayObject *__pyx_v_record_name = 0;
+  PyArrayObject *__pyx_v_atom_name = 0;
+  PyArrayObject *__pyx_v_alt_loc = 0;
+  PyArrayObject *__pyx_v_residue_name = 0;
+  PyArrayObject *__pyx_v_chain_id = 0;
+  PyArrayObject *__pyx_v_insertion = 0;
+  PyArrayObject *__pyx_v_element_symbol = 0;
+  PyArrayObject *__pyx_v_charge = 0;
+  PyObject *__pyx_v_result = NULL;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_alt_loc;
+  __Pyx_Buffer __pyx_pybuffer_alt_loc;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_atom_name;
+  __Pyx_Buffer __pyx_pybuffer_atom_name;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_atom_number;
+  __Pyx_Buffer __pyx_pybuffer_atom_number;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_b_factors;
+  __Pyx_Buffer __pyx_pybuffer_b_factors;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_chain_id;
+  __Pyx_Buffer __pyx_pybuffer_chain_id;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_charge;
+  __Pyx_Buffer __pyx_pybuffer_charge;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_element_symbol;
+  __Pyx_Buffer __pyx_pybuffer_element_symbol;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_insertion;
+  __Pyx_Buffer __pyx_pybuffer_insertion;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_model_idx;
+  __Pyx_Buffer __pyx_pybuffer_model_idx;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_occupancies;
+  __Pyx_Buffer __pyx_pybuffer_occupancies;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_record_name;
+  __Pyx_Buffer __pyx_pybuffer_record_name;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_residue_name;
+  __Pyx_Buffer __pyx_pybuffer_residue_name;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_residue_number;
+  __Pyx_Buffer __pyx_pybuffer_residue_number;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_x_coords;
+  __Pyx_Buffer __pyx_pybuffer_x_coords;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_y_coords;
+  __Pyx_Buffer __pyx_pybuffer_y_coords;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_z_coords;
+  __Pyx_Buffer __pyx_pybuffer_z_coords;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  char *__pyx_t_7;
+  int __pyx_t_8;
+  int __pyx_t_9;
+  int __pyx_t_10;
+  char const *__pyx_t_11;
+  char const *__pyx_t_12;
+  char const *__pyx_t_13;
+  PyObject *__pyx_t_14 = NULL;
+  PyArrayObject *__pyx_t_15 = NULL;
+  PyArrayObject *__pyx_t_16 = NULL;
+  PyArrayObject *__pyx_t_17 = NULL;
+  PyArrayObject *__pyx_t_18 = NULL;
+  PyArrayObject *__pyx_t_19 = NULL;
+  PyArrayObject *__pyx_t_20 = NULL;
+  PyArrayObject *__pyx_t_21 = NULL;
+  PyArrayObject *__pyx_t_22 = NULL;
+  PyArrayObject *__pyx_t_23 = NULL;
+  PyArrayObject *__pyx_t_24 = NULL;
+  PyArrayObject *__pyx_t_25 = NULL;
+  PyArrayObject *__pyx_t_26 = NULL;
+  PyArrayObject *__pyx_t_27 = NULL;
+  PyArrayObject *__pyx_t_28 = NULL;
+  PyArrayObject *__pyx_t_29 = NULL;
+  PyArrayObject *__pyx_t_30 = NULL;
+  int __pyx_t_31;
+  int __pyx_t_32;
+  int __pyx_t_33;
+  float __pyx_t_34;
+  Py_ssize_t __pyx_t_35;
+  int __pyx_t_36;
+  PyObject **__pyx_t_37;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("parse_pdb_string", 0);
+  __pyx_pybuffer_x_coords.pybuffer.buf = NULL;
+  __pyx_pybuffer_x_coords.refcount = 0;
+  __pyx_pybuffernd_x_coords.data = NULL;
+  __pyx_pybuffernd_x_coords.rcbuffer = &__pyx_pybuffer_x_coords;
+  __pyx_pybuffer_y_coords.pybuffer.buf = NULL;
+  __pyx_pybuffer_y_coords.refcount = 0;
+  __pyx_pybuffernd_y_coords.data = NULL;
+  __pyx_pybuffernd_y_coords.rcbuffer = &__pyx_pybuffer_y_coords;
+  __pyx_pybuffer_z_coords.pybuffer.buf = NULL;
+  __pyx_pybuffer_z_coords.refcount = 0;
+  __pyx_pybuffernd_z_coords.data = NULL;
+  __pyx_pybuffernd_z_coords.rcbuffer = &__pyx_pybuffer_z_coords;
+  __pyx_pybuffer_occupancies.pybuffer.buf = NULL;
+  __pyx_pybuffer_occupancies.refcount = 0;
+  __pyx_pybuffernd_occupancies.data = NULL;
+  __pyx_pybuffernd_occupancies.rcbuffer = &__pyx_pybuffer_occupancies;
+  __pyx_pybuffer_b_factors.pybuffer.buf = NULL;
+  __pyx_pybuffer_b_factors.refcount = 0;
+  __pyx_pybuffernd_b_factors.data = NULL;
+  __pyx_pybuffernd_b_factors.rcbuffer = &__pyx_pybuffer_b_factors;
+  __pyx_pybuffer_atom_number.pybuffer.buf = NULL;
+  __pyx_pybuffer_atom_number.refcount = 0;
+  __pyx_pybuffernd_atom_number.data = NULL;
+  __pyx_pybuffernd_atom_number.rcbuffer = &__pyx_pybuffer_atom_number;
+  __pyx_pybuffer_residue_number.pybuffer.buf = NULL;
+  __pyx_pybuffer_residue_number.refcount = 0;
+  __pyx_pybuffernd_residue_number.data = NULL;
+  __pyx_pybuffernd_residue_number.rcbuffer = &__pyx_pybuffer_residue_number;
+  __pyx_pybuffer_model_idx.pybuffer.buf = NULL;
+  __pyx_pybuffer_model_idx.refcount = 0;
+  __pyx_pybuffernd_model_idx.data = NULL;
+  __pyx_pybuffernd_model_idx.rcbuffer = &__pyx_pybuffer_model_idx;
+  __pyx_pybuffer_record_name.pybuffer.buf = NULL;
+  __pyx_pybuffer_record_name.refcount = 0;
+  __pyx_pybuffernd_record_name.data = NULL;
+  __pyx_pybuffernd_record_name.rcbuffer = &__pyx_pybuffer_record_name;
+  __pyx_pybuffer_atom_name.pybuffer.buf = NULL;
+  __pyx_pybuffer_atom_name.refcount = 0;
+  __pyx_pybuffernd_atom_name.data = NULL;
+  __pyx_pybuffernd_atom_name.rcbuffer = &__pyx_pybuffer_atom_name;
+  __pyx_pybuffer_alt_loc.pybuffer.buf = NULL;
+  __pyx_pybuffer_alt_loc.refcount = 0;
+  __pyx_pybuffernd_alt_loc.data = NULL;
+  __pyx_pybuffernd_alt_loc.rcbuffer = &__pyx_pybuffer_alt_loc;
+  __pyx_pybuffer_residue_name.pybuffer.buf = NULL;
+  __pyx_pybuffer_residue_name.refcount = 0;
+  __pyx_pybuffernd_residue_name.data = NULL;
+  __pyx_pybuffernd_residue_name.rcbuffer = &__pyx_pybuffer_residue_name;
+  __pyx_pybuffer_chain_id.pybuffer.buf = NULL;
+  __pyx_pybuffer_chain_id.refcount = 0;
+  __pyx_pybuffernd_chain_id.data = NULL;
+  __pyx_pybuffernd_chain_id.rcbuffer = &__pyx_pybuffer_chain_id;
+  __pyx_pybuffer_insertion.pybuffer.buf = NULL;
+  __pyx_pybuffer_insertion.refcount = 0;
+  __pyx_pybuffernd_insertion.data = NULL;
+  __pyx_pybuffernd_insertion.rcbuffer = &__pyx_pybuffer_insertion;
+  __pyx_pybuffer_element_symbol.pybuffer.buf = NULL;
+  __pyx_pybuffer_element_symbol.refcount = 0;
+  __pyx_pybuffernd_element_symbol.data = NULL;
+  __pyx_pybuffernd_element_symbol.rcbuffer = &__pyx_pybuffer_element_symbol;
+  __pyx_pybuffer_charge.pybuffer.buf = NULL;
+  __pyx_pybuffer_charge.refcount = 0;
+  __pyx_pybuffernd_charge.data = NULL;
+  __pyx_pybuffernd_charge.rcbuffer = &__pyx_pybuffer_charge;
+
+  /* "cpdb/parser.pyx":165
+ * @cython.nonecheck(False)
+ * def parse_pdb_string(cnp.str input_str, int max_atoms=1000000) -> object:
+ *     cdef char *line = NULL             # <<<<<<<<<<<<<<
+ *     cdef int n_atoms = 0
+ *     cdef int i = 0
+ */
+  __pyx_v_line = NULL;
+
+  /* "cpdb/parser.pyx":166
+ * def parse_pdb_string(cnp.str input_str, int max_atoms=1000000) -> object:
+ *     cdef char *line = NULL
+ *     cdef int n_atoms = 0             # <<<<<<<<<<<<<<
+ *     cdef int i = 0
+ *     cdef int n_model = 1
+ */
+  __pyx_v_n_atoms = 0;
+
+  /* "cpdb/parser.pyx":167
+ *     cdef char *line = NULL
+ *     cdef int n_atoms = 0
+ *     cdef int i = 0             # <<<<<<<<<<<<<<
+ *     cdef int n_model = 1
+ *     cdef bytes py_bytes
+ */
+  __pyx_v_i = 0;
+
+  /* "cpdb/parser.pyx":168
+ *     cdef int n_atoms = 0
+ *     cdef int i = 0
+ *     cdef int n_model = 1             # <<<<<<<<<<<<<<
+ *     cdef bytes py_bytes
+ * 
+ */
+  __pyx_v_n_model = 1;
+
+  /* "cpdb/parser.pyx":171
+ *     cdef bytes py_bytes
+ * 
+ *     cdef AtomData *atom_data = <AtomData *> malloc(max_atoms * cython.sizeof(AtomData))             # <<<<<<<<<<<<<<
+ * 
+ *     lines = input_str.splitlines()
+ */
+  __pyx_v_atom_data = ((struct __pyx_t_4cpdb_6parser_AtomData *)malloc((__pyx_v_max_atoms * (sizeof(struct __pyx_t_4cpdb_6parser_AtomData)))));
+
+  /* "cpdb/parser.pyx":173
+ *     cdef AtomData *atom_data = <AtomData *> malloc(max_atoms * cython.sizeof(AtomData))
+ * 
+ *     lines = input_str.splitlines()             # <<<<<<<<<<<<<<
+ * 
+ *     for python_line in lines:
+ */
+  if (unlikely(__pyx_v_input_str == Py_None)) {
+    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "splitlines");
+    __PYX_ERR(0, 173, __pyx_L1_error)
+  }
+  __pyx_t_1 = PyUnicode_Splitlines(__pyx_v_input_str, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_lines = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "cpdb/parser.pyx":175
+ *     lines = input_str.splitlines()
+ * 
+ *     for python_line in lines:             # <<<<<<<<<<<<<<
+ *         py_bytes = python_line.encode('utf-8')
+ *         line = py_bytes
+ */
+  if (likely(PyList_CheckExact(__pyx_v_lines)) || PyTuple_CheckExact(__pyx_v_lines)) {
+    __pyx_t_1 = __pyx_v_lines; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_lines); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 175, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_python_line, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":176
+ * 
+ *     for python_line in lines:
+ *         py_bytes = python_line.encode('utf-8')             # <<<<<<<<<<<<<<
+ *         line = py_bytes
+ *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':
+ */
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_python_line, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_kp_u_utf_8);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_XDECREF_SET(__pyx_v_py_bytes, ((PyObject*)__pyx_t_4));
+    __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":177
+ *     for python_line in lines:
+ *         py_bytes = python_line.encode('utf-8')
+ *         line = py_bytes             # <<<<<<<<<<<<<<
+ *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':
+ *             strncpy(atom_data[n_atoms].record_type, line, 6)
+ */
+    if (unlikely(__pyx_v_py_bytes == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
+      __PYX_ERR(0, 177, __pyx_L1_error)
+    }
+    __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_py_bytes); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_v_line = __pyx_t_7;
+
+    /* "cpdb/parser.pyx":178
+ *         py_bytes = python_line.encode('utf-8')
+ *         line = py_bytes
+ *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':             # <<<<<<<<<<<<<<
+ *             strncpy(atom_data[n_atoms].record_type, line, 6)
+ *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
+ */
+    __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 4 - 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_9 = (__Pyx_PyBytes_Equals(__pyx_t_4, __pyx_n_b_ATOM, Py_EQ)); if (unlikely(__pyx_t_9 < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_10 = (__pyx_t_9 != 0);
+    if (!__pyx_t_10) {
+    } else {
+      __pyx_t_8 = __pyx_t_10;
+      goto __pyx_L6_bool_binop_done;
+    }
+    __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 6 - 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_10 = (__Pyx_PyBytes_Equals(__pyx_t_4, __pyx_n_b_HETATM, Py_EQ)); if (unlikely(__pyx_t_10 < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_9 = (__pyx_t_10 != 0);
+    __pyx_t_8 = __pyx_t_9;
+    __pyx_L6_bool_binop_done:;
+    if (__pyx_t_8) {
+
+      /* "cpdb/parser.pyx":179
+ *         line = py_bytes
+ *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':
+ *             strncpy(atom_data[n_atoms].record_type, line, 6)             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
+ * 
+ */
+      (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).record_type, __pyx_v_line, 6));
+
+      /* "cpdb/parser.pyx":180
+ *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':
+ *             strncpy(atom_data[n_atoms].record_type, line, 6)
+ *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator             # <<<<<<<<<<<<<<
+ * 
+ *             atom_data[n_atoms].atom_serial = atoi(line[6:11])
+ */
+      ((__pyx_v_atom_data[__pyx_v_n_atoms]).record_type[6]) = '\x00';
+
+      /* "cpdb/parser.pyx":182
+ *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
+ * 
+ *             atom_data[n_atoms].atom_serial = atoi(line[6:11])             # <<<<<<<<<<<<<<
+ * 
+ *             strncpy(atom_data[n_atoms].atom_name, line[12:16], 4)
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 6, 11 - 6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 182, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_11 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 182, __pyx_L1_error)
+      (__pyx_v_atom_data[__pyx_v_n_atoms]).atom_serial = atoi(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":184
+ *             atom_data[n_atoms].atom_serial = atoi(line[6:11])
+ * 
+ *             strncpy(atom_data[n_atoms].atom_name, line[12:16], 4)             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].atom_name[4] = b'\0'
+ * 
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 12, 16 - 12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 184, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_12 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 184, __pyx_L1_error)
+      (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).atom_name, __pyx_t_12, 4));
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":185
+ * 
+ *             strncpy(atom_data[n_atoms].atom_name, line[12:16], 4)
+ *             atom_data[n_atoms].atom_name[4] = b'\0'             # <<<<<<<<<<<<<<
+ * 
+ *             strncpy(atom_data[n_atoms].alt_loc, line[16:17], 1)
+ */
+      ((__pyx_v_atom_data[__pyx_v_n_atoms]).atom_name[4]) = '\x00';
+
+      /* "cpdb/parser.pyx":187
+ *             atom_data[n_atoms].atom_name[4] = b'\0'
+ * 
+ *             strncpy(atom_data[n_atoms].alt_loc, line[16:17], 1)             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].alt_loc[1] = b'\0'
+ * 
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 16, 17 - 16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_12 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L1_error)
+      (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).alt_loc, __pyx_t_12, 1));
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":188
+ * 
+ *             strncpy(atom_data[n_atoms].alt_loc, line[16:17], 1)
+ *             atom_data[n_atoms].alt_loc[1] = b'\0'             # <<<<<<<<<<<<<<
+ * 
+ *             strncpy(atom_data[n_atoms].residue_name, line[17:20], 3)
+ */
+      ((__pyx_v_atom_data[__pyx_v_n_atoms]).alt_loc[1]) = '\x00';
+
+      /* "cpdb/parser.pyx":190
+ *             atom_data[n_atoms].alt_loc[1] = b'\0'
+ * 
+ *             strncpy(atom_data[n_atoms].residue_name, line[17:20], 3)             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].residue_name[3] = b'\0'
+ * 
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 17, 20 - 17); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_12 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 190, __pyx_L1_error)
+      (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).residue_name, __pyx_t_12, 3));
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":191
+ * 
+ *             strncpy(atom_data[n_atoms].residue_name, line[17:20], 3)
+ *             atom_data[n_atoms].residue_name[3] = b'\0'             # <<<<<<<<<<<<<<
+ * 
+ *             strncpy(atom_data[n_atoms].chain_id, line[21:22], 1)
+ */
+      ((__pyx_v_atom_data[__pyx_v_n_atoms]).residue_name[3]) = '\x00';
+
+      /* "cpdb/parser.pyx":193
+ *             atom_data[n_atoms].residue_name[3] = b'\0'
+ * 
+ *             strncpy(atom_data[n_atoms].chain_id, line[21:22], 1)             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].chain_id[1] = b'\0'
+ * 
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 21, 22 - 21); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_12 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L1_error)
+      (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).chain_id, __pyx_t_12, 1));
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":194
+ * 
+ *             strncpy(atom_data[n_atoms].chain_id, line[21:22], 1)
+ *             atom_data[n_atoms].chain_id[1] = b'\0'             # <<<<<<<<<<<<<<
+ * 
+ *             atom_data[n_atoms].res_num = atoi(line[22:26])
+ */
+      ((__pyx_v_atom_data[__pyx_v_n_atoms]).chain_id[1]) = '\x00';
+
+      /* "cpdb/parser.pyx":196
+ *             atom_data[n_atoms].chain_id[1] = b'\0'
+ * 
+ *             atom_data[n_atoms].res_num = atoi(line[22:26])             # <<<<<<<<<<<<<<
+ * 
+ *             strncpy(atom_data[n_atoms].iCode, line[26:27], 1)
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 22, 26 - 22); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_11 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L1_error)
+      (__pyx_v_atom_data[__pyx_v_n_atoms]).res_num = atoi(__pyx_t_11);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":198
+ *             atom_data[n_atoms].res_num = atoi(line[22:26])
+ * 
+ *             strncpy(atom_data[n_atoms].iCode, line[26:27], 1)             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].iCode[1] = b'\0'
+ * 
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 26, 27 - 26); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_12 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L1_error)
+      (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).iCode, __pyx_t_12, 1));
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":199
+ * 
+ *             strncpy(atom_data[n_atoms].iCode, line[26:27], 1)
+ *             atom_data[n_atoms].iCode[1] = b'\0'             # <<<<<<<<<<<<<<
+ * 
+ *             atom_data[n_atoms].x = atof(line[30:38])
+ */
+      ((__pyx_v_atom_data[__pyx_v_n_atoms]).iCode[1]) = '\x00';
+
+      /* "cpdb/parser.pyx":201
+ *             atom_data[n_atoms].iCode[1] = b'\0'
+ * 
+ *             atom_data[n_atoms].x = atof(line[30:38])             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].y = atof(line[38:46])
+ *             atom_data[n_atoms].z = atof(line[46:54])
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 30, 38 - 30); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
+      (__pyx_v_atom_data[__pyx_v_n_atoms]).x = atof(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":202
+ * 
+ *             atom_data[n_atoms].x = atof(line[30:38])
+ *             atom_data[n_atoms].y = atof(line[38:46])             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].z = atof(line[46:54])
+ * 
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 38, 46 - 38); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 202, __pyx_L1_error)
+      (__pyx_v_atom_data[__pyx_v_n_atoms]).y = atof(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":203
+ *             atom_data[n_atoms].x = atof(line[30:38])
+ *             atom_data[n_atoms].y = atof(line[38:46])
+ *             atom_data[n_atoms].z = atof(line[46:54])             # <<<<<<<<<<<<<<
+ * 
+ *             atom_data[n_atoms].occupancy = atof(line[54:60])
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 46, 54 - 46); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 203, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L1_error)
+      (__pyx_v_atom_data[__pyx_v_n_atoms]).z = atof(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":205
+ *             atom_data[n_atoms].z = atof(line[46:54])
+ * 
+ *             atom_data[n_atoms].occupancy = atof(line[54:60])             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].temp_factor = atof(line[60:66])
+ * 
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 54, 60 - 54); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 205, __pyx_L1_error)
+      (__pyx_v_atom_data[__pyx_v_n_atoms]).occupancy = atof(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":206
+ * 
+ *             atom_data[n_atoms].occupancy = atof(line[54:60])
+ *             atom_data[n_atoms].temp_factor = atof(line[60:66])             # <<<<<<<<<<<<<<
+ * 
+ *             strncpy(atom_data[n_atoms].element_symbol, line[76:78], 2)
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 60, 66 - 60); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_13 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_13) && PyErr_Occurred())) __PYX_ERR(0, 206, __pyx_L1_error)
+      (__pyx_v_atom_data[__pyx_v_n_atoms]).temp_factor = atof(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":208
+ *             atom_data[n_atoms].temp_factor = atof(line[60:66])
+ * 
+ *             strncpy(atom_data[n_atoms].element_symbol, line[76:78], 2)             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].element_symbol[2] = b'\0'
+ * 
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 76, 78 - 76); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 208, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_12 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 208, __pyx_L1_error)
+      (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).element_symbol, __pyx_t_12, 2));
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":209
+ * 
+ *             strncpy(atom_data[n_atoms].element_symbol, line[76:78], 2)
+ *             atom_data[n_atoms].element_symbol[2] = b'\0'             # <<<<<<<<<<<<<<
+ * 
+ *             strncpy(atom_data[n_atoms].charge, line[78:79], 2)
+ */
+      ((__pyx_v_atom_data[__pyx_v_n_atoms]).element_symbol[2]) = '\x00';
+
+      /* "cpdb/parser.pyx":211
+ *             atom_data[n_atoms].element_symbol[2] = b'\0'
+ * 
+ *             strncpy(atom_data[n_atoms].charge, line[78:79], 2)             # <<<<<<<<<<<<<<
+ *             atom_data[n_atoms].model_idx = n_model
+ *             n_atoms += 1
+ */
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 78, 79 - 78); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_12 = __Pyx_PyBytes_AsString(__pyx_t_4); if (unlikely((!__pyx_t_12) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L1_error)
+      (void)(strncpy((__pyx_v_atom_data[__pyx_v_n_atoms]).charge, __pyx_t_12, 2));
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "cpdb/parser.pyx":212
+ * 
+ *             strncpy(atom_data[n_atoms].charge, line[78:79], 2)
+ *             atom_data[n_atoms].model_idx = n_model             # <<<<<<<<<<<<<<
+ *             n_atoms += 1
+ * 
+ */
+      (__pyx_v_atom_data[__pyx_v_n_atoms]).model_idx = __pyx_v_n_model;
+
+      /* "cpdb/parser.pyx":213
+ *             strncpy(atom_data[n_atoms].charge, line[78:79], 2)
+ *             atom_data[n_atoms].model_idx = n_model
+ *             n_atoms += 1             # <<<<<<<<<<<<<<
+ * 
+ *             if n_atoms >= max_atoms:
+ */
+      __pyx_v_n_atoms = (__pyx_v_n_atoms + 1);
+
+      /* "cpdb/parser.pyx":215
+ *             n_atoms += 1
+ * 
+ *             if n_atoms >= max_atoms:             # <<<<<<<<<<<<<<
+ *                 break
+ *         elif line[:6] == b'ENDMDL':
+ */
+      __pyx_t_8 = ((__pyx_v_n_atoms >= __pyx_v_max_atoms) != 0);
+      if (__pyx_t_8) {
+
+        /* "cpdb/parser.pyx":216
+ * 
+ *             if n_atoms >= max_atoms:
+ *                 break             # <<<<<<<<<<<<<<
+ *         elif line[:6] == b'ENDMDL':
+ *             n_model += 1
+ */
+        goto __pyx_L4_break;
+
+        /* "cpdb/parser.pyx":215
+ *             n_atoms += 1
+ * 
+ *             if n_atoms >= max_atoms:             # <<<<<<<<<<<<<<
+ *                 break
+ *         elif line[:6] == b'ENDMDL':
+ */
+      }
+
+      /* "cpdb/parser.pyx":178
+ *         py_bytes = python_line.encode('utf-8')
+ *         line = py_bytes
+ *         if line[:4] == b'ATOM' or line[:6] == b'HETATM':             # <<<<<<<<<<<<<<
+ *             strncpy(atom_data[n_atoms].record_type, line, 6)
+ *             atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
+ */
+      goto __pyx_L5;
+    }
+
+    /* "cpdb/parser.pyx":217
+ *             if n_atoms >= max_atoms:
+ *                 break
+ *         elif line[:6] == b'ENDMDL':             # <<<<<<<<<<<<<<
+ *             n_model += 1
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_line + 0, 6 - 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_8 = (__Pyx_PyBytes_Equals(__pyx_t_4, __pyx_n_b_ENDMDL, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_9 = (__pyx_t_8 != 0);
+    if (__pyx_t_9) {
+
+      /* "cpdb/parser.pyx":218
+ *                 break
+ *         elif line[:6] == b'ENDMDL':
+ *             n_model += 1             # <<<<<<<<<<<<<<
+ * 
+ *     # free(line)
+ */
+      __pyx_v_n_model = (__pyx_v_n_model + 1);
+
+      /* "cpdb/parser.pyx":217
+ *             if n_atoms >= max_atoms:
+ *                 break
+ *         elif line[:6] == b'ENDMDL':             # <<<<<<<<<<<<<<
+ *             n_model += 1
+ * 
+ */
+    }
+    __pyx_L5:;
+
+    /* "cpdb/parser.pyx":175
+ *     lines = input_str.splitlines()
+ * 
+ *     for python_line in lines:             # <<<<<<<<<<<<<<
+ *         py_bytes = python_line.encode('utf-8')
+ *         line = py_bytes
+ */
+  }
+  __pyx_L4_break:;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "cpdb/parser.pyx":223
+ * 
+ *     # Create memory view arrays
+ *     cdef cnp.ndarray[float, ndim=1] x_coords = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float32); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_14) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  __pyx_t_14 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!(likely(((__pyx_t_14) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_14, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_15 = ((PyArrayObject *)__pyx_t_14);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_x_coords.rcbuffer->pybuffer, (PyObject*)__pyx_t_15, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_x_coords = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_x_coords.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 223, __pyx_L1_error)
+    } else {__pyx_pybuffernd_x_coords.diminfo[0].strides = __pyx_pybuffernd_x_coords.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_x_coords.diminfo[0].shape = __pyx_pybuffernd_x_coords.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_15 = 0;
+  __pyx_v_x_coords = ((PyArrayObject *)__pyx_t_14);
+  __pyx_t_14 = 0;
+
+  /* "cpdb/parser.pyx":224
+ *     # Create memory view arrays
+ *     cdef cnp.ndarray[float, ndim=1] x_coords = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  __pyx_t_14 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_14);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_14);
+  __pyx_t_14 = 0;
+  __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_float32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_14); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 224, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_16 = ((PyArrayObject *)__pyx_t_6);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_y_coords.rcbuffer->pybuffer, (PyObject*)__pyx_t_16, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_y_coords = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_y_coords.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 224, __pyx_L1_error)
+    } else {__pyx_pybuffernd_y_coords.diminfo[0].strides = __pyx_pybuffernd_y_coords.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_y_coords.diminfo[0].shape = __pyx_pybuffernd_y_coords.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_16 = 0;
+  __pyx_v_y_coords = ((PyArrayObject *)__pyx_t_6);
+  __pyx_t_6 = 0;
+
+  /* "cpdb/parser.pyx":225
+ *     cdef cnp.ndarray[float, ndim=1] x_coords = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_17 = ((PyArrayObject *)__pyx_t_4);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_z_coords.rcbuffer->pybuffer, (PyObject*)__pyx_t_17, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_z_coords = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_z_coords.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 225, __pyx_L1_error)
+    } else {__pyx_pybuffernd_z_coords.diminfo[0].strides = __pyx_pybuffernd_z_coords.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_z_coords.diminfo[0].shape = __pyx_pybuffernd_z_coords.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_17 = 0;
+  __pyx_v_z_coords = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "cpdb/parser.pyx":226
+ *     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_float32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_18 = ((PyArrayObject *)__pyx_t_1);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_occupancies.rcbuffer->pybuffer, (PyObject*)__pyx_t_18, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_occupancies = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_occupancies.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 226, __pyx_L1_error)
+    } else {__pyx_pybuffernd_occupancies.diminfo[0].strides = __pyx_pybuffernd_occupancies.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_occupancies.diminfo[0].shape = __pyx_pybuffernd_occupancies.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_18 = 0;
+  __pyx_v_occupancies = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "cpdb/parser.pyx":227
+ *     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
+ *     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_float32); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_14) < 0) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  __pyx_t_14 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!(likely(((__pyx_t_14) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_14, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_19 = ((PyArrayObject *)__pyx_t_14);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_b_factors.rcbuffer->pybuffer, (PyObject*)__pyx_t_19, &__Pyx_TypeInfo_float, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_b_factors = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_b_factors.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 227, __pyx_L1_error)
+    } else {__pyx_pybuffernd_b_factors.diminfo[0].strides = __pyx_pybuffernd_b_factors.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_b_factors.diminfo[0].shape = __pyx_pybuffernd_b_factors.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_19 = 0;
+  __pyx_v_b_factors = ((PyArrayObject *)__pyx_t_14);
+  __pyx_t_14 = 0;
+
+  /* "cpdb/parser.pyx":228
+ *     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)
+ *     cdef cnp.ndarray[int, ndim=1] model_idx = np.empty(n_atoms, dtype=np.int32)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  __pyx_t_14 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_14);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_14);
+  __pyx_t_14 = 0;
+  __pyx_t_14 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_int32); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (PyDict_SetItem(__pyx_t_14, __pyx_n_s_dtype, __pyx_t_6) < 0) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_14); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_t_20 = ((PyArrayObject *)__pyx_t_6);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_atom_number.rcbuffer->pybuffer, (PyObject*)__pyx_t_20, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_atom_number = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_atom_number.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 228, __pyx_L1_error)
+    } else {__pyx_pybuffernd_atom_number.diminfo[0].strides = __pyx_pybuffernd_atom_number.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_atom_number.diminfo[0].shape = __pyx_pybuffernd_atom_number.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_20 = 0;
+  __pyx_v_atom_number = ((PyArrayObject *)__pyx_t_6);
+  __pyx_t_6 = 0;
+
+  /* "cpdb/parser.pyx":229
+ *     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
+ *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
+ *     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[int, ndim=1] model_idx = np.empty(n_atoms, dtype=np.int32)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_14 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_int32); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_t_4) < 0) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_14, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_21 = ((PyArrayObject *)__pyx_t_4);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_residue_number.rcbuffer->pybuffer, (PyObject*)__pyx_t_21, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_residue_number = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_residue_number.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 229, __pyx_L1_error)
+    } else {__pyx_pybuffernd_residue_number.diminfo[0].strides = __pyx_pybuffernd_residue_number.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_residue_number.diminfo[0].shape = __pyx_pybuffernd_residue_number.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_21 = 0;
+  __pyx_v_residue_number = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "cpdb/parser.pyx":230
+ *     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
+ *     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)
+ *     cdef cnp.ndarray[int, ndim=1] model_idx = np.empty(n_atoms, dtype=np.int32)             # <<<<<<<<<<<<<<
+ * 
+ *     # Create NumPy arrays for string columns
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_np); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_14);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_14, __pyx_n_s_int32); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_1) < 0) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 230, __pyx_L1_error)
+  __pyx_t_22 = ((PyArrayObject *)__pyx_t_1);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_model_idx.rcbuffer->pybuffer, (PyObject*)__pyx_t_22, &__Pyx_TypeInfo_int, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_model_idx = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_model_idx.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 230, __pyx_L1_error)
+    } else {__pyx_pybuffernd_model_idx.diminfo[0].strides = __pyx_pybuffernd_model_idx.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_model_idx.diminfo[0].shape = __pyx_pybuffernd_model_idx.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_22 = 0;
+  __pyx_v_model_idx = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "cpdb/parser.pyx":233
+ * 
+ *     # Create NumPy arrays for string columns
+ *     cdef cnp.ndarray[object, ndim=1] record_name = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_23 = ((PyArrayObject *)__pyx_t_6);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_record_name.rcbuffer->pybuffer, (PyObject*)__pyx_t_23, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_record_name = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_record_name.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 233, __pyx_L1_error)
+    } else {__pyx_pybuffernd_record_name.diminfo[0].strides = __pyx_pybuffernd_record_name.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_record_name.diminfo[0].shape = __pyx_pybuffernd_record_name.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_23 = 0;
+  __pyx_v_record_name = ((PyArrayObject *)__pyx_t_6);
+  __pyx_t_6 = 0;
+
+  /* "cpdb/parser.pyx":234
+ *     # Create NumPy arrays for string columns
+ *     cdef cnp.ndarray[object, ndim=1] record_name = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_24 = ((PyArrayObject *)__pyx_t_4);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_atom_name.rcbuffer->pybuffer, (PyObject*)__pyx_t_24, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_atom_name = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_atom_name.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 234, __pyx_L1_error)
+    } else {__pyx_pybuffernd_atom_name.diminfo[0].strides = __pyx_pybuffernd_atom_name.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_atom_name.diminfo[0].shape = __pyx_pybuffernd_atom_name.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_24 = 0;
+  __pyx_v_atom_name = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "cpdb/parser.pyx":235
+ *     cdef cnp.ndarray[object, ndim=1] record_name = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_25 = ((PyArrayObject *)__pyx_t_1);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_alt_loc.rcbuffer->pybuffer, (PyObject*)__pyx_t_25, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_alt_loc = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_alt_loc.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 235, __pyx_L1_error)
+    } else {__pyx_pybuffernd_alt_loc.diminfo[0].strides = __pyx_pybuffernd_alt_loc.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_alt_loc.diminfo[0].shape = __pyx_pybuffernd_alt_loc.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_25 = 0;
+  __pyx_v_alt_loc = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "cpdb/parser.pyx":236
+ *     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_26 = ((PyArrayObject *)__pyx_t_6);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_residue_name.rcbuffer->pybuffer, (PyObject*)__pyx_t_26, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_residue_name = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_residue_name.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 236, __pyx_L1_error)
+    } else {__pyx_pybuffernd_residue_name.diminfo[0].strides = __pyx_pybuffernd_residue_name.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_residue_name.diminfo[0].shape = __pyx_pybuffernd_residue_name.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_26 = 0;
+  __pyx_v_residue_name = ((PyArrayObject *)__pyx_t_6);
+  __pyx_t_6 = 0;
+
+  /* "cpdb/parser.pyx":237
+ *     cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_27 = ((PyArrayObject *)__pyx_t_4);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_chain_id.rcbuffer->pybuffer, (PyObject*)__pyx_t_27, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_chain_id = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_chain_id.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 237, __pyx_L1_error)
+    } else {__pyx_pybuffernd_chain_id.diminfo[0].strides = __pyx_pybuffernd_chain_id.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_chain_id.diminfo[0].shape = __pyx_pybuffernd_chain_id.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_27 = 0;
+  __pyx_v_chain_id = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "cpdb/parser.pyx":238
+ *     cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] charge = np.empty(n_atoms, dtype=object)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_empty); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_28 = ((PyArrayObject *)__pyx_t_1);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_insertion.rcbuffer->pybuffer, (PyObject*)__pyx_t_28, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_insertion = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_insertion.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 238, __pyx_L1_error)
+    } else {__pyx_pybuffernd_insertion.diminfo[0].strides = __pyx_pybuffernd_insertion.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_insertion.diminfo[0].shape = __pyx_pybuffernd_insertion.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_28 = 0;
+  __pyx_v_insertion = ((PyArrayObject *)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "cpdb/parser.pyx":239
+ *     cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
+ *     cdef cnp.ndarray[object, ndim=1] charge = np.empty(n_atoms, dtype=object)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_5, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!(likely(((__pyx_t_6) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_6, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_29 = ((PyArrayObject *)__pyx_t_6);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_element_symbol.rcbuffer->pybuffer, (PyObject*)__pyx_t_29, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_element_symbol = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_element_symbol.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 239, __pyx_L1_error)
+    } else {__pyx_pybuffernd_element_symbol.diminfo[0].strides = __pyx_pybuffernd_element_symbol.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_element_symbol.diminfo[0].shape = __pyx_pybuffernd_element_symbol.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_29 = 0;
+  __pyx_v_element_symbol = ((PyArrayObject *)__pyx_t_6);
+  __pyx_t_6 = 0;
+
+  /* "cpdb/parser.pyx":240
+ *     cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)
+ *     cdef cnp.ndarray[object, ndim=1] charge = np.empty(n_atoms, dtype=object)             # <<<<<<<<<<<<<<
+ * 
+ *     # Fill memory view arrays
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_np); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_empty); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_n_atoms); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_6);
+  __pyx_t_6 = 0;
+  __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_dtype, __pyx_builtin_object) < 0) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_t_30 = ((PyArrayObject *)__pyx_t_4);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_charge.rcbuffer->pybuffer, (PyObject*)__pyx_t_30, &__Pyx_TypeInfo_object, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 1, 0, __pyx_stack) == -1)) {
+      __pyx_v_charge = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_charge.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 240, __pyx_L1_error)
+    } else {__pyx_pybuffernd_charge.diminfo[0].strides = __pyx_pybuffernd_charge.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_charge.diminfo[0].shape = __pyx_pybuffernd_charge.rcbuffer->pybuffer.shape[0];
+    }
+  }
+  __pyx_t_30 = 0;
+  __pyx_v_charge = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "cpdb/parser.pyx":243
+ * 
+ *     # Fill memory view arrays
+ *     for i in range(n_atoms):             # <<<<<<<<<<<<<<
+ *         x_coords[i] = atom_data[i].x
+ *         y_coords[i] = atom_data[i].y
+ */
+  __pyx_t_31 = __pyx_v_n_atoms;
+  __pyx_t_32 = __pyx_t_31;
+  for (__pyx_t_33 = 0; __pyx_t_33 < __pyx_t_32; __pyx_t_33+=1) {
+    __pyx_v_i = __pyx_t_33;
+
+    /* "cpdb/parser.pyx":244
+ *     # Fill memory view arrays
+ *     for i in range(n_atoms):
+ *         x_coords[i] = atom_data[i].x             # <<<<<<<<<<<<<<
+ *         y_coords[i] = atom_data[i].y
+ *         z_coords[i] = atom_data[i].z
+ */
+    __pyx_t_34 = (__pyx_v_atom_data[__pyx_v_i]).x;
+    __pyx_t_35 = __pyx_v_i;
+    *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_x_coords.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_x_coords.diminfo[0].strides) = __pyx_t_34;
+
+    /* "cpdb/parser.pyx":245
+ *     for i in range(n_atoms):
+ *         x_coords[i] = atom_data[i].x
+ *         y_coords[i] = atom_data[i].y             # <<<<<<<<<<<<<<
+ *         z_coords[i] = atom_data[i].z
+ *         occupancies[i] = atom_data[i].occupancy
+ */
+    __pyx_t_34 = (__pyx_v_atom_data[__pyx_v_i]).y;
+    __pyx_t_35 = __pyx_v_i;
+    *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_y_coords.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_y_coords.diminfo[0].strides) = __pyx_t_34;
+
+    /* "cpdb/parser.pyx":246
+ *         x_coords[i] = atom_data[i].x
+ *         y_coords[i] = atom_data[i].y
+ *         z_coords[i] = atom_data[i].z             # <<<<<<<<<<<<<<
+ *         occupancies[i] = atom_data[i].occupancy
+ *         b_factors[i] = atom_data[i].temp_factor
+ */
+    __pyx_t_34 = (__pyx_v_atom_data[__pyx_v_i]).z;
+    __pyx_t_35 = __pyx_v_i;
+    *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_z_coords.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_z_coords.diminfo[0].strides) = __pyx_t_34;
+
+    /* "cpdb/parser.pyx":247
+ *         y_coords[i] = atom_data[i].y
+ *         z_coords[i] = atom_data[i].z
+ *         occupancies[i] = atom_data[i].occupancy             # <<<<<<<<<<<<<<
+ *         b_factors[i] = atom_data[i].temp_factor
+ *         model_idx[i] = atom_data[i].model_idx
+ */
+    __pyx_t_34 = (__pyx_v_atom_data[__pyx_v_i]).occupancy;
+    __pyx_t_35 = __pyx_v_i;
+    *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_occupancies.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_occupancies.diminfo[0].strides) = __pyx_t_34;
+
+    /* "cpdb/parser.pyx":248
+ *         z_coords[i] = atom_data[i].z
+ *         occupancies[i] = atom_data[i].occupancy
+ *         b_factors[i] = atom_data[i].temp_factor             # <<<<<<<<<<<<<<
+ *         model_idx[i] = atom_data[i].model_idx
+ *         atom_number[i] = atom_data[i].atom_serial
+ */
+    __pyx_t_34 = (__pyx_v_atom_data[__pyx_v_i]).temp_factor;
+    __pyx_t_35 = __pyx_v_i;
+    *__Pyx_BufPtrStrided1d(float *, __pyx_pybuffernd_b_factors.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_b_factors.diminfo[0].strides) = __pyx_t_34;
+
+    /* "cpdb/parser.pyx":249
+ *         occupancies[i] = atom_data[i].occupancy
+ *         b_factors[i] = atom_data[i].temp_factor
+ *         model_idx[i] = atom_data[i].model_idx             # <<<<<<<<<<<<<<
+ *         atom_number[i] = atom_data[i].atom_serial
+ *         residue_number[i] = atom_data[i].res_num
+ */
+    __pyx_t_36 = (__pyx_v_atom_data[__pyx_v_i]).model_idx;
+    __pyx_t_35 = __pyx_v_i;
+    *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_model_idx.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_model_idx.diminfo[0].strides) = __pyx_t_36;
+
+    /* "cpdb/parser.pyx":250
+ *         b_factors[i] = atom_data[i].temp_factor
+ *         model_idx[i] = atom_data[i].model_idx
+ *         atom_number[i] = atom_data[i].atom_serial             # <<<<<<<<<<<<<<
+ *         residue_number[i] = atom_data[i].res_num
+ * 
+ */
+    __pyx_t_36 = (__pyx_v_atom_data[__pyx_v_i]).atom_serial;
+    __pyx_t_35 = __pyx_v_i;
+    *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_atom_number.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_atom_number.diminfo[0].strides) = __pyx_t_36;
+
+    /* "cpdb/parser.pyx":251
+ *         model_idx[i] = atom_data[i].model_idx
+ *         atom_number[i] = atom_data[i].atom_serial
+ *         residue_number[i] = atom_data[i].res_num             # <<<<<<<<<<<<<<
+ * 
+ *         # Fill NumPy arrays for string columns
+ */
+    __pyx_t_36 = (__pyx_v_atom_data[__pyx_v_i]).res_num;
+    __pyx_t_35 = __pyx_v_i;
+    *__Pyx_BufPtrStrided1d(int *, __pyx_pybuffernd_residue_number.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_residue_number.diminfo[0].strides) = __pyx_t_36;
+
+    /* "cpdb/parser.pyx":254
+ * 
+ *         # Fill NumPy arrays for string columns
+ *         record_name[i] = atom_data[i].record_type[:strlen(atom_data[i].record_type)].decode('ascii', errors='replace').strip()             # <<<<<<<<<<<<<<
+ *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
+ *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
+ */
+    __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).record_type) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).record_type) - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__2, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_strip); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_1);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_35 = __pyx_v_i;
+    __pyx_t_37 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_record_name.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_record_name.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_37);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_37);
+    *__pyx_t_37 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_37);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":255
+ *         # Fill NumPy arrays for string columns
+ *         record_name[i] = atom_data[i].record_type[:strlen(atom_data[i].record_type)].decode('ascii', errors='replace').strip()
+ *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()             # <<<<<<<<<<<<<<
+ *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
+ *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
+ */
+    __pyx_t_6 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).atom_name, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).atom_name), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_strip); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 255, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_35 = __pyx_v_i;
+    __pyx_t_37 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_atom_name.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_atom_name.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_37);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_37);
+    *__pyx_t_37 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_37);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":256
+ *         record_name[i] = atom_data[i].record_type[:strlen(atom_data[i].record_type)].decode('ascii', errors='replace').strip()
+ *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
+ *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()             # <<<<<<<<<<<<<<
+ *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
+ *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
+ */
+    __pyx_t_1 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).alt_loc, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).alt_loc), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_strip); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_1);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_35 = __pyx_v_i;
+    __pyx_t_37 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_alt_loc.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_alt_loc.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_37);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_37);
+    *__pyx_t_37 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_37);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":257
+ *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
+ *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
+ *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
+ *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
+ *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
+ */
+    __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).residue_name) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).residue_name) - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 257, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_strip); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 257, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_35 = __pyx_v_i;
+    __pyx_t_37 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_residue_name.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_residue_name.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_37);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_37);
+    *__pyx_t_37 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_37);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":258
+ *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
+ *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
+ *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
+ *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
+ *         element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()
+ */
+    __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).chain_id) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).chain_id) - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__3, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_strip); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_1);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_35 = __pyx_v_i;
+    __pyx_t_37 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_chain_id.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_chain_id.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_37);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_37);
+    *__pyx_t_37 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_37);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":259
+ *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
+ *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
+ *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
+ *         element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()
+ *         charge[i] = atom_data[i].charge[:strlen(atom_data[i].charge)].decode('utf-8').strip()
+ */
+    __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).iCode) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).iCode) - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_tuple__3, __pyx_t_6); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_strip); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_35 = __pyx_v_i;
+    __pyx_t_37 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_insertion.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_insertion.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_37);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_37);
+    *__pyx_t_37 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_37);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":260
+ *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
+ *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
+ *         element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
+ *         charge[i] = atom_data[i].charge[:strlen(atom_data[i].charge)].decode('utf-8').strip()
+ * 
+ */
+    __pyx_t_6 = __Pyx_PyBytes_FromStringAndSize(((const char*)(__pyx_v_atom_data[__pyx_v_i]).element_symbol) + 0, strlen((__pyx_v_atom_data[__pyx_v_i]).element_symbol) - 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_decode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    if (PyDict_SetItem(__pyx_t_6, __pyx_n_s_errors, __pyx_n_u_replace) < 0) __PYX_ERR(0, 260, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_tuple__3, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_strip); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
+      __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_6);
+      if (likely(__pyx_t_1)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
+        __Pyx_INCREF(__pyx_t_1);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_6, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_6);
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 260, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_35 = __pyx_v_i;
+    __pyx_t_37 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_element_symbol.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_element_symbol.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_37);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_37);
+    *__pyx_t_37 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_37);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+    /* "cpdb/parser.pyx":261
+ *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
+ *         element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()
+ *         charge[i] = atom_data[i].charge[:strlen(atom_data[i].charge)].decode('utf-8').strip()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+    __pyx_t_6 = __Pyx_decode_c_string((__pyx_v_atom_data[__pyx_v_i]).charge, 0, strlen((__pyx_v_atom_data[__pyx_v_i]).charge), NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_strip); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
+      }
+    }
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 261, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_35 = __pyx_v_i;
+    __pyx_t_37 = __Pyx_BufPtrStrided1d(PyObject **, __pyx_pybuffernd_charge.rcbuffer->pybuffer.buf, __pyx_t_35, __pyx_pybuffernd_charge.diminfo[0].strides);
+    __Pyx_XGOTREF(*__pyx_t_37);
+    __Pyx_INCREF(__pyx_t_4); __Pyx_XDECREF(*__pyx_t_37);
+    *__pyx_t_37 = __pyx_t_4;
+    __Pyx_XGIVEREF(*__pyx_t_37);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  }
+
+  /* "cpdb/parser.pyx":266
+ *     # Convert the C struct data to Python objects and return
+ *     result = {
+ *         'record_name': record_name,             # <<<<<<<<<<<<<<
+ *         'atom_number': atom_number,
+ *         'atom_name': atom_name,
+ */
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(16); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_record_name, ((PyObject *)__pyx_v_record_name)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":267
+ *     result = {
+ *         'record_name': record_name,
+ *         'atom_number': atom_number,             # <<<<<<<<<<<<<<
+ *         'atom_name': atom_name,
+ *         'alt_loc': alt_loc,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_atom_number, ((PyObject *)__pyx_v_atom_number)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":268
+ *         'record_name': record_name,
+ *         'atom_number': atom_number,
+ *         'atom_name': atom_name,             # <<<<<<<<<<<<<<
+ *         'alt_loc': alt_loc,
+ *         'residue_name': residue_name,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_atom_name, ((PyObject *)__pyx_v_atom_name)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":269
+ *         'atom_number': atom_number,
+ *         'atom_name': atom_name,
+ *         'alt_loc': alt_loc,             # <<<<<<<<<<<<<<
+ *         'residue_name': residue_name,
+ *         'chain_id': chain_id,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_alt_loc, ((PyObject *)__pyx_v_alt_loc)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":270
+ *         'atom_name': atom_name,
+ *         'alt_loc': alt_loc,
+ *         'residue_name': residue_name,             # <<<<<<<<<<<<<<
+ *         'chain_id': chain_id,
+ *         'residue_number': residue_number,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_residue_name, ((PyObject *)__pyx_v_residue_name)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":271
+ *         'alt_loc': alt_loc,
+ *         'residue_name': residue_name,
+ *         'chain_id': chain_id,             # <<<<<<<<<<<<<<
+ *         'residue_number': residue_number,
+ *         "insertion": insertion,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_chain_id, ((PyObject *)__pyx_v_chain_id)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":272
+ *         'residue_name': residue_name,
+ *         'chain_id': chain_id,
+ *         'residue_number': residue_number,             # <<<<<<<<<<<<<<
+ *         "insertion": insertion,
+ *         'x_coord': x_coords,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_residue_number, ((PyObject *)__pyx_v_residue_number)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":273
+ *         'chain_id': chain_id,
+ *         'residue_number': residue_number,
+ *         "insertion": insertion,             # <<<<<<<<<<<<<<
+ *         'x_coord': x_coords,
+ *         'y_coord': y_coords,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_insertion, ((PyObject *)__pyx_v_insertion)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":274
+ *         'residue_number': residue_number,
+ *         "insertion": insertion,
+ *         'x_coord': x_coords,             # <<<<<<<<<<<<<<
+ *         'y_coord': y_coords,
+ *         'z_coord': z_coords,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_x_coord, ((PyObject *)__pyx_v_x_coords)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":275
+ *         "insertion": insertion,
+ *         'x_coord': x_coords,
+ *         'y_coord': y_coords,             # <<<<<<<<<<<<<<
+ *         'z_coord': z_coords,
+ *         'occupancy': occupancies,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_y_coord, ((PyObject *)__pyx_v_y_coords)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":276
+ *         'x_coord': x_coords,
+ *         'y_coord': y_coords,
+ *         'z_coord': z_coords,             # <<<<<<<<<<<<<<
+ *         'occupancy': occupancies,
+ *         'b_factor': b_factors,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_z_coord, ((PyObject *)__pyx_v_z_coords)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":277
+ *         'y_coord': y_coords,
+ *         'z_coord': z_coords,
+ *         'occupancy': occupancies,             # <<<<<<<<<<<<<<
+ *         'b_factor': b_factors,
+ *         'element_symbol': element_symbol,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_occupancy, ((PyObject *)__pyx_v_occupancies)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":278
+ *         'z_coord': z_coords,
+ *         'occupancy': occupancies,
+ *         'b_factor': b_factors,             # <<<<<<<<<<<<<<
+ *         'element_symbol': element_symbol,
+ *         'charge': charge,
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_b_factor, ((PyObject *)__pyx_v_b_factors)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":279
+ *         'occupancy': occupancies,
+ *         'b_factor': b_factors,
+ *         'element_symbol': element_symbol,             # <<<<<<<<<<<<<<
+ *         'charge': charge,
+ *         'model_idx': model_idx
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_element_symbol, ((PyObject *)__pyx_v_element_symbol)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":280
+ *         'b_factor': b_factors,
+ *         'element_symbol': element_symbol,
+ *         'charge': charge,             # <<<<<<<<<<<<<<
+ *         'model_idx': model_idx
+ *     }
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_charge, ((PyObject *)__pyx_v_charge)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":281
+ *         'element_symbol': element_symbol,
+ *         'charge': charge,
+ *         'model_idx': model_idx             # <<<<<<<<<<<<<<
+ *     }
+ * 
+ */
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_u_model_idx, ((PyObject *)__pyx_v_model_idx)) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_v_result = ((PyObject*)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "cpdb/parser.pyx":285
+ * 
+ *     # Free the allocated memory for the atom_data array
+ *     free(atom_data)             # <<<<<<<<<<<<<<
+ * 
+ *     return result
+ */
+  free(__pyx_v_atom_data);
+
+  /* "cpdb/parser.pyx":287
+ *     free(atom_data)
+ * 
+ *     return result             # <<<<<<<<<<<<<<
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_result);
+  __pyx_r = __pyx_v_result;
+  goto __pyx_L0;
+
+  /* "cpdb/parser.pyx":164
+ * @cython.wraparound(False)
+ * @cython.nonecheck(False)
+ * def parse_pdb_string(cnp.str input_str, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
+ *     cdef char *line = NULL
+ *     cdef int n_atoms = 0
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_14);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_alt_loc.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_atom_name.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_atom_number.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_b_factors.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_chain_id.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_charge.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_element_symbol.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_insertion.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_model_idx.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_occupancies.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_record_name.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_residue_name.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_residue_number.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_coords.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_y_coords.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z_coords.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("cpdb.parser.parse_pdb_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   goto __pyx_L2;
   __pyx_L0:;
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_alt_loc.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_atom_name.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_atom_number.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_b_factors.rcbuffer->pybuffer);
@@ -4166,14 +6338,17 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_record_name.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_residue_name.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_residue_number.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_x_coords.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_y_coords.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_z_coords.rcbuffer->pybuffer);
   __pyx_L2:;
+  __Pyx_XDECREF(__pyx_v_py_bytes);
+  __Pyx_XDECREF(__pyx_v_lines);
+  __Pyx_XDECREF(__pyx_v_python_line);
   __Pyx_XDECREF((PyObject *)__pyx_v_x_coords);
   __Pyx_XDECREF((PyObject *)__pyx_v_y_coords);
   __Pyx_XDECREF((PyObject *)__pyx_v_z_coords);
   __Pyx_XDECREF((PyObject *)__pyx_v_occupancies);
   __Pyx_XDECREF((PyObject *)__pyx_v_b_factors);
   __Pyx_XDECREF((PyObject *)__pyx_v_atom_number);
   __Pyx_XDECREF((PyObject *)__pyx_v_residue_number);
@@ -4188,15 +6363,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_charge);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4205,29 +6380,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4238,15 +6413,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4255,29 +6430,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4288,15 +6463,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4305,29 +6480,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4338,15 +6513,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4355,29 +6530,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4388,15 +6563,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4405,29 +6580,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4438,212 +6613,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":928
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":932
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":934
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":936
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":940
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4659,15 +6842,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4675,84 +6858,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":943
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4767,15 +6950,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":946
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4791,15 +6974,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4807,84 +6990,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":949
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4899,15 +7082,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":952
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4923,15 +7106,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4939,84 +7122,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":955
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":956
+      /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5031,176 +7214,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":966
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":981
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":996
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+/* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5273,46 +7456,51 @@
   {&__pyx_n_s_b_factors, __pyx_k_b_factors, sizeof(__pyx_k_b_factors), 0, 0, 1, 1},
   {&__pyx_n_s_chain_id, __pyx_k_chain_id, sizeof(__pyx_k_chain_id), 0, 0, 1, 1},
   {&__pyx_n_u_chain_id, __pyx_k_chain_id, sizeof(__pyx_k_chain_id), 0, 1, 0, 1},
   {&__pyx_n_s_charge, __pyx_k_charge, sizeof(__pyx_k_charge), 0, 0, 1, 1},
   {&__pyx_n_u_charge, __pyx_k_charge, sizeof(__pyx_k_charge), 0, 1, 0, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_cpdb_parser, __pyx_k_cpdb_parser, sizeof(__pyx_k_cpdb_parser), 0, 0, 1, 1},
-  {&__pyx_kp_s_cpdb_protein_cpdb_parser_pyx, __pyx_k_cpdb_protein_cpdb_parser_pyx, sizeof(__pyx_k_cpdb_protein_cpdb_parser_pyx), 0, 0, 1, 0},
+  {&__pyx_kp_s_cpdb_parser_pyx, __pyx_k_cpdb_parser_pyx, sizeof(__pyx_k_cpdb_parser_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_decode, __pyx_k_decode, sizeof(__pyx_k_decode), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_element_symbol, __pyx_k_element_symbol, sizeof(__pyx_k_element_symbol), 0, 0, 1, 1},
   {&__pyx_n_u_element_symbol, __pyx_k_element_symbol, sizeof(__pyx_k_element_symbol), 0, 1, 0, 1},
   {&__pyx_n_s_empty, __pyx_k_empty, sizeof(__pyx_k_empty), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_errors, __pyx_k_errors, sizeof(__pyx_k_errors), 0, 0, 1, 1},
   {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
   {&__pyx_n_s_float32, __pyx_k_float32, sizeof(__pyx_k_float32), 0, 0, 1, 1},
   {&__pyx_n_s_fp, __pyx_k_fp, sizeof(__pyx_k_fp), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+  {&__pyx_n_s_input_str, __pyx_k_input_str, sizeof(__pyx_k_input_str), 0, 0, 1, 1},
   {&__pyx_n_s_insertion, __pyx_k_insertion, sizeof(__pyx_k_insertion), 0, 0, 1, 1},
   {&__pyx_n_u_insertion, __pyx_k_insertion, sizeof(__pyx_k_insertion), 0, 1, 0, 1},
   {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_s_line, __pyx_k_line, sizeof(__pyx_k_line), 0, 0, 1, 1},
+  {&__pyx_n_s_lines, __pyx_k_lines, sizeof(__pyx_k_lines), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_max_atoms, __pyx_k_max_atoms, sizeof(__pyx_k_max_atoms), 0, 0, 1, 1},
   {&__pyx_n_s_model_idx, __pyx_k_model_idx, sizeof(__pyx_k_model_idx), 0, 0, 1, 1},
   {&__pyx_n_u_model_idx, __pyx_k_model_idx, sizeof(__pyx_k_model_idx), 0, 1, 0, 1},
   {&__pyx_n_s_n_atoms, __pyx_k_n_atoms, sizeof(__pyx_k_n_atoms), 0, 0, 1, 1},
   {&__pyx_n_s_n_model, __pyx_k_n_model, sizeof(__pyx_k_n_model), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
   {&__pyx_n_s_occupancies, __pyx_k_occupancies, sizeof(__pyx_k_occupancies), 0, 0, 1, 1},
   {&__pyx_n_u_occupancy, __pyx_k_occupancy, sizeof(__pyx_k_occupancy), 0, 1, 0, 1},
-  {&__pyx_n_s_parse_pdb, __pyx_k_parse_pdb, sizeof(__pyx_k_parse_pdb), 0, 0, 1, 1},
+  {&__pyx_n_s_parse_pdb_file, __pyx_k_parse_pdb_file, sizeof(__pyx_k_parse_pdb_file), 0, 0, 1, 1},
+  {&__pyx_n_s_parse_pdb_string, __pyx_k_parse_pdb_string, sizeof(__pyx_k_parse_pdb_string), 0, 0, 1, 1},
+  {&__pyx_n_s_py_bytes, __pyx_k_py_bytes, sizeof(__pyx_k_py_bytes), 0, 0, 1, 1},
+  {&__pyx_n_s_python_line, __pyx_k_python_line, sizeof(__pyx_k_python_line), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_record_name, __pyx_k_record_name, sizeof(__pyx_k_record_name), 0, 0, 1, 1},
   {&__pyx_n_u_record_name, __pyx_k_record_name, sizeof(__pyx_k_record_name), 0, 1, 0, 1},
   {&__pyx_n_u_replace, __pyx_k_replace, sizeof(__pyx_k_replace), 0, 1, 0, 1},
   {&__pyx_n_s_residue_name, __pyx_k_residue_name, sizeof(__pyx_k_residue_name), 0, 0, 1, 1},
   {&__pyx_n_u_residue_name, __pyx_k_residue_name, sizeof(__pyx_k_residue_name), 0, 1, 0, 1},
   {&__pyx_n_s_residue_number, __pyx_k_residue_number, sizeof(__pyx_k_residue_number), 0, 0, 1, 1},
@@ -5326,92 +7514,104 @@
   {&__pyx_n_u_y_coord, __pyx_k_y_coord, sizeof(__pyx_k_y_coord), 0, 1, 0, 1},
   {&__pyx_n_s_y_coords, __pyx_k_y_coords, sizeof(__pyx_k_y_coords), 0, 0, 1, 1},
   {&__pyx_n_u_z_coord, __pyx_k_z_coord, sizeof(__pyx_k_z_coord), 0, 1, 0, 1},
   {&__pyx_n_s_z_coords, __pyx_k_z_coords, sizeof(__pyx_k_z_coords), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 104, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 114, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 941, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "cpdb/parser.pyx":45
+  /* "cpdb/parser.pyx":46
  *     fp = fopen(filename.encode('utf-8'), "r, ccs=UTF-8")
  *     if fp == NULL:
  *         raise FileNotFoundError("Could not open file")             # <<<<<<<<<<<<<<
  * 
  *     while fgets(line, 82, fp) != NULL: # 82
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Could_not_open_file); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Could_not_open_file); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "cpdb/parser.pyx":125
+  /* "cpdb/parser.pyx":126
  * 
  *         # Fill NumPy arrays for string columns
  *         record_name[i] = atom_data[i].record_type[:strlen(atom_data[i].record_type)].decode('ascii', errors='replace').strip()             # <<<<<<<<<<<<<<
  *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
  *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_u_ascii); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_u_ascii); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "cpdb/parser.pyx":128
+  /* "cpdb/parser.pyx":129
  *         atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
  *         alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
  *         residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()             # <<<<<<<<<<<<<<
  *         chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
  *         insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_utf_8); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_utf_8); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "cpdb/parser.pyx":33
+  /* "cpdb/parser.pyx":34
  * @cython.wraparound(False)
  * @cython.nonecheck(False)
- * def parse_pdb(filename, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
+ * def parse_pdb_file(filename, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
  *     cdef FILE *fp = NULL
  *     cdef char *line = NULL
  */
-  __pyx_tuple__6 = PyTuple_Pack(25, __pyx_n_s_filename, __pyx_n_s_max_atoms, __pyx_n_s_fp, __pyx_n_s_line, __pyx_n_s_n_atoms, __pyx_n_s_i, __pyx_n_s_n_model, __pyx_n_s_atom_data, __pyx_n_s_x_coords, __pyx_n_s_y_coords, __pyx_n_s_z_coords, __pyx_n_s_occupancies, __pyx_n_s_b_factors, __pyx_n_s_atom_number, __pyx_n_s_residue_number, __pyx_n_s_model_idx, __pyx_n_s_record_name, __pyx_n_s_atom_name, __pyx_n_s_alt_loc, __pyx_n_s_residue_name, __pyx_n_s_chain_id, __pyx_n_s_insertion, __pyx_n_s_element_symbol, __pyx_n_s_charge, __pyx_n_s_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(25, __pyx_n_s_filename, __pyx_n_s_max_atoms, __pyx_n_s_fp, __pyx_n_s_line, __pyx_n_s_n_atoms, __pyx_n_s_i, __pyx_n_s_n_model, __pyx_n_s_atom_data, __pyx_n_s_x_coords, __pyx_n_s_y_coords, __pyx_n_s_z_coords, __pyx_n_s_occupancies, __pyx_n_s_b_factors, __pyx_n_s_atom_number, __pyx_n_s_residue_number, __pyx_n_s_model_idx, __pyx_n_s_record_name, __pyx_n_s_atom_name, __pyx_n_s_alt_loc, __pyx_n_s_residue_name, __pyx_n_s_chain_id, __pyx_n_s_insertion, __pyx_n_s_element_symbol, __pyx_n_s_charge, __pyx_n_s_result); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cpdb_protein_cpdb_parser_pyx, __pyx_n_s_parse_pdb, 33, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 25, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cpdb_parser_pyx, __pyx_n_s_parse_pdb_file, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 34, __pyx_L1_error)
+
+  /* "cpdb/parser.pyx":164
+ * @cython.wraparound(False)
+ * @cython.nonecheck(False)
+ * def parse_pdb_string(cnp.str input_str, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
+ *     cdef char *line = NULL
+ *     cdef int n_atoms = 0
+ */
+  __pyx_tuple__8 = PyTuple_Pack(27, __pyx_n_s_input_str, __pyx_n_s_max_atoms, __pyx_n_s_line, __pyx_n_s_n_atoms, __pyx_n_s_i, __pyx_n_s_n_model, __pyx_n_s_py_bytes, __pyx_n_s_atom_data, __pyx_n_s_lines, __pyx_n_s_python_line, __pyx_n_s_x_coords, __pyx_n_s_y_coords, __pyx_n_s_z_coords, __pyx_n_s_occupancies, __pyx_n_s_b_factors, __pyx_n_s_atom_number, __pyx_n_s_residue_number, __pyx_n_s_model_idx, __pyx_n_s_record_name, __pyx_n_s_atom_name, __pyx_n_s_alt_loc, __pyx_n_s_residue_name, __pyx_n_s_chain_id, __pyx_n_s_insertion, __pyx_n_s_element_symbol, __pyx_n_s_charge, __pyx_n_s_result); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 27, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_cpdb_parser_pyx, __pyx_n_s_parse_pdb_string, 164, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5482,25 +7682,25 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -5718,49 +7918,61 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "cpdb/parser.pyx":3
- * cimport cython
+  /* "cpdb/parser.pyx":4
  * cimport numpy as cnp
+ * 
  * import numpy as np             # <<<<<<<<<<<<<<
- * from libc.stdio cimport FILE, fopen, fclose, fgets
- * from libc.stdlib cimport malloc, free
+ * 
+ * from libc.stdint cimport uint8_t
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "cpdb/parser.pyx":33
+  /* "cpdb/parser.pyx":34
  * @cython.wraparound(False)
  * @cython.nonecheck(False)
- * def parse_pdb(filename, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
+ * def parse_pdb_file(filename, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
  *     cdef FILE *fp = NULL
  *     cdef char *line = NULL
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4cpdb_6parser_1parse_pdb, NULL, __pyx_n_s_cpdb_parser); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4cpdb_6parser_1parse_pdb_file, NULL, __pyx_n_s_cpdb_parser); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parse_pdb, __pyx_t_1) < 0) __PYX_ERR(0, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parse_pdb_file, __pyx_t_1) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "cpdb/parser.pyx":164
+ * @cython.wraparound(False)
+ * @cython.nonecheck(False)
+ * def parse_pdb_string(cnp.str input_str, int max_atoms=1000000) -> object:             # <<<<<<<<<<<<<<
+ *     cdef char *line = NULL
+ *     cdef int n_atoms = 0
+ */
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_4cpdb_6parser_3parse_pdb_string, NULL, __pyx_n_s_cpdb_parser); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parse_pdb_string, __pyx_t_1) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "cpdb/parser.pyx":1
  * cimport cython             # <<<<<<<<<<<<<<
  * cimport numpy as cnp
- * import numpy as np
+ * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../micromamba/envs/test/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../micromamba/envs/cpdb/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7142,14 +9354,75 @@
     if (decode_func) {
         return decode_func(cstring, length, errors);
     } else {
         return PyUnicode_Decode(cstring, length, encoding, errors);
     }
 }
 
+/* ArgTypeTest */
+  static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+{
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    }
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
+        name, type->tp_name, Py_TYPE(obj)->tp_name);
+    return 0;
+}
+
+/* WriteUnraisableException */
+  static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
```

### Comparing `cpdb-protein-0.1.0/cpdb/parser.pyx` & `cpdb-protein-0.2.0/cpdb/parser.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 cimport cython
 cimport numpy as cnp
+
 import numpy as np
-from libc.stdio cimport FILE, fopen, fclose, fgets
-from libc.stdlib cimport malloc, free
-from libc.stdlib cimport atof, atoi
-from libc.string cimport strncpy, strlen
+
 from libc.stdint cimport uint8_t
+from libc.stdio cimport FILE, fclose, fgets, fopen
+from libc.stdlib cimport atof, atoi, free, malloc
+from libc.string cimport strlen, strncpy
 
 
 cdef struct AtomData:
     char[7] record_type
     int atom_serial
     char[5] atom_name
     char[2] alt_loc
@@ -26,15 +27,15 @@
     char[2] charge
     int model_idx
 
 
 @cython.boundscheck(False)
 @cython.wraparound(False)
 @cython.nonecheck(False)
-def parse_pdb(filename, int max_atoms=1000000) -> object:
+def parse_pdb_file(filename, int max_atoms=1000000) -> object:
     cdef FILE *fp = NULL
     cdef char *line = NULL
     cdef int n_atoms = 0
     cdef int i = 0
     cdef int n_model =1
 
     cdef AtomData *atom_data = <AtomData *> malloc(max_atoms * cython.sizeof(AtomData))
@@ -92,14 +93,142 @@
 
     # Create memory view arrays
     cdef cnp.ndarray[float, ndim=1] x_coords = np.empty(n_atoms, dtype=np.float32)
     cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)
     cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
     cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
     cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
+    cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
+    cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)
+    cdef cnp.ndarray[int, ndim=1] model_idx = np.empty(n_atoms, dtype=np.int32)
+    
+    # Create NumPy arrays for string columns
+    cdef cnp.ndarray[object, ndim=1] record_name = np.empty(n_atoms, dtype=object)
+    cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)
+    cdef cnp.ndarray[object, ndim=1] alt_loc = np.empty(n_atoms, dtype=object)
+    cdef cnp.ndarray[object, ndim=1] residue_name = np.empty(n_atoms, dtype=object)
+    cdef cnp.ndarray[object, ndim=1] chain_id = np.empty(n_atoms, dtype=object)
+    cdef cnp.ndarray[object, ndim=1] insertion = np.empty(n_atoms, dtype=object)
+    cdef cnp.ndarray[object, ndim=1] element_symbol = np.empty(n_atoms, dtype=object)
+    cdef cnp.ndarray[object, ndim=1] charge = np.empty(n_atoms, dtype=object)
+
+    # Fill memory view arrays
+    for i in range(n_atoms):
+        x_coords[i] = atom_data[i].x
+        y_coords[i] = atom_data[i].y
+        z_coords[i] = atom_data[i].z
+        occupancies[i] = atom_data[i].occupancy
+        b_factors[i] = atom_data[i].temp_factor
+        model_idx[i] = atom_data[i].model_idx
+        atom_number[i] = atom_data[i].atom_serial
+        residue_number[i] = atom_data[i].res_num
+
+        # Fill NumPy arrays for string columns
+        record_name[i] = atom_data[i].record_type[:strlen(atom_data[i].record_type)].decode('ascii', errors='replace').strip()
+        atom_name[i] = atom_data[i].atom_name[:strlen(atom_data[i].atom_name)].decode('utf-8').strip()
+        alt_loc[i] = atom_data[i].alt_loc[:strlen(atom_data[i].alt_loc)].decode('utf-8').strip()
+        residue_name[i] = atom_data[i].residue_name[:strlen(atom_data[i].residue_name)].decode('utf-8', errors='replace').strip()
+        chain_id[i] = atom_data[i].chain_id[:strlen(atom_data[i].chain_id)].decode('utf-8', errors='replace').strip()
+        insertion[i] = atom_data[i].iCode[:strlen(atom_data[i].iCode)].decode('utf-8', errors='replace').strip()
+        element_symbol[i] = atom_data[i].element_symbol[:strlen(atom_data[i].element_symbol)].decode('utf-8', errors='replace').strip()
+        charge[i] = atom_data[i].charge[:strlen(atom_data[i].charge)].decode('utf-8').strip()
+
+
+    # Convert the C struct data to Python objects and return
+    result = {
+        'record_name': record_name,
+        'atom_number': atom_number,
+        'atom_name': atom_name,
+        'alt_loc': alt_loc,
+        'residue_name': residue_name,
+        'chain_id': chain_id,
+        'residue_number': residue_number,
+        "insertion": insertion,
+        'x_coord': x_coords,
+        'y_coord': y_coords,
+        'z_coord': z_coords,
+        'occupancy': occupancies,
+        'b_factor': b_factors,
+        'element_symbol': element_symbol,
+        'charge': charge,
+        'model_idx': model_idx
+    }
+
+    # Free the allocated memory for the atom_data array
+    free(atom_data)
+
+    return result
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+@cython.nonecheck(False)
+def parse_pdb_string(cnp.str input_str, int max_atoms=1000000) -> object:
+    cdef char *line = NULL
+    cdef int n_atoms = 0
+    cdef int i = 0
+    cdef int n_model = 1
+    cdef bytes py_bytes
+
+    cdef AtomData *atom_data = <AtomData *> malloc(max_atoms * cython.sizeof(AtomData))
+
+    lines = input_str.splitlines()
+
+    for python_line in lines:
+        py_bytes = python_line.encode('utf-8')
+        line = py_bytes
+        if line[:4] == b'ATOM' or line[:6] == b'HETATM':
+            strncpy(atom_data[n_atoms].record_type, line, 6)
+            atom_data[n_atoms].record_type[6] = b'\0' # Add Null terminator
+
+            atom_data[n_atoms].atom_serial = atoi(line[6:11])
+
+            strncpy(atom_data[n_atoms].atom_name, line[12:16], 4)
+            atom_data[n_atoms].atom_name[4] = b'\0'
+
+            strncpy(atom_data[n_atoms].alt_loc, line[16:17], 1)
+            atom_data[n_atoms].alt_loc[1] = b'\0'
+
+            strncpy(atom_data[n_atoms].residue_name, line[17:20], 3)
+            atom_data[n_atoms].residue_name[3] = b'\0'
+
+            strncpy(atom_data[n_atoms].chain_id, line[21:22], 1)
+            atom_data[n_atoms].chain_id[1] = b'\0'
+            
+            atom_data[n_atoms].res_num = atoi(line[22:26])
+            
+            strncpy(atom_data[n_atoms].iCode, line[26:27], 1)
+            atom_data[n_atoms].iCode[1] = b'\0'
+
+            atom_data[n_atoms].x = atof(line[30:38])
+            atom_data[n_atoms].y = atof(line[38:46])
+            atom_data[n_atoms].z = atof(line[46:54])
+
+            atom_data[n_atoms].occupancy = atof(line[54:60])
+            atom_data[n_atoms].temp_factor = atof(line[60:66])
+            
+            strncpy(atom_data[n_atoms].element_symbol, line[76:78], 2)
+            atom_data[n_atoms].element_symbol[2] = b'\0'
+
+            strncpy(atom_data[n_atoms].charge, line[78:79], 2)
+            atom_data[n_atoms].model_idx = n_model
+            n_atoms += 1
+
+            if n_atoms >= max_atoms:
+                break
+        elif line[:6] == b'ENDMDL':
+            n_model += 1
+
+    # free(line)
+
+    # Create memory view arrays
+    cdef cnp.ndarray[float, ndim=1] x_coords = np.empty(n_atoms, dtype=np.float32)
+    cdef cnp.ndarray[float, ndim=1] y_coords = np.empty(n_atoms, dtype=np.float32)
+    cdef cnp.ndarray[float, ndim=1] z_coords = np.empty(n_atoms, dtype=np.float32)
+    cdef cnp.ndarray[float, ndim=1] occupancies = np.empty(n_atoms, dtype=np.float32)
+    cdef cnp.ndarray[float, ndim=1] b_factors = np.empty(n_atoms, dtype=np.float32)
     cdef cnp.ndarray[int, ndim=1] atom_number = np.empty(n_atoms, dtype=np.int32)
     cdef cnp.ndarray[int, ndim=1] residue_number = np.empty(n_atoms, dtype=np.int32)
     cdef cnp.ndarray[int, ndim=1] model_idx = np.empty(n_atoms, dtype=np.int32)
     
     # Create NumPy arrays for string columns
     cdef cnp.ndarray[object, ndim=1] record_name = np.empty(n_atoms, dtype=object)
     cdef cnp.ndarray[object, ndim=1] atom_name = np.empty(n_atoms, dtype=object)
```

### Comparing `cpdb-protein-0.1.0/tests/test_similarity_to_biopandas.py` & `cpdb-protein-0.2.0/tests/test_similarity_to_biopandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pyximport
 from biopandas.pdb import PandasPdb
 from pandas.testing import assert_frame_equal
 
 pyximport.install(setup_args={
                               "include_dirs": np.get_include()},
                   reload_support=True)
-from cpdb import parse_pdb
+from cpdb import parse
 
 #from cpdb.parser import parse_pdb as parse
 
 COLUMNS_TO_CHECK = ['record_name', 'atom_number', 'atom_name', 'alt_loc',
                     'residue_name', 'chain_id', 'residue_number', 'insertion',
                     'x_coord', 'y_coord', 'z_coord', 'occupancy', 'b_factor',
                     'element_symbol']
@@ -26,15 +26,15 @@
 def test():
     TEST_FILES = os.listdir(DATA_DIR)
     print(TEST_FILES)
 
     for f in TEST_FILES:
         print(f)
         ppdb = PandasPdb().read_pdb(str(DATA_DIR / f))
-        cp = parse_pdb(str(DATA_DIR / f))
+        cp = parse(str(DATA_DIR / f))
         cp = pd.DataFrame.from_dict(cp)
         cp = cp[COLUMNS_TO_CHECK]
         print(len(cp))
 
         atom_df = ppdb.df['ATOM'][COLUMNS_TO_CHECK].reset_index(drop=True)
         print(len(atom_df))
         print(cp.record_name.value_counts())
```

