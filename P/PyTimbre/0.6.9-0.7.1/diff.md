# Comparing `tmp/PyTimbre-0.6.9.tar.gz` & `tmp/PyTimbre-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTimbre-0.6.9.tar", last modified: Tue Apr 25 22:56:06 2023, max compression
+gzip compressed data, was "PyTimbre-0.7.1.tar", last modified: Mon Jun 26 00:46:08 2023, max compression
```

## Comparing `PyTimbre-0.6.9.tar` & `PyTimbre-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 22:56:06.042948 PyTimbre-0.6.9/
--rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.6.9/LICENSE.txt
--rw-rw-rw-   0        0        0    13388 2023-04-25 22:56:06.041929 PyTimbre-0.6.9/PKG-INFO
--rw-rw-rw-   0        0        0     5339 2023-04-25 22:51:37.000000 PyTimbre-0.6.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-25 22:56:06.043960 PyTimbre-0.6.9/setup.cfg
--rw-rw-rw-   0        0        0     1072 2023-04-25 22:52:22.000000 PyTimbre-0.6.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:56:05.913020 PyTimbre-0.6.9/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 22:56:05.950152 PyTimbre-0.6.9/src/PyTimbre.egg-info/
--rw-rw-rw-   0        0        0    13388 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      775 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 22:56:05.000000 PyTimbre-0.6.9/src/PyTimbre.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-25 22:56:05.968586 PyTimbre-0.6.9/src/pytimbre/
--rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.6.9/src/pytimbre/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:56:05.996687 PyTimbre-0.6.9/src/pytimbre/audio_files/
--rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.6.9/src/pytimbre/audio_files/__init__.py
--rw-rw-rw-   0        0        0    23794 2023-04-14 21:21:46.000000 PyTimbre-0.6.9/src/pytimbre/audio_files/ansi_standard_formatted_files.py
--rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.6.9/src/pytimbre/audio_files/calibrated_binary_files.py
--rw-rw-rw-   0        0        0    69970 2023-04-25 22:21:07.000000 PyTimbre-0.6.9/src/pytimbre/audio_files/wavefile.py
-drwxrwxrwx   0        0        0        0 2023-04-25 22:56:06.039895 PyTimbre-0.6.9/src/pytimbre/spectral/
--rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.6.9/src/pytimbre/spectral/__init__.py
--rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.6.9/src/pytimbre/spectral/acoustic_weights.py
--rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.6.9/src/pytimbre/spectral/fractional_octave_band.py
--rw-rw-rw-   0        0        0    16910 2023-04-15 02:25:52.000000 PyTimbre-0.6.9/src/pytimbre/spectral/fundamental_frequency.py
--rw-rw-rw-   0        0        0    58636 2023-04-21 14:52:01.000000 PyTimbre-0.6.9/src/pytimbre/spectral/spectra.py
--rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.6.9/src/pytimbre/spectral/spectrogram.py
--rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.6.9/src/pytimbre/spectral/swipe.py
--rw-rw-rw-   0        0        0    32410 2023-04-25 22:23:53.000000 PyTimbre-0.6.9/src/pytimbre/spectral/time_histories.py
--rw-rw-rw-   0        0        0    85520 2023-04-24 21:54:08.000000 PyTimbre-0.6.9/src/pytimbre/waveform.py
--rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.6.9/src/pytimbre/yin.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:46:08.816487 PyTimbre-0.7.1/
+-rw-rw-rw-   0        0        0     1106 2023-02-28 16:15:07.000000 PyTimbre-0.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    14433 2023-06-26 00:46:08.816487 PyTimbre-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5339 2023-04-25 22:51:37.000000 PyTimbre-0.7.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-26 00:46:08.816487 PyTimbre-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1071 2023-06-26 00:45:06.000000 PyTimbre-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:46:08.773683 PyTimbre-0.7.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-26 00:46:08.807021 PyTimbre-0.7.1/src/PyTimbre.egg-info/
+-rw-rw-rw-   0        0        0    14433 2023-06-26 00:46:08.000000 PyTimbre-0.7.1/src/PyTimbre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      775 2023-06-26 00:46:08.000000 PyTimbre-0.7.1/src/PyTimbre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 00:46:08.000000 PyTimbre-0.7.1/src/PyTimbre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-06-26 00:46:08.000000 PyTimbre-0.7.1/src/PyTimbre.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-26 00:46:08.000000 PyTimbre-0.7.1/src/PyTimbre.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 00:46:08.809034 PyTimbre-0.7.1/src/pytimbre/
+-rw-rw-rw-   0        0        0       75 2023-04-13 00:23:16.000000 PyTimbre-0.7.1/src/pytimbre/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:46:08.811273 PyTimbre-0.7.1/src/pytimbre/audio_files/
+-rw-rw-rw-   0        0        0      108 2023-04-04 13:59:30.000000 PyTimbre-0.7.1/src/pytimbre/audio_files/__init__.py
+-rw-rw-rw-   0        0        0    24251 2023-06-26 00:38:01.000000 PyTimbre-0.7.1/src/pytimbre/audio_files/ansi_standard_formatted_files.py
+-rw-rw-rw-   0        0        0    15392 2023-04-14 23:28:06.000000 PyTimbre-0.7.1/src/pytimbre/audio_files/calibrated_binary_files.py
+-rw-rw-rw-   0        0        0    70823 2023-06-26 00:36:51.000000 PyTimbre-0.7.1/src/pytimbre/audio_files/wavefile.py
+drwxrwxrwx   0        0        0        0 2023-06-26 00:46:08.815473 PyTimbre-0.7.1/src/pytimbre/spectral/
+-rw-rw-rw-   0        0        0      150 2023-03-03 22:01:28.000000 PyTimbre-0.7.1/src/pytimbre/spectral/__init__.py
+-rw-rw-rw-   0        0        0    15326 2023-04-13 01:01:21.000000 PyTimbre-0.7.1/src/pytimbre/spectral/acoustic_weights.py
+-rw-rw-rw-   0        0        0    15705 2023-04-13 21:59:41.000000 PyTimbre-0.7.1/src/pytimbre/spectral/fractional_octave_band.py
+-rw-rw-rw-   0        0        0    16910 2023-04-15 02:25:52.000000 PyTimbre-0.7.1/src/pytimbre/spectral/fundamental_frequency.py
+-rw-rw-rw-   0        0        0    59502 2023-05-31 18:17:14.000000 PyTimbre-0.7.1/src/pytimbre/spectral/spectra.py
+-rw-rw-rw-   0        0        0     6656 2023-04-13 01:01:21.000000 PyTimbre-0.7.1/src/pytimbre/spectral/spectrogram.py
+-rw-rw-rw-   0        0        0    13865 2023-04-13 17:16:30.000000 PyTimbre-0.7.1/src/pytimbre/spectral/swipe.py
+-rw-rw-rw-   0        0        0    32990 2023-05-31 18:33:10.000000 PyTimbre-0.7.1/src/pytimbre/spectral/time_histories.py
+-rw-rw-rw-   0        0        0   100362 2023-06-26 00:38:01.000000 PyTimbre-0.7.1/src/pytimbre/waveform.py
+-rw-rw-rw-   0        0        0     7703 2023-04-13 01:31:15.000000 PyTimbre-0.7.1/src/pytimbre/yin.py
```

### Comparing `PyTimbre-0.6.9/LICENSE.txt` & `PyTimbre-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/PKG-INFO` & `PyTimbre-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.9
+Version: 0.7.1
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
@@ -198,14 +198,29 @@
 - Version 0.6.3 integrated the libf0 library. After attempting to integrate this library directly, it was determined that using the raw code would be a better implementation for this package.
 - The swipe.py file was taken from version 1.0.2 on 1 April 2023 to provide the fundamental frequency
 - __Version 0.6.7__
 - Updates to the calculation of the fundamental frequency
 - Updates to the calculation of the harmonic features
 - Updates to methods to get the features from the spectrum and time history objects
 
+#### May
+- Added a flag in the constructor of the waveform to remove the finding the maximum of the waveform
+- Created the initial version of the Sphinx documentation for the module.
+- Integrated code for the reading of impulse waveforms into the Waveform class.
+- Integrated code the correct calculation of spectral levels from an impulse waveform into SpectrumByFFT
+- Updated the __get_features__ function to return different data in the DataFrame when the waveform is labeled as an impulse waveform.
+
+#### June
+- Updated trim method to copy properties that could have been altered from the defaults in the constructor
+- Reduced requirements for standard packages
+- Worked on temporal features for EEG data that possesses significantly lower sample rates than audio data
+- Added a property to set the method for the thresholding required in the attack determination
+- Updated the tests so that they will execute with python setup.py test
+- Incremented to 0.7.1 with the completion of all issues slated for the 0.7.1 increment.
+
 
 MIT License
 
 Copyright (c) 2021 Frank Mobley, Gregory Bowers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `PyTimbre-0.6.9/README.md` & `PyTimbre-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/setup.py` & `PyTimbre-0.7.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,28 +7,28 @@
         HISTORY = history_file.read()
 
         with open('LICENSE.txt') as license_file:
             LICENSE = license_file.read()
 
 setup(
     name='PyTimbre',
-    version='0.6.9',
+    version='0.7.1',
     description='Python conversion of Timbre Toolbox',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY + '\n\n' + LICENSE,
     license='MIT',
     packages=find_packages('src'),
     author='Dr. Frank Mobley',
     author_email='frank.mobley.1@afrl.af.mil',
     keywords=['machine learning', 'feature extraction', 'MATLAB', 'audio'],
     url='https://gitlab.com/python-audio-feature-extraction/pytimbre',
     download_url='',
     install_requires=[
-        'numpy>=1.23.5',
-        'pandas>=1.5.3',
-        'scipy>=1.10.1',
+        'numpy>=1.21.5',
+        'pandas>=1.4.3',
+        'scipy>=1.9.1',
         'statsmodels>=0.13.2',
         'mosqito>=1.0.8',
         'colorednoise>=2.1.0'
     ],
     package_dir={'': 'src'}
 )
```

### Comparing `PyTimbre-0.6.9/src/PyTimbre.egg-info/PKG-INFO` & `PyTimbre-0.7.1/src/PyTimbre.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTimbre
-Version: 0.6.9
+Version: 0.7.1
 Summary: Python conversion of Timbre Toolbox
 Home-page: https://gitlab.com/python-audio-feature-extraction/pytimbre
 Download-URL: 
 Author: Dr. Frank Mobley
 Author-email: frank.mobley.1@afrl.af.mil
 License: MIT
 Keywords: machine learning,feature extraction,MATLAB,audio
@@ -198,14 +198,29 @@
 - Version 0.6.3 integrated the libf0 library. After attempting to integrate this library directly, it was determined that using the raw code would be a better implementation for this package.
 - The swipe.py file was taken from version 1.0.2 on 1 April 2023 to provide the fundamental frequency
 - __Version 0.6.7__
 - Updates to the calculation of the fundamental frequency
 - Updates to the calculation of the harmonic features
 - Updates to methods to get the features from the spectrum and time history objects
 
