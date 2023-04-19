# Comparing `tmp/sdgrate-0.2.2.tar.gz` & `tmp/sdgrate-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdgrate-0.2.2.tar", last modified: Fri Apr 14 18:27:58 2023, max compression
+gzip compressed data, was "sdgrate-0.2.3.tar", last modified: Wed Apr 19 18:52:30 2023, max compression
```

## Comparing `sdgrate-0.2.2.tar` & `sdgrate-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 18:27:58.079668 sdgrate-0.2.2/
--rw-r--r--   0 damian     (501) staff       (20)    34523 2017-09-30 07:16:25.000000 sdgrate-0.2.2/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)       26 2023-02-19 13:57:54.000000 sdgrate-0.2.2/MANIFEST.in
--rw-r--r--   0 damian     (501) staff       (20)    10485 2023-04-14 18:27:58.079545 sdgrate-0.2.2/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)     9909 2023-04-14 18:27:34.000000 sdgrate-0.2.2/README.md
--rw-r--r--   0 damian     (501) staff       (20)      953 2023-04-14 18:10:52.000000 sdgrate-0.2.2/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-14 18:27:58.079706 sdgrate-0.2.2/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 18:27:58.075359 sdgrate-0.2.2/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 18:27:58.078560 sdgrate-0.2.2/src/sdgrate/
--rw-r--r--   0 damian     (501) staff       (20)   159676 2023-02-19 12:53:47.000000 sdgrate-0.2.2/src/sdgrate/LibreBaskerville-DpdE.ttf
--rw-r--r--   0 damian     (501) staff       (20)       21 2023-02-19 12:53:47.000000 sdgrate-0.2.2/src/sdgrate/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    16376 2023-02-28 22:12:45.000000 sdgrate-0.2.2/src/sdgrate/checkpoint_merger_mbw.py
--rw-r--r--   0 damian     (501) staff       (20)    28585 2023-04-14 18:17:41.000000 sdgrate-0.2.2/src/sdgrate/grate.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-14 18:27:58.079328 sdgrate-0.2.2/src/sdgrate.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    10485 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      376 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       45 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/entry_points.txt
--rw-r--r--   0 damian     (501) staff       (20)       90 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        8 2023-04-14 18:27:58.000000 sdgrate-0.2.2/src/sdgrate.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-19 18:52:30.712838 sdgrate-0.2.3/
+-rw-r--r--   0 damian     (501) staff       (20)    34523 2017-09-30 07:16:25.000000 sdgrate-0.2.3/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)       26 2023-02-19 13:57:54.000000 sdgrate-0.2.3/MANIFEST.in
+-rw-r--r--   0 damian     (501) staff       (20)    10570 2023-04-19 18:52:30.712684 sdgrate-0.2.3/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)     9994 2023-04-19 18:51:14.000000 sdgrate-0.2.3/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      953 2023-04-19 18:31:40.000000 sdgrate-0.2.3/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-04-19 18:52:30.712877 sdgrate-0.2.3/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-19 18:52:30.706255 sdgrate-0.2.3/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-19 18:52:30.710906 sdgrate-0.2.3/src/sdgrate/
+-rw-r--r--   0 damian     (501) staff       (20)   159676 2023-02-19 12:53:47.000000 sdgrate-0.2.3/src/sdgrate/LibreBaskerville-DpdE.ttf
+-rw-r--r--   0 damian     (501) staff       (20)       21 2023-02-19 12:53:47.000000 sdgrate-0.2.3/src/sdgrate/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    16376 2023-02-28 22:12:45.000000 sdgrate-0.2.3/src/sdgrate/checkpoint_merger_mbw.py
+-rw-r--r--   0 damian     (501) staff       (20)    28759 2023-04-19 18:30:59.000000 sdgrate-0.2.3/src/sdgrate/grate.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-04-19 18:52:30.712448 sdgrate-0.2.3/src/sdgrate.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    10570 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      376 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       45 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/entry_points.txt
+-rw-r--r--   0 damian     (501) staff       (20)       90 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        8 2023-04-19 18:52:30.000000 sdgrate-0.2.3/src/sdgrate.egg-info/top_level.txt
```

### Comparing `sdgrate-0.2.2/LICENSE` & `sdgrate-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.2/PKG-INFO` & `sdgrate-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgrate
-Version: 0.2.2
+Version: 0.2.3
 Summary: A grid image generator for Stable Diffusion models based on 🧨diffusers.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/grate
 Project-URL: Bug Tracker, https://github.com/damian0815/grate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -177,8 +177,10 @@
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
 
 ## Changelog
 
-#### 0.2.2 - added `--use_penultimate_clip_layer` arg for improved SD2 generation quality (aka "clip skip")
+#### 0.2.3 - fix crash when running compel, fix diffusers 0.15 support actually
+
+#### 0.2.2 - added `--use_penultimate_clip_layer` arg ~~for improved SD2 generation quality~~ (aka "clip skip")
```

### Comparing `sdgrate-0.2.2/README.md` & `sdgrate-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -163,8 +163,10 @@
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
 
 ## Changelog
 
