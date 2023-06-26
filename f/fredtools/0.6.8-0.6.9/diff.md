# Comparing `tmp/fredtools-0.6.8-py3-none-any.whl.zip` & `tmp/fredtools-0.6.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 52343 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     8326 b- defN 21-Aug-16 08:11 fredtools/__init__.py
+Zip file size: 54076 bytes, number of entries: 18
+-rw-rw-r--  2.0 unx     8870 b- defN 21-Aug-18 07:29 fredtools/__init__.py
 -rw-rw-r--  2.0 unx    27051 b- defN 21-Aug-06 16:16 fredtools/ft_braggPeak.py
--rw-rw-r--  2.0 unx    16359 b- defN 21-Aug-16 08:25 fredtools/ft_displayImg.py
--rw-rw-r--  2.0 unx     7125 b- defN 21-Aug-16 08:26 fredtools/ft_dvh.py
+-rw-rw-r--  2.0 unx    16206 b- defN 21-Aug-18 07:33 fredtools/ft_displayImg.py
+-rw-rw-r--  2.0 unx     7125 b- defN 21-Aug-16 08:57 fredtools/ft_dvh.py
 -rw-rw-r--  2.0 unx    33964 b- defN 21-Aug-14 09:26 fredtools/ft_imgAnalyse.py
--rw-rw-r--  2.0 unx    30711 b- defN 21-Aug-11 13:57 fredtools/ft_imgGetSubimg.py
--rw-rw-r--  2.0 unx    32445 b- defN 21-Aug-11 13:57 fredtools/ft_imgManipulate.py
+-rw-rw-r--  2.0 unx    30705 b- defN 21-Aug-18 06:36 fredtools/ft_imgGetSubimg.py
+-rw-rw-r--  2.0 unx    39905 b- defN 21-Aug-18 09:25 fredtools/ft_imgManipulate.py
 -rw-rw-r--  2.0 unx     8734 b- defN 21-Aug-06 14:40 fredtools/ft_simTools.py
 -rw-rw-r--  2.0 unx     6918 b- defN 21-Jul-08 11:35 fredtools/smparallel.py
 -rw-rw-r--  2.0 unx       92 b- defN 21-Aug-11 13:57 fredtools/ft_imgIO/__init__.py
--rw-rw-r--  2.0 unx    25420 b- defN 21-Aug-16 08:15 fredtools/ft_imgIO/dicom_io.py
+-rw-rw-r--  2.0 unx    25420 b- defN 21-Aug-16 08:57 fredtools/ft_imgIO/dicom_io.py
 -rw-rw-r--  2.0 unx     2785 b- defN 21-Aug-11 13:57 fredtools/ft_imgIO/dij_io.py
 -rw-rw-r--  2.0 unx     6103 b- defN 21-Aug-06 14:45 fredtools/ft_imgIO/map3d_io.py
 -rw-rw-r--  2.0 unx     4853 b- defN 21-Aug-06 14:46 fredtools/ft_imgIO/mhd_io.py
--rw-rw-r--  2.0 unx     3265 b- defN 21-Aug-16 08:50 fredtools-0.6.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Aug-16 08:50 fredtools-0.6.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 21-Aug-16 08:50 fredtools-0.6.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1475 b- defN 21-Aug-16 08:50 fredtools-0.6.8.dist-info/RECORD
-18 files, 215728 bytes uncompressed, 49947 bytes compressed:  76.8%
+-rw-rw-r--  2.0 unx     3265 b- defN 21-Aug-18 09:26 fredtools-0.6.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 21-Aug-18 09:26 fredtools-0.6.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 21-Aug-18 09:26 fredtools-0.6.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1475 b- defN 21-Aug-18 09:26 fredtools-0.6.9.dist-info/RECORD
+18 files, 223573 bytes uncompressed, 51680 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: fredtools/ft_imgIO/map3d_io.py
 Comment: 
 
 Filename: fredtools/ft_imgIO/mhd_io.py
 Comment: 
 
-Filename: fredtools-0.6.8.dist-info/METADATA
+Filename: fredtools-0.6.9.dist-info/METADATA
 Comment: 
 
-Filename: fredtools-0.6.8.dist-info/WHEEL
+Filename: fredtools-0.6.9.dist-info/WHEEL
 Comment: 
 
-Filename: fredtools-0.6.8.dist-info/top_level.txt
+Filename: fredtools-0.6.9.dist-info/top_level.txt
 Comment: 
 
-Filename: fredtools-0.6.8.dist-info/RECORD
+Filename: fredtools-0.6.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fredtools/__init__.py

```diff
@@ -8,15 +8,15 @@
 from .ft_displayImg import *
 
 import itk
 import SimpleITK as sitk
 
 import sys
 
-version_info = [0, 6, 8]
+version_info = [0, 6, 9]
 __version__ = ".".join(map(str, version_info))
 
 
 def _checkJupyterMode():
     try:
         if get_ipython().config["IPKernelApp"]:
             return True
@@ -187,14 +187,31 @@
     instanceBool = "vector" in img.GetPixelIDTypeAsString()
 
     if raiseError and not instanceBool:
         raise TypeError(f"The object '{type(img)}' is an instance of SimspleITK image but not vector image.")
     return instanceBool
 
 
+def _isSITK_transform(img, raiseError=False):
+    try:
+        return "Transform" in img.GetName()
+    except:
+        if raiseError:
+            raise TypeError(f"The object '{type(img)}' is not an instance of SimspleITK transform object.")
+
+
+def _copyImgMetaData(imgSrc, imgDes):
+    """Copy meta data to the image source to the image destination"""
+    _isSITK(imgSrc, raiseError=True)
+    _isSITK(imgDes, raiseError=True)
+    for key in imgSrc.GetMetaDataKeys():
+        imgDes.SetMetaData(key, imgSrc.GetMetaData(key))
+    return imgDes
+
+
 def SITK2ITK(imgSITK):
     r"""Convert image from SimpleITK.Image object to ITK.Image object."""
     import numpy as np
     import itk
     import SimpleITK as sitk
 
     ft._isSITK(imgSITK, raiseError=True)
```