+#### May
+- Added a flag in the constructor of the waveform to remove the finding the maximum of the waveform
+- Created the initial version of the Sphinx documentation for the module.
+- Integrated code for the reading of impulse waveforms into the Waveform class.
+- Integrated code the correct calculation of spectral levels from an impulse waveform into SpectrumByFFT
+- Updated the __get_features__ function to return different data in the DataFrame when the waveform is labeled as an impulse waveform.
+
+#### June
+- Updated trim method to copy properties that could have been altered from the defaults in the constructor
+- Reduced requirements for standard packages
+- Worked on temporal features for EEG data that possesses significantly lower sample rates than audio data
+- Added a property to set the method for the thresholding required in the attack determination
+- Updated the tests so that they will execute with python setup.py test
+- Incremented to 0.7.1 with the completion of all issues slated for the 0.7.1 increment.
+
 
 MIT License
 
 Copyright (c) 2021 Frank Mobley, Gregory Bowers
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
```

### Comparing `PyTimbre-0.6.9/src/PyTimbre.egg-info/SOURCES.txt` & `PyTimbre-0.7.1/src/PyTimbre.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/src/pytimbre/audio_files/ansi_standard_formatted_files.py` & `PyTimbre-0.7.1/src/pytimbre/audio_files/ansi_standard_formatted_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,14 +65,17 @@
         """
 
         self._header = None
 
         if filename is not None:
             self._read_file(filename, header_element_count, sample_rate_key, start_time_key, sample_format_key,
                             data_format_key, sample_count_key, header_only, s0, s1)
+            if header_only == False:
+                super().__init__(self.samples, self.sample_rate, self.start_time)
+
         elif wfm is not None:
             super().__init__(wfm.samples, wfm.sample_rate, wfm.start_time)
             self._header = None
         else:
             self._samples = None
             self.fs = None
             self.time0 = None
@@ -82,18 +85,20 @@
         if key not in self.header.keys():
             raise ValueError("The name of the sample rate element of the waveform is not located within the "
                              "header dictionary. Please provide the correct name of the sample rate property")
         else:
             self.fs = float(self.header[key])
 
     def _read_start_time(self, key):
-        if key not in self.header.keys():
+        if key not in self.header.keys() and "TIME (TPM)" not in self.header.keys():
             raise ValueError(
                 "The name of the start time element of the waveform is not located within the "
                 "header dictionary. Please provide the correct name of the start time property")
+        elif "TIME (TPM)" in self.header.keys():
+            self.time0 = float(self.header['TIME (TPM)'])
         else:
             self.time0 = parser.parse(self.header[key])
 
     def _read_sample_count(self, key):
         if key not in self.header.keys():
             raise ValueError("The number of samples must be provided, and the expected header element is not "
                              "found within the list of objects in the header.")
@@ -137,15 +142,15 @@
 
         return samples_to_read
 
     def _read_file(self, filename, header_element_count: int = None,
                    sample_rate_key: str = 'SAMPLE RATE (HZ)', start_time_key: str = 'TIME (UTC ZULU)',
                    sample_format_key: str = 'SAMPLE FORMAT', data_format_key: str = 'DATA FORMAT',
                    sample_count_key: str = 'SAMPLES TOTAL', header_only: bool = False, s0=None, s1=None):
-        #   Get the header and the location of the binary data
+    #   Get the header and the location of the binary data
         f_in, header = StandardBinaryFile.read_header(filename, header_element_count)
         self._header = header
 
         if header_only:
             self._samples = None
             return
 
@@ -178,15 +183,16 @@
         #   Now we need to determine how many sample to read
         samples_to_read = self._define_samples_to_read(s0, s1)
 
         #   Read the data - At this point we only support 32-bit/4-byte data samples
         data = f_in.read(4 * samples_to_read)
 
         #   Now unpack the data from the array of bytes into an array of floating point data
-        self._samples = np.asarray(struct.unpack('f' * samples_to_read, data))
+        samples = np.asarray(struct.unpack('f' * samples_to_read, data))
+        super().__init__(samples, self.sample_rate, self.start_time)
 
         if samples_to_read < self.sample_count:
             self.sample_count = samples_to_read
             self._samples -= np.mean(self.samples)
 
         #   close the file
         f_in.close()
@@ -299,15 +305,19 @@
 
         header = orig_header.copy()
 
         # Append sample format and encoding method if they don't exist to the header dict
 
         header['SAMPLE RATE (HZ)'] = int(np.floor(wfm.sample_rate))
         header['SAMPLES TOTAL'] = len(wfm.samples)
-        header['TIME (UTC ZULU)'] = wfm.start_time.strftime('%Y/%m/%d %H:%M:%S.%f')
+        if isinstance(wfm.start_time, datetime):
+            header['TIME (UTC ZULU)'] = wfm.start_time.strftime('%Y/%m/%d %H:%M:%S.%f')
+        else:
+            header['TIME (TPM)'] = wfm.start_time
+
         header['SAMPLE FORMAT'] = "LITTLE ENDIAN"
         header['DATA FORMAT'] = 'REAL*4'
 
         # Check to see if output path exist and open file if it doesn't exist
 
         if not os.path.exists(output_filename):
             f = open(output_filename, 'wb')
```

### Comparing `PyTimbre-0.6.9/src/pytimbre/audio_files/calibrated_binary_files.py` & `PyTimbre-0.7.1/src/pytimbre/audio_files/calibrated_binary_files.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/src/pytimbre/audio_files/wavefile.py` & `PyTimbre-0.7.1/src/pytimbre/audio_files/wavefile.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,14 +292,25 @@
         elif self.chunk_size == 40:
             self.audio_format = struct.unpack('<H', reader.read(2))[0]
             self.num_channels = struct.unpack('<H', reader.read(2))[0]
             self.fs = struct.unpack('<I', reader.read(4))[0]
             self.byte_rate = struct.unpack('<I', reader.read(4))[0]
             self.block_align = struct.unpack('<H', reader.read(2))[0]
             self.bits_per_sample = struct.unpack('<H', reader.read(2))[0]
+        else:
+            try:
+                self.audio_format = struct.unpack('<H', reader.read(2))[0]
+                self.num_channels = struct.unpack('<H', reader.read(2))[0]
+                self.fs = struct.unpack('<I', reader.read(4))[0]
+                self.byte_rate = struct.unpack('<I', reader.read(4))[0]
+                self.block_align = struct.unpack('<H', reader.read(2))[0]
+                self.bits_per_sample = struct.unpack('<H', reader.read(2))[0]
+            except Exception as e:
+                raise e
+
 
     @property
     def waveform_format(self):
         if self.audio_format == 1:
             return "PCM - Uncompressed"
         elif self.audio_format == 3:
             return "IEEE Floating Point"
@@ -1240,25 +1251,26 @@
                            'duration': duration,
                            'has_peak_chunk': scanner.peak_chunk is not None,
                            'has_list_chunk': scanner.list_chunk is not None,
                            'has_xml_chunk': scanner.xml_chunk is not None}
 
         return information
 
-    def __init__(self, path=None, s0: int = None, s1: int = None, fs: int = None, samples=None, time=None):
+    def __init__(self, path=None, s0: int = None, s1: int = None, fs: int = None, samples=None, time=None, get_peak:bool = True):
         """
         This constructor reads the chunks from the wave file and then processes those that are canonical.
 
         :param path: str - the full path to the file that we want to read
         :param s0: int - the starting sample for the reading of the audio file
         :param s1: int - the ending sample for the reading of the audio file
         :param fs: int - the number of samples per second.  This facilitates calling the based class with the required
             data
         :param samples: ndarray - the actual samples to define the waveform
         :param time: float or datetime - the time of the first sample
+        :param get_peak: bool - whether or not the constructor should get the peak value (and create the peak chunk). Getting this value doubles memory usage.
         """
 
         # warnings.warn('Test for Insert Start Time using wfm.start_time=...is failing.')
         # TODO - Correct the wfm.start_time setting feature.
 
         if path is None:
             if(fs is None) and (samples is None) and (time is None):
@@ -1375,15 +1387,15 @@
                                         s0,
                                         s1,
                                         self.normalized)
 
             #   If the peak chunk was not read from the file, we need to create one from the data that was read from
             #   the wav file.
 
-            if self.peak_chunk is None:
+            if self.peak_chunk is None and get_peak:
                 self.peak_chunk = PeakChunk()
                 self.peak_chunk.peak_amplitude = np.max(self.data_chunk.waveform, axis=0)
                 self.peak_chunk.peak_sample = np.argmax(self.data_chunk.waveform, axis=0)
 
         #   Create the data and build the information for the generic_time_waveform
 
         super().__init__(self.data_chunk.waveform, self.format_chunk.sample_rate, time0)
@@ -1784,33 +1796,33 @@
 
             file.write("data".encode('utf-8'))
             file.write(struct.pack("<i", 4 * len(self.samples) * self.channel_count))
 
             #   Now we will loop through the data elements and write the information, scaled to 1.0f full scale based
             #   on the data within the PEAK chunk
 
-            peak_value = np.max(self.samples)
-
             if self.normalized:
                 if self.format_chunk.channel_count > 1:
                     for i in range(self.samples.shape[1]):
                         self.samples[:, i] /= np.max(self.samples[:, i])
                 else:
                     self.samples[:] /= np.max(self.samples[:])
 
             samples_to_write = np.reshape(self.samples, (np.product(self.samples.shape),))
             file.write(samples_to_write.astype("<f").tobytes())
 
             #   Write the LIST chunk
 
             # if self.list_chunk is not None: # There will always be a list chunk
-            if self.creation_date is not None and self.creation_date > self.start_time:
+            if self.creation_date is not None:
                 self.list_chunk.time0 = self.creation_date
             else:
-                self.list_chunk.time0 = self.start_time
+                #   To ensure that the wave file can be saved without saving the start time as a start time
+                if self.start_time is not None and not isinstance(self.start_time, datetime):
+                    self.list_chunk.time0 = datetime.now()
             self.list_chunk.write_chunk(file)
 
             #   Get the current number of bytes within the file
 
             file_size = file.tell()
 
             #   Search for the file size - 8 within the header and update the information
```

### Comparing `PyTimbre-0.6.9/src/pytimbre/spectral/acoustic_weights.py` & `PyTimbre-0.7.1/src/pytimbre/spectral/acoustic_weights.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/src/pytimbre/spectral/fractional_octave_band.py` & `PyTimbre-0.7.1/src/pytimbre/spectral/fractional_octave_band.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/src/pytimbre/spectral/fundamental_frequency.py` & `PyTimbre-0.7.1/src/pytimbre/spectral/fundamental_frequency.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/src/pytimbre/spectral/spectra.py` & `PyTimbre-0.7.1/src/pytimbre/spectral/spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,19 +87,23 @@
         self._inharmonicity = None
 
     #   ------------------------------------------ Protected functions -------------------------------------------------
 
     def _calculate_spectrum(self):
         import warnings
 
-        warnings.warn("This function does nothing. You will need to implement this function in the child class to build"
-                      "the spectrum with the correct units and format.")
+        warnings.warn(
+            "This function does nothing. You will need to implement this function in the child class to build"
+            "the spectrum with the correct units and format."
+            )
 
-        raise ValueError('This method must be implemented and assigned frequencies within the calculation '
-                         'of each type of spectrum class.')
+        raise ValueError(
+            'This method must be implemented and assigned frequencies within the calculation '
+            'of each type of spectrum class.'
+            )
 
     #   ------------------------------------- Class properties ---------------------------------------------------------
 
     @property
     def waveform(self):
         if self._waveform is None:
             warnings.warn('No Waveform object has been passed to this Spectrum object.')
@@ -433,16 +437,20 @@
         tonal signals, the spectral flatness is close to 0( a peaky spectrum), whereas for noisy signals it is close to
         1 (flat spectrum).
         """
         if self._acoustic_pressures_pascals is None and self._frequencies is None:
             self._calculate_spectrum()
 
         if self.flatness is None:
-            self.geometric_mean = np.exp((1 / len(self._frequencies)) * np.sum(np.log(self._acoustic_pressures_pascals),
-                                                                               axis=0))
+            self.geometric_mean = np.exp(
+                (1 / len(self._frequencies)) * np.sum(
+                    np.log(self._acoustic_pressures_pascals),
+                    axis=0
+                    )
+                )
             self.arithmetic_mean = np.mean(self._acoustic_pressures_pascals, axis=0)
             self.flatness = self.geometric_mean / self.arithmetic_mean
 
         return self.flatness
 
     @property
     def spectral_crest(self):
@@ -641,16 +649,18 @@
                 self._inharmonicity = np.nan
             else:
                 frequency_departure = 0
                 for i in range(1, len(self.partial_frequencies_indices)):
                     frequency_departure += (self.frequencies[self.partial_frequencies_indices[i]] - (i + 1) * f0) * \
                                            self.pressures_pascals[self.partial_frequencies_indices[i]]
 
-                self._inharmonicity = (2 / f0) * frequency_departure / np.sum(self.pressures_pascals[
-                                                                                  self.partial_frequencies_indices] ** 2)
+                self._inharmonicity = (2 / f0) * frequency_departure / np.sum(
+                    self.pressures_pascals[
+                        self.partial_frequencies_indices] ** 2
+                    )
 
         return self._inharmonicity
 
     @property
     def fundamental_frequency(self):
         if self._fundamental_frequency is None:
             self._calculate_fundamental_frequency()
@@ -695,16 +705,18 @@
         sens = calibration_level - calibration_values
         sens /= 20
         sens *= -1
         sens = 10.0 ** sens
 
         return sens
 
