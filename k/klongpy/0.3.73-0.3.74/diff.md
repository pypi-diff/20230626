# Comparing `tmp/klongpy-0.3.73.tar.gz` & `tmp/klongpy-0.3.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klongpy-0.3.73.tar", last modified: Fri Jun 23 23:30:35 2023, max compression
+gzip compressed data, was "klongpy-0.3.74.tar", last modified: Mon Jun 26 15:15:24 2023, max compression
```

## Comparing `klongpy-0.3.73.tar` & `klongpy-0.3.74.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/
--rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.73/LICENSE
--rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 23:30:35.058063 klongpy-0.3.73/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)    10605 2023-04-13 20:55:52.000000 klongpy-0.3.73/README.md
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/klongpy/
--rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.73/klongpy/__init__.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    12840 2023-06-23 22:40:09.000000 klongpy-0.3.73/klongpy/adverbs.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2904 2023-04-13 22:28:51.000000 klongpy-0.3.73/klongpy/backend.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    27722 2023-06-23 23:29:21.000000 klongpy-0.3.73/klongpy/core.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    30746 2023-06-23 23:29:21.000000 klongpy-0.3.73/klongpy/dyads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    20414 2023-06-23 22:40:09.000000 klongpy-0.3.73/klongpy/interpreter.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    14191 2023-04-13 20:55:52.000000 klongpy-0.3.73/klongpy/monads.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11920 2023-03-12 00:53:23.000000 klongpy-0.3.73/klongpy/sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.73/klongpy/sys_var.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.73/klongpy/utils.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/klongpy.egg-info/
--rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/PKG-INFO
--rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/SOURCES.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/dependency_links.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/requires.txt
--rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-06-23 23:30:35.000000 klongpy-0.3.73/klongpy.egg-info/top_level.txt
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/scripts/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6355 2023-03-07 16:11:08.000000 klongpy-0.3.73/scripts/kgpy
--rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-06-23 23:30:35.058063 klongpy-0.3.73/setup.cfg
--rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-06-23 23:29:21.000000 klongpy-0.3.73/setup.py
-drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-23 23:30:35.058063 klongpy-0.3.73/tests/
--rw-rw-r--   0 brian     (1000) brian     (1000)     6326 2023-06-23 00:44:02.000000 klongpy-0.3.73/tests/test_accel.py
--rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.73/tests/test_examples.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    21632 2023-06-23 23:29:21.000000 klongpy-0.3.73/tests/test_extra_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2021 2023-06-23 22:40:09.000000 klongpy-0.3.73/tests/test_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     2790 2023-03-12 16:05:26.000000 klongpy-0.3.73/tests/test_interop.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3762 2023-06-23 22:40:09.000000 klongpy-0.3.73/tests/test_join_over.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.73/tests/test_prog.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.73/tests/test_suite.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.73/tests/test_suite_file.py
--rw-rw-r--   0 brian     (1000) brian     (1000)    11903 2023-03-12 00:53:23.000000 klongpy-0.3.73/tests/test_sys_fn.py
--rw-rw-r--   0 brian     (1000) brian     (1000)     7954 2022-12-08 17:42:38.000000 klongpy-0.3.73/tests/test_util.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-26 15:15:24.211805 klongpy-0.3.74/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1071 2022-07-06 22:06:17.000000 klongpy-0.3.74/LICENSE
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-26 15:15:24.211805 klongpy-0.3.74/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)    10605 2023-04-13 20:55:52.000000 klongpy-0.3.74/README.md
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-26 15:15:24.211805 klongpy-0.3.74/klongpy/
+-rw-rw-r--   0 brian     (1000) brian     (1000)       73 2022-11-28 18:56:01.000000 klongpy-0.3.74/klongpy/__init__.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    13002 2023-06-26 15:14:16.000000 klongpy-0.3.74/klongpy/adverbs.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2903 2023-06-26 15:14:16.000000 klongpy-0.3.74/klongpy/backend.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    28113 2023-06-26 15:14:16.000000 klongpy-0.3.74/klongpy/core.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    30769 2023-06-26 15:14:16.000000 klongpy-0.3.74/klongpy/dyads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    20414 2023-06-23 22:40:09.000000 klongpy-0.3.74/klongpy/interpreter.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    14191 2023-04-13 20:55:52.000000 klongpy-0.3.74/klongpy/monads.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11920 2023-03-12 00:53:23.000000 klongpy-0.3.74/klongpy/sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4322 2022-12-02 00:49:20.000000 klongpy-0.3.74/klongpy/sys_var.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      801 2022-12-11 20:11:48.000000 klongpy-0.3.74/klongpy/utils.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-26 15:15:24.211805 klongpy-0.3.74/klongpy.egg-info/
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11140 2023-06-26 15:15:24.000000 klongpy-0.3.74/klongpy.egg-info/PKG-INFO
+-rw-rw-r--   0 brian     (1000) brian     (1000)      615 2023-06-26 15:15:24.000000 klongpy-0.3.74/klongpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        1 2023-06-26 15:15:24.000000 klongpy-0.3.74/klongpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)      216 2023-06-26 15:15:24.000000 klongpy-0.3.74/klongpy.egg-info/requires.txt
+-rw-rw-r--   0 brian     (1000) brian     (1000)        8 2023-06-26 15:15:24.000000 klongpy-0.3.74/klongpy.egg-info/top_level.txt
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-26 15:15:24.211805 klongpy-0.3.74/scripts/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6592 2023-06-26 15:14:16.000000 klongpy-0.3.74/scripts/kgpy
+-rw-rw-r--   0 brian     (1000) brian     (1000)       38 2023-06-26 15:15:24.211805 klongpy-0.3.74/setup.cfg
+-rw-rw-r--   0 brian     (1000) brian     (1000)     1095 2023-06-26 15:14:16.000000 klongpy-0.3.74/setup.py
+drwxrwxr-x   0 brian     (1000) brian     (1000)        0 2023-06-26 15:15:24.211805 klongpy-0.3.74/tests/
+-rw-rw-r--   0 brian     (1000) brian     (1000)     6326 2023-06-23 00:44:02.000000 klongpy-0.3.74/tests/test_accel.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)      657 2022-12-04 18:57:44.000000 klongpy-0.3.74/tests/test_examples.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    22097 2023-06-26 15:14:16.000000 klongpy-0.3.74/tests/test_extra_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2091 2023-06-26 15:14:16.000000 klongpy-0.3.74/tests/test_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     2786 2023-06-26 15:14:16.000000 klongpy-0.3.74/tests/test_interop.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3879 2023-06-26 15:14:16.000000 klongpy-0.3.74/tests/test_join_over.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     3311 2023-03-12 00:53:23.000000 klongpy-0.3.74/tests/test_prog.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    73048 2023-03-12 00:53:23.000000 klongpy-0.3.74/tests/test_suite.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     4325 2023-03-12 00:53:23.000000 klongpy-0.3.74/tests/test_suite_file.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)    11903 2023-03-12 00:53:23.000000 klongpy-0.3.74/tests/test_sys_fn.py
+-rw-rw-r--   0 brian     (1000) brian     (1000)     7954 2022-12-08 17:42:38.000000 klongpy-0.3.74/tests/test_util.py
```

### Comparing `klongpy-0.3.73/LICENSE` & `klongpy-0.3.74/LICENSE`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/PKG-INFO` & `klongpy-0.3.74/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.73
+Version: 0.3.74
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `klongpy-0.3.73/README.md` & `klongpy-0.3.74/README.md`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/klongpy/adverbs.py` & `klongpy-0.3.74/klongpy/adverbs.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,20 +86,27 @@
 
         Example: -'[1 2 3]  -->  [-1 -2 -3]
 
     """
     if isinstance(a,str):
         if is_empty(a):
             return a
-        r = np.asarray([f(x) for x in str_to_chr_arr(a)])
-        return ''.join(r) if r.dtype == '<U1' else r
+        has_str = False
+        r = []
+        for x in str_to_chr_arr(a):
+            u = f(x)
+            has_str |= isinstance(u,str)
+            r.append(u)
+        return ''.join(r) if has_str else safe_asarray(r)
     if is_iterable(a):
-        return a if is_empty(a) else np.asarray([f(x) for x in a])
+        r = [f(x) for x in a]
+        return a if is_empty(a) else safe_asarray(r)
     elif is_dict(a):
-        return np.asarray([f(np.asarray(x)) for x in a.items()])
+        r = [f(np.asarray(x)) for x in a.items()]
+        return safe_asarray(r)
     return f(a)
 
 
 def eval_adverb_each2(f, a, b):
     """
 
         a f'b                                                   [Each-2]
@@ -297,18 +304,19 @@
                   0,\[1 2 3]  -->  [0 [0 1] [0 1 2] [0 1 2 3]]
     """
     if is_empty(b):
         return a
     if is_atom(b):
         b = [b]
     b = [f(a,b[0]), *b[1:]]
-    q = np.asarray(list(itertools.accumulate(b,f)))
+    r = list(itertools.accumulate(b,f))
+    q = safe_asarray(r)
     r = [a, *q]
     try:
-        return np.asarray(r)
+        return safe_asarray(r)
     except ValueError:
         return cast_malformed_array(r)
 
 
 def eval_adverb_scan_over(f, a, op):
     """
         see eval_adverb_scan_over_neutral
@@ -322,15 +330,15 @@
         return np.subtract.accumulate(a)
     elif safe_eq(f, eval_dyad_multiply) and hasattr(np.multiple, 'accumulate'):
         return np.multiple.accumulate(a)
     elif safe_eq(f, eval_dyad_divide) and hasattr(np.divide, 'accumulate'):
         return np.divide.accumulate(a)
     r = list(itertools.accumulate(a, f))
     try:
-        return np.asarray(r)
+        return safe_asarray(r)
     except ValueError:
         return cast_malformed_array(r)
 
 
 def eval_adverb_scan_converging(f, a, op):
     """
 
@@ -356,15 +364,15 @@
     r = [a, xx]
     while not array_equal(x,xx):
         x = xx
         xx = f(x)
         r.append(xx)
     r.pop()
     try:
-        return np.asarray(r)
+        return safe_asarray(r)
     except ValueError:
         return cast_malformed_array(r)
 
 
 def eval_adverb_scan_while(klong, f, a, b):
     """
 
@@ -387,15 +395,15 @@
     r = [b]
     # TODO: fix arity
     while klong.eval(KGCall(a, b, arity=1)):
         b = f(b)
         r.append(b)
     r.pop()
     try:
-        return np.asarray(r)
+        return safe_asarray(r)
     except ValueError:
         return cast_malformed_array(r)
 
 
 def eval_adverb_scan_iterating(f, a, b):
     """
 
@@ -411,15 +419,15 @@
         return b
     r = [b]
     while not safe_eq(a, 0):
         b = f(b)
         r.append(b)
         a = a - 1
     try:
-        return np.asarray(r)
+        return safe_asarray(r)
     except ValueError:
         return cast_malformed_array(r)
 
 
 def eval_adverb_while(klong, f, a, b):
     """
```

