# Comparing `tmp/gistdawater-0.0.3.tar.gz` & `tmp/gistdawater-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gistdawater-0.0.3.tar", last modified: Mon Jun 26 04:27:57 2023, max compression
+gzip compressed data, was "gistdawater-0.0.4.tar", last modified: Mon Jun 26 04:33:04 2023, max compression
```

## Comparing `gistdawater-0.0.3.tar` & `gistdawater-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 04:27:57.521493 gistdawater-0.0.3/
--rw-rw-rw-   0        0        0     1068 2022-07-25 06:10:12.000000 gistdawater-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1089 2022-07-25 06:10:12.000000 gistdawater-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       38 2023-04-27 03:39:29.000000 gistdawater-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2081 2023-06-26 04:27:57.521493 gistdawater-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1540 2023-06-22 07:56:15.000000 gistdawater-0.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-26 04:27:57.064618 gistdawater-0.0.3/gistdawater/
--rw-rw-rw-   0        0        0      180 2023-06-26 04:26:11.000000 gistdawater-0.0.3/gistdawater/__init__.py
--rw-rw-rw-   0        0        0    20826 2023-06-26 04:25:02.000000 gistdawater-0.0.3/gistdawater/mainfile.py
-drwxrwxrwx   0        0        0        0 2023-06-26 04:27:57.519490 gistdawater-0.0.3/gistdawater.egg-info/
--rw-rw-rw-   0        0        0     2081 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-26 04:27:56.000000 gistdawater-0.0.3/gistdawater.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-26 04:27:57.523488 gistdawater-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1319 2023-06-26 04:26:16.000000 gistdawater-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 04:33:04.555816 gistdawater-0.0.4/
+-rw-rw-rw-   0        0        0     1068 2022-07-25 06:10:12.000000 gistdawater-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1089 2022-07-25 06:10:12.000000 gistdawater-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       38 2023-04-27 03:39:29.000000 gistdawater-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2081 2023-06-26 04:33:04.556814 gistdawater-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1540 2023-06-22 07:56:15.000000 gistdawater-0.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-26 04:33:04.522812 gistdawater-0.0.4/gistdawater/
+-rw-rw-rw-   0        0        0      180 2023-06-26 04:32:00.000000 gistdawater-0.0.4/gistdawater/__init__.py
+-rw-rw-rw-   0        0        0    26909 2023-06-26 04:31:40.000000 gistdawater-0.0.4/gistdawater/mainfile.py
+drwxrwxrwx   0        0        0        0 2023-06-26 04:33:04.554815 gistdawater-0.0.4/gistdawater.egg-info/
+-rw-rw-rw-   0        0        0     2081 2023-06-26 04:33:04.000000 gistdawater-0.0.4/gistdawater.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-26 04:33:04.000000 gistdawater-0.0.4/gistdawater.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 04:33:04.000000 gistdawater-0.0.4/gistdawater.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-26 04:33:04.000000 gistdawater-0.0.4/gistdawater.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-26 04:33:04.000000 gistdawater-0.0.4/gistdawater.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-26 04:33:04.558815 gistdawater-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1319 2023-06-26 04:31:56.000000 gistdawater-0.0.4/setup.py
```

### Comparing `gistdawater-0.0.3/LICENSE` & `gistdawater-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gistdawater-0.0.3/LICENSE.txt` & `gistdawater-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gistdawater-0.0.3/PKG-INFO` & `gistdawater-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gistdawater
-Version: 0.0.3
+Version: 0.0.4
 Summary: Waterdetection for landsat8
 Author: Gistda
 Author-email: gistdathailand@gmail.com
 License: MIT
 Keywords: geo,oepn data cube,earth
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
```

### Comparing `gistdawater-0.0.3/README.rst` & `gistdawater-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `gistdawater-0.0.3/gistdawater/mainfile.py` & `gistdawater-0.0.4/gistdawater/mainfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -444,8 +444,123 @@
                     matrice_cluster[indices_array[0][clusters_labels == label_i],
                                     indices_array[1][clusters_labels == label_i]] = new_label
 
                     new_label += 1
                 else:
                     pass
                     # print('Skipping cluster_id {}'.format(label_i))
-            return matrice_cluster
+
+            return matrice_cluster
+
+
+        ################################################ waterdetection #################################################
+        def waterdetect(self):
+            """
+            waterdetection
+            :return : watermask
+            """
+            ## wd.DWImageClustering
+            # get the first band as reference of size
+            ref_band = list(self.bands.keys())[0]
+            ref_shape = self.bands[ref_band].shape
+
+            #check the invalid_mask
+            invalid_mask = np.zeros(ref_shape,dtype=bool)
+            
+            #check if the MNDWI index is necessary and if it exists
+            if 'mndwi' in self.required_indices and 'mndwi' not in self.bands:
+                mndwi,mndwi_mask = self.calc_normalized_difference(self.bands['Green'],self.bands['Mir2'],invalid_mask)
+                invalid_mask |= mndwi_mask
+                self.bands.update({'mndwi':mndwi})
+
+            #check if the NDWI index exist
+            if 'ndwi' in self.required_bands and 'ndwi' not in self.bands.keys():
+                ndwi,ndwi_mask = self.calc_normalized_difference(self.bands['Green'],self.bands['Nir'],invalid_mask)
+                invalid_mask |= ndwi_mask
+                self.bands.update({'ndwi':ndwi})
+
+            #check if the MBWI index exist
+            if 'mbwi' in self.required_bands and 'mbwi' not in self.bands.keys():
+                mbwi,mbwi_mask = self.calc_mbwi(self.bands,3,invalid_mask)
+                invalid_mask |= mbwi_mask
+
+            #check if the list contains the required bands
+            for band in self.listify(self.bands_keys):
+                if band == 'otsu' or band == 'canny':
+                    continue
+                if band not in self.bands.keys():
+                    raise OSError('Band {}, not available in the dictionary'.format(self.band))
+                if type(self.bands[band]) is not np.ndarray:
+                    raise OSError('Band {} is not a numpy array'.format(self.band))
+                if ref_shape != self.bands[band].shape:
+                    raise OSError('Bands {} and {} with different size in clustering core'.format(self.band, ref_band))
+                else:
+                    pass
+                    # print("band : ",band+"In require bands list")
+
+            ## run_detect_water
+            # print('My.DataComponent : self.bands_keys[0] :',self.bands_keys[0])
+            #if passed options,override the existing options
+            if self.bands_keys[0] == 'otsu':
+                cluster_matrix = self.apply_otsu_treshold()
+            elif self.bands_keys[0] == 'canny':
+                cluster_matrix = self.apply_canny_treshold()
+            elif False:
+                cluster_matrix = None
+
+            #Transform the rasters in a matrix where each band is a column
+            data_as_columns = self.bands_to_columns(self.bands,invalid_mask)
+
+            # two line vectors indicating the indexes (line column) of valid pixels
+            ind_data = np.where(~invalid_mask)   
+
+            # if algorithm is not kmeans,split data for a smaller ser (for performnce purposes)
+            if self.clustering_method == 'kmean':
+                train_data_as_columns=data_as_columns
+            else:
+                train_data_as_columns,ts= self.get_train_test_split(data_as_columns,self.train_size,self.min_train_size,self.max_train_size)
+
+            #split1
+            split_train_data_as_columns = self.split_data_by_bands(self.bands,train_data_as_columns,self.bands_keys)
+            #split2
+            split_data_as_columns = self.split_data_by_bands(self.bands,data_as_columns,self.bands_keys)
+
+            #find best_k
+            best_k = self.find_best_k(split_train_data_as_columns)
+
+            #apply the clusterization algorithm and return labels and train dataset
+            train_clusters_labels = self.apply_cluster(split_train_data_as_columns,best_k)
+
+            #cals statistics for each cluster
+            self.clusters_params = self.calc_clusters_params(train_data_as_columns,train_clusters_labels,best_k)
+
+            #detect the water cluster
+            water_cluster = self.identify_water_cluster(self.detect_water_cluster,self.bands)
+
+            if self.clustering_method != 'kmeans':
+                clusters_labels = self.supervised_classification(split_data_as_columns,split_train_data_as_columns,train_clusters_labels)
+            else:
+                clusters_labels = train_clusters_labels
+            # print('My.DataComponent : clusters_labels :',clusters_labels)
+            # after obtain the final labels,clip bands with superios limit
+            for band,value in zip(self.clip_band,self.clip_sup_value):
+                if value is not None:
+                    if self.glint_mode and self.glint_processor is not None:
+                        print('0')
+                    else:
+                        comp_array = value
+                    clusters_labels[(clusters_labels == water_cluster['clusterid']) & (self.bands[band][~invalid_mask]>comp_array)] = -1
+            #after obtainting the final labels,clip bands with inferior limit
+            for band,value in zip(self.clip_band,self.clip_inf_value):
+                if value is not None:
+                    if self.glint_mode and self.glint_processor is not None:
+                        print('0')
+                    else:
+                        comp_array = value
+                    clusters_labels[(clusters_labels == water_cluster['clusterid']) & (self.bands[band][~invalid_mask]<comp_array)] = -1
+            
+            #create an cluster array based on the cluster result (water will be value1)
+            cluster_matrix = self.create_matrice_cluster(ind_data,self.bands,clusters_labels,water_cluster,best_k)
+            water_mask = np.where(cluster_matrix == 1,1,np.where(invalid_mask == 1,255,0)).astype('int8')
+            watermask0 = water_mask==0
+            watermask1 = water_mask==1
+            return watermask1
```

### Comparing `gistdawater-0.0.3/gistdawater.egg-info/PKG-INFO` & `gistdawater-0.0.4/gistdawater.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gistdawater
-Version: 0.0.3
+Version: 0.0.4
 Summary: Waterdetection for landsat8
 Author: Gistda
 Author-email: gistdathailand@gmail.com
 License: MIT
 Keywords: geo,oepn data cube,earth
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
```

### Comparing `gistdawater-0.0.3/setup.py` & `gistdawater-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'gistdawater',                # Name project the same with folder
   packages = ['gistdawater'],          # Name project the same with folder
-  version = '0.0.3',                   # version
+  version = '0.0.4',                   # version
   license='MIT', 
   description = 'Waterdetection for landsat8',    #Show on PyPi
   long_description=DESCRIPTION,
   author = 'Gistda',            #          
   author_email = 'gistdathailand@gmail.com',     #  
   keywords = ['geo','oepn data cube','earth'],      # When someone search
   # Dont add any library bz It's gonna error waiting
```

