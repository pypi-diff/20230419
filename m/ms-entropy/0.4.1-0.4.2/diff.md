# Comparing `tmp/ms_entropy-0.4.1.tar.gz` & `tmp/ms_entropy-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.4.1.tar", last modified: Mon Mar 27 21:09:55 2023, max compression
+gzip compressed data, was "ms_entropy-0.4.2.tar", last modified: Wed Apr 19 04:58:36 2023, max compression
```

## Comparing `ms_entropy-0.4.1.tar` & `ms_entropy-0.4.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.021646 ms_entropy-0.4.1/
--rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.4.1/LICENSE
--rw-rw-r--   0 yli       (1000) yli       (1000)       48 2023-03-24 01:05:23.000000 ms_entropy-0.4.1/MANIFEST.in
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-03-27 21:09:55.021646 ms_entropy-0.4.1/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     3175 2023-03-27 19:21:41.000000 ms_entropy-0.4.1/README.md
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.017646 ms_entropy-0.4.1/manuscript/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.017646 ms_entropy-0.4.1/manuscript/src/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.017646 ms_entropy-0.4.1/manuscript/src/mimas/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.017646 ms_entropy-0.4.1/manuscript/src/mimas/spectra/
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.017646 ms_entropy-0.4.1/manuscript/src/mimas/spectra/fast_entropy_search/
--rw-rw-r--   0 yli       (1000) yli       (1000)     4939 2023-03-24 01:05:23.000000 ms_entropy-0.4.1/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.017646 ms_entropy-0.4.1/manuscript/src/mimas/spectra/similarity/
--rw-rw-r--   0 yli       (1000) yli       (1000)     5950 2023-03-24 01:05:23.000000 ms_entropy-0.4.1/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     5153 2023-03-24 01:05:23.000000 ms_entropy-0.4.1/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     6002 2023-03-24 01:05:23.000000 ms_entropy-0.4.1/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.017646 ms_entropy-0.4.1/manuscript/src/mimas/spectra/spectral_entropy_published/
--rw-rw-r--   0 yli       (1000) yli       (1000)    16189 2023-03-24 01:05:23.000000 ms_entropy-0.4.1/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.021646 ms_entropy-0.4.1/ms_entropy/
--rw-rw-r--   0 yli       (1000) yli       (1000)      107 2023-03-24 01:05:23.000000 ms_entropy-0.4.1/ms_entropy/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    19651 2023-03-27 20:38:57.000000 ms_entropy-0.4.1/ms_entropy/flash_entropy_search.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    33392 2023-03-27 19:39:45.000000 ms_entropy-0.4.1/ms_entropy/flash_entropy_search_core.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     4317 2023-03-25 18:55:15.000000 ms_entropy-0.4.1/ms_entropy/tools.py
--rw-rw-r--   0 yli       (1000) yli       (1000)   958514 2023-03-25 19:23:59.000000 ms_entropy-0.4.1/ms_entropy/tools_cython.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     7974 2023-03-25 18:55:15.000000 ms_entropy-0.4.1/ms_entropy/tools_cython.pyx
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-03-27 21:09:55.021646 ms_entropy-0.4.1/ms_entropy.egg-info/
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-03-27 21:09:54.000000 ms_entropy-0.4.1/ms_entropy.egg-info/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)      751 2023-03-27 21:09:54.000000 ms_entropy-0.4.1/ms_entropy.egg-info/SOURCES.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-03-27 21:09:54.000000 ms_entropy-0.4.1/ms_entropy.egg-info/dependency_links.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       44 2023-03-27 21:09:54.000000 ms_entropy-0.4.1/ms_entropy.egg-info/requires.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-03-27 21:09:54.000000 ms_entropy-0.4.1/ms_entropy.egg-info/top_level.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.4.1/pyproject.toml
--rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-03-27 21:09:55.021646 ms_entropy-0.4.1/setup.cfg
--rw-rw-r--   0 yli       (1000) yli       (1000)     1371 2023-03-27 21:09:41.000000 ms_entropy-0.4.1/setup.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/
+-rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.4.2/LICENSE
+-rw-rw-r--   0 yli       (1000) yli       (1000)       48 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/MANIFEST.in
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.4.2/README.md
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.599015 ms_entropy-0.4.2/manuscript/
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.599015 ms_entropy-0.4.2/manuscript/src/
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.599015 ms_entropy-0.4.2/manuscript/src/mimas/
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.599015 ms_entropy-0.4.2/manuscript/src/mimas/spectra/
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/manuscript/src/mimas/spectra/fast_entropy_search/
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4939 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5950 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5153 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     6002 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/manuscript/src/mimas/spectra/spectral_entropy_published/
+-rw-rw-r--   0 yli       (1000) yli       (1000)    16189 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/ms_entropy/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      107 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/ms_entropy/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    20202 2023-04-19 04:56:46.000000 ms_entropy-0.4.2/ms_entropy/flash_entropy_search.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    33392 2023-03-27 19:39:45.000000 ms_entropy-0.4.2/ms_entropy/flash_entropy_search_core.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4317 2023-04-19 04:48:23.000000 ms_entropy-0.4.2/ms_entropy/tools.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)   958514 2023-03-25 19:23:59.000000 ms_entropy-0.4.2/ms_entropy/tools_cython.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     7974 2023-03-25 18:55:15.000000 ms_entropy-0.4.2/ms_entropy/tools_cython.pyx
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/ms_entropy.egg-info/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)      751 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       44 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/requires.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-04-19 04:58:36.000000 ms_entropy-0.4.2/ms_entropy.egg-info/top_level.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.4.2/pyproject.toml
+-rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-04-19 04:58:36.603015 ms_entropy-0.4.2/setup.cfg
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1371 2023-04-19 04:51:23.000000 ms_entropy-0.4.2/setup.py
```

### Comparing `ms_entropy-0.4.1/LICENSE` & `ms_entropy-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/README.md` & `ms_entropy-0.4.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Flash Entropy Search
 
 This repository contains the source code for Flash Entropy Search, a method using entropy similarity for fast searching mass spectrometry spectral library.
 
