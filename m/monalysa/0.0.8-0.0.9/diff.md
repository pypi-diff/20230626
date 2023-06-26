# Comparing `tmp/monalysa-0.0.8.tar.gz` & `tmp/monalysa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monalysa-0.0.8.tar", max compression
+gzip compressed data, was "monalysa-0.0.9.tar", max compression
```

## Comparing `monalysa-0.0.8.tar` & `monalysa-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1082 2022-10-22 00:53:43.665720 monalysa-0.0.8/LICENSE
--rw-r--r--   0        0        0     1040 2023-06-13 10:59:45.465067 monalysa-0.0.8/README.md
--rw-r--r--   0        0        0     6148 2022-10-25 06:19:52.579292 monalysa-0.0.8/monalysa/.DS_Store
--rw-r--r--   0        0        0       47 2023-02-02 06:36:48.059401 monalysa-0.0.8/monalysa/.idea/.gitignore
--rw-r--r--   0        0        0      478 2023-02-02 06:36:48.059726 monalysa-0.0.8/monalysa/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2023-02-02 06:36:48.059929 monalysa-0.0.8/monalysa/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      192 2023-02-02 06:36:48.060142 monalysa-0.0.8/monalysa/.idea/misc.xml
--rw-r--r--   0        0        0      268 2023-02-02 06:36:48.060359 monalysa-0.0.8/monalysa/.idea/modules.xml
--rw-r--r--   0        0        0      443 2023-02-02 06:36:48.060569 monalysa-0.0.8/monalysa/.idea/monalysa.iml
--rw-r--r--   0        0        0      183 2023-02-02 06:36:48.060775 monalysa-0.0.8/monalysa/.idea/vcs.xml
--rw-r--r--   0        0        0       37 2022-10-25 06:57:35.628454 monalysa-0.0.8/monalysa/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2022-10-25 06:57:35.628525 monalysa-0.0.8/monalysa/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2022-10-25 06:57:35.628367 monalysa-0.0.8/monalysa/.pytest_cache/README.md
--rw-r--r--   0        0        0      213 2022-10-26 04:26:12.613167 monalysa-0.0.8/monalysa/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      327 2022-10-26 04:27:01.645422 monalysa-0.0.8/monalysa/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2022-10-26 04:27:01.647487 monalysa-0.0.8/monalysa/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1624 2022-10-26 03:50:31.898961 monalysa-0.0.8/monalysa/README.md
--rw-r--r--   0        0        0      167 2023-06-17 07:47:38.742131 monalysa-0.0.8/monalysa/__init__.py
--rw-r--r--   0        0        0     1274 2023-06-17 06:31:40.892658 monalysa-0.0.8/monalysa/misc.py
--rw-r--r--   0        0        0    10877 2023-06-17 07:16:21.095262 monalysa-0.0.8/monalysa/movements.py
--rw-r--r--   0        0        0        0 2022-10-23 07:09:30.198480 monalysa-0.0.8/monalysa/preprocess/__init__.py
--rw-r--r--   0        0        0      170 2022-10-23 07:14:33.644553 monalysa-0.0.8/monalysa/preprocess/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0       25 2023-06-17 07:53:37.117921 monalysa-0.0.8/monalysa/quality/__init__.py
--rw-r--r--   0        0        0      167 2022-10-23 07:14:33.644259 monalysa-0.0.8/monalysa/quality/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13572 2023-06-17 07:10:09.110552 monalysa-0.0.8/monalysa/quality/__pycache__/smoothness.cpython-39.pyc
--rw-r--r--   0        0        0    14823 2023-06-17 07:07:45.172172 monalysa-0.0.8/monalysa/quality/smoothness.py
--rw-r--r--   0        0        0     7549 2023-06-17 07:09:54.658172 monalysa-0.0.8/monalysa/readers.py
--rw-r--r--   0        0        0        0 2022-10-25 05:53:15.931456 monalysa-0.0.8/monalysa/tests/__init__.py
--rw-r--r--   0        0        0      174 2022-10-25 06:57:34.579384 monalysa-0.0.8/monalysa/tests/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2653 2022-10-25 06:57:34.582061 monalysa-0.0.8/monalysa/tests/__pycache__/test_basic.cpython-39-pytest-7.1.3.pyc
--rw-r--r--   0        0        0     5456 2022-10-26 06:32:30.680020 monalysa-0.0.8/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.1.pyc
--rw-r--r--   0        0        0     5456 2022-10-26 06:10:01.482787 monalysa-0.0.8/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.3.pyc
--rw-r--r--   0        0        0     2878 2022-10-26 06:09:30.228921 monalysa-0.0.8/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.1.pyc
--rw-r--r--   0        0        0     2878 2022-10-26 06:09:40.412593 monalysa-0.0.8/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.3.pyc
--rw-r--r--   0        0        0     1604 2022-10-26 06:32:29.378486 monalysa-0.0.8/monalysa/tests/test_misc.py
--rw-r--r--   0        0        0      629 2022-10-26 06:09:06.257416 monalysa-0.0.8/monalysa/tests/test_ulfunc.py
--rw-r--r--   0        0        0      383 2023-02-02 06:53:26.896946 monalysa-0.0.8/monalysa/todo.md
--rw-r--r--   0        0        0     6148 2022-10-25 06:19:57.616213 monalysa-0.0.8/monalysa/ulfunc/.DS_Store
--rw-r--r--   0        0        0       92 2022-10-26 06:03:58.851573 monalysa-0.0.8/monalysa/ulfunc/__init__.py
--rw-r--r--   0        0        0      301 2022-10-26 06:04:05.162412 monalysa-0.0.8/monalysa/ulfunc/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6662 2023-06-17 05:52:52.196446 monalysa-0.0.8/monalysa/ulfunc/__pycache__/measures.cpython-39.pyc
--rw-r--r--   0        0        0     6428 2022-10-23 07:30:14.065832 monalysa-0.0.8/monalysa/ulfunc/__pycache__/ulfunc.cpython-39.pyc
--rw-r--r--   0        0        0     4154 2023-06-17 06:26:50.387422 monalysa-0.0.8/monalysa/ulfunc/__pycache__/ulint.cpython-39.pyc
--rw-r--r--   0        0        0     7497 2023-06-17 06:15:39.748132 monalysa-0.0.8/monalysa/ulfunc/__pycache__/uluse.cpython-39.pyc
--rw-r--r--   0        0        0      181 2023-06-15 08:16:11.174423 monalysa-0.0.8/monalysa/ulfunc/__pycache__/visualizations.cpython-39.pyc
--rw-r--r--   0        0        0    12452 2023-06-17 05:52:21.294309 monalysa-0.0.8/monalysa/ulfunc/measures.py
--rw-r--r--   0        0        0     4014 2023-06-17 06:26:26.797777 monalysa-0.0.8/monalysa/ulfunc/ulint.py
--rw-r--r--   0        0        0     8067 2023-06-17 06:15:33.539036 monalysa-0.0.8/monalysa/ulfunc/uluse.py
--rw-r--r--   0        0        0        0 2023-06-15 08:15:23.254131 monalysa-0.0.8/monalysa/ulfunc/visualizations.py
--rw-r--r--   0        0        0      559 2023-06-17 07:53:56.945740 monalysa-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 monalysa-0.0.8/setup.py
--rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 monalysa-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2022-10-22 00:53:43.665720 monalysa-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1040 2023-06-13 10:59:45.465067 monalysa-0.0.9/README.md
+-rw-r--r--   0        0        0     6148 2022-10-25 06:19:52.579292 monalysa-0.0.9/monalysa/.DS_Store
+-rw-r--r--   0        0        0       47 2023-02-02 06:36:48.059401 monalysa-0.0.9/monalysa/.idea/.gitignore
+-rw-r--r--   0        0        0      478 2023-02-02 06:36:48.059726 monalysa-0.0.9/monalysa/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2023-02-02 06:36:48.059929 monalysa-0.0.9/monalysa/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      192 2023-02-02 06:36:48.060142 monalysa-0.0.9/monalysa/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2023-02-02 06:36:48.060359 monalysa-0.0.9/monalysa/.idea/modules.xml
+-rw-r--r--   0        0        0      443 2023-02-02 06:36:48.060569 monalysa-0.0.9/monalysa/.idea/monalysa.iml
+-rw-r--r--   0        0        0      183 2023-02-02 06:36:48.060775 monalysa-0.0.9/monalysa/.idea/vcs.xml
+-rw-r--r--   0        0        0       37 2022-10-25 06:57:35.628454 monalysa-0.0.9/monalysa/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2022-10-25 06:57:35.628525 monalysa-0.0.9/monalysa/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2022-10-25 06:57:35.628367 monalysa-0.0.9/monalysa/.pytest_cache/README.md
+-rw-r--r--   0        0        0      213 2022-10-26 04:26:12.613167 monalysa-0.0.9/monalysa/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      327 2022-10-26 04:27:01.645422 monalysa-0.0.9/monalysa/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2022-10-26 04:27:01.647487 monalysa-0.0.9/monalysa/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1624 2022-10-26 03:50:31.898961 monalysa-0.0.9/monalysa/README.md
+-rw-r--r--   0        0        0      167 2023-06-17 07:47:38.742131 monalysa-0.0.9/monalysa/__init__.py
+-rw-r--r--   0        0        0     1274 2023-06-17 06:31:40.892658 monalysa-0.0.9/monalysa/misc.py
+-rw-r--r--   0        0        0    10877 2023-06-17 07:16:21.095262 monalysa-0.0.9/monalysa/movements.py
+-rw-r--r--   0        0        0        0 2022-10-23 07:09:30.198480 monalysa-0.0.9/monalysa/preprocess/__init__.py
+-rw-r--r--   0        0        0      170 2022-10-23 07:14:33.644553 monalysa-0.0.9/monalysa/preprocess/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0       25 2023-06-17 07:53:37.117921 monalysa-0.0.9/monalysa/quality/__init__.py
+-rw-r--r--   0        0        0      167 2022-10-23 07:14:33.644259 monalysa-0.0.9/monalysa/quality/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13572 2023-06-17 07:10:09.110552 monalysa-0.0.9/monalysa/quality/__pycache__/smoothness.cpython-39.pyc
+-rw-r--r--   0        0        0    14649 2023-06-17 14:27:31.388382 monalysa-0.0.9/monalysa/quality/smoothness.py
+-rw-r--r--   0        0        0     7549 2023-06-17 07:09:54.658172 monalysa-0.0.9/monalysa/readers.py
+-rw-r--r--   0        0        0        0 2022-10-25 05:53:15.931456 monalysa-0.0.9/monalysa/tests/__init__.py
+-rw-r--r--   0        0        0      174 2022-10-25 06:57:34.579384 monalysa-0.0.9/monalysa/tests/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2653 2022-10-25 06:57:34.582061 monalysa-0.0.9/monalysa/tests/__pycache__/test_basic.cpython-39-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     5456 2022-10-26 06:32:30.680020 monalysa-0.0.9/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.1.pyc
+-rw-r--r--   0        0        0     5456 2022-10-26 06:10:01.482787 monalysa-0.0.9/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     2878 2022-10-26 06:09:30.228921 monalysa-0.0.9/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.1.pyc
+-rw-r--r--   0        0        0     2878 2022-10-26 06:09:40.412593 monalysa-0.0.9/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0     1604 2022-10-26 06:32:29.378486 monalysa-0.0.9/monalysa/tests/test_misc.py
+-rw-r--r--   0        0        0      629 2022-10-26 06:09:06.257416 monalysa-0.0.9/monalysa/tests/test_ulfunc.py
+-rw-r--r--   0        0        0      383 2023-02-02 06:53:26.896946 monalysa-0.0.9/monalysa/todo.md
+-rw-r--r--   0        0        0     6148 2022-10-25 06:19:57.616213 monalysa-0.0.9/monalysa/ulfunc/.DS_Store
+-rw-r--r--   0        0        0       92 2022-10-26 06:03:58.851573 monalysa-0.0.9/monalysa/ulfunc/__init__.py
+-rw-r--r--   0        0        0      301 2022-10-26 06:04:05.162412 monalysa-0.0.9/monalysa/ulfunc/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6662 2023-06-17 05:52:52.196446 monalysa-0.0.9/monalysa/ulfunc/__pycache__/measures.cpython-39.pyc
+-rw-r--r--   0        0        0     6428 2022-10-23 07:30:14.065832 monalysa-0.0.9/monalysa/ulfunc/__pycache__/ulfunc.cpython-39.pyc
+-rw-r--r--   0        0        0     4154 2023-06-17 06:26:50.387422 monalysa-0.0.9/monalysa/ulfunc/__pycache__/ulint.cpython-39.pyc
+-rw-r--r--   0        0        0     7497 2023-06-17 06:15:39.748132 monalysa-0.0.9/monalysa/ulfunc/__pycache__/uluse.cpython-39.pyc
+-rw-r--r--   0        0        0      181 2023-06-15 08:16:11.174423 monalysa-0.0.9/monalysa/ulfunc/__pycache__/visualizations.cpython-39.pyc
+-rw-r--r--   0        0        0    12452 2023-06-17 05:52:21.294309 monalysa-0.0.9/monalysa/ulfunc/measures.py
+-rw-r--r--   0        0        0     4014 2023-06-17 06:26:26.797777 monalysa-0.0.9/monalysa/ulfunc/ulint.py
+-rw-r--r--   0        0        0     8067 2023-06-17 06:15:33.539036 monalysa-0.0.9/monalysa/ulfunc/uluse.py
+-rw-r--r--   0        0        0        0 2023-06-15 08:15:23.254131 monalysa-0.0.9/monalysa/ulfunc/visualizations.py
+-rw-r--r--   0        0        0      559 2023-06-17 14:27:59.162470 monalysa-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 monalysa-0.0.9/setup.py
+-rw-r--r--   0        0        0     1761 1970-01-01 00:00:00.000000 monalysa-0.0.9/PKG-INFO
```

### Comparing `monalysa-0.0.8/LICENSE` & `monalysa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/README.md` & `monalysa-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/.DS_Store` & `monalysa-0.0.9/monalysa/.DS_Store`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/README.md` & `monalysa-0.0.9/monalysa/README.md`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/misc.py` & `monalysa-0.0.9/monalysa/misc.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/movements.py` & `monalysa-0.0.9/monalysa/movements.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/quality/__pycache__/smoothness.cpython-39.pyc` & `monalysa-0.0.9/monalysa/quality/__pycache__/smoothness.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/quality/smoothness.py` & `monalysa-0.0.9/monalysa/quality/smoothness.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,48 +53,45 @@
     >>> t = np.arange(-1, 1, 0.01)
     >>> move = np.exp(-5*pow(t, 2))
     >>> smooth, _, _ = sparc(move, fs=100.)
     >>> print(f'{smooth:0.5f}')
     '-1.41403'
 
     """
-    try:
-        # Number of zeros to be padded.
-        nfft = int(pow(2, np.ceil(np.log2(len(movement))) + padlevel))
-
-        # Frequency
-        f = np.arange(0, fs, fs / nfft)
-        # Normalized magnitude spectrum
-        Mf = abs(np.fft.fft(movement, nfft))
-        Mf = Mf / max(Mf)
-
-        # Indices to choose only the spectrum within the given cut off
-        # frequency Fc.
-        # NOTE: This is a low pass filtering operation to get rid of high
-        # frequency noise from affecting the next step (amplitude threshold
-        # based cut off for  arc length calculation).
-        fc_inx = ((f <= fc) * 1).nonzero()
-        f_sel = f[fc_inx]
-        Mf_sel = Mf[fc_inx]
-
-        # Choose the amplitude threshold based cut off frequency.
-        # Index of the last point on the magnitude spectrum that is greater
-        # than or equal to the amplitude threshold.
-        inx = ((Mf_sel >= amp_th) * 1).nonzero()[0]
-        fc_inx = range(inx[0], inx[-1] + 1)
-        f_sel = f_sel[fc_inx]
-        Mf_sel = Mf_sel[fc_inx]
-
-        # Calculate arc length
-        new_sal = -sum(
-            np.sqrt(pow(np.diff(f_sel) / (f_sel[-1] - f_sel[0]), 2) +
-                    pow(np.diff(Mf_sel), 2)))
-        return new_sal, (f, Mf), (f_sel, Mf_sel)
-    finally:
-        return np.NaN, np.NaN, np.NaN
+    # Number of zeros to be padded.
+    nfft = int(pow(2, np.ceil(np.log2(len(movement))) + padlevel))
+
+    # Frequency
+    f = np.arange(0, fs, fs / nfft)
+    # Normalized magnitude spectrum
+    Mf = abs(np.fft.fft(movement, nfft))
+    Mf = Mf / max(Mf)
+
+    # Indices to choose only the spectrum within the given cut off frequency
+    # Fc.
+    # NOTE: This is a low pass filtering operation to get rid of high frequency
+    # noise from affecting the next step (amplitude threshold based cut off for
+    # arc length calculation).
+    fc_inx = ((f <= fc) * 1).nonzero()
+    f_sel = f[fc_inx]
+    Mf_sel = Mf[fc_inx]
+
+    # Choose the amplitude threshold based cut off frequency.
+    # Index of the last point on the magnitude spectrum that is greater than
+    # or equal to the amplitude threshold.
+    inx = ((Mf_sel >= amp_th) * 1).nonzero()[0]
+    fc_inx = range(inx[0], inx[-1] + 1)
+    f_sel = f_sel[fc_inx]
+    Mf_sel = Mf_sel[fc_inx]
+
+    # Calculate arc length
+    sal = -sum(np.sqrt(pow(np.diff(f_sel) / (f_sel[-1] - f_sel[0]), 2) +
+                           pow(np.diff(Mf_sel), 2)))
+    return sal, (f, Mf), (f_sel, Mf_sel)
+
 
 
 def dimensionless_jerk_factors(movement, fs, data_type='vel', rem_mean=False):
     """
     Returns the individual factors of the dimensionless jerk metric.
 
     Parameters