-    def get_average_features(self, include_sq_metrics: bool = True, include_temporal_features: bool = True,
-                             include_spectral_features: bool = True, include_harmonic_features: bool = True):
+    def get_average_features(
+            self, include_sq_metrics: bool = True, include_temporal_features: bool = True,
+            include_spectral_features: bool = True, include_harmonic_features: bool = True
+            ):
         """
         This will return a dict of the various elements within the spectrum and waveform (if it was used to create the
         spectrogram object) with any time variant elements averaged.
         """
 
         #   Create the dictionary that will hold the data
         features = dict()
@@ -749,20 +761,24 @@
             features['tri_stimulus_03'] = self.tri_stimulus[2]
             features['harmonic_spectral_deviation'] = self.harmonic_spectral_deviation
             features['odd_even_ratio'] = self.odd_even_ratio
             features['inharmonicity'] = self.inharmonicity
 
         return features
 
-    def get_feature_names(self, include_sq_metrics: bool = True, include_temporal_features: bool = True,
-                          include_spectral_features: bool = True, include_harmonic_features: bool = True):
-        return self.get_average_features(include_sq_metrics=include_sq_metrics,
-                                         include_harmonic_features=include_harmonic_features,
-                                         include_spectral_features=include_spectral_features,
-                                         include_temporal_features=include_temporal_features).keys()
+    def get_feature_names(
+            self, include_sq_metrics: bool = True, include_temporal_features: bool = True,
+            include_spectral_features: bool = True, include_harmonic_features: bool = True
+            ):
+        return self.get_average_features(
+            include_sq_metrics=include_sq_metrics,
+            include_harmonic_features=include_harmonic_features,
+            include_spectral_features=include_spectral_features,
+            include_temporal_features=include_temporal_features
+            ).keys()
 
     def _calculate_normalized_distribution(self):
         if self._acoustic_pressures_pascals is None:
             self._calculate_spectrum()
 
         self.probability_distribution = self._acoustic_pressures_pascals
         self.probability_distribution /= np.sum(self._acoustic_pressures_pascals, axis=0)
@@ -784,17 +800,14 @@
     def _calculate_fundamental_frequency(self):
         from .fundamental_frequency import FundamentalFrequencyCalculator
 
         calculator = FundamentalFrequencyCalculator(frequency_window_size=self._fft_size)
 
         f0 = list()
         f0.append(calculator.fundamental_swipe(self))
-        # f0.append(calculator.fundamental_by_peaks(self))
-        # if self._waveform is not None:
-        #     f0.append(calculator.fundamental_by_time(self.waveform))
 
         #   Convert the list to an array and remove any Nan values
         f0 = np.asarray(f0)
         f0 = f0[np.logical_not(np.isnan(f0))]
 
         if len(f0) < 1:
             self._fundamental_frequency = np.nan
@@ -816,48 +829,34 @@
         self.partial_frequencies_indices = np.zeros((max_partial_frequencies,), dtype=int)
 
         for i in range(0, max_partial_frequencies):
             self.partial_frequencies_indices[i] = np.where(f_ratio >= i + 1)[0][0]
 
     def _calculate_harmonic_features(self):
         from ..yin import yin
-        # self.stft = STFT.STFT(sound, self.config)
-        # self.t_support = self.stft.t_support
-        # maxSwipepWinSize = self.stft.hop_size * np.ceil(
-        #     2 ** (round(np.log2(8 * self.sound.reps['AudioSignal'].sampleRate / 50)) - 1) / self.stft.hop_size)
-        # freqCorrs = np.linspace(-5, 5, 101)
-        # nFreqCorrs = len(freqCorrs)
-        # inharmCoeffs = np.linspace(0, 0.001, 21)
-        # nInharmCoeffs = 21
-        # tSupport = np.subtract(self.t_support, self.t_support[0])
-        # tSize = len(tSupport)
-        # distr = self.stft.value
-        # signalChunk = a.value
-        # pitchLims = np.array([50, 500])
-        # estimated_pitches, estimated_times, estStrengths = self.swipep(signalChunk, self.sound.reps['AudioSignal'].sampleRate,
-        #                                                  pitchLims, (self.stft.hop_size / self.sound.reps[
-        #         'AudioSignal'].sampleRate), 1 / 48, 0.1, 0.2, -np.inf)
 
         estimated_pitches, estimated_times, estimated_pitch_strengths = yin(
             self.waveform.samples,
             self.waveform.sample_rate,
             F_max=10000,
             F_min=10,
             N=int(np.floor(self.sample_rate / 10)),
-            H=int(np.floor(self.sample_rate / 10 / 4)))
+            H=int(np.floor(self.sample_rate / 10 / 4))
+        )
 
         try:
             current_maximum = np.nanmax(estimated_pitch_strengths)
         except ValueError:
             current_maximum = np.max(estimated_pitch_strengths)
         nans = np.isnan(estimated_pitches)
         anyy = any(nans)
         if anyy:
             estimated_pitches[np.isnan(estimated_pitches)] = np.median(
-                estimated_pitches[not np.isnan(estimated_pitches)])
+                estimated_pitches[not np.isnan(estimated_pitches)]
+            )
         fundamental_frequencies = None
         if current_maximum > self.pitch_threshold:
             estimated_time_pitch_pairs = np.zeros((len(estimated_times), 2))
             estimated_time_pitch_pairs[:, 0] = estimated_times
             estimated_time_pitch_pairs[:, 1] = estimated_pitches
             fundamental_frequencies = Harmonic.Fevalbp(estimated_time_pitch_pairs, tSupport)
             fundamental_frequencies = np.transpose(fundamental_frequencies)
@@ -882,16 +881,18 @@
         b1 = b[:, None]
         b2 = inharmCoeffs[None, :]
         c = np.matmul(b1, b2)
         d = np.add(1, c)
         inharmFactorsHI = np.multiply(a, np.sqrt(d))
         shape1 = np.reshape(corrFreqsTF, (tSize * nFreqCorrs, 1), order='F')
         shape2 = np.reshape(inharmFactorsHI, (1, self.config['n_harms'] * nInharmCoeffs), order='F')
-        shape3 = np.reshape(np.multiply(shape1, shape2), (tSize, nFreqCorrs, self.config['n_harms'], nInharmCoeffs),
-                            order='F')
+        shape3 = np.reshape(
+            np.multiply(shape1, shape2), (tSize, nFreqCorrs, self.config['n_harms'], nInharmCoeffs),
+            order='F'
+            )
         shape4 = np.divide(1, self.stft.bin_size)
         shape5 = np.multiply(shape4, shape3)
         shape6 = np.round(shape5)
         fSupIdcsTFHI = np.add(1, shape6)
         fSupIdcsTFHI[fSupIdcsTFHI > self.stft.f_size] = self.stft.f_size
 
         a = np.array([*range(0, tSize)])
@@ -924,15 +925,16 @@
         colIdcs = np.reshape(np.add(repmat1, repmat2), (tSize * nFreqCorrs, 1), order='F')
         totalErgTFI_flat = totalErgTFI.flatten('F')
         totalErgTF = np.take(totalErgTFI_flat, np.subtract(colIdcs, 1))
         totalErgTF = np.reshape(totalErgTF, (tSize, nFreqCorrs), order='F')
 
         reshape1 = np.reshape(
             np.add([*range(1, tSize + 1)], np.multiply(tSize * nFreqCorrs * self.config['n_harms'], inharmCoeffIdcsT)),
-            (tSize, 1, 1), order='F')
+            (tSize, 1, 1), order='F'
+        )
         repmat1 = np.tile(reshape1, (1, nFreqCorrs, self.config['n_harms']))
         reshape2 = np.reshape([*range(1, nFreqCorrs + 1)], (1, nFreqCorrs, 1), order='F')
         repmat2 = np.tile(reshape2, (tSize, 1, self.config['n_harms']))
         reshape3 = np.reshape([*range(1, self.config['n_harms'] + 1)], (1, 1, self.config['n_harms']), order='F')
         repmat3 = np.tile(reshape3, (tSize, nFreqCorrs, 1))
 
         a = np.subtract(repmat3, 1)
@@ -991,15 +993,18 @@
         that originate with the Fourier transform methodologies.
         """
         #   Call the base constructor to define the waveform within the class
         super().__init__(a)
 
         #   Now define some information within the class related to the frequencies and the information generated
         #   specifically for the FFT methods
-        self._fft_size = fft_size
+        if a is not None and a.is_impulsive:
+            self._fft_size = len(a.samples)
+        else:
+            self._fft_size = fft_size
         self._frequencies_double_sided = None
         self._frequencies_nb = None
 
         #   Define some other representations of the acoustic information that might be needed in various
         #   analyses.
         self._pressures_double_sided_complex = None
 
@@ -1018,43 +1023,74 @@
         """
         This function generates the complex spectra using an FFT of multiple blocks of an input waveform,
         where the blocks have 50% overlap and are each weighted by a Hanning window.
 
         The FFT blocks are then scaled to contain the appropriate amount of energy for input into a power
         spectrum calculation.
         """
-
-        #   Create the frequency arrays
-        self._frequencies_double_sided = self.sample_rate * np.arange(0, self._fft_size) / self._fft_size
-        self._frequencies_nb = self._frequencies_double_sided[:int(self._fft_size / 2)]
-        df = self._frequencies_nb[1] - self._frequencies_nb[0]
-
-        #   enforce a zero mean value
-        x = self.waveform.samples - np.mean(self.waveform.samples)
-
-        #   Generate a Hanning window
-        ww = np.hanning(self._fft_size)
-        W = np.mean(ww ** 2)
-
-        #   Divide the total data into blocks with 50% overlap and Hanning window
-        blocks = np.zeros(shape=(int(np.floor(2 * len(x) / self._fft_size - 1)), self._fft_size))
-
-        for k in range(blocks.shape[0]):
-            i = int(k * self._fft_size / 2)
-            j = i + blocks.shape[1]
-            blocks[k, :] = ww * x[i:j]
-
-        #   Determine complex pressure amplitude
-        self._pressures_double_sided_complex = np.sqrt(2 * df / self._fft_size /
-                                                       self.sample_rate / W) * scipy.fft.fft(blocks, n=self._fft_size)
-
-        #   Now assign the values for the acoustic pressures using this information, but only using the first hold of
-        #   the frequency data.
-        self._frequencies = self._frequencies_nb
-        self._acoustic_pressures_pascals = self.auto_correlation_spectrum
+        if self.waveform is not None and self.waveform.is_continuous:
+            #   Create the frequency arrays
+            self._frequencies_double_sided = self.sample_rate * np.arange(0, self._fft_size) / self._fft_size
+            self._frequencies_nb = self._frequencies_double_sided[:int(self._fft_size / 2)]
+            df = self._frequencies_nb[1] - self._frequencies_nb[0]
+
+            #   enforce a zero mean value
+            x = self.waveform.samples - np.mean(self.waveform.samples)
+
+            #   Generate a Hanning window
+            ww = np.hanning(self._fft_size)
+            W = np.mean(ww ** 2)
+
+            #   Divide the total data into blocks with 50% overlap and Hanning window
+            blocks = np.zeros(shape=(int(np.floor(2 * len(x) / self._fft_size - 1)), self._fft_size))
+
+            for k in range(blocks.shape[0]):
+                i = int(k * self._fft_size / 2)
+                j = i + blocks.shape[1]
+                blocks[k, :] = ww * x[i:j]
+
+            #   Determine complex pressure amplitude
+            self._pressures_double_sided_complex = np.sqrt(2 * df / self._fft_size / self.sample_rate / W) * \
+                                                   scipy.fft.fft(blocks, n=self._fft_size)
+
+            #   Now assign the values for the acoustic pressures using this information, but only using the first hold
+            #   of the frequency data.
+            self._frequencies = self._frequencies_nb
+            self._acoustic_pressures_pascals = self.auto_correlation_spectrum
+        elif self.waveform is not None and self.waveform.is_impulsive:
+            #   Create the frequency arrays
+            self._frequencies_double_sided = self.sample_rate * np.arange(0, self._fft_size) / self._fft_size
+            self._frequencies_nb = self._frequencies_double_sided[:int(self._fft_size / 2)]
+            df = self._frequencies_nb[1] - self._frequencies_nb[0]
+
+            #   enforce a zero mean value
+            x = self.waveform.samples - np.mean(self.waveform.samples)
+
+            #   Generate a Tukey window
+            ww = scipy.signal.windows.tukey(self._fft_size, alpha=0.1)
+            W = np.mean(ww ** 2)
+
+            #   Divide the total data into blocks with 50% overlap and Hanning window
+            blocks = np.zeros(shape=(int(np.floor(2 * len(x) / self._fft_size - 1)), self._fft_size))
+
+            for k in range(blocks.shape[0]):
+                i = int(k * self._fft_size / 2)
+                j = i + blocks.shape[1]
+                blocks[k, :] = ww * x[i:j]
+
+            #   Determine complex pressure amplitude
+            self._pressures_double_sided_complex = np.sqrt(
+                2 * df / self._fft_size /
+                self.sample_rate / W
+                ) * scipy.fft.fft(blocks, n=self._fft_size)
+
+            #   Now assign the values for the acoustic pressures using this information, but only using the first hold of
+            #   the frequency data.
+            self._frequencies = self._frequencies_nb
+            self._acoustic_pressures_pascals = self.auto_correlation_spectrum
 
     @property
     def frequency_increment(self):
         return self.frequencies[1] - self.frequencies[0]
 
     @property
     def frequencies_double_sided(self):
@@ -1099,16 +1135,18 @@
     def power_spectral_density(self):
         """
         Numpy array of single-sided real-values. Pressures scaled by frequency, in units of Pascals / sqrt(Hz).
         """
         return self.pressures_pascals / np.sqrt(self.frequency_increment)
 
     @staticmethod
-    def convert_nb_to_fob(frequencies_nb, pressures_pascals_nb, fob_band_width: int = 3, f0: float = 10,
-                          f1: float = 10000):
+    def convert_nb_to_fob(
+            frequencies_nb, pressures_pascals_nb, fob_band_width: int = 3, f0: float = 10,
+            f1: float = 10000
+            ):
         """
         This function converts the frequency and pressure arrays sampled in narrowband resolution to the fractional
         octave band resolution.
 
         Parameters
         ----------
         frequencies_nb: nd_array - the collection of narrowband frequencies that we want to convert
