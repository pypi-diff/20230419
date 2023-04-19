# Comparing `tmp/pyGPUreg-0.1.1.tar.gz` & `tmp/pyGPUreg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGPUreg-0.1.1.tar", last modified: Thu Mar 23 16:02:21 2023, max compression
+gzip compressed data, was "pyGPUreg-0.1.2.tar", last modified: Wed Apr 19 10:27:33 2023, max compression
```

## Comparing `pyGPUreg-0.1.1.tar` & `pyGPUreg-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:21.617427 pyGPUreg-0.1.1/
--rw-rw-rw-   0        0        0    17099 2023-03-23 08:54:10.000000 pyGPUreg-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0       73 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      274 2023-03-23 16:02:21.617427 pyGPUreg-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4781 2023-03-23 08:54:10.000000 pyGPUreg-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:21.595486 pyGPUreg-0.1.1/pyGPUreg/
--rw-rw-rw-   0        0        0      114 2023-03-23 16:02:16.000000 pyGPUreg-0.1.1/pyGPUreg/__init__.py
--rw-rw-rw-   0        0        0     5995 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/opengl_classes.py
--rw-rw-rw-   0        0        0    28173 2023-03-23 15:56:23.000000 pyGPUreg-0.1.1/pyGPUreg/pyGPUreg.py
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:21.615433 pyGPUreg-0.1.1/pyGPUreg/shaders/
--rw-rw-rw-   0        0        0     1477 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/butterflytexture.glsl
--rw-rw-rw-   0        0        0      398 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/copy_r_to_rg.glsl
--rw-rw-rw-   0        0        0      392 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/cos_filter.glsl
--rw-rw-rw-   0        0        0      404 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/cos_filter_r.glsl
--rw-rw-rw-   0        0        0     3377 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/fft.glsl
--rw-rw-rw-   0        0        0      746 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/fft_inversion_permutation.glsl
--rw-rw-rw-   0        0        0      458 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/fft_inversion_permutation_single.glsl
--rw-rw-rw-   0        0        0      532 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/fft_phase_correlation.glsl
--rw-rw-rw-   0        0        0      582 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/fft_phase_correlation_single.glsl
--rw-rw-rw-   0        0        0     2802 2023-03-22 07:56:15.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/fft_single.glsl
--rw-rw-rw-   0        0        0      805 2023-03-23 13:56:33.000000 pyGPUreg-0.1.1/pyGPUreg/shaders/resample_image.glsl
-drwxrwxrwx   0        0        0        0 2023-03-23 16:02:21.602467 pyGPUreg-0.1.1/pyGPUreg.egg-info/
--rw-rw-rw-   0        0        0      274 2023-03-23 16:02:21.000000 pyGPUreg-0.1.1/pyGPUreg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      706 2023-03-23 16:02:21.000000 pyGPUreg-0.1.1/pyGPUreg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-23 16:02:21.000000 pyGPUreg-0.1.1/pyGPUreg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-03-23 16:02:21.000000 pyGPUreg-0.1.1/pyGPUreg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-23 16:02:21.000000 pyGPUreg-0.1.1/pyGPUreg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-23 16:02:21.617427 pyGPUreg-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-03-23 16:02:16.000000 pyGPUreg-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:27:33.347639 pyGPUreg-0.1.2/
+-rw-rw-rw-   0        0        0    17099 2023-03-23 08:54:10.000000 pyGPUreg-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       73 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      274 2023-04-19 10:27:33.347639 pyGPUreg-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4777 2023-04-19 10:23:36.000000 pyGPUreg-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 10:27:33.327499 pyGPUreg-0.1.2/pyGPUreg/
+-rw-rw-rw-   0        0        0      114 2023-04-19 10:23:37.000000 pyGPUreg-0.1.2/pyGPUreg/__init__.py
+-rw-rw-rw-   0        0        0     5995 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/opengl_classes.py
+-rw-rw-rw-   0        0        0    28338 2023-04-19 10:24:44.000000 pyGPUreg-0.1.2/pyGPUreg/pyGPUreg.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:27:33.347639 pyGPUreg-0.1.2/pyGPUreg/shaders/
+-rw-rw-rw-   0        0        0     1477 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/butterflytexture.glsl
+-rw-rw-rw-   0        0        0      398 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/copy_r_to_rg.glsl
+-rw-rw-rw-   0        0        0      392 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/cos_filter.glsl
+-rw-rw-rw-   0        0        0      404 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/cos_filter_r.glsl
+-rw-rw-rw-   0        0        0     3377 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft.glsl
+-rw-rw-rw-   0        0        0      746 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_inversion_permutation.glsl
+-rw-rw-rw-   0        0        0      458 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_inversion_permutation_single.glsl
+-rw-rw-rw-   0        0        0      532 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_phase_correlation.glsl
+-rw-rw-rw-   0        0        0      582 2023-04-19 10:23:36.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_phase_correlation_single.glsl
+-rw-rw-rw-   0        0        0     2802 2023-03-22 07:56:15.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/fft_single.glsl
+-rw-rw-rw-   0        0        0      805 2023-04-19 10:23:36.000000 pyGPUreg-0.1.2/pyGPUreg/shaders/resample_image.glsl
+drwxrwxrwx   0        0        0        0 2023-04-19 10:27:33.335559 pyGPUreg-0.1.2/pyGPUreg.egg-info/
+-rw-rw-rw-   0        0        0      274 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      706 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-19 10:27:33.000000 pyGPUreg-0.1.2/pyGPUreg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 10:27:33.347639 pyGPUreg-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      521 2023-04-19 10:27:30.000000 pyGPUreg-0.1.2/setup.py
```

### Comparing `pyGPUreg-0.1.1/LICENSE.txt` & `pyGPUreg-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/README.md` & `pyGPUreg-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 When tested on a Quadro P2200, pyGPUreg is more than 40x faster than StackReg, the Python port of TurboReg (https://pystackreg.readthedocs.io/). For smaller images (32 x 32 pixels or less), CPU-based processing with StackReg is faster. A comparison is plotted below.
 
 ![](res/pyPGUreg_vs_StackReg.png)
 ### Usage ###
 For now, pyGPUreg only works on images that are square and with size 2^n (e.g. 128, 256, 512, etc. pixel width and height)
 
 #### Installation ####
-pyGPUreg is available on pypi. Install with pip using the this command:
+pyGPUreg is available on pypi. Install with pip using this command:
 ```
 pip install pyGPUreg
 ```
 #### Initialization ####
 Prior to calling any of the core functions, pyGPUreg has to be initialized.
 
 ```
```

### Comparing `pyGPUreg-0.1.1/pyGPUreg/opengl_classes.py` & `pyGPUreg-0.1.2/pyGPUreg/opengl_classes.py`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/pyGPUreg/pyGPUreg.py` & `pyGPUreg-0.1.2/pyGPUreg/pyGPUreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .opengl_classes import *
 import glfw
 import math
-import matplotlib.pyplot as plt
+
 
 # Module enums
 EDGE_MODE_ZERO = 0
 EDGE_MODE_CLAMP = 1
 EDGE_MODE_REFLECT = 2
 SUBPIXEL_MODE_NONE = 0  # no subpixel peak detection. limits shift resolution to pixel size.
 SUBPIXEL_MODE_COM = 1  # detect sub-pixel shift by calculating the center of mass of the peak in the FFT(phase correlation)
@@ -179,14 +179,15 @@
     x_shift = -x_shift
     y_shift = -y_shift
     return x_shift, y_shift
 
 def sample_texture_with_shift(texture, shift, edge_mode=EDGE_MODE_ZERO, interpolation_mode=INTERPOLATION_MODE_LINEAR):
     """
     Identical to sample_image_with_shift(), except requires manual uploading of pixeldata to a texture and takes the texture as argument.
+    When using pyGPUreg in an application with multiple openGL contexts, use of this functions requires manual context managing as well.
     """
     texture.bind()
     # set edge and interpolation mode for that texture
     if edge_mode in [EDGE_MODE_ZERO, EDGE_MODE_CLAMP]:
         glTexParameter(GL_TEXTURE_2D, GL_TEXTURE_WRAP_S, GL_CLAMP_TO_EDGE)
         glTexParameter(GL_TEXTURE_2D, GL_TEXTURE_WRAP_T, GL_CLAMP_TO_EDGE)
     elif edge_mode == EDGE_MODE_REFLECT:
@@ -216,14 +217,16 @@
     cs_resample.unbind()
 
     # copy result to CPU
     texture_resample_b.bind()
     resampled = glGetTexImage(GL_TEXTURE_2D, 0, GL_RED, GL_FLOAT)
     glMemoryBarrier(GL_TEXTURE_FETCH_BARRIER_BIT)
 
+    resampled = np.reshape(resampled, (height, width))
+
     return resampled
 
 
 def sample_image_with_shift(image, shift, edge_mode=EDGE_MODE_ZERO, interpolation_mode=INTERPOLATION_MODE_LINEAR):
     """
     :param image: 2D numpy array of pixel values
     :param shift: tuple (dx, dy), the image shift in pixel units
```

### Comparing `pyGPUreg-0.1.1/pyGPUreg/shaders/butterflytexture.glsl` & `pyGPUreg-0.1.2/pyGPUreg/shaders/butterflytexture.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/pyGPUreg/shaders/fft.glsl` & `pyGPUreg-0.1.2/pyGPUreg/shaders/fft.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/pyGPUreg/shaders/fft_inversion_permutation.glsl` & `pyGPUreg-0.1.2/pyGPUreg/shaders/fft_inversion_permutation.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/pyGPUreg/shaders/fft_phase_correlation.glsl` & `pyGPUreg-0.1.2/pyGPUreg/shaders/fft_phase_correlation.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/pyGPUreg/shaders/fft_phase_correlation_single.glsl` & `pyGPUreg-0.1.2/pyGPUreg/shaders/fft_phase_correlation_single.glsl`

 * *Files 1% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 
 void main(void)
 {
     ivec2 x = ivec2(gl_GlobalInvocationID.xy);
     vec2 T = imageLoad(FT_T, x).rg;
     vec2 I = imageLoad(FT_I, x).rg;
     float amplitude = sqrt(pow(T.r * I.r + T.g * I.g, 2) + pow(I.r * T.g - T.r * I.g, 2));
-    float real = (T.r * I.r + T.g * I.r) / amplitude;
+    float real = (T.r * I.r + T.g * I.g) / amplitude;
     float imag = (I.r * T.g - T.r * I.g) / amplitude;
     imageStore(FT_I, x, vec4(real, imag, 0.0, 0.0));
 }
```

### Comparing `pyGPUreg-0.1.1/pyGPUreg/shaders/fft_single.glsl` & `pyGPUreg-0.1.2/pyGPUreg/shaders/fft_single.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/pyGPUreg/shaders/resample_image.glsl` & `pyGPUreg-0.1.2/pyGPUreg/shaders/resample_image.glsl`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/pyGPUreg.egg-info/SOURCES.txt` & `pyGPUreg-0.1.2/pyGPUreg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGPUreg-0.1.1/setup.py` & `pyGPUreg-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyGPUreg',
-    version='0.1.1',
+    version='0.1.2',
     license='GPLv3',
     author="Mart G.F. Last",
     author_email='m.g.f.last@lumc.nl',
     description='GPU-accelerated image registration.\ngithub.com/bionanopatterning/pyGPUreg',
     packages=find_packages(),
     package_data={'pyGPUreg': ['*.glsl', 'shaders/*glsl']},
     include_package_data=True,
```