```

### Comparing `monalysa-0.0.8/monalysa/readers.py` & `monalysa-0.0.9/monalysa/readers.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/tests/__pycache__/test_basic.cpython-39-pytest-7.1.3.pyc` & `monalysa-0.0.9/monalysa/tests/__pycache__/test_basic.cpython-39-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.1.pyc` & `monalysa-0.0.9/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.1.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.3.pyc` & `monalysa-0.0.9/monalysa/tests/__pycache__/test_misc.cpython-39-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.1.pyc` & `monalysa-0.0.9/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.1.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.3.pyc` & `monalysa-0.0.9/monalysa/tests/__pycache__/test_ulfunc.cpython-39-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/tests/test_misc.py` & `monalysa-0.0.9/monalysa/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/tests/test_ulfunc.py` & `monalysa-0.0.9/monalysa/tests/test_ulfunc.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/ulfunc/.DS_Store` & `monalysa-0.0.9/monalysa/ulfunc/.DS_Store`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/ulfunc/__pycache__/measures.cpython-39.pyc` & `monalysa-0.0.9/monalysa/ulfunc/__pycache__/measures.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/ulfunc/__pycache__/ulfunc.cpython-39.pyc` & `monalysa-0.0.9/monalysa/ulfunc/__pycache__/ulfunc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/ulfunc/__pycache__/ulint.cpython-39.pyc` & `monalysa-0.0.9/monalysa/ulfunc/__pycache__/ulint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/ulfunc/__pycache__/uluse.cpython-39.pyc` & `monalysa-0.0.9/monalysa/ulfunc/__pycache__/uluse.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/ulfunc/measures.py` & `monalysa-0.0.9/monalysa/ulfunc/measures.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/ulfunc/ulint.py` & `monalysa-0.0.9/monalysa/ulfunc/ulint.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/monalysa/ulfunc/uluse.py` & `monalysa-0.0.9/monalysa/ulfunc/uluse.py`

 * *Files identical despite different names*