@@ -1125,17 +1163,23 @@
 
         frequencies_fob = fob_tools.get_frequency_array(fob_band_width, f0, f1)
 
         #   Build the array of pressures that are the same size as the list of frequencies
         pressures_pascals_fob = np.zeros((len(frequencies_fob),))
 
         for i in range(len(frequencies_fob)):
-            pressures_pascals_fob[i] = np.sqrt(sum(pressures_pascals_nb ** 2 *
-                                                   fob_tools.filter_shape(fob_band_width, frequencies_fob[i],
-                                                                          frequencies_nb)))
+            pressures_pascals_fob[i] = np.sqrt(
+                sum(
+                    pressures_pascals_nb ** 2 *
+                    fob_tools.filter_shape(
+                        fob_band_width, frequencies_fob[i],
+                        frequencies_nb
+                        )
+                    )
+                )
 
         return frequencies_fob, pressures_pascals_fob
 
     def to_fractional_octave_band(self, bandwidth: int = 3, f0: float = 10, f1: float = 10000):
         """
         This function will convert the spectrum from a narrowband resolution to a factional octave band resolution by
         applying the shape functions to the narrowband spectral values and determining the weighted value within the
@@ -1271,58 +1315,84 @@
         frequency = list()
 
         #   Determine the octave bands that will need to be calculated to cover the desired frequency range.
         low_band = int(np.floor(fob_tools.nearest_band(1, self.start_fractional_octave_frequency)))
         hi_band = int(np.floor(fob_tools.nearest_band(1, self.stop_fractional_octave_frequency)))
 
         #   Get the index of the band at the top of the full octave filter
-        fob_band_index = int(np.floor(fob_tools.nearest_band(self.fractional_octave_bandwidth,
-                                                             fob_tools.upper_frequency(1, hi_band))))
+        fob_band_index = int(
+            np.floor(
+                fob_tools.nearest_band(
+                    self.fractional_octave_bandwidth,
+                    fob_tools.upper_frequency(1, hi_band)
+                    )
+                )
+            )
 
         #   Make a copy of the waveform that can be decimated
-        wfm = Waveform(pressures=self.waveform.samples.copy(),
-                       sample_rate=self.sample_rate,
-                       start_time=self.waveform.start_time)
+        wfm = Waveform(
+            pressures=self.waveform.samples.copy(),
+            sample_rate=self.sample_rate,
+            start_time=self.waveform.start_time
+            )
 
         #   Loop through the frequencies in reverse order
         for band_index in range(hi_band, low_band - 1, -1):
             #   if there are insufficient number of points in the waveform, terminate the process now
             if len(wfm.samples) < 3 * self._b_coefficients.shape[1]:
-                warnings.warn("The number of points within the Waveform are insufficient to calculate digital filters "
-                              "lower than these frequencies")
+                warnings.warn(
+                    "The number of points within the Waveform are insufficient to calculate digital filters "
+                    "lower than these frequencies"
+                    )
                 break
 
             #   Now loop through the filter definitions that are presented in decreasing frequency magnitude
             for filter_index in range(self._b_coefficients.shape[0]):
-                filtered_waveform = wfm.apply_iir_filter(self._b_coefficients[filter_index, :],
-                                                         self._a_coefficients[filter_index, :])
+                filtered_waveform = wfm.apply_iir_filter(
+                    self._b_coefficients[filter_index, :],
+                    self._a_coefficients[filter_index, :]
+                    )
 
                 frequency.append(fob_tools.center_frequency(self.fractional_octave_bandwidth, fob_band_index))
                 pressures.append(np.std(filtered_waveform.samples))
 
                 fob_band_index -= 1
 
             #   Decimate the waveform, halving the sample rate and making the filter definitions move down a full octave
             if len(wfm.samples) / 2 < 3 * self._b_coefficients.shape[1]:
-                warnings.warn("The number of points within the Waveform are insufficient to calculate digital filters "
-                              "lower than these frequencies")
+                warnings.warn(
+                    "The number of points within the Waveform are insufficient to calculate digital filters "
+                    "lower than these frequencies"
+                    )
 
                 break
 
-            wfm = Waveform(pressures=scipy.signal.decimate(wfm.samples, 2),
-                           sample_rate=wfm.sample_rate,
-                           start_time=wfm.start_time)
+            wfm = Waveform(
+                pressures=scipy.signal.decimate(wfm.samples, 2),
+                sample_rate=wfm.sample_rate,
+                start_time=wfm.start_time
+                )
 
         #   Convert the information within the pressures and frequency arrays into the correct elements for the class
         frequency = np.asarray(frequency)[::-1]
         pressures = np.asarray(pressures)[::-1]
 
-        idx0 = np.where(frequency > fob_tools.lower_frequency(self.fractional_octave_bandwidth,
-                                                              fob_tools.nearest_band(
-                                                                  self.fractional_octave_bandwidth,
-                                                                  self.start_fractional_octave_frequency)))[0][0]
-        idx1 = np.where(frequency < fob_tools.upper_frequency(self.fractional_octave_bandwidth,
-                                                              fob_tools.nearest_band(
-                                                                  self.fractional_octave_bandwidth,
-                                                                  self.stop_fractional_octave_frequency)))[0][-1]
+        idx0 = np.where(
+            frequency > fob_tools.lower_frequency(
+                self.fractional_octave_bandwidth,
+                fob_tools.nearest_band(
+                    self.fractional_octave_bandwidth,
+                    self.start_fractional_octave_frequency
+                )
+                )
+            )[0][0]
+        idx1 = np.where(
+            frequency < fob_tools.upper_frequency(
+                self.fractional_octave_bandwidth,
+                fob_tools.nearest_band(
+                    self.fractional_octave_bandwidth,
+                    self.stop_fractional_octave_frequency
+                )
+                )
+            )[0][-1]
         self._frequencies = frequency[np.arange(idx0, idx1 + 1)]
         self._acoustic_pressures_pascals = pressures[np.arange(idx0, idx1 + 1)]
```

### Comparing `PyTimbre-0.6.9/src/pytimbre/spectral/spectrogram.py` & `PyTimbre-0.7.1/src/pytimbre/spectral/spectrogram.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/src/pytimbre/spectral/swipe.py` & `PyTimbre-0.7.1/src/pytimbre/spectral/swipe.py`

 * *Files identical despite different names*

### Comparing `PyTimbre-0.6.9/src/pytimbre/spectral/time_histories.py` & `PyTimbre-0.7.1/src/pytimbre/spectral/time_histories.py`

 * *Files 2% similar despite different names*

```diff
@@ -665,49 +665,63 @@
         tpm = np.zeros((len(self.spectra),))
 
         for i in range(len(tpm)):
             tpm[i] = self.spectra[i].time_past_midnight
 
         return tpm
 
-    def concatenate(self, b=None, inplace: bool = False):
+    def concatenate(self, b=None, inplace: bool = False, normalize_time: bool = False):
+        """
+        This function will concatenate the TimeHistory that is passed as an argument to the current element. If the
+        inplace argument is True, the data is concatenated to the current object, otherwise it is returned as a new
+        object.
+
+        Parameters
+        ----------
+        :param b: TimeHistory
+            This is the object to concatenate with the current object
+        :param inplace: bool
+            Default = False - When False, this function will return a new TimeHistory Object, otherwise it returns a
+            new TimeHistory object
+        :param normalize_time: bool
+            Default = False - This will normalize the time to a zero for the first spectra.
+        """
         if not isinstance(b, TimeHistory):
             raise ValueError("The first argument is required to be a TimeHistory object.")
         if not np.array_equal(self.frequencies, b.frequencies):
             raise ValueError("Two TimeHistory objects must have same frequency content.")
-        if self.integration_time != b.integration_time:
+        if np.round(self.integration_time, decimals=3) != np.round(b.integration_time, decimals=3):
             raise AttributeError("Two TimeHistory objects must have same integration time.")
         warnings.warn('Concatenated TimeHistory object currently returns the header equal to the header of the first '
                       'TimeHistory object only.')
 
         if not inplace:
+            #   Create the TimeHistory object without any data
             th = TimeHistory(integration_time=self.integration_time)
-
             th._header = self._header
-
             th._spectra = np.empty(len(self.times) + len(b.times), dtype=Spectrum)
+            n = 0
+
+            #   Loop through the current object and copy the contents of the spectra to the new object
             for i in range(len(self.times)):
-                th._spectra[i] = self.spectra[i]
-                th._spectra[i]._time0 = i * self._integration_time
+                th._spectra[n] = self.spectra[i]
+                if normalize_time:
+                    th._spectra[n]._time0 = n * self._integration_time
+                n += 1
+
             for i in range(len(b.times)):
-                th._spectra[len(self.times) + i] = b.spectra[i]
-                th._spectra[len(self.times) + i]._time0 = (len(self.times) + i) * self._integration_time
+                th._spectra[n] = b.spectra[i]
+                if normalize_time:
+                    th._spectra[n]._time0 = n * self._integration_time
+                n += 1
 
             return th
 
         else:
 
-            # self._spectra = np.empty(len(self.times) + len(b.times), dtype=Spectrum)
-            # for i in range(len(self.times)):
-            #     self._spectra[i] = self.spectra[i]
-            #     self._spectra[i]._time0 = i * self._integration_time
-            # for i in range(len(b.times)):
-            #     self._spectra[len(self.times) + i] = b.spectra[i]
-            #     self._spectra[len(self.times) + i]._time0 = (len(self.times) + i) * self._integration_time
-
             raise NotImplementedError("inplace concatenation not yet implemented.")
 
 
 class NarrowbandTimeHistory(TimeHistory):
     """
     This class implements the _calculate_spectrogram function using the Narrowband_Spectrum class
     """
```

### Comparing `PyTimbre-0.6.9/src/pytimbre/waveform.py` & `PyTimbre-0.7.1/src/pytimbre/waveform.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-import math
+"""
+| Description: This is a base class for the storage or information as a collection of samples, a number of samples
+per second and the start time of these samples.
+| Contributors: Drs. Frank Mobley and Alan Wall, Conner Campbell, Gregory Bowers
+"""
+import sys
 import numpy as np
 from datetime import datetime, timedelta
 from enum import Enum
 from scipy.signal.windows import hamming, tukey
 import scipy.signal
 import statsmodels.api as sm
 import colorednoise as cn
 import warnings
 from typing import Dict, Tuple
 import numpy.typing as npt
 from .yin import yin
+import warnings
 
 
 class WindowingMethods(Enum):
     """
     The available windowing methods for the waveform
     """
 
@@ -75,42 +81,67 @@
     The available types of time scaling for conversion of a signal to equivalent levels
     """
 
     steady_state = 0
     transient = 1
 
 
