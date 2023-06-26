# Comparing `tmp/gmltools-0.0.81.tar.gz` & `tmp/gmltools-0.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmltools-0.0.81.tar", last modified: Wed Jun 14 08:54:29 2023, max compression
+gzip compressed data, was "gmltools-0.0.82.tar", last modified: Mon Jun 26 15:34:26 2023, max compression
```

## Comparing `gmltools-0.0.81.tar` & `gmltools-0.0.82.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.523493 gmltools-0.0.81/
--rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.81/LICENSE
--rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.81/Models.ipynb
--rw-rw-rw-   0        0        0     1021 2023-06-14 08:54:29.522419 gmltools-0.0.81/PKG-INFO
--rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.81/README.md
--rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.81/gmltools.yml
--rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.81/mltools.yml
--rw-rw-rw-   0        0        0      618 2023-06-14 08:54:20.000000 gmltools-0.0.81/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-14 08:54:29.523493 gmltools-0.0.81/setup.cfg
--rw-rw-rw-   0        0        0     1746 2023-06-14 08:54:18.000000 gmltools-0.0.81/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.486267 gmltools-0.0.81/src/
-drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.498153 gmltools-0.0.81/src/gmltools/
--rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.81/src/gmltools/To_Do.txt
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.81/src/gmltools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.503714 gmltools-0.0.81/src/gmltools/eda/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.81/src/gmltools/eda/__init__.py
--rw-rw-rw-   0        0        0    42538 2023-05-29 11:18:21.000000 gmltools-0.0.81/src/gmltools/eda/eda.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.515690 gmltools-0.0.81/src/gmltools/models/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.81/src/gmltools/models/__init__.py
--rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.81/src/gmltools/models/bayes.py
--rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.81/src/gmltools/models/custom_scorings.py
--rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.81/src/gmltools/models/dummy_model.py
--rw-rw-rw-   0        0        0   160613 2023-06-14 08:54:19.000000 gmltools-0.0.81/src/gmltools/models/model.py
--rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.81/src/gmltools/models/models_info.py
--rw-rw-rw-   0        0        0    13212 2023-05-12 09:20:42.000000 gmltools-0.0.81/src/gmltools/models/timeseriesplit.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.518680 gmltools-0.0.81/src/gmltools/models_analysis/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.81/src/gmltools/models_analysis/__init__.py
--rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.81/src/gmltools/models_analysis/classification_analysis.py
--rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.81/src/gmltools/models_analysis/xai.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.522419 gmltools-0.0.81/src/gmltools/preprocess/
--rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.81/src/gmltools/preprocess/__init__.py
--rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.81/src/gmltools/preprocess/autoregressive_features.py
--rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.81/src/gmltools/preprocess/manage_holidays.py
--rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.81/src/gmltools/preprocess/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-06-14 08:54:29.502258 gmltools-0.0.81/src/gmltools.egg-info/
--rw-rw-rw-   0        0        0     1021 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      906 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      137 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-14 08:54:29.000000 gmltools-0.0.81/src/gmltools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 15:34:26.078104 gmltools-0.0.82/
+-rw-rw-rw-   0        0        0    35782 2023-03-08 11:55:03.000000 gmltools-0.0.82/LICENSE
+-rw-rw-rw-   0        0        0    10875 2023-03-07 08:36:17.000000 gmltools-0.0.82/Models.ipynb
+-rw-rw-rw-   0        0        0     1021 2023-06-26 15:34:26.077043 gmltools-0.0.82/PKG-INFO
+-rw-rw-rw-   0        0        0      755 2023-03-09 09:37:42.000000 gmltools-0.0.82/README.md
+-rw-rw-rw-   0        0        0    17876 2023-03-16 08:30:12.000000 gmltools-0.0.82/gmltools.yml
+-rw-rw-rw-   0        0        0    17555 2023-03-06 11:09:12.000000 gmltools-0.0.82/mltools.yml
+-rw-rw-rw-   0        0        0      618 2023-06-26 15:33:34.000000 gmltools-0.0.82/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-26 15:34:26.079114 gmltools-0.0.82/setup.cfg
+-rw-rw-rw-   0        0        0     1746 2023-06-26 15:33:09.000000 gmltools-0.0.82/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:34:25.833625 gmltools-0.0.82/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 15:34:25.913647 gmltools-0.0.82/src/gmltools/
+-rw-rw-rw-   0        0        0      879 2023-03-14 15:28:10.000000 gmltools-0.0.82/src/gmltools/To_Do.txt
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.82/src/gmltools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:34:25.939075 gmltools-0.0.82/src/gmltools/eda/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:28.000000 gmltools-0.0.82/src/gmltools/eda/__init__.py
+-rw-rw-rw-   0        0        0    45883 2023-06-26 15:33:16.000000 gmltools-0.0.82/src/gmltools/eda/eda.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:34:26.000450 gmltools-0.0.82/src/gmltools/models/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:51:09.000000 gmltools-0.0.82/src/gmltools/models/__init__.py
+-rw-rw-rw-   0        0        0     4893 2023-03-13 11:20:44.000000 gmltools-0.0.82/src/gmltools/models/bayes.py
+-rw-rw-rw-   0        0        0     1983 2023-03-16 08:43:00.000000 gmltools-0.0.82/src/gmltools/models/custom_scorings.py
+-rw-rw-rw-   0        0        0     5653 2023-05-24 10:54:18.000000 gmltools-0.0.82/src/gmltools/models/dummy_model.py
+-rw-rw-rw-   0        0        0   160613 2023-06-14 08:54:19.000000 gmltools-0.0.82/src/gmltools/models/model.py
+-rw-rw-rw-   0        0        0     7038 2023-06-06 11:25:02.000000 gmltools-0.0.82/src/gmltools/models/models_info.py
+-rw-rw-rw-   0        0        0    24373 2023-06-26 15:33:19.000000 gmltools-0.0.82/src/gmltools/models/timeseriesplit.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:34:26.030677 gmltools-0.0.82/src/gmltools/models_analysis/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:54.000000 gmltools-0.0.82/src/gmltools/models_analysis/__init__.py
+-rw-rw-rw-   0        0        0    73636 2023-04-30 15:51:16.000000 gmltools-0.0.82/src/gmltools/models_analysis/classification_analysis.py
+-rw-rw-rw-   0        0        0     5653 2023-04-30 15:57:34.000000 gmltools-0.0.82/src/gmltools/models_analysis/xai.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:34:26.074530 gmltools-0.0.82/src/gmltools/preprocess/
+-rw-rw-rw-   0        0        0      327 2023-03-08 11:50:40.000000 gmltools-0.0.82/src/gmltools/preprocess/__init__.py
+-rw-rw-rw-   0        0        0    18728 2023-03-06 08:35:56.000000 gmltools-0.0.82/src/gmltools/preprocess/autoregressive_features.py
+-rw-rw-rw-   0        0        0     8133 2023-02-23 12:30:28.000000 gmltools-0.0.82/src/gmltools/preprocess/manage_holidays.py
+-rw-rw-rw-   0        0        0     4045 2023-03-30 08:41:18.000000 gmltools-0.0.82/src/gmltools/preprocess/preprocess.py
+drwxrwxrwx   0        0        0        0 2023-06-26 15:34:25.927377 gmltools-0.0.82/src/gmltools.egg-info/
+-rw-rw-rw-   0        0        0     1021 2023-06-26 15:34:24.000000 gmltools-0.0.82/src/gmltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2023-06-26 15:34:25.000000 gmltools-0.0.82/src/gmltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 15:34:24.000000 gmltools-0.0.82/src/gmltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-06-26 15:34:24.000000 gmltools-0.0.82/src/gmltools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 15:34:24.000000 gmltools-0.0.82/src/gmltools.egg-info/top_level.txt
```

### Comparing `gmltools-0.0.81/LICENSE` & `gmltools-0.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/Models.ipynb` & `gmltools-0.0.82/Models.ipynb`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/PKG-INFO` & `gmltools-0.0.82/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.81
+Version: 0.0.82
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.81/README.md` & `gmltools-0.0.82/README.md`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/gmltools.yml` & `gmltools-0.0.82/gmltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/mltools.yml` & `gmltools-0.0.82/mltools.yml`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/pyproject.toml` & `gmltools-0.0.82/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmltools"
-version = "0.0.81"
+version = "0.0.82"
 description = "Machine Learning library aiming for a higher level programming, organizing best tools"
 authors = ["Diego Sanz-Gadea Sánchez"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gmltools-0.0.81/setup.py` & `gmltools-0.0.82/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.6.3,<4.0.0', 'numpy>=1.21.6,<2.0.0', 'pandas>=1.5.0,<2.0.0', 'xgboost==1.5.0', 'lightgbm>=3.3.5', 'linear-tree>=0.3.5', 'scikit-learn>=1.2.1']
 
 setup_kwargs = {
     'name': 'gmltools',
-    'version': '0.0.81',
+    'version': '0.0.82',
     'description': 'Machine Learning library aiming for a higher level programming, organizing best tools',
     'long_description': '# gmltools\n\nMachine Learning library aiming for a higher level programming, organizing best tools\n\n```bash\n$ pip install gmltools\n```\n\n## Usage\n\n- TODO\n\n## Contributing\n\nInterested in contributing? Check out the contributing guidelines. Please note that this project is released with a Code of Conduct. By contributing to this project, you agree to abide by its terms.\n\n## License\n\n`gmltutils` was created by Diego Sanz-Gadea Sánchez. It is licensed under the terms of the GNU General Public License v3.0 license.\n\n## Credits\n\n`gmltutils` was created with [`cookiecutter`](https://cookiecutter.readthedocs.io/en/latest/) and the `py-pkgs-cookiecutter` [template](https://github.com/py-pkgs/py-pkgs-cookiecutter).\n',
     'author': 'Diego Sanz-Gadea Sánchez',
     'author_email': 'dsanzgadeasanchez@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `gmltools-0.0.81/src/gmltools/To_Do.txt` & `gmltools-0.0.82/src/gmltools/To_Do.txt`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/eda/eda.py` & `gmltools-0.0.82/src/gmltools/eda/eda.py`

 * *Files 3% similar despite different names*

