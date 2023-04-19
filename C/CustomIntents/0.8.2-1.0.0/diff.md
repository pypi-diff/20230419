# Comparing `tmp/CustomIntents-0.8.2.tar.gz` & `tmp/CustomIntents-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CustomIntents-0.8.2.tar", last modified: Fri Feb 10 10:51:25 2023, max compression
+gzip compressed data, was "CustomIntents-1.0.0.tar", last modified: Wed Apr 19 11:54:10 2023, max compression
```

## Comparing `CustomIntents-0.8.2.tar` & `CustomIntents-1.0.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-10 10:51:25.699583 CustomIntents-0.8.2/
-drwxrwxrwx   0        0        0        0 2023-02-10 10:51:25.635582 CustomIntents-0.8.2/CustomIntents/
--rw-rw-rw-   0        0        0      237 2023-01-12 12:14:43.000000 CustomIntents-0.8.2/CustomIntents/Bcolor.py
--rw-rw-rw-   0        0        0    26621 2023-01-19 13:27:12.000000 CustomIntents-0.8.2/CustomIntents/BinaryImageClassificator.py
--rw-rw-rw-   0        0        0    31609 2023-01-17 15:57:54.000000 CustomIntents-0.8.2/CustomIntents/Chatbot.py
--rw-rw-rw-   0        0        0    36776 2023-02-02 04:43:27.000000 CustomIntents-0.8.2/CustomIntents/ImageClassificator.py
--rw-rw-rw-   0        0        0     3431 2023-02-10 10:30:17.000000 CustomIntents-0.8.2/CustomIntents/ImageGenerator.py
--rw-rw-rw-   0        0        0     5881 2023-01-12 12:14:42.000000 CustomIntents-0.8.2/CustomIntents/JsonIntents.py
--rw-rw-rw-   0        0        0    55975 2023-01-12 14:52:13.000000 CustomIntents-0.8.2/CustomIntents/Legacy.py
--rw-rw-rw-   0        0        0    13114 2023-01-17 21:59:43.000000 CustomIntents-0.8.2/CustomIntents/MusicGan.py
--rw-rw-rw-   0        0        0     7124 2023-01-12 15:04:17.000000 CustomIntents-0.8.2/CustomIntents/PLinearRegression.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:51:25.678587 CustomIntents-0.8.2/CustomIntents/Pfunction/
--rw-rw-rw-   0        0        0    18059 2023-01-30 15:07:29.000000 CustomIntents-0.8.2/CustomIntents/Pfunction/Pfunctions.py
--rw-rw-rw-   0        0        0        2 2023-01-12 15:00:24.000000 CustomIntents-0.8.2/CustomIntents/Pfunction/__init__.py
--rw-rw-rw-   0        0        0    10842 2023-01-26 17:32:35.000000 CustomIntents-0.8.2/CustomIntents/StyleTransformer.py
--rw-rw-rw-   0        0        0      326 2023-02-10 10:11:23.000000 CustomIntents-0.8.2/CustomIntents/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:51:25.695626 CustomIntents-0.8.2/CustomIntents/cascades/
--rw-rw-rw-   0        0        0   963439 2023-01-03 15:25:52.000000 CustomIntents-0.8.2/CustomIntents/cascades/haarcascade_frontalcatface.xml
--rw-rw-rw-   0        0        0     6912 2023-02-02 23:14:41.000000 CustomIntents-0.8.2/CustomIntents/scanner.py
-drwxrwxrwx   0        0        0        0 2023-02-10 10:51:25.668589 CustomIntents-0.8.2/CustomIntents.egg-info/
--rw-rw-rw-   0        0        0    30503 2023-02-10 10:51:25.000000 CustomIntents-0.8.2/CustomIntents.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      699 2023-02-10 10:51:25.000000 CustomIntents-0.8.2/CustomIntents.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-10 10:51:25.000000 CustomIntents-0.8.2/CustomIntents.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      291 2023-02-10 10:51:25.000000 CustomIntents-0.8.2/CustomIntents.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-10 10:51:25.000000 CustomIntents-0.8.2/CustomIntents.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35184 2023-01-11 15:03:33.000000 CustomIntents-0.8.2/LICENSE.md
--rw-rw-rw-   0        0        0    30503 2023-02-10 10:51:25.698584 CustomIntents-0.8.2/PKG-INFO
--rw-rw-rw-   0        0        0    30214 2023-02-10 10:49:32.000000 CustomIntents-0.8.2/README.md
--rw-rw-rw-   0        0        0       42 2023-02-10 10:51:25.699583 CustomIntents-0.8.2/setup.cfg
--rw-rw-rw-   0        0        0     1140 2023-02-10 10:49:32.000000 CustomIntents-0.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:54:10.891827 CustomIntents-1.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-19 11:54:10.465058 CustomIntents-1.0.0/CustomIntents/
+-rw-rw-rw-   0        0        0      237 2023-01-12 12:14:43.000000 CustomIntents-1.0.0/CustomIntents/Bcolor.py
+-rw-rw-rw-   0        0        0    26621 2023-01-19 13:27:12.000000 CustomIntents-1.0.0/CustomIntents/BinaryImageClassificator.py
+-rw-rw-rw-   0        0        0    31609 2023-01-17 15:57:54.000000 CustomIntents-1.0.0/CustomIntents/Chatbot.py
+-rw-rw-rw-   0        0        0    36776 2023-02-02 04:43:27.000000 CustomIntents-1.0.0/CustomIntents/ImageClassificator.py
+-rw-rw-rw-   0        0        0     3431 2023-02-10 10:30:17.000000 CustomIntents-1.0.0/CustomIntents/ImageGenerator.py
+-rw-rw-rw-   0        0        0     5881 2023-01-12 12:14:42.000000 CustomIntents-1.0.0/CustomIntents/JsonIntents.py
+-rw-rw-rw-   0        0        0    55975 2023-01-12 14:52:13.000000 CustomIntents-1.0.0/CustomIntents/Legacy.py
+-rw-rw-rw-   0        0        0    13114 2023-01-17 21:59:43.000000 CustomIntents-1.0.0/CustomIntents/MusicGan.py
+-rw-rw-rw-   0        0        0     7124 2023-01-12 15:04:17.000000 CustomIntents-1.0.0/CustomIntents/PLinearRegression.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:54:10.883827 CustomIntents-1.0.0/CustomIntents/Pfunction/
+-rw-rw-rw-   0        0        0    18059 2023-01-30 15:07:29.000000 CustomIntents-1.0.0/CustomIntents/Pfunction/Pfunctions.py
+-rw-rw-rw-   0        0        0        2 2023-01-12 15:00:24.000000 CustomIntents-1.0.0/CustomIntents/Pfunction/__init__.py
+-rw-rw-rw-   0        0        0    10842 2023-01-26 17:32:35.000000 CustomIntents-1.0.0/CustomIntents/StyleTransformer.py
+-rw-rw-rw-   0        0        0    29268 2023-04-19 10:32:09.000000 CustomIntents-1.0.0/CustomIntents/Super_Res.py
+-rw-rw-rw-   0        0        0      357 2023-04-19 10:32:09.000000 CustomIntents-1.0.0/CustomIntents/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:54:10.885841 CustomIntents-1.0.0/CustomIntents/cascades/
+-rw-rw-rw-   0        0        0   963439 2023-01-03 15:25:52.000000 CustomIntents-1.0.0/CustomIntents/cascades/haarcascade_frontalcatface.xml
+-rw-rw-rw-   0        0        0     6912 2023-02-02 23:14:41.000000 CustomIntents-1.0.0/CustomIntents/scanner.py
+-rw-rw-rw-   0        0        0    12923 2023-04-19 10:32:09.000000 CustomIntents-1.0.0/CustomIntents/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-19 11:54:10.878846 CustomIntents-1.0.0/CustomIntents.egg-info/
+-rw-rw-rw-   0        0        0    36493 2023-04-19 11:54:10.000000 CustomIntents-1.0.0/CustomIntents.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      749 2023-04-19 11:54:10.000000 CustomIntents-1.0.0/CustomIntents.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 11:54:10.000000 CustomIntents-1.0.0/CustomIntents.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      291 2023-04-19 11:54:10.000000 CustomIntents-1.0.0/CustomIntents.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-19 11:54:10.000000 CustomIntents-1.0.0/CustomIntents.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35184 2023-01-11 15:03:33.000000 CustomIntents-1.0.0/LICENSE.md
+-rw-rw-rw-   0        0        0    36493 2023-04-19 11:54:10.890831 CustomIntents-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    36204 2023-04-19 11:47:59.000000 CustomIntents-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-19 11:54:10.891827 CustomIntents-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1140 2023-04-19 11:47:59.000000 CustomIntents-1.0.0/setup.py
```

### Comparing `CustomIntents-0.8.2/CustomIntents/BinaryImageClassificator.py` & `CustomIntents-1.0.0/CustomIntents/BinaryImageClassificator.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/Chatbot.py` & `CustomIntents-1.0.0/CustomIntents/Chatbot.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/ImageClassificator.py` & `CustomIntents-1.0.0/CustomIntents/ImageClassificator.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/ImageGenerator.py` & `CustomIntents-1.0.0/CustomIntents/ImageGenerator.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/JsonIntents.py` & `CustomIntents-1.0.0/CustomIntents/JsonIntents.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/Legacy.py` & `CustomIntents-1.0.0/CustomIntents/Legacy.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/MusicGan.py` & `CustomIntents-1.0.0/CustomIntents/MusicGan.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/PLinearRegression.py` & `CustomIntents-1.0.0/CustomIntents/PLinearRegression.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/Pfunction/Pfunctions.py` & `CustomIntents-1.0.0/CustomIntents/Pfunction/Pfunctions.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/StyleTransformer.py` & `CustomIntents-1.0.0/CustomIntents/StyleTransformer.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/cascades/haarcascade_frontalcatface.xml` & `CustomIntents-1.0.0/CustomIntents/cascades/haarcascade_frontalcatface.xml`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents/scanner.py` & `CustomIntents-1.0.0/CustomIntents/scanner.py`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/CustomIntents.egg-info/PKG-INFO` & `CustomIntents-1.0.0/CustomIntents.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: CustomIntents
-Version: 0.8.2
+Version: 1.0.0
 Home-page: https://github.com/iparsw/custom-intent.git
 Author: Parsa Roshanak (iparsw)
 Author-email: parsaroshanak@gmail.com
 Requires-Python: >=3.9, <=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 # Custom Intents
 
