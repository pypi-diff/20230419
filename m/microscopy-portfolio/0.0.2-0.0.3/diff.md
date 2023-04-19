# Comparing `tmp/microscopy_portfolio-0.0.2.tar.gz` & `tmp/microscopy_portfolio-0.0.3.tar.gz`

## Comparing `microscopy_portfolio-0.0.2.tar` & `microscopy_portfolio-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/.copier-answers.yml
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/.github/dependabot.yml
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/.github/workflows/datasets_ci.yml
--rw-r--r--   0        0        0     8264 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/datasets/datasets.json
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/examples/example.ipynb
--rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/scripts/export_portfolio_to_json.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/src/microscopy_portfolio/__init__.py
--rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/src/microscopy_portfolio/denoiseg_datasets.py
--rw-r--r--   0        0        0     5579 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/src/microscopy_portfolio/denoising_datasets.py
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/src/microscopy_portfolio/portfolio.py
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/src/microscopy_portfolio/portfolio_entry.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/src/microscopy_portfolio/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/tests/test_denoiseg_datasets.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/tests/test_denoising_datasets.py
--rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/tests/test_portfolio.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/tests/test_portfolio_entry.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/tests/utils.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/.gitignore
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/LICENSE
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/README.md
--rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/.copier-answers.yml
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/.github/workflows/datasets_ci.yml
+-rw-r--r--   0        0        0     8848 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/datasets/datasets.json
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/examples/example.ipynb
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/scripts/download_and_examine.py
+-rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/scripts/export_portfolio_to_json.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/src/microscopy_portfolio/__init__.py
+-rw-r--r--   0        0        0     8506 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/src/microscopy_portfolio/denoiseg_datasets.py
+-rw-r--r--   0        0        0     7742 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/src/microscopy_portfolio/denoising_datasets.py
+-rw-r--r--   0        0        0    11273 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/src/microscopy_portfolio/portfolio.py
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/src/microscopy_portfolio/portfolio_entry.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/src/microscopy_portfolio/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/tests/test_denoiseg_datasets.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/tests/test_denoising_datasets.py
+-rw-r--r--   0        0        0     2804 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/tests/test_portfolio.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/tests/test_portfolio_entry.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/tests/utils.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/README.md
+-rw-r--r--   0        0        0     4513 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 microscopy_portfolio-0.0.3/PKG-INFO
```

### Comparing `microscopy_portfolio-0.0.2/.copier-answers.yml` & `microscopy_portfolio-0.0.3/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/.pre-commit-config.yaml` & `microscopy_portfolio-0.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/.github/workflows/ci.yml` & `microscopy_portfolio-0.0.3/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
       - name: Coverage
         uses: codecov/codecov-action@v3
 
   update_json:
     name: Update datasets summary
     needs: test
+    # run on PR so that we can check it out later
     if: success() && github.event_name == 'pull_request'
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       
       - name: Checkout PR
