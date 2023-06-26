# Comparing `tmp/gsoup-0.0.8.tar.gz` & `tmp/gsoup-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsoup-0.0.8.tar", last modified: Sun Apr  9 14:09:34 2023, max compression
+gzip compressed data, was "gsoup-0.0.9.tar", last modified: Mon Jun 26 08:01:06 2023, max compression
```

## Comparing `gsoup-0.0.8.tar` & `gsoup-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.404677 gsoup-0.0.8/
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     1088 2022-11-18 02:40:35.000000 gsoup-0.0.8/LICENSE
--rw-rw-r--   0 yotam     (1003) yotam     (1003)       45 2022-12-05 04:54:57.000000 gsoup-0.0.8/MANIFEST.in
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     3154 2023-04-09 14:09:34.400678 gsoup-0.0.8/PKG-INFO
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     1392 2023-02-15 10:00:37.000000 gsoup-0.0.8/README.md
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     1210 2023-04-09 14:09:07.000000 gsoup-0.0.8/pyproject.toml
--rw-rw-r--   0 yotam     (1003) yotam     (1003)       38 2023-04-09 14:09:34.404677 gsoup-0.0.8/setup.cfg
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.396678 gsoup-0.0.8/src/
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.400678 gsoup-0.0.8/src/gsoup/
--rwx------   0 yotam     (1003) yotam     (1003)   343980 2012-02-17 04:17:40.000000 gsoup-0.0.8/src/gsoup/FreeMono.ttf
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     2370 2023-04-09 14:09:07.000000 gsoup-0.0.8/src/gsoup/__init__.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    26648 2023-04-09 12:29:27.000000 gsoup-0.0.8/src/gsoup/core.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     7842 2022-12-14 08:18:43.000000 gsoup-0.0.8/src/gsoup/geometry_advanced.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    14710 2023-03-11 12:33:08.000000 gsoup-0.0.8/src/gsoup/geometry_basic.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    16714 2023-03-11 13:26:05.000000 gsoup-0.0.8/src/gsoup/gsoup_io.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    22251 2023-03-21 09:44:07.000000 gsoup-0.0.8/src/gsoup/image.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    18798 2023-03-11 12:33:36.000000 gsoup-0.0.8/src/gsoup/procam.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     8189 2023-02-28 10:40:05.000000 gsoup-0.0.8/src/gsoup/sphere_trace.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     9104 2023-02-17 14:37:19.000000 gsoup-0.0.8/src/gsoup/structures.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    10012 2023-02-17 13:20:00.000000 gsoup-0.0.8/src/gsoup/video.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     7409 2023-03-10 03:21:59.000000 gsoup-0.0.8/src/gsoup/viewer.py
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     6542 2023-03-10 03:21:59.000000 gsoup-0.0.8/src/gsoup/viewer_drivers.py
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.400678 gsoup-0.0.8/src/gsoup.egg-info/
--rw-rw-r--   0 yotam     (1003) yotam     (1003)     3154 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/PKG-INFO
--rw-rw-r--   0 yotam     (1003) yotam     (1003)      528 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 yotam     (1003) yotam     (1003)        1 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 yotam     (1003) yotam     (1003)      110 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/requires.txt
--rw-rw-r--   0 yotam     (1003) yotam     (1003)        6 2023-04-09 14:09:34.000000 gsoup-0.0.8/src/gsoup.egg-info/top_level.txt
-drwxrwxr-x   0 yotam     (1003) yotam     (1003)        0 2023-04-09 14:09:34.400678 gsoup-0.0.8/tests/
--rw-rw-r--   0 yotam     (1003) yotam     (1003)    14734 2023-04-09 08:06:28.000000 gsoup-0.0.8/tests/test_basic.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.734643 gsoup-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2022-12-12 04:07:15.000000 gsoup-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       47 2022-12-12 04:07:15.000000 gsoup-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3037 2023-06-26 08:01:06.734643 gsoup-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1202 2023-06-25 06:21:55.000000 gsoup-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1252 2023-06-26 07:58:21.000000 gsoup-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 08:01:06.734643 gsoup-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.680651 gsoup-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.713699 gsoup-0.0.9/src/gsoup/
+-rw-rw-rw-   0        0        0   343980 2022-12-12 04:07:15.000000 gsoup-0.0.9/src/gsoup/FreeMono.ttf
+-rw-rw-rw-   0        0        0     2734 2023-06-26 07:58:21.000000 gsoup-0.0.9/src/gsoup/__init__.py
+-rw-rw-rw-   0        0        0    25250 2023-06-26 07:42:32.000000 gsoup-0.0.9/src/gsoup/core.py
+-rw-rw-rw-   0        0        0     7363 2023-06-26 07:38:01.000000 gsoup-0.0.9/src/gsoup/geometry_advanced.py
+-rw-rw-rw-   0        0        0    14707 2023-06-25 06:21:55.000000 gsoup-0.0.9/src/gsoup/geometry_basic.py
+-rw-rw-rw-   0        0        0    20248 2023-06-26 07:55:45.000000 gsoup-0.0.9/src/gsoup/gsoup_io.py
+-rw-rw-rw-   0        0        0    24244 2023-06-25 06:21:55.000000 gsoup-0.0.9/src/gsoup/image.py
+-rw-rw-rw-   0        0        0    19684 2023-06-25 06:21:55.000000 gsoup-0.0.9/src/gsoup/procam.py
+-rw-rw-rw-   0        0        0     8189 2023-02-28 11:28:59.000000 gsoup-0.0.9/src/gsoup/sphere_trace.py
+-rw-rw-rw-   0        0        0     9104 2023-02-16 04:29:03.000000 gsoup-0.0.9/src/gsoup/structures.py
+-rw-rw-rw-   0        0        0     5691 2023-06-26 07:44:21.000000 gsoup-0.0.9/src/gsoup/transforms.py
+-rw-rw-rw-   0        0        0    11926 2023-06-25 06:21:55.000000 gsoup-0.0.9/src/gsoup/video.py
+-rw-rw-rw-   0        0        0     7409 2023-02-26 12:22:36.000000 gsoup-0.0.9/src/gsoup/viewer.py
+-rw-rw-rw-   0        0        0     6542 2023-02-28 11:44:06.000000 gsoup-0.0.9/src/gsoup/viewer_drivers.py
+drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.732648 gsoup-0.0.9/src/gsoup.egg-info/
+-rw-rw-rw-   0        0        0     3037 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-26 08:01:06.000000 gsoup-0.0.9/src/gsoup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 08:01:06.733675 gsoup-0.0.9/tests/
+-rw-rw-rw-   0        0        0    16532 2023-06-26 07:54:08.000000 gsoup-0.0.9/tests/test_basic.py
```

### Comparing `gsoup-0.0.8/LICENSE` & `gsoup-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.8/README.md` & `gsoup-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # gsoup
 
 ## In a nutshell
-A python library implementing various computational geometry / graphics algorithms with focus on clarity rather than performance.
+A python library implementing various geometry / graphics algorithms, with focus on clarity rather than performance.
 
 ## Long version
-This library is the result of me getting tired of replicating pieces of utility code to do similar work across different projects. I decided to push any fundamental piece of code into this repository. Later on I also wanted a place I can implement any related algorithm and easily verify/test/modify them so I decided it would be usefull to add them to the same place. The focus is on clarity and concisness for all implementations, but here and there some immediate/easy performance gains are used.
+This library is the result of me getting tired of replicating pieces of utility code to do similar work across different projects. I decided to push any fundamental piece of code into this repository. The focus is on clarity and concisness for all implementations, but here and there some immediate/easy performance gains are used.
 
-The majority of the code uses numpy, but a significant effort has been made to also be compatible with pytorch for GPU computations, as many of my interests rely on a strong auto-differentiaion (and GPU enabled) package.
+The majority of the code uses numpy, but some effort has been made to also be compatible with pytorch for GPU computations, as many of my interests rely on a strong auto-differentiaion (and GPU enabled) package.
 
 All the code is used for self-educational purposes and to facilitate faster research of concepts in computational geometry / graphics.
 
 ## Installation
 `pip install gsoup`
 
 ## Usage
