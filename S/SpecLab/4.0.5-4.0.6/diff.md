# Comparing `tmp/SpecLab-4.0.5.tar.gz` & `tmp/SpecLab-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SpecLab-4.0.5.tar", last modified: Fri Jun 16 16:14:07 2023, max compression
+gzip compressed data, was "dist/SpecLab-4.0.6.tar", last modified: Mon Jun 26 18:09:07 2023, max compression
```

## Comparing `SpecLab-4.0.5.tar` & `SpecLab-4.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-16 16:14:07.000000 SpecLab-4.0.5/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-16 16:14:07.000000 SpecLab-4.0.5/SpecLab/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-16 16:14:07.000000 SpecLab-4.0.5/SpecLab/imXam/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.0.5/SpecLab/imXam/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48580 2023-06-16 16:13:05.000000 SpecLab-4.0.5/SpecLab/imXam/imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-16 16:14:07.000000 SpecLab-4.0.5/SpecLab/cfg/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.0.5/SpecLab/cfg/SpecLab_config.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.0.5/SpecLab/cfg/epar_imXam.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-16 16:14:07.000000 SpecLab-4.0.5/SpecLab/gen/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53071 2023-06-14 20:52:49.000000 SpecLab-4.0.5/SpecLab/gen/SpecLabFunctions.py
--rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.0.5/SpecLab/gen/globals.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.0.5/SpecLab/gen/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.0.5/SpecLab/gen/myfunc.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.0.5/SpecLab/__init__.py
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-16 16:14:07.000000 SpecLab-4.0.5/SpecLab/aux/
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-16 16:14:07.000000 SpecLab-4.0.5/SpecLab/aux/param_files/
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2110 2023-06-15 01:05:24.000000 SpecLab-4.0.5/SpecLab/aux/param_files/imXam_param.default.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.0.5/SpecLab/aux/param_files/__init__.py
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2107 2023-06-14 15:08:54.000000 SpecLab-4.0.5/SpecLab/aux/param_files/imXam_param_ARCES.dat
--rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2110 2023-06-15 01:05:47.000000 SpecLab-4.0.5/SpecLab/aux/param_files/imXam_param.dat
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.0.5/SpecLab/aux/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   625389 2023-05-30 23:11:52.000000 SpecLab-4.0.5/SpecLab/aux/pyqtgraph10_speclab.tar.gz
-drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-16 16:14:07.000000 SpecLab-4.0.5/SpecLab/doc/
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.0.5/SpecLab/doc/__init__.py
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      223 2023-06-16 16:13:33.000000 SpecLab-4.0.5/SpecLab/doc/CHANGELOG.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     3570 2023-06-16 16:13:20.000000 SpecLab-4.0.5/SpecLab/doc/README.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      757 2023-06-14 16:21:19.000000 SpecLab-4.0.5/SpecLab/doc/KNOWN_ISSUES.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.0.5/SpecLab/doc/LICENSE.txt
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      213 2023-06-16 16:14:07.000000 SpecLab-4.0.5/PKG-INFO
--rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1161 2023-06-16 16:12:27.000000 SpecLab-4.0.5/setup.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/imXam/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-05-30 23:51:42.000000 SpecLab-4.0.6/SpecLab/imXam/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)    48679 2023-06-26 18:03:14.000000 SpecLab-4.0.6/SpecLab/imXam/imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/cfg/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     2025 2023-06-14 20:25:01.000000 SpecLab-4.0.6/SpecLab/cfg/SpecLab_config.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      379 2023-06-15 15:54:47.000000 SpecLab-4.0.6/SpecLab/cfg/epar_imXam.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/gen/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    53071 2023-06-14 20:52:49.000000 SpecLab-4.0.6/SpecLab/gen/SpecLabFunctions.py
+-rwxr--r--   0 adamkowalski  (1000) adamkowalski  (1000)      656 2023-06-02 18:44:11.000000 SpecLab-4.0.6/SpecLab/gen/globals.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:30.000000 SpecLab-4.0.6/SpecLab/gen/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)    20199 2023-06-14 19:40:28.000000 SpecLab-4.0.6/SpecLab/gen/myfunc.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-01 23:14:48.000000 SpecLab-4.0.6/SpecLab/__init__.py
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/aux/
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/aux/param_files/
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2133 2023-06-26 18:07:15.000000 SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param.default.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:07.000000 SpecLab-4.0.6/SpecLab/aux/param_files/__init__.py
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2130 2023-06-26 18:06:59.000000 SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param_ARCES.dat
+-rw-r--r--   0 adamkowalski  (1000) adamkowalski  (1000)     2134 2023-06-26 18:06:44.000000 SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param.dat
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:21:46.000000 SpecLab-4.0.6/SpecLab/aux/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)   625389 2023-05-30 23:11:52.000000 SpecLab-4.0.6/SpecLab/aux/pyqtgraph10_speclab.tar.gz
+drwxrwxr-x   0 adamkowalski  (1000) adamkowalski  (1000)        0 2023-06-26 18:09:07.000000 SpecLab-4.0.6/SpecLab/doc/
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)        3 2023-06-02 00:22:19.000000 SpecLab-4.0.6/SpecLab/doc/__init__.py
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      420 2023-06-26 17:45:13.000000 SpecLab-4.0.6/SpecLab/doc/CHANGELOG.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     4403 2023-06-26 18:04:52.000000 SpecLab-4.0.6/SpecLab/doc/README.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1072 2023-06-26 17:41:16.000000 SpecLab-4.0.6/SpecLab/doc/KNOWN_ISSUES.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1119 2023-06-14 15:39:40.000000 SpecLab-4.0.6/SpecLab/doc/LICENSE.txt
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)      213 2023-06-26 18:09:07.000000 SpecLab-4.0.6/PKG-INFO
+-rw-rw-r--   0 adamkowalski  (1000) adamkowalski  (1000)     1161 2023-06-26 18:08:59.000000 SpecLab-4.0.6/setup.py
```

### Comparing `SpecLab-4.0.5/SpecLab/imXam/imXam.py` & `SpecLab-4.0.6/SpecLab/imXam/imXam.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,22 +83,23 @@
     z2_zscale = imclean[midpoint] + (coeffsz[0] / 1.0) * (npoints - midpoint)
     return z1_zscale, z2_zscale
 
 
 
 print('======================================================')
 print('======================================================')
