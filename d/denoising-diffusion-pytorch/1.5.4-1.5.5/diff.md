# Comparing `tmp/denoising-diffusion-pytorch-1.5.4.tar.gz` & `tmp/denoising-diffusion-pytorch-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.5.4.tar", last modified: Wed Mar 29 15:16:51 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.5.5.tar", last modified: Wed Apr 19 18:17:48 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.5.4.tar` & `denoising-diffusion-pytorch-1.5.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 15:16:51.711503 denoising-diffusion-pytorch-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-29 15:16:51.711503 denoising-diffusion-pytorch-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 15:16:51.707503 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    25038 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 15:16:51.711503 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-29 15:16:51.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-29 15:16:51.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 15:16:51.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-29 15:16:51.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-29 15:16:51.000000 denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 15:16:51.711503 denoising-diffusion-pytorch-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-29 15:16:41.000000 denoising-diffusion-pytorch-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:17:48.389421 denoising-diffusion-pytorch-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 18:17:48.389421 denoising-diffusion-pytorch-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:17:48.385420 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27954 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36748 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:17:48.389421 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-19 18:17:48.000000 denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:17:48.389421 denoising-diffusion-pytorch-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-19 18:17:37.000000 denoising-diffusion-pytorch-1.5.5/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.5.4/LICENSE` & `denoising-diffusion-pytorch-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/PKG-INFO` & `denoising-diffusion-pytorch-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.5.4
+Version: 1.5.5
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.5.4/README.md` & `denoising-diffusion-pytorch-1.5.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -102,43 +102,59 @@
 $ accelerate launch train.py
 ```
 
 ## Miscellaneous
 
 ### 1D Sequence
 
-By popular request, a 1D Unet + Gaussian Diffusion implementation. You will have to do the training code yourself
-
+By popular request, a 1D Unet + Gaussian Diffusion implementation.
 ```python
 import torch
-from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D
+from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D
 
 model = Unet1D(
     dim = 64,
     dim_mults = (1, 2, 4, 8),
     channels = 32
 )
 
 diffusion = GaussianDiffusion1D(
     model,
     seq_length = 128,
     timesteps = 1000,
     objective = 'pred_v'
 )
 
-training_seq = torch.rand(8, 32, 128) # features are normalized from 0 to 1
+training_seq = torch.rand(64, 32, 128) # features are normalized from 0 to 1
 loss = diffusion(training_seq)
 loss.backward()
 
+# Or using trainer
+
+trainer = Trainer1D(
+    diffusion,
+    dataset = training_seq,
+    train_batch_size = 32,
+    train_lr = 8e-5,
+    train_num_steps = 700000,         # total training steps
+    gradient_accumulate_every = 2,    # gradient accumulation steps
+    ema_decay = 0.995,                # exponential moving average decay
+    amp = True,                       # turn on mixed precision
+)
+trainer.train()
+
 # after a lot of training
 
 sampled_seq = diffusion.sample(batch_size = 4)
 sampled_seq.shape # (4, 32, 128)
-```
 
+```
+`Trainer1D` does not evaluate the generated samples in any way since the type of data is not known. 
+You could consider adding a suitable metric to the training loop yourself after doing an editable install of this package
+`pip install -e .`.
 ## Citations
 
 ```bibtex
 @inproceedings{NEURIPS2020_4c5bcfec,
     author      = {Ho, Jonathan and Jain, Ajay and Abbeel, Pieter},
     booktitle   = {Advances in Neural Information Processing Systems},
     editor      = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan and H. Lin},
```

#### html2text {}

```diff
@@ -32,27 +32,34 @@
 calculate_fid = True # whether to calculate fid during training ) trainer.train
 () ``` Samples and model checkpoints will be logged to `./results` periodically
 ## Multi-GPU Training The `Trainer` class is now equipped with ð¤
 Accelerator. You can easily do multi-gpu training in two steps using their
 `accelerate` CLI At the project root directory, where the training script is,
 run ```python $ accelerate config ``` Then, in the same directory ```python $
 accelerate launch train.py ``` ## Miscellaneous ### 1D Sequence By popular