## fredtools/ft_displayImg.py

```diff
@@ -1,8 +1,8 @@
-def showSlice(ax, imgA=None, imgB=None, plane="XY", point=None, imgCmap="jet", imgROIs=None, doseVmax=None, showLegend=True, fontsize=8, raiseWarrning=True):
+def showSlice(ax, imgA=None, imgB=None, plane="XY", point=None, imgCmap="jet", imgROIs=None, doseVmax=None, showLegend=True, fontsize=8, raiseWarning=True):
     """Display dose slice on a CT slice including contours.
 
     The function displays on `ax` a `plane` going through `point`
     of a 3D image describing dose overlapped on an image of a CT.
     Basically, it forms a simple wrapper to matplotlib.pyplot.imshow
     allowing for a quick display of a slice from a 3D image of dose
     and/or CT.
@@ -39,34 +39,30 @@
     doseVmax : scalar, optional
         Maximum value on dose map. If None then the
         maximum value of 3D dose image will be used (def. None)
     showLegend : bool, optional
         Show legend of the ROI contour names if they exist. (def. True)
     fontsize : scalar, optional
         Basic font size to be used for ticks, labels, legend, etc. (def. 8)
-    raiseWarrning : bool, optional
+    raiseWarning : bool, optional
         Raise warnings. (def. True)
 
     Returns
     -------
     matplotlib.image.AxesImage
         Dose image (or CT image if dose was not given) attached to the axes `ax`.
 
     See Also
     --------
         showSlices: show three projections of an 3D image overlapped on CT, also interactively.
         getSlice: get 2D image slice from SimpleITK Image.
 
     Examples
     --------
-    See example jupyter notebook at [1]_
-
-    References
-    ----------
-    .. [1] `Jupyter notebook of Image Display Tutorial <https://github.com/jasqs/FREDtools/blob/main/examples/Image%20Display%20Tutorial.ipynb>`_
+    See `Jupyter notebook of Image Display Tutorial <https://github.com/jasqs/FREDtools/blob/main/examples/Image%20Display%20Tutorial.ipynb>`_.
     """
     import fredtools as ft
     import numpy as np
     import matplotlib as mpl
     import re
 
     # set background of the axis to black
@@ -118,34 +114,34 @@
         raise ValueError(f"Cannot recognise colormap {imgCmap}.")
 
     # show CT slice
     if imgCT:
         # check if imgCT is a 3D SimpleITK image
         ft._isSITK_volume(imgCT)
 
-        slCT = ft.getSlice(imgCT, point=point, plane=plane, raiseWarrning=raiseWarrning)
+        slCT = ft.getSlice(imgCT, point=point, plane=plane, raiseWarning=raiseWarning)
         axesImage = ax.imshow(ft.arr(slCT), cmap="bone", extent=ft.getExtMpl(slCT))
 
     # show Dose slice
     if imgDose:
         # check if imgDose is a 3D SimpleITK image
         ft._isSITK_volume(imgDose)
 
         # use the maximum value of the 3D dose image as vmax id no doseVmax given
         if not doseVmax:
             statDose = ft.getStatistics(imgDose)
             doseVmax = statDose.GetMaximum()
 
-        slDose = ft.getSlice(imgDose, point=point, plane=plane, raiseWarrning=raiseWarrning)
+        slDose = ft.getSlice(imgDose, point=point, plane=plane, raiseWarning=raiseWarning)
         axesImage = ax.imshow(ft.arr(slDose), cmap=imgCmap, extent=ft.getExtMpl(slDose), alpha=0.7, vmin=0, vmax=doseVmax)
 
     # show ROIs slice
     if imgROIs:
         for imgROI in imgROIs if isinstance(imgROIs, list) else [imgROIs]:
-            slROI = ft.getSlice(imgROI, point=point, plane=plane, raiseWarrning=raiseWarrning)
+            slROI = ft.getSlice(imgROI, point=point, plane=plane, raiseWarning=raiseWarning)
             color = np.array(re.findall("\d+", imgROI.GetMetaData("ROIColor")), dtype="int") / 255
             if ft.getStatistics(slROI).GetMaximum() > 0:
                 plROI = ax.contour(ft.arr(slROI), extent=ft.getExtMpl(slROI), colors=[color], linewidths=1, origin="upper")
                 plROI.collections[0].set_label(imgROI.GetMetaData("ROIName"))
         if len(ax.get_legend_handles_labels()[0]) > 0 and showLegend:
             ax.legend(fontsize=fontsize)
 
@@ -195,19 +191,15 @@
         Colormap to display dose image slice. (def. 'jet')
     interactive : bool, optional
         Display in interactive mode using ipwidgets.
         Works only in jupyter. (def. True)
 
     Examples
     --------
-    See example jupyter notebook at [1]_
-
-    References
-    ----------
-    .. [1] `Jupyter notebook of Image Display Tutorial <https://github.com/jasqs/FREDtools/blob/main/examples/Image%20Display%20Tutorial.ipynb>`_
+    See `Jupyter notebook of Image Display Tutorial <https://github.com/jasqs/FREDtools/blob/main/examples/Image%20Display%20Tutorial.ipynb>`_.
     """
 
     def __init__(self, imgCT, imgDose, imgROIs=None, point=None, DCO=0.1, figsize=[15, 5], imgCmap="jet", interactive=True):
         import ipywidgets as ipyw
         import matplotlib as mpl
         import matplotlib.pyplot as plt
         import fredtools as ft
