# Comparing `tmp/neetbox-0.1.513.tar.gz` & `tmp/neetbox-0.1.514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neetbox-0.1.513.tar", max compression
+gzip compressed data, was "neetbox-0.1.514.tar", max compression
```

## Comparing `neetbox-0.1.513.tar` & `neetbox-0.1.514.tar`

### file list

```diff
@@ -1,47 +1,46 @@
--rw-r--r--   0        0        0     1067 2023-04-18 02:55:46.703036 neetbox-0.1.513/LICENSE
--rw-r--r--   0        0        0      397 2023-04-18 02:55:46.703036 neetbox-0.1.513/README.md
--rw-r--r--   0        0        0     2827 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/cli/__init__.py
--rw-r--r--   0        0        0     2910 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/cli/parse.py
--rw-r--r--   0        0        0     1154 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/config/__init__.py
--rw-r--r--   0        0        0     1390 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/config/_config.py
--rw-r--r--   0        0        0       66 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/core/__init__.py
--rw-r--r--   0        0        0     5874 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/core/registry.py
--rw-r--r--   0        0        0     2984 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/__init__.py
--rw-r--r--   0        0        0      872 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/_apis.py
--rw-r--r--   0        0        0     2161 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/_daemon.py
--rw-r--r--   0        0        0     3086 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/_daemon_client.py
--rw-r--r--   0        0        0     3226 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/daemon/_win_service.py
--rw-r--r--   0        0        0      337 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/__init__.py
--rw-r--r--   0        0        0     1182 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/engine.py
--rw-r--r--   0        0        0     3962 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/environment/hardware.py
--rw-r--r--   0        0        0     1748 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/environment/platform.py
--rw-r--r--   0        0        0     8536 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/integrations/resource.py
--rw-r--r--   0        0        0      313 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/__init__.py
--rw-r--r--   0        0        0     2106 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/_colorama.py
--rw-r--r--   0        0        0    12181 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/ansiregular.flf
--rw-r--r--   0        0        0    12181 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/ansishadow.flf
--rw-r--r--   0        0        0    11585 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/isometrixc2.flf
--rw-r--r--   0        0        0    23112 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/nscripts.flf
--rw-r--r--   0        0        0    21669 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/flfs/nvscript.flf
--rw-r--r--   0        0        0     3921 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/formatting.py
--rw-r--r--   0        0        0    18762 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/logging/logger.py
--rw-r--r--   0        0        0      241 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/pipeline/__init__.py
--rw-r--r--   0        0        0      299 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/pipeline/_pipe.py
--rw-r--r--   0        0        0     5167 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/pipeline/_signal_and_slot.py
--rw-r--r--   0        0        0        0 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/plotting/__init__.py
--rw-r--r--   0        0        0     4922 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/plotting/plot.py
--rw-r--r--   0        0        0      108 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/__init__.py
--rw-r--r--   0        0        0     5636 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/arch/canny.py
--rw-r--r--   0        0        0     6703 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/arch/cnn.py
--rw-r--r--   0        0        0     2400 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/arch/kernels.py
--rw-r--r--   0        0        0     2699 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/arch/mask_boundary_finder.py
--rw-r--r--   0        0        0     3678 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/nlp.py
--rw-r--r--   0        0        0     4702 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/torch/profile.py
--rw-r--r--   0        0        0       78 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/__init__.py
--rw-r--r--   0        0        0     2705 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/_package.py
--rw-r--r--   0        0        0     1019 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/format.py
--rw-r--r--   0        0        0     2303 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/framing.py
--rw-r--r--   0        0        0     1238 2023-04-18 02:55:46.707036 neetbox-0.1.513/neetbox/utils/mvc.py
--rw-r--r--   0        0        0     1271 2023-04-18 02:55:46.707036 neetbox-0.1.513/pyproject.toml
--rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 neetbox-0.1.513/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-19 04:05:41.060662 neetbox-0.1.514/LICENSE
+-rw-r--r--   0        0        0      397 2023-04-19 04:05:41.060662 neetbox-0.1.514/README.md
+-rw-r--r--   0        0        0     2827 2023-04-19 04:05:41.064662 neetbox-0.1.514/neetbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 04:05:41.064662 neetbox-0.1.514/neetbox/cli/__init__.py
+-rw-r--r--   0        0        0     2910 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/cli/parse.py
+-rw-r--r--   0        0        0     1154 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/config/__init__.py
+-rw-r--r--   0        0        0     1390 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/config/_config.py
+-rw-r--r--   0        0        0       66 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/core/__init__.py
+-rw-r--r--   0        0        0     5874 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/core/registry.py
+-rw-r--r--   0        0        0     2984 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/__init__.py
+-rw-r--r--   0        0        0      872 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/_apis.py
+-rw-r--r--   0        0        0     2161 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/_daemon.py
+-rw-r--r--   0        0        0     3086 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/_daemon_client.py
+-rw-r--r--   0        0        0     3226 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/daemon/_win_service.py
+-rw-r--r--   0        0        0      337 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/__init__.py
+-rw-r--r--   0        0        0     1182 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/engine.py
+-rw-r--r--   0        0        0     3924 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/environment/hardware.py
+-rw-r--r--   0        0        0     1748 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/environment/platform.py
+-rw-r--r--   0        0        0     8870 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/integrations/resource.py
+-rw-r--r--   0        0        0      313 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/__init__.py
+-rw-r--r--   0        0        0    12181 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/ansiregular.flf
+-rw-r--r--   0        0        0    12181 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/ansishadow.flf
+-rw-r--r--   0        0        0    11585 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/isometrixc2.flf
+-rw-r--r--   0        0        0    23112 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/nscripts.flf
+-rw-r--r--   0        0        0    21669 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/flfs/nvscript.flf
+-rw-r--r--   0        0        0     2526 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/formatting.py
+-rw-r--r--   0        0        0    18871 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/logging/logger.py
+-rw-r--r--   0        0        0      241 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/pipeline/__init__.py
+-rw-r--r--   0        0        0      299 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/pipeline/_pipe.py
+-rw-r--r--   0        0        0     5167 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/pipeline/_signal_and_slot.py
+-rw-r--r--   0        0        0        0 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/plotting/__init__.py
+-rw-r--r--   0        0        0     4922 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/plotting/plot.py
+-rw-r--r--   0        0        0      108 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/__init__.py
+-rw-r--r--   0        0        0     5636 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/arch/canny.py
+-rw-r--r--   0        0        0     6703 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/arch/cnn.py
+-rw-r--r--   0        0        0     2400 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/arch/kernels.py
+-rw-r--r--   0        0        0     2699 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/arch/mask_boundary_finder.py
+-rw-r--r--   0        0        0     3678 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/nlp.py
+-rw-r--r--   0        0        0     4702 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/torch/profile.py
+-rw-r--r--   0        0        0       78 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/__init__.py
+-rw-r--r--   0        0        0     2705 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/_package.py
+-rw-r--r--   0        0        0     1019 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/format.py
+-rw-r--r--   0        0        0     2303 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/framing.py
+-rw-r--r--   0        0        0     1238 2023-04-19 04:05:41.068662 neetbox-0.1.514/neetbox/utils/mvc.py
+-rw-r--r--   0        0        0     1239 2023-04-19 04:05:41.068662 neetbox-0.1.514/pyproject.toml
+-rw-r--r--   0        0        0     1620 1970-01-01 00:00:00.000000 neetbox-0.1.514/PKG-INFO
```

### Comparing `neetbox-0.1.513/LICENSE` & `neetbox-0.1.514/LICENSE`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/__init__.py` & `neetbox-0.1.514/neetbox/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/cli/parse.py` & `neetbox-0.1.514/neetbox/cli/parse.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/config/__init__.py` & `neetbox-0.1.514/neetbox/config/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/config/_config.py` & `neetbox-0.1.514/neetbox/config/_config.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/core/registry.py` & `neetbox-0.1.514/neetbox/core/registry.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/daemon/__init__.py` & `neetbox-0.1.514/neetbox/daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/daemon/_apis.py` & `neetbox-0.1.514/neetbox/daemon/_apis.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/daemon/_daemon.py` & `neetbox-0.1.514/neetbox/daemon/_daemon.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/daemon/_daemon_client.py` & `neetbox-0.1.514/neetbox/daemon/_daemon_client.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/daemon/_win_service.py` & `neetbox-0.1.514/neetbox/daemon/_win_service.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/integrations/engine.py` & `neetbox-0.1.514/neetbox/integrations/engine.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/integrations/environment/hardware.py` & `neetbox-0.1.514/neetbox/integrations/environment/hardware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# gputil = ">=1.4"
-# psutil = ">=5.0"
 # -*- coding: utf-8 -*-
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230413
```

