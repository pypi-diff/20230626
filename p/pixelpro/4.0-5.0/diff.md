# Comparing `tmp/pixelpro-4.0-py3-none-any.whl.zip` & `tmp/pixelpro-5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5809 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat    13203 b- defN 23-Jun-23 01:15 pixelpro/__init__.py
--rw-rw-rw-  2.0 fat     1048 b- defN 23-Jun-23 01:24 pixelpro-4.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      364 b- defN 23-Jun-23 01:24 pixelpro-4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-23 01:24 pixelpro-4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-23 01:24 pixelpro-4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      461 b- defN 23-Jun-23 01:24 pixelpro-4.0.dist-info/RECORD
-6 files, 15177 bytes uncompressed, 4975 bytes compressed:  67.2%
+Zip file size: 7313 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat    23229 b- defN 23-Jun-26 01:10 pixelpro/__init__.py
+-rw-rw-rw-  2.0 fat     1048 b- defN 23-Jun-26 01:11 pixelpro-5.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      364 b- defN 23-Jun-26 01:11 pixelpro-5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-26 01:11 pixelpro-5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-26 01:11 pixelpro-5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      461 b- defN 23-Jun-26 01:11 pixelpro-5.0.dist-info/RECORD
+6 files, 25203 bytes uncompressed, 6479 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pixelpro/__init__.py
 Comment: 
 
-Filename: pixelpro-4.0.dist-info/LICENSE.txt
+Filename: pixelpro-5.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pixelpro-4.0.dist-info/METADATA
+Filename: pixelpro-5.0.dist-info/METADATA
 Comment: 
 
-Filename: pixelpro-4.0.dist-info/WHEEL
+Filename: pixelpro-5.0.dist-info/WHEEL
 Comment: 
 
-Filename: pixelpro-4.0.dist-info/top_level.txt
+Filename: pixelpro-5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pixelpro-4.0.dist-info/RECORD
+Filename: pixelpro-5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pixelpro/__init__.py