```

### Comparing `microscopy_portfolio-0.0.2/.github/workflows/datasets_ci.yml` & `microscopy_portfolio-0.0.3/.github/workflows/datasets_ci.yml`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/datasets/datasets.json` & `microscopy_portfolio-0.0.3/datasets/datasets.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9425%*

 * *Differences: {"'Denoising'": "{'N2V_SEM': {'License': 'CC-BY-4.0'}, 'N2V_RGB': {'License': 'CC-BY-4.0'}, "*

 * *                "'Flywing': {'License': 'CC-BY-4.0'}, 'Convallaria': OrderedDict([('URL', "*

 * *                "'https://cloud.mpi-cbg.de/index.php/s/BE8raMtHQlgLDF3/download'), ('Description', "*

 * *                "'Image of a convallaria flower (35x692x520 pixels).\\nThe image also comes with a "*

 * *                "defocused image in order to allow \\nestimating the noise distribution.'), "*

 * *                "('Citation',  […]*

```diff
@@ -61,37 +61,44 @@
             "Description": "A dataset depicting diverse and non-uniformly clustered nuclei in the mouse skull, consisting of 908 training and 160 validation patches. The test set counts 67 additional images",
             "File size": "160.0 MB",
             "License": "CC BY-SA 4.0",
             "URL": "https://zenodo.org/record/5157008/files/Mouse_n20.zip?download=1"
         }
     },
     "Denoising": {
+        "Convallaria": {
+            "Citation": "Krull, A., Vi\u010dar, T., Prakash, M., Lalit, M., & Jug, F. (2020). Probabilistic noise2void: Unsupervised content-aware denoising. Frontiers in Computer Science, 2, 5.",
+            "Description": "Image of a convallaria flower (35x692x520 pixels).\nThe image also comes with a defocused image in order to allow \nestimating the noise distribution.",
+            "File size": "344.0 MB",
+            "License": "CC-BY-4.0",
+            "URL": "https://cloud.mpi-cbg.de/index.php/s/BE8raMtHQlgLDF3/download"
+        },
         "Flywing": {
             "Citation": "Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, F.: Denoiseg: joint denoising and segmentation. In: European Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             "Description": "Image of a membrane-labeled fly wing (35x692x520 pixels).",
             "File size": "10.2 MB",
-            "License": "CC-BY",
+            "License": "CC-BY-4.0",
             "URL": "https://download.fht.org/jug/n2v/flywing-data.zip"
         },
         "N2V_BSD68": {
             "Citation": "D. Martin, C. Fowlkes, D. Tal and J. Malik, \"A database of human segmented natural images and its application to evaluating segmentation algorithms and measuring ecological statistics,\" Proceedings Eighth IEEE International Conference on Computer Vision. ICCV 2001, Vancouver, BC, Canada, 2001, pp. 416-423 vol.2, doi: 10.1109/ICCV.2001.937655.",
             "Description": "This dataset is taken from K. Zhang et al (TIP, 2017). \nIt consists of 400 gray-scale 180x180 images (cropped from the BSD dataset) and splitted between training and validation, and 68 gray-scale test images (BSD68).\nAll images were corrupted with Gaussian noise with standard deviation of 25 pixels. The test dataset contains the uncorrupted images as well.\nOriginal dataset: https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/bsds/",
             "File size": "875.0 MB",
             "License": "Unknown",
             "URL": "https://download.fht.org/jug/n2v/BSD68_reproducibility.zip"
         },
         "N2V_RGB": {
             "Citation": "A. Krull, T.-O. Buchholz and F. Jug, \"Noise2Void - Learning Denoising From Single Noisy Images,\" 2019 IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2019, pp. 2124-2132",
             "Description": "Banner of the CVPR 2019 conference with extra noise.",
             "File size": "10.4 MB",
-            "License": "CC0",
+            "License": "CC-BY-4.0",
             "URL": "https://download.fht.org/jug/n2v/RGB.zip"
         },
         "N2V_SEM": {
             "Citation": "T.-O. Buchholz, A. Krull, R. Shahidi, G. Pigino, G. J\u00e9kely, F. Jug, \"Content-aware image restoration for electron microscopy\", Methods Cell Biol 152, 277-289",
             "Description": "Cropped images from a SEM dataset from T.-O. Buchholz et al (Methods Cell Biol, 2020).",
             "File size": "13.0 MB",
-            "License": "CC-BY",
+            "License": "CC-BY-4.0",
             "URL": "https://download.fht.org/jug/n2v/SEM.zip"
         }
     }
 }
