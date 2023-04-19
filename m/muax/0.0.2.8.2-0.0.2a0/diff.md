# Comparing `tmp/muax-0.0.2.8.2.tar.gz` & `tmp/muax-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muax-0.0.2.8.2.tar", last modified: Wed Apr 19 18:24:25 2023, max compression
+gzip compressed data, was "muax-0.0.2a0.tar", last modified: Wed Jan 18 20:25:19 2023, max compression
```

## Comparing `muax-0.0.2.8.2.tar` & `muax-0.0.2a0.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:24:25.456444 muax-0.0.2.8.2/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6322 2023-04-19 18:24:25.456444 muax-0.0.2.8.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5897 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:24:25.455444 muax-0.0.2.8.2/muax/
--rw-r--r--   0 root         (0) root         (0)      607 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7278 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/episode_tracer.py
--rw-r--r--   0 root         (0) root         (0)     2994 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/loss.py
--rw-r--r--   0 root         (0) root         (0)    20353 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/model.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/nn.py
--rw-r--r--   0 root         (0) root         (0)     8348 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/replay_buffer.py
--rw-r--r--   0 root         (0) root         (0)     1694 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/test.py
--rw-r--r--   0 root         (0) root         (0)     9071 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/train.py
--rw-r--r--   0 root         (0) root         (0)     6089 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/utils.py
--rw-r--r--   0 root         (0) root         (0)    17288 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/muax/wrappers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 18:24:25.455444 muax-0.0.2.8.2/muax.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6322 2023-04-19 18:24:25.000000 muax-0.0.2.8.2/muax.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-19 18:24:25.000000 muax-0.0.2.8.2/muax.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 18:24:25.000000 muax-0.0.2.8.2/muax.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-04-19 18:24:25.000000 muax-0.0.2.8.2/muax.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-19 18:24:25.000000 muax-0.0.2.8.2/muax.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 18:24:25.456444 muax-0.0.2.8.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      812 2023-04-19 18:24:13.000000 muax-0.0.2.8.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 20:25:19.294833 muax-0.0.2a0/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-01-18 20:25:19.293833 muax-0.0.2a0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      105 2023-01-18 20:24:35.000000 muax-0.0.2a0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 20:25:19.291833 muax-0.0.2a0/examples/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-01-18 20:24:35.000000 muax-0.0.2a0/examples/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 20:25:19.292833 muax-0.0.2a0/muax/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-18 20:24:35.000000 muax-0.0.2a0/muax/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6728 2023-01-18 20:24:35.000000 muax-0.0.2a0/muax/episode_tracer.py
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-01-18 20:24:35.000000 muax-0.0.2a0/muax/model.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-01-18 20:24:35.000000 muax-0.0.2a0/muax/nn.py
+-rw-r--r--   0 root         (0) root         (0)     7778 2023-01-18 20:24:35.000000 muax-0.0.2a0/muax/replay_buffer.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-01-18 20:24:35.000000 muax-0.0.2a0/muax/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-18 20:25:19.293833 muax-0.0.2a0/muax.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-01-18 20:25:19.000000 muax-0.0.2a0/muax.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2023-01-18 20:25:19.000000 muax-0.0.2a0/muax.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-18 20:25:19.000000 muax-0.0.2a0/muax.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-01-18 20:25:19.000000 muax-0.0.2a0/muax.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-01-18 20:25:19.000000 muax-0.0.2a0/muax.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-01-18 20:25:19.294833 muax-0.0.2a0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      657 2023-01-18 20:24:47.000000 muax-0.0.2a0/setup.py
```

### Comparing `muax-0.0.2.8.2/muax/episode_tracer.py` & `muax-0.0.2a0/muax/episode_tracer.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 from abc import ABC, abstractmethod
 from typing import Any, Tuple
 import dataclasses
 from dataclasses import dataclass
 from collections import deque 
 from itertools import islice
-import numpy as np 
 import jax
 from jax import numpy as jnp
 
 from .utils import sliceable_deque
 
 
 @dataclass