### Comparing `klongpy-0.3.73/klongpy/backend.py` & `klongpy-0.3.74/klongpy/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,11 +93,11 @@
     np.divide = CuPyReductionKernelWrapper(cupy.divide, divide_reduce_1, divide_reduce_2)
 
     np.isarray = lambda x: isinstance(x, (numpy.ndarray, cupy.ndarray))
 
 #    np.hstack = lambda x: cupy.hstack(x) if use_gpu and is_supported_type(x) else numpy.hstack(x)
 else:
     np.seterr(divide='ignore')
-    warnings.filterwarnings("ignore", category=np.VisibleDeprecationWarning)
+    warnings.filterwarnings("error", category=np.VisibleDeprecationWarning)
     np.isarray = lambda x: isinstance(x, np.ndarray)
 
 np
```

### Comparing `klongpy-0.3.73/klongpy/core.py` & `klongpy-0.3.74/klongpy/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,28 @@
 def in_map(x, v):
     try:
         return x in v
     except Exception:
         return False
 
 
+def safe_asarray(a):
+    """
+    Attempt to create a NumPy array, but if it's jagged then we default to object dtype
+    
+    Note: it is way faster to do it this way vs checking in advance since the detection
+    happens in NumPy vs Python.
+    """
+    try:
+        arr = np.asarray(a)
+    except (np.VisibleDeprecationWarning, ValueError):
+        arr = np.asarray(a,dtype=object)
+    return arr
+
+
 def array_equal(a, b):
     """
     Recursively determine if two values or arrays are equal.
 
     NumPy ops (e.g. array_equal) are not sufficiently general purpose for this, so we need our own.
     """
     if is_list(a):
