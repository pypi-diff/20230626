# Comparing `tmp/breizorro-0.1.1.tar.gz` & `tmp/breizorro-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breizorro-0.1.1.tar", last modified: Mon Jan  9 12:53:41 2023, max compression
+gzip compressed data, was "breizorro-0.1.2.tar", max compression
```

## Comparing `breizorro-0.1.1.tar` & `breizorro-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,6 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:53:41.980476 breizorro-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-01-09 12:53:41.000000 breizorro-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-09 12:53:41.000000 breizorro-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-01-09 12:53:41.976476 breizorro-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-01-09 12:53:41.000000 breizorro-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:53:41.976476 breizorro-0.1.1/breizorro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 12:53:41.000000 breizorro-0.1.1/breizorro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:53:41.976476 breizorro-0.1.1/breizorro/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-01-09 12:53:41.000000 breizorro-0.1.1/breizorro/bin/breizorro
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-01-09 12:53:41.000000 breizorro-0.1.1/breizorro/breizorro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 12:53:41.976476 breizorro-0.1.1/breizorro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-01-09 12:53:41.000000 breizorro-0.1.1/breizorro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-09 12:53:41.000000 breizorro-0.1.1/breizorro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 12:53:41.000000 breizorro-0.1.1/breizorro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-09 12:53:41.000000 breizorro-0.1.1/breizorro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-09 12:53:41.000000 breizorro-0.1.1/breizorro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-09 12:53:41.000000 breizorro-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 12:53:41.980476 breizorro-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-01-09 12:53:41.000000 breizorro-0.1.1/setup.py
+-rw-r--r--   0        0        0    35147 2023-06-26 10:59:12.831221 breizorro-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5000 2023-06-26 10:59:12.831221 breizorro-0.1.2/README.rst
+-rw-r--r--   0        0        0    16060 2023-06-26 10:59:12.831221 breizorro-0.1.2/breizorro/breizorro.py
+-rw-r--r--   0        0        0       63 2023-06-26 10:59:12.831221 breizorro-0.1.2/breizorro/main.py
+-rw-r--r--   0        0        0     1520 2023-06-26 10:59:12.831221 breizorro-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6301 1970-01-01 00:00:00.000000 breizorro-0.1.2/PKG-INFO
```

### Comparing `breizorro-0.1.1/LICENSE` & `breizorro-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `breizorro-0.1.1/PKG-INFO` & `breizorro-0.1.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: breizorro
-Version: 0.1.1
-Summary: Creates a binary mask given a FITS image
-Home-page: https://github.com/ratt-ru/breizorro
-Author: Ian Heywood & RATT
-Author-email: ian.heywood@physics.ox.ac.uk
-License: GNU GPL 3
-Keywords: fits dataset models mask
-Platform: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 =========
 breizorro
 =========
 |Pypi Version|
 |Python Versions|
 |Project License|
 
@@ -49,59 +30,67 @@
    
    $ breizorro --help
 
      breizorro.breizorro - 2022-08-24 11:07:39,311 INFO - Welcome to breizorro
      breizorro.breizorro - 2022-08-24 11:07:39,375 INFO - Version: 0.1.1
      breizorro.breizorro - 2022-08-24 11:07:39,375 INFO - Usage: breizorro --help
      usage: breizorro [-h] [-r IMAGE] [-m MASK] [-t THRESHOLD] [-b BOXSIZE]
-                 [--savenoise] [--merge MASKs|REGs) [MASK(s|REGs) ...]]
-                 [--subtract MASK(s|REGs) [MASK(s|REGs ...]]
-                 [--number-islands] [--remove-islands N|COORD [N|COORD ...]]
-                 [--extract-islands N|COORD [N|COORD ...]] [--make-binary]
-                 [--invert] [--dilate R] [--fill-holes] [--sum-peak SUM_PEAK]
-                 [-o OUTFILE] [--gui]
+                      [--savenoise] [--merge MASKs|REGs) [MASK(s|REGs) ...]]
+                      [--subtract MASK(s|REGs) [MASK(s|REGs ...]]
+                      [--number-islands] [--remove-islands N|COORD [N|COORD ...]]
+                      [--ignore-missing-islands]
+                      [--extract-islands N|COORD [N|COORD ...]]
+                      [--minimum-size MINSIZE] [--make-binary] [--invert]
+                      [--dilate R] [--erode N] [--fill-holes] [--sum-peak SUM_PEAK]
+                      [-o OUTFILE] [--gui]
 
      breizorro [options] --restored-image restored_image
 
-      optional arguments:
-      -h, --help            show this help message and exit
-      -r IMAGE, --restored-image IMAGE
-                            Restored image file from which to build mask
-      -m MASK, --mask-image MASK
-                            Input mask file(s). Either --restored-image or --mask-
-                            image must be specfied.
-      -t THRESHOLD, --threshold THRESHOLD
-                            Sigma threshold for masking (default = 6.5)
-      -b BOXSIZE, --boxsize BOXSIZE
-                            Box size over which to compute stats (default = 50)
-      --savenoise           Enable to export noise image as FITS file (default=do
-                            not save noise image)
-      --merge MASK(s)|REG(s) [MASK(s)|REG(s) ...]
-                            Merge in one or more masks or region files
-      --subtract MASK(s)|REG(s) [MASK(s)|REG(s) ...]
-                            Subract one or more masks or region files
-      --number-islands      Number the islands detected (default=do not number
-                            islands)
-      --remove-islands N|COORD [N|COORD ...]
-                            List of islands to remove from input mask. e.g.
-                            --remove-islands 1 18 20 20h10m13s,14d15m20s
-      --extract-islands N|COORD [N|COORD ...]
-                            List of islands to extract from input mask. e.g.
-                            --extract-islands 1 18 20 20h10m13s,14d15m20s
-      --make-binary         Replace all island numbers with 1
-      --invert              Invert the mask
-      --dilate R            Apply dilation with a radius of R pixels
-      --fill-holes          Fill holes (i.e. entirely closed regions) in mask
-      --sum-peak SUM_PEAK   Sum to peak ratio of flux islands to mask in original
-                            image.e.g. --sum-peak 100 will mask everything with a
-                            ratio above 100
-      -o OUTFILE, --outfile OUTFILE
-                            Suffix for mask image (default based on input name
-      --gui                 Open mask in gui.
-
+     optional arguments:
+          -h, --help            show this help message and exit
+          -r IMAGE, --restored-image IMAGE
+                                Restored image file from which to build mask
+          -m MASK, --mask-image MASK
+                                Input mask file(s). Either --restored-image or --mask-
+                                image must be specfied.
+          -t THRESHOLD, --threshold THRESHOLD
+                                Sigma threshold for masking (default = 6.5)
+          -b BOXSIZE, --boxsize BOXSIZE
+                                Box size over which to compute stats (default = 50)
+          --savenoise           Enable to export noise image as FITS file (default=do
+                                not save noise image)
+          --merge MASK(s)|REG(s) [MASK(s)|REG(s) ...]
+                                Merge in one or more masks or region files
+          --subtract MASK(s)|REG(s) [MASK(s)|REG(s) ...]
+                                Subract one or more masks or region files
+          --number-islands      Number the islands detected (default=do not number
+                                islands)
+          --remove-islands N|COORD [N|COORD ...]
+                                List of islands to remove from input mask. e.g.
+                                --remove-islands 1 18 20 20h10m13s,14d15m20s
+          --ignore-missing-islands
+                                If an island specified by coordinates does not exist,
+                                do not throw an error
+          --extract-islands N|COORD [N|COORD ...]
+                                List of islands to extract from input mask. e.g.
+                                --extract-islands 1 18 20 20h10m13s,14d15m20s
+          --minimum-size MINSIZE
+                                Remove islands that have areas fewer than or equal to
+                                the specified number of pixels
+          --make-binary         Replace all island numbers with 1
+          --invert              Invert the mask
+          --dilate R            Apply dilation with a radius of R pixels
+          --erode N             Apply N iterations of erosion
+          --fill-holes          Fill holes (i.e. entirely closed regions) in mask
+          --sum-peak SUM_PEAK   Sum to peak ratio of flux islands to mask in original
+                                image.e.g. --sum-peak 100 will mask everything with a
+                                ratio above 100
+          -o OUTFILE, --outfile OUTFILE
+                                Suffix for mask image (default based on input name
+          --gui                 Open mask in gui.
 
 =======
 License
 =======
 
 This project is licensed under the GNU General Public License v3.0 - see license_ for details.
```

