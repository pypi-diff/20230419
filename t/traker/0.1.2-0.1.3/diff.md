# Comparing `tmp/traker-0.1.2.tar.gz` & `tmp/traker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traker-0.1.2.tar", last modified: Wed Apr 12 17:51:30 2023, max compression
+gzip compressed data, was "traker-0.1.3.tar", last modified: Wed Apr 19 18:30:35 2023, max compression
```

## Comparing `traker-0.1.2.tar` & `traker-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:51:30.688856 traker-0.1.2/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-04-12 17:51:30.676856 traker-0.1.2/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3311 2023-04-10 13:58:42.000000 traker-0.1.2/README.md
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-04-12 17:51:30.692856 traker-0.1.2/setup.cfg
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      756 2023-04-12 17:48:19.000000 traker-0.1.2/setup.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:51:30.240849 traker-0.1.2/tests/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     5575 2023-04-12 13:40:47.000000 traker-0.1.2/tests/test_accuracy.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     2989 2023-04-11 13:28:04.000000 traker-0.1.2/tests/test_cifar_accuracy.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4143 2023-04-10 13:58:43.000000 traker-0.1.2/tests/test_class.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4571 2023-03-27 15:11:24.000000 traker-0.1.2/tests/test_integration_cifar.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1545 2023-03-27 15:11:24.000000 traker-0.1.2/tests/test_integration_clip.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    10812 2023-03-27 15:11:24.000000 traker-0.1.2/tests/test_jl.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4065 2023-03-27 15:11:24.000000 traker-0.1.2/tests/test_parallel.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3116 2023-04-12 17:48:19.000000 traker-0.1.2/tests/test_rademacher.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:51:30.468853 traker-0.1.2/trak/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       72 2023-04-12 17:48:19.000000 traker-0.1.2/trak/__init__.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     8766 2023-03-28 20:01:05.000000 traker-0.1.2/trak/gradient_computers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    20281 2023-04-12 17:48:19.000000 traker-0.1.2/trak/modelout_functions.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11180 2023-04-12 17:48:19.000000 traker-0.1.2/trak/projectors.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    12660 2023-03-27 15:11:24.000000 traker-0.1.2/trak/savers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3499 2023-03-27 15:11:24.000000 traker-0.1.2/trak/score_computers.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    16926 2023-04-12 17:48:19.000000 traker-0.1.2/trak/traker.py
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1527 2023-03-27 15:11:24.000000 traker-0.1.2/trak/utils.py
-drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-12 17:51:30.640855 traker-0.1.2/traker.egg-info/
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/PKG-INFO
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      525 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/SOURCES.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/dependency_links.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       96 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/requires.txt
--rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        5 2023-04-12 17:51:28.000000 traker-0.1.2/traker.egg-info/top_level.txt
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-19 18:30:35.829877 traker-0.1.3/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-04-19 18:30:35.825877 traker-0.1.3/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3338 2023-04-19 18:30:13.000000 traker-0.1.3/README.md
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       38 2023-04-19 18:30:35.833877 traker-0.1.3/setup.cfg
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      756 2023-04-19 18:30:13.000000 traker-0.1.3/setup.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-19 18:30:35.649875 traker-0.1.3/tests/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     5575 2023-04-12 13:40:47.000000 traker-0.1.3/tests/test_accuracy.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     2989 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_cifar_accuracy.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4143 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_class.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4571 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_integration_cifar.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1545 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_integration_clip.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    10812 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_jl.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     4065 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_parallel.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3116 2023-04-18 20:47:31.000000 traker-0.1.3/tests/test_rademacher.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-19 18:30:35.749876 traker-0.1.3/trak/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       72 2023-04-19 18:30:13.000000 traker-0.1.3/trak/__init__.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     8766 2023-04-18 20:47:31.000000 traker-0.1.3/trak/gradient_computers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    20281 2023-04-18 20:47:31.000000 traker-0.1.3/trak/modelout_functions.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    11180 2023-04-18 20:47:31.000000 traker-0.1.3/trak/projectors.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    12660 2023-04-18 20:47:31.000000 traker-0.1.3/trak/savers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     3499 2023-04-18 20:47:31.000000 traker-0.1.3/trak/score_computers.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)    18787 2023-04-19 18:30:13.000000 traker-0.1.3/trak/traker.py
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)     1527 2023-04-18 20:47:31.000000 traker-0.1.3/trak/utils.py
+drwxrwxr-x   0 krisgrg  (25606) krisgrg  (25606)        0 2023-04-19 18:30:35.809877 traker-0.1.3/traker.egg-info/
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      248 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/PKG-INFO
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)      525 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/SOURCES.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        1 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/dependency_links.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)       96 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/requires.txt
+-rw-rw-r--   0 krisgrg  (25606) krisgrg  (25606)        5 2023-04-19 18:30:35.000000 traker-0.1.3/traker.egg-info/top_level.txt
```

### Comparing `traker-0.1.2/README.md` & `traker-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,29 @@
-[![PyPI version](https://badge.fury.io/py/traker.svg)](https://badge.fury.io/py/traker)
 [![arXiv](https://img.shields.io/badge/arXiv-2303.14186-b31b1b.svg?style=flat-square)](https://arxiv.org/abs/2303.14186)
+[![PyPI version](https://badge.fury.io/py/traker.svg)](https://badge.fury.io/py/traker)
+
+# TRAK: Attributing Model Behavior at Scale
 
 [[docs & tutorials]](https://trak.readthedocs.io/en/latest/)
-[[paper]](https://arxiv.org/abs/2303.14186)
 [[blog post]](https://gradientscience.org/trak/)
 [[website]](https://trak.csail.mit.edu)
 
-# TRAK: Attributing Model Behavior at Scale
-
 In our [paper](https://arxiv.org/abs/2303.14186), we introduce a new data attribution method called `TRAK` (Tracing with the
 Randomly-Projected After Kernel). Using `TRAK`, you can make  accurate
 counterfactual predictions (e.g., answers to questions of the form “what would
 happen to this prediction if these examples are removed from the training set?").
 Computing  data attribution with  TRAK is 2-3 orders of magnitude cheaper than
 comparably effective methods, e.g., see our evaluation on:
 
 ![Main figure](/docs/assets/main_figure.png)
 
-## Citation
-If you use this code in your work, please cite using the following BibTeX entry:
-```
-@inproceedings{park2023trak,
-  title = {TRAK: Attributing Model Behavior at Scale},
-  author = {Sung Min Park and Kristian Georgiev and Andrew Ilyas and Guillaume Leclerc and Aleksander Madry},
-  booktitle = {Arxiv preprint arXiv:2303.14186},
-  year = {2023}
-}
-```
-
 ## Usage
 
-
-[[Quickstart]](https://trak.readthedocs.io/en/latest/quickstart.html)
+[[quickstart]](https://trak.readthedocs.io/en/latest/quickstart.html)
+[[pre-computed TRAK scores for CIFAR-10]](https://colab.research.google.com/drive/1Mlpzno97qpI3UC1jpOATXEHPD-lzn9Wg?usp=sharing)
 
 Check [our docs](https://trak.readthedocs.io/en/latest/) for more detailed examples and
 tutorials on how to use `TRAK`.  Below, we provide a brief blueprint of using `TRAK`'s API to compute attribution scores.
 
 ### Make a `TRAKer` instance
 
 ```python
@@ -70,14 +58,25 @@
 
 scores = traker.finalize_scores()
 ```
 
 ## Examples
 You can find several end-to-end examples in the `examples/` directory.
 
+## Citation
+If you use this code in your work, please cite using the following BibTeX entry:
+```
+@inproceedings{park2023trak,
+  title = {TRAK: Attributing Model Behavior at Scale},
+  author = {Sung Min Park and Kristian Georgiev and Andrew Ilyas and Guillaume Leclerc and Aleksander Madry},
+  booktitle = {Arxiv preprint arXiv:2303.14186},
+  year = {2023}
+}
+```
+
 ## Installation
 
 To install the version of our package which contains a fast, custom `CUDA`
 kernel for the JL projection step, use
 ```bash
 pip install traker[fast]
 ```
@@ -89,13 +88,12 @@
 pip install traker
 ```
 
 ## Questions?
 
 Please send an email to trak@mit.edu
 
-## Maintainers:
+## Maintainers
 
 [Kristian Georgiev](https://twitter.com/kris_georgiev1)<br>
 [Andrew Ilyas](https://twitter.com/andrew_ilyas)<br>
-[Guillaume Leclerc](https://twitter.com/gpoleclerc)<br>
 [Sung Min Park](https://twitter.com/smsampark)
```

### Comparing `traker-0.1.2/setup.py` & `traker-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(name="traker",
-      version="0.1.2",
+      version="0.1.3",
       description="TRAK: Attributing Model Behavior at Scale",
       long_description="Check https://trak.csail.mit.edu/ to learn more about TRAK",
       author="MadryLab",
       author_email='trak@mit.edu',
       license_files=('LICENSE.txt', ),
       packages=['trak'],
       install_requires=[
```

### Comparing `traker-0.1.2/tests/test_accuracy.py` & `traker-0.1.3/tests/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/tests/test_cifar_accuracy.py` & `traker-0.1.3/tests/test_cifar_accuracy.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/tests/test_class.py` & `traker-0.1.3/tests/test_class.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/tests/test_integration_cifar.py` & `traker-0.1.3/tests/test_integration_cifar.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/tests/test_integration_clip.py` & `traker-0.1.3/tests/test_integration_clip.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/tests/test_jl.py` & `traker-0.1.3/tests/test_jl.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/tests/test_parallel.py` & `traker-0.1.3/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/tests/test_rademacher.py` & `traker-0.1.3/tests/test_rademacher.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/trak/gradient_computers.py` & `traker-0.1.3/trak/gradient_computers.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/trak/modelout_functions.py` & `traker-0.1.3/trak/modelout_functions.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/trak/projectors.py` & `traker-0.1.3/trak/projectors.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/trak/savers.py` & `traker-0.1.3/trak/savers.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/trak/score_computers.py` & `traker-0.1.3/trak/score_computers.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/trak/traker.py` & `traker-0.1.3/trak/traker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .modelout_functions import AbstractModelOutput, TASK_TO_MODELOUT
-from .projectors import ProjectionType, AbstractProjector, CudaProjector
+from .projectors import ProjectionType, AbstractProjector, CudaProjector, BasicProjector
 from .gradient_computers import FunctionalGradientComputer,\
                                 AbstractGradientComputer
-from .score_computers import BasicScoreComputer
-from .savers import MmapSaver, ModelIDException
+from .score_computers import AbstractScoreComputer, BasicScoreComputer
+from .savers import AbstractSaver, MmapSaver, ModelIDException
 from .utils import get_num_params
 
 from typing import Iterable, Optional, Union
 from pathlib import Path
 from tqdm import tqdm
 from torch import Tensor
 
@@ -27,14 +27,16 @@
                  task: Union[AbstractModelOutput, str],
                  train_set_size: int,
                  save_dir: str = './trak_results',
                  load_from_save_dir: bool = True,
                  device: Union[str, torch.device] = 'cuda',
                  gradient_computer: AbstractGradientComputer = FunctionalGradientComputer,
                  projector: Optional[AbstractProjector] = None,
+                 saver: Optional[AbstractSaver] = None,
+                 score_computer: Optional[AbstractScoreComputer] = None,
                  proj_dim: int = 2048,
                  ) -> None:
         """
 
         Args:
             model (torch.nn.Module):
                 model to use for TRAK
@@ -62,14 +64,21 @@
                 :class:`.AbstractGradientComputer` for more details. Defaults to
                 :class:`.FunctionalGradientComputer`.
             projector (Optional[AbstractProjector], optional):
                 Either set :code:`proj_dim` and a :class:`.CudaProjector`
                 Rademacher projector will be used or give a custom subclass of
                 :class:`.AbstractProjector` class and leave :code:`proj_dim` as
                 None. Defaults to None.
+            saver (Optional[AbstractSaver], optional):
+                Class to use for saving intermediate results and final TRAK
+                scores to RAM/disk. If None, the :class:`.MmapSaver` will
+                be used. Defaults to None.
+            score_computer (Optional[AbstractScoreComputer], optional):
+                Class to use for computing the final TRAK scores. If None, the
+                :class:`.BasicScoreComputer` will be used. Defaults to None.
             proj_dim (int, optional):
                 Dimension of the projected TRAK features. See Section 4.3 of
                 `our paper <https://arxiv.org/abs/2303.14186>`_ for more
                 details. Defaults to 2048.
 
         """
 
@@ -87,25 +96,30 @@
         if type(self.task) is str:
             self.task = TASK_TO_MODELOUT[(self.task, gradient_computer.is_functional)]
 
         self.gradient_computer = gradient_computer(model=self.model,
                                                    modelout_fn=self.task,
                                                    grad_dim=self.num_params)
 
-        self.score_computer = BasicScoreComputer(device=self.device)
+        if score_computer is None:
+            score_computer = BasicScoreComputer
+        self.score_computer = score_computer(device=self.device)
 
         metadata = {
             'JL dimension': self.projector.proj_dim,
             'JL matrix type': self.projector.proj_type,
         }
-        self.saver = MmapSaver(save_dir=self.save_dir,
-                               metadata=metadata,
-                               train_set_size=self.train_set_size,
-                               proj_dim=self.proj_dim,
-                               load_from_save_dir=self.load_from_save_dir)
+
+        if saver is None:
+            saver = MmapSaver
+        self.saver = saver(save_dir=self.save_dir,
+                           metadata=metadata,
+                           train_set_size=self.train_set_size,
+                           proj_dim=self.proj_dim,
+                           load_from_save_dir=self.load_from_save_dir)
 
     def init_projector(self, projector, proj_dim) -> None:
         """ Initialize the projector for a traker class
 
         Args:
             projector (AbstractProjector):
                 JL projector
@@ -113,19 +127,31 @@
         """
 
         self.projector = projector
         if projector is not None:
             self.proj_dim = self.projector.proj_dim
         else:
             self.proj_dim = proj_dim
-            self.projector = CudaProjector(grad_dim=self.num_params,
-                                           proj_dim=self.proj_dim,
-                                           seed=0,
-                                           proj_type=ProjectionType.rademacher,
-                                           device=self.device)
+            try:
+                import fast_jl
+                test_gradient = ch.ones(1, self.num_params).cuda()
+                num_sms = ch.cuda.get_device_properties('cuda').multi_processor_count
+                fast_jl.project_rademacher_8(test_gradient, self.proj_dim, 0, num_sms)
+                projector = CudaProjector
+
+            except (ImportError, RuntimeError, AttributeError) as e:
+                print(f'Could not use CudaProjector.\nReason: {str(e)}')
+                print('Defaulting to BasicProjector.')
+                projector = BasicProjector
+
+            self.projector = projector(grad_dim=self.num_params,
+                                       proj_dim=self.proj_dim,
+                                       seed=0,
+                                       proj_type=ProjectionType.rademacher,
+                                       device=self.device)
 
     def load_checkpoint(self,
                         checkpoint: Iterable[Tensor],
                         model_id: int,
                         _allow_featurizing_already_registered=None) -> None:
         """ Loads state dictionary for the given checkpoint; initializes arrays
         to store TRAK features for that checkpoint, tied to the model ID.
@@ -318,28 +344,33 @@
         grads = self.projector.project(grads, model_id=self.saver.current_model_id)
 
         self.saver.current_target_grads[inds] = grads.cpu().clone().detach()
 
     def finalize_scores(self,
                         model_ids: Iterable[int] = None,
                         del_grads: bool = False,
+                        allow_skip: bool = False,
                         exp_name: str = None) -> Tensor:
         """ This method computes the final TRAK scores for the given targets,
         train samples, and model checkpoints (specified by model IDs).
 
         Args:
             model_ids (Iterable[int], optional):
                 A list of model IDs for which
                 scores should be finalized. If None, scores are computed
                 for all model IDs in the :code:`save_dir` of the :class:`.TRAKer`
                 class. Defaults to None.
             del_grads (bool, optional):
                 If True, the target gradients (intermediate results) are deleted
                 from the internal store of the :class:`.TRAKer` class.  Defaults
-                to True.
+                to False.
+            allow_skip (bool, optional):
+                If True, raises only a warning, instead of an error, when target
+                gradients are not computed for a given model ID. Defaults to
+                False.
             exp_name (str, optional):
                 Used to name the scores :code:`.npy` array produced by this
                 method in the :code:`save_dir` of the :class:`.TRAKer` class. If
                 None, a random uuid is generated.  Defaults to None.
 
         Returns:
             Tensor: TRAK scores
@@ -355,15 +386,22 @@
         _scores = ch.zeros(self.train_set_size,
                            self.saver.num_targets,
                            device=self.device)
         _avg_out_to_losses = ch.zeros(self.saver.train_set_size, 1, device=self.device)
 
         for j, model_id in enumerate(tqdm(model_ids, desc='Finalizing scores for all model IDs..')):
             self.saver.load_store(model_id)
-            self.saver.load_target_store(model_id, self.saver.num_targets)
+            try:
+                self.saver.load_target_store(model_id, self.saver.num_targets)
+            except OSError as e:
+                if allow_skip:
+                    print(f'Could not read target gradients for model ID {model_id}. Skipping.')
+                    continue
+                else:
+                    raise e
 
             # TODO: currently this is breaking abstraction -- either define dict
             # items in abstract __init__, or don't access them here
             if self.saver.model_ids[self.saver.current_model_id]['finalized'] == 0:
                 print(f'Model ID {self.saver.current_model_id} not finalized, cannot score')
                 continue
```

### Comparing `traker-0.1.2/trak/utils.py` & `traker-0.1.3/trak/utils.py`

 * *Files identical despite different names*

### Comparing `traker-0.1.2/traker.egg-info/SOURCES.txt` & `traker-0.1.3/traker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