@@ -217,15 +209,15 @@
 
         self.imgCT = imgCT
         self.imgDose = imgDose
 
         self.imgROIs = imgROIs
 
         # determine point
-        if not point:
+        if not list(point):
             self.point = list(ft.getMassCenter(self.imgDose))
         else:
             self.point = list(point)
 
         # check if point is correct
         if len(self.point) != 3:
             raise ValueError(f"The `point` must be a 3-element vector and is {self.point}.")
@@ -362,25 +354,25 @@
         self.axs[2].axhline(self.point[2])
 
     def showSliceAX0(self, Z):
         import fredtools as ft
 
         self.point[2] = Z
         self.removeArtist(self.axs[0])
-        ft.showSlice(self.axs[0], plane="XY", point=self.point, imgA=self.imgCT, imgB=self.imgDose, imgROIs=self.imgROIs, showLegend=True, imgCmap=self.imgCmap, fontsize=8, raiseWarrning=False)
+        ft.showSlice(self.axs[0], plane="XY", point=self.point, imgA=self.imgCT, imgB=self.imgDose, imgROIs=self.imgROIs, showLegend=True, imgCmap=self.imgCmap, fontsize=8, raiseWarning=False)
         self.replotPointLines()
 
     def showSliceAX1(self, X):
         import fredtools as ft
 
         self.point[0] = X
         self.removeArtist(self.axs[1])
-        ft.showSlice(self.axs[1], plane="ZY", point=self.point, imgA=self.imgCT, imgB=self.imgDose, imgROIs=self.imgROIs, showLegend=True, imgCmap=self.imgCmap, fontsize=8, raiseWarrning=False)
+        ft.showSlice(self.axs[1], plane="ZY", point=self.point, imgA=self.imgCT, imgB=self.imgDose, imgROIs=self.imgROIs, showLegend=True, imgCmap=self.imgCmap, fontsize=8, raiseWarning=False)
         self.replotPointLines()
 
     def showSliceAX2(self, Y):
         import fredtools as ft
 
         self.point[1] = Y
         self.removeArtist(self.axs[2])
-        ft.showSlice(self.axs[2], plane="X-Z", point=self.point, imgA=self.imgCT, imgB=self.imgDose, imgROIs=self.imgROIs, showLegend=True, imgCmap=self.imgCmap, fontsize=8, raiseWarrning=False)
+        ft.showSlice(self.axs[2], plane="X-Z", point=self.point, imgA=self.imgCT, imgB=self.imgDose, imgROIs=self.imgROIs, showLegend=True, imgCmap=self.imgCmap, fontsize=8, raiseWarning=False)
         self.replotPointLines()
```

## fredtools/ft_imgGetSubimg.py

```diff
@@ -38,15 +38,15 @@
             return sitk.sitkBSplineResamplerOrder4
         elif splineOrder == 5:
             return sitk.sitkBSplineResamplerOrder5
     else:
         raise ValueError(f"Interpolation type '{interpolation}' cannot be recognized. Only 'linear', 'nearest' and 'spline' are supported.")
 
 
-def getSlice(img, point, plane="XY", interpolation="linear", splineOrder=3, raiseWarrning=True, displayInfo=False):
+def getSlice(img, point, plane="XY", interpolation="linear", splineOrder=3, raiseWarning=True, displayInfo=False):
     """Get 2D slice from image.
 
     The function calculates a 2D slice image through a specified
     `point` in a specified `plane` from an image defined as SimpleITK
     image object. The slice is returned as an instance of a SimpleITK image
     object of the same dimension but describing a slice (the dimension
     of only two axes are different than one). The slice through a specified
@@ -70,15 +70,15 @@
         with the axes displayed with matplotlib.pyplot.imshow. For instance
         plane `Z-X` will display Z-axis on X-axis in imshow and Y-axis of
         of imshow will be a reversed X-axis of the image. (def. 'XY')
     interpolation : {'linear', 'nearest', 'spline'}, optional
         Determine the interpolation method. (def. 'linear')
     splineOrder : int, optional
         Order of spline interpolation. Must be in range 0-5. (def. 3)
-    raiseWarrning : bool, optional
+    raiseWarning : bool, optional
         Raise warnings. (def. True)
     displayInfo : bool, optional
         Displays a summary of the function results. (def. False)
 
     Returns
     -------
     SimpleITK Image
@@ -146,19 +146,19 @@
     if not (ft._isSITK3D(img) or ft._isSITK4D(img)):
         raise TypeError(f"The object '{type(img)}' is not an instance of a 3D or 4D SimpleITK image.")
 
     # check if point dimension matches the img dim.
     if len(point) != img.GetDimension():
         raise ValueError(f"Dimension of 'point' {point} does not match 'img' dimension {img.GetDimension()}.")
 
-    # set interplator
+    # set interpolator
     interpolator = ft.ft_imgGetSubimg._setSITKInterpolator(interpolation=interpolation, splineOrder=splineOrder)
 
     # check if point is inside the image
-    if not ft.isPointInside(img, point) and raiseWarrning:
+    if not ft.isPointInside(img, point) and raiseWarning:
         warnings.warn(f"Warning: the point {point} is not inside the image extent: {ft.getExtent(img)}.")
 
     # check if plane is in proper format
     plane = plane.upper()
     if not {"X", "Y", "Z", "T", "-", "+"}.issuperset(plane):
         raise ValueError(f"Plane parameter '{plane}' cannot be recognized. Only letters 'X','Y','Z','T','-','+' are supported.")
     if len(plane) > 4:
@@ -221,15 +221,15 @@
         print("# Point: ", np.array(point))
         print("# Plane: '{:s}'".format(plane))
         ft.ft_imgAnalyse._displayImageInfo(sl)
         print("#" * len(f"### {ft._currentFuncName()} ###"))
     return sl
 
 
-def getProfile(img, point, axis="X", interpolation="linear", splineOrder=3, raiseWarrning=True, displayInfo=False):
+def getProfile(img, point, axis="X", interpolation="linear", splineOrder=3, raiseWarning=True, displayInfo=False):
     """Get 1D profile from image along axis.
 
     The function calculates a 1D profile image through a specified
     `point` in a specified `axis` from an image defined as SimpleITK
     image object. The profile is returned as an instance of a SimpleITK image
     object of the same dimension but describing a profile (the dimension
     of only one axes is different than one). The profile through a specified