### Comparing `breizorro-0.1.1/breizorro/breizorro.py` & `breizorro-0.1.2/breizorro/breizorro.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 import numpy as np
 from astropy.io import fits
 from astropy.coordinates import SkyCoord
 from astropy.wcs import WCS
 import regions
 from argparse import ArgumentParser
 
-from scipy.ndimage.morphology import binary_dilation, binary_fill_holes
+from scipy.ndimage.morphology import binary_dilation, binary_erosion, binary_fill_holes
 from scipy.ndimage.measurements import label, find_objects
 import scipy.special
 import scipy.ndimage
 
-from bokeh.models import BoxEditTool, ColumnDataSource, FreehandDrawTool
-from bokeh.plotting import figure, output_file, show
-from bokeh.themes import built_in_themes
-from bokeh.io import curdoc
 
 def create_logger():
     """Create a console logger"""
     log = logging.getLogger(__name__)
     cfmt = logging.Formatter(('%(name)s - %(asctime)s %(levelname)s - %(message)s'))
     log.setLevel(logging.DEBUG)
     console = logging.StreamHandler(sys.stdout)
@@ -159,14 +155,16 @@
     parser.add_argument('--make-binary', action="store_true",
                          help='Replace all island numbers with 1')
     parser.add_argument('--invert', action="store_true",
                          help='Invert the mask')
     
     parser.add_argument('--dilate', dest='dilate', metavar="R", type=int, default=0,
                         help='Apply dilation with a radius of R pixels')