-V0.8.2
+V1.0.0
 (it's still in buggy alpha)
 
-## a simple way to create chatbots Ai, image classification Ai and more!!
+## a simple way to create chatbots Ai, image classification Ai, image generation Ai, image supper resolution Ai and more!!
 
 # installation
 
 you can install the package from pypi (pip)
 
 ```commandline
 pip install CustomIntents
@@ -28,18 +28,192 @@
 
 ![Demo1](images/img2.png)
 
 ![Demo2](images/img.png)
 
 
 
-A package build on top of keras for creating and training deep learning chatbots (text classification), binary image classification and linear regression models in just three lines of code 
+A package build on top of keras for creating and training deep learning chatbots (text classification), image classification, image generation Ai, image super resolution, style transforming and linear regression models in just three lines of code 
 
 the package is inspired by NeuralNine, neuralintents package a packege that let you build chatbot models with 3 lines of code
 
+# list of features:
+* [SuperRes class](#superres-class)
+* [ImageGenerator class](#imagegenerator-class)
+* [ChatBot class](#chatbot-class)
+* [JsonIntents](#jsonintents-class)
+* [ImageClassificator class](#imageclassificator-class)
+* [StyleTransformer class](#styletransformer-class)
+* [BinaryImageClassificator](#binaryimageclassificator-class)
+* [PLinearRegression class](#plinearregression-class)
+* [scanner moudule](#scanner-moudule)
+
+# SuperRes class
+
+## Init arguments
+```python
+def __init__(self, input_size: tuple = (300, 300),
+             upscale_factor: int = 3,
+             cpu_only: bool = False):
+```
+
+input_size : this is only required when training or finetuning
+
+upscale_factor : the upscale factor
+
+cpu_only : whether to use only CPU or not
+
+## upscale_image method
+```python
+def upscale_image(self, img,
+                  save_name: str = None,
+                  save_image: bool = True):
+```
+img : the image you want to upscale
+
+save_image : whether to save the image
+
+save_name : the name of the saved file
+
+## upscale_image_from_path method
+```python
+def upscale_image_from_path(self, img_path,
+                            save_name: str = None,
+                            save_image: bool = True)
+```
+its like upscale_image method except that it requires a path to the image
+
+## load_training_data method
+```python
+def load_training_data(self, dataset_path: str,
+                       validation_split: float = 0.2,
+                       batch_size: int = 8)
+```
+dataset_path : path to the training and validation data directory
+
+validation_split : a float between 0 and 1 where the validation split is specified
+
+batch_size : batch size
+
+## train method
+```python
+def train(self, lr: float = 0.001,
+          optimizer: str = "Adam",
+          epochs: int = 50,
+          ESPCNCallback_usage: bool = True,
+          ESPCNCallback_test_path: str = "test",
+          epoch_per_psnr: int = 20,
+          psnr_plot: bool = True,
+          model_type: str = "xs1",
+          loss_fns: list = None,
+          loss_fns_weight: list = None):
+```
+optimizer : name of the optimizer (corently supported optimizers are : Adam, Adagrad, Adamax, Adadelta, SGD, RMSprop, Nadam)
+
+epochs : number of epochs to train
+
+ESPCNCallback_usage : wether to use ESPCNCallback or not
+
+ESPCNCallback_test_path : a path to the test data directory for ESPCNCallback
+
+epoch_per_psnr : if you use ESPCNCallback it will show a sample every few epochs you can choose that number here
+
+psnr_plot : if you use ESPCNCall you can turn plutting a sample off
+
+model_type : the type of the model (there are some different types in this package but for now i recommend using using the diffault xs1)
+
+loss_fns : a list containing loss functions you want to use if you want only one loss function to use you can pass a list with only on loss functions 
+
+(corently supported loss functions are : mse, mae, mape, ssim, psnr, ipcusl (this is a custom loss function for more information read IPCUSL.md), charbonnier, tv (total variation), tvd (total variation difference))
+
+loss_fns_weight : if you use multiple loss functions the model will calculate their weighted sum and this is a list that contains their sum in this order (mse,mae,mape,ssim,psnr,ipcusl,charbonnier,tv,tvd)
+
+## fine_tuning method
+```python
+def fine_tuning(self, lr: float = 0.001,
+                epochs: int = 50,
+                model_name: str = "super_res",
+                ESPCNCallback_usage: bool = True,
+                ESPCNCallback_test_path: str = "test",
+                epoch_per_psnr: int = 20,
+                psnr_plot: bool = True,
+                recompile: bool = False,
+                optimizer: str = None,
+                loss_fns: list = None,
+                loss_fns_weight: list = None)
+```
+its almost equivalent to the train method except you should load a model first
+
+## load_model method
+
+```python
+def load_model(self, model_name: str = "super_res")
+```
+
+model_name : the name of the model
+
+## save_model method
+
+```python
+def save_model(self, model_name: str = "super_res")
+```
+
+model_name : the name of the model
+
+## benchmark method
+
+```python
+def benchmark(self, image_path: str = "testimage.jpg",
+              input_size: tuple = (300, 300))
+```
+
+this method will benchmark the model based on a single image
+
+input_size : the image will be resized to the given size image and then upscaled by model
+
+## benchmark_from_directory method
+
+```python
+def benchmark_from_directory(self, image_directory_path: str = "test",
+                             input_size: tuple = None)
+```
+
+this method will benchmark the model based on a directory of images
+
+input_size : the image will be resized to the given size image and then upscaled by model
+
+## example of training a model
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(300, 300), upscale_factor=3)
+model.load_training_data(dataset_path="dataset", batch_size=8)
+model.train(epochs=5, model_type="xs1", psnr_plot=True, loss_fns=["IPCUSL"], epoch_per_psnr=4)
+```
+## example of fine tuning a model
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(100, 100), upscale_factor=3)
+model.load_training_data(dataset_path="dataset", batch_size=32)
+model.fine_tuning(epochs=2, lr=0.00008, model_name="CSR3X-1.1.3", psnr_plot=False, loss_fns=["mse", "mae"])
+```
+## example of using the model to generate upscaled images
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(300, 300), upscale_factor=3)
+model.load_model("CSR3X-1.1.2")
+model.upscale_image_from_path(img_path="test_image_2_300x300.jpg", save_name="test_result_300x300_to_900x900_7.jpg")
+```
+
+## image example
+![DemoSuperRes](images/superres2.jpg)
+
+
 # ImageGenerator class
 you can easily use state of the art StableDiffiusion model with this class
 
 ## Init arguments
 ```python
 def __init__(self, *,
              model: str = "StableDiffusion",
```