+class AnalysisMethod(Enum):
+    """
+    |Description: Method for processing impulse metrics.
+    """
+
+    NONE = 0
+    MIL_STD_1474E = 1
+    MIL_STD_1474E_AFRL_PREF = 2
+    NO_A_DURATION_CORRECTIONS = 3
+
+
 class Waveform:
     """
-    This is a generic base class that contains the start time, samples and sample rate for a waveform.  Some limited
-    operations exist within this class for manipulation of the base data within the class.
+    |Description: This is a generic base class that contains the start time, samples and sample rate for a waveform.
+    Some limited operations exist within this class for manipulation of the base data within the class.
 
-    #   TODO: Add function to overload the __add__ operator so that two waveforms can be combined appropriately
     #   TODO: Add convolution function
-    #   TODO: Connect the WaveFile Start time to the Waveform start time
     #   TODO: Add function for SEL calculation
     #   TODO: Add filter array function
     Remarks
     2022-05-11 - FSM - added the function to determine whether the waveform is a calibration signal or not.
     """
 
-    def __init__(self, pressures, sample_rate, start_time, remove_dc_offset: bool = True):
+    def __init__(
+            self, pressures, sample_rate, start_time, remove_dc_offset: bool = True,
+            is_continuous_wfm: bool = True, is_steady_state: bool = True,
+            impulse_analysis_method: AnalysisMethod = AnalysisMethod.NO_A_DURATION_CORRECTIONS
+    ):
         """
         Default constructor
-        :param pressures: float, array-like - the list of pressure values
-        :param sample_rate: float - the number of samples per second
-        :param start_time: float or datetime - the time of the first sample
-        :param remove_dc_offset: bool, default = True - remove a DC offset from the samples
+        :param pressures:
+            float, array-like - the list of pressure values
+        :param sample_rate:
+            float - the number of samples per second
+        :param start_time:
+            float or datetime - the time of the first sample
+        :param remove_dc_offset:
+            bool, default = True - remove a DC offset from the samples
+        :param is_continuous_wfm:
+            bool - flag to determine whether this waveform is continuous or impulsive in nature. Default is True
+        :param is_steady_state:
+            bool - flag to determine whether this waveform is steady-state or transient in nature. Default is True
+        :param impulse_analysis_method:
+            Enumeration - this is a collection of the methods that might be used in the creation of impulse metrics.
         """
+        warnings.filterwarnings('ignore')
 
         self._samples = pressures
-        if remove_dc_offset:
-            self._samples -= np.mean(self._samples)
         self.fs = sample_rate
         self.time0 = start_time
+        self._is_continuous = is_continuous_wfm
+        self._is_steady_state = is_steady_state
+        self._impulse_analysis_method = impulse_analysis_method
         self._forward_coefficients = None
         self._reverse_coefficients = None
 
         self._coefficient_count = 12
         self._hop_size_seconds = 0.0029
         self._window_size_seconds = 0.0232
         self._cutoff_frequency = 5
@@ -118,22 +149,37 @@
         self._effective_duration_threshold = 0.4
 
         self._signal_envelope = None
         self._normal_signal_envelope = None
         self._log_attack = None
         self._increase = None
         self._decrease = None
-        self._Addresses = None
+        self._addresses = None
         self._amplitude_modulation = None
         self._frequency_modulation = None
         self._auto_correlation_coefficients = None
         self._zero_cross_rate = None
         self._temporal_centroid = None
         self._effective_duration = None
         self._temporal_feature_times = None
+        self._temporal_threshold_finding = 3
+
+        self._corrected_a_duration = None
+        self._liaeqT = None
+        self._liaeq100ms = None
+        self._liaeq8hr = None
+        self._SELA = None
+        self._noise_dose = None
+
+        #   Run some checks on the data based on the information in the constructors
+        if remove_dc_offset or self.is_impulsive:
+            self._samples -= np.mean(self._samples)
+
+        if self.is_impulsive and np.max(pressures) < -1.0 * np.min(pressures):
+            pressures *= -1.0
 
     # ---------------------- Collection of properties - this is both getters and setters -------------------------------
 
     @property
     def duration(self):
         """
         Determine the duration of the waveform by examining the number of samples and the sample rate
@@ -187,14 +233,61 @@
         return self.time0
 
     @start_time.setter
     def start_time(self, value):
         self.time0 = value
 
     @property
+    def is_continuous(self):
+        return self._is_continuous
+
+    @is_continuous.setter
+    def is_continuous(self, value):
+        self._is_continuous = value
+
+    @property
+    def is_impulsive(self):
+        return not self.is_continuous
+
+    @is_impulsive.setter
+    def is_impulsive(self, value):
+        """
+        Set to True to enable properties and methods tailored to impulsive acoustic signals.
+        """
+        self.is_continuous = not value
+
+    @property
+    def is_steady_state(self):
+        return self._is_steady_state
+
+    @is_steady_state.setter
+    def is_steady_state(self, value):
+        self._is_steady_state = value
+
+    @property
+    def is_transient(self):
+        return not self.is_steady_state
+
+    @is_transient.setter
+    def is_transient(self, value):
+        self.is_steady_state = not value
+
+    @property
+    def impulse_analysis_method(self):
+        return self._impulse_analysis_method
+
+    @impulse_analysis_method.setter
+    def impulse_analysis_method(self, method):
+        self._impulse_analysis_method = method
+        self._liaeqT = None
+        self._liaeq8hr = None
+        self._noise_dose = None
+        self._corrected_a_duration = None
+
+    @property
     def forward_coefficients(self):
         return self._forward_coefficients
 
     @property
     def reverse_coefficients(self):
         return self._reverse_coefficients
 
@@ -266,72 +359,82 @@
         """
         Set the number of coefficients for the analysis
         """
 
         self._coefficient_count = value
 
     @property
+    def temporal_threshold_finding(self):
+        return self._temporal_threshold_finding
+
+    @temporal_threshold_finding.setter
+    def temporal_threshold_finding(self,value):
+        self._temporal_threshold_finding = value
+
+
+
+    @property
     def attack(self):
-        if self._Addresses is None:
+        if self._addresses is None:
             self._calculate_signal_envelope()
-            self._log_attack, self._increase, self._decrease, self._Addresses = self.calculate_log_attack()
+            self._log_attack, self._increase, self._decrease, self._addresses = self.calculate_log_attack()
 
-        return self._Addresses[0]
+        return self._addresses[0]
 
     @property
     def decrease(self):
-        if self._Addresses is None:
+        if self._addresses is None:
             self._calculate_signal_envelope()
-            self._log_attack, self._increase, self._decrease, self._Addresses = self.calculate_log_attack()
+            self._log_attack, self._increase, self._decrease, self._addresses = self.calculate_log_attack()
 
-        return self._Addresses[1]
+        return self._addresses[1]
 
     @property
     def release(self):
-        if self._Addresses is None:
+        if self._addresses is None:
             self._calculate_signal_envelope()
-            self._log_attack, self._increase, self._decrease, self._Addresses = self.calculate_log_attack()
+            self._log_attack, self._increase, self._decrease, self._addresses = self.calculate_log_attack()
 
-        return self._Addresses[4]
+        return self._addresses[4]
 
     @property
     def log_attack(self):
         """
         The log-attack-time is simply defined as LAT = log_10(t[-1]-t[0])
         """
-        if self._Addresses is None:
+        if self._addresses is None:
             self._calculate_signal_envelope()
-            self._log_attack, self._increase, self._decrease, self._Addresses = self.calculate_log_attack()
+            self._log_attack, self._increase, self._decrease, self._addresses = self.calculate_log_attack()
 
         return self._log_attack
 
     @property
     def attack_slope(self):
         """
         The attack slope is defined as the average temporal slope of the energy during the attack segment. We compute
         the local slopes of the energy corresponding to each effort w_i. We then compute a weighted average of the
         slopes. The weights are chosen in order to emphasize slope values in the middle of the attack (the weights are
         the values of a Gaussian function centered around the threshold = 50% and with a standard-deviation of 0.5).
         """
-        if self._Addresses is None:
+        if self._addresses is None:
             self._calculate_signal_envelope()
-            self._log_attack, self._increase, self._decrease, self._Addresses = self.calculate_log_attack()
+            self._log_attack, self._increase, self._decrease, self._addresses = self.calculate_log_attack()
 
         return self._increase
 
     @property
     def decrease_slope(self):
         """
         The temporal decrease is a measure of the rate of decrease of the signal energy. It distinguishes non-sustained
         (e.g. percussive, pizzicato) sounds from sustained sounds. Its calculation is based on a decreasing exponential
         model of the energy envelope starting from it maximum.
         """
-        if self._Addresses is None:
+        if self._addresses is None:
             self._calculate_signal_envelope()
-            self._log_attack, self._increase, self._decrease, self._Addresses = self.calculate_log_attack()
+            self._log_attack, self._increase, self._decrease, self._addresses = self.calculate_log_attack()
 
         return self._decrease
 
     @property
     def temporal_centroid(self):
         """
         The temporal centroid is the center of gravity of the energy envelope. It distinguishes percussive from
@@ -355,24 +458,20 @@
             self._effective_duration = self.calculate_effective_duration()
 
         return self._effective_duration
 
     @property
     def amplitude_modulation(self):
         if self._amplitude_modulation is None:
-            self._calculate_signal_envelope()
-            self._log_attack, self._increase, self._decrease, self._Addresses = self.calculate_log_attack()
             self._frequency_modulation, self._amplitude_modulation = self.calculate_modulation()
         return self._amplitude_modulation
 
     @property
     def frequency_modulation(self):
         if self._frequency_modulation is None:
-            self._calculate_signal_envelope()
-            self._log_attack, self._increase, self._decrease, self._Addresses = self.calculate_log_attack()
             self._frequency_modulation, self._amplitude_modulation = self.calculate_modulation()
         return self._frequency_modulation
 
     @property
     def auto_correlation(self):
         if self._auto_correlation_coefficients is None:
             self._temporal_feature_times, self._auto_correlation_coefficients, self._zero_cross_rate = \
@@ -440,22 +539,165 @@
 
         clipped_sections, total_clipped_samples = Waveform._detect_clipping(self.samples)
 
         return not ((total_clipped_samples / len(self.samples)) < 0.01)
 
     @property
     def fundamental_frequency(self):