+    parser.add_argument('--erode', dest='erode', metavar="N", type=int, default=0,
+                        help='Apply N iterations of erosion')
     parser.add_argument('--fill-holes', dest='fill_holes', action='store_true', 
                         help='Fill holes (i.e. entirely closed regions) in mask')
 
     parser.add_argument('--sum-peak', dest='sum_peak', default=None,
                         help='Sum to peak ratio of flux islands to mask in original image.'
                              'e.g. --sum-peak 100 will mask everything with a ratio above 100')
 
@@ -180,34 +178,34 @@
     boxsize = int(args.boxsize)
     dilate = int(args.dilate)
     savenoise = args.savenoise
     outfile = args.outfile
 
     if args.imagename and args.maskname:
         parser.error("Either --restored-image or --mask-image must be specified, but not both")
+    elif not args.imagename and not args.maskname:
+        parser.error("Either --restored-image or --mask-image must be specified")
 
     # define input file, and get its name and extension
     input_file = args.imagename or args.maskname
-#    name, ext = os.path.split(input_file)
     name = '.'.join(input_file.split('.')[:-1])
     ext = input_file.split('.')[-1]
 
     # first, load or generate mask
-
     if args.imagename:
         input_image, input_header = get_image(input_file)
         LOGGER.info(f"Generating mask using threshold {threshold}")
 
         noise_image = make_noise_map(input_image, boxsize)
         if savenoise:
             noise_fits = f"{name}.noise.fits"
             shutil.copyfile(input_file, noise_fits)
             flush_fits(noise_image, noise_fits)
 
-        mask_image = input_image > threshold * noise_image
+        mask_image = (input_image > threshold * noise_image).astype('float64')
 
         mask_image[:, -1]=0
         mask_image[:, 0]=0
         mask_image[0, :]=0
         mask_image[-1, :]=0
 
         mask_header = input_header
@@ -309,14 +307,19 @@
 
     if args.dilate:
         LOGGER.info(f"Dilating mask using a ball of R={args.dilate}pix")
         R = args.dilate
         r = np.arange(-R, R+1)
         struct = np.sqrt(r[:, np.newaxis]**2 + r[np.newaxis,:]**2) <= R
         mask_image = binary_dilation(input=mask_image, structure=struct)
+
+    if args.erode:
+        LOGGER.info(f"Applying {args.erode} iteration(s) of erosion")
+        N = args.erode
+        mask_image = binary_erosion(input=mask_image, iterations=N)
         
     if args.fill_holes:
         LOGGER.info(f"Filling closed regions")
         mask_image = binary_fill_holes(mask_image)
 
     if args.sum_peak:
         # This mainly to produce an image that mask out super extended sources (via sum-to-peak flux ratio)