```

### Comparing `gsoup-0.0.8/pyproject.toml` & `gsoup-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "gsoup"
-version = "0.0.8"
-description = "A geoemtry & graphics library with focus on clarity rather than performance."
-readme = "README.md"
-authors = [{ name = "Yotam Erel", email = "erelyotam@gmail.com" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-]
-keywords = ["geometry", "graphics", "autograd", "vision"]
-dependencies = [
-    "torch >= 1.10",
-    "numpy",
-    "Pillow", 
-    "scipy",
-    "ffmpeg-python",
-    "opencv-contrib-python",
-]
-requires-python = ">=3.7"
-
-[project.optional-dependencies]
-build = ["build", "twine"]
-dev = ["bumpver", "pytest"]
-
-[project.urls]
-Homepage = "https://github.com/yoterel/gsoup"
-
-[tool.bumpver]
-current_version = "0.0.8"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message = "bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = false
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = [
-    'current_version = "{version}"',
-    'version = "{version}"',
-]
-"src/gsoup/__init__.py" = [
-    "{version}"
-]
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "gsoup"
+version = "0.0.9"
+description = "A geoemtry & graphics library with focus on clarity rather than performance."
+readme = "README.md"
+authors = [{ name = "Yotam Erel", email = "erelyotam@gmail.com" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+]
+keywords = ["geometry", "graphics", "autograd", "vision"]
+dependencies = [
+    "torch >= 1.10",
+    "numpy",
+    "Pillow", 
+    "scipy",
+    "ffmpeg-python",
+    "opencv-python",
+]
+requires-python = ">=3.7"
+
+[project.optional-dependencies]
+build = ["build", "twine"]
+dev = ["bumpver", "pytest"]
+
+[project.urls]
+Homepage = "https://github.com/yoterel/gsoup"
+
+[tool.bumpver]
+current_version = "0.0.9"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = false
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = [
+    'current_version = "{version}"',
+    'version = "{version}"',
+]
+"src/gsoup/__init__.py" = [
+    "{version}"
+]
```

### Comparing `gsoup-0.0.8/src/gsoup/FreeMono.ttf` & `gsoup-0.0.9/src/gsoup/FreeMono.ttf`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.8/src/gsoup/core.py` & `gsoup-0.0.9/src/gsoup/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -429,106 +429,28 @@
     if x.ndim == 3:
         return Image.fromarray(to_8b(x))
     elif x.ndim == 2:
         return Image.fromarray(to_8b(x[:, :, None]), mode="L")
     else:
         raise ValueError("unsupported array dimensions")
 
-def translate(t):
-    """
-    creates a translation matrix from a translation vector
-    :param t: translation vector or batch of translation vectors
-    :return: 4x4 translation matrix
-    """
-    if t.shape[-1] != 3:
-        raise ValueError("translation vector must be 3d")
-    if t.ndim == 1:
-        t = t[None, :]
-    mat = np.concatenate((np.eye(3)[None, :, :], t[:, :, None]), axis=-1)
-    return to_44(mat)
-
-def scale(s):
-    """
-    creates a scaling matrix from a scaling vector
-    :param s: scaling vector or batch of scaling vectors
-    :return: nx4x4 scaling matrix
-    """
-    if s.shape[-1] != 3:
-        raise ValueError("translation vector must be 3d")
-    if s.ndim == 1:
-        s = s[None, :]
-    mat = np.diag(s)
-    return to_44(mat)
-
-def sincos(a, degrees=True):
-    """
-    sin and cos of an angle
-    :param a: angle
-    :param degrees: if True, a is in degrees
-    """
-    if degrees:
-        a = np.deg2rad(a)
-    return np.sin(a), np.cos(a)
-
-def rotate(a, r):
-    """
-    creates a rotation matrix from an angle a and an axis of rotation r
-    """
-    s, c = sincos(a)
-    r = normalize(r)
-    nc = 1 - c
-    x, y, z = r
-    return np.array([[x*x*nc +   c, x*y*nc - z*s, x*z*nc + y*s, 0],
-                      [y*x*nc + z*s, y*y*nc +   c, y*z*nc - x*s, 0],
-                      [x*z*nc - y*s, y*z*nc + x*s, z*z*nc +   c, 0],
-                      [           0,            0,            0, 1]])
-
-def rotx(a, degrees=True):
-    """
-    creates a homogeneous 3D rotation matrix around the x axis
-    a: angle
-    degrees: if True, a is in degrees, else radians
-    """
-    s, c = sincos(a, degrees)
-    return np.array([[1,0,0,0],
-                      [0,c,-s,0],
-                      [0,s,c,0],
-                      [0,0,0,1]])
-
-def roty(a, degrees=True):
-    """
-    creates a homogeneous 3D rotation matrix around the y axis
-    a: angle
-    degrees: if True, a is in degrees, else radians
-    """
-    s, c = sincos(a, degrees)
-    return np.array([[c,0,s,0],
-                      [0,1,0,0],
-                      [-s,0,c,0],
-                      [0,0,0,1]])
-
-def rotz(a, degrees=True):
-    """
-    creates a homogeneous 3D rotation matrix around the z axis
-    a: angle
-    degrees: if True, a is in degrees, else radians
-    """
-    s, c = sincos(a, degrees)
-    return np.array([[c,-s,0,0],
-                      [s,c,0,0],
-                      [0,0,1,0],
-                      [0,0,0,1]])
-
-def map_range(x, in_min, in_max, out_min, out_max):
+def map_range(x, out_min, out_max):
     """
     given an input and a range, maps it to a new range
     """
-    if not in_min <= x <= in_max:
-        raise ValueError("input must be inside range ({} - {})".format(in_min, in_max))
-    return int((x-in_min) * (out_max-out_min) / (in_max-in_min) + out_min)
+    if type(x) == np.ndarray:
+        return np.clip((x-x.min()) * (out_max-out_min) / (x.max()-x.min()) + out_min, out_min, out_max)
+    elif type(x) == torch.Tensor:
+        return torch.clamp((x-x.min()) * (out_max-out_min) / (x.max()-x.min()) + out_min, out_min, out_max)
+    else:
+        raise ValueError("unsupported type")
+
+def map_to_01(x):
+    return map_range(x, 0, 1)
+
 
 def vec2skew(v):
     """
     returns the skew operator matrix given a vector
     :param v:  (3, ) torch tensor
     :return:   (3, 3)
     """
@@ -590,14 +512,46 @@
     """
     o = np.random.randn(n, 4)
     s = (o * o).sum(1)
     denom = np.copysign(np.sqrt(s), o[:, 0])[:, None]
     o = o / denom
     return o
 
+def random_affine(ang_range=20.0, trans_range=10.0, scale=2.0):
+    """
+    generates a random 2D affine transformation matrix
+    """
+    R = np.eye(3)
+    ang_rot = np.random.uniform(ang_range)-ang_range/2
+    tx = trans_range*np.random.uniform()-trans_range/2
+    ty = trans_range*np.random.uniform()-trans_range/2
+    sx = np.random.rand() * scale
+    sy = np.random.rand() * scale
+    R[0, 0] = np.cos(ang_rot * np.pi / 180)
+    R[0, 1] = -np.sin(ang_rot * np.pi / 180)
+    R[1, 0] = np.sin(ang_rot * np.pi / 180)
+    R[1, 1] = np.cos(ang_rot * np.pi / 180)
+    T = np.eye(3)
+    T[0, 2] = tx
+    T[1, 2] = ty
+    S = np.eye(3)
+    S[0, 0] = sx
+    S[1, 1] = sy
+    H = T @ S @ R
+    return H
+
+def random_perspective():
+    """
+    generates a random 2D perspective transformation matrix
+    """
+    P = random_affine()
+    P[2, 0] = np.random.rand() / 100
+    P[2, 1] = np.random.rand() / 100
+    return P
+
 def random_vectors_on_sphere(n, normal=None, device="cpu"):
     """
     create a batch of uniformly distributed random unit vectors on a sphere
     note: if normal is provided, returns random unit vectors on the hemisphere around the normal, but isn't uniform anymore.
     :param n: number of vectors
     :param normal: normals to orient the hemisphere (,3) or (n,3)
     :param device: device to put the tensors on
```

### Comparing `gsoup-0.0.8/src/gsoup/geometry_advanced.py` & `gsoup-0.0.9/src/gsoup/geometry_advanced.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,152 @@
-import torch
-import numpy as np
-from .core import to_hom
-from .geometry_basic import get_edges, edge_contraction
-
-def compute_incident_triangles(f):
-    """
-    compute the incident triangles per vertex
-    :param v: vertices of the mesh
-    :param f: faces of the mesh
-    :return: list of lists of incident triangles per vertex
-    """
-    incident_triangles = [[] for _ in range(np.unique(f).shape[0])]
-    for i, face in enumerate(f):
-        for vertex in face:
-            incident_triangles[vertex].append(i)
-    return incident_triangles
-
-def compute_quadtratic_surface(v, f):
-    """
-    given a mesh, compute the quadratic surface coefficients per vertex in a tensor of size Vx4x4
-    the per vertex quadratic surface is computed from the sum of quadtratic surfaces of incident faces to each vertex
-    :param v: vertices of the mesh
-    :param f: faces of the mesh
-    :return: tensor of size Vx4x4 of quadtratic surface coefficients per vertex
-    """
-    e1 = v[f[:, 1]] - v[f[:, 0]]
-    e2 = v[f[:, 2]] - v[f[:, 0]]
-    e1 = e1 / np.linalg.norm(e1, axis=-1)[: ,None]
-    e2 = e2 / np.linalg.norm(e2, axis=-1)[: ,None]
-    n = np.cross(e1, e2)
-    n = n / np.linalg.norm(n, axis=-1)[: ,None]
-    d = ((-v[f[:, 0]])[:, None, :] @ n[:, :, None]).squeeze()
-    Qf = np.zeros((f.shape[0], 4, 4))
-    Qf[:, :3, :3] = n[:, :, None] @ n[:, None, :]
-    Qf[:, -1, :-1] = d[:, None] * n
-    Qf[:, :-1, -1] = Qf[:, -1, :-1]
-    Qf[:, -1, -1] = d * d
-    Qv = distribute_field(v, f, Qf)
-    return Qv
-
-def compute_contraction_costs(v_hats, valid_pairs, Qv):
-    """
-    compute the costs of contracting the valid pairs
-    :param v_hats: the new vertices after contraction
-    :param valid_pairs: the valid pairs of vertices to contract
-    :param Qv: the quadratic surface coefficients per v_hat
-    :return: the costs of contracting the valid pairs
-    """
-    v_hats = to_hom(v_hats)
-    Q_hats = np.sum(Qv[valid_pairs], axis=1)
-    return (v_hats[:, None, :] @ (Q_hats @ v_hats[:, :, None])).squeeze()
-
-def compute_v_hats(v, valid_pairs, Qv):
-    """
-    computes the optimal vertex positions for each valid pair of vertices given the quadratic surface coefficients of contracting the pairs
-    :param v: vertices of the mesh
-    :param valid_pairs: list of valid pairs of vertices
-    :param Qv: tensor of size Vx4x4 of quadtratic surface coefficients per vertex
-    :return: tensor of size Vx3 of (almost) optimal vertex positions
-    """
-    v_hats = np.zeros((valid_pairs.shape[0], 3), dtype=np.float32)
-    Q_hats = np.sum(Qv[valid_pairs], axis=1)
-    Q_hats[:, -1, :] = np.array([0, 0, 0, 1])[None, :]
-    mask = np.linalg.det(Q_hats) != 0
-    v_hats[mask] = (np.linalg.inv(Q_hats[mask]) @ np.array([0, 0, 0, 1])[None, :, None]).squeeze()[:, :3]  # d(cost)/d(v_hat) = 0
-    # note: orig paper searches for the minimum along the segment between the two vertices if Q_hat is singular
-    v_hats[~mask] = np.mean(v[valid_pairs[~mask]], axis=1)  # if Q_hats is singular, use the mean of the two vertices
-    return v_hats
-
-def qem(v: np.ndarray, f: np.ndarray, budget: int):
-    """
-    A slightly naive (and slow) implementation of "Surface Simplification Using Quadric Error Metrics", 1997
-    """
-    if v.ndim != 2 or v.shape[-1] != 3:
-        raise ValueError("v must be V x 3 array")
-    if f.ndim != 2 or f.shape[-1] != 3:
-        raise ValueError("f must be F x 3 array")
-    if budget < 4:
-        raise ValueError("minimum budget is 3 triangles")
-    while f.shape[0] > budget:
-        print("current # faces: {}".format(f.shape[0]))
-        valid_pairs = get_edges(f)
-        Qv = compute_quadtratic_surface(v, f)
-        v_hats = compute_v_hats(v, valid_pairs, Qv)
-        costs = compute_contraction_costs(v_hats, valid_pairs, Qv)
-        lowest_cost = np.argmin(costs)
-        v, f = edge_contraction(v, f, valid_pairs[lowest_cost], v_hats[lowest_cost])
-    return v, f
-
-def distribute_field(v, f, field, avg=False):
-    """
-    given a field of size F (with any number of addtional dimensions), distribute it to the vertices of the mesh by summing up the values of the incident faces
-    :param v: vertices of the mesh
-    :param f: faces of the mesh
-    :param field: field of size F
-    :param avg: if True, the field is averaged over the incident faces instead of summed up
-    :return: scalar field of size V
-    """
-    # compute the incident triangles per vertex
-    incident_triangles = compute_incident_triangles(f)
-    # compute the scalar field per vertex
-    field_per_vertex = np.zeros((v.shape[0], *field.shape[1:]))
-    for i, face in enumerate(f):
-        for vertex in face:
-            field_per_vertex[vertex] += field[i]
-    if avg:
-        field_per_vertex /= len(incident_triangles)
-    return field_per_vertex
-
-def distribute_scalar_field(num_vertices, f, per_face_scalar_field, avg=False):
-    """
-    computes a scalar field per vertex by summing / averaging the incident face scalar field
-    :param num_vertices: number of vertices in the mesh
-    :param f: faces of the mesh
-    :param per_face_scalar_field: scalar field of size F
-    :param avg: if True, the field is averaged over the incident faces instead of summed up
-    :return: scalar field of size V
-    """
-    device = f.device
-    incident_face_areas = torch.zeros([num_vertices, 1], device=device)
-    f_unrolled = f.flatten()
-    face_indices_repeated_per_vertex = torch.arange(f.shape[0], device=f.device)
-    face_indices_repeated_per_vertex = torch.repeat_interleave(face_indices_repeated_per_vertex, repeats=3)
-    face_areas_repeated_per_face = per_face_scalar_field[face_indices_repeated_per_vertex].unsqueeze(-1)
-    incident_face_areas = torch.index_add(incident_face_areas, dim=0, index=f_unrolled,
-                                          source=face_areas_repeated_per_face)
-    if avg:
-        neighbors = torch.index_add(torch.zeros_like(incident_face_areas), dim=0, index=f_unrolled,
-                                    source=torch.ones_like(face_areas_repeated_per_face))
-        incident_face_areas = incident_face_areas / neighbors
-    return incident_face_areas
-
-def distribute_vector_field(num_vertices, f, per_face_vector_field):
-    """
-    computes a vector field per vertex by summing the incident face vector field
-    :param num_vertices: number of vertices in the mesh
-    :param f: faces of the mesh
-    :param per_face_vector_field: vector field of size Fx3
-    :return: vector field of size Vx3
-    """
-    device = f.device
-    incident_face_areas = torch.zeros([num_vertices, 1], device=device)
-    f_unrolled = f.flatten()
-    face_indices_repeated_per_vertex = torch.arange(f.shape[0], device=f.device)
-    face_indices_repeated_per_vertex = torch.repeat_interleave(face_indices_repeated_per_vertex, repeats=3)
-    normals_repeated_per_face = per_face_vector_field[face_indices_repeated_per_vertex]
-    normals_repeated_per_face = normals_repeated_per_face
-    incident_face_vectors = torch.zeros([num_vertices,per_face_vector_field.shape[-1]], device=device)
-    incident_face_vectors = torch.index_add(incident_face_vectors, dim=0, index=f_unrolled,
-                                            source=normals_repeated_per_face)
-    return incident_face_vectors
-
-def rigid_transform_3d(A, B):
-    """
-    finds best rigid transformation between pc a and pc b (in terms of rmse) based on "Least-Squares Rigid Motion Using SVD"
-    :param A: point cloud a
-    :param B: point cloud b
-    :return: R, t such that B = R @ A + t
-    """
-    centroid_A = np.mean(A, axis=0)
-    centroid_B = np.mean(B, axis=0)
-
-    A_mean = A - centroid_A
-    B_mean = B - centroid_B
-
-    H = A_mean.T @ B_mean
-    U, S, Vt = np.linalg.svd(H)
-
-    flip = np.linalg.det(Vt.T @ U.T)
-    ones = np.identity(len(Vt))
-    ones[-1, -1] = flip
-    R = Vt.T @ ones @ U.T
-    t = centroid_B - R @ centroid_A
-    return R, t
+import torch
+import numpy as np
+from .core import to_hom
+from .geometry_basic import get_edges, edge_contraction
+
+def compute_incident_triangles(f):
+    """
+    compute the incident triangles per vertex
+    :param v: vertices of the mesh
+    :param f: faces of the mesh
+    :return: list of lists of incident triangles per vertex
+    """
+    incident_triangles = [[] for _ in range(np.unique(f).shape[0])]
+    for i, face in enumerate(f):
+        for vertex in face:
+            incident_triangles[vertex].append(i)
+    return incident_triangles
+
+def compute_quadtratic_surface(v, f):
+    """
+    given a mesh, compute the quadratic surface coefficients per vertex in a tensor of size Vx4x4
+    the per vertex quadratic surface is computed from the sum of quadtratic surfaces of incident faces to each vertex
+    :param v: vertices of the mesh
+    :param f: faces of the mesh
+    :return: tensor of size Vx4x4 of quadtratic surface coefficients per vertex
+    """
+    e1 = v[f[:, 1]] - v[f[:, 0]]
+    e2 = v[f[:, 2]] - v[f[:, 0]]
+    e1 = e1 / np.linalg.norm(e1, axis=-1)[: ,None]
+    e2 = e2 / np.linalg.norm(e2, axis=-1)[: ,None]
+    n = np.cross(e1, e2)
+    n = n / np.linalg.norm(n, axis=-1)[: ,None]
+    d = ((-v[f[:, 0]])[:, None, :] @ n[:, :, None]).squeeze()
+    Qf = np.zeros((f.shape[0], 4, 4))
+    Qf[:, :3, :3] = n[:, :, None] @ n[:, None, :]
+    Qf[:, -1, :-1] = d[:, None] * n
+    Qf[:, :-1, -1] = Qf[:, -1, :-1]
+    Qf[:, -1, -1] = d * d
+    Qv = distribute_field(v, f, Qf)
+    return Qv
+
+def compute_contraction_costs(v_hats, valid_pairs, Qv):
+    """
+    compute the costs of contracting the valid pairs
+    :param v_hats: the new vertices after contraction
+    :param valid_pairs: the valid pairs of vertices to contract
+    :param Qv: the quadratic surface coefficients per v_hat
+    :return: the costs of contracting the valid pairs
+    """
+    v_hats = to_hom(v_hats)
+    Q_hats = np.sum(Qv[valid_pairs], axis=1)
+    return (v_hats[:, None, :] @ (Q_hats @ v_hats[:, :, None])).squeeze()
+
+def compute_v_hats(v, valid_pairs, Qv):
+    """
+    computes the optimal vertex positions for each valid pair of vertices given the quadratic surface coefficients of contracting the pairs
+    :param v: vertices of the mesh
+    :param valid_pairs: list of valid pairs of vertices
+    :param Qv: tensor of size Vx4x4 of quadtratic surface coefficients per vertex
+    :return: tensor of size Vx3 of (almost) optimal vertex positions
+    """
+    v_hats = np.zeros((valid_pairs.shape[0], 3), dtype=np.float32)
+    Q_hats = np.sum(Qv[valid_pairs], axis=1)
+    Q_hats[:, -1, :] = np.array([0, 0, 0, 1])[None, :]
+    mask = np.linalg.det(Q_hats) != 0
+    v_hats[mask] = (np.linalg.inv(Q_hats[mask]) @ np.array([0, 0, 0, 1])[None, :, None]).squeeze()[:, :3]  # d(cost)/d(v_hat) = 0
+    # note: orig paper searches for the minimum along the segment between the two vertices if Q_hat is singular
+    v_hats[~mask] = np.mean(v[valid_pairs[~mask]], axis=1)  # if Q_hats is singular, use the mean of the two vertices
+    return v_hats
+
+def qem(v: np.ndarray, f: np.ndarray, budget: int):
+    """
+    A slightly naive (and slow) implementation of "Surface Simplification Using Quadric Error Metrics", 1997
+    """
+    if v.ndim != 2 or v.shape[-1] != 3:
+        raise ValueError("v must be V x 3 array")
+    if f.ndim != 2 or f.shape[-1] != 3:
+        raise ValueError("f must be F x 3 array")
+    if budget < 4:
+        raise ValueError("minimum budget is 3 triangles")
+    while f.shape[0] > budget:
+        print("current # faces: {}".format(f.shape[0]))
+        valid_pairs = get_edges(f)
+        Qv = compute_quadtratic_surface(v, f)
+        v_hats = compute_v_hats(v, valid_pairs, Qv)
+        costs = compute_contraction_costs(v_hats, valid_pairs, Qv)
+        lowest_cost = np.argmin(costs)
+        v, f = edge_contraction(v, f, valid_pairs[lowest_cost], v_hats[lowest_cost])
+    return v, f
+
+def distribute_field(v, f, field, avg=False):
+    """
+    given a field of size F (with any number of addtional dimensions), distribute it to the vertices of the mesh by summing up the values of the incident faces
+    :param v: vertices of the mesh
+    :param f: faces of the mesh
+    :param field: field of size F
+    :param avg: if True, the field is averaged over the incident faces instead of summed up
+    :return: scalar field of size V
+    """
+    # compute the incident triangles per vertex
+    incident_triangles = compute_incident_triangles(f)
+    # compute the scalar field per vertex
+    field_per_vertex = np.zeros((v.shape[0], *field.shape[1:]))
+    for i, face in enumerate(f):
+        for vertex in face:
+            field_per_vertex[vertex] += field[i]
+    if avg:
+        field_per_vertex /= len(incident_triangles)
+    return field_per_vertex
+
+def distribute_scalar_field(num_vertices, f, per_face_scalar_field, avg=False):
+    """
+    computes a scalar field per vertex by summing / averaging the incident face scalar field
+    :param num_vertices: number of vertices in the mesh
+    :param f: faces of the mesh
+    :param per_face_scalar_field: scalar field of size F
+    :param avg: if True, the field is averaged over the incident faces instead of summed up
+    :return: scalar field of size V
+    """
+    device = f.device
+    incident_face_areas = torch.zeros([num_vertices, 1], device=device)
+    f_unrolled = f.flatten()
+    face_indices_repeated_per_vertex = torch.arange(f.shape[0], device=f.device)
+    face_indices_repeated_per_vertex = torch.repeat_interleave(face_indices_repeated_per_vertex, repeats=3)
+    face_areas_repeated_per_face = per_face_scalar_field[face_indices_repeated_per_vertex].unsqueeze(-1)
+    incident_face_areas = torch.index_add(incident_face_areas, dim=0, index=f_unrolled,
+                                          source=face_areas_repeated_per_face)
+    if avg:
+        neighbors = torch.index_add(torch.zeros_like(incident_face_areas), dim=0, index=f_unrolled,
+                                    source=torch.ones_like(face_areas_repeated_per_face))
+        incident_face_areas = incident_face_areas / neighbors
+    return incident_face_areas
+
+def distribute_vector_field(num_vertices, f, per_face_vector_field):
+    """
+    computes a vector field per vertex by summing the incident face vector field
+    :param num_vertices: number of vertices in the mesh
+    :param f: faces of the mesh
+    :param per_face_vector_field: vector field of size Fx3
+    :return: vector field of size Vx3
+    """
+    device = f.device
+    incident_face_areas = torch.zeros([num_vertices, 1], device=device)
+    f_unrolled = f.flatten()
+    face_indices_repeated_per_vertex = torch.arange(f.shape[0], device=f.device)
+    face_indices_repeated_per_vertex = torch.repeat_interleave(face_indices_repeated_per_vertex, repeats=3)
+    normals_repeated_per_face = per_face_vector_field[face_indices_repeated_per_vertex]
+    normals_repeated_per_face = normals_repeated_per_face
+    incident_face_vectors = torch.zeros([num_vertices,per_face_vector_field.shape[-1]], device=device)
+    incident_face_vectors = torch.index_add(incident_face_vectors, dim=0, index=f_unrolled,
+                                            source=normals_repeated_per_face)
+    return incident_face_vectors
```

### Comparing `gsoup-0.0.8/src/gsoup/geometry_basic.py` & `gsoup-0.0.9/src/gsoup/geometry_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,15 @@
 def remove_unreferenced_vertices(v, f):
     """
     removes unreferenced vertices from a mesh
     :param v: Vx3 np array of vertices
     :param f: Fx3 np array of faces
     :return: the new vertices and faces, and a map from new to old indices (-1 if unreferenced)
     """
-    referenced = np.zeros((v.shape[0]), dtype=np.bool)
+    referenced = np.zeros((v.shape[0]), dtype=bool)
     referenced[f.flatten()] = True
     idx = -1 * np.ones((v.shape[0]), dtype=np.int64)
     idx[referenced] = np.arange(np.sum(referenced), dtype=np.int64)
     f = idx[f.flatten()].reshape((-1, f.shape[1]))
     v = v[referenced]
     return v, f, idx
```

### Comparing `gsoup-0.0.8/src/gsoup/gsoup_io.py` & `gsoup-0.0.9/src/gsoup/gsoup_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     :param path: path to file
     :param to_float: if True, converts image to float
     :param return_paths: if True, returns a list of file paths
     :param to_torch: if True, returns a torch tensor
     :param device: device to load tensor to
     :param resize_wh: a tuple (w, h) to resize the image using nearest neighbor interpolation
     :param as_grayscale: if True, loads image as grayscale by averaging over the channels
-    :return: (b x H x W x 3) tensor, and optionally a list of file names
+    :return: (H x W x C) tensor, and optionally a list of file names
     """
     path = Path(path)
     if not path.exists():
         raise FileNotFoundError("Path does not exist")
     if path.is_dir():
         raise FileNotFoundError("Path must be a file")
     elif path.is_file():
@@ -121,15 +121,15 @@
     :param return_paths: if True, returns a list of file paths
     :param to_torch: if True, returns a torch tensor
     :param device: device to load tensor to
     :param resize_wh: a tuple (w, h) to resize all images using nearest neighbor interpolation
     :param as_grayscale: if True, loads images as grayscale by averaging over the channels
     :return: (b x H x W x C) tensor, and optionally a list of file names
     """
-    supported_suffixes = [".png", ".jpg", ".jpeg"]
+    supported_suffixes = [".png", ".jpg", ".jpeg", ".tiff"]
     if type(source) == list or type(source) == tuple or type(source) == np.ndarray:
         images = []
         file_paths = []
         for p in source:
             p = Path(p)
             if not p.exists():
                 raise FileNotFoundError("Path does not exist")
@@ -199,115 +199,192 @@
                 images = torch.tensor(images, device=device)
             images = images[None, ...]
     if return_paths:
         return images, file_paths
     else:
         return images
 
-def load_mesh(path: Path, to_torch=False, device=None, verbose=True):
+def load_mesh(path: Path,
+              return_vert_uvs=False,
+              return_vert_norms=False,
+              return_vert_color=False,
+              to_torch=False, device=None, verbose=True):
     """
     loads a mesh from a file
     :param path: path to mesh file
     :param to_torch: if True, returns a torch tensor
     :param device: device to load tensor to
     :return: (V x 3) tensor of vertices, (F x 3) tensor of faces, and optionally (V x 3) tensor of normals
     """
     path = Path(path)
     if path.suffix != ".obj":
         raise ValueError("Only .obj are supported")
-    return load_obj(path, to_torch=to_torch, device=device, verbose=verbose)
+    return load_obj(path,
+                    return_vert_uvs=return_vert_uvs,
+                    return_vert_norms=return_vert_norms,
+                    return_vert_color=return_vert_color,
+                    to_torch=to_torch, device=device, verbose=verbose)
 
-def load_obj(path: Path, to_torch=False, device=None, verbose=True):
+def load_obj(path: Path,
+             return_vert_uvs=False,
+             return_vert_norms=False,
+             return_vert_color=False,
+             to_torch=False, device=None, verbose=True):
     """
     :param path: path to obj file
     :param to_torch: if True, returns a torch tensor
     :param device: device to load tensor to
     :return: (V x 3) tensor, (F x 3) tensor, and optionally (V x 3) tensor
     """
     path = Path(path)
     if not path.exists():
         raise ValueError("Path does not exist")
     if not path.is_file():
         raise ValueError("Path must be a file")
     if path.suffix != ".obj":
         raise ValueError("Only .obj are supported")
-    v, f = parse_obj(path, verbose=verbose)
+    v, f, vt, vn, vc, ft, fn = parse_obj(path, verbose=verbose)
     if to_torch and device is not None:
         v = torch.tensor(v, dtype=torch.float, device=device)
-        f = torch.tensor(f,dtype=torch.long, device=device)
+        f = torch.tensor(f, dtype=torch.long, device=device)
         # n = torch.tensor(n, dtype=torch.float, device=device)
-    return v, f
+        if return_vert_norms and vn is not None and fn is not None:
+            vn = torch.tensor(vn, dtype=torch.float, device=device)
+            fn = torch.tensor(fn, dtype=torch.long, device=device)
+        if return_vert_uvs and vt is not None and ft is not None:
+            vt = torch.tensor(vt, dtype=torch.float, device=device)
+            ft = torch.tensor(ft, dtype=torch.long, device=device)
+        if return_vert_color and vc is not None:
+            vc = torch.tensor(vc, dtype=torch.float, device=device)
+    # very ew. consider returning a dict / named tuple ?
+    if return_vert_norms and return_vert_uvs and return_vert_color:
+        return v, f, vt, ft, vn, fn, vc
+    elif return_vert_uvs and return_vert_norms:
+        return v, f, vt, ft, vn, fn
+    elif return_vert_uvs and return_vert_color:
+        return v, f, vt, ft, vc
+    elif return_vert_norms and return_vert_color:
+        return v, f, vn, fn, vc
+    elif return_vert_uvs:
+        return v, f, vt, ft
+    elif return_vert_norms:
+        return v, f, vn, fn
+    elif return_vert_color:
+        return v, f, vc
+    else:
+        return v, f
 
 def parse_obj(path: Path, verbose=True):
     """
     A simple obj parser
     currently supports vertex and triangular face elements only
     """
     path = Path(path)
-    vertexList = []
-    vertexTextureList = []
-    vertexNormalList = []
-    colorList = []
-    faceList = []
+    vertex_list = []
+    vertex_texture_list = []
+    vertex_normal_list = []
+    color_list = []
+    face_list = []
+    face_texture_list = []
+    face_normal_list = []
     finite_flag = False
     with open(path, 'r') as objFile:
         for line in objFile:
             line = line.split("#")[0]  # remove comments
             split = line.split()
             if not len(split):  # skip empty lines
                 continue
             if split[0] == "v":
                 if 3 <= len(split[1:]) <= 4:  # x y z [w]
                     float_vertex = np.array([np.float64(x) for x in split[1:]])
                     if not np.isfinite(float_vertex).all():
                         finite_flag=True
-                    vertexList.append(float_vertex)
+                    vertex_list.append(float_vertex)
                 elif len(split[1:]) == 6:
                     float_vertex = np.array([np.float64(x) for x in split[1:4]])
                     float_color = np.array([np.float64(x) for x in split[4:]])
-                    vertexList.append(float_vertex)
-                    colorList.append(float_color)
+                    if (float_color < 0.0).any() or (float_color > 1.0).any():
+                        raise ValueError("color values must be in [0, 1]")
+                    vertex_list.append(float_vertex)
+                    color_list.append(float_color)
                 else:
-                    raise ValueError("vertex {} has {} entries, but only 3 or 6 are supported".format(len(vertexList), len(split[1:])))
+                    raise ValueError("vertex {} has {} entries, but only 3 or 6 are supported".format(len(vertex_list), len(split[1:])))
             elif split[0] == "f":
                 if len(split[1:]) != 3:
                     raise ValueError("only triangular faces are supported")
                 else:
-                    face = [x.split("/")[0] for x in split[1:]]
-                    int_face = np.array([int(x)-1 for x in face])
+                    face = np.array([x.split("/") for x in split[1:]])
+                    if face.shape == (3, 1):  # v
+                        int_face = face.squeeze().astype(np.int32) - 1
+                        face_list.append(int_face)
+                    elif face.shape == (3, 2):  # v/vt
+                        int_face = face.astype(np.int32) - 1
+                        face_list.append(int_face[:, 0])
+                        face_texture_list.append(int_face[:, 1])
+                    elif face.shape == (3, 3):  # v/vt/vn or v/vn
+                        if np.all([len(x)==0 for x in face[:, 1]]):  # v//vn
+                            face = face[:, 0::2]
+                            int_face = face.astype(np.int32) - 1
+                            face_list.append(int_face[:, 0])
+                            face_normal_list.append(int_face[:, 1])
+                        else:  # v/vt/vn
+                            if np.any([len(x)==0 for x in face[:, 1]]):
+                                raise ValueError("face {} is corrupt".format(len(face_list)))
+                            else:
+                                int_face = face.astype(np.int32) - 1
+                                face_list.append(int_face[:, 0])
+                                face_texture_list.append(int_face[:, 1])
+                                face_normal_list.append(int_face[:, 2])
                     if np.any(int_face < 0):
                         raise ValueError("negative face indices are not supported")
-                    faceList.append(int_face)
             elif split[0] == "vn":
                 if len(split[1:]) != 3:  # xn yn zn
-                    raise ValueError("vertex normal {} has {} entries, but only 3 are supported".format(len(vertexNormalList), len(split[1:])))
+                    raise ValueError("vertex normal {} has {} entries, but only 3 are supported".format(len(vertex_normal_list), len(split[1:])))
                 else:
                     float_vertex_normal = np.array([np.float64(x) for x in split[1:]])
-                    vertexNormalList.append(float_vertex_normal)
+                    vertex_normal_list.append(float_vertex_normal)
             elif split[0] == "vt":
                 if 2 <= len(split[1:]) <= 3:  # u [v, w]
                     float_vertex_tex = np.array([np.float64(x) for x in split[1:]])
                     if (float_vertex_tex < 0).any():
                         raise ValueError("negative texture coordinates are not supported")
                     if (float_vertex_tex > 1).any():
                         raise ValueError("texture coordinates must be between 0 and 1")
-                    vertexTextureList.append(float_vertex_tex)
+                    vertex_texture_list.append(float_vertex_tex)
                 else:
-                    raise ValueError("vertex normal {} has {} entries, but only 3 are supported".format(len(vertexNormalList), len(split[1:])))
+                    raise ValueError("vertex normal {} has {} entries, but only 3 are supported".format(len(vertex_normal_list), len(split[1:])))
             elif split[0] == "l":  # ignore polyline elements
                 continue
             elif split[0] == "vp":  # ignore parameter space vertices
                 continue
-    v = np.stack(vertexList)
-    f = np.stack(faceList)
+    v = np.stack(vertex_list)
+    f = np.stack(face_list)
     if finite_flag and verbose:
         print("Warning: some vertices in file were not finite")
-    # vn = np.stack(vertexNormalList)
-    # vt = np.stack(vertexTextureList)
-    return v, f #, vn, vt
+    if len(vertex_normal_list) > 0:
+        vn = np.stack(vertex_normal_list)
+    else:
+        vn = None
+    if len(vertex_texture_list) > 0:
+        vt = np.stack(vertex_texture_list)
+    else:
+        vt = None
+    if len(color_list) > 0:
+        vc = np.stack(color_list)
+    else:
+        vc = None
+    if len(face_texture_list) > 0:
+        ft = np.stack(face_texture_list)
+    else:
+        ft = None
+    if len(face_normal_list) > 0:
+        fn = np.stack(face_normal_list)
+    else:
+        fn = None
+    return v, f, vt, vn, vc, ft, fn
 
 def save_obj(vertices, faces, path: Path):
     """"
     :param path: path to save obj file to
     :param vertices: (n x 3) tensor of vertices
     :param faces: (m x 3) tensor of vertex indices
     """
```

### Comparing `gsoup-0.0.8/src/gsoup/image.py` & `gsoup-0.0.9/src/gsoup/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,60 @@
 import numpy as np
 import torch
 from PIL import Image, ImageDraw, ImageFont
 from scipy import interpolate, spatial
-from .core import to_8b, to_float, to_hom, homogenize, broadcast_batch, is_np
+from .core import to_8b, to_float, to_hom, homogenize, broadcast_batch, is_np, to_torch
 from .structures import get_gizmo_coords
 from .gsoup_io import save_image
 
-def alpha_compose(images, bg_color=None):
+def alpha_compose(images, backgrounds=None, bg_color=None):
     """
-    composes a single or batch of RGBA images into a single or batch of RGB images
+    composes a single or batch of RGBA images into a single or batch of RGB images.
+    if no backgrounds or bg_color is provided, the background is assumed to be black.
     :param image: b x H x W x 4 or H x W x 4
-    :param bg_color: 3 or b x 3
+    :param background: b x H x W x 3 or H x W x 3
+    :param bg_color: 3 or b x 3 float32 array
     :return: b x H x W x 3 or H x W x 3
     """
     if images.ndim != 3 and images.ndim != 4:
         raise ValueError("image must be 3 or 4 dimensional")
     if images.shape[-1] != 4:
         raise ValueError("image must have 4 channels")
+    if backgrounds is not None:
+        if images.shape[:-1] != backgrounds.shape[:-1]:
+            raise ValueError("backgrounds must have same shape as images")
     if is_np(images):
         if bg_color is None:
             bg_color = np.array([0., 0., 0.]).astype(np.float32)
         if images.dtype != np.float32:
             images = to_float(images)
     else:
         if bg_color is None:
             bg_color = torch.tensor([0., 0., 0.], dtype=images.dtype, device=images.device)
         if images.dtype != torch.float32:
             images = to_float(images)
+    if backgrounds is not None:
+        if backgrounds.dtype != np.float32:
+            backgrounds = to_float(backgrounds)
+        bg_color = backgrounds
     alpha = images[..., 3:4]
     rgb = images[..., :3]
     return alpha * rgb + (1 - alpha) * bg_color
 
 def draw_text_on_image(images, text_per_image, fill_white=True):
     """
     writes text on images given as np array (b x H x W x 3)
     :param images: (b x H x W x 3) numpy array
     :param text_per_image: b x 1 numpy array of strings
     :param fill_white: if True, text is white, otherwise black
     :return: new (b x H x W x 3) numpy array with text written
     """
+    is_numpy = is_np(images)
+    if not is_numpy:
+        device = images.device
     is_float = images.dtype == np.float32
     if is_float:
         images = to_8b(images)
     rgbs = [Image.fromarray(x) for x in images]
     font = ImageFont.truetype("./FreeMono.ttf", 48)
     if fill_white:
         fill = "white"
@@ -50,14 +62,16 @@
         fill = "black"
     for i, rgb in enumerate(rgbs):
         text = text_per_image[i]
         ImageDraw.Draw(rgb).text((0, 0), text, fill=fill, font=font)
     rgbs = np.array([np.asarray(rgb) for rgb in rgbs])
     if is_float:
         rgbs = to_float(rgbs)
+    if not is_numpy:
+        rgbs = to_torch(rgbs, device=device)
     return rgbs
 
 def draw_gizmo_on_image(np_images, w2c, opengl=False, scale=.05):
     """
     adds a gizmo to a batch of np images.
     note: will broadcast np_images and w2c against eachother.
     :param np_images: b x H x W x 3
@@ -168,18 +182,18 @@
 def generate_checkerboard(h, w, blocksize):
     """
     generates a checkerboard pattern
     note: if blocksize is not a divisor of w or h, the pattern will have extra "crops" at the edges
     :param h: height of the image
     :param w: width of the image
     :param blocksize: size of the squares
-    :return: (H x W x 1) numpy array (np.bool)
+    :return: (H x W x 1) numpy array (bool)
     """
     c0, c1 = 0, 1  # color of the squares, for binary these are just 0,1
-    tile = np.array([[c0, c1],[c1, c0]], dtype=np.bool).repeat(blocksize, axis=0).repeat(blocksize, axis=1)[..., None]
+    tile = np.array([[c0, c1],[c1, c0]], dtype=bool).repeat(blocksize, axis=0).repeat(blocksize, axis=1)[..., None]
     grid = np.tile(tile, ( h//(2*blocksize)+1, w//(2*blocksize)+1, 1))
     return grid[:h,:w]
 
 def generate_stripe_pattern(height, width, background="black", direction="vert", thickness=5, spacing=50, dst=None):
     """
     generates an image with colored stripes in a certain direction
     :param height: height of the image
@@ -353,15 +367,18 @@
     :return: grid image
     """
     if images.ndim != 4:
         raise ValueError("images must be a 4D array")
     if len(images) != rows * cols:
         raise ValueError("number of images must be equal to rows * cols")
     tmp = images.reshape(rows, cols, images.shape[1], images.shape[2], -1)
-    result = tmp.transpose(0, 2, 1, 3, 4).reshape(rows * images.shape[1], cols * images.shape[2], -1)
+    if type(tmp) == torch.Tensor:
+        result = tmp.permute(0, 2, 1, 3, 4).reshape(rows * images.shape[1], cols * images.shape[2], -1)
+    elif type(tmp) == np.ndarray:
+        result = tmp.transpose(0, 2, 1, 3, 4).reshape(rows * images.shape[1], cols * images.shape[2], -1)
     return result
 
 def resize_images_naive(images, H, W, channels_last=True, mode="mean"):
     """
     resize images to output_size, but only if the output size has a common divisor of the input size
     :param images: numpy array of images (N x H x W x C)
     :param H: output height size that has a common divisor with the input height size
@@ -386,15 +403,49 @@
         small_images = images.reshape((images.shape[0], output_size[0], bin_size[0], output_size[1], bin_size[1], channels_size)).mean(4).mean(2)
         if images.dtype == np.uint8:
             small_images = small_images.astype(np.uint8)
     else:
         raise ValueError("mode must be one of 'max', 'mean'")
     return small_images
 
-def pad_image_to_res(images, res_h, res_w, bg_color=None):
+def pad_to_square(images, color=None):
+    """
+    pads a batch of images to a square shape
+    note: smaller dimension is padded
+    :param image: numpy image b x h x w x c
+    :param color: color to pad with
+    :return: padded image
+    """
+    if images.ndim != 4:
+        raise ValueError("image must be a 4D array")
+    diff = images.shape[1] - images.shape[2]
+    if diff == 0:
+        return images
+    if diff > 0:
+        return pad_to_res(images, images.shape[1], images.shape[1], color)
+    else:
+        return pad_to_res(images, images.shape[2], images.shape[2], color)
+
+def crop_to_square(images):
+    """
+    crops a batch of images to a square shape
+    note: bigger dimension is cropped
+    :param img: numpy image h x w x c
+    :return: the cropped square image
+    """
+    if images.ndim != 4:
+        raise ValueError("image must be a 4D array")
+    if images.shape[1] > images.shape[2]:
+        s = int((images.shape[1] - images.shape[2]) / 2)
+        return images[s:(s + images.shape[2])]
+    else:
+        s = int((images.shape[2] - images.shape[1]) / 2)
+        return images[:, :, s:(s + images.shape[1])]
+
+def pad_to_res(images, res_h, res_w, bg_color=None):
     """
     pads a batch of numpy images to a specific resolution
     :param image: numpy image b x h x w x c
     :param res_h: height of the output image
     :param res_w: width of the output image
     :param bg_color: background color c (defaults to black)
     :return: padded image b x res_h x res_w x c
```

### Comparing `gsoup-0.0.8/src/gsoup/procam.py` & `gsoup-0.0.9/src/gsoup/procam.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,226 +1,107 @@
 import numpy as np
 import torch
 import cv2
 from .gsoup_io import save_image, save_images, load_images, load_image
 from .core import to_8b
 from .image import interpolate_multi_channel, change_brightness
 from pathlib import Path
+from scipy.interpolate import LinearNDInterpolator
 
-def warp_image(p2c, cam_image, cam_h=None, cam_w=None, output_path=None):
+def warp_image(backward_map, desired_image, cam_wh=None, output_path=None):
     """
-    todo: explain p2c structure
-    given a 2D dense mapping between pixels from optical device 1 to optical device 2,
-    warp an image from optical device 1 to optical device 2
-    :param p2c: 2D dense mapping between pixels from optical device 1 to optical device 2
-    :param cam_image: path to image from optical device 1, or float np array channels last, or pytorch tensor channels last
-    :param cam_h: camera height, if not supplied assumes cam_image is in the correct dimensions in relation to p2c
-    :param cam_w: camera width, if not supplied assumes cam_image is in the correct dimensions in relation to p2c
+    given a 2D dense map of corresponding pixels between projector and camera, computes a warped image such that if projected, the desired image appears when observed using camera
+    :param backward_map: 2D dense mapping between pixels from projector 2 camera (proj_h x proj_w x 2) uint32
+    :param desired_image: path to desired image from camera, or float np array channels last (cam_h x cam_w x 3) uint8
+    :param cam_wh: device1 (width, height) as tuple, if not supplied assumes desired_image is in the correct dimensions in relation to backward_map
     :param output_path: path to save warped image to
-    :return: warped image np array uint8
+    :return: warped image (proj_h x proj_w x 3) uint8
     """
-    if type(cam_image) == np.ndarray:
-        unwarped = torch.tensor(cam_image)
-    elif type(cam_image) == torch.Tensor:
-        unwarped = cam_image
+    if backward_map.ndim != 3:
+        raise ValueError("backward_map must be 3D")
+    if backward_map.shape[-1] != 2:
+        raise ValueError("backward_map must have shape (cam_h, cam_w, 2)")
+    if type(desired_image) == np.ndarray:
+        if desired_image.ndim != 3:
+            raise ValueError("desired_image must be 3D")
     else:
-        unwarped = load_image(cam_image, to_float=True, to_torch=True, resize_wh=(cam_w, cam_h))
-    if unwarped.dtype != torch.float32 and unwarped.dtype != torch.float64:
-        raise ValueError("cam_image must be float32 or float64")
-    if unwarped.ndim != 3:
-        raise ValueError("cam_image must be 3D")
-    if unwarped.shape[2] != 3:
-        raise ValueError("cam_image must be a channels last image.")
-    if cam_h is not None:
-        if unwarped.shape[0] != cam_h:
-            raise ValueError("cam_image must be of shape cam_h, cam_w, 3")
-    if cam_w is not None:
-        if unwarped.shape[1] != cam_w:
-            raise ValueError("cam_image must be of shape cam_h, cam_w, 3")
-    #print(p2c.shape)
-    #p2c = Image.open(Path(interpolated_p2c_path))
-    if type(p2c) != np.ndarray:
-        p2c_data = np.load(p2c)
-    else:
-        p2c_data = p2c.copy()
-    p2c_data = np.asarray(p2c_data)[:, :, :2]
-    #p2c = p2c/255
-    p2c_data[:, :, 0] = (p2c_data[:, :, 0] * 2) - 1
-    p2c_data[:, :, 1] = (p2c_data[:, :, 1] * 2) - 1
-    p2c_data[:, :, [1, 0]] = p2c_data[:, :, [0, 1]]
-    # p2c = np.round(p2c).astype(np.int32)
-    grid = torch.tensor(p2c_data.astype(np.float32)).unsqueeze(0)
-    input = torch.tensor(unwarped).permute(2, 0, 1).unsqueeze(0)
-    warped = torch.nn.functional.grid_sample(input, grid).squeeze().permute(1, 2, 0).numpy()
-    warped_int = to_8b(warped)
+        if cam_wh is not None:
+            desired_image = load_image(desired_image, resize_wh=cam_wh)
+        else:
+            desired_image = load_image(desired_image)
+    warpped = desired_image[(backward_map[..., 0], backward_map[..., 1])]
     if output_path is not None:
-        output_path.parent.mkdir(exist_ok=True, parents=True)
-        save_image(warped_int, output_path)
-    return warped_int
-
-def generate_gray_code(height, width, step, output_dir=None):
-    """
-    generate gray code patterns for structured light scanning
-    :param height: height of the pattern
-    :param width: width of the pattern
-    :param step: step size of the pattern (e.g. 2 means the patterns are half the resolution)
-    :param output_dir: directory to save the patterns to
-    :return: n x height x width array of patterns
-    """
-    gc_height = int((height-1)/step)+1
-    gc_width = int((width-1)/step)+1
-    graycode = cv2.structured_light_GrayCodePattern.create(gc_width, gc_height)
-    patterns = graycode.generate()[1]
-    # decrease pattern resolution
-    exp_patterns = []
-    for pat in patterns:
-        img = np.zeros((height, width), np.uint8)
-        for y in range(height):
-            for x in range(width):
-                img[y, x] = pat[int(y/step), int(x/step)]
-        exp_patterns.append(img)
-    exp_patterns.append(255*np.ones((height, width), np.uint8))  # white
-    exp_patterns.append(np.zeros((height, width), np.uint8))    # black
-    exp_patterns = np.stack(exp_patterns)
-    if output_dir is not None:
-        output_dir = Path(output_dir)
-        output_dir.mkdir(exist_ok=True, parents=True)
-        file_names = ["pattern_{:02d}.png".format(i) for i in range(len(exp_patterns))]
-        save_images(exp_patterns[..., None], output_dir, file_names=file_names)
-    return exp_patterns
+        output_path = Path(output_path)
+        output_path.parent.mkdir(parents=True, exist_ok=True)
+        save_image(warpped, output_path)
+    return warpped
 
-def pix2pix_correspondence(proj_width, proj_height, step, captures,
-                           BLACKTHR = 2, WHITETHR = 30, output_dir=None, verbose=True, debug=False):
-    """
-    finds dense pixel to pixel pix2pix_correspondence between a projector and a camera
-    note: assumes gray code patterns used for projections were generated using generate_gray_code
-    :param proj_width: width of projector
-    :param proj_height: height of projector
-    :param step: step factor used for gray code patterns (e.g. 2 means half resolution)
-    :param captures: the actual n x cam_height x cam_width x 3 captured images, or a directory containing the images
-    :param BLACKTHR: threshold for black pixels
-    :param WHITETHR: threshold for white pixels
-    :param output_dir: directory to save results to
-    :param verbose: if True, prints progress and status
-    :param debug: if True, saves debug images (must provide output_dir)
+def compute_backward_map(proj_wh, forward_map, foreground, output_dir=None, debug=False): 
     """
+    computes the inverse map of forward_map by piece-wise interpolating a triangulated version of it.
+    :param proj_wh: projector (width, height) as a tuple
+    :param forward_map: forward map as a numpy array of shape (height, width, 2) of type int32
+    :param output_dir: directory to save the inverse map to
+    :param debug: if True, saves a visualization of the inverse map to output_dir
+    :return: inverse map as a numpy array of shape (projector_height, projector_width, 2) of type int32
+    """   
     if output_dir is not None:
         output_dir = Path(output_dir)
         output_dir.mkdir(parents=True, exist_ok=True)
-    # prep decoder
-    gc_width = int((proj_width-1)/step)+1
-    gc_height = int((proj_height-1)/step)+1
-    graycode = cv2.structured_light_GrayCodePattern.create(gc_width, gc_height)
-    graycode.setBlackThreshold(BLACKTHR)
-    graycode.setWhiteThreshold(WHITETHR)
-    correct_pattern_amount = graycode.getNumberOfPatternImages() + 2
-    if type(captures) != np.ndarray:
-        captures = load_images(captures)
-    captures = captures.mean(axis=-1).astype(np.uint8)  # convert to grayscale
-    if len(captures) != correct_pattern_amount:
-        raise ValueError('Number of images is not right (right number is {})'.format(correct_pattern_amount))
-    imgs = list(captures)
-    black = imgs.pop()
-    white = imgs.pop()
-    cam_height = white.shape[0]
-    cam_width = white.shape[1]
-    if debug:
-        diff_pic = white.astype(np.uint64) - black.astype(np.uint64)
-        diff_pic[diff_pic < 0] = 0
-        save_image(diff_pic[..., None].astype(np.uint8), Path(output_dir, "white_black_diff.png"))
-        if verbose:
-            print('camera image size :', white.shape)
-    # initialize
-    viz_c2p = np.zeros((cam_height, cam_width, 3), np.float32)
-    ragged_p2c = np.empty((proj_height, proj_width), dtype=object)
-    for i in np.ndindex(ragged_p2c.shape): ragged_p2c[i] = []
-    missing_values_c2p = np.ones((cam_height, cam_width), np.bool8)
-    # c2p
-    c2p_list = [] # [((cam x, y), (proj x, y))]
-    for y in range(cam_height):
-        for x in range(cam_width):
-            if int(white[y, x]) - int(black[y, x]) <= BLACKTHR:  # background
-                continue
-            err, proj_pix = graycode.getProjPixel(imgs, x, y)
-            if not err:
-                fixed_pix = step*(proj_pix[0]+0.5), step*(proj_pix[1]+0.5)  # x, y
-                ragged_p2c[int(fixed_pix[1]), int(fixed_pix[0])].append([y, x])
-                viz_c2p[y, x, :] = [fixed_pix[1] / proj_height, fixed_pix[0] / proj_width, 0.0]
-                missing_values_c2p[y, x] = False
-                c2p_list.append(((x, y), fixed_pix))
-    # p2c
-    total_size = ragged_p2c.size
-    counter = 0
-    for i in range(proj_height):
-        for j in range(proj_width):
-            if verbose:
-                print("{} / {}".format(counter, total_size), end="\r", flush=True)
-            val = np.mean(ragged_p2c[i, j], dtype=np.float32, axis=0)
-            if np.isnan(val).any():
-                val = np.zeros(2)
-            else:
-                val = np.round(val).astype(np.int32)
-            ragged_p2c[i, j] = val
-            counter += 1
-    viz_p2c = np.vstack(ragged_p2c.reshape(-1)).reshape(proj_height, proj_width, 2).astype(np.uint32)
-    viz_p2c = viz_p2c / np.array([cam_height, cam_width], dtype=np.float32)[None, None, :]
-    viz_p2c = np.concatenate((viz_p2c, np.zeros_like(viz_p2c)[:, :, 0:1]), axis=-1)
-    missing_values_p2c = (viz_p2c == 0).all(axis=-1)
-    # interpolate missing values
-    interpolated_c2p = interpolate_multi_channel(viz_c2p, missing_values_c2p)
-    interpolated_p2c = interpolate_multi_channel(viz_p2c, missing_values_p2c)
-    # save results
-    if output_dir is not None:
-        np.save(Path(output_dir, "c2p.npy"), interpolated_c2p) 
-        np.save(Path(output_dir, "p2c.npy"), interpolated_p2c) 
+    data = np.argwhere(foreground)
+    points = forward_map[foreground]
+    interp = LinearNDInterpolator(points, data, fill_value=0.0)
+    X, Y = np.meshgrid(np.arange(proj_wh[1]), np.arange(proj_wh[0]))
+    result = interp(X, Y).transpose(1, 0, 2)  # eww
+    if output_dir:
+        np.save(Path(output_dir, "backward_map.npy"), result)
         if debug:
-            save_image(interpolated_c2p, Path(output_dir, "interpolated_c2p.png"))
-            save_image(interpolated_p2c, Path(output_dir, "interpolated_p2c.png"))
-            save_image(viz_c2p, Path(output_dir, "c2p.png"))
-            save_image(viz_p2c, Path(output_dir, "p2c.png"))
-            if verbose:
-                print('Amount of c2p correspondences :', len(c2p_list))
-    return interpolated_c2p, interpolated_p2c
+            result_normalized = result / np.array([forward_map.shape[0], forward_map.shape[1]])
+            result_normalized_8b = to_8b(result_normalized)
+            result_normalized_8b_3c = np.concatenate((result_normalized_8b, np.zeros_like(result_normalized_8b[..., :1])), axis=-1)
+            save_image(result_normalized_8b_3c, Path(output_dir, "backward_map.png"))
+    return result.round().astype(np.uint32)
 
-def naive_color_compensate(target_image, all_white_image, all_black_image, cam_width, cam_height, brightness_decrease=-127, output_path=None, debug=False):
+def naive_color_compensate(target_image, all_white_image, all_black_image, cam_width, cam_height, brightness_decrease=-127, projector_gamma=2.2, output_path=None, debug=False):
     """
     color compensate a projected image such that it appears closer to a target image from the perspective of a camera
     loosly based on "Embedded entertainment with smart projectors"
     :param target_image the desired image path from the perspective of the camera
     :param all_white_image a path to picture taken by camera when projector had all pixels fully on (float32)
     :param all_black_image a path to picture taken by camera when projector had all pixels fully off (float32)
     :param cam_width camera image width
     :param cam_height camera image height
     :param brightness_decrease a hyper parameter controlling how much the total brightness is decreased. without this, the result is saturated because of dividing by small numbers
+    :param projector_gamma under normal circumstances the projector does not actually output linear values, so we need to compensate for that
     :output_path if passed, result will be saved to this path
-    :debug if true, will save debug info into output_path 
+    :debug if true, will save debug info into output_path parent directory
     """
     if output_path is not None:
         output_path = Path(output_path)
         output_path.parent.mkdir(parents=True, exist_ok=True)
-    target_image = load_image(target_image, to_float=True, resize_wh=(cam_width, cam_height))
+    target_image = load_image(target_image, to_float=True, resize_wh=(cam_width, cam_height))[..., :3]
     target_image = change_brightness(target_image, brightness_decrease)
     if debug:
         save_image(target_image, Path(output_path.parent, "decrease_brightness.png"))
     all_white_image = load_image(all_white_image, to_float=True, resize_wh=(cam_width, cam_height))
     all_black_image = load_image(all_black_image, to_float=True, resize_wh=(cam_width, cam_height))
-    #unwarped_image = np.power(unwarped_image, -2.2)
     compensated = (target_image - all_black_image) / all_white_image
-    compensated = np.power(compensated, (1/2.2))
+    compensated = np.power(compensated, (1/projector_gamma))
     compensated = np.nan_to_num(compensated, nan=0.0, posinf=0.0, neginf=0.0)
     compensated = np.clip(compensated, 0, 1)
     if output_path:
         save_image(compensated, output_path)
     return compensated
 
 def calibrate_procam(proj_height, proj_width, graycode_step, capture_dir, 
                      chess_vert=10, chess_hori=7,
-                     black_thr=40, white_thr=5, chess_block_size=10.0, verbose=True):
+                     black_thr=40, chess_block_size=10.0, verbose=True):
     """
     calibrates a projection-camera pair using local homographies
+    based on "Simple, accurate, and robust projector-camera calibration."
     :param proj_height projector pixel height
     :param proj_width projector pixel width
     :param chess_vert number of cross points of chessboard in vertical direction (not including the border, i.e. internal corners)
     :param chess_hori number of cross points of chessboard in horizontal direction (not including the border, i.e. internal corners)
     :param graycode_step factor used to downsample the graycode images (see generate_gray_code)
     :param capture_dir directory containing the captured images when gray code patterns were projected, assumes structure as follows:
         capture_dir
@@ -228,15 +109,14 @@
                 - 0000.png
                 - 0001.png
                 - ...
             - folder2
                 - 0000.png
                 - ...
     :param black_thr threshold for detecting black pixels in the chessboard
-    :param white_thr threshold for detecting white pixels in the chessboard
     :param chess_block_size size of blocks of chessboard in real world in any unit of measurement (will only effect the translation componenet between camera and projector)
     :param verbose if true, will print out the calibration results
     :return camera intrinsics, camera extrinsics, projector intrinsics, projector extrinsics, cam_proj_rmat, cam_proj_tvec
     """
     proj_shape = (proj_height, proj_width)
     chess_shape = (chess_vert, chess_hori)
     gc_step = graycode_step
@@ -253,87 +133,71 @@
         if len(gc_fnames) == 0:
             continue
         used_dirnames.append(str(dname))
         gc_fname_lists.append([str(x) for x in gc_fnames])
     dirnames = used_dirnames
     objps = np.zeros((chess_shape[0]*chess_shape[1], 3), np.float32)
     objps[:, :2] = chess_block_size * np.mgrid[0:chess_shape[0], 0:chess_shape[1]].T.reshape(-1, 2)
-    gc_height = int((proj_shape[0]-1)/gc_step)+1
-    gc_width = int((proj_shape[1]-1)/gc_step)+1
-    graycode = cv2.structured_light_GrayCodePattern.create(gc_width, gc_height)
-    graycode.setBlackThreshold(black_thr)
-    graycode.setWhiteThreshold(white_thr)
+    graycode = GrayCode()
+    patterns = graycode.encode((proj_shape[1], proj_shape[0]))
     cam_shape = load_image(gc_fname_lists[0][0], as_grayscale=True).shape
     patch_size_half = int(np.ceil(cam_shape[1] / 180))
-    # print('  patch size :', patch_size_half * 2 + 1)
-
     cam_corners_list = []
     cam_objps_list = []
     cam_corners_list2 = []
     proj_objps_list = []
     proj_corners_list = []
     for dname, gc_filenames in zip(dirnames, gc_fname_lists):
-        if len(gc_filenames) != graycode.getNumberOfPatternImages() + 2:
+        if len(gc_filenames) != len(patterns):
             raise ValueError("invalid number of images in " + dname)
-
-        imgs = []
-        for fname in gc_filenames:
-            img = load_image(fname, as_grayscale=True)
-            if cam_shape != img.shape:
-                raise ValueError("image size of {} does not match other images".format(fname))
-            imgs.append(img)
-        black_img = imgs.pop()
-        white_img = imgs.pop()
-
+        imgs = load_images(gc_filenames, as_grayscale=True)[..., None]
+        forwardmap, fg = graycode.decode(imgs, (proj_shape[1], proj_shape[0]), mode="ij")
+        black_img = imgs[-1]
+        white_img = imgs[-2]
+        imgs = imgs[:-2]
         res, cam_corners = cv2.findChessboardCorners(white_img, chess_shape)
         if not res:
             raise RuntimeError("chessboard was not found in {}".format(gc_filenames[-2]))
         cam_objps_list.append(objps)
         cam_corners_list.append(cam_corners)
-
         proj_objps = []
         proj_corners = []
         cam_corners2 = []
-        # viz_proj_points = np.zeros(proj_shape, np.uint8)
         for corner, objp in zip(cam_corners, objps):
             c_x = int(round(corner[0][0]))
             c_y = int(round(corner[0][1]))
             src_points = []
             dst_points = []
+            # todo: vectorize these loops
             for dx in range(-patch_size_half, patch_size_half + 1):
                 for dy in range(-patch_size_half, patch_size_half + 1):
                     x = c_x + dx
                     y = c_y + dy
                     if int(white_img[y, x]) - int(black_img[y, x]) <= black_thr:
                         continue
-                    err, proj_pix = graycode.getProjPixel(imgs, x, y)
-                    if not err:
+                    if fg[y, x]:
+                        proj_pix = forwardmap[y, x]  # backward map ?
                         src_points.append((x, y))
                         dst_points.append(gc_step*np.array(proj_pix))
             if len(src_points) < patch_size_half**2:
                 if verbose:
-                    print('corner {}, {} was skiped because too few decoded pixels found (check your images and threasholds)'.format(c_x, c_y))
+                    print('corner {}, {} was skiped because too few decoded pixels found (check your images and thresholds)'.format(c_x, c_y))
                 continue
             h_mat, inliers = cv2.findHomography(
                 np.array(src_points), np.array(dst_points))
             point = h_mat@np.array([corner[0][0], corner[0][1], 1]).transpose()
             point_pix = point[0:2]/point[2]
             proj_objps.append(objp)
             proj_corners.append([point_pix])
             cam_corners2.append(corner)
-            # viz_proj_points[int(round(point_pix[1])),
-            #                 int(round(point_pix[0]))] = 255
         if len(proj_corners) < 3:
             raise RuntimeError("too few corners were found in {} (less than 3)".format(dname))
         proj_objps_list.append(np.float32(proj_objps))
         proj_corners_list.append(np.float32(proj_corners))
         cam_corners_list2.append(np.float32(cam_corners2))
-        # cv2.imwrite('visualize_corners_projector_' +
-        #             str(cnt) + '.png', viz_proj_points)
-        # cnt += 1
 
     # Initial solution of camera's intrinsic parameters
     ret, cam_int, cam_dist, cam_rvecs, cam_tvecs = cv2.calibrateCamera(
         cam_objps_list, cam_corners_list, cam_shape, None, None, None, None)
     if verbose:
         print('Initial camera intrinsic parameters: {}'.format(cam_int))
         print('Initial camera distortion parameters: {}'.format(cam_dist))
@@ -354,8 +218,130 @@
     if verbose:
         print('RMS: {}'.format(ret))
         print('Camera intrinsic parameters: {}'.format(cam_int))
         print('Camera distortion parameters: {}'.format(cam_dist))
         print('Projector intrinsic parameters: {}'.format(proj_int))
         print('Projector distortion parameters: {}'.format(proj_dist))
         print('Rotation matrix / translation vector from camera to projector (cam2proj transform): {}, {}'.format(cam_proj_rmat, cam_proj_tvec))
-    return cam_int, cam_dist, proj_int, proj_dist, cam_proj_rmat, cam_proj_tvec
+    return cam_int, cam_dist, proj_int, proj_dist, cam_proj_rmat, cam_proj_tvec
+
+class GrayCode:
+    """
+    a class that handles encoding and decoding graycode patterns
+    """
+    def encode1d(self, length):
+        total_images = len(bin(length-1)[2:])
+
+        def xn_to_gray(n, x):
+            # infer a coordinate gray code from its position x and index n (the index of the image out of total_images)
+            # gray code is obtained by xoring the bits of x with itself shifted, and selecting the n-th bit
+            return (x^(x>>1))&(1<<(total_images-1-n))!=0
+        
+        imgs_code = 255*np.fromfunction(xn_to_gray, (total_images, length), dtype=int).astype(np.uint8)
+        return imgs_code
+    
+    def encode(self, proj_wh, flipped_patterns=True):
+        """
+        encode projector's width and height into gray code patterns
+        :param proj_wh: projector's (width, height) in pixels as a tuple
+        :param flipped_patterns: if True, flipped patterns are also generated for better binarization
+        :return: a 3D numpy array of shape (total_images, height, width) where total_images is the number of gray code patterns
+        """
+        width, height = proj_wh
+        codes_width_1d = self.encode1d(width)[:, None, :]
+        codes_width_2d = codes_width_1d.repeat(height, axis=1)
+        codes_height_1d = self.encode1d(height)[:, :, None]
+        codes_height_2d = codes_height_1d.repeat(width, axis=2)
+        
+        img_white = np.full((height, width), 255, dtype=np.uint8)[None, ...]
+        img_black = np.full((height, width),  0, dtype=np.uint8)[None, ...]
+        all_images = np.concatenate((codes_width_2d, codes_height_2d), axis=0)
+        if flipped_patterns:
+            all_images = np.concatenate((all_images, 255-codes_width_2d), axis=0)
+            all_images = np.concatenate((all_images, 255-codes_height_2d), axis=0)
+        all_images = np.concatenate((all_images, img_white, img_black), axis=0)
+        return all_images[..., None]
+    
+    def binarize(self, captures, flipped_patterns=True, bg_threshold=5, bin_threshold=5):
+        """
+        binarize a batch of images
+        :param captures: a 4D numpy array of shape (n, height, width, 1) of captured images
+        :param flipped_patterns: if true, patterns also contain their flipped version for better binarization
+        :param bg_threshold: a threshold used for background detection using the all-white and all-black captures
+        :param bin_threshold: a threshold used for binarization between the flipped and non-flipped patterns
+        :return: a 4D numpy binary array for decoding (total_images, height, width, 1) where total_images is the number of gray code patterns
+        and a binary foreground mask (height, width, 1)
+        """
+        captures, bw = captures[:-2], captures[-2:]
+        foreground = np.abs(bw[0].astype(np.int32) - bw[1].astype(np.int32)) > bg_threshold
+        # img_bin = np.zeros_like(captures, dtype=np.uint8)
+        if flipped_patterns:
+            captures, flipped = captures[:len(captures)//2], captures[len(captures)//2:]
+            valid = np.abs(captures.astype(np.int32) - flipped.astype(np.int32)) > bin_threshold
+            binary = captures > flipped
+            foreground = foreground & np.all(valid, axis=0)  # do not use pixels that do not meet threshold in any of the images
+        else:  # slightly naive threhsolding
+            threhold = 0.5*(bw[1] + bw[0])
+            binary = captures >= threhold
+        return binary, foreground
+
+    def decode1d(self, gc_imgs):
+        # gray code to binary
+        n, h, w = gc_imgs.shape
+        binary_imgs = gc_imgs.copy()
+        for i in range(1, n):  # xor with previous image except MSB
+            binary_imgs[i, :, :] = np.bitwise_xor(binary_imgs[i, :, :], binary_imgs[i-1, :, :])
+        # decode binary
+        cofficient = np.fromfunction(lambda i,y,x: 2**(n-1-i), (n,h,w), dtype=int)
+        img_index = np.sum(binary_imgs * cofficient, axis=0)
+        return img_index
+
+    def decode(self, captures, proj_wh,
+               flipped_patterns=True, bg_threshold=10, bin_threshold=30,
+               mode="xy", output_dir=None, debug=False):
+        """
+        decodes a batch of images encoded with gray code
+        :param captures: a 4D numpy array of shape (n, height, width, c) of captured images
+        :param flipped_patterns: if true, patterns also contain their flipped version for better binarization
+        :param bg_threshold: a threshold used for background detection using teh all-white and all-black captures
+        :param bin_threshold: a threshold used for binarization
+        :param mode: "xy" or "ij" decides the order of last dimension coordinates (ij -> height first, xy -> width first)
+        :return: a 2D numpy array of shape (height, width, 2) specifying the coordinates of decoded result, and foreground mask (height, width)
+        """
+        if captures.ndim != 4:
+            raise ValueError("captures must be a 4D numpy array")
+        if captures.dtype != np.uint8:
+            raise ValueError("captures must be uint8")
+        if output_dir is not None:
+            output_dir = Path(output_dir)
+            output_dir.mkdir(parents=True, exist_ok=True)
+        b, _, _, c = captures.shape
+        b = b - 2 # dont count white and black images
+        if flipped_patterns:
+            b = b // 2  # dont count flipped patterns
+        encoded = self.encode(proj_wh, flipped_patterns)  # sanity: encode with same arguments to verify enough captures are present
+        if len(encoded) != len(captures):
+            raise ValueError("captures must have length of {}".format(len(encoded)))
+        if c != 1:  # naively convert to grayscale
+            captures = captures.mean(axis=-1, keepdims=True).astype(np.uint8)
+        imgs_binary, fg = self.binarize(captures, flipped_patterns, bg_threshold, bin_threshold)
+        imgs_binary = imgs_binary[:, :, :, 0]
+        fg = fg[:, :, 0]
+        x = self.decode1d(imgs_binary[:b // 2])
+        y = self.decode1d(imgs_binary[b // 2:])
+        if mode == "ij":
+            forward_map = np.concatenate((y[..., None], x[..., None]), axis=-1)
+        elif mode == "xy":
+            forward_map = np.concatenate((x[..., None], y[..., None]), axis=-1)
+        else:
+            raise ValueError("mode must be 'ij' or 'xy'")
+        if output_dir is not None:
+            np.save(Path(output_dir, "forward_map.npy"), forward_map)
+            if debug:
+                save_images(imgs_binary[..., None], Path(output_dir, "imgs_binary"))
+                composed = forward_map * fg[..., None]
+                composed_normalized = composed / np.array([proj_wh[1], proj_wh[0]])
+                composed_normalized_8b = to_8b(composed_normalized)
+                composed_normalized_8b_3c = np.concatenate((composed_normalized_8b, np.zeros_like(composed_normalized_8b[..., :1])), axis=-1)
+                save_image(composed_normalized_8b_3c, Path(output_dir, "forward_map.png"))
+        return forward_map, fg
+
```

### Comparing `gsoup-0.0.8/src/gsoup/sphere_trace.py` & `gsoup-0.0.9/src/gsoup/sphere_trace.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.8/src/gsoup/structures.py` & `gsoup-0.0.9/src/gsoup/structures.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.8/src/gsoup/video.py` & `gsoup-0.0.9/src/gsoup/video.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import time
 import collections
 import numpy as np
+import pathlib
 from pathlib import Path
 import ffmpeg
 from .image import resize_images_naive
 import subprocess
+
 def get_ffmpeg_version():
     """
-    returns ffmpeg version
     :return: ffmpeg version
     """
     try:
         ffmpeg_output = subprocess.run(["ffmpeg", "-version"], capture_output=True, text=True).stdout
         parts = ffmpeg_output.split()
         version = parts[parts.index("version") + 1]
         if version[0] != "5":
             print("Warning, detected ffmpeg version: {}. Video module May fail for versions lower than 5".format(version))
     except ValueError:
         print("Warning, could not detect ffmpeg version. Video module May fail")
+    except FileNotFoundError:
+        print("Warning, ffmpeg not found. Video module May fail")
 get_ffmpeg_version()
 
 class FPS:
     """
     calculates current fps and returns it, see https://stackoverflow.com/a/54539292
     example usage:
         fps = FPS()
@@ -85,42 +88,79 @@
     )
     video = np.frombuffer(out, np.uint8).reshape([-1, h, w, 3])
     return video
 
 def save_video(frames, output_path, fps, lossy=False, verbose=False):
     """
     saves a video from a t x h x w x 3 numpy tensor
-    :param frames: (t x h x w x 3) tensor
+    :param frames: (t x h x w x 3) numpy array or directory path containing images of same format and resolution
     :param output_path: path to save video to
     :param fps: frames per second of output video
     :param lossy: if True, use lossy compression (default: False, but then only .avi is supported)
     """
     output_path = Path(output_path)
     output_path.parent.mkdir(parents=True, exist_ok=True)
-    if lossy:
-        (
-        ffmpeg
-        .input('pipe:', format='rawvideo', pix_fmt='rgb24', s='{}x{}'.format(frames.shape[2], frames.shape[1]), r=fps)
-        .output(str(output_path), pix_fmt='yuv420p')
-        .overwrite_output()
-        .run(input=frames.tobytes(), quiet=not verbose)
-        )
-    else:
-        if output_path.suffix == ".avi":
-            pix_fmt = "bgr24"
-        else:
-            # todo: figure out lossless pixel formats for other containers
-            raise ValueError("Lossless video only supported for .avi container")
-        (
+    if type(frames) == np.ndarray:
+        if lossy:
+            (
             ffmpeg
             .input('pipe:', format='rawvideo', pix_fmt='rgb24', s='{}x{}'.format(frames.shape[2], frames.shape[1]), r=fps)
-            .output(str(output_path), vcodec='rawvideo', pix_fmt=pix_fmt)
+            .output(str(output_path), pix_fmt='yuv420p')
             .overwrite_output()
             .run(input=frames.tobytes(), quiet=not verbose)
-        )
+            )
+        else:
+            if output_path.suffix == ".avi":
+                pix_fmt = "bgr24"
+            else:
+                # todo: figure out lossless pixel formats for other containers
+                raise ValueError("Lossless video only supported for .avi container")
+            (
+                ffmpeg
+                .input('pipe:', format='rawvideo', pix_fmt='rgb24', s='{}x{}'.format(frames.shape[2], frames.shape[1]), r=fps)
+                .output(str(output_path), vcodec='rawvideo', pix_fmt=pix_fmt)
+                .overwrite_output()
+                .run(input=frames.tobytes(), quiet=not verbose)
+            )
+    elif isinstance(frames, pathlib.PurePath):
+        if not frames.exists():
+            raise FileNotFoundError("Image directory not found: {}".format(frames))
+        if not frames.is_dir():
+            raise ValueError("frames must be numpy array or path to directory of images")
+        files = sorted(list(frames.glob("*")))
+        if len(files) == 0:
+            raise FileNotFoundError("No images found in directory: {}".format(frames))
+        extensions = []
+        for file in files:
+            extensions.append(file.suffix)
+        if len(set(extensions)) > 1:
+            raise ValueError("All images in directory must have same extension")
+        glob_pattern = str(frames) + "/*" + extensions[0]
+        if lossy:
+            (
+                ffmpeg
+                .input(glob_pattern, pattern_type='glob', framerate=fps)
+                .output(str(output_path))
+                .run(quiet=not verbose)
+            )
+        else:
+            if output_path.suffix == ".avi":
+                pix_fmt = "bgr24"
+            else:
+                # todo: figure out lossless pixel formats for other containers
+                raise ValueError("Lossless video only supported for .avi container")
+            (
+                ffmpeg
+                .input(glob_pattern, pattern_type='glob', pix_fmt='rgb24', r=fps)
+                .output(str(output_path), vcodec='rawvideo', pix_fmt=pix_fmt)
+                .overwrite_output()
+                .run(quiet=not verbose)
+            )
+    else:
+        raise ValueError("frames must be numpy array or path to directory of images")
 
 def reverse_video(video_path, output_path=None, verbose=False):
     """
     reverses a video and possibly saves it to disk
     :param video_path: path to video
     :param output_path: path to save video to
     :return: (n x h x w x 3) tensor of reversed video
```

### Comparing `gsoup-0.0.8/src/gsoup/viewer.py` & `gsoup-0.0.9/src/gsoup/viewer.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.8/src/gsoup/viewer_drivers.py` & `gsoup-0.0.9/src/gsoup/viewer_drivers.py`

 * *Files identical despite different names*

### Comparing `gsoup-0.0.8/src/gsoup.egg-info/SOURCES.txt` & `gsoup-0.0.9/src/gsoup.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/gsoup/geometry_advanced.py
 src/gsoup/geometry_basic.py
 src/gsoup/gsoup_io.py
 src/gsoup/image.py
 src/gsoup/procam.py
 src/gsoup/sphere_trace.py
 src/gsoup/structures.py
+src/gsoup/transforms.py
 src/gsoup/video.py
 src/gsoup/viewer.py
 src/gsoup/viewer_drivers.py
 src/gsoup.egg-info/PKG-INFO
 src/gsoup.egg-info/SOURCES.txt
 src/gsoup.egg-info/dependency_links.txt
 src/gsoup.egg-info/requires.txt
```

### Comparing `gsoup-0.0.8/tests/test_basic.py` & `gsoup-0.0.9/tests/test_basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,22 +173,31 @@
     v, f = gsoup.load_obj("resource/cube.obj")
     assert v.shape[0] == 8
     assert f.shape[0] == 12
 
 def test_image():
     checkboard = gsoup.generate_checkerboard(512, 512, 8)
     gsoup.save_image(checkboard, "resource/checkboard.png")
+    checkboard_RGBA = np.tile(checkboard, (1, 1, 4))
+    checkboard_RGB = gsoup.alpha_compose(checkboard_RGBA, ~checkboard_RGBA[..., :3])
+    assert (checkboard_RGB == 1.0).all()
+    checkboard_RGB = gsoup.alpha_compose(checkboard_RGBA, bg_color=np.array([0.0, 0.0, 1.0]))
+    assert (checkboard_RGB[..., -1] == 1.0).all()
     lollipop_path = Path("resource/lollipop.png")
     lollipop = gsoup.generate_lollipop_pattern(512, 512, dst=lollipop_path)
     gsoup.save_image(lollipop, lollipop_path)
     lollipop2 = gsoup.load_image(lollipop_path)
     assert np.allclose(lollipop, lollipop2)
     gsoup.save_images(lollipop[None, ...], lollipop_path.parent, file_names=["test_save.png"])
-    lollipop_pad = gsoup.pad_image_to_res(lollipop[None, ...], 512, 1024)
+    lollipop_pad = gsoup.pad_to_res(lollipop[None, ...], 512, 1024)
     assert lollipop_pad.shape == (1, 512, 1024, 3)
+    lollipop_padded_square = gsoup.pad_to_square(lollipop_pad)
+    assert lollipop_padded_square.shape == (1, 1024, 1024, 3)
+    lollipop_cropped_square = gsoup.crop_to_square(lollipop_pad)
+    assert lollipop_cropped_square.shape == (1, 512, 512, 3)
     lollipop_srgb = gsoup.linear_to_srgb(lollipop)
     lollipop_linear = gsoup.srgb_to_linear(lollipop_srgb)
     assert np.allclose(lollipop, lollipop_linear)
     gsoup.generate_concentric_circles(256, 512, dst=Path("resource/circles.png"))
     gsoup.generate_stripe_pattern(256, 512, direction="both", dst=Path("resource/stripe.png"))
     gsoup.generate_dot_pattern(512, 256, dst=Path("resource/dots.png"))
     gray1 = gsoup.generate_gray_gradient(256, 256, grayscale=True, dst=Path("resource/gg_vert.png"))
@@ -252,52 +261,73 @@
     assert img.shape == (4, 128, 128, 3)
     img, paths = gsoup.load_images([dst, dst, dst, dst], resize_wh=(128, 256), as_grayscale=True, channels_last=False, return_paths=True, to_float=True, to_torch=True)
     assert len(paths) == 4
     assert img.dtype == torch.float32
     assert img.shape == (4, 256, 128)
 
 def test_video():
+    # import os
+    # FFMPEG_DIR = os.path.join("/usr/bin")
+    # os.environ['PATH'] = FFMPEG_DIR + ":" + os.environ['PATH']
     frame_number = 100
     images = np.random.randint(0, 255, (frame_number, 512, 512, 3), dtype=np.uint8)
     # im1 = gsoup.generate_voronoi_diagram(512, 512, 1000)
     # im2 = gsoup.generate_voronoi_diagram(512, 512, 1000)
     # im1s = np.tile(im1[None, ...], (10, 1, 1, 1))
     # im2s = np.tile(im2[None, ...], (10, 1, 1, 1))
     # images = np.vstack([im1s, im2s])
     dst = Path("resource/noise.avi")
     gsoup.save_video(images, dst, fps=10)
+    gsoup.save_video(images, Path("resource/noise_lossy.avi"), lossy=True, fps=10)
     reader = gsoup.VideoReader(dst, h=512, w=512)
     fps = gsoup.FPS()
     for i, frame in enumerate(reader):
         print("{}: {}, fps: {}".format(i, frame.shape, fps()))
         assert np.all(frame == images[i])
     video_frames = gsoup.load_video(dst)
     assert video_frames.shape == (frame_number, 512, 512, 3)
     assert np.all(video_frames == images)
     video_frames_reversed = gsoup.reverse_video(dst)
     assert (video_frames_reversed[-1] == video_frames[0]).all()
     sliced_frames = gsoup.slice_from_video(dst, every_n_frames=2, start_frame=0, end_frame=6)
     assert (sliced_frames == video_frames[:7:2, :, :, :]).all()
     gsoup.video_to_images(dst, Path("resource/noise"))
+    gsoup.save_video(Path("resource/noise"), Path("resource/noise2.avi"), fps=10)
+    gsoup.save_video(Path("resource/noise"), Path("resource/noise_lossy2.avi"), lossy=True, fps=10)
     discrete_images = gsoup.load_images(Path("resource/noise"))
     assert discrete_images.shape == (frame_number, 512, 512, 3)
     timestamps = gsoup.get_frame_timestamps(dst)
     assert timestamps[0] == 0
 
 def test_procam():
-    gc_patterns = gsoup.generate_gray_code(128, 128, 1)
-    c2p, p2c = gsoup.pix2pix_correspondence(gc_patterns.shape[2], gc_patterns.shape[1],
-                                            1, gc_patterns[..., None].repeat(3, axis=-1),
-                                            verbose=False, debug=True, output_dir=Path("resource/pix2pix"))
+    gray = gsoup.GrayCode()
+    patterns = gray.encode((128, 128))
+    forward_map, fg = gray.decode(patterns, (128, 128),
+                                  output_dir=Path("resource/pix2pix"), mode="ij", debug=True)
+    backward_map = gsoup.compute_backward_map((128, 128), forward_map, fg,
+                                              output_dir=Path("resource/pix2pix"), debug=True)
     desired = gsoup.generate_lollipop_pattern(128, 128)
-    desired = gsoup.to_float(desired)
-    warp_image = gsoup.warp_image(p2c, desired, output_path=Path("resource/warp.png"))
+    # desired = gsoup.to_float(desired)
+    warp_image = gsoup.warp_image(backward_map, desired, cam_wh=(forward_map.shape[1], forward_map.shape[0]),
+                                  output_path=Path("resource/warp.png"))
     assert warp_image.shape == (128, 128, 3)
     assert warp_image.dtype == np.uint8
-    assert np.mean(np.abs(gsoup.to_8b(desired) - warp_image)) < 50  # surely an identity corrospondence & warp can't be too bad
+    assert np.mean(np.abs(desired - warp_image)) < 10  # surely an identity corrospondence & warp can't be too bad
+    calibration_dir = Path("resource/calibration")
+    calibration_dir.mkdir(exist_ok=True, parents=True)
+    checkerboard = gsoup.to_float(gsoup.generate_checkerboard(128, 128, 16))
+    # T = gsoup.random_perspective()
+    # T_opencv = T[:2, :]
+    # img_transformed = cv2.warpPerspective(checkerboard, T, (128, 128))
+    captures = np.bitwise_and(patterns==255, checkerboard[None, ...]==1.0)
+    gsoup.save_images(captures, Path(calibration_dir, "0"))
+    gsoup.save_images(captures, Path(calibration_dir, "1"))
+    cam_int, cam_dist,\
+    proj_int, proj_dist,\
+    cam_proj_rmat, cam_proj_tvec = gsoup.calibrate_procam(128, 128, 1, calibration_dir, chess_vert=7, chess_hori=7)
 
 def test_sphere_tracer():
     image_size = 512
     device = "cuda:0"
     w2v, v2c = gsoup.create_random_cameras_on_unit_sphere(5, 1.0, opengl=True, device=device)
     ray_origins, ray_directions = gsoup.generate_rays(w2v, v2c[0], image_size, image_size, device=device)
     sdf = gsoup.structures.sphere_sdf(0.25)
```