```

### Comparing `microscopy_portfolio-0.0.2/examples/example.ipynb` & `microscopy_portfolio-0.0.3/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/src/microscopy_portfolio/__init__.py` & `microscopy_portfolio-0.0.3/src/microscopy_portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/src/microscopy_portfolio/denoiseg_datasets.py` & `microscopy_portfolio-0.0.3/src/microscopy_portfolio/denoiseg_datasets.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/src/microscopy_portfolio/denoising_datasets.py` & `microscopy_portfolio-0.0.3/src/microscopy_portfolio/denoising_datasets.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 class N2V_BSD68(PortfolioEntry):
     """BSD68 dataset.
 
     Attributes
     ----------
     name (str): Name of the dataset.
     url (str): URL of the dataset.
+    file_name (str): Name of the downloaded file.
+    md5_hash (str): MD5 hash of the downloaded file.
     description (str): Description of the dataset.
     license (str): License of the dataset.
     citation (str): Citation to use when referring to the dataset.
     files (dict): Dictionary containing the files to download.
+    size (float): Size of the dataset in MB.
     """
 
     def __init__(self) -> None:
         super().__init__(
             name="N2V_BSD68",
             url="https://download.fht.org/jug/n2v/BSD68_reproducibility.zip",
             file_name="BSD68_reproducibility.zip",
@@ -54,29 +57,32 @@
 class N2V_SEM(PortfolioEntry):
     """SEM dataset.
 
     Attributes
     ----------
     name (str): Name of the dataset.
     url (str): URL of the dataset.
+    file_name (str): Name of the downloaded file.
+    md5_hash (str): MD5 hash of the downloaded file.
     description (str): Description of the dataset.
     license (str): License of the dataset.
     citation (str): Citation to use when referring to the dataset.
     files (dict): Dictionary containing the files to download.
+    size (float): Size of the dataset in MB.
     """
 
     def __init__(self) -> None:
         super().__init__(
             name="N2V_SEM",
             url="https://download.fht.org/jug/n2v/SEM.zip",
             file_name="SEM.zip",
             md5_hash="953a815333805a423b7019bd16cc3341",
             description="Cropped images from a SEM dataset from T.-O. Buchholz et al "
             "(Methods Cell Biol, 2020).",
-            license="CC-BY",
+            license="CC-BY-4.0",
             citation="T.-O. Buchholz, A. Krull, R. Shahidi, G. Pigino, G. Jékely, "
             'F. Jug, "Content-aware image restoration for electron '
             'microscopy", Methods Cell Biol 152, 277-289',
             files={
                 ".": ["train.tif", "validation.tif"],
             },
             size=13.0,
@@ -86,28 +92,31 @@
 class N2V_RGB(PortfolioEntry):
     """RGB dataset.
 
     Attributes
     ----------
     name (str): Name of the dataset.
     url (str): URL of the dataset.
+    file_name (str): Name of the downloaded file.
+    md5_hash (str): MD5 hash of the downloaded file.
     description (str): Description of the dataset.
     license (str): License of the dataset.
     citation (str): Citation to use when referring to the dataset.
     files (dict): Dictionary containing the files to download.
+    size (float): Size of the dataset in MB.
     """
 
     def __init__(self) -> None:
         super().__init__(
             name="N2V_RGB",
             url="https://download.fht.org/jug/n2v/RGB.zip",
             file_name="RGB.zip",
             md5_hash="ad80d2fee3ae0a93208687e30ad2b63a",
             description="Banner of the CVPR 2019 conference with extra noise.",
-            license="CC0",
+            license="CC-BY-4.0",
             citation='A. Krull, T.-O. Buchholz and F. Jug, "Noise2Void - Learning '
             'Denoising From Single Noisy Images," 2019 IEEE/CVF '
             "Conference on Computer Vision and Pattern Recognition (CVPR),"
             " 2019, pp. 2124-2132",
             files={
                 ".": ["longBeach.png"],
             },
@@ -118,29 +127,71 @@
 class Flywing(PortfolioEntry):
     """Flywing dataset.
 
     Attributes
     ----------
     name (str): Name of the dataset.
     url (str): URL of the dataset.
+    file_name (str): Name of the downloaded file.
+    md5_hash (str): MD5 hash of the downloaded file.
     description (str): Description of the dataset.
     license (str): License of the dataset.
     citation (str): Citation to use when referring to the dataset.
     files (dict): Dictionary containing the files to download.
+    size (float): Size of the dataset in MB.
     """
 
     def __init__(self) -> None:
         super().__init__(
             name="Flywing",
             url="https://download.fht.org/jug/n2v/flywing-data.zip",
             file_name="flywing-data.zip",
             md5_hash="769f4e265f8ab8ccea1893087df019da",
             description="Image of a membrane-labeled fly wing (35x692x520 pixels).",
-            license="CC-BY",
+            license="CC-BY-4.0",
             citation="Buchholz, T.O., Prakash, M., Schmidt, D., Krull, A., Jug, "
             "F.: Denoiseg: joint denoising and segmentation. In: European "
             "Conference on Computer Vision (ECCV). pp. 324-337. Springer (2020) 8, 9",
             files={
                 ".": ["flywing.tif"],
             },
             size=10.2,
         )
+
+
+class Convallaria(PortfolioEntry):
+    """Convallaria dataset.
+
+    Attributes
+    ----------
+    name (str): Name of the dataset.
+    url (str): URL of the dataset.
+    file_name (str): Name of the file to download.
+    md5_hash (str): MD5 hash of the file to download.
+    description (str): Description of the dataset.
+    license (str): License of the dataset.
+    citation (str): Citation to use when referring to the dataset.
+    files (dict): Dictionary containing the files to download.
+    size (float): Size of the dataset in MB.
+    """
+
+    def __init__(self) -> None:
+        super().__init__(
+            name="Convallaria",
+            url="https://cloud.mpi-cbg.de/index.php/s/BE8raMtHQlgLDF3/download",
+            file_name="Convallaria_diaphragm.zip",
+            md5_hash="7b8df3a83939decaede6753b8d38b52f",
+            description="Image of a convallaria flower (35x692x520 pixels).\n"
+            "The image also comes with a defocused image in order to allow \n"
+            "estimating the noise distribution.",
+            license="CC-BY-4.0",
+            citation="Krull, A., Vičar, T., Prakash, M., Lalit, M., & Jug, F. (2020). "
+            "Probabilistic noise2void: Unsupervised content-aware denoising. Frontiers"
+            " in Computer Science, 2, 5.",
+            files={
+                "Convallaria_diaphragm": [
+                    "20190520_tl_25um_50msec_05pc_488_130EM_Conv.tif",
+                    "20190726_tl_50um_500msec_wf_130EM_FD.tif",
+                ],
+            },
+            size=344.0,
+        )
```

### Comparing `microscopy_portfolio-0.0.2/src/microscopy_portfolio/portfolio.py` & `microscopy_portfolio-0.0.3/src/microscopy_portfolio/portfolio.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 from dataclasses import dataclass
 from json import JSONEncoder
 from pathlib import Path
 
 from .denoiseg_datasets import DSB2018, MouseNuclei, NoiseLevel, SegFlywing
-from .denoising_datasets import N2V_BSD68, N2V_RGB, N2V_SEM, Flywing
+from .denoising_datasets import N2V_BSD68, N2V_RGB, N2V_SEM, Convallaria, Flywing
 from .portfolio_entry import PortfolioEntry
 
 
 class IterablePortfolio:
     """Iterable portfolio class.
 
     Subclass this class and add PortfolioEntry objects as attributes.
@@ -284,21 +284,23 @@
 
     Attributes
     ----------
     N2V_BSD68 (N2V_BSD68): BSD68 dataset.
     N2V_SEM (N2V_SEM): SEM dataset.
     N2V_RGB (N2V_RGB): RGB dataset.
     flywing (Flywing): Flywing dataset.
+    Convallaria (Convallaria): Convallaria dataset.
     """
 
     def __init__(self) -> None:
         self._N2V_BSD68 = N2V_BSD68()
         self._N2V_SEM = N2V_SEM()
         self._N2V_RGB = N2V_RGB()
         self._flywing = Flywing()
+        self._Convallaria = Convallaria()
 
         super().__init__("Denoising")
 
     @property
     def N2V_BSD68(self) -> N2V_BSD68:
         """BSD68 dataset.
 
@@ -334,18 +336,29 @@
     @property
     def flywing(self) -> Flywing:
         """Flywing dataset.
 
         Returns
         -------
         Flywing
-        Flywing dataset.
+            Flywing dataset.
         """
         return self._flywing
 
+    @property
+    def Convallaria(self) -> Convallaria:
+        """Convallaria dataset.
+
+        Returns
+        -------
+        Convallaria
+            Convallaria dataset.
+        """
+        return self._Convallaria
+
 
 @dataclass
 class Portfolio:
     """Portfolio of datasets.
 
     Attributes
     ----------
```

### Comparing `microscopy_portfolio-0.0.2/src/microscopy_portfolio/portfolio_entry.py` & `microscopy_portfolio-0.0.3/src/microscopy_portfolio/portfolio_entry.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/tests/conftest.py` & `microscopy_portfolio-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/tests/test_denoiseg_datasets.py` & `microscopy_portfolio-0.0.3/tests/test_denoiseg_datasets.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/tests/test_denoising_datasets.py` & `microscopy_portfolio-0.0.3/tests/test_denoising_datasets.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/tests/test_portfolio.py` & `microscopy_portfolio-0.0.3/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/tests/test_portfolio_entry.py` & `microscopy_portfolio-0.0.3/tests/test_portfolio_entry.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/tests/utils.py` & `microscopy_portfolio-0.0.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/.gitignore` & `microscopy_portfolio-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/LICENSE` & `microscopy_portfolio-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/README.md` & `microscopy_portfolio-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/pyproject.toml` & `microscopy_portfolio-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microscopy_portfolio-0.0.2/PKG-INFO` & `microscopy_portfolio-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microscopy-portfolio
-Version: 0.0.2
+Version: 0.0.3
 Summary: A helper package to download example datasets used in various publications and deep-learning algorithms, including data featured in N2V, P(P)N2V, DivNoising, HDN, EmbedSeg, etc.
 Project-URL: homepage, https://github.com/juglab-torch/microscopy-portfolio
 Project-URL: repository, https://github.com/juglab-torch/microscopy-portfolio
 Author-email: Joran Deschamps <joran.deschamps@fht.org>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

