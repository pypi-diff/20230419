# Comparing `tmp/nwebclient-1.0.68.tar.gz` & `tmp/nwebclient-1.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.68.tar", last modified: Tue Apr  4 09:32:11 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.69.tar", last modified: Wed Apr 19 20:16:53 2023, max compression
```

## Comparing `nwebclient-1.0.68.tar` & `nwebclient-1.0.69.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-04 09:32:11.486804 nwebclient-1.0.68/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.68/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-04 09:32:11.486804 nwebclient-1.0.68/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.68/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-04 09:32:11.486804 nwebclient-1.0.68/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.68/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.68/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.68/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6499 2023-04-04 09:30:24.000000 nwebclient-1.0.68/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.68/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.68/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-04 09:32:11.486804 nwebclient-1.0.68/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-04 09:32:11.000000 nwebclient-1.0.68/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-04 09:32:11.000000 nwebclient-1.0.68/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-04 09:32:11.000000 nwebclient-1.0.68/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-04 09:32:11.000000 nwebclient-1.0.68/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-04 09:32:11.000000 nwebclient-1.0.68/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-04 09:32:11.000000 nwebclient-1.0.68/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-04 09:32:11.486804 nwebclient-1.0.68/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-04 09:32:07.000000 nwebclient-1.0.68/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-19 20:16:53.527566 nwebclient-1.0.69/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.69/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-19 20:16:53.527566 nwebclient-1.0.69/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.69/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-19 20:16:53.527566 nwebclient-1.0.69/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.69/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.69/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3104 2023-03-29 20:50:31.000000 nwebclient-1.0.69/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6979 2023-04-19 19:11:30.000000 nwebclient-1.0.69/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     5582 2023-03-29 09:33:58.000000 nwebclient-1.0.69/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3218 2023-03-27 16:42:32.000000 nwebclient-1.0.69/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-04-19 20:16:53.527566 nwebclient-1.0.69/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-04-19 20:16:53.000000 nwebclient-1.0.69/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-04-19 20:16:53.000000 nwebclient-1.0.69/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-04-19 20:16:53.000000 nwebclient-1.0.69/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       84 2023-04-19 20:16:53.000000 nwebclient-1.0.69/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-04-19 20:16:53.000000 nwebclient-1.0.69/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-04-19 20:16:53.000000 nwebclient-1.0.69/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-04-19 20:16:53.527566 nwebclient-1.0.69/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      829 2023-04-19 20:16:48.000000 nwebclient-1.0.69/setup.py
```

### Comparing `nwebclient-1.0.68/LICENSE` & `nwebclient-1.0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.68/PKG-INFO` & `nwebclient-1.0.69/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.68
+Version: 1.0.69
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.68/README.md` & `nwebclient-1.0.69/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.68/nwebclient/__init__.py` & `nwebclient-1.0.69/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.68/nwebclient/__main__.py` & `nwebclient-1.0.69/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.68/nwebclient/crypt.py` & `nwebclient-1.0.69/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.68/nwebclient/sd.py` & `nwebclient-1.0.69/nwebclient/sd.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
   ig = ImageGen()
   ig.prompt = "photo"
   ig.loop(5)
   
   ig.executeFromUrl('https://...')
 """
 class ImageGen:
+    generator = 'diffusers'
     # scheduler
     pipe = None
     prompt = "photo"
     negative_prompt = "text, cartoon, anime, drawing, meme, postcard, painting, ((fuzzy)), ((blurred)), ((low resolution)), ((b&w)), ((monochrome)), ambiguous, ((deformed)), oversaturated, ((out of shot)), ((incoherent)), (((glitched))), (((3d render))), cgi, ((incorrect anatomy)), bad hands, lowres, long body, ((blurry)), double, ((duplicate body parts)), (disfigured), (extra limbs), fused fingers, extra fingers, malformed hands, ((((mutated hands and fingers)))), conjoined, ((missing limbs)), logo, signature, mutated, jpeg artifacts, low quality, bad eyes, oversized, disproportionate, (((incorrect proportions))), exaggerated, (((aliasing)))"
     guidance_scale = 7.5
     num_inference_steps=25
     height=800
@@ -60,15 +61,25 @@
            self.pipe = StableDiffusionPipeline.from_pretrained(self.model_id, torch_dtype=torch.float16, revision=model_revision)
         else:
            self.pipe = StableDiffusionPipeline.from_pretrained(self.model_id, scheduler=self.scheduler, custom_pipeline="lpw_stable_diffusion", torch_dtype=torch.float16, revision=model_revision)
         self.pipe = self.pipe.to(device)
         if self.model_id=="XpucT/Deliberate" or self.model_id == "SG161222/Realistic_Vision_V1.4_Fantasy.ai":
             self.pipe.safety_checker = lambda images, clip_input: (images, False)
         self.load_model = self.model_id
+    def initA1111():
+        #self.api
     def gen(self, loop_number=1):
+        if self.generator == 'diffusers':
+            self.genDiffusers(loop_number)
+        elif self.generator == 'automatic1111':
+            self.genA1111(loop_number)
+    def genA1111(self, loop_number=1):  
+        result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, cfg_scale=7)
+        self.save_image(result.image, 0,loop_number)
+    def genDiffusers(self, loop_number=1):
         if self.pipe is None:
             self.load()
         images = self.pipe(self.prompt,
             height = self.height,
             width = self.width,
             num_inference_steps = self.num_inference_steps,      # higher better quali default=45
             guidance_scale = self.guidance_scale,                # Prioritize creativity  7.5  Prioritize prompt (higher)
```

### Comparing `nwebclient-1.0.68/nwebclient/sdb.py` & `nwebclient-1.0.69/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.68/nwebclient/ticker.py` & `nwebclient-1.0.69/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.68/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.69/nwebclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.68
+Version: 1.0.69
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.68/setup.py` & `nwebclient-1.0.69/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.68",
+    version="1.0.69",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