@@ -249,15 +249,15 @@
         (if no sign provided, then + is assumed). For instance it can be:
         `X`,`Y`,`-Z`, etc. If the minus sign is found, then the
         image is flipped in the following direction.
     interpolation : {'linear', 'nearest', 'spline'}, optional
         Determine the interpolation method. (def. 'linear')
     splineOrder : int, optional
         Order of spline interpolation. Must be in range 0-5. (def. 3)
-    raiseWarrning : bool, optional
+    raiseWarning : bool, optional
         Raise warnings. (def. True)
     displayInfo : bool, optional
         Displays a summary of the function results. (def. False)
 
     Returns
     -------
     SimpleITK Image
@@ -336,19 +336,19 @@
 
     # correct point is needed
     if len(point) < img.GetDimension():
         pointCorr = np.array(img.GetOrigin())
         pointCorr[list(ft.ft_imgAnalyse._getAxesNumberNotUnity(img))] = point
         point = pointCorr
 
-    # set interplator
+    # set interpolator
     interpolator = ft.ft_imgGetSubimg._setSITKInterpolator(interpolation=interpolation, splineOrder=splineOrder)
 
     # check if point is inside the image
-    if not ft.isPointInside(img, point) and raiseWarrning:
+    if not ft.isPointInside(img, point) and raiseWarning:
         warnings.warn(f"Warning: the point {point} is not inside the image extent: {ft.getExtent(img)}.")
 
     # check if axis is in proper format
     axis = axis.upper()
     if not {"X", "Y", "Z", "T", "-", "+"}.issuperset(axis):
         raise ValueError(f"Axis parameter {axis} cannot be recognized. Only letters 'X','Y','Z','T','-','+' are supported.")
     if len(axis) > 2:
@@ -398,15 +398,15 @@
         print("# Point: ", np.array(point))
         print("# Axis: '{:s}'".format(axis))
         ft.ft_imgAnalyse._displayImageInfo(prof)
         print("#" * len(f"### {ft._currentFuncName()} ###"))
     return prof
 
 
-def getPoint(img, point, interpolation="linear", splineOrder=3, raiseWarrning=True, displayInfo=False):
+def getPoint(img, point, interpolation="linear", splineOrder=3, raiseWarning=True, displayInfo=False):
     """Get point value from image.
 
     The function calculates a point value in a specified `point` from an
     image defined as SimpleITK image object. The point is returned as an
     instance of a SimpleITK image object of the same dimension but describing
     a point (the dimension of all axes is equal to one). The point value in
     a specified point is calculated with a specified `interpolation` type.
@@ -419,15 +419,15 @@
         Point to generate the value. It should have length of the image
         dimension. A warning will be generated if the point is not inside
         the image extent.
     interpolation : {'linear', 'nearest', 'spline'}, optional
         Determine the interpolation method. (def. 'linear')
     splineOrder : int, optional
         Order of spline interpolation. Must be in range 0-5. (def. 3)
-    raiseWarrning : bool, optional
+    raiseWarning : bool, optional
         Raise warnings. (def. True)
     displayInfo : bool, optional
         Displays a summary of the function results. (def. False)
 
     Returns
     -------
     SimpleITK Image
@@ -504,19 +504,19 @@
 
     # correct point if needed
     if len(point) < img.GetDimension():
         pointCorr = np.array(img.GetOrigin(), dtype="float64")
         pointCorr[list(ft.ft_imgAnalyse._getAxesNumberNotUnity(img))] = point
         point = pointCorr
 
-    # set interplator
+    # set interpolator
     interpolator = ft.ft_imgGetSubimg._setSITKInterpolator(interpolation=interpolation, splineOrder=splineOrder)
 
     # check if point is inside the image
-    if not ft.isPointInside(img, point) and raiseWarrning:
+    if not ft.isPointInside(img, point) and raiseWarning:
         warnings.warn(f"Warning: the point {point} is not inside the image extent: {ft.getExtent(img)}.")
 
     # generate point value
     pointVal = sitk.Resample(
         img,
         size=[1] * img.GetDimension(),
         outputSpacing=img.GetSpacing(),
@@ -537,15 +537,15 @@
 def getInteg(img, axis="X", displayInfo=False):
     """Get 1D integral profile from image.
 
     The function calculates a 1D integral profile image along specified `axis`
     from an image defined as SimpleITK image object. The integral profile is
     returned as an instance of a SimpleITK image object of the same dimension
     but describing a profile (the dimension of only one axes is different than one).