-request, a 1D Unet + Gaussian Diffusion implementation. You will have to do the
-training code yourself ```python import torch from denoising_diffusion_pytorch
-import Unet1D, GaussianDiffusion1D model = Unet1D( dim = 64, dim_mults = (1, 2,
-4, 8), channels = 32 ) diffusion = GaussianDiffusion1D( model, seq_length =
-128, timesteps = 1000, objective = 'pred_v' ) training_seq = torch.rand(8, 32,
-128) # features are normalized from 0 to 1 loss = diffusion(training_seq)
-loss.backward() # after a lot of training sampled_seq = diffusion.sample
-(batch_size = 4) sampled_seq.shape # (4, 32, 128) ``` ## Citations ```bibtex
-@inproceedings{NEURIPS2020_4c5bcfec, author = {Ho, Jonathan and Jain, Ajay and
-Abbeel, Pieter}, booktitle = {Advances in Neural Information Processing
-Systems}, editor = {H. Larochelle and M. Ranzato and R. Hadsell and M.F. Balcan
-and H. Lin}, pages = {6840--6851}, publisher = {Curran Associates, Inc.}, title
-= {Denoising Diffusion Probabilistic Models}, url = {https://
+request, a 1D Unet + Gaussian Diffusion implementation. ```python import torch
+from denoising_diffusion_pytorch import Unet1D, GaussianDiffusion1D, Trainer1D
+model = Unet1D( dim = 64, dim_mults = (1, 2, 4, 8), channels = 32 ) diffusion =
+GaussianDiffusion1D( model, seq_length = 128, timesteps = 1000, objective =
+'pred_v' ) training_seq = torch.rand(64, 32, 128) # features are normalized
+from 0 to 1 loss = diffusion(training_seq) loss.backward() # Or using trainer
+trainer = Trainer1D( diffusion, dataset = training_seq, train_batch_size = 32,
+train_lr = 8e-5, train_num_steps = 700000, # total training steps
+gradient_accumulate_every = 2, # gradient accumulation steps ema_decay = 0.995,
+# exponential moving average decay amp = True, # turn on mixed precision )
+trainer.train() # after a lot of training sampled_seq = diffusion.sample
+(batch_size = 4) sampled_seq.shape # (4, 32, 128) ``` `Trainer1D` does not
+evaluate the generated samples in any way since the type of data is not known.
+You could consider adding a suitable metric to the training loop yourself after
+doing an editable install of this package `pip install -e .`. ## Citations
+```bibtex @inproceedings{NEURIPS2020_4c5bcfec, author = {Ho, Jonathan and Jain,
+Ajay and Abbeel, Pieter}, booktitle = {Advances in Neural Information
+Processing Systems}, editor = {H. Larochelle and M. Ranzato and R. Hadsell and
+M.F. Balcan and H. Lin}, pages = {6840--6851}, publisher = {Curran Associates,
+Inc.}, title = {Denoising Diffusion Probabilistic Models}, url = {https://
 proceedings.neurips.cc/paper/2020/file/4c5bcfec8584af0d967f1ab10179ca4b-
 Paper.pdf}, volume = {33}, year = {2020} } ``` ```bibtex @InProceedings{pmlr-
 v139-nichol21a, title = {Improved Denoising Diffusion Probabilistic Models},
 author = {Nichol, Alexander Quinn and Dhariwal, Prafulla}, booktitle =
 {Proceedings of the 38th International Conference on Machine Learning}, pages =
 {8162--8171}, year = {2021}, editor = {Meila, Marina and Zhang, Tong}, volume =
 {139}, series = {Proceedings of Machine Learning Research}, month = {18--24
```

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,9 +2,9 @@
 
 from denoising_diffusion_pytorch.learned_gaussian_diffusion import LearnedGaussianDiffusion
 from denoising_diffusion_pytorch.continuous_time_gaussian_diffusion import ContinuousTimeGaussianDiffusion
 from denoising_diffusion_pytorch.weighted_objective_gaussian_diffusion import WeightedObjectiveGaussianDiffusion
 from denoising_diffusion_pytorch.elucidated_diffusion import ElucidatedDiffusion
 from denoising_diffusion_pytorch.v_param_continuous_time_gaussian_diffusion import VParamContinuousTimeGaussianDiffusion
 
-from denoising_diffusion_pytorch.denoising_diffusion_pytorch_1d import GaussianDiffusion1D, Unet1D
+from denoising_diffusion_pytorch.denoising_diffusion_pytorch_1d import GaussianDiffusion1D, Unet1D, Trainer1D
```

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import math
+from multiprocessing import cpu_count
+from pathlib import Path
 from random import random
 from functools import partial
 from collections import namedtuple
 
 import torch
+from accelerate import Accelerator
+from ema_pytorch import EMA
 from torch import nn, einsum
 import torch.nn.functional as F
 
 from einops import rearrange, reduce
 from einops.layers.torch import Rearrange
+from torch.optim import Adam
+from torch.utils.data import Dataset, DataLoader
 
 from tqdm.auto import tqdm
 
+from denoising_diffusion_pytorch.version import __version__
+
 # constants
 
 ModelPrediction =  namedtuple('ModelPrediction', ['pred_noise', 'pred_x_start'])
 
 # helpers functions
 
 def exists(x):
@@ -709,7 +717,174 @@
     def forward(self, img, *args, **kwargs):
         b, c, n, device, seq_length, = *img.shape, img.device, self.seq_length
         assert n == seq_length, f'seq length must be {seq_length}'
         t = torch.randint(0, self.num_timesteps, (b,), device=device).long()
 
         img = self.normalize(img)
         return self.p_losses(img, t, *args, **kwargs)
+
+# trainer class
+
+class Trainer1D(object):
+    def __init__(
+        self,
+        diffusion_model: GaussianDiffusion1D,
+        dataset: Dataset,
+        *,
+        train_batch_size = 16,
+        gradient_accumulate_every = 1,
+        train_lr = 1e-4,
+        train_num_steps = 100000,
+        ema_update_every = 10,
+        ema_decay = 0.995,
+        adam_betas = (0.9, 0.99),
+        save_and_sample_every = 1000,
+        num_samples = 25,
+        results_folder = './results',
+        amp = False,
+        fp16 = False,
+        split_batches = True,
+    ):
+        super().__init__()
+
+        # accelerator
+
+        self.accelerator = Accelerator(
+            split_batches = split_batches,
+            mixed_precision = 'fp16' if fp16 else 'no'
+        )
+
+        self.accelerator.native_amp = amp
+
+        # model
+
+        self.model = diffusion_model
+        self.channels = diffusion_model.channels
+
+        # sampling and training hyperparameters
+
+        assert has_int_squareroot(num_samples), 'number of samples must have an integer square root'
+        self.num_samples = num_samples
+        self.save_and_sample_every = save_and_sample_every
+
+        self.batch_size = train_batch_size
+        self.gradient_accumulate_every = gradient_accumulate_every
+
+        self.train_num_steps = train_num_steps
+
+        # dataset and dataloader
+
+        dl = DataLoader(dataset, batch_size = train_batch_size, shuffle = True, pin_memory = True, num_workers = cpu_count())
+
+        dl = self.accelerator.prepare(dl)
+        self.dl = cycle(dl)
+
+        # optimizer
+
+        self.opt = Adam(diffusion_model.parameters(), lr = train_lr, betas = adam_betas)
+
+        # for logging results in a folder periodically
+
+        if self.accelerator.is_main_process:
+            self.ema = EMA(diffusion_model, beta = ema_decay, update_every = ema_update_every)
+            self.ema.to(self.device)
+
+        self.results_folder = Path(results_folder)
+        self.results_folder.mkdir(exist_ok = True)
+
+        # step counter state
+
+        self.step = 0
+
+        # prepare model, dataloader, optimizer with accelerator
+
+        self.model, self.opt = self.accelerator.prepare(self.model, self.opt)
+
+    @property
+    def device(self):
+        return self.accelerator.device
+
+    def save(self, milestone):
+        if not self.accelerator.is_local_main_process:
+            return
+
+        data = {
+            'step': self.step,
+            'model': self.accelerator.get_state_dict(self.model),
+            'opt': self.opt.state_dict(),
+            'ema': self.ema.state_dict(),
+            'scaler': self.accelerator.scaler.state_dict() if exists(self.accelerator.scaler) else None,
+            'version': __version__
+        }
+
+        torch.save(data, str(self.results_folder / f'model-{milestone}.pt'))
+
+    def load(self, milestone):
+        accelerator = self.accelerator
+        device = accelerator.device
+
+        data = torch.load(str(self.results_folder / f'model-{milestone}.pt'), map_location=device)
+
+        model = self.accelerator.unwrap_model(self.model)
+        model.load_state_dict(data['model'])
+
+        self.step = data['step']
+        self.opt.load_state_dict(data['opt'])
+        if self.accelerator.is_main_process:
+            self.ema.load_state_dict(data["ema"])
+
+        if 'version' in data:
+            print(f"loading from version {data['version']}")
+
+        if exists(self.accelerator.scaler) and exists(data['scaler']):
+            self.accelerator.scaler.load_state_dict(data['scaler'])
+
+    def train(self):
+        accelerator = self.accelerator
+        device = accelerator.device
+
+        with tqdm(initial = self.step, total = self.train_num_steps, disable = not accelerator.is_main_process) as pbar:
+
+            while self.step < self.train_num_steps:
+
+                total_loss = 0.
+
+                for _ in range(self.gradient_accumulate_every):
+                    data = next(self.dl).to(device)
+
+                    with self.accelerator.autocast():
+                        loss = self.model(data)
+                        loss = loss / self.gradient_accumulate_every
+                        total_loss += loss.item()
+
+                    self.accelerator.backward(loss)
+
+                accelerator.clip_grad_norm_(self.model.parameters(), 1.0)
+                pbar.set_description(f'loss: {total_loss:.4f}')
+
+                accelerator.wait_for_everyone()
+
+                self.opt.step()
+                self.opt.zero_grad()
+
+                accelerator.wait_for_everyone()
+
+                self.step += 1
+                if accelerator.is_main_process:
+                    self.ema.update()
+
+                    if self.step != 0 and self.step % self.save_and_sample_every == 0:
+                        self.ema.ema_model.eval()
+
+                        with torch.no_grad():
+                            milestone = self.step // self.save_and_sample_every
+                            batches = num_to_groups(self.num_samples, self.batch_size)
+                            all_samples_list = list(map(lambda n: self.ema.ema_model.sample(batch_size=n), batches))
+                        #
+                        all_samples = torch.cat(all_samples_list, dim = 0)
+                        #
+                        torch.save(all_samples, str(self.results_folder / f'sample-{milestone}.png'))
+                        self.save(milestone)
+
+                pbar.update(1)
+
+        accelerator.print('training complete')
```

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.5.4
+Version: 1.5.5
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.5.4/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.5.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.5.4/setup.py` & `denoising-diffusion-pytorch-1.5.5/setup.py`

 * *Files identical despite different names*

