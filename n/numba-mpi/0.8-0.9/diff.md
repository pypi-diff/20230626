# Comparing `tmp/numba-mpi-0.8.tar.gz` & `tmp/numba-mpi-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba-mpi-0.8.tar", last modified: Wed Aug 24 13:27:44 2022, max compression
+gzip compressed data, was "numba-mpi-0.9.tar", last modified: Thu Aug 25 12:21:09 2022, max compression
```

## Comparing `numba-mpi-0.8.tar` & `numba-mpi-0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 13:27:44.863967 numba-mpi-0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 13:27:44.859966 numba-mpi-0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 13:27:44.863967 numba-mpi-0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-08-24 13:27:27.000000 numba-mpi-0.8/.github/workflows/pdoc.yml
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-08-24 13:27:27.000000 numba-mpi-0.8/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-08-24 13:27:27.000000 numba-mpi-0.8/.github/workflows/readme.yml
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-08-24 13:27:27.000000 numba-mpi-0.8/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-08-24 13:27:27.000000 numba-mpi-0.8/.github/workflows/tests+artifacts+pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-08-24 13:27:27.000000 numba-mpi-0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-24 13:27:27.000000 numba-mpi-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-08-24 13:27:44.863967 numba-mpi-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-08-24 13:27:27.000000 numba-mpi-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 13:27:44.863967 numba-mpi-0.8/numba_mpi/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-24 13:27:27.000000 numba-mpi-0.8/numba_mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4708 2022-08-24 13:27:27.000000 numba-mpi-0.8/numba_mpi/mpi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 13:27:44.863967 numba-mpi-0.8/numba_mpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-08-24 13:27:44.000000 numba-mpi-0.8/numba_mpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      414 2022-08-24 13:27:44.000000 numba-mpi-0.8/numba_mpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 13:27:44.000000 numba-mpi-0.8/numba_mpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-24 13:27:44.000000 numba-mpi-0.8/numba_mpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-24 13:27:44.000000 numba-mpi-0.8/numba_mpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 13:27:44.863967 numba-mpi-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-08-24 13:27:27.000000 numba-mpi-0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 13:27:44.863967 numba-mpi-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2536 2022-08-24 13:27:27.000000 numba-mpi-0.8/tests/test_mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 12:21:09.001228 numba-mpi-0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 12:21:08.997228 numba-mpi-0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 12:21:08.997228 numba-mpi-0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-08-25 12:20:52.000000 numba-mpi-0.9/.github/workflows/pdoc.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-08-25 12:20:52.000000 numba-mpi-0.9/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-08-25 12:20:52.000000 numba-mpi-0.9/.github/workflows/readme.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      717 2022-08-25 12:20:52.000000 numba-mpi-0.9/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-08-25 12:20:52.000000 numba-mpi-0.9/.github/workflows/tests+artifacts+pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-08-25 12:20:52.000000 numba-mpi-0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-08-25 12:20:52.000000 numba-mpi-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-08-25 12:21:09.001228 numba-mpi-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2187 2022-08-25 12:20:52.000000 numba-mpi-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 12:21:08.997228 numba-mpi-0.9/numba_mpi/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-25 12:20:52.000000 numba-mpi-0.9/numba_mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5562 2022-08-25 12:20:52.000000 numba-mpi-0.9/numba_mpi/mpi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 12:21:09.001228 numba-mpi-0.9/numba_mpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-08-25 12:21:08.000000 numba-mpi-0.9/numba_mpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      414 2022-08-25 12:21:08.000000 numba-mpi-0.9/numba_mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 12:21:08.000000 numba-mpi-0.9/numba_mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-25 12:21:08.000000 numba-mpi-0.9/numba_mpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-08-25 12:21:08.000000 numba-mpi-0.9/numba_mpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-25 12:21:09.001228 numba-mpi-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-08-25 12:20:52.000000 numba-mpi-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 12:21:09.001228 numba-mpi-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-08-25 12:20:52.000000 numba-mpi-0.9/tests/test_mpi.py
```

### Comparing `numba-mpi-0.8/.github/workflows/pdoc.yml` & `numba-mpi-0.9/.github/workflows/pdoc.yml`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/.github/workflows/pylint.yml` & `numba-mpi-0.9/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/.github/workflows/readme.yml` & `numba-mpi-0.9/.github/workflows/readme.yml`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/.github/workflows/stale.yml` & `numba-mpi-0.9/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/.github/workflows/tests+artifacts+pypi.yml` & `numba-mpi-0.9/.github/workflows/tests+artifacts+pypi.yml`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/.gitignore` & `numba-mpi-0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/LICENSE` & `numba-mpi-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/PKG-INFO` & `numba-mpi-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-mpi
-Version: 0.8
+Version: 0.9
 Summary: Numba @njittable MPI wrappers tested on Linux, macOS and Windows
 Home-page: https://github.com/atmos-cloud-sim-uj/numba-mpi
 Author: https://github.com/atmos-cloud-sim-uj/numba-mpi/graphs/contributors
 License: GPL v3
 Project-URL: Tracker, https://github.com/atmos-cloud-sim-uj/numba-mpi/issues
 Project-URL: Documentation, https://atmos-cloud-sim-uj.github.io/numba-mpi
 Project-URL: Source, https://github.com/atmos-cloud-sim-uj/numba-mpi
```