@@ -588,16 +602,16 @@
         if safe_eq(q, '['):
             i,q = read_list(t, ']', i=i, module=module)
         arr.append(q)
         i = skip(t,i,ignore_newline=True)
     if cmatch(t,i,delim):
         i += 1
     try:
-        aa = np.asarray(arr)
-        if aa.dtype.kind != 'i' and aa.dtype.kind != 'f':
+        aa = safe_asarray(arr)
+        if aa.dtype.kind not in ['O','i','f']:
             aa = np.asarray(arr, dtype=object)
         return i, aa
     except ValueError:
         return i,cast_malformed_array(arr)
 
 
 def read_string(t, i=0):
```

### Comparing `klongpy-0.3.73/klongpy/dyads.py` & `klongpy-0.3.74/klongpy/dyads.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                     r[i] = b[0]
         return "".join(["".join(x) for x in r])
     r = np.array(a) # clone
     if is_list(b[0]): # TOOD: use np.put if we can
         r = r.tolist()
         for i in b[1:]:
             r[i] = b[0]
-        r = np.asarray(r)
+        r = safe_asarray(r)
     else:
         np.put(r, np.asarray(b[1:],dtype=int), b[0])
     return r
 
 
 def eval_dyad_amend_in_depth(a, b):
     """
@@ -128,15 +128,15 @@
     """
     j = isinstance(b, str)
     b = np.asarray(str_to_chr_arr(b) if j else b)
     a = a if np.isarray(a) else [a]
     r = np.array_split(b, a)
     if len(b) == 0 and len(a) > 0:
         r = r[1:]