### Comparing `neetbox-0.1.513/neetbox/integrations/environment/platform.py` & `neetbox-0.1.514/neetbox/integrations/environment/platform.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/integrations/resource.py` & `neetbox-0.1.514/neetbox/integrations/resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,39 @@
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230315
 
 from random import random
 import os
 from neetbox.utils import pkg
-assert pkg.is_installed('numpy', try_install_if_not=True)
+
+assert pkg.is_installed("numpy", try_install_if_not=True)
 import numpy as np
 import threading
 from neetbox.logging import logger
 from neetbox.integrations import engine
+from typing import Iterable
 from typing import Dict
 import pathlib
-import urllib.request
-from tqdm import tqdm
+import signal
+from functools import partial
+from urllib.request import urlopen
+from concurrent.futures import ThreadPoolExecutor
+from threading import Event
 from typing import List, Union, Dict, Any
+from rich.progress import track
+from rich.progress import (
+    BarColumn,
+    DownloadColumn,
+    Progress,
+    TaskID,
+    TextColumn,
+    TimeRemainingColumn,
+    TransferSpeedColumn,
+)
 
 
 _loader_pool: Dict[
     str, "ResourceLoader"
 ] = dict()  # all ResourceLoaders are stored here
 
 
@@ -68,29 +83,29 @@
             raise Exception("another scanning requested during the previous one.")
         self._ready = False
 
         def can_match(path: pathlib.Path):
             if not path.is_file():
                 return False
             for file_type in self._file_types:
-                if path.match('*.' + file_type):
+                if path.match("*." + file_type):
                     return True
             return False
 
         def perform_scan():
-            glob_str = '**/*' if self._scan_sub_dirs else "*"
+            glob_str = "**/*" if self._scan_sub_dirs else "*"
             if not verbose:  # do not output
                 self.file_path_list = [
                     str(path)
                     for path in pathlib.Path(self.path).glob(glob_str)
                     if can_match(path)
                 ]
             else:
                 self.file_path_list = []
-                for path in tqdm(pathlib.Path(self.path).glob(glob_str)):
+                for path in pathlib.Path(self.path).glob(glob_str):
                     if can_match(path):
                         self.file_path_list.append(path)
             self._ready = True
             if not self._initialized:
                 self._initialized = True
             logger.ok(
                 f"Resource loader '{self.path}' ready with {len(self._file_types)} file types({len(self.file_path_list)} files)."
@@ -110,20 +125,27 @@
         if not self._ready:
             raise Exception("not ready.")
         if type(index) is int:
             return self.file_path_list[index]
 
 
 class ImagesLoader(ResourceLoader):
-    
-    def __init__(self, folder, file_types=["png", "jpg"], sub_dirs=True, async_scan=False, verbose=False):
-        pkg.is_installed('PIL', try_install_if_not='pillow')
+    def __init__(
+        self,
+        folder,
+        file_types=["png", "jpg"],
+        sub_dirs=True,
+        async_scan=False,
+        verbose=False,
+    ):
+        pkg.is_installed("PIL", try_install_if_not="pillow")
         from PIL import Image
+
         super().__init__(folder, file_types, sub_dirs, async_scan, verbose)
-        
+
     def get_random_image(self):
         rand_img_path = self.file_path_list[int(random() * len(self.file_path_list))]
         image = Image.open(rand_img_path).convert("RGB")
         return image
 
     def get_random_images(self, howmany=1):
         assert howmany < len(self.file_path_list)
@@ -157,33 +179,62 @@
 
     # todo to_dataset
 
 
 def download(
     urls: Union[str, List[str], Dict[str, str]],
     filenames: Union[str, List[str]] = None,
-    overwrite=True,
-    retry=3,
-    verbose=True,
+    max_workers=4,
 ):
     """download both online and local files from urls
 
     Example: download('')
 
     Args:
         urls (Union[str, List[str], Dict[str, str]]): single str to download from url; list of strs to download from urls; dict(filename:url) to download urls and rename them to filenames
         filenames (Union[str, List[str]], optional): str to rename the downloaded file; list of strs to rename downloaded files; None means no rename. Defaults to None.
         overwrite Bool: whether to skip exist files. Default to True.
         retry (int, optional): retries when error occures. Defaults to 3.
         verbose (bool, optional): tell what happening in output. Defaults to True.
-
-    Returns:
-        _type_: _description_
     """
+    progress = Progress(
+        TextColumn("[bold blue]{task.fields[filename]}", justify="right"),
+        BarColumn(bar_width=None),
+        "[progress.percentage]{task.percentage:>3.1f}%",
+        "•",
+        DownloadColumn(),
+        "•",
+        TransferSpeedColumn(),
+        "•",
+        TimeRemainingColumn(),
+    )
+
+    done_event = Event()
+
+    def handle_sigint(signum, frame):
+        done_event.set()
+
+    signal.signal(signal.SIGINT, handle_sigint)
+
+    def copy_url(task_id: TaskID, url: str, path: str) -> None:
+        """Copy data from a url to a local file."""
+        response = urlopen(url)
+        # This will break if the response doesn't contain content length
+        progress.update(task_id, total=int(response.info()["Content-length"]))
+        with open(path, "wb") as dest_file:
+            progress.start_task(task_id)
+            for data in iter(partial(response.read, 32768), b""):
+                dest_file.write(data)
+                progress.update(task_id, advance=len(data))
+                if done_event.is_set():
+                    return
+        logger.log(f"Downloaded {path}.")
+
     assert type(urls) in [str, list, dict], "unkown format of url"
+
     if type(urls) is str:
         assert (
             filenames is None
             or type(filenames) is str
             or (type(filenames) is list and len(filenames) == 1)
         ), "num of urls and filenames mismatch"
         urls = [
@@ -203,49 +254,14 @@
             filenames
         ), "num of urls and filenames mismatch"
 
         urls = {filenames[i]: urls[i] for i in range(len(urls))}
 
     logger.log(f"Downloading {len(urls)} file(s)...")
 
-    if verbose:
-        outer_pbar = tqdm(total=len(urls), desc=f"Overall process")
-
-    _reporthook = None
-    _results = []
-    for fname, furl in tqdm(urls.items()):
-        if fname and os.path.isfile(fname):
-            if not overwrite:
-                _results.append((fname,None))
-                logger.log(
-                    f"File {fname} already exists. If you want to redownload it, try to pass 'overwrite=True'"
-                )
-                continue
-        if verbose:
-            inner_pbar = tqdm(total=100, leave=False, desc=f"Currently downloading")
-
-            def reporthook(p1, p2, p3):
-                inner_pbar.total = p3
-                inner_pbar.n = p1 * p2
-                inner_pbar.refresh()
-
-            _reporthook = reporthook
-            outer_pbar.update(1)
-        retry = 1 if not retry else retry
-        while retry:
-            try:
-                res = urllib.request.urlretrieve(
-                    url=furl, filename=fname, reporthook=_reporthook
-                )
-                _results.append(res)
-                break
-            except:
-                retry -= 1
-                logger.err(f"Download interrupt. {retry} retry(s) remaining.")
-                if not retry:
-                    raise RuntimeError(f"Download failed after retries")
-    results = [fname for fname, reqmsg in _results]
-    if not len(results):
-        results = None
-    if len(results) == 1:
-        results = results[0]
-    return results
+    with progress:
+        with ThreadPoolExecutor(max_workers=max_workers) as pool:
+            for fname, url in urls.items():
+                filename = url.split("/")[-1]
+                dest_path = os.path.join(fname)
+                task_id = progress.add_task("download", filename=filename, start=False)
+                pool.submit(copy_url, task_id, url, dest_path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `neetbox-0.1.513/neetbox/logging/flfs/ansiregular.flf` & `neetbox-0.1.514/neetbox/logging/flfs/ansiregular.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/logging/flfs/ansishadow.flf` & `neetbox-0.1.514/neetbox/logging/flfs/ansishadow.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/logging/flfs/isometrixc2.flf` & `neetbox-0.1.514/neetbox/logging/flfs/isometrixc2.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/logging/flfs/nscripts.flf` & `neetbox-0.1.514/neetbox/logging/flfs/nscripts.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/logging/flfs/nvscript.flf` & `neetbox-0.1.514/neetbox/logging/flfs/nvscript.flf`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/logging/formatting.py` & `neetbox-0.1.514/neetbox/logging/formatting.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,121 +2,87 @@
 #
 # Author: GavinGong aka VisualDust
 # URL:    https://gong.host
 # Date:   20230318
 
 import warnings
 import os
-from colorama import Fore, Back, Style
 from random import random
-from ._colorama import *
-from typing import Optional, Union
-
-# todo use @cache when migrate to python 3.9
-def get_supported_colors():
-    supported_colors = []
-    for color in AnsiColor:
-        supported_colors.append(color)
-    return supported_colors
-
-def get_supported_styles():
-    supported_styles = []
-    for style in AnsiStyle:
-        supported_styles.append(style)
-    return supported_styles
+from typing import Optional
 
 
 class LogStyle:
+    @classmethod
+    def get_supported_colors(cls):
+        return ["red", "green", "blue", "cyan", "yellow", "magenta"]
+
+    @classmethod
+    def get_supported_text_style(cls):
+        return ["bold", "italic", "blink"]
+
     def __init__(self) -> None:
-        self.fore: Optional[AnsiColor] = None
-        self.back: Optional[AnsiColor] = None
+        self.color: Optional[str] = None
         self.prefix: str = ""
-        self.pattern = ""  # todo default pattern
+        self.text_style: Optional[str] = None
         self.datetime_format: str = "%Y-%m-%d-%H:%M:%S"
         self.with_identifier: bool = True
         self.trace_level = 3
         self.with_datetime: bool = True
         self.split_char_cmd = " > "
         self.split_char_identity = "/"
         self.split_char_txt = " | "
-        
-    def parse(self,pattern:str):
+
+    def parse(self, pattern: str):
         # todo
         pass
 
-    def set_foreground_color(self, color: AnsiColor):
+    def set_color(self, color: str):
         self.fore = color
         return self
 
-    def set_background_color(self, color: AnsiColor):
-        self.back = color
+    def set_text_style(self, text_style: str):
+        self.text_style = text_style
         return self
 
     def set_prefix(self, prefix: str):
         self.prefix = prefix
         return self
 
     def set_datetime_format(self, datetime_format: str):
         self.datetime_format = datetime_format
         return self
 
     def randcolor(self):
-        colors = get_supported_colors()
-        split_index = int(random() * len(colors) / 2)
-        index_offset = -1
-        while index_offset == 0:  # fore and back shoud not be the same
-            index_offset = int(random() * len(colors) / 2)
-        self.back = colors[(split_index + index_offset) % len(colors)]
-        self.fore = colors[(split_index - index_offset) % len(colors)]
+        colors = LogStyle.get_supported_colors()
+        # split_index = int(random() * len(colors) / 2)
+        # index_offset = -1
+        # while index_offset == 0:  # fore and back shoud not be the same
+        #     index_offset = int(random() * len(colors) / 2)
+        # self.back = colors[(split_index + index_offset) % len(colors)]
+        # self.fore = colors[(split_index - index_offset) % len(colors)]
+        self.color = colors[int(random() * len(colors))]
         return self
 
 
 DEFAULT_STYLE = LogStyle()
 
 
-def colored(
-    text, color_foreground: Optional[Union[AnsiColor,str]] = None, color_background: Optional[Union[AnsiColor,str]] = None
-):
-    """_summary_
-
-    Args:
-        text (str): original raw string
-        color (AnsiColor): which color
-
-    Raises: Nothing
-
-    Returns:
-        str: colored string
-    """
-    if "ANSI_COLORS_DISABLED" in os.environ or "NO_COLOR" in os.environ:
-        warnings.warn(
-            "Notice that current running environment does not supported colored text. NEETBOX logging facilities will still work but may not output colored text in console."
-        )
-
-    # Resolving foreground color
-    if color_foreground:
-        if type(color_foreground) is AnsiColor:
-            color_foreground = color_foreground.value
-        if hasattr(Fore, color_foreground.upper()):
-            text = getattr(Fore, color_foreground.upper()) + text + Fore.RESET
-        else:
-            raise ValueError("Wrong color was inputed in colored func.")
-
-    # Resolving background color
-    if color_background:
-        if type(color_background) is AnsiColor:
-            color_background = color_background.value
-        color_background = color_background.value
-        if hasattr(Back, color_background.upper()):
-            text = getattr(Back, color_background.upper()) + text + Fore.RESET
-        else:
-            raise ValueError("Wrong color was inputed in colored func.")
-
-    return text
-
-
-def colored_by_style(text, style: LogStyle):
-    if style.fore is not None:  # applied foreground color
-        return colored(text, color_foreground=style.fore)
-    if style.back is not None:  # applied background color
-        return colored(text, color_background=style.back)
-    return text  # nothing applied
+def styled_text(text, style: LogStyle):
+    attributes = []
+    if style.color:
+        attributes.append(style.color)
+    if style.text_style:
+        attributes.append(style.text_style)
+    render_stack = []
+    _prefix = ""
+    _postfix = ""
+    while len(attributes):
+        attr = attributes.pop(-1)
+        _prefix += f"[{attr}]"
+        render_stack.append(attr)
+    while len(render_stack):
+        _postfix += f"[/{render_stack.pop(-1)}]"
+    return f"{_prefix}{text}{_postfix}"
+
+
+def colored_text(text: str, color):
+    return f"[{color}]{text}[/{color}]"
```

### Comparing `neetbox-0.1.513/neetbox/logging/logger.py` & `neetbox-0.1.514/neetbox/logging/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from neetbox.utils import format
 from neetbox.logging.formatting import *
 from inspect import isclass, iscoroutinefunction, isgeneratorfunction
 import functools
 import pathlib
 from random import randint
 from typing import *
+from rich import print as rprint
+from rich.panel import Panel
 
 
 class LogLevel(Enum):
     ALL = 4
     INFO = 3
     DEBUG = 2
     WARNING = 1
@@ -301,91 +303,91 @@
                 id_seq.append(_caller_identity.func_name)  # skip for jupyters
             for i in range(len(id_seq)):
                 if len(_whom) != 0:
                     _whom += _style.split_char_identity
                 _whom += id_seq[i]
 
         # converting args into a single string
-        _message = ""
+        _pure_str_message = ""
         for msg in content:
-            _message += str(msg) + " "
+            _pure_str_message += str(msg) + " "
 
         # perform log
         if into_stdout:
-            print(
+            rprint(
                 _prefix
                 + _datetime
                 + _style.split_char_cmd * min(len(_datetime), 1)
-                + colored_by_style(_whom, style=_style)
-                + _style.split_char_cmd * min(len(_whom), 1)
-                + _message
+                + styled_text(_whom, style=_style)
+                + _style.split_char_cmd * min(len(_whom), 1),
+                _pure_str_message,
             )
         if into_file and self.file_writer:
             self.file_writer.write(
                 _prefix
                 + _datetime
                 + _style.split_char_txt * min(len(_datetime), 1)
                 + _whom
                 + _style.split_char_txt * min(len(_whom), 1)
-                + _message
+                + _pure_str_message
                 + "\n"
             )
         return self
 
     def ok(self, *message, flag="OK"):
         if _global_log_level >= LogLevel.INFO:
             self.log(
                 *message,
-                prefix=f"[{colored(flag, AnsiColor.GREEN)}]",
+                prefix=f"[{colored_text(flag, 'green')}]",
                 into_file=False,
                 traceback=3,
             )
             self.log(*message, prefix=flag, into_stdout=False, traceback=3)
         return self
 
     def debug(self, *message, flag=f"DEBUG"):
         if _global_log_level >= LogLevel.DEBUG:
             self.log(
                 *message,
-                prefix=f"[{colored(flag, AnsiColor.CYAN)}]",
+                prefix=f"[{colored_text(flag, 'cyan')}]",
                 into_file=False,
                 traceback=3,
             )
             self.log(*message, prefix=flag, into_stdout=False, traceback=3)
         return self
 
     def info(self, *message, flag="INFO"):
         if _global_log_level >= LogLevel.INFO:
             self.log(
                 *message,
-                prefix=f"[{colored(flag, AnsiColor.WHITE)}]",
+                prefix=f"[{colored_text(flag, 'white')}]",
                 into_file=False,
                 traceback=3,
             )
             self.log(*message, prefix=flag, into_stdout=False, traceback=3)
         return self
 
     def warn(self, *message, flag="WARNING"):
         if _global_log_level >= LogLevel.WARNING:
             self.log(
                 *message,
-                prefix=f"[{colored(flag, AnsiColor.YELLOW)}]",
+                prefix=f"[{colored_text(flag, 'yellow')}]",
                 into_file=False,
                 traceback=3,
             )
             self.log(*message, prefix=flag, into_stdout=False, traceback=3)
         return self
 
     def err(self, err, flag="ERROR", reraise=False):
         if type(err) is not Exception:
             err = RuntimeError(str(err))
         if _global_log_level >= LogLevel.ERROR:
             self.log(
                 str(err),
-                prefix=f"[{colored(flag,AnsiColor.RED)}]",
+                prefix=f"[{colored_text(flag,'red')}]",
                 into_file=False,
                 traceback=3,
             )
             self.log(str(err), prefix=flag, into_stdout=False, traceback=3)
         if reraise:
             raise err
         return self
@@ -489,15 +491,16 @@
                         FigletFont.installFonts(f"res/flfs/{font}.flf")
                     except:
                         self.err("Could not install font {font}. Fallback to default.")
                         font = None
                 else:
                     font = file[0]
         f = Figlet(font)
-        self.log(f.renderText(text), with_datetime=False, with_identifier=False)
+        rendered_text = f.renderText(text)
+        rprint(Panel.fit(f"{rendered_text}", border_style="green"))
         return self
 
     def skip_lines(self, line_cnt=1):
         """Let the logger log some empty lines
 
         Args:
             line_cnt (int, optional): how many empty line. Defaults to 1.
```

### Comparing `neetbox-0.1.513/neetbox/pipeline/_signal_and_slot.py` & `neetbox-0.1.514/neetbox/pipeline/_signal_and_slot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/plotting/plot.py` & `neetbox-0.1.514/neetbox/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/torch/arch/canny.py` & `neetbox-0.1.514/neetbox/torch/arch/canny.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/torch/arch/cnn.py` & `neetbox-0.1.514/neetbox/torch/arch/cnn.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/torch/arch/kernels.py` & `neetbox-0.1.514/neetbox/torch/arch/kernels.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/torch/arch/mask_boundary_finder.py` & `neetbox-0.1.514/neetbox/torch/arch/mask_boundary_finder.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/torch/nlp.py` & `neetbox-0.1.514/neetbox/torch/nlp.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/torch/profile.py` & `neetbox-0.1.514/neetbox/torch/profile.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/utils/_package.py` & `neetbox-0.1.514/neetbox/utils/_package.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/utils/format.py` & `neetbox-0.1.514/neetbox/utils/format.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/utils/framing.py` & `neetbox-0.1.514/neetbox/utils/framing.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/neetbox/utils/mvc.py` & `neetbox-0.1.514/neetbox/utils/mvc.py`

 * *Files identical despite different names*

### Comparing `neetbox-0.1.513/pyproject.toml` & `neetbox-0.1.514/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neetbox"
-version = "0.1.513"
+version = "0.1.514"
 description = "NEETBox contains useless CV code snippets."
 license = "MIT"
 authors = ["VisualDust <gavin@gong.host>"]
 maintainers = [
     "VisualDust <gavin@gong.host>",
     "PommesPeter <me@pommespeter.space>",
     "PaperCube <imzhy@hotmail.com>"
@@ -29,16 +29,14 @@
 # [[tool.poetry.source]]
 # name = "pypi"
 # url = "https://pypi.org/simple"
 # default = true
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
-tqdm = ">=4"
-colorama = ">=0.3"
 toml = ">0.10"
 injector = ">=0.20"
 setproctitle = "^1.3.2"
 rich = "^13.3.4"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.0.0"
```

### Comparing `neetbox-0.1.513/PKG-INFO` & `neetbox-0.1.514/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neetbox
-Version: 0.1.513
+Version: 0.1.514
 Summary: NEETBox contains useless CV code snippets.
 Home-page: https://neetbox.550w.host
 License: MIT
 Keywords: computer vision,tools,logging
 Author: VisualDust
 Author-email: gavin@gong.host
 Maintainer: VisualDust
@@ -20,20 +20,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: Utilities
-Requires-Dist: colorama (>=0.3)
 Requires-Dist: injector (>=0.20)
 Requires-Dist: rich (>=13.3.4,<14.0.0)
 Requires-Dist: setproctitle (>=1.3.2,<2.0.0)
 Requires-Dist: toml (>0.10)
-Requires-Dist: tqdm (>=4)
 Project-URL: Repository, https://github.com/visualDust/neetbox
 Description-Content-Type: text/markdown
 
 # NEETBox contains use~~ful~~less tiny deeplearning code snippets
 
 ~~一个自产自销的仓库~~
```