### Comparing `CustomIntents-0.8.2/CustomIntents.egg-info/SOURCES.txt` & `CustomIntents-1.0.0/CustomIntents.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 CustomIntents/ImageClassificator.py
 CustomIntents/ImageGenerator.py
 CustomIntents/JsonIntents.py
 CustomIntents/Legacy.py
 CustomIntents/MusicGan.py
 CustomIntents/PLinearRegression.py
 CustomIntents/StyleTransformer.py
+CustomIntents/Super_Res.py
 CustomIntents/__init__.py
 CustomIntents/scanner.py
+CustomIntents/utils.py
 CustomIntents.egg-info/PKG-INFO
 CustomIntents.egg-info/SOURCES.txt
 CustomIntents.egg-info/dependency_links.txt
 CustomIntents.egg-info/requires.txt
 CustomIntents.egg-info/top_level.txt
 CustomIntents/Pfunction/Pfunctions.py
 CustomIntents/Pfunction/__init__.py
```

### Comparing `CustomIntents-0.8.2/LICENSE.md` & `CustomIntents-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CustomIntents-0.8.2/PKG-INFO` & `CustomIntents-1.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: CustomIntents
-Version: 0.8.2
+Version: 1.0.0
 Home-page: https://github.com/iparsw/custom-intent.git
 Author: Parsa Roshanak (iparsw)
 Author-email: parsaroshanak@gmail.com
 Requires-Python: >=3.9, <=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 
 # Custom Intents
 