-    The integral means the sum of the vaxel values multiplied by the voxel volume.
+    The integral means the sum of the voxel values multiplied by the voxel volume.
     The routine is usefull to calculate an integral depth dose (IDD) distributions.
 
     Parameters
     ----------
     img : SimpleITK Image
         Object of a SimpleITK image.
     axis : str, optional
```

## fredtools/ft_imgManipulate.py

```diff
@@ -10,15 +10,15 @@
     of the `img` is not specified, in particular, the Z-spacing does not have to
     be the same as the structure Z-spacing.
 
     Two methods of mapping voxels are available of are available: 'allinside', which
     maps the voxels which are all inside the contour (including voxel size and edges),
     and 'centreInside' (default method), which maps only the centre of the voxels.
 
-    Two algorithms of mapping are available: 'matplotlib', which utilises the
+    Two algorithms of mapping are available: 'matplotlib', which utilizes the
     matplotlib.path.Path.contains_points functionality, and 'smparallel', which exploits
     the algorithm described in [1]_.
 
     .
 
     Parameters
     ----------
@@ -68,28 +68,28 @@
     functionality, it would be recommended to move this functionality to GPU. Such implementation
     is described in [1]_ but has not been tested yet.
 
     3. Two methods of mapping voxels are available of are available: 'allinside', which
     maps the voxels which are all inside the contour (including voxel size and edges),
     and 'centreInside' (default method), which maps only the centre of the voxels.
     Obviously, the 'centreInside' method is faster. On the other hand it usually calculates
-    the volume of the structure sligtly larger than the real volume. Contrary, the 'allinside'
+    the volume of the structure slightly larger than the real volume. Contrary, the 'allinside'
     method should always calculate smaller volume and should converge to the real volume while
-    the `img` resolutiuon increases.
+    the `img` resolution increases.
 
-    4. Two algorithms of mapping are available: 'matplotlib', which utilises the
+    4. Two algorithms of mapping are available: 'matplotlib', which utilizes the
     matplotlib.path.Path.contains_points functionality, and 'smparallel', which exploits
     the algorithm described in [1]_ (search for 'Comparison of different methods') along with numba functionality of
     multiprocessing [2]_ (default algorithm). The 'matplotlib'
     algorithm calculates on a single CPU thread and is the slowest but it does not require
-    any specific modules to be installed (basically the matplotlib) and should work on eny platform.
+    any specific modules to be installed (basically the matplotlib) and should work on any platform.
     The 'smparallel' has been adapted from the above mentioned conversations and no significant
     changes have been made. Nevertheless, it has been tested against clinical Treatment Planning System
     (Varian Eclipse 15.6) and the standard 'matplotlib' method, showing no significant difference.
-    Because, the 'smparallel' method utilises numba module to speed and parallelise the computation,
+    Because, the 'smparallel' method utilizes numba module to speed and parallelise the computation,
     it might happen that it will not work on all platforms. Basically, the numba and tbb packages
     should be installed, but no testing on other platforms has been done.
 
     5. The mapping is done for each contour separately and based on the direction (CW or CCW)
     of the contour it is treated as an inclusive (mask, CW) or exclusive (hole, CCW) contour.
     The mapping of each contour is done in 2D, meaning slice by slice. The resulting image has
     the voxel size and shape the same as the input `img` in X and Y directions. The voxel size
@@ -131,18 +131,18 @@
     if not ft.getDicomType(RSfileName) == "RS":
         raise ValueError(f"The file {RSfileName} is not a proper dicom describing structures.")
 
     # check if method is correct
     if not method.lower() in ["centreinside", "centerinside", "centre", "center", "allinside", "all"]:
         raise ValueError(f"The method '{method}' can not be recognised. Only ('centerinside','allinside') are possible")
 
-    # get structure contour and struct info
+    # get structure contour and structure info
     StructureContours, StructInfo = ft.dicom_io._getStructureContoursByName(RSfileName, structName)
 
-    # add the first point at the end of the contour for each contour (to make shure that the contour is closed)
+    # add the first point at the end of the contour for each contour (to make sure that the contour is closed)
     StructureContours = [np.append(StructureContour, np.expand_dims(StructureContour[0], axis=0), axis=0) for StructureContour in StructureContours]
     # check if all Z positions are the same for each contour
     for StructureContour in StructureContours:
         if not len(np.unique(StructureContour[:, 2])) == 1:
             raise ValueError(f"Not all Z (depth) position in controur are the same.")
     # get depth for each contour
     StructureContoursDepth = np.array([StructureContour[0, 2] for StructureContour in StructureContours])
@@ -291,17 +291,17 @@
     return imgMask
 
 
 def cropImgToMask(img, imgMask, displayInfo=False):
     """Crop image to mask boundary.
 
     The function calculates the boundaries of the `imgMask` defined
-    as an instance of a SinmpleITK image object describing a mask
+    as an instance of a SimpleITK image object describing a mask
     (i.e. type uint8 and only 0/1 values) and crops the `img` defined
-    as an instance of a SinmpleITK image object to these boundaries. The boundaries
+    as an instance of a SimpleITK image object to these boundaries. The boundaries
     mean here the most extreme positions of positive values of the mask in
     each direction. The function exploits SimpleITK.Crop routine.
 
     Parameters
     ----------
     img : SimpleITK Image
         Object of a SimpleITK image.
@@ -343,15 +343,15 @@
     return imgCrop
 
 
 def setValueMask(img, imgMask, value, outside=True, displayInfo=False):
     """Set value inside/outside mask.
 
     The function sets those the values of the `img` defined as an instance of