-#### 0.2.2 - added `--use_penultimate_clip_layer` arg for improved SD2 generation quality (aka "clip skip")
+#### 0.2.3 - fix crash when running compel, fix diffusers 0.15 support actually
+
+#### 0.2.2 - added `--use_penultimate_clip_layer` arg ~~for improved SD2 generation quality~~ (aka "clip skip")
```

### Comparing `sdgrate-0.2.2/pyproject.toml` & `sdgrate-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdgrate"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A grid image generator for Stable Diffusion models based on 🧨diffusers."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `sdgrate-0.2.2/src/sdgrate/LibreBaskerville-DpdE.ttf` & `sdgrate-0.2.3/src/sdgrate/LibreBaskerville-DpdE.ttf`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.2/src/sdgrate/checkpoint_merger_mbw.py` & `sdgrate-0.2.3/src/sdgrate/checkpoint_merger_mbw.py`

 * *Files identical despite different names*

### Comparing `sdgrate-0.2.2/src/sdgrate/grate.py` & `sdgrate-0.2.3/src/sdgrate/grate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import argparse
 import pathlib
 from typing import Optional
 
 import torch
 from compel import Compel
-from diffusers.pipelines.stable_diffusion.convert_from_ckpt import load_pipeline_from_original_stable_diffusion_ckpt
 from diffusers import StableDiffusionPipeline, DPMSolverMultistepScheduler
 from PIL import Image, ImageDraw, ImageFont
 from diffusers.pipelines.stable_diffusion import StableDiffusionPipelineOutput
 from diffusers.utils import is_xformers_available
 from tqdm import tqdm
 
 from huggingface_hub import list_repo_refs
@@ -153,14 +152,17 @@
 
 
 def load_model(repo_id_or_path, prefer_fp16: bool = True, local_files_only: bool=False):
     if os.path.isfile(repo_id_or_path):
         yaml_file = (os.path.splitext(repo_id_or_path)[0] + ".yaml")
         if not os.path.exists(yaml_file):
             yaml_file = None
+        # this won't work on diffusers 0.15+, need to find a way to reliably support old + new
+        from diffusers.pipelines.stable_diffusion.convert_from_ckpt import \
+                load_pipeline_from_original_stable_diffusion_ckpt
         return load_pipeline_from_original_stable_diffusion_ckpt(repo_id_or_path, original_config_file=yaml_file)
     elif os.path.isdir(repo_id_or_path):
         return StableDiffusionPipeline.from_pretrained(repo_id_or_path)
     else:
         revision = None  # use default
         if prefer_fp16:
             refs = list_repo_refs(repo_id_or_path)
@@ -205,15 +207,14 @@
                     text_encoder=pipeline.text_encoder,
                     use_penultimate_clip_layer=use_penultimate_clip_layer)
     for batch in progress_bar:
         batch_prompts, batch_negative_prompts, batch_seeds = zip(*batch)
         print(f" - {batch_prompts}")
         generator_device = 'cpu' if device == 'mps' else device
         manual_seed_generators = [torch.Generator(generator_device).manual_seed(seed) for seed in batch_seeds]
-        positive_embeds = compel(batch_prompts)
         pipeline_output: StableDiffusionPipelineOutput = pipeline(prompt=list(batch_prompts),
                                                                   negative_prompt=list(batch_negative_prompts),
                                                                   generator=manual_seed_generators,
                                                                   width=sample_w,
                                                                   height=sample_h,
                                                                   num_inference_steps=num_inference_steps,
                                                                   guidance_scale=cfg)
@@ -305,15 +306,15 @@
                size: tuple[int, int],
                batch_size: int,
                inference_steps: int = 15,
                save_partial_filename: Optional[str] = None,
                local_files_only: bool = False,
                merge_config: Optional[dict] = None,
                disable_nsfw_checker: bool = False,
-               use_penultimate_clip_layer: bool = False,
+               use_penultimate_clip_layer: Optional[bool] = False, # autodetect if None
                ) -> Image:
     all_images = []
     print(f"{len(prompts)} prompts")
 
     row_labels = []
 
     def save_partial_if_requested():
@@ -511,15 +512,15 @@
                         type=str,
                         help="(Optional) If doing a merge, save all merge combinations using this path as a prefix.")
     parser.add_argument("--save_merge_float32",
                         action="store_true",
                         help="(Optional) If saving merges, save with float32 precision (default is float16).")
     parser.add_argument("--use_penultimate_clip_layer",
                         action="store_true",
-                        help="(Optional) Use the outputs from penultimate (second to last) CLIP hidden layer.")
+                        help="(Optional) Use the outputs from penultimate (second to last) CLIP hidden layer. On detected SD2.x models this defaults on, otherwise it defaults off.")
     args = parser.parse_args()
 
 
     def use_arg_list_or_expand_or_default(arg: list, required_count: int, default: list|None) -> list:
         if arg is None:
             return default
         elif len(arg) == 1:
```

### Comparing `sdgrate-0.2.2/src/sdgrate.egg-info/PKG-INFO` & `sdgrate-0.2.3/src/sdgrate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdgrate
-Version: 0.2.2
+Version: 0.2.3
 Summary: A grid image generator for Stable Diffusion models based on 🧨diffusers.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/grate
 Project-URL: Bug Tracker, https://github.com/damian0815/grate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
@@ -177,8 +177,10 @@
 
 The main `sdgrate.grate` module includes the following functions, which may be useful: `merge_models`, `render_row`, `render_all`. 
 
 The model merger is implemented as a custom pipeline based on a modified version of the (checkpoint_merger pipeline)
 
 ## Changelog
 
-#### 0.2.2 - added `--use_penultimate_clip_layer` arg for improved SD2 generation quality (aka "clip skip")
+#### 0.2.3 - fix crash when running compel, fix diffusers 0.15 support actually
+
+#### 0.2.2 - added `--use_penultimate_clip_layer` arg ~~for improved SD2 generation quality~~ (aka "clip skip")
```