@@ -48,17 +47,14 @@
     pi: Any = 0.
     w: float = 1.
 
     def __iter__(self):
       for field in dataclasses.fields(self):
         yield getattr(self, field.name)
 
-    def __getitem__(self, index):
-      return Transition(*(_attr[index] for _attr in self))
-
 def flatten_transition_func(transition: Transition) -> Tuple:
   return iter(transition), None 
 
 def unflatten_transition_func(treedef, leaves) -> Transition:
   return Transition(*leaves)
 
 jax.tree_util.register_pytree_node(
@@ -101,15 +97,15 @@
 
     @abstractmethod
     def pop(self):
         r"""
         Pop a single transition from the cache.
         Returns
         -------
-        transition : An instance of Transition
+        transition : 
             
         """
         pass
 
 
 class NStep(BaseTracer):
     r"""
@@ -129,22 +125,19 @@
 
     def __init__(self, n, gamma):
         self.n = int(n)
         self.gamma = float(gamma)
         self.reset()
 
     def reset(self):
-        r"""
-        Reset the cache to the initial state.
-        """
         self._deque_s = sliceable_deque([])
         self._deque_r = sliceable_deque([])
         self._done = False
-        self._gammas = np.power(self.gamma, np.arange(self.n))
-        self._gamman = np.power(self.gamma, self.n)
+        self._gammas = jnp.power(self.gamma, jnp.arange(self.n))
+        self._gamman = jnp.power(self.gamma, self.n)
 
     def add(self, obs, a, r, done, v=0.0, pi=0.0, w=1.0):
         # if self._done and len(self):
         #     raise EpisodeDoneError(
         #         "please flush cache (or repeatedly call popleft) before appending new transitions")
 
         self._deque_s.append((obs, a, v, pi, w))
@@ -154,55 +147,44 @@
     def __len__(self):
         return len(self._deque_s)
 
     def __bool__(self):
         return bool(len(self)) and (self._done or len(self) > self.n)
 
     def pop(self):
-        r"""
-        Pops a single transition from the cache. Computes n-step bootstrapping value.
-        Returns
-        -------
-        transition : An instance of Transition
-            
-        """
         # if not self:
         #     raise InsufficientCacheError(
         #         "cache needs to receive more transitions before it can be popped from")
 
         # pop state-action (propensities) pair
         obs, a, v, pi, w = self._deque_s.popleft()
 
         # n-step partial return
-        rs = np.array(self._deque_r[:self.n])
-        Rn = np.sum(self._gammas[:len(rs)] * rs).item()
+        rs = jnp.array(self._deque_r[:self.n])
+        Rn = jnp.sum(self._gammas[:len(rs)] * rs).item()
         r = self._deque_r.popleft()
 
         # keep in mind that we've already popped 
         if len(self) >= self.n:
             obs_next, a_next, v_next, pi_next, _ = self._deque_s[self.n - 1]
             done = False
             gamman = self._gamman
         else:
             # no more bootstrapping
-            v_next = 0
-            done = True
-            gamman = self._gammas[len(rs) - 1]
+            obs_next, a_next, v_next, pi_next, done = obs, a, v, pi, True
+            gamman = self._gammas[len(rs)]
         
         Rn += v_next * gamman
 
         return Transition(obs=obs, a=a, r=r, done=done, Rn=Rn, v=v, pi=pi, w=w)
 
 
 class PNStep(NStep):
     r"""
     A short-term cache for :math:`n`-step bootstrapping with priority.
-    The weight `w` is calcualted as: `w=abs(v - Rn) ** alpha`, 
-    where `v` is the value predicted from the model, 
-    `Rn` is the n-step bootstrapping value calculated from the rewards.
 
     Parameters
     ----------
     n : positive int
 
         The number of steps over which to bootstrap.
 
@@ -222,27 +204,26 @@
         #     raise InsufficientCacheError(
         #         "cache needs to receive more transitions before it can be popped from")
 
         # pop state-action (propensities) pair
         obs, a, v, pi, w = self._deque_s.popleft()
 
         # n-step partial return
-        rs = np.array(self._deque_r[:self.n])
-        Rn = np.sum(self._gammas[:len(rs)] * rs).item()
+        rs = jnp.array(self._deque_r[:self.n])
+        Rn = jnp.sum(self._gammas[:len(rs)] * rs).item()
         r = self._deque_r.popleft()
 
         # keep in mind that we've already popped 
         if len(self) >= self.n:
             obs_next, a_next, v_next, pi_next, _ = self._deque_s[self.n - 1]
             done = False
             gamman = self._gamman
         else:
             # no more bootstrapping
-            v_next = 0
-            done = True
-            gamman = self._gammas[len(rs) - 1]
+            obs_next, a_next, v_next, pi_next, done = obs, a, v, pi, True
+            gamman = self._gammas[len(rs)]
         
         Rn += v_next * gamman
 
         w = abs(v - Rn) ** self.alpha
 
         return Transition(obs=obs, a=a, r=r, done=done, Rn=Rn, v=v, pi=pi, w=w)
```

### Comparing `muax-0.0.2.8.2/muax/nn.py` & `muax-0.0.2a0/muax/nn.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,77 +4,58 @@
 
 
 class Representation(hk.Module):
   def __init__(self, embedding_dim, name='representation'):
     super().__init__(name=name)
 
     self.repr_func = hk.Sequential([
-        hk.Linear(embedding_dim)
+        hk.Linear(embedding_dim), jax.nn.relu
     ])
 
   def __call__(self, obs):
     s = self.repr_func(obs)
     return s 
 
 
 class Prediction(hk.Module):
-  def __init__(self, num_actions, full_support_size, name='prediction'):
+  def __init__(self, num_actions, name='prediction'):
     super().__init__(name=name)        
     
     self.v_func = hk.Sequential([
-        hk.Linear(16), jax.nn.elu,
-        hk.Linear(full_support_size)
+        hk.Linear(16), jax.nn.relu,
+        hk.Linear(1)
     ])
     self.pi_func = hk.Sequential([
-        hk.Linear(16), jax.nn.elu,
+        hk.Linear(16), jax.nn.relu,
         hk.Linear(num_actions)
     ])
   
   def __call__(self, s):
     v = self.v_func(s)
     logits = self.pi_func(s)
     logits = jax.nn.softmax(logits, axis=-1)
     return v, logits
 
 
 class Dynamic(hk.Module):
-  def __init__(self, embedding_dim, num_actions, full_support_size, name='dynamic'):
+  def __init__(self, embedding_dim, num_actions, name='dynamic'):
     super().__init__(name=name)
     
     self.ns_func = hk.Sequential([
-        hk.Linear(16), jax.nn.elu,
+        hk.Linear(16), jax.nn.relu,
         hk.Linear(embedding_dim)
     ])
     self.r_func = hk.Sequential([
-        hk.Linear(16), jax.nn.elu,
-        hk.Linear(full_support_size)
+        hk.Linear(16), jax.nn.relu,
+        hk.Linear(1)
     ])
     self.cat_func = jax.jit(lambda s, a: 
                             jnp.concatenate([s, jax.nn.one_hot(a, num_actions)],
                                             axis=1)
                             )
   
   def __call__(self, s, a):
     sa = self.cat_func(s, a)
     r = self.r_func(sa)
     ns = self.ns_func(sa)
     return r, ns
-
-
-def _init_representation_func(representation_module, embedding_dim):
-    def representation_func(obs):
-      repr_model = representation_module(embedding_dim)
-      return repr_model(obs)
-    return representation_func
-  
-def _init_prediction_func(prediction_module, num_actions, full_support_size):
-  def prediction_func(s):
-    pred_model = prediction_module(num_actions, full_support_size)
-    return pred_model(s)
-  return prediction_func
-
-def _init_dynamic_func(dynamic_module, embedding_dim, num_actions, full_support_size):
-  def dynamic_func(s, a):
-    dy_model = dynamic_module(embedding_dim, num_actions, full_support_size)
-    return dy_model(s, a)
-  return dynamic_func
```

### Comparing `muax-0.0.2.8.2/muax/replay_buffer.py` & `muax-0.0.2a0/muax/replay_buffer.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,102 +24,86 @@
     SOFTWARE
 """    
 
 from abc import ABC, abstractmethod
 from collections import deque 
 from itertools import chain
 import random
-import numpy as np 
 import jax 
 from jax import numpy as jnp
 
 from .utils import sliceable_deque
 from .episode_tracer import Transition
 
    
 class Trajectory:
     r"""
     A simple trajectory to hold episodical transitions.
     """
     def __init__(self):
       self.trajectory = sliceable_deque([])
       self._transition_weight = sliceable_deque([])
-      self._batched_transitions = None
     
     def add(self, transition):
       """Adds a transition to the trajectory
       
       Parameters
       ----------
       transition: An instance of muax.episode_tracer.Transition. 
       
       """
       self.trajectory.append(transition)
       self._transition_weight.append(transition.w)
 
     
-    def finalize(self):
-      """vstack individual transitions into one instance of Transition."""
-      batched_transitions = jax.tree_util.tree_transpose(
-          outer_treedef=jax.tree_util.tree_structure([0 for i in self.trajectory]),
-          inner_treedef=jax.tree_util.tree_structure(Transition()),
-          pytree_to_transpose=self.trajectory
-          )
-      batched_transitions = Transition(*(np.expand_dims(np.vstack(_attr), axis=0)
-          for _attr in batched_transitions))
-      self._batched_transitions = batched_transitions
-
-    
     def sample(self, num_samples: int = 1, k_steps: int = 5):
       """Samples consecutive transitions of k steps from the trajectory.
       
       Parameters
       ----------
       num_samples: int, positive int. Number of samples to draw from the trajectory. 
           Each sample is chosen given the weight(transition.w) as probability.
-      
       k_steps: int, positive int. Determines the length of consecutive steps in each sample.
           If k_steps >= len(trajectory), no samples would be collected.
       
       Returns
       ----------
       samples: List[Transition]. For each transition in the list, 
           the attributes of which have the dimension `[B, L, ...]`, where B is the batch size(1) and 
           L is the length(k) of the consecutive transitions.
       """
       if len(self) <= k_steps: return []
       max_idx = len(self) - k_steps
       idxes = random.choices(range(max_idx), 
-                            weights=self._transition_weight[:max_idx], 
-                            k=num_samples)
-                            
-      if self.batched_transitions is None:
-        self.finalize()
-
+                             weights=self._transition_weight[:max_idx], 
+                             k=num_samples)
+      
       samples = [self._get_sample(idx, k_steps) for idx in idxes]
       
       return samples
 
-    @property
-    def batched_transitions(self):
-      return self._batched_transitions
-
     def _get_sample(self, idx, k_steps):
       end_idx = idx + k_steps 
-      sample = self.batched_transitions[:, idx: end_idx, :]
+      k_steps_sample = self[idx: end_idx]
+      sample = jax.tree_util.tree_transpose(
+          outer_treedef=jax.tree_util.tree_structure([0 for i in k_steps_sample]),
+          inner_treedef=jax.tree_util.tree_structure(Transition()),
+          pytree_to_transpose=k_steps_sample
+          )
+      sample = Transition(*(jnp.expand_dims(jnp.vstack(_attr), axis=0) for _attr in sample))
       return sample
 
     def __getitem__(self, index):
       return self.trajectory[index]
 
     def __len__(self):
       return len(self.trajectory)
 
     def __repr__(self):
-      return f'{type(self)}(len={len(self)})'
+      return f'{type(self)(len={len(self)})}'
       
 
 class BaseReplayBuffer(ABC):
 
     @property
     @abstractmethod
     def capacity(self):
@@ -149,20 +133,18 @@
     def __iter__(self):
         pass
 
 
 class TrajectoryReplayBuffer(BaseReplayBuffer):
     r"""
     A simple ring buffer for experience replay.
-    
     Parameters
     ----------
     capacity : positive int
         The capacity of the experience replay buffer.
-    
     random_seed : int, optional
         To get reproducible results.
     """
     def __init__(self, capacity, random_seed=None):
         self._capacity = int(capacity)
         random.seed(random_seed)
         self._random_state = random.getstate()
@@ -171,57 +153,50 @@
     @property
     def capacity(self):
         return self._capacity
 
     def add(self, trajectory, w=1.):
         r"""
         Add a trajectory to the experience replay buffer.
-        
         Parameters
         ----------
         trajectory : Trajectory
             A :class: `Trajectory` object.
-        
         w: float
             sample probability weight of input trajectory
         """
         self._storage.append(trajectory)
         self._trajectory_weight.append(w)
 
     def sample(self, 
                batch_size=32, 
                num_trajectory: int = None,
                k_steps: int = 5,
                sample_per_trajectory: int = 1):
         r"""
         Get a batch of transitions to be used for bootstrapped updates.
-        
         Parameters
         ----------
         batch_size : positive int, optional
             The desired batch size of the sample. One sample from a single trajectory.
-        
         num_trajectory: positive int, optional
             Number of trajectory to be sampled. Either num_trajectory or batch_size 
             need to be given.
-        
         k_steps: positive int
             Consecutive k steps from each trajectory. k steps unrolled for training. 
-        
         sample_per_trajectory: positive int, optional
             Number of Transition to be sampled. Used when num_trajectory is provided.
             The batch size will be num_trajectory * sample_per_trajectory.
-        
         Returns
         -------
         transitions : Batch of consecutive transitions.
         """
         if batch_size is None and num_trajectory is None: 
           raise ValueError('Either num_trajectory or batch_size need to be given.')
-        elif batch_size is not None and num_trajectory is None:
+        if batch_size is not None:
           num_trajectory = batch_size 
           sample_per_trajectory = 1
         # sandwich sample in between setstate/getstate in case global random state was tampered with
         random.setstate(self._random_state)
         trajectories = random.choices(self._storage, 
                                       weights=self._trajectory_weight,
                                       k=num_trajectory)
@@ -230,15 +205,15 @@
                      for traj in trajectories
                      ))
         
         batch = jax.tree_util.tree_transpose(
           outer_treedef=jax.tree_util.tree_structure([0 for i in batch]),
           inner_treedef=jax.tree_util.tree_structure(Transition()),
           pytree_to_transpose=batch)
-        batch = Transition(*(np.vstack(v) for v in batch))
+        batch = Transition(*(jnp.vstack(v) for v in batch))
         return batch
 
     def clear(self):
         r""" Clear the experience replay buffer. """
         self._storage = sliceable_deque([], maxlen=self.capacity)
         self._trajectory_weight = sliceable_deque([], maxlen=self.capacity)
```

### Comparing `muax-0.0.2.8.2/setup.py` & `muax-0.0.2a0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import setuptools 
 
 with open('README.md', 'r') as f:
   long_description = f.read()
   
 setuptools.setup(
   name='muax',
-  version='0.0.2.8.2',
-  authors = [{ 'name': "Bowen Fang", 'email': "bf2504@columbia.edu" },
-             {'name': 'Ian Chie', 'email': 'cc4893@columbia.edu'}],
+  version='0.0.2a',
+  authors = [{ 'name': "Bowen Fang", 'email': "bf2504@columbia.edu" }],
   description="A library written in Jax that provides help for using DeepMind's mctx on gym-style environments.",
   long_description=long_description,
-  long_description_content_type='text/markdown',
   packages=setuptools.find_packages(),
   classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
   python_requires='>=3.6',
   py_modules=['muax'],
-  install_requires=['mctx', 'dm-haiku', 'optax', 'gymnasium', 'lz4', 'tensorboardX']
+  install_requires=['mctx', 'dm-haiku', 'optax']
 )
```