-    a SinmpleITK object which are inside or outside a mask described by the
+    a SimpleITK object which are inside or outside a mask described by the
     `imgMask` defined as an instance of a SimpleITK object describing a mask
     (i.e. type uint8 and only 0/1 values). The function is a simple wrapper for
     SimpleITK.Mask routine.
 
     Parameters
     ----------
     img : SimpleITK Image
@@ -403,15 +403,15 @@
 def resampleImg(img, spacing, interpolation="linear", splineOrder=3, displayInfo=False):
     """Resample image to other voxel spacing.
 
     The function resamples an image defined as an instance of a
     SimpleITK image object to different voxel spacing using
     a specified interpolation method. The assumption is that
     the 'low extent' is not changed, i.e. the coordinates of
-    the corner of the first volex preserved. The size of
+    the corner of the first voxel preserved. The size of
     the interpolated image is calculated to fit all the voxels' centres
     in the original image extent. The function exploits the
     SimpleITK.Resample routine.
 
     Parameters
     ----------
     img : SimpleITK Image
@@ -449,15 +449,15 @@
         raise ValueError(f"Shape of 'spacing' is {spacing} but must match the dimension of 'img' {img.GetDimension()} or number of nonunity axes {len(ft.ft_imgAnalyse._getAxesNumberNotUnity(img))}.")
     if spacing.size == len(ft.ft_imgAnalyse._getAxesNumberNotUnity(img)):
         spacingCorr = np.array(img.GetSpacing())
         spacingCorr[np.array(ft.ft_imgAnalyse._getAxesNumberNotUnity(img))] = spacing
     else:
         spacingCorr = spacing
 
-    # set interplator
+    # set interpolator
     interpolator = ft.ft_imgGetSubimg._setSITKInterpolator(interpolation=interpolation, splineOrder=splineOrder)
 
     # correct spacing according to image direction
     spacingCorr = np.dot(ft.ft_imgAnalyse._getDirectionArray(img).T, spacingCorr)
 
     # calculate new size
     newSize = np.array(ft.getSize(img)) / np.abs(spacingCorr)
@@ -533,15 +533,15 @@
     return img
 
 
 def createCylindricalMask(img, startPoint, endPoint, dimension, displayInfo=False):
     """Create a cylindrical Mask in image field of reference
 
     The function creates a cylindrical mask with a given `dimension` and height
-    calculated from the starting and ending poits of the cylinder in the frame of
+    calculated from the starting and ending points of the cylinder in the frame of
     references of an image defined as SimpleITK image object describing a 3D image.
     Only 3D images are supported. The routine might be helpful for instance for making
     a geometrical acceptance correction of a chamber used for Bragg peak measurements.
     The routine was adapted from a GitHub repository: https://github.com/heydude1337/SimplePhantomToolkit/.
 
     Parameters
     ----------
@@ -665,7 +665,175 @@
     imgSum = ft.sumImg(imgs)
 
     if displayInfo:
         print(f"### {ft._currentFuncName()} ###")
         ft.ft_imgAnalyse._displayImageInfo(imgSum)
         print("#" * len(f"### {ft._currentFuncName()} ###"))
     return imgSum
