# Comparing `tmp/histoprep-2.0.1.tar.gz` & `tmp/histoprep-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histoprep-2.0.1.tar", max compression
+gzip compressed data, was "histoprep-2.0.2.tar", max compression
```

## Comparing `histoprep-2.0.1.tar` & `histoprep-2.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1064 2023-02-21 10:11:24.560924 histoprep-2.0.1/LICENSE
--rw-r--r--   0        0        0     4498 2023-04-13 12:06:06.845518 histoprep-2.0.1/README.md
--rw-r--r--   0        0        0      208 2023-04-12 16:08:51.730543 histoprep-2.0.1/histoprep/__init__.py
--rw-r--r--   0        0        0    12824 2023-04-13 11:58:17.436440 histoprep-2.0.1/histoprep/_backend.py
--rw-r--r--   0        0        0    12916 2023-04-13 11:57:10.830117 histoprep-2.0.1/histoprep/_cli.py
--rw-r--r--   0        0        0     2632 2023-04-12 15:47:00.972683 histoprep-2.0.1/histoprep/_data.py
--rw-r--r--   0        0        0    27360 2023-04-13 11:56:18.924307 histoprep-2.0.1/histoprep/_reader.py
--rw-r--r--   0        0        0      907 2023-04-13 12:20:57.494642 histoprep-2.0.1/histoprep/functional/__init__.py
--rw-r--r--   0        0        0     1021 2023-04-12 15:40:13.626407 histoprep-2.0.1/histoprep/functional/_check.py
--rw-r--r--   0        0        0     1297 2023-04-12 16:23:34.711207 histoprep-2.0.1/histoprep/functional/_concurrent.py
--rw-r--r--   0        0        0     5400 2023-04-12 15:45:03.944588 histoprep-2.0.1/histoprep/functional/_dearray.py
--rw-r--r--   0        0        0     4305 2023-04-12 15:45:01.032486 histoprep-2.0.1/histoprep/functional/_draw.py
--rw-r--r--   0        0        0     2641 2023-04-13 12:19:15.958972 histoprep-2.0.1/histoprep/functional/_images.py
--rw-r--r--   0        0        0      410 2023-04-12 16:02:13.168518 histoprep-2.0.1/histoprep/functional/_level.py
--rw-r--r--   0        0        0     1881 2023-04-13 12:19:50.132209 histoprep-2.0.1/histoprep/functional/_mean_std.py
--rw-r--r--   0        0        0     5490 2023-04-13 12:20:09.164897 histoprep-2.0.1/histoprep/functional/_metrics.py
--rw-r--r--   0        0        0     5476 2023-04-12 15:44:49.396078 histoprep-2.0.1/histoprep/functional/_normalize.py
--rw-r--r--   0        0        0     8211 2023-04-13 12:21:53.940676 histoprep-2.0.1/histoprep/functional/_tiles.py
--rw-r--r--   0        0        0     4766 2023-04-12 15:45:57.762471 histoprep-2.0.1/histoprep/functional/_tissue.py
--rw-r--r--   0        0        0      421 2023-04-13 12:05:05.503101 histoprep-2.0.1/histoprep/utils/__init__.py
--rw-r--r--   0        0        0     5870 2023-04-13 11:58:49.445556 histoprep-2.0.1/histoprep/utils/_normalize.py
--rw-r--r--   0        0        0    12291 2023-04-13 12:16:52.593762 histoprep-2.0.1/histoprep/utils/_process.py
--rw-r--r--   0        0        0     4891 2023-04-12 15:58:31.116776 histoprep-2.0.1/histoprep/utils/_torch.py
--rw-r--r--   0        0        0      724 2023-04-13 12:23:06.887300 histoprep-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     5637 1970-01-01 00:00:00.000000 histoprep-2.0.1/setup.py
--rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 histoprep-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-13 12:39:17.917382 histoprep-2.0.2/LICENSE
+-rw-r--r--   0        0        0     4498 2023-04-13 12:39:17.917382 histoprep-2.0.2/README.md
+-rw-r--r--   0        0        0      208 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/__init__.py
+-rw-r--r--   0        0        0    12824 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/_backend.py
+-rw-r--r--   0        0        0    12916 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/_cli.py
+-rw-r--r--   0        0        0     2632 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/_data.py
+-rw-r--r--   0        0        0    27360 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/_reader.py
+-rw-r--r--   0        0        0      907 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/__init__.py
+-rw-r--r--   0        0        0     1021 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/_check.py
+-rw-r--r--   0        0        0     1297 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/_concurrent.py
+-rw-r--r--   0        0        0     5400 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/_dearray.py
+-rw-r--r--   0        0        0     4305 2023-04-13 12:39:17.921382 histoprep-2.0.2/histoprep/functional/_draw.py
+-rw-r--r--   0        0        0     2641 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_images.py
+-rw-r--r--   0        0        0      410 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_level.py
+-rw-r--r--   0        0        0     1881 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_mean_std.py
+-rw-r--r--   0        0        0     5490 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_metrics.py
+-rw-r--r--   0        0        0     5476 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_normalize.py
+-rw-r--r--   0        0        0     8211 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_tiles.py
+-rw-r--r--   0        0        0     4766 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/functional/_tissue.py
+-rw-r--r--   0        0        0      421 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/utils/__init__.py
+-rw-r--r--   0        0        0     5870 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/utils/_normalize.py
+-rw-r--r--   0        0        0    12291 2023-04-13 12:39:17.925382 histoprep-2.0.2/histoprep/utils/_process.py
+-rw-r--r--   0        0        0     5008 2023-04-19 08:36:38.807381 histoprep-2.0.2/histoprep/utils/_torch.py
+-rw-r--r--   0        0        0      724 2023-04-19 08:38:19.227324 histoprep-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5637 1970-01-01 00:00:00.000000 histoprep-2.0.2/setup.py
+-rw-r--r--   0        0        0     5310 1970-01-01 00:00:00.000000 histoprep-2.0.2/PKG-INFO
```

### Comparing `histoprep-2.0.1/LICENSE` & `histoprep-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/README.md` & `histoprep-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/_backend.py` & `histoprep-2.0.2/histoprep/_backend.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/_cli.py` & `histoprep-2.0.2/histoprep/_cli.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/_data.py` & `histoprep-2.0.2/histoprep/_data.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/_reader.py` & `histoprep-2.0.2/histoprep/_reader.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/__init__.py` & `histoprep-2.0.2/histoprep/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_check.py` & `histoprep-2.0.2/histoprep/functional/_check.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_concurrent.py` & `histoprep-2.0.2/histoprep/functional/_concurrent.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_dearray.py` & `histoprep-2.0.2/histoprep/functional/_dearray.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_draw.py` & `histoprep-2.0.2/histoprep/functional/_draw.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_images.py` & `histoprep-2.0.2/histoprep/functional/_images.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_mean_std.py` & `histoprep-2.0.2/histoprep/functional/_mean_std.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_metrics.py` & `histoprep-2.0.2/histoprep/functional/_metrics.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_normalize.py` & `histoprep-2.0.2/histoprep/functional/_normalize.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_tiles.py` & `histoprep-2.0.2/histoprep/functional/_tiles.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/functional/_tissue.py` & `histoprep-2.0.2/histoprep/functional/_tissue.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/utils/_normalize.py` & `histoprep-2.0.2/histoprep/utils/_normalize.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/utils/_process.py` & `histoprep-2.0.2/histoprep/utils/_process.py`

 * *Files identical despite different names*

### Comparing `histoprep-2.0.1/histoprep/utils/_torch.py` & `histoprep-2.0.2/histoprep/utils/_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 ERROR_PYTORCH = "Could not import torch, make sure it has been installed!"
 ERROR_LENGTH_MISMATCH = "Path length ({}) does not match label length ({})."
 ERROR_TILE_SHAPE = "Tile shape must be defined to create a cache array."
 
 
 class SlideReaderDataset(Dataset):