-        return np.median(yin(
-            self.samples,
-            self.sample_rate,
-            F_max=10000,
-            F_min=10,
-            N=int(np.floor(self.sample_rate / 10)),
-            H=int(np.floor(self.sample_rate / 10 / 4))
-        )[0])
+        return np.median(
+            yin(
+                self.samples,
+                self.sample_rate,
+                F_max=10000,
+                F_min=10,
+                N=int(np.floor(self.sample_rate / 10)),
+                H=int(np.floor(self.sample_rate / 10 / 4))
+            )[0]
+        )
+
+    @property
+    def peak_pressure(self):
+        return np.max(self.samples)
+
+    @property
+    def peak_level(self):
+        return 20 * np.log10(self.peak_pressure / 20e-6)
+
+    @property
+    def peak_time(self):
+        return self.times[np.argmax(self.samples)]
+
+    @property
+    def a_duration(self):
+        """"
+        -20220329 - SCC - Fixed code. Was flipping polairty of every signal and couldn't find right zero crossing.
+        """
+        p2 = self.samples
+        p2 -= np.mean(p2[:400000])
+        max_p = np.max(p2)
+        max_p_idx = np.argmax(np.abs(p2))
+
+        maximum_pressure = self.samples[max_p_idx]
+        if maximum_pressure < 0:
+            p2 *= -1
+
+        #   Find the start time for the A-duration, whcih is the first zero-crossing before the peak pressure
+
+        if (max_p_idx > 1) and (max_p_idx <= len(p2)):
+            e1 = max_p_idx
+        else:
+            e1 = 0
+
+        located = False
+        while (not located) and (e1 > 0):
+            e1 -= 1
+            if p2[e1] <= 0:
+                located = True
+                break
+
+        #   Interpolate to determine a more accurate representation of this time
+
+        if (abs(p2[e1] - p2[e1 + 1]) >= 1e-12) and (located is True):
+            at1 = (0 - p2[e1]) / (p2[e1 + 1] - p2[e1]) + e1 + 1
+        else:
+            at1 = e1
+
+        #   find the end time for the A-duration, which is the last zero-crossing after the peak
+
+        if (max_p_idx > 1) and (max_p_idx <= len(p2)):
+            e1 = max_p_idx
+        else:
+            e1 = 1
+
+        located = False
+        while (not located) and (e1 < len(p2)):
+            e1 += 1
+            if p2[e1] <= 0:
+                located = True
+                break
+
+        #   Interpolate to determine a more accurate representation of this time
+
+        if (abs(p2[e1] - p2[e1 - 1]) >= 1e-12) and (located is True):
+            at2 = (0 - p2[e1 - 1]) / (p2[e1] - p2[e1 - 1]) + e1
+        else:
+            at2 = e1
+
+        return (at2 - at1) / self.sample_rate
+
+    @property
+    def leqT(self):
+        if self.is_impulsive:
+            # Sum and average energy across waveform for total recording time
+            return self.equivalent_level(
+                WeightingFunctions.unweighted, self.duration,
+                leq_mode=LeqDurationMode.transient
+                )
+
+    @property
+    def SEL(self):
+        if self.is_impulsive:
+            # Sum and average energy across waveform and scale to 1 second
+            return self.equivalent_level(WeightingFunctions.unweighted, 1.0, leq_mode=LeqDurationMode.transient)
+        elif self.is_continuous:
+            raise NotImplementedError()
+
+    @property
+    def noise_dose(self):
+        if self.is_impulsive:
+            if self._noise_dose is None:
+                self._process_analysis()
+            return self._noise_dose
+        else:
+            raise ValueError("This waveform is not impulsive")
+
+    @property
+    def liaeqT(self):
+        if self.is_impulsive:
+            if self._liaeqT is None:
+                self._process_analysis()
+            return self._liaeqT
+        else:
+            raise ValueError("This waveform is not impulsive")
+
+    @property
+    def liaeq100ms(self):
+        if self.is_impulsive:
+            if self._liaeq100ms is None:
+                self._process_analysis()
+            return self._liaeq100ms
+        else:
+            raise ValueError("This waveform is not impulsive")
+
+    @property
+    def liaeq8hr(self):
+        if self.is_impulsive:
+            if self._liaeq8hr is None:
+                self._process_analysis()
+            return self._liaeq8hr
+        else:
+            raise ValueError("This waveform is not impulsive")
+
+    @property
+    def SELA(self):
+        if self.is_impulsive:
+            if self._SELA is None:
+                self._process_analysis()
+            return self._SELA
+        else:
+            raise NotImplementedError()
+
+    @property
+    def corrected_a_duration(self):
+        if self.is_impulsive:
+            if self._corrected_a_duration is None:
+                self._process_analysis()
+            return self._corrected_a_duration
+        else:
+            raise ValueError("This waveform is not impulsive")
 
     # ------------------ Static functions for the calculation of filter shapes and timbre features ---------------------
     @staticmethod
     def _detect_clipping(
             samples_array: npt.NDArray, max_threshold=0.995, min_threshold=0.995
     ) -> Tuple[Dict[str, int], int]:
         """
@@ -747,16 +989,18 @@
                       sample_rate)
         date = datetime(int(elements[9][4:]) + 2000, int(elements[9][2:4]), int(elements[9][:2])) + \
                timedelta(seconds=start_time)
 
         return date
 
     @staticmethod
-    def generate_tone(frequency: float = 100, sample_rate: float = 48000, duration: float = 1.0,
-                      amplitude_db: float = 94):
+    def generate_tone(
+            frequency: float = 100, sample_rate: float = 48000, duration: float = 1.0,
+            amplitude_db: float = 94
+    ):
         """
         This function generates a sine wave tone function with the specific frequency and duration specified in the
         argument list.
 
         Parameters
         ----------
         frequency: float, default: 100 - the linear frequency of the waveform
@@ -772,25 +1016,76 @@
         amplitude_rms = 10 ** (amplitude_db / 20) * 2e-5
         x = np.arange(0, duration, 1 / sample_rate)
         y = amplitude_rms * np.sqrt(2) * np.sin(2 * np.pi * frequency * x)
 
         return Waveform(y, sample_rate, 0)
 
     @staticmethod
-    def generate_noise(sample_rate: float = 48000, duration: float = 1.0, amplitude_db: float = 94,
-                       noise_color=NoiseColor.pink):
+    def generate_noise(
+            sample_rate: float = 48000, duration: float = 1.0, amplitude_db: float = 94,
+            noise_color=NoiseColor.pink
+    ):
         samples = cn.powerlaw_psd_gaussian(noise_color.value, int(np.floor(duration * sample_rate)))
 
         wfm = Waveform(samples, sample_rate, 0)
         scaling = amplitude_db - wfm.overall_level()
         wfm.scale_signal(scaling, True, ScalingMethods.logarithmic)
 
         return wfm
 
     @staticmethod
+    def generate_friedlander(
+            peak_level: float = 165, a_duration: float = 0.005, duration: float = 3
+            , sample_rate: float = 200e3, blast_time: float = 0.005 / 2.0, noise: bool = False
+    ):
+        """
+        Generates a generic_time_waveform object containing a Friedlander waveform
+        :param peak_level: float, defaults to 165dB.
+        :param a_duration: float, defaults to 0.005s.
+        :param duration: float, length of total waveform in s. Defaults to 3s.
+        :param sample_rate: float, defaults to 200e3 Hz.
+        :param blast_time: float, time when friedlander starts in signal. Defualts to half the default a_duration and
+        must be less than the duration of the signal minus 2 * a_duration.
+        :param noise: bool, if True adds +/-94dB random noise (1pa) to the signal.
+
+        -20220325 - SCC - Created method.
+        """
+        # time array, sec.
+        t0 = 0.0
+
+        if blast_time >= duration - 2.0 * a_duration:
+            raise ValueError("Blast time inout must be before the end of the duration of the signal!")
+
+        else:
+
+            t = np.arange(t0, duration + 1 / sample_rate, 1 / sample_rate)
+
+            if noise is True:
+                p = np.random.randint(-1, 1, size=(len(t) - 1,)) / 1.0
+
+            else:
+                p = np.zeros(len(t) - 1)
+
+            t_fried = np.arange(t0 / sample_rate, duration - blast_time + 1 / sample_rate, 1 / sample_rate)
+
+            p_fried = np.exp(-1.0 * t_fried / a_duration)
+            p_fried = np.multiply(p_fried, (1.0 - t_fried / a_duration))
+            p_fried = (10.0 ** (peak_level / 20.0) * 2e-5) * p_fried
+
+            p[round(blast_time * sample_rate - 1):] = p_fried
+
+            fried = Waveform(
+                pressures=p, sample_rate=sample_rate, start_time=t0, is_continuous_wfm=False,
+                is_steady_state=False
+                )
+            fried.is_impulsive = True
+
+            return fried
+
+    @staticmethod
     def irig_converter(signal):
         """
         Compute the time of the signal using the IRIG-B format as reference.
 
         Parameters
         ----------
         signal : double, array-like
@@ -921,15 +1216,16 @@
         timevector = times[0] + (index - prrise[0]) / sps
 
         return times[0] - prrise[0] / sps, day_of_year
 
     @staticmethod
     def irig_converter_for_arc(data, fs):
         """
-        The timecode generators present at the Aeroacoustic Research Complex (ARC) produce the signal that defines the IRIG-
+        The timecode generators present at the Aeroacoustic Research Complex (ARC) produce the signal that defines
+        the IRIG-
         B timecode differently. The previous methods do not return the correct information for the ARC data.
 
 
         """
         #   Find the index of the first minimum - which is assumed to occur within the first second of the waveform
 
         index = np.where(data[:fs] == np.min(data[:fs]))[0][0]
@@ -1079,31 +1375,40 @@
 
         Returns
         _______
         :returns: Waveform - a subset of the waveform samples
         """
 
         #   Handle the start/stop samples may be passed as None arguments
-
         if s0 is None:
             s0 = 0
 
         if s1 is None:
             s1 = self._samples.shape[0]
 
         #   Determine the new start time of the waveform
-
         if isinstance(self.start_time, datetime):
             t0 = self.start_time + timedelta(seconds=s0 / self.sample_rate)
         else:
             t0 = self.start_time + s0 / self.sample_rate
 
         #   Create the waveform based on the new time, and the subset of the samples
+        wfm = Waveform(self.samples[np.arange(s0, s1)].copy(), self.sample_rate, t0, remove_dc_offset=False)
 
-        return Waveform(self.samples[np.arange(s0, s1)].copy(), self.sample_rate, t0, remove_dc_offset=False)
+        #   Copy values that can be changed through properties, but are set in the constructor
+        wfm.is_continuous = self.is_continuous
+        wfm.is_steady_state = self.is_steady_state
+        wfm.impulse_analysis_method = self.impulse_analysis_method
+        wfm.cutoff_frequency = self.cutoff_frequency
+        wfm.window_size_seconds = self.window_size_seconds
+        wfm.hop_size_seconds = self.hop_size_seconds
+        wfm.coefficient_count = self.coefficient_count
+        wfm.temporal_threshold_finding = self.temporal_threshold_finding
+
+        return wfm
 
     def _scale_waveform(self, scale_factor: float = 1.0, inplace: bool = False):
         """
         This function applies a scaling factor to the waveform's sample in a linear scale factor.
 
         Parameters
         __________
@@ -1118,14 +1423,120 @@
         if inplace:
             self._samples *= scale_factor
 
             return None
         else:
             return Waveform(self._samples * scale_factor, self.sample_rate, self.start_time)
 
+    def _process_mil_std_1474e(self):
+        # Process A-weighted equivalent energy metrics in accordance to MIL-STD 1474E B.5.3.2 EQ 1A
+        # Sum and average energy across waveform for total recording time
+        self._liaeqT = self.equivalent_level(
+            weighting=WeightingFunctions.a_weighted,
+            equivalent_duration=self.duration,
+            leq_mode=LeqDurationMode.transient
+        )
+        self._liaeq100ms = self.equivalent_level(
+            weighting=WeightingFunctions.a_weighted,
+            equivalent_duration=0.1,
+            leq_mode=LeqDurationMode.transient
+        )
+
+        # Limit A-duration according to Notes 1-3 in MIL-STD-1474E B.5.4.1
+        if self.a_duration < 2e-4:
+            self._corrected_a_duration = 2e-4
+        elif self.a_duration > 2.5e-3:
+            self._corrected_a_duration = 2.5e-3
+        else:
+            self._corrected_a_duration = self.a_duration
+
+        # Process A-weighted 8-hour equivalent energy metric in accordance to MIL-STD 1474E B.5.4.1 EQ 3A and 3B
+
+        self._liaeq8hr = self._liaeqT + 10.0 * np.log10(self.duration / 28800.0) - 1.5 * 10.0 * \
+                         np.log10(self._corrected_a_duration / 2e-4)
+        self._SELA = self._liaeq8hr + 10.0 * np.log10(28800.0 / 1.0)
+
+        # Process noise dose with 3 db exchange rate, 85dBA limit for 8 hours from MIL-STD 1474E B.5.3.4.2 EQ 4
+        self._noise_dose = 100.0 / (2 ** ((85 - self._liaeq8hr) / 3.0))
+
+    def _process_mil_std_1474e_afrl_pref(self):
+        # Process A-weighted equivalent energy metrics in accordance to MIL-STD 1474E B.5.3.2 EQ 1A
+        # Sum and average energy across waveform for total recording time
+        # Limit A-duration according to Notes 1-3 in MIL-STD-1474E B.5.4.1
+        if self.a_duration < 2e-4:
+            self._corrected_a_duration = 2e-4
+        elif self.a_duration > 2.5e-3:
+            self._corrected_a_duration = 2.5e-3
+        else:
+            self._corrected_a_duration = self.a_duration
+
+        self._liaeqT = self.equivalent_level(
+            weighting=WeightingFunctions.a_weighted,
+            equivalent_duration=self.duration,
+            leq_mode=LeqDurationMode.transient
+            )
+        self._liaeqT -= 1.5 * 10.0 * np.log10(self._corrected_a_duration / 2e-4)
+
+        self._SELA = self._liaeqT + 10.0 * np.log10(self.duration / 1.0)
+
+        self._liaeq100ms = self._liaeqT + 10.0 * np.log10(self.duration / 0.1)
+
+        # Process A-weighted 8-hour equivalent energy metric in accordance to MIL-STD 1474E B.5.4.1 EQ 3A and 3B
+        self._liaeq8hr = self._liaeqT + 10.0 * np.log10(self.duration / 28800.0)
+
+        # Process noise dose with 3 db exchange rate, 85dBA limit for 8 hours from MIL-STD 1474E B.5.3.4.2 EQ 4
+        self._noise_dose = 100.0 / (2 ** ((85 - self._liaeq8hr) / 3.0))
+
+    def _process_no_a_duration_correction(self):
+        self._corrected_a_duration = self.a_duration
+
+        # Process A-weighted equivalent energy metrics in accordance to MIL-STD 1474E without a_duration corrections
+        self._liaeqT = self.equivalent_level(
+            weighting=WeightingFunctions.a_weighted,
+            equivalent_duration=self.duration,
+            leq_mode=LeqDurationMode.transient
+            )
+
+        self._SELA = self.equivalent_level(
+            weighting=WeightingFunctions.a_weighted,
+            equivalent_duration=1.0,
+            leq_mode=LeqDurationMode.transient
+            )
+
+        self._liaeq100ms = self.equivalent_level(
+            weighting=WeightingFunctions.a_weighted,
+            equivalent_duration=0.1,
+            leq_mode=LeqDurationMode.transient
+            )
+
+        self._liaeq8hr = self.equivalent_level(
+            weighting=WeightingFunctions.a_weighted,
+            equivalent_duration=8 * 60 * 60,
+            leq_mode=LeqDurationMode.transient
+            )
+
+        # Process noise dose with 3 db exchange rate, 85dBA limit for 8 hours from MIL-STD 1474E B.5.3.4.2 EQ 4
+        self._noise_dose = 100.0 / (2 ** ((85 - self._liaeq8hr) / 3.0))
+
+    def _process_analysis(self):
+        # Method with MIL STD 1474E
+        if self.impulse_analysis_method == AnalysisMethod.MIL_STD_1474E:
+            self._process_mil_std_1474e()
+
+            # Method with MIL STD 1474E and a_durations corrected at liaegT instead of liaeq8hr.
+        elif self.impulse_analysis_method == AnalysisMethod.MIL_STD_1474E_AFRL_PREF:
+            self._process_mil_std_1474e_afrl_pref()
+
+        # Method without a duration corrections in MIL STD 1474E
+        elif self.impulse_analysis_method == AnalysisMethod.NO_A_DURATION_CORRECTIONS:
+            self._process_no_a_duration_correction()
+
+        elif self.impulse_analysis_method == AnalysisMethod.NONE:
+            raise Warning("You should not call this function without declaring this as an impulsive waveform.")
+
     # -------------------- Public functions for operations on the samples within the Waveform --------------------------
 
     def determine_calibration_scale_factor(self, level: float = 114, frequency: float = 1000):
         """
         This function will take the information within the current Waveform and determine the scaling factor that can be
         applied to this, or any other file, to ensure that the acoustic reference is obtained.
 