+
+
+def _getFORTransformed(img, transform):
+    """Calculate image FOR after transformation.
+
+    The function is calculating a new Field of Reference (FOR) for an image defined
+    as an instance od a SimpleITK image object. The purpose of this calculation is
+    that transformed images can be 'cropped'. This function is calculating new FOR based
+    of the positions of the transformed image corners.
+
+    Parameters
+    ----------
+    img : SimpleITK Image
+        Object of a SimpleITK image.
+    transform : SimpleITK Transform
+        Object of a SimpleITK transform.
+
+    Returns
+    -------
+    size, origin, spacing, direction
+        Calculated image size, origin, spacing (the same as original)
+        and direction (identity).
+
+    Notes
+    -----
+    The implementation was adapted from the idea presented in
+    https://discourse.itk.org/t/dont-lose-data-with-rotation/3325/2
+    """
+    from itertools import product
+    import numpy as np
+    import fredtools as ft
+
+    ft._isSITK(img, raiseError=True)
+    ft._isSITK_transform(transform, raiseError=True)
+
+    startPX = [0, 0, 0]
+    endPX = [int(size) for size in np.array(img.GetSize()) - 1]
+    cornersPX = list(product(*zip(startPX, endPX)))
+    cornersRW = [img.TransformIndexToPhysicalPoint(cornerPX) for cornerPX in cornersPX]
+    cornersRWTransformed = [transform.TransformPoint(cornerRW) for cornerRW in cornersRW]
+    sizeRW = np.max(cornersRWTransformed, 0) - np.min(cornersRWTransformed, 0)
+    originRW = np.min(cornersRWTransformed, 0)
+    sizePX = [int(size) for size in np.ceil((sizeRW + 1) / img.GetSpacing())]
+    spacingRW = img.GetSpacing()
+    directionIdentity = np.identity(img.GetDimension()).flatten().tolist()
+
+    return sizePX, originRW, spacingRW, directionIdentity
+
+
+def getImgBEV(img, isocentrePosition, gantryAngle, couchAngle, defaultPixelValue="auto", interpolation="linear", splineOrder=3, displayInfo=False):
+    """Transform an image to Beam's Eye View (BEV).
+
+    The function transforms a 3D image defined as a SimpleITK 3D image object to
+    the Beam's Eye View (BEV) based on the given isocentre position,
+    gantry angle and couch rotation, using defined interpolation method.
+    The BEV Field of Reference (FOR) means that the Z+ direction is along the field
+    (along the beam of relative position [0,0]) and X/Y positions are consistend with
+    the DICOM and FRED Monte Carlo definitions.
+
+    Parameters
+    ----------
+    img : SimpleITK 3D Image
+        Object of a SimpleITK 3D image.
+    isocentrePosition : array_like, (3x1)
+        Position of the isocentre with respect to the `img` FOR.
+    gantryAngle : scalar
+        Rotation of the gantry around the isocentre position in [deg].
+    couchAngle: scalar
+        Rotation of the couch around the isocentre position in [deg].
+    defaultPixelValue: 'auto' or scalar, optional
+        The value to fill the voxels with, outside the original `img`.
+        If 'auto', then the value will be calculated automatically as the
+        minimum value of the `img`. (def. 'auto')
+    interpolation : {'linear', 'nearest', 'spline'}, optional
+        Determine the interpolation method. (def. 'linear')
+    splineOrder : int, optional
+        Order of spline interpolation. Must be in range 0-5. (def. 3)
+    displayInfo : bool, optional
+        Displays a summary of the function results. (def. False)
+
+    Returns
+    -------
+    SimpleITK 3D Image
+        Object of a transformed SimpleITK 3D image.
+
+    Notes
+    -----
+    The basic workflow follows:
+
+        1. translate the image to the isocentre so to have the isocentre at zero position,
+        2. rotate the couch around the isocentre,
+        3. rotate the gantry around the isocentre,
+        4. rotate and flip image to get BEV.
+
+    Note that the isocentre of the transformed image is at the zero point.
+
+    Note that the isocentre defined in the delivery sequence of the FRED rtplan is
+    a negative isocentre defined in the DICOM RN plan, the couch rotation defined
+    in the delivery sequence of the FRED rtplan is a negative couch rotation defined
+    in the DICOM RN plan, but the gantry rotation defined in the delivery sequence
+    of the FRED rtplan is equal to the gantry rotation the DICOM RN plan.
+    """
+    import numpy as np
+    import SimpleITK as sitk
+    import fredtools as ft
+
+    ft._isSITK3D(img, raiseError=True)
+
+    # set interpolator
+    interpolator = ft.ft_imgGetSubimg._setSITKInterpolator(interpolation=interpolation, splineOrder=splineOrder)
+
+    # check if isocentrePosition dimension matches the img dim.
+    if len(isocentrePosition) != img.GetDimension():
+        raise ValueError(f"Dimension of 'isocentrePosition' {isocentrePosition} does not match 'img' dimension {img.GetDimension()}.")
+
+    # determine default pixelvalue
+    if isinstance(defaultPixelValue, str) and defaultPixelValue.lower() == "auto":
+        defaultPixelValue = ft.getStatistics(img).GetMinimum()
+    elif not np.isscalar(defaultPixelValue):
+        raise ValueError(f"The parameter 'defaultPixelValue' must be a scalar or 'auto'")
+
+    # define translation to isocentre (to have isocentre at the zero position)
+    translationTransformIsocentre = sitk.TranslationTransform(img.GetDimension())
+    translationTransformIsocentre.SetOffset(isocentrePosition)
+
+    # define gantry rotation around the zero position
+    eulerTransformGantry = sitk.Euler3DTransform()
+    eulerTransformGantry.SetRotation(angleX=0, angleY=0, angleZ=np.deg2rad(gantryAngle))
+
+    # define couch rotation around the zero position
+    eulerTransformCouch = sitk.Euler3DTransform()
+    eulerTransformCouch.SetRotation(angleX=0, angleY=np.deg2rad(couchAngle), angleZ=0)
+
+    # define rotation and flipping to get BEV (Z+ along the field) and to be consistent with FRED coordinate system of PB
+    rotateBEVTransform = sitk.Euler3DTransform()
+    rotateBEVTransform.SetRotation(angleX=np.deg2rad(-90), angleY=0, angleZ=0)
+    flipXYTransform = sitk.ScaleTransform(img.GetDimension(), (-1, -1, 1))
+    compositTransformBEV = sitk.CompositeTransform(img.GetDimension())
+    compositTransformBEV.AddTransform(rotateBEVTransform)
+    compositTransformBEV.AddTransform(flipXYTransform)
+
+    # define composite transform
+    compositTransform = sitk.CompositeTransform(img.GetDimension())
+    compositTransform.AddTransform(translationTransformIsocentre)
+    compositTransform.AddTransform(eulerTransformCouch)
+    compositTransform.AddTransform(eulerTransformGantry)
+    compositTransform.AddTransform(compositTransformBEV)
+
+    # calculate new FOR for a new, not cropped image
+    size, origin, spacing, direction = ft.ft_imgManipulate._getFORTransformed(img, compositTransform.GetInverse())
+
+    # make transformation with resampling
+    imgBEV = sitk.Resample(
+        img, transform=compositTransform, size=size, outputOrigin=origin, outputSpacing=spacing, interpolator=interpolator, outputDirection=direction, defaultPixelValue=defaultPixelValue
+    )
+
+    # copy metadata if they exist
+    imgBEV = ft._copyImgMetaData(img, imgBEV)
+
+    if displayInfo:
+        print(f"### {ft._currentFuncName()} ###")
+        print("# Isocentre position [mm]: ", np.array(isocentrePosition))
+        print("# Gantry angle [deg]: {:.1f}".format(gantryAngle))
+        print("# Couch angle [deg]: {:.1f}".format(couchAngle))
+        ft.ft_imgAnalyse._displayImageInfo(imgBEV)
+        print("#" * len(f"### {ft._currentFuncName()} ###"))
+
+    return imgBEV
```

## Comparing `fredtools-0.6.8.dist-info/METADATA` & `fredtools-0.6.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: fredtools
-Version: 0.6.8
+Version: 0.6.9
 Summary: FRED tools is a collection of python functions for image manipulation and analysis. See more on https://github.com/jasqs/FREDtools.
 Home-page: https://github.com/jasqs/FREDtools
 Author: FRED Collaboration
 Author-email: jan.gajewski@ifj.edu.pl
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8,<4.0
 Description-Content-Type: text/markdown
