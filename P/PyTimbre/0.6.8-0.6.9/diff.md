# Comparing `tmp/PyTimbre-0.6.8.tar.gz` & `tmp/PyTimbre-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTimbre-0.6.8.tar", last modified: Mon Apr 24 21:56:27 2023, max compression
+gzip compressed data, was "PyTimbre-0.6.9.tar", last modified: Tue Apr 25 22:56:06 2023, max compression
```

## Comparing `PyTimbre-0.6.8.tar` & `PyTimbre-0.6.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.908564 PyTimbre-0.6.8/
--rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.8/LICENSE.txt
--rw-rw-rw-   0        0        0    13338 2023-04-24 21:56:27.907567 PyTimbre-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     5289 2023-04-13 01:01:21.000000 PyTimbre-0.6.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 21:56:27.908564 PyTimbre-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-04-24 21:55:20.000000 PyTimbre-0.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.841008 PyTimbre-0.6.8/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.853483 PyTimbre-0.6.8/src/PyTimbre.egg-info/
--rw-rw-rw-   0        0        0    13338 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 21:56:27.000000 PyTimbre-0.6.8/src/PyTimbre.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.861785 PyTimbre-0.6.8/src/pytimbre/
--rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.6.8/src/pytimbre/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.881215 PyTimbre-0.6.8/src/pytimbre/audio_files/
--rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.8/src/pytimbre/audio_files/__init__.py
--rw-rw-rw-   0        0        0    23794 2023-04-14 21:21:46.000000 PyTimbre-0.6.8/src/pytimbre/audio_files/ansi_standard_formatted_files.py
--rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.6.8/src/pytimbre/audio_files/calibrated_binary_files.py
--rw-rw-rw-   0        0        0    70669 2023-03-31 16:13:47.000000 PyTimbre-0.6.8/src/pytimbre/audio_files/wavefile.py
-drwxrwxrwx   0        0        0        0 2023-04-24 21:56:27.906556 PyTimbre-0.6.8/src/pytimbre/spectral/
--rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.8/src/pytimbre/spectral/__init__.py
--rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.6.8/src/pytimbre/spectral/acoustic_weights.py
--rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.6.8/src/pytimbre/spectral/fractional_octave_band.py
--rw-rw-rw-   0        0        0    16910 2023-04-15 02:25:52.000000 PyTimbre-0.6.8/src/pytimbre/spectral/fundamental_frequency.py
--rw-rw-rw-   0        0        0    58636 2023-04-21 14:52:01.000000 PyTimbre-0.6.8/src/pytimbre/spectral/spectra.py
--rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.6.8/src/pytimbre/spectral/spectrogram.py
--rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.6.8/src/pytimbre/spectral/swipe.py
--rw-rw-rw-   0        0        0    32278 2023-04-24 21:48:22.000000 PyTimbre-0.6.8/src/pytimbre/spectral/time_histories.py
--rw-rw-rw-   0        0        0    85520 2023-04-24 21:54:08.000000 PyTimbre-0.6.8/src/pytimbre/waveform.py
--rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.6.8/src/pytimbre/yin.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:56:06.042948 PyTimbre-0.6.9/
+-rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    13388 2023-04-25 22:56:06.041929 PyTimbre-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2023-04-25 22:51:37.000000 PyTimbre-0.6.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 22:56:06.043960 PyTimbre-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     1072 2023-04-25 22:52:22.000000 PyTimbre-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:56:05.913020 PyTimbre-0.6.9/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 22:56:05.950152 PyTimbre-0.6.9/src/PyTimbre.egg-info/
+-rw-rw-rw-   0        0        0    13388 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 22:56:05.968586 PyTimbre-0.6.9/src/pytimbre/
+-rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.6.9/src/pytimbre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:56:05.996687 PyTimbre-0.6.9/src/pytimbre/audio_files/
+-rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.9/src/pytimbre/audio_files/__init__.py
+-rw-rw-rw-   0        0        0    23794 2023-04-14 21:21:46.000000 PyTimbre-0.6.9/src/pytimbre/audio_files/ansi_standard_formatted_files.py
+-rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.6.9/src/pytimbre/audio_files/calibrated_binary_files.py
+-rw-rw-rw-   0        0        0    69970 2023-04-25 22:21:07.000000 PyTimbre-0.6.9/src/pytimbre/audio_files/wavefile.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:56:06.039895 PyTimbre-0.6.9/src/pytimbre/spectral/
+-rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.9/src/pytimbre/spectral/__init__.py
+-rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.6.9/src/pytimbre/spectral/acoustic_weights.py
+-rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.6.9/src/pytimbre/spectral/fractional_octave_band.py
+-rw-rw-rw-   0        0        0    16910 2023-04-15 02:25:52.000000 PyTimbre-0.6.9/src/pytimbre/spectral/fundamental_frequency.py
+-rw-rw-rw-   0        0        0    58636 2023-04-21 14:52:01.000000 PyTimbre-0.6.9/src/pytimbre/spectral/spectra.py
+-rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.6.9/src/pytimbre/spectral/spectrogram.py
+-rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.6.9/src/pytimbre/spectral/swipe.py
+-rw-rw-rw-   0        0        0    32410 2023-04-25 22:23:53.000000 PyTimbre-0.6.9/src/pytimbre/spectral/time_histories.py
+-rw-rw-rw-   0        0        0    85520 2023-04-24 21:54:08.000000 PyTimbre-0.6.9/src/pytimbre/waveform.py
+-rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.6.9/src/pytimbre/yin.py
```

### Comparing `PyTimbre-0.6.8/LICENSE.txt` & `PyTimbre-0.6.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/PKG-INFO` & `PyTimbre-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+![PyTimbre Logo](pytimbre_bing_gen_a.png " ") 
+
 # PyTimbre
 
 ## PyTimbre is a Python conversion of the Matlab package Timbre Toolbox, found here (https://github.com/VincentPerreault0/timbretoolbox).
 
 This package was created in association with work conducted at the United States Air Force Research Laboratory on human 
 perception of sound. Generally, models of perception have focused on sound pressure level spectra, and time histories of 
 sound pressure. But auditory detection, identification/classification, and localization may be described better by