@@ -337,15 +340,21 @@
             isl_slice = mask_image[ext_isl] == 0
             new_mask_image[ext_isl] = isl_slice
         mask_header['BUNIT'] = 'Jy/beam'
         mask_image = input_image * new_mask_image
         LOGGER.info(f"Number of extended islands found: {len(extended_islands)}")
 
     if args.gui:
-        curdoc().theme = 'caliber'
+        try:
+            from bokeh.models import BoxEditTool, ColumnDataSource, FreehandDrawTool
+            from bokeh.plotting import figure, output_file, show
+            from bokeh.io import curdoc
+            curdoc().theme = 'caliber'
+        except ModuleNotFoundError:
+            LOGGER.error("Running breizorro gui requires optional dependencies, please re-install with: pip install breizorro[gui]")
 
         LOGGER.info("Loading Gui ...")
         d = mask_image
         p = figure(tooltips=[("x", "$x"), ("y", "$y"), ("value", "@image")])
         p.x_range.range_padding = p.y_range.range_padding = 0
         p.title.text = out_mask_fits
```

### Comparing `breizorro-0.1.1/breizorro.egg-info/PKG-INFO` & `breizorro-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 Metadata-Version: 2.1
 Name: breizorro
-Version: 0.1.1
+Version: 0.1.2
 Summary: Creates a binary mask given a FITS image
 Home-page: https://github.com/ratt-ru/breizorro
+License: GNU GPL v3
+Keywords: Astronomy,Masking,Imaging
 Author: Ian Heywood & RATT
-Author-email: ian.heywood@physics.ox.ac.uk
-License: GNU GPL 3
-Keywords: fits dataset models mask
-Platform: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
+Author-email: ian.heywood@phyics.ox.ac.uk
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Provides-Extra: gui
+Provides-Extra: testing
+Requires-Dist: astropy
+Requires-Dist: bokeh ; extra == "gui"
+Requires-Dist: numpy
+Requires-Dist: pytest ; extra == "testing"
+Requires-Dist: pytest-flake8 ; extra == "testing"
+Requires-Dist: regions
+Requires-Dist: scipy
+Project-URL: Repository, https://github.com/ratt-ru/breizorro.git
 Description-Content-Type: text/x-rst
-License-File: LICENSE
 
 =========
 breizorro
 =========
 |Pypi Version|
 |Python Versions|
 |Project License|
@@ -49,59 +64,67 @@
    
    $ breizorro --help
 
      breizorro.breizorro - 2022-08-24 11:07:39,311 INFO - Welcome to breizorro
      breizorro.breizorro - 2022-08-24 11:07:39,375 INFO - Version: 0.1.1
      breizorro.breizorro - 2022-08-24 11:07:39,375 INFO - Usage: breizorro --help
      usage: breizorro [-h] [-r IMAGE] [-m MASK] [-t THRESHOLD] [-b BOXSIZE]