-print('imXam: adam f kowalski, v4.0.5: June 15, 2023')
-print(' To shut down gui, type q into terminal, type h for commands, use middle mouse wheel to zoom in and out')
+print('imXam: adam f kowalski, v4.0.6: June 26, 2023')
+print(' To shut down gui, type q into terminal, type h for interactive commands, use middle mouse wheel to zoom in and out')
 print(' You may have to click on gui with left mouse button in order to use interactive commands')
+print(' To get a list of command-line options, type imXam.py -h from a terminal.')
 print('======================================================')
 print('imXam.py located in ',your_site_packages_location[0]+'/SpecLab/imXam/')
 print(' and .../anaconda3/envs/<your_env_name>/bin/')
 print('Default param files located in ',your_site_packages_location[0]+'/SpecLab/aux/param_files/')
-print('New (v4.0.5):  can edit imXam_param.dat with vim by invoking epar_imXam.py in Unix command line')
+print('--> To edit imXam_param.dat with vim, type epar_imXam.py from a terminal.')
 print('======================================================')
 print('======================================================')
 
 from argparse import ArgumentParser
 from argparse import RawTextHelpFormatter
 parser = ArgumentParser(formatter_class=RawTextHelpFormatter)
 
@@ -294,14 +295,15 @@
     data = datax -  biasx
 else:
     data = datax
 
 
 imv1.setImage(data)
 imv1.view.invertY(False)
+#imv1.setColorMap('viridis')
 
 print('   ')
 print('File [ny , nx] = ',ifile,'[',nyy,',',nxx,']','   Max = ',np.max(data),'   Median = ',np.median(data))
 print('   ')
 
 roi = pg.LineSegmentROI([[int(nxx*0.03), int(nyy*0.5)], [int(nxx*0.97),int(nyy*0.5)]], pen=rcol)#,handlePen=(220,5,12),hoverPen=(0,0,0),handleHoverPen=(0,0,0))  # x = 0, y = 0 is at the top, left
 roi_v = pg.LineSegmentROI([[int(nxx*0.5), int(nyy*0.15)], [int(nxx*0.5),int(nyy*0.85)]], pen=rcol)#,handlePen=(220,5,12),hoverPen=(0,0,0),handleHoverPen=(0,0,0))  # x = 0, y = 0 is at the top, left
@@ -414,14 +416,15 @@
 
     
 BuRd = ["#2166AC", "#4393C3", "#92C5DE", "#D1E5F0","#F7F7F7", "#FDDBC7","#F4A582", "#D6604D", "#B2182B"]  # bad = 255,238,153 = FFEE99
 cmap_name = 'BuRd'  # smooth rainbow.
 map_burd = LinearSegmentedColormap.from_list(cmap_name, BuRd, N=100)
 
 