```diff
@@ -803,15 +803,15 @@
         self.df = df
         self.subsequence = subsequence
         self.y = df.stack().reset_index(drop=True)
         self.x = df.stack().reset_index(drop=True).index
         self.m = subsequence*df.columns.size
         
     def get_matrix_profile(self):
-        
+
         matrix_profile = stumpy.stump(self.y, self.m)
         self.matrix_profile_df = pd.DataFrame(matrix_profile, columns=['profile', 'profile index', 'left profile index', 'right profile index'])
         return self.matrix_profile_df
     
     def _get_values(self,df,columns,remove_):
         """
         Obtains the different values of a dataframe selecting the columns to seek
@@ -847,59 +847,126 @@
         -------
         patron: str or tuple
             Date of the similar pattern
         """
         slice_index=self.df.index.get_loc(date)
         start_index=slice_index.start
         self.stumpy_index=start_index*self.df.columns.size
-
+        patron=0 #initialize the patron variable
         matrix_profile_df=self.get_matrix_profile()
         matrix_profile_df_=matrix_profile_df[(matrix_profile_df['right profile index'] != -1) & (matrix_profile_df['left profile index'] != -1)]
-        self.seek_motif=matrix_profile_df[matrix_profile_df['profile index'] == self.stumpy_index]
-        close_values=self._get_values(self.seek_motif,['left profile index','right profile index'],self.stumpy_index.item())
-        self.stumpy_close_values=close_values
-        self.close_values=close_values/self.df.columns.size
-        self.close_values=self.close_values.astype(int)
-            
+        try:
+            self.seek_motif=matrix_profile_df[matrix_profile_df['profile index'] == self.stumpy_index]
+            #order the values of the seek motif smallest to biggest on column profile
+            self.seek_motif=self.seek_motif.sort_values(by="profile")
 
-        patron= [self.df.iloc[int(i)].to_frame().T.index[0].strftime('%Y-%m-%d') for i in self.close_values]
+        
+            close_values=self._get_values(self.seek_motif,['left profile index','right profile index'],self.stumpy_index.item())
+        except:
+            try:
+                self.seek_motif=matrix_profile_df[matrix_profile_df['right profile index'] == self.stumpy_index]
+                self.seek_motif=self.seek_motif.sort_values(by="profile")
+                close_values=self._get_values(self.seek_motif,['left profile index','right profile index'],self.stumpy_index.item())
+
+            except:
+                try:
+                    self.seek_motif=matrix_profile_df[matrix_profile_df['left profile index'] == self.stumpy_index]
+                    self.seek_motif=self.seek_motif.sort_values(by="profile")
+                    close_values=self._get_values(self.seek_motif,['left profile index','right profile index'],self.stumpy_index.item())
+                except:
+                    patron= ["No se ha podido encontrar el día más parecido"]
+
+        if patron != ["No se ha podido encontrar el día más parecido"]:            
+
+            self.stumpy_close_values=close_values
+            #if in the self.stumpy close values ther is -1 value, and tehres also a 0 quit the -1 and if there irs only a -1 alone convert it to 0
+            if -1 in self.stumpy_close_values:
+
+                if 0 in close_values:
+                    self.stumpy_close_values=self.stumpy_close_values[self.stumpy_close_values!=-1]
+                else:
+                    self.stumpy_close_values[self.stumpy_close_values==-1]=0
+            self.close_values=close_values/self.df.columns.size
+            self.close_values=self.close_values.astype(int)
+                
+
+            patron= [self.df.iloc[int(i)].to_frame().T.index[0].strftime('%Y-%m-%d') for i in self.close_values]
+        else:
+            pass
 
         return patron
     
     def plot_similar_pattern(self,date):
         """
         Plot similar pattern of a given date
         Parameters
         ----------
         date : str
             Date to plot similar pattern
         """
         patron=self.get_similar_pattern(date)
+        #drop on eif its duplicated
+        patron=list(set(patron))
         self.patron=patron
         height_adjuts= len(patron)
-        try:
-            patron_profile=[pat + ", " + str(round(self.seek_motif.reset_index().profile.iloc[i],3)) for i, pat in enumerate(patron)]
-        except:
+        if patron != ["No se ha podido encontrar el día más parecido"]:
+            try:
+                patron_profile=[pat + ", " + str(round(self.seek_motif.reset_index().profile.iloc[i],3)) for i, pat in enumerate(patron)]
+            except:
+                
+                patron_profile=patron
+
+            fig = make_subplots(rows=len(patron), cols=1, vertical_spacing=0.1, subplot_titles= patron_profile , )
+
+            for i,idx in enumerate(self.stumpy_close_values):
+                plot_y = self.y.iloc[idx:idx.item()+self.m].to_list()
+                plot_base = self.y.iloc[self.stumpy_index:self.stumpy_index+self.m].to_list()
             
-            patron_profile=patron
+                fig.add_trace(go.Scatter(x=np.linspace(0,self.subsequence-1,len(list(range(len(plot_y))))), y=plot_y, name=patron[i] ), row=i+1, col=1)
+                fig.add_trace(go.Scatter(x=np.linspace(0,self.subsequence-1,len(list(range(len(plot_base))))), y=plot_base, name=date, line={'color': '#000000'}), row=i+1, col=1)
+                fig.update_yaxes(title_text="Serie {}".format(i+1), row=i+1, col=1)
+
+            #indicate all int x values in the x axis
+                fig.update_xaxes(tickmode = 'array', tickvals = np.linspace(0,self.subsequence-1,self.subsequence), row=i+1, col=1)
+            fig.update_layout(title_text=f"Patrones similares para {date} {self.df.columns.values}", title_x=0.5, height=800+height_adjuts*100)
+            #x name as Hour
+            fig.update_xaxes(title_text="Hour", tickfont=dict(size=24))
+            fig.update_yaxes(title_text="Valor", tickfont=dict(size=24))
+
+            if len(patron) ==1:
+                height=1200/1.4
+                width=3950
+            else:
+                height=1200
+                width=3950
+            #tight layout automatically adjusts subplot params so that the subplot(s) fits in to the figure area
+            fig.update_layout(showlegend=True, title_x=0.5, title_y=0.999, title_font_size=45, title_font_color="black", title_font_family="Arial", title_xanchor="center", title_yanchor="top",
+                            margin=dict(t=100, b=50, l=50, r=50),legend=dict(font=dict(size=35)), height=height, width=width) 
+            fig.update_annotations(font_size=40)
+            #increase size of xticks values
+
+            fig.show()
+        else:
+            fig = go.Figure()
+
+            fig.add_annotation(
+                dict(
+                    x=0.5, # posición en x
+                    y=0.5, # posición en y
+                    showarrow=False,
+                    text="No se ha podido encontrar el día más parecido", # mensaje de texto
+                    xref="paper",
+                    yref="paper",
+                    font=dict(size=45, color='black'), # tamaño y color del texto
+                )
+            )
+            fig.update_layout(title_text=f"Patrones similares para {date} {self.df.columns.values}", title_x=0.5, height=800+height_adjuts*100, title_font_size=45)
+            fig.update_layout(
+                xaxis=dict(showgrid=False, zeroline=False, showticklabels=False), # esconde el eje x
+                yaxis=dict(showgrid=False, zeroline=False, showticklabels=False), # esconde el eje y
+                height=1200/1.4,
 
-        fig = make_subplots(rows=len(patron), cols=1, vertical_spacing=0.1, subplot_titles= patron_profile )
-
-        for i,idx in enumerate(self.stumpy_close_values):
-            plot_y = self.y.iloc[idx:idx.item()+self.m].to_list()
-            plot_base = self.y.iloc[self.stumpy_index:self.stumpy_index+self.m].to_list()
-           
-            fig.add_trace(go.Scatter(x=np.linspace(0,self.subsequence-1,len(list(range(len(plot_y))))), y=plot_y, name=patron[i] ), row=i+1, col=1)
-            fig.add_trace(go.Scatter(x=np.linspace(0,self.subsequence-1,len(list(range(len(plot_base))))), y=plot_base, name=date, line={'color': '#000000'}), row=i+1, col=1)
-            fig.update_yaxes(title_text="Serie {}".format(i+1), row=i+1, col=1)
-
-        #indicate all int x values in the x axis
-            fig.update_xaxes(tickmode = 'array', tickvals = np.linspace(0,self.subsequence-1,self.subsequence), row=i+1, col=1)
-        fig.update_layout(title_text="Patrones similares para {}".format(date), title_x=0.5, height=800+height_adjuts*100)
-        #x name as Hour
-        fig.update_xaxes(title_text="Hour")
-        fig.update_yaxes(title_text="Valor")
-        #tight layout automatically adjusts subplot params so that the subplot(s) fits in to the figure area
-        fig.update_layout(showlegend=True, title_x=0.5, title_font_size=20, title_font_color="black", title_font_family="Arial", title_xanchor="center", title_yanchor="top",
-                          margin=dict(t=100, b=50, l=50, r=50))
-        fig.show()
+                width=3950)
+            
+            fig.show()
 
+        self.fig=fig
```