-    return np.asarray(["".join(x) for x in r]) if j else np.asarray(r)
+    return np.asarray(["".join(x) for x in r]) if j else safe_asarray(r)
 
 
 def eval_dyad_at_index(klong, a, b):
     """
 
         a@b                                                   [At/Index]
         a@b                                                   [At/Apply]
@@ -517,15 +517,15 @@
         if len(a.shape) == len(b.shape) and a.shape[-1] == b.shape[-1]:
             return np.concatenate((a,b))
 
     aa = dyad_join_to_list(a)
     bb = dyad_join_to_list(b)
  
     r = [*aa,*bb]
-    nr = np.asarray(r)
+    nr = safe_asarray(r)
     t = nr.dtype.type
     return nr if issubclass(t, np.integer) or issubclass(t, np.floating) else np.asarray(r,dtype=object)
 
 
 def eval_dyad_less(a, b):
     """
 
@@ -791,27 +791,27 @@
                 r = np.asarray(["".join(x) for x in r]) if j else r
                 j = False
             elif a_s == b_s:
                 r = b.reshape(a)
             else:
                 r = np.resize(b, a)
         else:
-            r = np.ones(a)*b
+            r = np.full(a, b)
     else:
         if a == 0:
             r = b
         elif np.isarray(b):
             if a < b.shape[0]:
                 r = np.resize(b, (a,))
             else:
                 ns = np.ones(len(b.shape),dtype=int)
                 ns[0] = a // b.shape[0]
                 r = np.concatenate((np.tile(b,ns), b[:a - b.shape[0]*ns[0]]))
         else:
-            r = np.ones((a,))*b
+            r = np.full((a,), b)
     return "".join(r) if j else r
 
 
 def eval_dyad_rotate(a, b):
     """
 
         a:+b                                                    [Rotate]
@@ -882,15 +882,15 @@
         while q < len(b):
             r.append(b[q:q+a[p]])
             q += a[p]
             p += 1
             if p >= len(a):
                 p = 0
 
-    return np.asarray(["".join(x) for x in r]) if j else np.asarray(r)
+    return np.asarray(["".join(x) for x in r],dtype=object) if j else safe_asarray(r)
 
 
 def eval_dyad_subtract(a, b):
     """
 
         a-b                                                      [Minus]
