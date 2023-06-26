# Comparing `tmp/katalytic_images-0.5.0.tar.gz` & `tmp/katalytic_images-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic_images-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "katalytic_images-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `katalytic_images-0.5.0.tar` & `katalytic_images-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.5.0/.coveragerc
--rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.5.0/.gitignore
--rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.5.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     2970 2023-06-02 05:42:41.662349 katalytic_images-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.5.0/README.md
--rw-r--r--   0        0        0     1549 2023-06-02 05:42:41.662349 katalytic_images-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    22846 2023-06-02 05:33:42.682090 katalytic_images-0.5.0/src/katalytic/images.py
--rw-r--r--   0        0        0    16369 2023-06-02 05:38:26.405653 katalytic_images-0.5.0/tests/test_images.py
--rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      109 2023-04-09 19:59:19.451546 katalytic_images-0.6.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-05-01 06:38:08.285250 katalytic_images-0.6.0/.gitignore
+-rw-r--r--   0        0        0     3308 2023-05-05 03:58:55.053635 katalytic_images-0.6.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3500 2023-06-26 19:15:12.396704 katalytic_images-0.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-06 18:07:34.500276 katalytic_images-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2218 2023-05-31 06:28:52.615620 katalytic_images-0.6.0/README.md
+-rw-r--r--   0        0        0     1549 2023-06-26 19:15:12.396704 katalytic_images-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    23183 2023-06-26 19:10:26.536185 katalytic_images-0.6.0/src/katalytic/images.py
+-rw-r--r--   0        0        0    16722 2023-06-26 19:11:21.424280 katalytic_images-0.6.0/tests/test_images.py
+-rw-r--r--   0        0        0     3694 1970-01-01 00:00:00.000000 katalytic_images-0.6.0/PKG-INFO
```

### Comparing `katalytic_images-0.5.0/.gitignore` & `katalytic_images-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.5.0/.gitlab-ci.yml` & `katalytic_images-0.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.5.0/CHANGELOG.md` & `katalytic_images-0.6.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 0.6.0 (2023-06-26)
+### feat
+- [[`7baa7e9`](https://gitlab.com/katalytic/katalytic-images/commit/7baa7e94f5786d23f6f87051e8c87c4cdfec1407)] when passing a PIL.Image to draw() or load_image(), return another PIL.Image
+### refactor
+- [[`eaa3cc6`](https://gitlab.com/katalytic/katalytic-images/commit/eaa3cc61705170539ec7076e63d86395ba57bf19)] make condition more explicit
+- [[`0d16675`](https://gitlab.com/katalytic/katalytic-images/commit/0d16675d3075eae62f31560c1e326a18057009a6)] use errno codes instead of hardcoded numbers
+
+
 ## 0.5.0 (2023-06-02)
 ### feat
 - [[`37afcb5`](https://gitlab.com/katalytic/katalytic-images/commit/37afcb5e74c8f6b081b8261136a873c291358cdd)] load_image(..., *, default=_UNDEFINED) and save_image(..., exists='replace', make_dirs=True, mode='RGB', ...)
 
 
 ## 0.4.1 (2023-05-31)
 ### fix
```

### Comparing `katalytic_images-0.5.0/LICENSE.txt` & `katalytic_images-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.5.0/README.md` & `katalytic_images-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `katalytic_images-0.5.0/pyproject.toml` & `katalytic_images-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-images"
-version = "0.5.0"
+version = "0.6.0"
 description = "This plugin adds utilities for working with images and videos to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `katalytic_images-0.5.0/src/katalytic/images.py` & `katalytic_images-0.6.0/src/katalytic/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import errno
 from pathlib import Path
 
 import cv2
 from cv2 import (
     imwrite as __cv2_imwrite,
     cvtColor as __cv2_cvtColor
 )
@@ -72,15 +73,18 @@
     """
     if not isinstance(before, str):
         raise TypeError(f'type(before) = {type(before)!r}')
     elif not isinstance(after, str):
         raise TypeError(f'type(after) = {type(after)!r}')
 
     return_PIL = isinstance(image, PIL.Image.Image)
-    image = load_image(image)
+    if return_PIL:
+        image = np.array(image)
+    else:
+        image = load_image(image)
 
     conversion_code = f'COLOR_{before}2{after}'
     conversion_code = conversion_code.replace('gray', 'GRAY')
     conversion_code = getattr(cv2, conversion_code, None)
 
     if conversion_code:
         img = __cv2_cvtColor(image, conversion_code)
@@ -288,17 +292,27 @@
     Raises:
         TypeError: If the 'data' parameter is not an iterable of shapes or a dict
         KeyError: If the 'type' key is missing in any shape dictionary.
         ValueError: If the 'type' key in any shape dictionary has an invalid value.
         ValueError: If the 'pts' key in a mask or polylines shape dictionary has an invalid format.
 
     """
-    new_image = image.copy()
+    if isinstance(image, __PIL_Image_Image):
+        new_image = np.array(image)
+        return_PIL = True
+    else:
+        new_image = image.copy()
+        return_PIL = False
+
     draw_inplace(new_image, data)
-    return new_image
+
+    if return_PIL:
+        return PIL.Image.fromarray(new_image)
+    else:
+        return new_image
 
 
 def draw_inplace(image, data):
     """Draws shapes on the input image by modifying it in-place
 
     This function takes an image and an collection specifying the shapes to be drawn on the image. The shapes can include lines, circles, rectangles, text, masks, and polylines. The function iterates over the collection in order and calls the corresponding drawing functions to draw each shape on the image.
 
@@ -465,15 +479,15 @@
 
     if isinstance(image, (str, Path)):
         if not Path(image).exists() and default is not _UNDEFINED:
             return default
         else:
             return __np_array(__PIL_Image_open(image))
     elif isinstance(image, __PIL_Image_Image):
-        return __np_array(image)
+        return image.copy()
     elif isinstance(image, __np_ndarray):
         return image.copy()
     else:
         raise TypeError(f'type(image) = {type(image)!r}')
 
 
 def hwc(arr):
@@ -569,27 +583,27 @@
     if not isinstance(mode, str):
         raise TypeError(f'type(mode) = {type(mode)!r}')
     elif exists not in ('error', 'skip', 'replace'):
         raise ValueError(f'exists must be one of \'error\', \'skip\', \'replace\'. Got {exists!r}')
 
     if Path(path).exists():
         if exists == 'error':
-            raise FileExistsError(f'[Errno 17] File exists: {str(path)!r}')
+            raise FileExistsError(f'[Errno {errno.EEXIST}] File exists: {str(path)!r}')
         elif exists == 'replace':
             pass  # continue executing
         elif exists == 'skip':
             return
 
     dest_dir = Path(path).parent
     if make_dirs:
         make_dir(dest_dir, create_parents=True, exists_ok=True)
     elif not dest_dir.exists():
-        raise FileNotFoundError(f'[Errno 2] Directory does not exist: {str(dest_dir)!r}')
-    elif not dest_dir.is_dir():
-        raise NotADirectoryError(f'[Errno 20] Not a directory: {str(dest_dir)!r}')
+        raise FileNotFoundError(f'[Errno {errno.ENOENT}] Directory does not exist: {str(dest_dir)!r}')
+    elif dest_dir.is_file():
+        raise NotADirectoryError(f'[Errno {errno.ENOTDIR}] Not a directory: {str(dest_dir)!r}')
 
     if isinstance(image, __PIL_Image_Image):
         image = __np_array(image)
 
     if isinstance(image, __np_ndarray):
         if mode != 'BGR':
             image = convert_image(image, mode, 'BGR')
```

### Comparing `katalytic_images-0.5.0/tests/test_images.py` & `katalytic_images-0.6.0/tests/test_images.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,14 +142,22 @@
 
 class Test_draw:
     @pytest.mark.parametrize('wrong_type', all_types_besides('iterables'))
     def test_wrong_type(self, wrong_type):
         with pytest.raises(TypeError):
             draw(np.zeros((5, 5)), wrong_type)
 
+    def test_returns_PIL_if_PIL(self):
+        img = np.zeros((5, 5, 3), dtype=np.uint8)
+        img = PIL.Image.fromarray(img)
+        shape = create_circle((4,4), 2, (0, 0, 255))
+
+        img2 = draw(img, shape)
+        assert isinstance(img2, PIL.Image.Image)
+
     def test_draws_on_a_copy(self):
         img = np.zeros((5, 5, 3), dtype=np.uint8)
         img_copy = img.copy()
         shapes = [
             create_line((0,0), (0,3), (0, 255, 0), thickness=1),
             create_rectangle([1,1], (3,3), (255, 0, 0), thickness=-1),
             create_circle((4,4), 2, (0, 0, 255))
@@ -331,15 +339,18 @@
         save_image(Image.fromarray(image_1), path)
         assert are_arrays_equal(image_1, load_image(path))
 
     def test_load_PIL_Image(self):
         image_1 = _create_RGB()
         path = Path(get_unique_path('{}.png'))
         save_image(image_1, path)
-        assert are_arrays_equal(image_1, load_image(Image.fromarray(image_1)))
+
+        image_2 = load_image(Image.fromarray(image_1))
+        assert are_arrays_equal(image_1, np.array(image_2))
+        assert isinstance(image_2, PIL.Image.Image)
 
     def test_load_returns_copy(self):
         img = _create_RGB()
         img_copy = load_image(img)
         img[0][0] = [255, 255, 255]
         assert not are_arrays_equal(img, img_copy)
```

### Comparing `katalytic_images-0.5.0/PKG-INFO` & `katalytic_images-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: katalytic-images
-Version: 0.5.0
+Version: 0.6.0
 Summary: This plugin adds utilities for working with images and videos to the katalytic namespace
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