-V0.8.2
+V1.0.0
 (it's still in buggy alpha)
 
-## a simple way to create chatbots Ai, image classification Ai and more!!
+## a simple way to create chatbots Ai, image classification Ai, image generation Ai, image supper resolution Ai and more!!
 
 # installation
 
 you can install the package from pypi (pip)
 
 ```commandline
 pip install CustomIntents
@@ -28,18 +28,192 @@
 
 ![Demo1](images/img2.png)
 
 ![Demo2](images/img.png)
 
 
 
-A package build on top of keras for creating and training deep learning chatbots (text classification), binary image classification and linear regression models in just three lines of code 
+A package build on top of keras for creating and training deep learning chatbots (text classification), image classification, image generation Ai, image super resolution, style transforming and linear regression models in just three lines of code 
 
 the package is inspired by NeuralNine, neuralintents package a packege that let you build chatbot models with 3 lines of code
 
+# list of features:
+* [SuperRes class](#superres-class)
+* [ImageGenerator class](#imagegenerator-class)
+* [ChatBot class](#chatbot-class)
+* [JsonIntents](#jsonintents-class)
+* [ImageClassificator class](#imageclassificator-class)
+* [StyleTransformer class](#styletransformer-class)
+* [BinaryImageClassificator](#binaryimageclassificator-class)
+* [PLinearRegression class](#plinearregression-class)
+* [scanner moudule](#scanner-moudule)
+
+# SuperRes class
+
+## Init arguments
+```python
+def __init__(self, input_size: tuple = (300, 300),
+             upscale_factor: int = 3,
+             cpu_only: bool = False):
+```
+
+input_size : this is only required when training or finetuning
+
+upscale_factor : the upscale factor
+
+cpu_only : whether to use only CPU or not
+
+## upscale_image method
+```python
+def upscale_image(self, img,
+                  save_name: str = None,
+                  save_image: bool = True):
+```
+img : the image you want to upscale
+
+save_image : whether to save the image
+
+save_name : the name of the saved file
+
+## upscale_image_from_path method
+```python
+def upscale_image_from_path(self, img_path,
+                            save_name: str = None,
+                            save_image: bool = True)
+```
+its like upscale_image method except that it requires a path to the image
+
+## load_training_data method
+```python
+def load_training_data(self, dataset_path: str,
+                       validation_split: float = 0.2,
+                       batch_size: int = 8)
+```
+dataset_path : path to the training and validation data directory
+
+validation_split : a float between 0 and 1 where the validation split is specified
+
+batch_size : batch size
+
+## train method
+```python
+def train(self, lr: float = 0.001,
+          optimizer: str = "Adam",
+          epochs: int = 50,
+          ESPCNCallback_usage: bool = True,
+          ESPCNCallback_test_path: str = "test",
+          epoch_per_psnr: int = 20,
+          psnr_plot: bool = True,
+          model_type: str = "xs1",
+          loss_fns: list = None,
+          loss_fns_weight: list = None):
+```
+optimizer : name of the optimizer (corently supported optimizers are : Adam, Adagrad, Adamax, Adadelta, SGD, RMSprop, Nadam)
+
+epochs : number of epochs to train
+
+ESPCNCallback_usage : wether to use ESPCNCallback or not
+
+ESPCNCallback_test_path : a path to the test data directory for ESPCNCallback
+
+epoch_per_psnr : if you use ESPCNCallback it will show a sample every few epochs you can choose that number here
+
+psnr_plot : if you use ESPCNCall you can turn plutting a sample off
+
+model_type : the type of the model (there are some different types in this package but for now i recommend using using the diffault xs1)
+
+loss_fns : a list containing loss functions you want to use if you want only one loss function to use you can pass a list with only on loss functions 
+
+(corently supported loss functions are : mse, mae, mape, ssim, psnr, ipcusl (this is a custom loss function for more information read IPCUSL.md), charbonnier, tv (total variation), tvd (total variation difference))
+
+loss_fns_weight : if you use multiple loss functions the model will calculate their weighted sum and this is a list that contains their sum in this order (mse,mae,mape,ssim,psnr,ipcusl,charbonnier,tv,tvd)
+
+## fine_tuning method
+```python
+def fine_tuning(self, lr: float = 0.001,
+                epochs: int = 50,
+                model_name: str = "super_res",
+                ESPCNCallback_usage: bool = True,
+                ESPCNCallback_test_path: str = "test",
+                epoch_per_psnr: int = 20,
+                psnr_plot: bool = True,
+                recompile: bool = False,
+                optimizer: str = None,
+                loss_fns: list = None,
+                loss_fns_weight: list = None)
+```
+its almost equivalent to the train method except you should load a model first
+
+## load_model method
+
+```python
+def load_model(self, model_name: str = "super_res")
+```
+
+model_name : the name of the model
+
+## save_model method
+
+```python
+def save_model(self, model_name: str = "super_res")
+```
+
+model_name : the name of the model
+
+## benchmark method
+
+```python
+def benchmark(self, image_path: str = "testimage.jpg",
+              input_size: tuple = (300, 300))
+```
+
+this method will benchmark the model based on a single image
+
+input_size : the image will be resized to the given size image and then upscaled by model
+
+## benchmark_from_directory method
+
+```python
+def benchmark_from_directory(self, image_directory_path: str = "test",
+                             input_size: tuple = None)
+```
+
+this method will benchmark the model based on a directory of images
+
+input_size : the image will be resized to the given size image and then upscaled by model
+
+## example of training a model
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(300, 300), upscale_factor=3)
+model.load_training_data(dataset_path="dataset", batch_size=8)
+model.train(epochs=5, model_type="xs1", psnr_plot=True, loss_fns=["IPCUSL"], epoch_per_psnr=4)
+```
+## example of fine tuning a model
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(100, 100), upscale_factor=3)
+model.load_training_data(dataset_path="dataset", batch_size=32)
+model.fine_tuning(epochs=2, lr=0.00008, model_name="CSR3X-1.1.3", psnr_plot=False, loss_fns=["mse", "mae"])
+```
+## example of using the model to generate upscaled images
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(300, 300), upscale_factor=3)
+model.load_model("CSR3X-1.1.2")
+model.upscale_image_from_path(img_path="test_image_2_300x300.jpg", save_name="test_result_300x300_to_900x900_7.jpg")
+```
+
+## image example
+![DemoSuperRes](images/superres2.jpg)
+
+
 # ImageGenerator class
 you can easily use state of the art StableDiffiusion model with this class
 
 ## Init arguments
 ```python
 def __init__(self, *,
              model: str = "StableDiffusion",
```