@@ -1139,21 +1550,25 @@
         """
 
         from .spectral.fractional_octave_band import FractionalOctaveBandTools as fob
 
         #   ensure that the calibration frequency is actually located within the Waveform.
         calibration, detected_frequency = self.is_calibration()
         if not calibration or abs(detected_frequency - frequency) > 25:
-            raise ValueError("The Waveform passed to the function does not contain a calibration tone or the tone is "
-                             "not at the expected frequency, based on the arguments of the function.")
+            raise ValueError(
+                "The Waveform passed to the function does not contain a calibration tone or the tone is "
+                "not at the expected frequency, based on the arguments of the function."
+            )
 
         #   Now we need to calculate the scale factor required to adjust the level of the calibration Waveform to the
         #   desired magnitude.
-        filtered_wfm = self.apply_bandpass(fob.lower_frequency(3, fob.nearest_band(3, frequency)),
-                                           fob.upper_frequency(3, fob.nearest_band(3, frequency)))
+        filtered_wfm = self.apply_bandpass(
+            fob.lower_frequency(3, fob.nearest_band(3, frequency)),
+            fob.upper_frequency(3, fob.nearest_band(3, frequency))
+        )
 
         #   Now assuming that the data within the samples array is a pressure
         rms_level = 20 * np.log10(np.std(filtered_wfm.samples) / 20e-6)
 
         sens = level - rms_level
         sens /= 20
         sens *= -1
@@ -1186,16 +1601,18 @@
         scaled_calibration_wfm = wfm.scale_signal(1 / sens)
 
         if abs(np.any(scaled_calibration_wfm.overall_level() - level)) > 2:
             raise ValueError("The method did not appropriately scale the calibration signal")
 
         return self.scale_signal(1 / sens, inplace=inplace)
 
-    def scale_signal(self, factor: float = 1.0, inplace: bool = False,
-                     scale_type: ScalingMethods = ScalingMethods.linear):
+    def scale_signal(
+            self, factor: float = 1.0, inplace: bool = False,
+            scale_type: ScalingMethods = ScalingMethods.linear
+    ):
         """
         This method will call the sub-function to scale the values of the waveform in linear fashion. If the scale
         factor is provided in logarithmic form, it will be converted to a linear value and sent to the sub-function.
 
         Parameters
         ----------
         :param factor: float - the scale factor that needs to be passed to the scaling sub-function, which will be
@@ -1294,15 +1711,16 @@
         return Waveform(scipy.signal.lfilter(b, a, self.samples), self.sample_rate, self.start_time)
 
     def apply_a_weight(self):
         """
         This function specifically applies the a-weighting filter to the acoustic data, and returns a new waveform with
         the filter applied.
 
-        :returns: generic_time_waveform - the filtered waveform
+        :returns:
+            generic_time_waveform - the filtered waveform
         """
         a, c = Waveform.AC_Filter_Design(self.sample_rate)
 
         return self.apply_iir_filter(a[0], a[1])
 
     def apply_c_weight(self):
         """
@@ -1404,16 +1822,18 @@
         Waveform - the new waveform object that contains the resampled data with the new sample rate.
         """
 
         #   Determine the ratio of the current sample rate to the new sample rate
 
         sr_ratio = new_sample_rate / self.sample_rate
 
-        return Waveform(scipy.signal.resample(self.samples, int(np.floor(len(self.samples) * sr_ratio))),
-                        new_sample_rate, self.start_time)
+        return Waveform(
+            scipy.signal.resample(self.samples, int(np.floor(len(self.samples) * sr_ratio))),
+            new_sample_rate, self.start_time
+        )
 
     def apply_tob_equalizer_filter(self, frequencies: np.ndarray, sound_pressure_levels: np.ndarray):
         from .spectral.fractional_octave_band import FractionalOctaveBandTools as fob
         import warnings
 
         """
         Pass the waveform through a series of filters adjusting the amplitude by the adjusted value of the arrays.
@@ -1474,17 +1894,19 @@
             low_band = int(np.floor(fob.nearest_band(1, frequencies[0])))
             hi_band = int(np.floor(fob.nearest_band(1, frequencies[-1])))
 
             #   Get the index of the band at the top of the full octave filter
             fob_band_index = int(np.floor(fob.nearest_band(3, fob.upper_frequency(1, hi_band))))
 
             #   Make a copy of the waveform that can be decimated
-            wfm = Waveform(pressures=self.samples.copy(),
-                           sample_rate=self.sample_rate,
-                           start_time=self.start_time)
+            wfm = Waveform(
+                pressures=self.samples.copy(),
+                sample_rate=self.sample_rate,
+                start_time=self.start_time
+            )
 
             #   Loop through the frequencies
             for band_index in range(hi_band, low_band - 1, -1):
                 #   Loop through the filter definitions
                 for filter_index in range(len(b_coefficients)):
                     filtered_waveform = wfm.apply_iir_filter(b_coefficients[filter_index], a_coefficients[filter_index])
 
@@ -1503,21 +1925,24 @@
                         samples += filtered_waveform.samples[:len(samples)]
 
                     #   Decimate the waveform, halving the sample rate and making the filter definitions move down a
                     #   full octave
                     if len(wfm.samples) / 2 < 3 * len(b_coefficients):
                         warnings.warn(
                             "The number of points within the Waveform are insufficient to calculate digital filters "
-                            "lower than these frequencies")
+                            "lower than these frequencies"
+                        )
 
                         break
 
-                    wfm = Waveform(pressures=scipy.signal.decimate(wfm.samples, 2),
-                                   sample_rate=wfm.sample_rate,
-                                   start_time=wfm.start_time)
+                    wfm = Waveform(
+                        pressures=scipy.signal.decimate(wfm.samples, 2),
+                        sample_rate=wfm.sample_rate,
+                        start_time=wfm.start_time
+                    )
 
         return Waveform(pressures=samples, sample_rate=self.sample_rate, start_time=self.start_time)
 
     def is_calibration(self):
         """
         This function examines the samples and determines whether the single contains a single pure tone.  If it does
         the function returns the approximate frequency of the tone.  This will examine every channel and determine
@@ -1569,33 +1994,43 @@
 
         Returns
         -------
         features : dict()
             The dictionary containing the various values calculated within this method.
         """
 
-        #   Create the dictionary that will hold the data for return to the user
-
-        features = {'attack': self.attack,
-                    'decrease': self.decrease,
-                    'release': self.release,
-                    'log_attack': self.log_attack,
-                    'attack slope': self.attack_slope,
-                    'decrease slope': self.decrease_slope,
-                    'temporal centroid': self.temporal_centroid,
-                    'effective duration': self.effective_duration,
-                    'amplitude modulation': self.amplitude_modulation,
-                    'frequency modulation': self.frequency_modulation,
-                    'auto-correlation': self.auto_correlation,
-                    'zero crossing rate': self.zero_crossing_rate}
-
-        if include_sq_metrics:
-            features['loudness'] = self.loudness
-            features['roughness'] = self.roughness
-            features['sharpness'] = self.sharpness
+        if self.is_continuous:
+            #   Create the dictionary that will hold the data for return to the user
+            features = {'attack': self.attack,
+                        'decrease': self.decrease,
+                        'release': self.release,
+                        'log_attack': self.log_attack,
+                        'attack slope': self.attack_slope,
+                        'decrease slope': self.decrease_slope,
+                        'temporal centroid': self.temporal_centroid,
+                        'effective duration': self.effective_duration,
+                        'amplitude modulation': self.amplitude_modulation,
+                        'frequency modulation': self.frequency_modulation,
+                        'auto-correlation': self.auto_correlation,
+                        'zero crossing rate': self.zero_crossing_rate}
+
+            if include_sq_metrics:
+                features['loudness'] = self.loudness
+                features['roughness'] = self.roughness
+                features['sharpness'] = self.sharpness
+        elif self.is_impulsive:
+            features = {'a-duration': self.a_duration,
+                        'equivalent level (T)': self.leqT,
+                        'equivalent level a-weighted (T)': self.liaeqT,
+                        'equivalent level a-weighted (8 hr)': self.liaeq8hr,
+                        'equivalent level a-weighted (100ms)': self.liaeq100ms,
+                        'peak level (dB)': self.peak_level,
+                        'peak pressure (Pa)': self.peak_pressure,
+                        'sound exposure level': self.SEL,
+                        'a-weighted sound exposure level': self.SELA}
 
         return features
 
     def calculate_temporal_centroid(self):
 
         env_max_idx = np.argmax(self.signal_envelope)
         over_threshold_idcs = np.where(self.normal_signal_envelope > self.centroid_threshold)[0]
@@ -1604,16 +2039,18 @@
         if over_threshold_start_idx == env_max_idx:
             over_threshold_start_idx = over_threshold_start_idx - 1
 
         over_threshold_end_idx = over_threshold_idcs[-1]
 
         over_threshold_TEE = self.signal_envelope[over_threshold_start_idx - 1:over_threshold_end_idx - 1]
         over_threshold_support = [*range(len(over_threshold_TEE))]
-        over_threshold_mean = np.divide(np.sum(np.multiply(over_threshold_support, over_threshold_TEE)),
-                                        np.sum(over_threshold_TEE))
+        over_threshold_mean = np.divide(
+            np.sum(np.multiply(over_threshold_support, over_threshold_TEE)),
+            np.sum(over_threshold_TEE)
+        )
 
         temporal_threshold = ((over_threshold_start_idx + 1 + over_threshold_mean) / self.sample_rate)
 
         return temporal_threshold
 
     def calculate_effective_duration(self):
 
@@ -1624,34 +2061,23 @@
         if over_threshold_start_idx == env_max_idx:
             over_threshold_start_idx = over_threshold_start_idx - 1
 
         over_threshold_end_idx = over_threshold_idcs[-1]
 
         return (over_threshold_end_idx - over_threshold_start_idx + 1) / self.sample_rate
 
-    # def rms_envelope(self):
-    #
-    #     win_size = int(round(self._window_size_seconds * self.sample_rate))
-    #     hop_size = int(round(self._hop_size_seconds * self.sample_rate))
-    #     t_support = [*range(0, int(round(hop_size * np.floor((len(self.samples) - win_size) / hop_size))), hop_size)]
-    #     value = []
-    #     for i in range(len(t_support)):
-    #         a = self.samples[np.subtract(np.add(t_support[i], [*range(1, win_size + 1)]), 1).astype(int)]
-    #         value.append(np.sqrt(np.mean(np.power(a, 2))))
-    #     t_support = np.divide(np.add(t_support, np.ceil(np.divide(win_size, 2))), self.sample_rate)
-    #     return value
-
     def instantaneous_temporal_features(self):
         """
         This function will calculate the instantaneous features within the temporal analysis.  This includes the
         auto-correlation and the zero crossing rate.
         """
         count = 0
         temporal_feature_times = np.zeros(
-            (int(np.floor((len(self.samples) - self.window_size_samples) / self.hop_size_samples) + 1),))
+            (int(np.floor((len(self.samples) - self.window_size_samples) / self.hop_size_samples) + 1),)
+        )
 
         auto_coefficients = np.zeros((len(temporal_feature_times), self.coefficient_count))
         zero_crossing_rate = np.zeros((len(temporal_feature_times),))
 
         #   Loop through the frames
 
         for n in range(0, len(temporal_feature_times)):
@@ -1690,16 +2116,19 @@
             A metric measuring the frequency modulation of the signal
         amplitude_modulation : double
             A metric measuring the amplitude modulation of the signal
         """
 
         sample_times = np.arange(len(self.signal_envelope) - 1) / self.sample_rate
 