```

### Comparing `klongpy-0.3.73/klongpy/interpreter.py` & `klongpy-0.3.74/klongpy/interpreter.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/klongpy/monads.py` & `klongpy-0.3.74/klongpy/monads.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/klongpy/sys_fn.py` & `klongpy-0.3.74/klongpy/sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/klongpy/sys_var.py` & `klongpy-0.3.74/klongpy/sys_var.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/klongpy/utils.py` & `klongpy-0.3.74/klongpy/utils.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/klongpy.egg-info/PKG-INFO` & `klongpy-0.3.74/klongpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klongpy
-Version: 0.3.73
+Version: 0.3.74
 Summary: Python implementation of Klong language.
 Author: Brian Guarraci
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `klongpy-0.3.73/klongpy.egg-info/SOURCES.txt` & `klongpy-0.3.74/klongpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/scripts/kgpy` & `klongpy-0.3.74/scripts/kgpy`

 * *Files 5% similar despite different names*

```diff
@@ -204,30 +204,38 @@
             print(failure("\nkg: error: interrupted"))
         except Exception as e:
             print(failure(f"Error: {e.args}"))
             import traceback
             traceback.print_exc(e)
 
 
+def run_file(fname):
+    with open(fname, "r") as f:
+        return klong(f.read())
+
+
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
-        prog = 'KlongPy',
-        description = 'KlongPy REPL',
-        epilog = 'For help, go to https://github.com/briangu/klongpy"')
+        prog='KlongPy',
+        description='KlongPy REPL',
+        epilog='For help, go to https://github.com/briangu/klongpy')
     parser.add_argument('-e', '--expr', help='evaluate expression, no interactive mode')
     parser.add_argument('-l', '--load', help='load program from file')
     parser.add_argument('-p', '--run', help='run program from file')
     parser.add_argument('-t', '--test', help='test program from file')
+    parser.add_argument('filename', nargs='?', help='filename to be run if no flags are specified')
 
     args = parser.parse_args()
+
     if args.expr:
         print(KlongInterpreter()(args.expr))
         exit()
 
     klong = KlongInterpreter()
+
     if args.load:
         print(f"Loading: {args.load}")
         with open(args.load, "r") as f:
             klong(f.read())
         repl(klong)
     elif args.run:
         print(f"Running: {args.run}")
@@ -238,9 +246,11 @@
         with open(args.test, "r") as f:
             for x in f.readlines():
                 x = x.strip()
                 if len(x) == 0 or x.startswith(":"):
                     continue
                 print(x)
                 klong(x)
+    elif args.filename:
+        run_file(args.filename)
     else:
         repl()
```