-You can find the benchmark results and the original code used in our manuscript under the `manuscript` folder.
+You can find the benchmark results and the original code used in our manuscript under the `manuscript` folder here: [manuscript](https://github.com/YuanyueLi/FlashEntropySearch/tree/main/manuscript).
 
 We are continuously improving the code, and the latest version of the code can be found under the `ms_entropy` folder.
 
 You can find a brief introduction below, or you can find a more detailed documentation here: [https://flashentropysearch.readthedocs.io](https://flashentropysearch.readthedocs.io/).
 
 ## In brief
```

### Comparing `ms_entropy-0.4.1/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx` & `ms_entropy-0.4.2/manuscript/src/mimas/spectra/fast_entropy_search/entropy_search_core_fast.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx` & `ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_match_spectra.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx` & `ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_spectral_entropy.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx` & `ms_entropy-0.4.2/manuscript/src/mimas/spectra/similarity/tools_spectrum.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx` & `ms_entropy-0.4.2/manuscript/src/mimas/spectra/spectral_entropy_published/tools_fast.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/ms_entropy/flash_entropy_search.py` & `ms_entropy-0.4.2/ms_entropy/flash_entropy_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,16 @@
 
     def build_index(self,
                     all_spectra_list: list = None,
                     max_indexed_mz: float = 1500.00005,
                     precursor_ions_removal_da: float = 1.6,
                     noise_threshold=0.01,
                     min_ms2_difference_in_da: float = 0.05,
-                    max_peak_num: int = None):
+                    max_peak_num: int = None,
+                    clean_spectra: bool = True):
         """
         Set the library spectra for entropy search.
 
         The `all_spectra_list` must be a list of dictionaries, with each dictionary containing at least two keys: "precursor_mz" and "peaks". 
         The dictionary should be in the format of {"precursor_mz": precursor_mz, "peaks": peaks, ...}, All keys in the dictionary, except "peaks,"
         will be saved as the metadata and can be accessed using the  __getitem__ function (e.g. entropy_search[0] returns the metadata for the
         first spectrum in the library).
@@ -206,32 +207,36 @@
         :param max_indexed_mz: The maximum m/z value that will be indexed. Default is 1500.00005.
         :param precursor_ions_removal_da:   The ions with m/z larger than precursor_mz - precursor_ions_removal_da will be removed.
                                             Default is 1.6.
         :param noise_threshold: The intensity threshold for removing the noise peaks. The peaks with intensity smaller than noise_threshold * max(intensity)
                                 will be removed. Default is 0.01.
         :param min_ms2_difference_in_da:    The minimum difference between two peaks in the MS/MS spectrum. Default is 0.05.
         :param max_peak_num:    The maximum number of peaks in the MS/MS spectrum. Default is None, which means no limit.
+        :param clean_spectra:   If True, the spectra will be cleaned before indexing. Default is True. If ALL spectra in the library are pre-cleaned with the
+                                function `clean_spectrum` or `clean_spectrum_for_search`, set this parameter to False. ALWAYS set this parameter to true if
+                                the spectra are not pre-prepossessed with the function `clean_spectrum` or `clean_spectrum_for_search`.
 
         :return:    If the all_spectra_list is provided, this function will return the sorted spectra list.
         """
 
         # Sort the spectra by the precursor m/z.
         all_sorted_spectra_list = sorted(all_spectra_list, key=lambda x: x["precursor_mz"])
 
         # Clean the spectra, and collect the non-empty spectra
         all_spectra_list = []
         all_metadata_list = []
         for spec in all_sorted_spectra_list:
             # Clean the peaks
-            spec["peaks"] = self.clean_spectrum_for_search(peaks=spec["peaks"],
-                                                           precursor_mz=spec["precursor_mz"],
-                                                           precursor_ions_removal_da=precursor_ions_removal_da,
-                                                           noise_threshold=noise_threshold,
-                                                           min_ms2_difference_in_da=min_ms2_difference_in_da,
-                                                           max_peak_num=max_peak_num)
+            if clean_spectra:
+                spec["peaks"] = self.clean_spectrum_for_search(peaks=spec["peaks"],
+                                                               precursor_mz=spec["precursor_mz"],
+                                                               precursor_ions_removal_da=precursor_ions_removal_da,
+                                                               noise_threshold=noise_threshold,
+                                                               min_ms2_difference_in_da=min_ms2_difference_in_da,
+                                                               max_peak_num=max_peak_num)
             if len(spec["peaks"]) > 0:
                 all_spectra_list.append(spec)
                 metadata = copy.copy(spec)
                 metadata.pop("peaks")
                 all_metadata_list.append(pickle.dumps(metadata))
 
         # Extract precursor m/z array
@@ -335,8 +340,7 @@
 
         This function is not required when you only use one thread to search the MS/MS spectra.
         When use multiple threads, this function is also not required but highly recommended, as it avoids the memory copy and saves a lot of memory and time.
 
         :return:    None
         """
         self.entropy_search.save_memory_for_multiprocessing()
-
```

### Comparing `ms_entropy-0.4.1/ms_entropy/flash_entropy_search_core.py` & `ms_entropy-0.4.2/ms_entropy/flash_entropy_search_core.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/ms_entropy/tools.py` & `ms_entropy-0.4.2/ms_entropy/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     3. Centroid the spectrum by merging the peaks within the +/- min_ms2_difference_in_da, sort the result spectrum by m/z.
 
     4. Remove the peaks with intensity less than the noise_threshold * maximum (intensity).
 
     5. Keep the top max_peak_num peaks, and remove the rest peaks.
     
-    5. Normalize the intensity to sum to 1.
+    6. Normalize the intensity to sum to 1.
 
     :param spectrum: The spectrum, a 2D numpy array with shape (n, 2), the first column is m/z, the second column is intensity.
     :param min_mz: The minimum m/z to keep, if None, all the peaks will be kept. Default is None.
     :param max_mz: The maximum m/z to keep, if None, all the peaks will be kept. Default is None.
     :param noise_threshold: The noise threshold, peaks have intensity lower than
                             noise_threshold * maximum (intensity) will be removed.
                             If None, all the peaks will be kept.
```

### Comparing `ms_entropy-0.4.1/ms_entropy/tools_cython.c` & `ms_entropy-0.4.2/ms_entropy/tools_cython.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/ms_entropy/tools_cython.pyx` & `ms_entropy-0.4.2/ms_entropy/tools_cython.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.4.2/ms_entropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.4.1/setup.py` & `ms_entropy-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 
 os.environ['CFLAGS'] = '-O3 -Wno-cpp -Wno-unused-function'
 
 setup(
     name='ms_entropy',
-    version='0.4.1',
+    version='0.4.2',
     license='Apache License 2.0',
     author='Yuanyue Li',
     url='https://github.com/YuanyueLi/SpectralEntropy',
     packages=['ms_entropy'],
     python_requires='>=3.8',
     install_requires=[
         "numpy >= 1.18",
```

