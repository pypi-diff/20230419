# Comparing `tmp/audclas-0.0.4.tar.gz` & `tmp/audclas-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audclas-0.0.4.tar", last modified: Wed Apr 19 05:44:54 2023, max compression
+gzip compressed data, was "audclas-0.0.5.tar", last modified: Wed Apr 19 15:41:14 2023, max compression
```

## Comparing `audclas-0.0.4.tar` & `audclas-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.566156 audclas-0.0.4/
--rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 audclas-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      600 2023-04-19 05:44:54.564567 audclas-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      131 2023-04-18 21:46:05.000000 audclas-0.0.4/README.md
--rw-rw-rw-   0        0        0      575 2023-04-19 05:44:25.000000 audclas-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-19 05:44:54.566156 audclas-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.426619 audclas-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.455786 audclas-0.0.4/src/audclas/
-drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.561572 audclas-0.0.4/src/audclas/modules/
--rw-rw-rw-   0        0        0     5541 2023-04-17 07:23:46.000000 audclas-0.0.4/src/audclas/modules/audio_mini_encoder.py
--rw-rw-rw-   0        0        0      809 2023-04-17 07:24:37.000000 audclas-0.0.4/src/audclas/modules/checkpoint.py
--rw-rw-rw-   0        0        0     4105 2023-04-18 14:21:32.000000 audclas-0.0.4/src/audclas/modules/dataset.py
--rw-rw-rw-   0        0        0     8390 2023-04-17 07:25:35.000000 audclas-0.0.4/src/audclas/modules/diffusion.py
--rw-rw-rw-   0        0        0    10164 2023-04-17 07:28:12.000000 audclas-0.0.4/src/audclas/modules/stft.py
--rw-rw-rw-   0        0        0     3153 2023-04-19 05:43:42.000000 audclas-0.0.4/src/audclas/tortoise_audio_classifier.py
-drwxrwxrwx   0        0        0        0 2023-04-19 05:44:54.497290 audclas-0.0.4/src/audclas.egg-info/
--rw-rw-rw-   0        0        0      600 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      415 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 05:44:54.000000 audclas-0.0.4/src/audclas.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.683608 audclas-0.0.5/
+-rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 audclas-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1816 2023-04-19 15:41:14.683608 audclas-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1347 2023-04-19 15:34:55.000000 audclas-0.0.5/README.md
+-rw-rw-rw-   0        0        0      575 2023-04-19 15:29:23.000000 audclas-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-19 15:41:14.685137 audclas-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.648785 audclas-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.655734 audclas-0.0.5/src/audclas/
+drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.682100 audclas-0.0.5/src/audclas/modules/
+-rw-rw-rw-   0        0        0     5541 2023-04-17 07:23:46.000000 audclas-0.0.5/src/audclas/modules/audio_mini_encoder.py
+-rw-rw-rw-   0        0        0      809 2023-04-17 07:24:37.000000 audclas-0.0.5/src/audclas/modules/checkpoint.py
+-rw-rw-rw-   0        0        0     4105 2023-04-18 14:21:32.000000 audclas-0.0.5/src/audclas/modules/dataset.py
+-rw-rw-rw-   0        0        0     8390 2023-04-17 07:25:35.000000 audclas-0.0.5/src/audclas/modules/diffusion.py
+-rw-rw-rw-   0        0        0    10164 2023-04-17 07:28:12.000000 audclas-0.0.5/src/audclas/modules/stft.py
+-rw-rw-rw-   0        0        0     3157 2023-04-19 15:27:25.000000 audclas-0.0.5/src/audclas/tortoise_audio_classifier.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:41:14.675372 audclas-0.0.5/src/audclas.egg-info/
+-rw-rw-rw-   0        0        0     1816 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      415 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-19 15:41:14.000000 audclas-0.0.5/src/audclas.egg-info/top_level.txt
```

### Comparing `audclas-0.0.4/LICENSE` & `audclas-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audclas-0.0.4/pyproject.toml` & `audclas-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "audclas"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Shmart", email="szprytnyd@gmail.com" },
 ]
 description = "Package that uses extracted audio classification model from neonbjb/DL-Art-School - for filtering fine audio files."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `audclas-0.0.4/src/audclas/modules/audio_mini_encoder.py` & `audclas-0.0.5/src/audclas/modules/audio_mini_encoder.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.4/src/audclas/modules/checkpoint.py` & `audclas-0.0.5/src/audclas/modules/checkpoint.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.4/src/audclas/modules/dataset.py` & `audclas-0.0.5/src/audclas/modules/dataset.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.4/src/audclas/modules/diffusion.py` & `audclas-0.0.5/src/audclas/modules/diffusion.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.4/src/audclas/modules/stft.py` & `audclas-0.0.5/src/audclas/modules/stft.py`

 * *Files identical despite different names*

### Comparing `audclas-0.0.4/src/audclas/tortoise_audio_classifier.py` & `audclas-0.0.5/src/audclas/tortoise_audio_classifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def __call__(self, file_path):
         batch_item = AudioFolderDataset.get_batch_item(file_path)
         batch = default_collate([batch_item])
         _, labels = self.classify_batch(batch)
         return to_label(labels[0])
 
-    def prepare_classify_dir(self, audio_dir: str, batch_size=16):
+    def prepare_classify_dir_job(self, audio_dir: str, batch_size=16):
         dataset = AudioFolderDataset(audio_dir)
         data_loader = DataLoader(dataset, batch_size, shuffle=False, num_workers=os.cpu_count() - 1)
         def callback():
             try:
                 for batch in data_loader:
                     max_len = max(batch['samples'])
                     batch['clip'] = batch['clip'][:, :max_len].cuda()
```