### Comparing `numba-mpi-0.8/README.md` & `numba-mpi-0.9/README.md`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/numba_mpi/mpi.py` & `numba-mpi-0.9/numba_mpi/mpi.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,19 +39,26 @@
 _MPI_Comm_size.restype = ctypes.c_int
 _MPI_Comm_size.argtypes = [_MpiComm, ctypes.c_void_p]
 
 _MPI_Comm_rank = libmpi.MPI_Comm_rank
 _MPI_Comm_rank.restype = ctypes.c_int
 _MPI_Comm_rank.argtypes = [_MpiComm, ctypes.c_void_p]
 
-# pylint: disable-next=protected-access
+# pylint: disable=protected-access
 _MPI_Comm_World_ptr = MPI._addressof(MPI.COMM_WORLD)
 
-# pylint: disable-next=protected-access
-_MPI_Double_ptr = MPI._addressof(MPI.DOUBLE)
+_MPI_DTYPES = {
+    np.dtype("int32"): MPI._addressof(MPI.INT32_T),
+    np.dtype("int64"): MPI._addressof(MPI.INT64_T),
+    np.dtype("float"): MPI._addressof(MPI.FLOAT),
+    np.dtype("double"): MPI._addressof(MPI.DOUBLE),
+    np.dtype("complex64"): MPI._addressof(MPI.C_FLOAT_COMPLEX),
+    np.dtype("complex128"): MPI._addressof(MPI.C_DOUBLE_COMPLEX)
+}
+# pylint: enable=protected-access
 
 _MPI_Send = libmpi.MPI_Send
 _MPI_Send.restype = ctypes.c_int
 _MPI_Send.argtypes = [
     ctypes.c_void_p,
     ctypes.c_int,
     _MpiDatatype,
@@ -85,28 +92,46 @@
             _address_as_void_pointer(_MPI_Comm_World_ptr),
             shape=(1,),
             dtype=np.intp
         )[0]
     return impl
 
 
-def _mpi_double():
-    return _MpiDatatype.from_address(_MPI_Double_ptr)
+def _get_dtype_numpy_to_mpi_ptr(arr):
+    for np_dtype, mpi_ptr in _MPI_DTYPES.items():
+        if np.can_cast(arr.dtype, np_dtype, casting="equiv"):
+            return mpi_ptr
+    raise NotImplementedError(f"Type: {arr.dtype}")
 
-# WIN DOUBLE - 0x4c00080b
 
-@numba.extending.overload(_mpi_double)
-def _mpi_double_njit():
-    def impl():
+def _get_dtype_numba_to_mpi_ptr(arr):
+    for np_dtype, mpi_ptr in _MPI_DTYPES.items():
+        if arr.dtype == numba.from_dtype(np_dtype):
+            return mpi_ptr
+    raise NotImplementedError(f"Type: {arr.dtype}")
+
+
+def _mpi_dtype(arr):
+    ptr = _get_dtype_numpy_to_mpi_ptr(arr)
+    return _MpiDatatype.from_address(ptr)
+
+
+@numba.extending.overload(_mpi_dtype)
+def _mpi_dtype_njit(arr):
+    mpi_dtype = _get_dtype_numba_to_mpi_ptr(arr)
+
+    # pylint: disable-next=unused-argument
+    def impl(arr):
         return numba.carray(
             # pylint: disable-next=no-value-for-parameter
-            _address_as_void_pointer(_MPI_Double_ptr),
+            _address_as_void_pointer(mpi_dtype),
             shape=(1,),
             dtype=np.intp
         )[0]
+
     return impl
 
 
 # https://stackoverflow.com/questions/61509903/how-to-pass-array-pointer-to-numba-function
 @numba.extending.intrinsic
 def _address_as_void_pointer(_, src):
     """ returns a void pointer from a given memory address """
@@ -147,15 +172,15 @@
 @numba.njit
 def send(data, dest, tag):
     """ wrapper for MPI_Send """
     data = np.ascontiguousarray(data)
     result = _MPI_Send(
         data.ctypes.data,
         data.size,
-        _mpi_double(),
+        _mpi_dtype(data),
         dest,
         tag,
         _mpi_comm_world()
     )
     assert result == 0
 
     # The following no-op prevents numba from too aggressive optimizations
