# Comparing `tmp/audclas-0.0.3.tar.gz` & `tmp/audclas-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audclas-0.0.3.tar", last modified: Tue Apr 18 22:17:39 2023, max compression
+gzip compressed data, was "audclas-0.0.4.tar", last modified: Wed Apr 19 05:44:54 2023, max compression
```

## Comparing `audclas-0.0.3.tar` & `audclas-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:17:39.942272 audclas-0.0.3/
--rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 audclas-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      600 2023-04-18 22:17:39.941275 audclas-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      131 2023-04-18 21:46:05.000000 audclas-0.0.3/README.md
--rw-rw-rw-   0        0        0      575 2023-04-18 22:17:05.000000 audclas-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-18 22:17:39.943269 audclas-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-18 22:17:39.872599 audclas-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-18 22:17:39.883164 audclas-0.0.3/src/audclas/
-drwxrwxrwx   0        0        0        0 2023-04-18 22:17:39.936764 audclas-0.0.3/src/audclas/modules/
--rw-rw-rw-   0        0        0     5541 2023-04-17 07:23:46.000000 audclas-0.0.3/src/audclas/modules/audio_mini_encoder.py
--rw-rw-rw-   0        0        0      809 2023-04-17 07:24:37.000000 audclas-0.0.3/src/audclas/modules/checkpoint.py
--rw-rw-rw-   0        0        0     4105 2023-04-18 14:21:32.000000 audclas-0.0.3/src/audclas/modules/dataset.py
--rw-rw-rw-   0        0        0     8390 2023-04-17 07:25:35.000000 audclas-0.0.3/src/audclas/modules/diffusion.py
--rw-rw-rw-   0        0        0    10164 2023-04-17 07:28:12.000000 audclas-0.0.3/src/audclas/modules/stft.py
--rw-rw-rw-   0        0        0     3136 2023-04-18 22:09:18.000000 audclas-0.0.3/src/audclas/tortoise_audio_classifier.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:17:39.920223 audclas-0.0.3/src/audclas.egg-info/
--rw-rw-rw-   0        0        0      600 2023-04-18 22:17:39.000000 audclas-0.0.3/src/audclas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-04-18 22:17:39.000000 audclas-0.0.3/src/audclas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:17:39.000000 audclas-0.0.3/src/audclas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-18 22:17:39.000000 audclas-0.0.3/src/audclas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 22:17:39.000000 audclas-0.0.3/src/audclas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.566156 audclas-0.0.4/
+-rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 audclas-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      600 2023-04-19 05:44:54.564567 audclas-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      131 2023-04-18 21:46:05.000000 audclas-0.0.4/README.md
+-rw-rw-rw-   0        0        0      575 2023-04-19 05:44:25.000000 audclas-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 05:44:54.566156 audclas-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.426619 audclas-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.455786 audclas-0.0.4/src/audclas/
+drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.561572 audclas-0.0.4/src/audclas/modules/
+-rw-rw-rw-   0        0        0     5541 2023-04-17 07:23:46.000000 audclas-0.0.4/src/audclas/modules/audio_mini_encoder.py
+-rw-rw-rw-   0        0        0      809 2023-04-17 07:24:37.000000 audclas-0.0.4/src/audclas/modules/checkpoint.py
+-rw-rw-rw-   0        0        0     4105 2023-04-18 14:21:32.000000 audclas-0.0.4/src/audclas/modules/dataset.py
+-rw-rw-rw-   0        0        0     8390 2023-04-17 07:25:35.000000 audclas-0.0.4/src/audclas/modules/diffusion.py
+-rw-rw-rw-   0        0        0    10164 2023-04-17 07:28:12.000000 audclas-0.0.4/src/audclas/modules/stft.py
+-rw-rw-rw-   0        0        0     3153 2023-04-19 05:43:42.000000 audclas-0.0.4/src/audclas/tortoise_audio_classifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.497290 audclas-0.0.4/src/audclas.egg-info/
+-rw-rw-rw-   0        0        0      600 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/top_level.txt
```

### Comparing `audclas-0.0.3/LICENSE` & `audclas-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audclas-0.0.3/PKG-INFO` & `audclas-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audclas
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package that uses extracted audio classification model from neonbjb/DL-Art-School - for filtering fine audio files.
 Author-email: Shmart <szprytnyd@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `audclas-0.0.3/pyproject.toml` & `audclas-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "audclas"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Shmart", email="szprytnyd@gmail.com" },
 ]
 description = "Package that uses extracted audio classification model from neonbjb/DL-Art-School - for filtering fine audio files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `audclas-0.0.3/src/audclas/modules/audio_mini_encoder.py` & `audclas-0.0.4/src/audclas/modules/audio_mini_encoder.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.3/src/audclas/modules/checkpoint.py` & `audclas-0.0.4/src/audclas/modules/checkpoint.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.3/src/audclas/modules/dataset.py` & `audclas-0.0.4/src/audclas/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.3/src/audclas/modules/diffusion.py` & `audclas-0.0.4/src/audclas/modules/diffusion.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.3/src/audclas/modules/stft.py` & `audclas-0.0.4/src/audclas/modules/stft.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.3/src/audclas/tortoise_audio_classifier.py` & `audclas-0.0.4/src/audclas/tortoise_audio_classifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,28 +45,30 @@
         dataset = AudioFolderDataset(audio_dir)
         data_loader = DataLoader(dataset, batch_size, shuffle=False, num_workers=os.cpu_count() - 1)
         def callback():
             try:
                 for batch in data_loader:
                     max_len = max(batch['samples'])
                     batch['clip'] = batch['clip'][:, :max_len].cuda()
-                    if torch.cuda.is_available():
-                        batch['clip'] = batch['clip'].cuda()
 
                     no_hifreq_data, labels = self.classify_batch(batch)
 
                     yield [(batch['path'][b], to_label(labels[b])) for b in range(labels.size(0)) if not no_hifreq_data[b]]
                         
             except:
                 print("Exception encountered. Will ignore and continue. Exception info follows.")
         return callback, len(data_loader)
     
     def classify_batch(self, batch):
         with torch.no_grad():
-            clips = batch['clip']
+            if torch.cuda.is_available():
+                clips = batch['clip'].cuda()
+            else:
+                clips = batch['clip']
+                
             mels = self.stft.mel_spectrogram(clips)
 
             def get_spec_mags(clip):
                 stft = torch.stft(clip, n_fft=22000, hop_length=1024, return_complex=True)
                 stft = stft[0, -2000:, :]
                 return (stft.real ** 2 + stft.imag ** 2).sqrt()
```

### Comparing `audclas-0.0.3/src/audclas.egg-info/PKG-INFO` & `audclas-0.0.4/src/audclas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audclas
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package that uses extracted audio classification model from neonbjb/DL-Art-School - for filtering fine audio files.
 Author-email: Shmart <szprytnyd@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