### Comparing `gmltools-0.0.81/src/gmltools/models/bayes.py` & `gmltools-0.0.82/src/gmltools/models/bayes.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/models/custom_scorings.py` & `gmltools-0.0.82/src/gmltools/models/custom_scorings.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/models/dummy_model.py` & `gmltools-0.0.82/src/gmltools/models/dummy_model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/models/model.py` & `gmltools-0.0.82/src/gmltools/models/model.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/models/models_info.py` & `gmltools-0.0.82/src/gmltools/models/models_info.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/models/timeseriesplit.py` & `gmltools-0.0.82/src/gmltools/models/timeseriesplit.py`

 * *Files 23% similar despite different names*

```diff
@@ -321,7 +321,276 @@
             plt.text(train_size[i]+test_size_[i]+1000, i+1, f"Train: {train_size[i]*100/n_samples:.2f}%  Test: {test_size_[i]*100/n_samples:.2f}%", fontsize=7)
 
         #extend the frame to the right to make room for the text
         plt.xlim(0, n_samples+n_samples*0.43)
 
     plt.show()
 
+
+
+
+
+
+class TimeSeriesWindowSplit():
+    """Time Series cross-validator with initial period
+    Provides time series splits for rolling origin type 
+    cross validation. This means users may set an initial
+    time period. gap size, and increment_size and intra gap.
+    Parameters:
+        initial : int, default=21
+            Number of splits.
+        increment_size : int, default=7
+            Sets the size of the test set to be added at each iteration
+        gap : int, default=0
+            Number of samples to exclude from the end of each train set before
+            the test set.
+        intra_gap : int, default=0
+            Number of samples of train to add constantly to the end of each train split.
+            Its apply after the fisrt split
+    Examples:
+    ```py
+
+    X = np.arange(0,50)
+    tscv = TimeSeriesInitialSplit(initial=20, increment_size=7, gap=0, intra_gap=0)
+    for train_index, test_index in tscv.split(X):
+        print("TRAIN:", train_index, "TEST:", test_index)
+        X_train, X_test = X[train_index], X[test_index]
+    > TRAIN: [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20] TEST: [21 22 23 24 25 26 27]
+    > TRAIN: [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27] TEST: [28 29 30 31 32 33 34]
+    > TRAIN: [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34] TEST: [35 36 37 38 39 40 41]
+    > TRAIN: [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 33 34 35 36 37 38 39 40 41] TEST: [42 43 44 45 46 47 48]
+    ```
+
+    ```py
+    X = np.arange(0,50)
+
+    tscv = TimeSeriesInitialSplit(initial=20, increment_size=7, gap=0,intra_gap=3)
+    for train_index, test_index in tscv.split(X):
+        print("TRAIN:", train_index, "TEST:", test_index)
+        X_train, X_test = X[train_index], X[test_index]
+    
+    > TRAIN: [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19] TEST: [20 21 22 23 24 25 26]
+    > TRAIN: [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 ] TEST: [30 31 32 33 34 35 36]
+    > TRAIN: [ 0  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30 31 32 32 33 34 35 36 37 38 39] TEST: [40 41 42 43 44 45 46]
+    """
+
+    def __init__(self, initial=7 * 3, increment_size=7, gap=0,intra_gap=0):
+        self.initial = initial
+        self.increment_size = increment_size
+        self.gap = gap
+        self.intra_gap=intra_gap
+        self.is_timeseriesinitialsplit = True
+
+
+    def split(self, X, y=None, groups=None):
+        """Generate indices to split data into training and test set.
+        Parameters:
+            X : array-like of shape (n_samples, n_features)
+                Training data, where `n_samples` is the number of samples
+                and `n_features` is the number of features.
+        Yields: 
+            train : ndarray
+                The training set indices for that split.
+            test : ndarray
+                The testing set indices for that split.
+        """
+        if isinstance(self.initial, str):
+            assert re.match(r"^\d{4}-\d{2}-\d{2}$", self.initial) or re.match(r"^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$", self.initial), "date format should be YYYY-MM-DD or YYYY-MM-DD HH:MM:SS, the same index as dataframe"
+            #obatin the iloc index of self.initial date
+            self.initial = X.index.get_loc(self.initial)
+        n_samples = len(X)
+        initial = self.initial
+        gap = self.gap
+        intra_gap=self.intra_gap
+        increment_size = self.increment_size
+
+        # Make sure we have enough samples for the given split parameters
+        if initial > n_samples:
+            raise ValueError(
+                f"Cannot have number of initial_size={initial} greater"
+                f" than the number of samples={n_samples}."
+            )
+        if n_samples - initial - increment_size - gap < 0:
+            raise ValueError(
+                f"Size of initial + increment_size + gap too large given sample"
+                f"={n_samples} with initial={initial} increment_size={increment_size} and gap={gap}."
+            )
+
+        indices = np.arange(n_samples)
+        test_starts = range(initial, n_samples, increment_size)
+        for i,test_start in enumerate(test_starts):
+            if i == 0 :
+                test = indices[test_start + gap : test_start + increment_size + gap]
+                if len(test) < increment_size:
+                    # break if the test set is smaller than a complete increment_size
+                    break
+                else:
+                    yield (
+                        indices[:test_start],
+                        indices[test_start + gap : test_start  + increment_size + gap],
+                    )
+            else:
+                test = indices[test_start + gap + intra_gap: test_start + increment_size + intra_gap + gap]
+                if len(test) < increment_size:
+                    # break if the test set is smaller than a complete increment_size
+                    break
+                else:
+                    yield (
+                        indices[i*increment_size:test_start+ intra_gap], #train
+                        indices[test_start + gap + intra_gap: test_start + intra_gap + increment_size + gap], #test
+                    )
+
+    def get_n_splits(self, X, y=None, groups=None)->int:
+        """
+        Returns the number of splitting iterations in the cross-validator
+
+        Parameters
+        ----------
+        
+        X : array-like of shape (n_samples, n_features)
+            Training data, where `n_samples` is the number of samples
+            and `n_features` is the number of features.
+
+        y : array-like of shape (n_samples,), default=None
+            The target variable for supervised learning problems.
+        
+        groups : array-like of shape (n_samples,), default=None
+            Group labels for the samples used while splitting the dataset into
+
+        Returns
+        -------
+        n_splits : int
+        """
+
+        n_samples = len(X)
+
+        # Make sure we have enough samples for the given split parameters
+        if self.initial > n_samples:
+            raise ValueError(
+                f"Cannot have number of initial_size={self.initial} greater"
+                f" than the number of samples={n_samples}."
+            )
+        if n_samples - self.initial - self.increment_size - self.gap < 0:
+            raise ValueError(
+                f"Size of initial + increment_size + gap too large given sample"
+                f"={n_samples} with initial={self.initial} increment_size={self.increment_size} and gap={self.gap}."
+            )
+        n_splits=0
+        for train_index, test_index in self.split(X):
+            n_splits +=1
+        return n_splits
+    
+    def get_index_splits(self,X,y=None,groups=None):
+        """
+        Returns the index of the train and test sets for each split
+
+        Parameters
+        ----------
+
+        X : array-like of shape (n_samples, n_features)
+            Training data, where `n_samples` is the number of samples
+            and `n_features` is the number of features.
+
+        y : array-like of shape (n_samples,), default=None
+            The target variable for supervised learning problems.
+
+        groups : array-like of shape (n_samples,), default=None
+            Group labels for the samples used while splitting the dataset into
+
+        Returns
+        -------
+        X_train_date : list
+            List of the index of the train set for each split
+        X_test_date : list
+            List of the index of the test set for each split
+        """
+        train_real_index=[]
+        test_real_index=[]
+        for train_index, test_index in self.split(X):
+            train_real_index.append(X.index[train_index])
+            test_real_index.append(X.index[test_index])
+
+        return train_real_index,test_real_index
+    
+    def get_test_days(self,X,y=None,groups=None):
+        """
+        Returns the days of the test sets for each split
+
+        Parameters
+        ----------
+        X : array-like of shape (n_samples, n_features)
+            Training data, where `n_samples` is the number of samples
+
+        y : array-like of shape (n_samples,), default=None
+            The target variable for supervised learning problems.
+
+        groups : array-like of shape (n_samples,), default=None
+            Group labels for the samples used while splitting the dataset into
+
+        Returns
+        -------
+        test_days : list
+            List of the days of the test set for each split
+        """
+        test_days=[]
+        train_real_index,test_real_index=self.get_index_splits(X)
+        for day in test_real_index:
+            day_=np.unique(day.date)
+            test_days.append(day_[0].strftime("%Y-%m-%d"))
+        return test_days
+    def __repr__(self):
+        return "TimeSeriesWindowSplit(initial={}, increment_size={}, gap={}, intra_gap={})".format(
+            self.initial, self.increment_size, self.gap, self.intra_gap
+        )
+
+def plot_timesplit(n_splits, n_samples,test_size=None , min_train_size=None, text=False,figsize=(20,10)):
+
+    """
+    Plot the train and test size depending on the number of splits for TimeSeriesSplit
+
+    Parameters
+    ----------
+    n_splits : int
+        Number of splits.
+
+    n_samples : int
+        Number of samples.
+    
+    test_size : int, optional
+        Size of the test set, by default None
+    
+    text : bool, optional
+        Add the percentage of the train and test size to the side of the bar, by default False
+
+    Returns
+    -------
+    None
+        Plot the train and test size depending on the number of splits for TimeSeriesSplit
+    """
+
+    n_splits=n_splits
+    n_samples=n_samples
+    if test_size is None:
+        test_size= n_samples // (n_splits+1)
+    train_size=[]
+    test_size_=[]
+    plt.figure(figsize=figsize)
+    for i in reversed(range(1,n_splits+1)):
+        train_set=i * n_samples // (n_splits + 1) + n_samples % (n_splits + 1)
+        train_size.append(train_set)
+        test_size_.append(test_size)
+    plt.barh(np.arange(1,n_splits+1),train_size)
+    plt.barh(np.arange(1,n_splits+1),test_size_, left=train_size)
+    plt.legend(["Train Size", "Test Size"])
+    plt.xlabel("Number of Splits")
+    plt.ylabel("Size")
+    plt.title("Train and Test Size depending on the number of splits")
+    #add the percentage of the train and test size to the side of the bar
+    if text == True:
+        for i in range(n_splits):
+            plt.text(train_size[i]+test_size_[i]+1000, i+1, f"Train: {train_size[i]*100/n_samples:.2f}%  Test: {test_size_[i]*100/n_samples:.2f}%", fontsize=7)
+
+        #extend the frame to the right to make room for the text
+        plt.xlim(0, n_samples+n_samples*0.43)
+
+    plt.show()
+
```

### Comparing `gmltools-0.0.81/src/gmltools/models_analysis/classification_analysis.py` & `gmltools-0.0.82/src/gmltools/models_analysis/classification_analysis.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/models_analysis/xai.py` & `gmltools-0.0.82/src/gmltools/models_analysis/xai.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/preprocess/autoregressive_features.py` & `gmltools-0.0.82/src/gmltools/preprocess/autoregressive_features.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/preprocess/manage_holidays.py` & `gmltools-0.0.82/src/gmltools/preprocess/manage_holidays.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools/preprocess/preprocess.py` & `gmltools-0.0.82/src/gmltools/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `gmltools-0.0.81/src/gmltools.egg-info/PKG-INFO` & `gmltools-0.0.82/src/gmltools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmltools
-Version: 0.0.81
+Version: 0.0.82
 Summary: Machine Learning library aiming for a higher level programming, organizing best tools
 Author: Diego Sanz-Gadea Sánchez
 Author-email: dsanzgadeasanchez@gmail.com
 Requires-Python: >=3.9,<4.0
 License-File: LICENSE
 
 # gmltools
```

### Comparing `gmltools-0.0.81/src/gmltools.egg-info/SOURCES.txt` & `gmltools-0.0.82/src/gmltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