-                 [--savenoise] [--merge MASKs|REGs) [MASK(s|REGs) ...]]
-                 [--subtract MASK(s|REGs) [MASK(s|REGs ...]]
-                 [--number-islands] [--remove-islands N|COORD [N|COORD ...]]
-                 [--extract-islands N|COORD [N|COORD ...]] [--make-binary]
-                 [--invert] [--dilate R] [--fill-holes] [--sum-peak SUM_PEAK]
-                 [-o OUTFILE] [--gui]
+                      [--savenoise] [--merge MASKs|REGs) [MASK(s|REGs) ...]]
+                      [--subtract MASK(s|REGs) [MASK(s|REGs ...]]
+                      [--number-islands] [--remove-islands N|COORD [N|COORD ...]]
+                      [--ignore-missing-islands]
+                      [--extract-islands N|COORD [N|COORD ...]]
+                      [--minimum-size MINSIZE] [--make-binary] [--invert]
+                      [--dilate R] [--erode N] [--fill-holes] [--sum-peak SUM_PEAK]
+                      [-o OUTFILE] [--gui]
 
      breizorro [options] --restored-image restored_image
 
-      optional arguments:
-      -h, --help            show this help message and exit
-      -r IMAGE, --restored-image IMAGE
-                            Restored image file from which to build mask
-      -m MASK, --mask-image MASK
-                            Input mask file(s). Either --restored-image or --mask-
-                            image must be specfied.
-      -t THRESHOLD, --threshold THRESHOLD
-                            Sigma threshold for masking (default = 6.5)
-      -b BOXSIZE, --boxsize BOXSIZE
-                            Box size over which to compute stats (default = 50)
-      --savenoise           Enable to export noise image as FITS file (default=do
-                            not save noise image)
-      --merge MASK(s)|REG(s) [MASK(s)|REG(s) ...]
-                            Merge in one or more masks or region files
-      --subtract MASK(s)|REG(s) [MASK(s)|REG(s) ...]
-                            Subract one or more masks or region files
-      --number-islands      Number the islands detected (default=do not number
-                            islands)
-      --remove-islands N|COORD [N|COORD ...]
-                            List of islands to remove from input mask. e.g.
-                            --remove-islands 1 18 20 20h10m13s,14d15m20s
-      --extract-islands N|COORD [N|COORD ...]
-                            List of islands to extract from input mask. e.g.
-                            --extract-islands 1 18 20 20h10m13s,14d15m20s
-      --make-binary         Replace all island numbers with 1
-      --invert              Invert the mask
-      --dilate R            Apply dilation with a radius of R pixels
-      --fill-holes          Fill holes (i.e. entirely closed regions) in mask
-      --sum-peak SUM_PEAK   Sum to peak ratio of flux islands to mask in original
-                            image.e.g. --sum-peak 100 will mask everything with a
-                            ratio above 100
-      -o OUTFILE, --outfile OUTFILE
-                            Suffix for mask image (default based on input name
-      --gui                 Open mask in gui.
-
+     optional arguments:
+          -h, --help            show this help message and exit
+          -r IMAGE, --restored-image IMAGE
+                                Restored image file from which to build mask
+          -m MASK, --mask-image MASK
+                                Input mask file(s). Either --restored-image or --mask-
+                                image must be specfied.
+          -t THRESHOLD, --threshold THRESHOLD
+                                Sigma threshold for masking (default = 6.5)
+          -b BOXSIZE, --boxsize BOXSIZE
+                                Box size over which to compute stats (default = 50)
+          --savenoise           Enable to export noise image as FITS file (default=do
+                                not save noise image)
+          --merge MASK(s)|REG(s) [MASK(s)|REG(s) ...]
+                                Merge in one or more masks or region files
+          --subtract MASK(s)|REG(s) [MASK(s)|REG(s) ...]
+                                Subract one or more masks or region files
+          --number-islands      Number the islands detected (default=do not number
+                                islands)
+          --remove-islands N|COORD [N|COORD ...]
+                                List of islands to remove from input mask. e.g.
+                                --remove-islands 1 18 20 20h10m13s,14d15m20s
+          --ignore-missing-islands
+                                If an island specified by coordinates does not exist,
+                                do not throw an error
+          --extract-islands N|COORD [N|COORD ...]
+                                List of islands to extract from input mask. e.g.
+                                --extract-islands 1 18 20 20h10m13s,14d15m20s
+          --minimum-size MINSIZE
+                                Remove islands that have areas fewer than or equal to
+                                the specified number of pixels
+          --make-binary         Replace all island numbers with 1
+          --invert              Invert the mask
+          --dilate R            Apply dilation with a radius of R pixels
+          --erode N             Apply N iterations of erosion
+          --fill-holes          Fill holes (i.e. entirely closed regions) in mask
+          --sum-peak SUM_PEAK   Sum to peak ratio of flux islands to mask in original
+                                image.e.g. --sum-peak 100 will mask everything with a
+                                ratio above 100
+          -o OUTFILE, --outfile OUTFILE
+                                Suffix for mask image (default based on input name
+          --gui                 Open mask in gui.
 
 =======
 License
 =======
 
 This project is licensed under the GNU General Public License v3.0 - see license_ for details.
 
@@ -123,7 +146,8 @@
 .. |Pypi Version| image:: https://img.shields.io/pypi/v/breizorro.svg
                   :target: https://pypi.python.org/pypi/breizorro
                   :alt:
 
 .. _source: https://github.com/ratt-ru/breizorro
 .. _license: https://github.com/ratt-ru/breizorro/blob/main/LICENSE
 .. _pep8: https://www.python.org/dev/peps/pep-0008
+
```