```diff
@@ -1,13 +1,14 @@
 def index():
     print("""
 
 1)  WAP to demonstrate the following aspects of signal processing on suitable data.
-1a) Upsampling and downsampling on Image/speech signal
-1b) Fast Fourier Transform to compute DFT
+1a) Downsampling on Image/speech signal
+1b) Upsampling on Image/speech signal
+1c) Fast Fourier Transform to compute DFT
 
 2) WAP to perform Convolution and correlation of gray scale image.
 
 3) WAP to perform the DFT of 4x4 Gray Scale Image
 
 4)  Write program to implement point/pixel intensity transformations such as:
 4a) Log and Power-law transformations
@@ -17,119 +18,171 @@
 
 5) WAP to apply various enhancements on images using image derivatives 
    by implementing Gradient and Laplacian operations.
 
 6) WAP to apply various image enhancement using image derivatives by 
    implementing smoothing, sharpening, and unsharp masking filters.
 
-7) WAP to Apply edge detection techniques such as Sobel and Canny 
-   to extract meaningful information
+7) WAP to Apply Edge detection techniques
+7a) Edge detection algorithms (Roberts, Scharr, Sobel, Prewitt, and Laplace)
+     on a grayscale images
+7b) Sobel edge detection algorithm. 
+    visualize the horizontal, vertical, and combined edge information. 
+7c) Edge Detection using Canny Filter for Noisy Images
 
 8) WAP to implement various morphological image processing techniques.
+8a) Erosion and Dilation
+8b) Image opening and closing
 
 9) Image Segmentation.   
 
           """)
           
 
 
 
 def prog(num):
     if(num=="1a"):
         print(""" 
 
+#1a) Code for Down-sampling:
+
+#pip install opencv-python
+#pip install matplotlib
+#pip install numpy
+
 import os
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 
-img1 = cv2.imread("my native place.jpg", 0)
+img1 = cv2.imread('nativeplace.jpg', 0)
 [m, n] = img1.shape
 
 print('Image Shape:', m, n)
 print('Original Image:')
 plt.imshow(img1, cmap="gray")
 plt.show()
 
 f = 4
-
-# Down sample
-img2 = np.zeros((m // f, n // f), dtype=int)
+img2 = np.zeros((m // f, n // f), dtype=np.int_)
 
 for i in range(0, m, f):
     for j in range(0, n, f):
         try:
             img2[i // f][j // f] = img1[i][j]
         except IndexError:
             pass
 
 print('Down Sampled Image:')
 plt.imshow(img2, cmap="gray")
 plt.show()
 
-# Up sample
-img3 = np.zeros((m - 1, n - 1), dtype=int)
+        
+              """) 
+
+        
+    elif(num=="1b"):
+        print("""
+
+#1b) Code for Up-sampling:
+
+#pip install opencv-python
+#pip install matplotlib
+#pip install numpy
+
+import os
+import cv2
+import matplotlib.pyplot as plt
+import numpy as np
+
+img1 = cv2.imread("nativeplace.jpg", 0)
+[m, n] = img1.shape
+
+print('Image Shape:', m, n)
+print('Original Image:')
+plt.imshow(img1, cmap="gray")
+plt.show()
+
+f = 4
+img2 = np.zeros((m//f, n//f), dtype=np.int_)
 
-for i in range(0, m - 1, f):
-    for j in range(0, n - 1, f):
+for i in range(0, m-1, f):
+    for j in range(0, n-1, f):
         try:
-            img3[i, j] = img2[i // f][j // f]
+            img2[i//f][j//f] = img1[i][j]
         except IndexError:
             pass
 
-for i in range(1, m - (f - 1), f):
-    for j in range(0, n - (f - 1)):
-        img3[i:i + (f - 1), j] = img3[i - 1, j]
-
-for i in range(0, m - 1):
-    for j in range(1, n - 1, f):
-        img3[i, j:j + (f - 1)] = img3[i, j - 1]
+img3 = np.zeros((m, n), dtype=np.int_)
+
+for i in range(1, m-(f-1), f):
+    for j in range(0, n-(f-1)):
+        img3[i:i+(f-1), j] = img2[i//f][j//f]
+
+for i in range(0, m-1):
+    for j in range(1, n-1, f):
+        img3[i, j:j+(f-1)] = img3[i, j-1]
 
 print('Up Sampled Image:')
 plt.imshow(img3, cmap="gray")
 plt.show()
-
-              """) 
-
         
-    elif(num=="1b"):
+                """)
+        
+
+    elif(num=="1c"):
         print("""
 
-import cv2
+
+#1c) Fast Fourier Transform to compute DFT
+
+#pip install opencv-python
+#pip install matplotlib
+#pip install Pillow
+#pip install scikit-image
+
+import cv2 # pip install opencv-python
 import matplotlib.pyplot as plt
 import numpy as np
-from PIL import Image
-from skimage.metrics import normalized_root_mse
+from PIL import Image 
+from skimage.metrics import normalized_root_mse 
 
-im = Image.open('elephant.PNG').convert('L')
+im = Image.open('Dark.png').convert('L')
 im = np.array(im)
 freq = np.fft.fft2(im)
 im1 = np.fft.ifft2(freq).real
 snr = normalized_root_mse(im, im1)
 print('SNR for the image obtained after reconstruction =', snr)
 assert np.allclose(im, im1)
 
 plt.figure(figsize=(20, 10))
 plt.subplot(121), plt.imshow(im, cmap='gray'), plt.axis('off')
 plt.title('Original Image', size=20)
 plt.subplot(122), plt.imshow(im1, cmap='gray'), plt.axis('off')
 plt.title('Image Obtained After Reconstruction', size=20)
 plt.show()
 
+
+        
                 """)
         
 
     elif(num=="2"):
         print("""
 
+#pip install opencv-python
+#pip install numpy
+#pip install matplotlib
+        
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 
-image = cv2.imread("my native place.jpg")
+image = cv2.imread("nativeplace.jpg")
 image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
 
 fig, ax = plt.subplots(1, figsize=(12, 8))
 plt.imshow(image)
 plt.show()
 
 abc = np.ones((3, 3))
@@ -147,26 +200,30 @@
 
 img = cv2.filter2D(image, -1, kernel)
 
 fig, ax = plt.subplots(1, 2, figsize=(10, 6))
 ax[0].imshow(image)
 ax[1].imshow(img)
 plt.show()
-
+ 
                 """)
 
 
     elif(num=="3"):
         print("""
 
+#pip install opencv-python
+#pip install numpy
+#pip install matplotlib
+        
 import numpy as np
 import cv2
 from matplotlib import pyplot as plt
 
-img = cv2.imread("puppy.jpg", 0)
+img = cv2.imread("sunflower.jpg", 0)
 rows, cols = img.shape
 optimalRows = cv2.getOptimalDFTSize(rows)
 optimalCols = cv2.getOptimalDFTSize(cols)
 optimalImg = np.zeros((optimalRows, optimalCols))
 optimalImg[:rows, :cols] = img
 dft = cv2.dft(np.float32(optimalImg), flags=cv2.DFT_COMPLEX_OUTPUT)
 dft_shift = np.fft.fftshift(dft)
@@ -188,26 +245,31 @@
     plt.xticks([])
     plt.yticks([])
 
 plt.show()
 cv2.waitKey()
 cv2.destroyAllWindows()
         
+
                 """)
 
 
     elif(num=="4a"):
         print("""
 
-# Log and Power-law transformations
+#4a. Log and Power-law transformations
+
+#pip install opencv-python
+#pip install matplotlib
+
 import cv2
 import numpy as np
 import matplotlib.pyplot as plt
 
-img = cv2.imread("camera_sample.jpg")
+img = cv2.imread("sunflower.jpg")
 
 # Apply log transform.
 c = 255 / (np.log(1 + np.max(img)))
 log_transformed = c * np.log(1 + img)
 
 # Specify the data type.
 log_transformed = np.array(log_transformed, dtype=np.uint8)
@@ -218,35 +280,44 @@
 plt.imshow(img)
 plt.show()
 
 plt.imshow(log_transformed)
 plt.show()
 
 # Open the image.
-img2 = cv2.imread("camera_sample.jpg")
+img2 = cv2.imread("sunflower.jpg")
 plt.imshow(img2)
 plt.show()
 
 # Trying 4 gamma values.
 for gamma in [0.1, 0.5, 1.2, 2.2, 5]:
     # Apply gamma correction.
     gamma_corrected = np.array(255 * (img2 / 255) ** gamma, dtype='uint8')
     cv2.imwrite('gamma_transformed' + str(gamma) + '.jpg', gamma_corrected)
 
     plt.imshow(gamma_corrected)
     plt.show()
 
+        
                 """)
 
 
 
     elif(num=="4b"):
         print(""" 
 
-# Contrast adjustments
+#4b. Contrast adjustments
+
+##pip install numpy
+##pip install scikit-image
+##pip install pillow
+##pip install scipy
+##pip install matplotlib
+##pip install opencv-python
+
 import numpy as np
 from skimage.io import imread
 from skimage.color import rgb2gray
 from skimage import data, img_as_float, img_as_ubyte, exposure, io, color
 from PIL import Image, ImageEnhance, ImageFilter
 from scipy import ndimage, misc
 import matplotlib.pyplot as pylab
@@ -262,15 +333,15 @@
     pylab.hist(np.array(r).ravel(), bins=256, range=(0, 256), color='r', alpha=0.3)
     pylab.hist(np.array(g).ravel(), bins=256, range=(0, 256), color='g', alpha=0.3)
     pylab.hist(np.array(b).ravel(), bins=256, range=(0, 256), color='b', alpha=0.3)
     pylab.xlabel('Pixel Values', size=20)
     pylab.ylabel('Frequency', size=20)
     pylab.title(title, size=10)
 
-im = Image.open("marigold.jpg")
+im = Image.open("sunflower.jpg")
 im_r, im_g, im_b = im.split()
 
 pylab.style.use('ggplot')
 pylab.figure(figsize=(15, 5))
 pylab.subplot(121)
 plot_image(im)
 pylab.subplot(122)
@@ -288,25 +359,30 @@
 pylab.subplot(121)
 plot_image(imc)
 pylab.subplot(122)
 plot_hist(im_rc, im_gc, im_bc)
 pylab.yscale('log')
 pylab.show()
 
+            
         """)
 
     
     elif(num=="4c"):
         print("""
 
-# Histogram equalization
+#4c. Histogram equalization
+
+#pip install opencv-python
+#pip install matplotlib
+
 import cv2
 from matplotlib import pyplot as plt
 
-img = cv2.imread("puppy.jpg", 0)
+img = cv2.imread("HistogramEqu.png", 0)
 hist = cv2.calcHist([img], [0], None, [256], [0, 256])
 eq = cv2.equalizeHist(img)
 cdf = hist.cumsum()
 cdfnmhist = cdf * hist.max() / cdf.max()
 histeq = cv2.calcHist([eq], [0], None, [256], [0, 256])
 cdfeq = histeq.cumsum()
 cdfnmhisteq = cdfeq * histeq.max() / cdf.max()
@@ -314,22 +390,30 @@
 plt.subplot(221), plt.imshow(img, 'gray')
 plt.subplot(222), plt.plot(hist), plt.plot(cdfnmhist)
 plt.subplot(223), plt.imshow(eq, 'gray')
 plt.subplot(224), plt.plot(histeq), plt.plot(cdfnmhisteq)
 plt.xlim([0, 256])
 plt.show()
 
+        
                 """)
 
 
 
     elif(num=="4d"):
         print("""
 
-# Thresholding, and halftoning operations 
+
+#4d. Thresholding, and halftoning operations
+
+#pip install opencv-python
+#pip install numpy
+#pip install matplotlib
+
+
 import cv2 as cv
 import numpy as np
 from matplotlib import pyplot as plt
 
 img = cv.imread("sunflower.jpg", 0)
 ret, thresh1 = cv.threshold(img, 127, 255, cv.THRESH_BINARY)
 ret, thresh2 = cv.threshold(img, 127, 255, cv.THRESH_BINARY_INV)
@@ -343,20 +427,28 @@
 for i in range(6):
     plt.subplot(2, 3, i + 1), plt.imshow(images[i], 'gray', vmin=0, vmax=255)
     plt.title(titles[i])
     plt.xticks([]), plt.yticks([])
 
 plt.show()
 
+        
                 """)
 
 
 
     elif(num=="5"):
         print(""" 
+
+##pip install numpy
+##pip install scipy
+##pip install scikit-image
+##pip install pillow
+##pip install matplotlib
+
 import numpy as np
 from scipy import signal, misc, ndimage
 from skimage import filters, feature, img_as_float
 from skimage.io import imread
 from skimage.color import rgb2gray
 from PIL import Image, ImageFilter
 import matplotlib.pylab as pylab
@@ -395,15 +487,15 @@
 pylab.subplot(232)
 plot_image(im_x, 'Gradient_x')
 pylab.subplot(233)
 plot_image(im_y, 'Gradient_y')
 pylab.subplot(234)
 plot_image(im_mag, '||Gradient||')
 pylab.subplot(235)
-plot_image(im_dir, r'$\theta$')
+plot_image(im_dir, r'$	heta$')
 pylab.subplot(236)
 pylab.plot(range(im.shape[1]), im[0, :], 'b-', label=r'$f(x,y)|_{x=0}$', linewidth=5)
 pylab.plot(range(im.shape[1]), im_x[0, :], 'r-', label=r'$grad_x (f(x,y))|_{x=0}$')
 pylab.title(r'$grad_x (f(x,y))|_{x=0}$', size=30)
 pylab.legend(prop={'size': 20})
 pylab.show()
 
@@ -420,20 +512,27 @@
 pylab.figure(figsize=(20, 10))
 pylab.subplot(121)
 plot_image(im, 'Original')
 pylab.subplot(122)
 plot_image(im1, 'Laplacian Convolved')
 pylab.show()
 
+      
+
         """)
     
     
     elif(num=="6"):
         print("""
 
+##pip install numpy
+##pip install scipy
+##pip install scikit-image
+##pip install matplotlib
+
 import numpy as np
 from scipy import ndimage
 from skimage import img_as_float
 from skimage.io import imread
 from skimage.color import rgb2gray
 from skimage.filters import laplace
 import matplotlib.pylab as pylab
@@ -492,37 +591,333 @@
     im_sharp = np.clip(im + alpha[i] * im_detail, 0, 1)
     axes[2].imshow(im_sharp)
     axes[2].set_title('Sharpened Image', size=15)
     ax.axis('off')
 
 fig.tight_layout()
 pylab.show()
-        
+               
                 """)
 
 
 
-    elif(num=="7"):
+    elif(num=="7a"):
         print("""
+#7a) Edge detection algorithms (Roberts, Scharr, Sobel, Prewitt, and Laplace)
+#    on a grayscale images 
+
+#pip install numpy
+#pip install scipy
+#pip install scikit-image
+#pip install pillow
+#pip install matplotlib
+
+import numpy as np
+from scipy import signal, misc, ndimage
+from skimage import filters, feature, img_as_float
+from skimage.io import imread
+from skimage.color import rgb2gray
+from PIL import Image, ImageFilter
+import matplotlib.pylab as pylab
+from skimage.transform import rescale
+
+def plot_image(image, title=""):
+    pylab.title(title, size=10)
+    pylab.imshow(image)
+    pylab.axis('off')
+
+def plot_hist(r, g, b, title=""):
+    r, g, b = r.astype(np.uint8), g.astype(np.uint8), b.astype(np.uint8)
+    pylab.hist(np.array(r).ravel(), bins=256, range=(0, 256), color='r', alpha=0.3)
+    pylab.hist(np.array(g).ravel(), bins=256, range=(0, 256), color='g', alpha=0.3)
+    pylab.hist(np.array(b).ravel(), bins=256, range=(0, 256), color='b', alpha=0.3)
+    pylab.xlabel('Pixel Values', size=20)
+    pylab.ylabel('Frequency', size=20)
+    pylab.title(title, size=10)
+
+# Edge Detectors with scikit-image-Prewitt, roberts, sobel, scharr, laplace
+im = Image.open("sunflower.jpg").convert('L')
+im_arr = np.asarray(im)
+pylab.gray()
+pylab.figure(figsize=(15, 15))
+pylab.subplot(3, 2, 1), plot_image(im, 'Original Image')
+edges = filters.roberts(im_arr)
+pylab.subplot(3, 2, 2), plot_image(edges, 'Roberts')
+edges = filters.scharr(im_arr)
+pylab.subplot(3, 2, 3), plot_image(edges, 'Scharr')
+edges = filters.sobel(im_arr)
+pylab.subplot(3, 2, 4), plot_image(edges, 'Sobel')
+edges = filters.prewitt(im_arr)
+pylab.subplot(3, 2, 5), plot_image(edges, 'Prewitt')
+edges = np.clip(filters.laplace(im_arr), 0, 1)
+pylab.subplot(3, 2, 6), plot_image(edges, 'Laplace')
+pylab.subplots_adjust(wspace=0.1, hspace=0.1)
+pylab.show()
+
 
                 """)
+    
+    elif(num=="7b"):
+        print("""
 
+#7b) Sobel edge detection algorithm.
+#    visualize the horizontal, vertical, and combined edge information.
 
+#pip install numpy
+#pip install scipy
+#pip install scikit-image
+#pip install matplotlib
 
-    elif(num=="8"):
+import numpy as np
+from scipy import signal, misc, ndimage
+from skimage import filters, feature, img_as_float
+from skimage.io import imread
+from skimage.color import rgb2gray
+from PIL import Image, ImageFilter
+from matplotlib import pyplot as plt
+import matplotlib.pylab as pylab
+from skimage.transform import rescale
+
+def plot_image(image, title=""):
+    pylab.title(title, size=10)
+    pylab.imshow(image)
+    pylab.axis('off')
+
+def plot_hist(r, g, b, title=""):
+    r, g, b = r.astype(np.uint8), g.astype(np.uint8), b.astype(np.uint8)
+    pylab.hist(np.array(r).ravel(), bins=256, range=(0, 256), color='r', alpha=0.3)
+    pylab.hist(np.array(g).ravel(), bins=256, range=(0, 256), color='g', alpha=0.3)
+    pylab.hist(np.array(b).ravel(), bins=256, range=(0, 256), color='b', alpha=0.3)
+    pylab.xlabel('Pixel Values', size=20)
+    pylab.ylabel('Frequency', size=20)
+    pylab.title(title, size=10)
+
+# SOBEL
+im = Image.open("sunflower.jpg").convert('L')
+im_array = np.asarray(im)
+pylab.gray()
+pylab.figure(figsize=(15, 15))
+pylab.subplot(2, 2, 1), plot_image(im, 'Original')
+pylab.subplot(2, 2, 2)
+edges_x = filters.sobel_h(im_array)
+plot_image(np.clip(edges_x, 0, 1), 'sobel_x')
+pylab.subplot(2, 2, 3)
+edges_y = filters.sobel_v(im_array)
+plot_image(np.clip(edges_y, 0, 1), 'Sobel_y')
+pylab.subplot(2, 2, 4)
+edges = filters.sobel(im_array)
+plot_image(np.clip(edges, 0, 1), 'Sobel')
+pylab.subplots_adjust(wspace=0.1, hspace=0.1)
+pylab.show()
+plt.show()
+
+
+                """)
+        
+    elif(num=="7c"):
         print("""
- 
+
+
+#7c) Edge Detection using Canny Filter for Noisy Images
+
+#pip install scipy
+#pip install scikit-image
+#pip install matplotlib
+
+import matplotlib.pyplot as plt
+from scipy import ndimage as ndi
+from skimage.util import random_noise
+from skimage import feature
+import numpy as np
+
+# Generate noisy image of a square
+image = np.zeros((128, 128), dtype=float)
+image[32:-32, 32:-32] = 1
+image = ndi.rotate(image, 15, mode='constant')
+image = ndi.gaussian_filter(image, 4)
+image = random_noise(image, mode='speckle', mean=0.05)
+
+# Compute the Canny filter for two values of sigma
+edges1 = feature.canny(image)
+edges2 = feature.canny(image, sigma=3)
+
+# Display results
+fig, ax = plt.subplots(nrows=1, ncols=3, figsize=(8, 3))
+ax[0].imshow(image, cmap='gray')
+ax[0].set_title('noisy image', fontsize=10)
+ax[1].imshow(edges1, cmap='gray')
+ax[1].set_title(r'Canny filter, $\sigma=1$', fontsize=10)
+ax[2].imshow(edges2, cmap='gray')
+ax[2].set_title(r'Canny filter, $\sigma=3$', fontsize=10)
+
+for a in ax:
+    a.axis('off')
+
+fig.tight_layout()
+plt.show()
+
+        
+                """)
+
+
+
+
+    elif(num=="8a"):
+        print("""
+
+#8a) Erosion and Dilation
+
+#pip install opencv-python
+#pip install matplotlib
+
+import cv2
+import numpy as np
+from matplotlib import pyplot as plt
+
+img = cv2.imread("sunflower.jpg", 0)
+ret, bw_img = cv2.threshold(img, 127, 255, cv2.THRESH_BINARY)
+kernel = np.ones((5, 5), np.uint8)
+img_erosion = cv2.erode(img, kernel, iterations=1)
+img_dilation = cv2.dilate(img, kernel, iterations=1)
+
+plt.figure(figsize=(5, 5))
+plt.imshow(img, cmap="gray")
+plt.axis('off')
+plt.title("ORIGINAL IMAGE")
+plt.show()
+
+plt.figure(figsize=(5, 5))
+plt.imshow(img_erosion)
+plt.axis('off')
+plt.title("EROSION")
+plt.show()
+
+plt.figure(figsize=(5, 5))
+plt.imshow(img_dilation, cmap="gray")
+plt.axis('off')
+plt.title("DILATION")
+plt.show()
+
+         
                 """)
 
+    elif(num=="8b"):
+        print("""
+ 
 
+#8b) Image opening and closing
+
+#pip install scikit-image
+#pip install matplotlib
+
+from skimage.morphology import binary_opening, binary_closing, disk
+from skimage.color import rgb2gray
+from skimage.io import imread
+import matplotlib.pyplot as plt
+
+def plot_image(image, title=""):
+    plt.title(title, size=10)
+    plt.imshow(image, cmap='gray')
+    plt.axis('off')
+
+im = rgb2gray(imread("sunflower.jpg"))
+im[im <= 0.5] = 0
+im[im > 0.5] = 1
+
+plt.gray()
+plt.figure(figsize=(20, 10))
+
+plt.subplot(1, 3, 1)
+plot_image(im, 'original')
+
+im1 = binary_opening(im, disk(6))
+plt.subplot(1, 3, 2)
+plot_image(im1, 'opening with disk size ' + str(10))
+
+im1 = binary_closing(im, disk(6))
+plt.subplot(1, 3, 3)
+plot_image(im1, 'closing with disk size ' + str(6))
+
+plt.show()
+
+        
+                """)
 
 
     elif(num=="9"):
         print("""
 
+#pip install numpy
+#pip install opencv-python
+#pip install matplotlib
+        
+import numpy as np
+import cv2
+from matplotlib import pyplot as plt
+
+# Loading original image
+img = cv2.imread('Original_img_segmentation.png')
+img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+
+plt.figure(figsize=(8, 8))
+plt.imshow(img, cmap="gray")
+plt.axis('off')
+plt.title("Original Image")
+plt.show()
+
+# Converting to grayscale
+gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+
+plt.figure(figsize=(8, 8))
+plt.imshow(gray, cmap="gray")
+plt.axis('off')
+plt.title("Grayscale Image")
+plt.show()
+
+# Converting to binary inverted image
+ret, thresh = cv2.threshold(gray, 0, 255, cv2.THRESH_BINARY_INV + cv2.THRESH_OTSU)
+
+plt.figure(figsize=(8, 8))
+plt.imshow(thresh, cmap="gray")
+plt.axis('off')
+plt.title("Threshold Image")
+plt.show()
+
+# Segmenting the images
+kernel = np.ones((3, 3), np.uint8)
+closing = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel, iterations=15)
+bg = cv2.dilate(closing, kernel, iterations=1)
+dist_transform = cv2.distanceTransform(closing, cv2.DIST_L2, 0)
+ret, fg = cv2.threshold(dist_transform, 0.02 * dist_transform.max(), 255, 0)
+
+plt.figure(figsize=(8, 8))
+plt.imshow(fg, cmap="gray")
+plt.axis('off')
+plt.title("Segmented Image")
+plt.show()
+
+# Final output
+plt.figure(figsize=(10, 10))
+plt.subplot(2, 2, 1)
+plt.axis('off')
+plt.title("Original Image")
+plt.imshow(img, cmap="gray")
+plt.subplot(2, 2, 2)
+plt.imshow(gray, cmap="gray")
+plt.axis('off')
+plt.title("Grayscale Image")
+plt.subplot(2, 2, 3)
+plt.imshow(thresh, cmap="gray")
+plt.axis('off')
+plt.title("Threshold Image")
+plt.subplot(2, 2, 4)
+plt.imshow(fg, cmap="gray")
+plt.axis('off')
+plt.title("Segmented Image")
+plt.show()
 
                 """)
 
 
 
 
     else:
```

## Comparing `pixelpro-4.0.dist-info/LICENSE.txt` & `pixelpro-5.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