-Requires-Dist: numpy (>=1.17.4)
 Requires-Dist: scipy (>=1.6.3)
-Requires-Dist: pandas (>=1.2.4)
-Requires-Dist: matplotlib (>=3.4.2)
 Requires-Dist: fredtools (>=0.2.10)
-Requires-Dist: lmfit (>=1.0.2)
 Requires-Dist: dicompyler-core (>=0.5.5)
-Requires-Dist: numba (>=0.53.1)
+Requires-Dist: lmfit (>=1.0.2)
 Requires-Dist: itk (>=5.2.0.post2)
 Requires-Dist: pydicom (>=2.1.2)
+Requires-Dist: matplotlib (>=3.4.2)
+Requires-Dist: pandas (>=1.2.4)
+Requires-Dist: numba (>=0.53.1)
+Requires-Dist: numpy (>=1.17.4)
 Requires-Dist: ipython (>=7.26.0)
 Requires-Dist: ipywidgets (>=7.6.3)
 Requires-Dist: psutil (>=5.8.0)
 Requires-Dist: SimpleITK (>=2.1.0)
 
 FRED tools repository
 ================================
```

## Comparing `fredtools-0.6.8.dist-info/RECORD` & `fredtools-0.6.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-fredtools/__init__.py,sha256=uThGHBv4APfOT2FqNw8o2pUA90XP_VJ2YsQ89WqFFBc,8326
+fredtools/__init__.py,sha256=_8p_C1mKdg1jVRwnrWzTHLkmPYVayZnFPJk5SaPy3fM,8870
 fredtools/ft_braggPeak.py,sha256=G85RugkurdVJ8Ae9PaozAI0q2ihAySgEzTvimZiBzR0,27051
-fredtools/ft_displayImg.py,sha256=pP1KO0s0_d8V_PZ0BOmWIqTBy0sebvxia_OGGMuGqhE,16359
+fredtools/ft_displayImg.py,sha256=THYtAA57yclezFJquhalxSNFtakYqd0ZWJD2W4bzOCM,16206
 fredtools/ft_dvh.py,sha256=oGt73xJIPnqzbryBtTzWGBxxv5tc6U5vl3JA220Y3n0,7125
 fredtools/ft_imgAnalyse.py,sha256=E7jZAPnFMbXiNY7KaPo-ucPMdHQ56uhKbdxx5oDvkNA,33964
-fredtools/ft_imgGetSubimg.py,sha256=UXjbj_-jF4l41gxKQDtBmXoMSMyViusHxZBnO14SRKA,30711
-fredtools/ft_imgManipulate.py,sha256=IFoZVWtY3NGi8hh1NHISPZM71_CGaOtIuWjsmyB0fJE,32445
+fredtools/ft_imgGetSubimg.py,sha256=3E9iEDyCGzdOSVPghwq7WNDK2Lxh_h6YTcRa8CB4slU,30705
+fredtools/ft_imgManipulate.py,sha256=AaDireYW2-TLKTOAAs2EnZgaiPe7Hwvg-k3I3simoO0,39905
 fredtools/ft_simTools.py,sha256=vW_IlKPZ_XJ0A6xaRditg9EuNNg1hp9Au_4-y1QCaS4,8734
 fredtools/smparallel.py,sha256=dR_SNGVRPG5SQWIUHhPgqPTt1ygoNR4x_ezieEAhkqg,6918
 fredtools/ft_imgIO/__init__.py,sha256=bvN-rh-hHX62b4z66IA15IZoqr0vdvazdLmv2kUmdDM,92
 fredtools/ft_imgIO/dicom_io.py,sha256=39XeGnVuuBEzkrebtl0_YAONLLC1eVbzeLxSUqTGqrw,25420
 fredtools/ft_imgIO/dij_io.py,sha256=I1pFB6JYHlIBHpBXSXWIAXybjQCdnKID7L5mjaqc7q0,2785
 fredtools/ft_imgIO/map3d_io.py,sha256=vXaFC0aW92_zzxsduZFpNGjU_GDNWfBKBUfkf6lGCjQ,6103
 fredtools/ft_imgIO/mhd_io.py,sha256=bO3GaoystAyHkySwINKIbh5Uy4rz0zthCMZBydosplo,4853
-fredtools-0.6.8.dist-info/METADATA,sha256=x-uGNNh4veZaoP5DQ7cbSTQYQfn8TWwE780IbbDv97M,3265
-fredtools-0.6.8.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-fredtools-0.6.8.dist-info/top_level.txt,sha256=E6A6ysomqbiGakufEZjE4VH4UU1W_mGffZ0qc3OobgM,10
-fredtools-0.6.8.dist-info/RECORD,,
+fredtools-0.6.9.dist-info/METADATA,sha256=ElF6-z4517VAQ7DQ33WwAMmhknPjPfsuhICko7hjyU0,3265
+fredtools-0.6.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+fredtools-0.6.9.dist-info/top_level.txt,sha256=E6A6ysomqbiGakufEZjE4VH4UU1W_mGffZ0qc3OobgM,10
+fredtools-0.6.9.dist-info/RECORD,,
```