### Comparing `klongpy-0.3.73/setup.py` & `klongpy-0.3.74/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 
 setup(
     name='klongpy',
     packages=['klongpy'],
-    version='0.3.73',
+    version='0.3.74',
     description='Python implementation of Klong language.',
     author='Brian Guarraci',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
-    install_requires=['numpy~=1.23.0'],
+    install_requires=['numpy~=1.24.0'],
     python_requires='>=3.8',
     extras_require={
         'cupy': ["cupy"],
         'cuda12x': ["cupy-cuda12x"],
         'cuda11x': ["cupy-cuda11x"],
         'cuda111': ["cupy-cuda111"],
         'cuda110': ["cupy-cuda110"],
```

### Comparing `klongpy-0.3.73/tests/test_accel.py` & `klongpy-0.3.74/tests/test_accel.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/tests/test_examples.py` & `klongpy-0.3.74/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/tests/test_extra_suite.py` & `klongpy-0.3.74/tests/test_extra_suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,30 +9,40 @@
 
 # add tests not included in the original kg suite
 class TestExtraCoreSuite(unittest.TestCase):
 
     def assert_eval_cmp(self, a, b, klong=None):
         self.assertTrue(eval_cmp(a, b, klong=klong))
 
+    def test_jagged_array_each(self):
+        klong = KlongInterpreter()
+        r = klong("""{:[x!2;[1];[1 2]]}'[1 2 3]""")
+        self.assertTrue(array_equal(r, np.array([[1],[1,2],[1]],dtype=object)))
+
+    def test_jagged_dict_each(self):
+        klong = KlongInterpreter()
+        r = klong("""{:[(x@0)!2;[1];[1 2]]}':{[1 2] [2 3] [3 4]}""")
+        self.assertTrue(array_equal(r, np.array([[1],[1,2],[1]],dtype=object)))
+
     def test_power(self):
         klong = KlongInterpreter()
         r = klong('[1 2 3]^2')
         self.assertTrue(array_equal(r, np.array([1,4,9])))
 
     def test_dyad_join_mixed_types(self):
         klong = KlongInterpreter()
         r = klong(',/["a" [1]]')
-        self.assertTrue(array_equal(r, np.array(['a', 1], dtype='object')))
+        self.assertTrue(array_equal(r, np.array(['a', 1], dtype=object)))
 
     def test_dyad_join_nested_array(self):
         klong = KlongInterpreter()
         r = klong('[1],[[2 3]]')
-        self.assertTrue(array_equal(r, np.array([1,[2,3]])))
+        self.assertTrue(array_equal(r, np.array([1,[2,3]],dtype=object)))
         r = klong(',/[0 [[1] [2]]]')
-        self.assertTrue(array_equal(r, np.array([0,[1],[2]])))
+        self.assertTrue(array_equal(r, np.array([0,[1],[2]],dtype=object)))
 
     @unittest.skip
     def test_dict_inner_create_syntax(self):
         klong = KlongInterpreter()
         with self.assertRaises(RuntimeError):
             # should fail to parse
             r = klong(":{[1 :{[2 3]}}")
@@ -637,15 +647,15 @@
     def test_scan_converge(self):
         klong = KlongInterpreter()
         r = klong('{(x+2%x)%2}\~2')
         e = np.asarray([2.        , 1.5       , 1.41666667, 1.41421569])
         self.assertTrue(np.isclose(r,e).all())
 
         r = klong(',/\~["a" ["b"] "c"]')
-        e = np.asarray([["a",["b"],"c"],["a","b","c"],"abc"])
+        e = np.asarray([["a",["b"],"c"],["a","b","c"],"abc"],dtype=object)
         x = r
         self.assertTrue(rec_flatten(rec_fn2(e,x, lambda a,b: a == b)).all())
 
     def test_converge_as_fn(self):
         klong = KlongInterpreter()
         klong('s::{(x+2%x)%2}:~2')
         r = klong('s')
```

### Comparing `klongpy-0.3.73/tests/test_fn.py` & `klongpy-0.3.74/tests/test_fn.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,9 +63,11 @@
         klong = KlongInterpreter()
         with open("tests/klong_fn.kg", "r") as f:
             klong(f.read())
             r = klong('err')
             self.assertEqual(r, 0)
 
 if __name__ == "__main__":
-    run_suite_file("klong_join_over.kg")
+    import timeit
+    print(timeit.timeit('run_suite_file("klong_fn.kg")', number=10, globals=locals()) / 10)
+
```

### Comparing `klongpy-0.3.73/tests/test_interop.py` & `klongpy-0.3.74/tests/test_interop.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,31 +53,31 @@
         r = klong['fn']([2])
         self.assertTrue(array_equal(r, [12]))
 
     def test_datetime_parsing_example(self):
         klong = KlongInterpreter()
         klong['strptime'] = lambda x: datetime.strptime(x, "%d %B, %Y")
         r = klong('a::strptime("21 June, 2018")')
-        self.assertEquals(r, datetime(2018, 6, 21, 0, 0))
+        self.assertEqual(r, datetime(2018, 6, 21, 0, 0))
         r = klong['a']
-        self.assertEquals(r, datetime(2018, 6, 21, 0, 0))
+        self.assertEqual(r, datetime(2018, 6, 21, 0, 0))
         r = klong('d:::{};d,"timestamp",a')
         self.assertEqual(r, {'timestamp': datetime(2018, 6, 21, 0, 0)})
 
     def test_datetime_parsing_example_one_call(self):
         # run everything in one go
         klong = KlongInterpreter()
         klong['strptime'] = lambda x: datetime.strptime(x, "%d %B, %Y")
         r = klong("""a::strptime("21 June, 2018");d:::{};d,"timestamp",a""")
         self.assertEqual(r, {'timestamp': datetime(2018, 6, 21, 0, 0)})
         r = klong['a']
-        self.assertEquals(r, datetime(2018, 6, 21, 0, 0))
+        self.assertEqual(r, datetime(2018, 6, 21, 0, 0))
 
     def test_callback_into_assertion(self):
         def assert_date(x):
             self.assertEqual(x, {'timestamp': datetime(2018, 6, 21, 0, 0)})
             return 42
         klong = KlongInterpreter()
         klong['strptime'] = lambda x: datetime.strptime(x, "%d %B, %Y")
         klong['assert'] = assert_date
         r = klong("""a::strptime("21 June, 2018");d:::{};d,"timestamp",a;assert(d)""")
-        self.assertEquals(r, 42)
+        self.assertEqual(r, 42)
```

### Comparing `klongpy-0.3.73/tests/test_join_over.py` & `klongpy-0.3.74/tests/test_join_over.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,35 +47,35 @@
         klong = KlongInterpreter()
         r = klong(",/[[[[1 2] [3 4]] [[5 6] [7 8]]] [[[9 10] [11 12]] [[13 14] [15 16]]]]")
         self.assertTrue(array_equal(r, np.array([[[1,2],[3,4]], [[5,6],[7,8]], [[9,10],[11,12]], [[13,14],[15,16]]])))
 
     def test_mixed_dim_arrays(self):
         klong = KlongInterpreter()
         r = klong(",/[[[1 2] [3 4]] [[5 6] [7]]]")
-        self.assertTrue(array_equal(r, np.array([[1,2],[3,4],[5,6],[7]])))
+        self.assertTrue(array_equal(r, np.array([[1,2],[3,4],[5,6],[7]],dtype=object)))
         r = klong(",/[[[1] [2] [3 4]] [[5] [6] [7]]]")
-        self.assertTrue(array_equal(r, np.array([[1],[2],[3,4],[5],[6],[7]])))
+        self.assertTrue(array_equal(r, np.array([[1],[2],[3,4],[5],[6],[7]],dtype=object)))
         r = klong(",/[[1] [[2 3]] 4]")
-        self.assertTrue(array_equal(r, np.array([1, [2, 3], 4], dtype='object')))
+        self.assertTrue(array_equal(r, np.array([1, [2, 3], 4], dtype=object)))
         r = klong(",/[[] [] [[]]]")
         self.assertTrue(array_equal(r, np.array([[]])))
 
     def test_string_elements(self): 
         klong = KlongInterpreter()
         r = klong(',/[["a" "b"] ["c" "d"]]')
         self.assertTrue(array_equal(r, np.array(['a', 'b', 'c', 'd'])))
 
     def test_mixed_elements(self):
         klong = KlongInterpreter()
         r = klong(',/[[1 "a"] ["b" 2]]')
-        self.assertTrue(array_equal(r, np.array([1, 'a', 'b', 2], dtype='object')))
+        self.assertTrue(array_equal(r, np.array([1, 'a', 'b', 2], dtype=object)))
         r = klong(',/[["a"] [1]]')
-        self.assertTrue(array_equal(r, np.array(['a', 1], dtype='object')))
+        self.assertTrue(array_equal(r, np.array(['a', 1], dtype=object)))
         r = klong(',/["a" [1]]')
-        self.assertTrue(array_equal(r, np.array(['a', 1], dtype='object')))
+        self.assertTrue(array_equal(r, np.array(['a', 1], dtype=object)))
 
     def test_file_by_lines(self):
         """
         Test the suite file line by line using our own t()
         """
         klong = create_test_klong()
         with open("tests/klong_join_over.kg", "r") as f:
@@ -98,10 +98,11 @@
         """
         Test the entire suite file.
         """
         self.assertEqual(run_suite_file('klong_join_over.kg'), 0)
 
 
 if __name__ == "__main__":
-    run_suite_file("klong_join_over.kg")
-
+    import timeit
+    number = 10
+    print(timeit.timeit('run_suite_file("klong_join_over.kg")', number=number, globals=locals()) / number)
```

### Comparing `klongpy-0.3.73/tests/test_prog.py` & `klongpy-0.3.74/tests/test_prog.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/tests/test_suite.py` & `klongpy-0.3.74/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/tests/test_suite_file.py` & `klongpy-0.3.74/tests/test_suite_file.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/tests/test_sys_fn.py` & `klongpy-0.3.74/tests/test_sys_fn.py`

 * *Files identical despite different names*

### Comparing `klongpy-0.3.73/tests/test_util.py` & `klongpy-0.3.74/tests/test_util.py`

 * *Files identical despite different names*