### Comparing `CustomIntents-0.8.2/README.md` & `CustomIntents-1.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 # Custom Intents
 
-V0.8.2
+V1.0.0
 (it's still in buggy alpha)
 
-## a simple way to create chatbots Ai, image classification Ai and more!!
+## a simple way to create chatbots Ai, image classification Ai, image generation Ai, image supper resolution Ai and more!!
 
 # installation
 
 you can install the package from pypi (pip)
 
 ```commandline
 pip install CustomIntents
@@ -18,18 +18,192 @@
 
 ![Demo1](images/img2.png)
 
 ![Demo2](images/img.png)
 
 
 
-A package build on top of keras for creating and training deep learning chatbots (text classification), binary image classification and linear regression models in just three lines of code 
+A package build on top of keras for creating and training deep learning chatbots (text classification), image classification, image generation Ai, image super resolution, style transforming and linear regression models in just three lines of code 
 
 the package is inspired by NeuralNine, neuralintents package a packege that let you build chatbot models with 3 lines of code
 
+# list of features:
+* [SuperRes class](#superres-class)
+* [ImageGenerator class](#imagegenerator-class)
+* [ChatBot class](#chatbot-class)
+* [JsonIntents](#jsonintents-class)
+* [ImageClassificator class](#imageclassificator-class)
+* [StyleTransformer class](#styletransformer-class)
+* [BinaryImageClassificator](#binaryimageclassificator-class)
+* [PLinearRegression class](#plinearregression-class)
+* [scanner moudule](#scanner-moudule)
+
+# SuperRes class
+
+## Init arguments
+```python
+def __init__(self, input_size: tuple = (300, 300),
+             upscale_factor: int = 3,
+             cpu_only: bool = False):
+```
+
+input_size : this is only required when training or finetuning
+
+upscale_factor : the upscale factor
+
+cpu_only : whether to use only CPU or not
+
+## upscale_image method
+```python
+def upscale_image(self, img,
+                  save_name: str = None,
+                  save_image: bool = True):
+```
+img : the image you want to upscale
+
+save_image : whether to save the image
+
+save_name : the name of the saved file
+
+## upscale_image_from_path method
+```python
+def upscale_image_from_path(self, img_path,
+                            save_name: str = None,
+                            save_image: bool = True)
+```
+its like upscale_image method except that it requires a path to the image
+
+## load_training_data method
+```python
+def load_training_data(self, dataset_path: str,
+                       validation_split: float = 0.2,
+                       batch_size: int = 8)
+```
+dataset_path : path to the training and validation data directory
+
+validation_split : a float between 0 and 1 where the validation split is specified
+
+batch_size : batch size
+
+## train method
+```python
+def train(self, lr: float = 0.001,
+          optimizer: str = "Adam",
+          epochs: int = 50,
+          ESPCNCallback_usage: bool = True,
+          ESPCNCallback_test_path: str = "test",
+          epoch_per_psnr: int = 20,
+          psnr_plot: bool = True,
+          model_type: str = "xs1",
+          loss_fns: list = None,
+          loss_fns_weight: list = None):
+```
+optimizer : name of the optimizer (corently supported optimizers are : Adam, Adagrad, Adamax, Adadelta, SGD, RMSprop, Nadam)
+
+epochs : number of epochs to train
+
+ESPCNCallback_usage : wether to use ESPCNCallback or not
+
+ESPCNCallback_test_path : a path to the test data directory for ESPCNCallback
+
+epoch_per_psnr : if you use ESPCNCallback it will show a sample every few epochs you can choose that number here
+
+psnr_plot : if you use ESPCNCall you can turn plutting a sample off
+
+model_type : the type of the model (there are some different types in this package but for now i recommend using using the diffault xs1)
+
+loss_fns : a list containing loss functions you want to use if you want only one loss function to use you can pass a list with only on loss functions 
+
+(corently supported loss functions are : mse, mae, mape, ssim, psnr, ipcusl (this is a custom loss function for more information read IPCUSL.md), charbonnier, tv (total variation), tvd (total variation difference))
+
+loss_fns_weight : if you use multiple loss functions the model will calculate their weighted sum and this is a list that contains their sum in this order (mse,mae,mape,ssim,psnr,ipcusl,charbonnier,tv,tvd)
+
+## fine_tuning method
+```python
+def fine_tuning(self, lr: float = 0.001,
+                epochs: int = 50,
+                model_name: str = "super_res",
+                ESPCNCallback_usage: bool = True,
+                ESPCNCallback_test_path: str = "test",
+                epoch_per_psnr: int = 20,
+                psnr_plot: bool = True,
+                recompile: bool = False,
+                optimizer: str = None,
+                loss_fns: list = None,
+                loss_fns_weight: list = None)
+```
+its almost equivalent to the train method except you should load a model first
+
+## load_model method
+
+```python
+def load_model(self, model_name: str = "super_res")
+```
+
+model_name : the name of the model
+
+## save_model method
+
+```python
+def save_model(self, model_name: str = "super_res")
+```
+
+model_name : the name of the model
+
+## benchmark method
+
+```python
+def benchmark(self, image_path: str = "testimage.jpg",
+              input_size: tuple = (300, 300))
+```
+
+this method will benchmark the model based on a single image
+
+input_size : the image will be resized to the given size image and then upscaled by model
+
+## benchmark_from_directory method
+
+```python
+def benchmark_from_directory(self, image_directory_path: str = "test",
+                             input_size: tuple = None)
+```
+
+this method will benchmark the model based on a directory of images
+
+input_size : the image will be resized to the given size image and then upscaled by model
+
+## example of training a model
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(300, 300), upscale_factor=3)
+model.load_training_data(dataset_path="dataset", batch_size=8)
+model.train(epochs=5, model_type="xs1", psnr_plot=True, loss_fns=["IPCUSL"], epoch_per_psnr=4)
+```
+## example of fine tuning a model
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(100, 100), upscale_factor=3)
+model.load_training_data(dataset_path="dataset", batch_size=32)
+model.fine_tuning(epochs=2, lr=0.00008, model_name="CSR3X-1.1.3", psnr_plot=False, loss_fns=["mse", "mae"])
+```
+## example of using the model to generate upscaled images
+```python
+from CustomIntents import SuperRes
+
+model = SuperRes(input_size=(300, 300), upscale_factor=3)
+model.load_model("CSR3X-1.1.2")
+model.upscale_image_from_path(img_path="test_image_2_300x300.jpg", save_name="test_result_300x300_to_900x900_7.jpg")
+```
+
+## image example
+![DemoSuperRes](images/superres2.jpg)
+
+
 # ImageGenerator class
 you can easily use state of the art StableDiffiusion model with this class
 
 ## Init arguments
 ```python
 def __init__(self, *,
              model: str = "StableDiffusion",
```

### Comparing `CustomIntents-0.8.2/setup.py` & `CustomIntents-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CustomIntents",
-    version="0.8.2",
+    version="1.0.0",
     author="Parsa Roshanak (iparsw)",
     author_email="parsaroshanak@gmail.com",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/iparsw/custom-intent.git",
     packages=["CustomIntents", "CustomIntents.Pfunction"],
     python_requires='>=3.9, <=3.11',
```