```

### Comparing `PyTimbre-0.6.8/README.md` & `PyTimbre-0.6.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![PyTimbre Logo](pytimbre_bing_gen_a.png " ") 
+
 # PyTimbre
 
 ## PyTimbre is a Python conversion of the Matlab package Timbre Toolbox, found here (https://github.com/VincentPerreault0/timbretoolbox).
 
 This package was created in association with work conducted at the United States Air Force Research Laboratory on human 
 perception of sound. Generally, models of perception have focused on sound pressure level spectra, and time histories of 
 sound pressure. But auditory detection, identification/classification, and localization may be described better by
```

### Comparing `PyTimbre-0.6.8/setup.py` & `PyTimbre-0.6.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         HISTORY = history_file.read()
 
         with open('LICENSE.txt') as license_file:
             LICENSE = license_file.read()
 
 setup(
     name='PyTimbre',
-    version='0.6.8',
+    version='0.6.9',
     description='Python conversion of Timbre Toolbox',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY + '\n\n' + LICENSE,
     license='MIT',
     packages=find_packages('src'),
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
```

### Comparing `PyTimbre-0.6.8/src/PyTimbre.egg-info/PKG-INFO` & `PyTimbre-0.6.9/src/PyTimbre.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+![PyTimbre Logo](pytimbre_bing_gen_a.png " ") 
+
 # PyTimbre
 
 ## PyTimbre is a Python conversion of the Matlab package Timbre Toolbox, found here (https://github.com/VincentPerreault0/timbretoolbox).
 
 This package was created in association with work conducted at the United States Air Force Research Laboratory on human 
 perception of sound. Generally, models of perception have focused on sound pressure level spectra, and time histories of 
 sound pressure. But auditory detection, identification/classification, and localization may be described better by
```

### Comparing `PyTimbre-0.6.8/src/PyTimbre.egg-info/SOURCES.txt` & `PyTimbre-0.6.9/src/PyTimbre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/audio_files/ansi_standard_formatted_files.py` & `PyTimbre-0.6.9/src/pytimbre/audio_files/ansi_standard_formatted_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/audio_files/calibrated_binary_files.py` & `PyTimbre-0.6.9/src/pytimbre/audio_files/calibrated_binary_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/audio_files/wavefile.py` & `PyTimbre-0.6.9/src/pytimbre/audio_files/wavefile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1253,15 +1253,15 @@
         :param s1: int - the ending sample for the reading of the audio file
         :param fs: int - the number of samples per second.  This facilitates calling the based class with the required
             data
         :param samples: ndarray - the actual samples to define the waveform
         :param time: float or datetime - the time of the first sample
         """
 
-        warnings.warn('Test for Insert Start Time using wfm.start_time=...is failing.')
+        # warnings.warn('Test for Insert Start Time using wfm.start_time=...is failing.')
         # TODO - Correct the wfm.start_time setting feature.
 
         if path is None:
             if(fs is None) and (samples is None) and (time is None):
                 self.samples = None
                 self.start_time = None
                 self.sample_rate = None
@@ -1857,41 +1857,18 @@
         the function returns the approximate frequency of the tone.  This will examine every channel and determine
         whether each channel is a calibration tone
 
         :returns: bool - flag determining whether the signal was pure tone
                   float - the approximate frequency of the pure tone
         """
 
-        calibration = None
-        frequency = None
-
         #   Loop through the channels
-
-        for ch_idx in range(self.channel_count):
-            #   To remove high frequency transients, we pass the signal through a 2 kHz low pass filter
-
-            wfm = Waveform(self.samples[:, ch_idx], self.sample_rate, self.start_time).apply_lowpass(2000)
-
-            peaks = scipy.signal.find_peaks(wfm.samples, height=0.8 * np.max(self.samples[:, ch_idx]))[0]
-
-            if len(peaks) >= 2:
-                calibration = np.zeros((self.samples.shape[1],), dtype=bool)
-                frequency = np.zeros((self.samples.shape[1],), dtype=float)
-
-                #   Determine the distance between any two adjacent peaks
-
-                distance_sample = np.diff(peaks)
-
-                #   Determine the distance between the samples in time
-
-                distance_time = distance_sample / self.sample_rate
-
-                #   Determine the frequencies
-
-                frequencies = 1 / distance_time
-
-                frequency = np.mean(frequencies)
-
-                calibration = (abs(frequencies[ch_idx]-1000) < 0.1 * 1000) or \
-                                      (abs(frequencies[ch_idx]-250) < 0.1 * 250)
-
-        return calibration, frequency
+        if self.channel_count > 1:
+            calibration = np.zeros((self.channel_count,))
+            frequency = np.zeros((self.channel_count,))
+
+            for ch_idx in range(self.channel_count):
+                wfm = Waveform(self.samples[:, ch_idx], self.sample_rate, self.start_time).apply_lowpass(2000)
+                calibration[ch_idx], frequency[ch_idx] = wfm.is_calibration()
+        else:
+            wfm = Waveform(self.samples, self.sample_rate, self.start_time).apply_lowpass(2000)
+            return wfm.is_calibration()
```

### Comparing `PyTimbre-0.6.8/src/pytimbre/spectral/acoustic_weights.py` & `PyTimbre-0.6.9/src/pytimbre/spectral/acoustic_weights.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/spectral/fractional_octave_band.py` & `PyTimbre-0.6.9/src/pytimbre/spectral/fractional_octave_band.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/spectral/fundamental_frequency.py` & `PyTimbre-0.6.9/src/pytimbre/spectral/fundamental_frequency.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/spectral/spectra.py` & `PyTimbre-0.6.9/src/pytimbre/spectral/spectra.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/spectral/spectrogram.py` & `PyTimbre-0.6.9/src/pytimbre/spectral/spectrogram.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/spectral/swipe.py` & `PyTimbre-0.6.9/src/pytimbre/spectral/swipe.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/spectral/time_histories.py` & `PyTimbre-0.6.9/src/pytimbre/spectral/time_histories.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,23 +47,26 @@
         self._spectra = None
         self._times = None
         self._waveform = a
         self._integration_time = integration_time
         self._header = None
 
         #   Now if the Waveform object possesses a header field then we need to assign it to the header object here
-        if isinstance(self.waveform, StandardBinaryFile):
-            self._header = self.waveform.header
-        elif isinstance(self.waveform, WaveFile):
-            if self.waveform.header is not None:
+        if self._waveform is not None:
+            if isinstance(self.waveform, StandardBinaryFile):
                 self._header = self.waveform.header
-        elif isinstance(self.header, dict):
-            self._header = self.header
-            if 'HEADER SIZE' in self._header.keys():
-                del self._header['HEADER SIZE']
+            elif isinstance(self.waveform, WaveFile):
+                if self.waveform.header is not None:
+                    self._header = self.waveform.header
+            elif isinstance(self.header, dict):
+                self._header = self.header
+                if 'HEADER SIZE' in self._header.keys():
+                    del self._header['HEADER SIZE']
+            else:
+                header_dict = None
         else:
             header_dict = None
 
     @abc.abstractmethod
     def _calculate_spectrogram(self):
         warnings.warn("This function must be implemented in any child class to create the collection of spectra objects"
                       " that define the time history")
@@ -411,15 +414,15 @@
         if self._times is None:
             if self.spectra[0].time_past_midnight is not None:
                 t = np.zeros((len(self._spectra),), dtype=datetime.datetime)
             else:
                 t = np.zeros((len(self._spectra),))
 
             for i in range(len(self.spectra)):
-                if self.spectra[i].waveform is not None:
+                if self.spectra[i]._waveform is not None:
                     t[i] = self.spectra[i].time
                 else:
                     t[i] = self.spectra[i].time_past_midnight
 
             self._times = t
 
         return self._times
```

### Comparing `PyTimbre-0.6.8/src/pytimbre/waveform.py` & `PyTimbre-0.6.9/src/pytimbre/waveform.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.8/src/pytimbre/yin.py` & `PyTimbre-0.6.9/src/pytimbre/yin.py`

 * *Files identical despite different names*