-    """Torch dataset yielding tile images from reader (requires `PyTorch`)."""
+    """Torch dataset yielding tile images and `xywh`-coordinates from reader (requires
+    `PyTorch`)."""
 
     def __init__(
         self,
         reader: SlideReader,
         coordinates: Iterator[tuple[int, int, int, int]],
         level: int = 0,
         transform: Optional[Callable[[np.ndarray], Any]] = None,
@@ -64,15 +65,16 @@
         tile = self.reader.read_region(xywh, level=self.level)
         if self.transform is not None:
             tile = self.transform(tile)
         return tile, np.array(xywh)
 
 
 class TileImageDataset(Dataset):
-    """Torch dataset yielding tile images from paths (requires `PyTorch`)."""
+    """Torch dataset yielding tile images, image paths and optional labels (requires
+    `PyTorch`)."""
 
     def __init__(
         self,
         paths: list[Union[str, Path]],
         *,
         labels: Optional[list[str]] = None,
         transform: Optional[Callable[[np.ndarray], Any]] = None,
@@ -113,14 +115,16 @@
             )
 
     def __len__(self) -> int:
         return len(self.paths)
 
     def __getitem__(self, index: int) -> tuple[Union[np.ndarray, Any], str]:
         path = self.paths[index]
+        if isinstance(path, Path):
+            path = str(path)
         if self._use_cache:
             if index not in self._cached_indices:
                 self._cache_array[index] = np.array(Image.open(path))
                 self._cached_indices.add(index)
             image = self._cache_array[index]
         else:
             image = np.array(Image.open(path))
```

### Comparing `histoprep-2.0.1/pyproject.toml` & `histoprep-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "histoprep"
-version = "2.0.1"
+version = "2.0.2"
 description = "Read and process histological slide images with python!"
 authors = ["jopo666 <jopo@birdlover.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 HistoPrep = 'histoprep._cli:cut_slides'
```

### Comparing `histoprep-2.0.1/setup.py` & `histoprep-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tqdm']
 
 entry_points = \
 {'console_scripts': ['HistoPrep = histoprep._cli:cut_slides']}
 
 setup_kwargs = {
     'name': 'histoprep',
-    'version': '2.0.1',
+    'version': '2.0.2',
     'description': 'Read and process histological slide images with python!',
     'long_description': '<div align="center">\n\n# HistoPrep\nPreprocessing large medical images for machine learning made easy!\n\n<p align="center">\n  <a href="#description">Description</a> •\n  <a href="#installation">Installation</a> •\n  <a href="#usage">Usage</a> •\n  <a href="https://jopo666.github.io/HistoPrep/">API Documentation</a> •\n  <a href="#citation">Citation</a>\n</p>\n\n</div>\n\n## Description\n\n`HistoPrep` makes is easy to prepare your histological slide images for deep\nlearning models. You can easily cut large slide images into smaller tiles and then\npreprocess those tiles (remove tiles with shitty tissue, finger  marks etc).\n\n## Installation \n\nInstall [`OpenSlide`](https://openslide.org/download/) on your system and then install histoprep with `pip`!\n\n```bash\npip install histoprep\n```\n\n## Usage\n\nTypical workflow for training deep learning models with histological images is the\nfollowing:\n\n1. Cut each slide image into smaller tile images.\n2. Preprocess smaller tile images by removing tiles with bad tissue, staining artifacts.\n3. Overfit a pretrained ResNet50 model, report 100% validation accuracy and publish it\n   in [Nature](https://www.nature.com) like everyone else. \n\nWith `HistoPrep`, steps 1. and 2. are as easy as accidentally drinking too much at the\nresearch group christmas party and proceeding to work remotely until June.\n\nLet\'s start by cutting a slide from the\n[PANDA](https://www.kaggle.com/c/prostate-cancer-grade-assessment) kaggle challenge into\nsmall tiles. \n\n```python\nfrom histoprep import SlideReader\n\n# Read slide image.\nreader = SlideReader("./slides/slide_with_ink.jpeg")\n# Detect tissue.\nthreshold, tissue_mask = reader.get_tissue_mask(level=-1)\n# Extract overlapping tile coordinates with less than 50% background.\ntile_coordinates = reader.get_tile_coordinates(\n    tissue_mask, width=512, overlap=0.5, max_background=0.5\n)\n# Save tile images with image metrics for preprocessing.\ntile_metadata = reader.save_regions(\n    "./train_tiles/", tile_coordinates, threshold=threshold, save_metrics=True\n)\n```\n```\nslide_with_ink: 100%|██████████| 390/390 [00:01<00:00, 295.90it/s]\n```\n\nLet\'s take a look at the output and visualise the thumbnails.\n\n```bash\njopo666@~$ tree train_tiles\ntrain_tiles\n└── slide_with_ink\n    ├── metadata.parquet       # tile metadata\n    ├── properties.json        # tile properties\n    ├── thumbnail.jpeg         # thumbnail image\n    ├── thumbnail_tiles.jpeg   # thumbnail with tiles\n    ├── thumbnail_tissue.jpeg  # thumbnail of the tissue mask\n    └── tiles [390 entries exceeds filelimit, not opening dir]\n```\n\n![Prostate biopsy sample](images/thumbnail.jpeg)\n![Tissue mask](images/thumbnail_tissue.jpeg)\n![Thumbnail with tiles](images/thumbnail_tiles.jpeg)\n\nThat was easy, but it can be annoying to whip up a new python script every time you want\nto cut slides, and thus it is recommended to use the `HistoPrep` CLI program!\n\n```bash\n# Repeat the above code for all images in the PANDA dataset!\njopo666@~$ HistoPrep --input \'./train_images/*.tiff\' --output ./tiles --width 512 --overlap 0.5 --max-background 0.5\n```\n\nAs we can see from the above images, histological slide images often contain areas that\nwe would not like to include into our training data. Might seem like a daunting task but\nlet\'s try it out!\n\n\n```python\nfrom histoprep.utils import OutlierDetector\n\n# Let\'s wrap the tile metadata with a helper class.\ndetector = OutlierDetector(tile_metadata)\n# Cluster tiles based on image metrics.\nclusters = detector.cluster_kmeans(num_clusters=4, random_state=666)\n# Visualise first cluster.\nreader.get_annotated_thumbnail(\n    image=reader.read_level(-1), coordinates=detector.coordinates[clusters == 0]\n)\n```\n![Tiles in cluster 0](images/thumbnail_blue.jpeg)\n\nI said it was gonna be easy! Now we can mark tiles in cluster `0` as outliers and\nstart overfitting our neural network! This was a simple example but the same code can be\nused to cluster all several _million_ tiles extracted from the `PANDA` dataset and discard\noutliers simultaneously!\n\n## Citation\n\nIf you use `HistoPrep` to process the images for your publication, please cite the github repository.\n\n```\n@misc{histoprep,\n  author = {Pohjonen, Joona and Ariotta, Valeria},\n  title = {HistoPrep: Preprocessing large medical images for machine learning made easy!},\n  year = {2022},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {https://github.com/jopo666/HistoPrep},\n}\n```\n',
     'author': 'jopo666',
     'author_email': 'jopo@birdlover.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['histoprep',
 'histoprep.functional', 'histoprep.utils'] package_data = \ {'': ['*']}
 install_requires = \ ['aicspylibczi>=3,<4', 'matplotlib', 'mpire>=2.6,<3.0',
 'numpy', 'opencv-python-headless>=4,<5', 'openslide-python>=1.2,<2.0',
 'pillow>=9,<10', 'polars>=0.16,<0.17', 'rich-click>=1.6,<2.0', 'scikit-
 learn>=1,<2', 'tqdm'] entry_points = \ {'console_scripts': ['HistoPrep =
 histoprep._cli:cut_slides']} setup_kwargs = { 'name': 'histoprep', 'version':
-'2.0.1', 'description': 'Read and process histological slide images with
+'2.0.2', 'description': 'Read and process histological slide images with
 python!', 'long_description': '
  \n\n# HistoPrep\nPreprocessing large medical images for machine learning made
                                    easy!\n\n
   \n Description â¢\n Installation â¢\n Usage â¢\n API_Documentation â¢\n
                                   Citation\n
                                      \n\n
 \n\n## Description\n\n`HistoPrep` makes is easy to prepare your histological
```

### Comparing `histoprep-2.0.1/PKG-INFO` & `histoprep-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histoprep
-Version: 2.0.1
+Version: 2.0.2
 Summary: Read and process histological slide images with python!
 Author: jopo666
 Author-email: jopo@birdlover.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: histoprep Version: 2.0.1 Summary: Read and process
+Metadata-Version: 2.1 Name: histoprep Version: 2.0.2 Summary: Read and process
 histological slide images with python! Author: jopo666 Author-email:
 jopo@birdlover.com Requires-Python: >=3.9,<4.0 Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: aicspylibczi (>=3,<4) Requires-Dist: matplotlib
 Requires-Dist: mpire (>=2.6,<3.0) Requires-Dist: numpy Requires-Dist: opencv-
 python-headless (>=4,<5) Requires-Dist: openslide-python (>=1.2,<2.0) Requires-
```