+
 #/anaconda3/envs/hst/lib/python3.6/site-packages/pyqtgraph/GraphicsScene/GraphicsScene.py
 def ifkeypress(evnt):
     # need to setClickable on pop up spectrum.
     # need to y-flip t-key and check coordinates.
     val = evnt.text()
     global user_x, user_y, apspec_radius, boxx0,boxx1, boxy0,boxy1, box_std,box_mean,box_med,box_min,box_max
     global uxlim1, uxlim2
@@ -526,15 +529,15 @@
         box_med.append(chk)
         chk = np.min(data[boxx0[-1]:boxx1[-1]+1, boxy0[-1]:boxy1[-1]+1])
         box_min.append(chk)
         chk = np.max(data[boxx0[-1]:boxx1[-1]+1, boxy0[-1]:boxy1[-1]+1])
         box_max.append(chk)
         n_boxes = len(boxx0)
         for nnn in range(0, n_boxes):
-            print('-- Box # ',nnn, ' of ', n_boxes, ' stored --')
+            print('-- Box # ',nnn+1, ' of ', n_boxes, ' stored --')
             print('Coordinates start at (0,0) relative to PyQTGraph display')
             print('x0 = {:8d}'.format(boxx0[nnn]))
             print('x1 = {:8d}'.format(boxx1[nnn]))
             print('y0 = {:8d}'.format(boxy0[nnn]))
             print('y1 = {:8d}'.format(boxy1[nnn]))
             print('dx = {:8d}'.format(np.abs(boxx0[nnn]- boxx1[nnn] + 1)))
             print('dy = {:8d}'.format(np.abs(boxy0[nnn]- boxy1[nnn] + 1)))
@@ -610,26 +613,26 @@
         fig.update_yaxes(title='Counts per pixel')
         fig.show()
                 
         QCoreApplication.processEvents()
            
     if val == 'c':
         yarr_1d = np.arange(0,len(data[user_x,:]),1)
-        fig = go.Figure(data=[go.Bar(x=yarr_1d, y=data[user_x,:], marker_color=[plotly_hist_color], width=np.ones(len(yarr_1d)) )])
+        fig = go.Figure(data=[go.Scatter(x=yarr_1d, y=data[user_x, :], marker_color="#000000",line_shape="hvh")])
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='Counts per pixel',nticks=10)
         fig.update_xaxes(title='y pixel')
         fig.show()
         QCoreApplication.processEvents()
         
     if val == 'l':
         
         f, ax = plt.subplots()
         xarr_1d = np.arange(0,len(data[:,user_y]),1) # starts at 0
-        fig = go.Figure(data=[go.Bar(x=xarr_1d, y=data[:,user_y], marker_color=[plotly_hist_color], width=np.ones(len(xarr_1d)) )])
+        fig = go.Figure(data=[go.Scatter(x=xarr_1d, y=data[:,user_y], marker_color="#000000",line_shape="hvh")])
         fig.update_layout(font_family='Times New Roman',font_size=15)
         fig.update_yaxes(title='Counts per pixel',nticks=10)
         fig.update_xaxes(title='x pixel')
         fig.show()
         QCoreApplication.processEvents()
 
     if val == 'm':
@@ -890,15 +893,15 @@
         fig.show()
     
 
         QCoreApplication.processEvents()
 
     if val == 'T':  # Find and show pixels above a threshold.
         thressh =  input('Enter threshold value: ')