-        sustain_start_time = self._Addresses[1]
-        sustain_end_time = self._Addresses[4]
+        if self._addresses is None:
+            self._log_attack, self._increase, self._decrease, self._addresses = self.calculate_log_attack()
+
+        sustain_start_time = self._addresses[1]
+        sustain_end_time = self._addresses[4]
 
         is_sustained = False
 
         if (sustain_end_time - sustain_start_time) > 0.02:
             pos_v = np.where((sustain_start_time <= sample_times) & (sample_times <= sustain_end_time))[0]
             if len(pos_v) > 0:
                 is_sustained = True
@@ -1752,16 +2181,19 @@
         release : TYPE
             DESCRIPTION.
         release_slope : TYPE
             DESCRIPTION.
 
         """
 
+        if self.normal_signal_envelope is None:
+            self._calculate_signal_envelope()
+
         #   Define some specific constants for this calculation
-        method = 3
+        method = self.temporal_threshold_finding
         noise_threshold = 0.15
         decrease_threshold = 0.4
         percent_step = 0.1
 
         #   Detection of the start (start_attack_position) and stop (end_attack_position) of the attack
         position_value = np.where(self.normal_signal_envelope > noise_threshold)[0]
 
@@ -1817,15 +2249,18 @@
 
             start_attack_position = percent_value_position[index]
 
             #   refinement: we are looking for the local minimum
             delta = int(np.round(0.25 * (percent_value_position[index + 1] - percent_value_position[index]))) - 1
             n = int(np.floor(percent_value_position[index]))
 
-            if n - delta >= 0:
+            if delta == 0:
+                min_position = n
+                end_attack_position = 2 * n
+            elif n - delta >= 0:
                 min_position = np.argmin(self.normal_signal_envelope[n - delta:n + delta])
                 start_attack_position = min_position + n - delta - 1
 
             #   Start the end attack calculation
             #   we STOP JUST BEFORE the effort to be made (temporal gap between percent) is too large
             position2_value = np.where(percent_position_value[e1att:e2att] > multiplier * M)[0]
 
@@ -1836,15 +2271,18 @@
 
             end_attack_position = percent_value_position[index]
 
             #   refinement: we are looking for the local minimum
             delta = int(np.round(0.25 * (percent_value_position[index] - percent_value_position[index - 1])))
             n = int(np.floor(percent_value_position[index]))
 
-            if n - delta >= 0:
+            if delta == 0:
+                min_position = n
+                end_attack_position = 2*n
+            elif n - delta >= 0:
                 min_position = np.argmax(self.normal_signal_envelope[n - delta:n + delta + 1])
                 end_attack_position = min_position + n - delta
 
         #   Calculate the Log-attack time
         if start_attack_position == end_attack_position:
             start_attack_position -= 1
 
@@ -1852,32 +2290,38 @@
         log_attack_time = np.log10(rise_time_n / self.sample_rate)
 
         #   Calculate the temporal growth - New 13 Jan 2003
         #   weighted average (Gaussian centered on percent=50%) slopes between start_attack_position and
         #   end_attack_position
         start_attack_position = int(np.round(start_attack_position))
         end_attack_position = int(np.round(end_attack_position))
+
+        if end_attack_position <= start_attack_position:
+            end_attack_position = start_attack_position + 1
+
         start_attack_value = self.normal_signal_envelope[start_attack_position]
         end_attack_value = self.normal_signal_envelope[end_attack_position]
 
         #   Now that we have determined where the attack occurs, we must define a set of thresholds as a proportion
         #   of the maximum pf the energy envelop. To ensure that the value is within the attack range, we seek for
         #   the maximum within this region.
         threshold_value = np.arange(0.1, 1.1, 0.1)
         threshold_value *= np.max(self.normal_signal_envelope[start_attack_position:end_attack_position])
         threshold_position_seconds = np.zeros(np.size(threshold_value))
         for i in range(len(threshold_value)):
             #   Find the index within the envelope where the value is greater than the selected threshold value
-            idx = np.where(self.normal_signal_envelope[start_attack_position:end_attack_position] >=
-                           threshold_value[i])[0]
+            idx = np.where(
+                self.normal_signal_envelope[start_attack_position:end_attack_position] >=
+                threshold_value[i]
+            )[0]
 
             if len(idx) > 0:
                 threshold_position_seconds[i] = idx[0] / self.sample_rate
 
-        slopes = np.divide(np.diff(threshold_value), np.diff(threshold_position_seconds))
+        slopes = np.divide(np.diff(threshold_value), np.diff(threshold_position_seconds) + sys.float_info.epsilon)
 
         #   Calculate the increase
         thresholds = (threshold_value[:-1] + threshold_value[1:]) / 2
         weights = np.exp(-(thresholds - 0.5) ** 2 / (0.5 ** 2))
         increase = np.sum(np.dot(slopes, weights)) / np.sum(weights)
 
         #   Calculate the time decay
@@ -1903,21 +2347,23 @@
 
         #   Create the list of addresses that we are interested in storing for later consumption
 
         addresses = np.array([start_attack_position, envelope_max_index, 0, 0, stop_position]) / self.sample_rate
 
         return log_attack_time, increase, decrease, addresses
 
-    def equivalent_level(self,
-                         weighting: WeightingFunctions = WeightingFunctions.a_weighted,
-                         equivalent_duration: float = 8 * 3600,
-                         start_sample: int = 0,
-                         stop_sample: int = None,
-                         leq_mode: LeqDurationMode = None,
-                         exposure_duration: float = None):
+    def equivalent_level(
+            self,
+            weighting: WeightingFunctions = WeightingFunctions.a_weighted,
+            equivalent_duration: float = 8 * 3600,
+            start_sample: int = 0,
+            stop_sample: int = None,
+            leq_mode: LeqDurationMode = None,
+            exposure_duration: float = None
+    ):
         """
         This function computes the equivalent level on the pressures within the waveform. If there is a weighting
         function specified this is applied before the pressures are summed. Additionally, the duration of the summation
         is specified (in seconds) for the new value with a default of 8 hours. Finally, if there is a cause to exclude
         portions of the data (i.e. calculating the SEL for the 10 dB down points in community noise) you can specify
         the start and stop index. If the stop index is None, then the last pressure defines the limit of the summation.
 
@@ -1966,16 +2412,18 @@
         elif leq_mode is None:
             raise ValueError("User must specify a signal duration mode of class LeqDurationMode.")
 
         average_energy_over_equivalent_duration = total_energy_of_exposure / equivalent_duration
 
         return 10.0 * np.log10(average_energy_over_equivalent_duration / 20e-6 / 20e-6)
 
-    def overall_level(self, integration_time: float = None,
-                      weighting: WeightingFunctions = WeightingFunctions.unweighted):
+    def overall_level(
+            self, integration_time: float = None,
+            weighting: WeightingFunctions = WeightingFunctions.unweighted
+    ):
         """
         Integrate the levels within the waveform to generate the weighted level. This will permit different weighting
         functions to be applied before the calculation of the overall level.
 
         Parameters
         ----------
         integration_time: float, default: None - The amount of time that we will collect prior to determining the
@@ -2065,35 +2513,14 @@
             correlation_values = np.zeros(2 * lag_limit + 1)
             for i in range(0, 2 * lag_limit + 1):
                 correlation_values[i] = sum(ref_sig_pad[i:len(sig) + i] * sig)
             lags = np.arange(-lag_limit, lag_limit + 1)
 
         return np.max(correlation_values), lags[np.argmax(correlation_values)]
 
-    def resample(self, new_sample_rate: int):
-        """
-        This function resamples the waveform and returns a new object with the correct sample rate and sample count.
-        This function employs the resample function within scipy.signal to conduct the resampling.
-
-        Parameters
-        ----------
-        new_sample_rate: int - the new sample rate that we want to create a signal for
-
-        Returns
-        -------
-        Waveform - the new waveform object that contains the resampled data with the new sample rate.
-        """
-
-        #   Determine the ratio of the current sample rate to the new sample rate
-
-        sr_ratio = new_sample_rate / self.sample_rate
-
-        return Waveform(scipy.signal.resample(self.samples, int(np.floor(len(self.samples) * sr_ratio))),
-                        new_sample_rate, self.start_time)
-
     def concatenate(self, wfm):
         """
         This will create a new audio file that contains the data from the current Waveform and adds the samples from the
         new Waveform to the list and then returns a new object.
 
         Parameters
         ----------
@@ -2126,18 +2553,18 @@
         """
 
         warnings.warn(
             message='waveform.add not yet tested. Use at your own risk.'
         )
 
         if not isinstance(other, Waveform):
-            ValueError("You must provide a new Waveform object to add to this object.")
+            raise ValueError("You must provide a new Waveform object to add to this object.")
 
         if self.sample_rate != other.sample_rate:
-            ValueError("At this time, the two waveforms must possess the same sample rate to add them together")
+            raise ValueError("At this time, the two waveforms must possess the same sample rate to add them together")
 
         s0 = int(other.start_time * other.sample_rate)
         s1 = s0 + len(other.samples)
 
         return Waveform(self.samples[s0:s1] + other.samples, self.sample_rate, self.start_time)
 
     def __sub__(self, other):
@@ -2145,11 +2572,13 @@
         This function subtracts another Waveform object from the current object and returns the value as a new
         Waveform. If the start times, durations, or sample rates are not equal then the function returns a ValueError
 
         """
 
         if self.start_time != other.start_time or self.duration != other.duration or self.sample_rate != \
                 other.sample_rate:
-            raise ValueError("The meta-data of these two waveforms is inconsistent making it impossible to know how "
-                             "to subtract the information in the pressures.")
+            raise ValueError(
+                "The meta-data of these two waveforms is inconsistent making it impossible to know how "
+                "to subtract the information in the pressures."
+            )
 
         return Waveform(self.samples - other.samples, self.sample_rate, self.start_time, False)
```

### Comparing `PyTimbre-0.6.9/src/pytimbre/yin.py` & `PyTimbre-0.7.1/src/pytimbre/yin.py`

 * *Files identical despite different names*