@@ -173,15 +198,15 @@
         data if data.flags.c_contiguous
         else np.empty_like(data)
     )
 
     result = _MPI_Recv(
         buffer.ctypes.data,
         buffer.size,
-        _mpi_double(),
+        _mpi_dtype(data),
         source,
         tag,
         _mpi_comm_world(),
         status.ctypes.data
     )
     assert result == 0
```

### Comparing `numba-mpi-0.8/numba_mpi.egg-info/PKG-INFO` & `numba-mpi-0.9/numba_mpi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numba-mpi
-Version: 0.8
+Version: 0.9
 Summary: Numba @njittable MPI wrappers tested on Linux, macOS and Windows
 Home-page: https://github.com/atmos-cloud-sim-uj/numba-mpi
 Author: https://github.com/atmos-cloud-sim-uj/numba-mpi/graphs/contributors
 License: GPL v3
 Project-URL: Tracker, https://github.com/atmos-cloud-sim-uj/numba-mpi/issues
 Project-URL: Documentation, https://atmos-cloud-sim-uj.github.io/numba-mpi
 Project-URL: Source, https://github.com/atmos-cloud-sim-uj/numba-mpi
```

### Comparing `numba-mpi-0.8/setup.py` & `numba-mpi-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `numba-mpi-0.8/tests/test_mpi.py` & `numba-mpi-0.9/tests/test_mpi.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 from mpi4py.MPI import COMM_WORLD
 import numpy as np
 import pytest
 import numba_mpi as mpi
 
 
 class TestMPI:
+
+    data_types = [
+        int, np.int32, np.int64,
+        float, np.float64, np.double,
+        complex, np.complex64, np.complex128
+    ]
+
     @staticmethod
     @pytest.mark.parametrize("sut", [mpi.initialized, mpi.initialized.py_func])
     def test_init(sut):
         assert sut()
 
     @staticmethod
     @pytest.mark.parametrize("sut", [mpi.size, mpi.size.py_func])
@@ -24,57 +31,57 @@
         assert rank == COMM_WORLD.Get_rank()
 
     @staticmethod
     @pytest.mark.parametrize("snd, rcv", [
         (mpi.send, mpi.recv),
         (mpi.send.py_func, mpi.recv.py_func)
     ])
-    @pytest.mark.parametrize("data_type", [np.float64])
+    @pytest.mark.parametrize("data_type", data_types)
     def test_send_recv(snd, rcv, data_type):
         src = np.array([1, 2, 3, 4, 5], dtype=data_type)
         dst_tst = np.empty(5, dtype=data_type)
         dst_exp = np.empty(5, dtype=data_type)
 
         if mpi.rank() == 0:
             snd(src, dest=1, tag=11)
             COMM_WORLD.Send(src, dest=1, tag=22)
         elif mpi.rank() == 1:
             rcv(dst_tst, source=0, tag=11)
             COMM_WORLD.Recv(dst_exp, source=0, tag=22)
 
-            assert np.all(dst_tst == src)
-            assert np.all(dst_tst == dst_exp)
+            np.testing.assert_equal(dst_tst, src)
+            np.testing.assert_equal(dst_tst, dst_exp)
 
     @staticmethod
     @pytest.mark.parametrize("snd, rcv", [
         (mpi.send, mpi.recv),
         (mpi.send.py_func, mpi.recv.py_func)
     ])
-    @pytest.mark.parametrize("data_type", [np.float64])
+    @pytest.mark.parametrize("data_type", data_types)
     def test_send_recv_noncontiguous(snd, rcv, data_type):
         src = np.array([1, 2, 3, 4, 5], dtype=data_type)
         dst_tst = np.zeros_like(src)
 
         if mpi.rank() == 0:
             snd(src[::2], dest=1, tag=11)
         elif mpi.rank() == 1:
             rcv(dst_tst[::2], source=0, tag=11)
 
-            assert np.all(dst_tst[1::2] == 0)
-            assert np.all(dst_tst[::2] == src[::2])
+            np.testing.assert_equal(dst_tst[1::2], 0)
+            np.testing.assert_equal(dst_tst[::2], src[::2])
 
     @staticmethod
     @pytest.mark.parametrize("snd, rcv", [
         (mpi.send, mpi.recv),
         (mpi.send.py_func, mpi.recv.py_func)
     ])
-    @pytest.mark.parametrize("data_type", [np.float64])
+    @pytest.mark.parametrize("data_type", data_types)
     def test_send_0d_arrays(snd, rcv, data_type):
         src = np.array(1, dtype=data_type)
         dst_tst = np.zeros_like(src)
 
         if mpi.rank() == 0:
             snd(src, dest=1, tag=11)
         elif mpi.rank() == 1:
             rcv(dst_tst, source=0, tag=11)
 
-            assert np.all(dst_tst == src)
+            np.testing.assert_equal(dst_tst, src)
```