-        thresh = int(thressh)
+        thresh = float(thressh)
         t_data = np.transpose(data)
 
         sat_pixels = (t_data >= thresh)
         inds2d = np.argwhere(sat_pixels)
         if inds2d.shape[0] > 0:
             
             fig_heatmap = go.Figure(data=go.Heatmap(z = t_data, zmin=Vmin,zmax=Vmax,\
@@ -993,14 +996,15 @@
 
 
 #https://stackoverflow.com/questions/40423999/pyqtgraph-where-to-find-signal-for-key-preses
 
 
 ## Display the data
 imv1.setImage(data)
+#imv1.setColorMap('CET-L17')
 
 #mpl_connect('key_press_event', on_key_event)
 
 zscale0, zscale1 = find_zscale(data)
 
 
 if args.z1 == None:
```

### Comparing `SpecLab-4.0.5/SpecLab/cfg/SpecLab_config.py` & `SpecLab-4.0.6/SpecLab/cfg/SpecLab_config.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.5/SpecLab/gen/SpecLabFunctions.py` & `SpecLab-4.0.6/SpecLab/gen/SpecLabFunctions.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.5/SpecLab/gen/globals.py` & `SpecLab-4.0.6/SpecLab/gen/globals.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.5/SpecLab/gen/myfunc.py` & `SpecLab-4.0.6/SpecLab/gen/myfunc.py`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.5/SpecLab/aux/param_files/imXam_param.default.dat` & `SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param.default.dat`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # For now, only integer values are allowed here.  You can reorder them anyway you want. The = signs just signify default values that work ok.  should fine tune them to your data.
 ix	param		value	description
-0	Color		gray	"color scheme (gray) "
+0	Color		gray	"color scheme (gray); currently only option "
 1	Window		40	"This is the half-size of a box around which to search for the star in centroiding for doing aperture photometry (40), should be > Back_2"
 2	Statsec		40	"for the m-key, stats are taken over a box with side length of twice this (40)."
 3	RMax		15	"plotting range for the r-key (15)"
 4	Apphot_Radius	5	"radius for the aperature phtometry vai the a- and r-keys  (~1.5x FWHM, ~5-8)"
 5	N_Contours	8	"number of contours to plot with the o-key (8)"
 6	Apspec_Upper	8	"+ value to extract spectrum (e.g., about 3 for ARCES, about 8 for DIS)"
 7	Apspec_Lower	8	"- value to extract spectrum (e.g., about 3 for ARCES, about 8 for DIS)"
```

### Comparing `SpecLab-4.0.5/SpecLab/aux/param_files/imXam_param_ARCES.dat` & `SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param_ARCES.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # For now, only integer values are allowed here.  You can reorder them anyway you want. The = signs just signify default values that work ok.  should fine tune them to your data.
 ix	param		value	description
-0	Color		gray	"color scheme (gray) "
+0	Color		gray	"color scheme (gray); currently only option "
 1	Window		40	"This is the half-size of a box around which to search for the star in centroiding for doing aperture photometry (40), should be > Back_2"
 2	Statsec		40	"for the m-key, stats are taken over a box with side length of twice this (40)."
 3	RMax		15	"plotting range for the r-key (15)"
 4	Apphot_Radius	5	"radius for the aperature phtometry vai the a- and r-keys  (~1.5x FWHM, ~5-8)"
 5	N_Contours	8	"number of contours to plot with the o-key (8)"
 6	Apspec_Upper	3	"+ value to extract spectrum (e.g., about 3 for ARCES, about 8 for DIS)"
 7	Apspec_Lower	3	"- value to extract spectrum (e.g., about 3 for ARCES, about 8 for DIS)"
```

### Comparing `SpecLab-4.0.5/SpecLab/aux/param_files/imXam_param.dat` & `SpecLab-4.0.6/SpecLab/aux/param_files/imXam_param.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # For now, only integer values are allowed here.  You can reorder them anyway you want. The = signs just signify default values that work ok.  should fine tune them to your data.
 ix	param		value	description
-0	Color		gray	"color scheme (gray) "
+0	Color		gray	"color scheme (gray); currently, only option "
 1	Window		40	"This is the half-size of a box around which to search for the star in centroiding for doing aperture photometry (40), should be > Back_2"
 2	Statsec		40	"for the m-key, stats are taken over a box with side length of twice this (40)."
 3	RMax		15	"plotting range for the r-key (15)"
 4	Apphot_Radius	8	"radius for the aperature phtometry vai the a- and r-keys  (~1.5x FWHM, ~5-8)"
 5	N_Contours	8	"number of contours to plot with the o-key (8)"
 6	Apspec_Upper	8	"+ value to extract spectrum (e.g., about 3 for ARCES, about 8 for DIS)"
 7	Apspec_Lower	8	"- value to extract spectrum (e.g., about 3 for ARCES, about 8 for DIS)"
```

### Comparing `SpecLab-4.0.5/SpecLab/aux/pyqtgraph10_speclab.tar.gz` & `SpecLab-4.0.6/SpecLab/aux/pyqtgraph10_speclab.tar.gz`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.5/SpecLab/doc/README.txt` & `SpecLab-4.0.6/SpecLab/doc/README.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,76 @@
 SpecLab
 ===============================
-imXam:  v4.0.5  (June 15, 2023)
+imXam:  v4.0.6  (June 26, 2023)
 
 imXam is the first interactive program finished for the SpecLab python-only
 data reduction package.  More (identify, standard, sensfunc, apall) will be added
 with the same GUI design (pyqtgraph10 + Plotly) in the future as these get finished.
 
-PyQTGraph:  https://www.pyqtgraph.org/ (this will be installed automatically with the commands below)
+PyQTGraph:  https://www.pyqtgraph.org/ (a customized version of v10 will be installed automatically with the commands below)
 
 Adam F Kowalski (adam.f.kowalski@colorado.edu)
+
 ===============================
+1) Creata conda environment to install in if you already have astroconda or another conda environment set up skip and you have
+run pip install SpecLab in that environment, then skep to step 2) below.
+
+
+To set up a fresh conda environment:
+
+[From a terminal window]
+      conda create --name your_env_name python=3.7
+
+      conda activate your_env_name
+
+      pip install SpecLab
+
+
+2) After pip install, run the command (from anywhere), which will untar v10 of pyqtgraph to your site-packages:
 
-After pip install, run the command (from anywhere) to untar v10 of pyqtgraph to your site-packages:
+      SpecLab_config.py
 
-SpecLab_config.py
+(You may have to open a fresh tab in your terminal for your system to see the new routines in <your_env_name>/bin/.  You can also:
+
+     cd /location_of_your_anaconda/anaconda3/envs/<your_env_name>/bin/
+     python SpecLab_config.py
 
 You will then be able to run imXam.py from anywhere (it is located in .../anaconda3/envs/<your_env_name>/bin/).
 
 Basic usage (or create an alias for "imXam.py -f" in your .bash_profile):
 
-imXam.py -f file.fits
+     imXam.py -f file.fits
+
+To get a list of command-line options, type in a Unix terminal:
+
+     imXam.py -h
 
 To load in a KOSMOS spectrum with the dispersion axis vertical:
 
-imXam.py -f KOSMOS_spectrum.fits -dispax 2
+     imXam.py -f KOSMOS_spectrum.fits -dispax 2
 
 To load in some reasonable parameters for tracing, extracting, etc with an ARCES / echelle spectrum, use:
 
-imXam.py -f ARCES_spectrum.fits -ec 1
+     imXam.py -f ARCES_spectrum.fits -ec 1
 
 You can also create your own imXam_param.dat file and specify to load it in with -i /full_path_to_custom_param/your_custom_param.dat
 
 You can edit imXam_param.dat directly from Unix command line by invoking:
 
-epar_imXam.py
-(requires vim)
+     epar_imXam.py
+     (requires vim)
 
 Please see KNOWN_ISSUES.
 
 Enjoy!
 
 
 ==== Acknowledgments ====
 
-Thanks to Isaiah Tristan and Yuta Notsu for testing an early version.
+Thanks to Isaiah Tristan and Yuta Notsu for testing and feedback on an early version.
 Thanks to Bill Ketzeback for helpful feedback and testing the most recent versions.  
 
 === Interactive Commands ===
 
 Will need to left mouse click on pyqtgraph display image for these to register.  Please use the wheel on your mouse to zoom in and out of the
   PyQTGraph display window.
 
@@ -70,12 +93,18 @@
 c:  plot a column through entire image at cursor location
 p:  show parameters in imXam_param.dat but dont edit.
 e:  edit parameters in imXam_param.dat; use p to see which can be edited.
 1 & 2:  clicking 1 in lower-left and 2 in upper-right will print stats within that box.
 H:  prints header to file.header.txt and lastheader.txt; also prints EXPTIME and DATE-OBS to screen.
 
 
+
+=== To Upgrade ===
+
+pip install SpecLab --upgrade
+
+
 === To Uninstall ===
 
 pip uninstall SpecLab
 
 Will have to remove pyqtgraph10_speclab/ from site-packages by hand.
```

### Comparing `SpecLab-4.0.5/SpecLab/doc/LICENSE.txt` & `SpecLab-4.0.6/SpecLab/doc/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SpecLab-4.0.5/setup.py` & `SpecLab-4.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='SpecLab',
-    version='4.0.5',
+    version='4.0.6',
     author='A. F. Kowalski',
     author_email='adam.f.kowalski@colorado.edu',
     packages=['SpecLab','SpecLab.aux','SpecLab.aux.param_files','SpecLab.imXam','SpecLab.doc','SpecLab.gen',],
     package_data = {'':['*.tar.gz', '*.txt', '*.dat'],},
    # include_package_data=True,
    # package_dir={"": ""},
     scripts=['SpecLab/cfg/SpecLab_config.py','SpecLab/imXam/imXam.py','SpecLab/cfg/epar_imXam.py',],
```