### Comparing `monalysa-0.0.8/pyproject.toml` & `monalysa-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monalysa"
-version = "0.0.8"
+version = "0.0.9"
 description = "A unified library for carrying out quantitative movement analysis."
 authors = ["Sivakumar Balasubramanian (Siva) <siva82kb@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/siva82kb/monalysa"
 repository = "https://github.com/siva82kb/monalysa"
 keywords = ["movement analysis", "biomechanics", "neurorehabilitation", "sport science"]
```

### Comparing `monalysa-0.0.8/setup.py` & `monalysa-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'monalysa': ['.idea/*',
               '.idea/inspectionProfiles/*',
               '.pytest_cache/*',
               '.pytest_cache/v/cache/*']}
 
 setup_kwargs = {
     'name': 'monalysa',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A unified library for carrying out quantitative movement analysis.',
     'long_description': '# <span style="color:#555"><span style="color:#A62B17">**Mo**</span>vement  A<span style="color:#A62B17">**nalys**</span>is Libr<span style="color:#A62B17">**a**</span>ry (Monalysa)</span>\n\nMonalysa, _aka_ <u>**Mo**</u>ovement a<u>**nalys**</u>is libr<u>**a**</u>y, is a unified python library for the quantitative analysis of sensorimotor behavior. Monalysa provides a set of data structures, functions, and classes for representing, analyzing, and visualizing movement-related data from different technologies (motion capture, inertial measurement units, robots, force/torque sensors, force plates, etc.).\n\n## Purpose of the library\nIn the spirit of open science, the monalysa library provides open-source code for a set of commonly used methods, measures, and tools for analyzing movement data. Such a library can be a step towards the standardization of procedures used for movement analysis.\n\n## Who is this library for?\nThis library is aimed at students, researchers, clinicians and industry professionals working with movement data.\n',
     'author': 'Sivakumar Balasubramanian (Siva)',
     'author_email': 'siva82kb@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/siva82kb/monalysa',
```

### Comparing `monalysa-0.0.8/PKG-INFO` & `monalysa-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monalysa
-Version: 0.0.8
+Version: 0.0.9
 Summary: A unified library for carrying out quantitative movement analysis.
 Home-page: https://github.com/siva82kb/monalysa
 License: MIT
 Keywords: movement analysis,biomechanics,neurorehabilitation,sport science
 Author: Sivakumar Balasubramanian (Siva)
 Author-email: siva82kb@gmail.com
 Requires-Python: >=3.9,<4.0
```

