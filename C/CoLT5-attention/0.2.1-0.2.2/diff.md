# Comparing `tmp/CoLT5-attention-0.2.1.tar.gz` & `tmp/CoLT5-attention-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.2.1.tar", last modified: Sat Apr 15 18:12:30 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.2.2.tar", last modified: Wed Apr 19 21:53:53 2023, max compression
```

## Comparing `CoLT5-attention-0.2.1.tar` & `CoLT5-attention-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-15 18:12:30.000000 CoLT5-attention-0.2.1/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/colt5_attention/sinkhorn.py
--rw-r--r--   0 runner    (1001) docker     (123)    19887 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 18:12:30.292684 CoLT5-attention-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-15 18:12:16.000000 CoLT5-attention-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:53:53.668233 CoLT5-attention-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:53:53.664233 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 21:53:53.000000 CoLT5-attention-0.2.2/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-19 21:53:53.668233 CoLT5-attention-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:53:53.668233 CoLT5-attention-0.2.2/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/colt5_attention/sinkhorn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23750 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 21:53:53.668233 CoLT5-attention-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-19 21:53:42.000000 CoLT5-attention-0.2.2/setup.py
```

### Comparing `CoLT5-attention-0.2.1/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.2.2/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.1
+Version: 0.2.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.1/LICENSE` & `CoLT5-attention-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.1/PKG-INFO` & `CoLT5-attention-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.2.1
+Version: 0.2.2
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.2.1/README.md` & `CoLT5-attention-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -98,16 +98,17 @@
 
 # conditionally routed cross attention
 
 cross_attn = ConditionalRoutedCrossAttention(
     dim = 512,
     dim_head = 64,
     heads = 8,
-    num_tokens_q = 512,   # only 512 routed from 1024
-    num_tokens_kv = 1024, # only 1024 routed from 1 million
+    num_tokens_q = 512,         # only 512 routed from 1024
+    num_tokens_kv = 1024,       # only 1024 routed from 1 million
+    kv_routing_tokens = 2,      # say you want 2 routing tokens to route different sets of key / values to the queries. 4 attention heads will be allocated to each routed set in this example (8 / 2)
 ).cuda()
 
 cross_attn_out = cross_attn(
     tokens,
     context = memories,
     mask = tokens_mask,
     context_mask = memories_mask
@@ -120,14 +121,16 @@
 
 - [x] add the coordinate descent method as another router
 - [x] figure out if it can be done autoregressively and try it out - moving to <a href="https://github.com/lucidrains/coordinate-descent-attention">this repo</a>
 
 - [ ] for variable sequence lengths, allow for setting k as a function of sequence lengths per sample in batch
 - [ ] create a variant of CoLT5 for high resolution feature maps (image attention) - then try out for diffusion
 - [ ] in the cross attention scenario, support for routing token that first queries the source tokens, before retrieving from memories
+- [ ] make flash attention compatible
+- [ ] allow for multi-headed routing (multiple routing tokens), only for key-values
 
 ## Citations
 
 ```bibtex
 @inproceedings{Ainslie2023CoLT5FL,
     title   = {CoLT5: Faster Long-Range Transformers with Conditional Computation},
     author  = {Joshua Ainslie and Tao Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit Sanghai},
```

#### html2text {}

```diff
@@ -38,22 +38,26 @@
 from colt5_attention import ConditionalRoutedCrossAttention # mock input, let
 us say it is a transformer of 1024 length attending to 1 million context past
 memories tokens = torch.randn(2, 1024, 512).cuda() tokens_mask = torch.ones(2,
 1024).bool().cuda() memories = torch.randn(2, int(1e6), 512).cuda()
 memories_mask = torch.ones(2, int(1e6)).bool().cuda() # conditionally routed
 cross attention cross_attn = ConditionalRoutedCrossAttention( dim = 512,
 dim_head = 64, heads = 8, num_tokens_q = 512, # only 512 routed from 1024
-num_tokens_kv = 1024, # only 1024 routed from 1 million ).cuda() cross_attn_out
-= cross_attn( tokens, context = memories, mask = tokens_mask, context_mask =
-memories_mask ) cross_attn_out.shape # (2, 1024, 512) - same as tokens ``` ##
-Todo - [x] add the coordinate descent method as another router - [x] figure out
-if it can be done autoregressively and try it out - moving to this_repo - [ ]
-for variable sequence lengths, allow for setting k as a function of sequence
-lengths per sample in batch - [ ] create a variant of CoLT5 for high resolution
-feature maps (image attention) - then try out for diffusion - [ ] in the cross
-attention scenario, support for routing token that first queries the source
-tokens, before retrieving from memories ## Citations ```bibtex @inproceedings
-{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range Transformers with
-Conditional Computation}, author = {Joshua Ainslie and Tao Lei and Michiel de
-Jong and Santiago Ontan'on and Siddhartha Brahma and Yury Zemlyanskiy and David
-Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and Yun-Hsuan Sung and Sumit
-Sanghai}, year = {2023} } ```
+num_tokens_kv = 1024, # only 1024 routed from 1 million kv_routing_tokens = 2,
+# say you want 2 routing tokens to route different sets of key / values to the
+queries. 4 attention heads will be allocated to each routed set in this example
+(8 / 2) ).cuda() cross_attn_out = cross_attn( tokens, context = memories, mask
+= tokens_mask, context_mask = memories_mask ) cross_attn_out.shape # (2, 1024,
+512) - same as tokens ``` ## Todo - [x] add the coordinate descent method as
+another router - [x] figure out if it can be done autoregressively and try it
+out - moving to this_repo - [ ] for variable sequence lengths, allow for
+setting k as a function of sequence lengths per sample in batch - [ ] create a
+variant of CoLT5 for high resolution feature maps (image attention) - then try
+out for diffusion - [ ] in the cross attention scenario, support for routing
+token that first queries the source tokens, before retrieving from memories -
+[ ] make flash attention compatible - [ ] allow for multi-headed routing
+(multiple routing tokens), only for key-values ## Citations ```bibtex
+@inproceedings{Ainslie2023CoLT5FL, title = {CoLT5: Faster Long-Range
+Transformers with Conditional Computation}, author = {Joshua Ainslie and Tao
+Lei and Michiel de Jong and Santiago Ontan'on and Siddhartha Brahma and Yury
+Zemlyanskiy and David Uthus and Mandy Guo and James Lee-Thorp and Yi Tay and
+Yun-Hsuan Sung and Sumit Sanghai}, year = {2023} } ```
```

### Comparing `CoLT5-attention-0.2.1/colt5_attention/coor_descent.py` & `CoLT5-attention-0.2.2/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.1/colt5_attention/sinkhorn.py` & `CoLT5-attention-0.2.2/colt5_attention/sinkhorn.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.2.1/colt5_attention/transformer_block.py` & `CoLT5-attention-0.2.2/colt5_attention/transformer_block.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 from functools import partial
 
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from local_attention import LocalMHA
-from einops import rearrange, repeat
+from einops import rearrange, repeat, pack, unpack
 
 # helper functions
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
 
+def divisible_by(numer, denom):
+    return (numer % denom) == 0
+
+def pack_one(t, pattern):
+    return pack([t], pattern)
+
+def unpack_one(t, ps, pattern):
+    return unpack(t, ps, pattern)[0]
+
 # tensor helpers
 
 def create_batch_range(t):
     b, device = t.shape[0], t.device
     batch_range = torch.arange(b, device = device)
     return rearrange(batch_range, 'b -> b 1')
 
@@ -74,58 +83,116 @@
         x = self.norm(x)
 
         if exists(context):
             context = self.norm(context)
 
         context = default(context, x)
 
-        q, k, v = (self.to_q(x), *self.to_kv(context).chunk(2, dim = -1))
-        q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = self.heads), (q, k, v))
+        # if routing dimension is not there, unsqueeze for 1 routing dimension
+
+        if context.ndim == 3:
+            context = rearrange(context, 'b n d -> b 1 n d')
+
+        if exists(normalized_scores_kv):
+            if normalized_scores_kv.ndim == 2:
+                normalized_scores_kv = rearrange(normalized_scores_kv, 'b n -> b 1 n')
+
+            normalized_scores_kv = rearrange(normalized_scores_kv, 'b r n -> b r 1 n 1')
+
+        num_kv_routes = context.shape[1]
+
+        # get queries
+
+        q = self.to_q(x)
+        q = rearrange(q, 'b n (h d) -> b h n d', h = h)
+
+        # handle key / values, with the routing dimension, dividing the number of heads in between the routes
+
+        assert divisible_by(h, num_kv_routes), 'number of heads must be divisible by the number of key / value routes'
+        heads_per_route = h // num_kv_routes
+
+        kv_weight = rearrange(self.to_kv.weight, '(r h d) i -> r h d i', h = heads_per_route, r = num_kv_routes)
+
+        kv = einsum('r h d i, b r n i -> b r h n d', kv_weight, context)
+        k, v = kv.chunk(2, dim = -1)
 
         if exists(normalized_scores_kv):
             # in paper, not sure how they passed back the signal from heavy attention to normalized scores for key/values. just multiply the values by the normalized kv scores for now
-            v = v * rearrange(normalized_scores_kv, 'b n -> b 1 n 1')
+            v = v * normalized_scores_kv
+
+        k, v = map(lambda t: rearrange(t, 'b r h n d -> b (r h) n d'), (k, v))
+
+        # scale and get similarity
 
         q = q * self.scale
         sim = einsum('b h i d, b h j d -> b h i j', q, k)
 
+        # masking
+
         if exists(mask):
-            mask = rearrange(mask, 'b j -> b 1 1 j')
+            if mask.ndim == 3:
+                mask = repeat(mask, 'b r j -> b (r h) 1 j', h = heads_per_route)
+            else:
+                mask = rearrange(mask, 'b j -> b 1 1 j')
+
             sim = sim.masked_fill(~mask, -torch.finfo(sim.dtype).max)
 
+        # attention
+
         attn = sim.softmax(dim = -1)
 
+        # aggregate
+
         out = einsum('b h i j, b h j d -> b h i d', attn, v)
+
+        # merge heads
+
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 # routing related logic
 
 class DifferentiableTopKRouter(nn.Module):
     """ differentiable topk using cumulative softmax """
 
     def __init__(
         self,
         dim,
         straight_through = True,
-        temperature = 1.
+        temperature = 1.,
+        num_routing_tokens = 1
     ):
         super().__init__()
-        self.routing_token = nn.Parameter(torch.randn(dim))
+        self.is_one_routing_token = num_routing_tokens == 1
+        self.num_routing_tokens = num_routing_tokens
+        self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
+
         self.straight_through = straight_through
         self.temperature = temperature
 
     def forward(
         self,
         x,
         *,
         num_tokens,
         mask = None
     ):
-        scores = einsum('b n d, d -> b n', x, self.routing_token)
+        num_routes = self.num_routing_tokens
+
+        # eventual normalized score
+
+        scores = einsum('b n d, r d -> b r n', x, self.routing_token)
+
+        # merge routing dimension into batch
+
+        x = repeat(x, 'b ... -> (b r) ...', r = num_routes)
+        scores, ps = pack_one(scores, '* n')
+
+        if exists(mask):
+            mask = repeat(mask, 'b ... -> (b r) ...', r = num_routes)
 
         scores = scores / self.temperature
 
         if exists(mask):
             mask_value = -torch.finfo(scores.dtype).max
             scores = scores.masked_fill(~mask, mask_value)
 
@@ -144,14 +211,20 @@
             selected_scores = selected_scores + (1. - selected_scores).detach()
 
             if exists(mask):
                 batch_range = create_batch_range(x)
                 selected_mask = mask[batch_range, selected_indices]
                 selected_scores = selected_scores.masked_fill(~selected_mask, 0.)
 
+        # split out routing dimension again if need be
+
+        if not self.is_one_routing_token:
+            selected_scores = unpack_one(selected_scores, ps, '* n')
+            selected_indices = unpack_one(selected_indices, ps, '* n')
+
         return selected_scores, selected_indices
 
 # sinkhorn type routing, with ties to optimal transport
 
 from colt5_attention.sinkhorn import gumbel_sinkhorn, scatter_mean, log
 
 class SinkhornRouter(nn.Module):
@@ -159,33 +232,48 @@
     """ ex. https://arxiv.org/abs/1910.09036 """
 
     def __init__(
         self,
         dim,
         straight_through = True,
         n_iters = 8,
-        temperature = 0.7
+        temperature = 0.7,
+        num_routing_tokens = 1
     ):
         super().__init__()
-        self.routing_token = nn.Parameter(torch.randn(dim))
+        self.is_one_routing_token = num_routing_tokens == 1
+        self.num_routing_tokens = num_routing_tokens
+        self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
 
         self.straight_through = straight_through
         self.gumbel_sinkhorn_fn = partial(gumbel_sinkhorn, temperature = temperature, n_iters = n_iters)
 
     def forward(
         self,
         x,
         *,
         num_tokens,
         mask = None
     ):
-        n = x.shape[-2]
+        n, num_routes = x.shape[-2], self.num_routing_tokens
         num_tokens = min(n, num_tokens)
 
-        scores = einsum('b n d, d -> b n', x, self.routing_token)
+        # eventual normalized score
+
+        scores = einsum('b n d, r d -> b r n', x, self.routing_token)
+
+        # merge routing dimension into batch
+
+        x = repeat(x, 'b ... -> (b r) ...', r = num_routes)
+        scores, ps = pack_one(scores, '* n')
+
+        if exists(mask):
+            mask = repeat(mask, 'b ... -> (b r) ...', r = num_routes)
+
+        # calculate scores
 
         scores = repeat(scores, '... j -> ... i j', i = num_tokens)
 
         if exists(mask):
             mask_value = -torch.finfo(scores.dtype).max
             sinkhorn_mask = rearrange(mask, 'b j -> b 1 j')
             scores = scores.masked_fill(~sinkhorn_mask, mask_value)
@@ -205,16 +293,23 @@
         if self.straight_through:
             # this would make sure all normalized scores returned are 1., but still differentiable using straight-through trick
             selected_scores = selected_scores + (1. - selected_scores).detach()
 
             if exists(mask):
                 batch_range = create_batch_range(x)
                 selected_mask = mask[batch_range, selected_indices]
+
                 selected_scores = selected_scores.masked_fill(~selected_mask, 0.)
 
+        # split out routing dimension again if need be
+
+        if not self.is_one_routing_token:
+            selected_scores = unpack_one(selected_scores, ps, '* n')
+            selected_indices = unpack_one(selected_indices, ps, '* n')
+
         return selected_scores, selected_indices
 
 from colt5_attention.coor_descent import coor_descent
 
 class CoordinateDescentRouter(nn.Module):
     """
     from Wright et al. https://arxiv.org/abs/1502.04759
@@ -224,38 +319,49 @@
 
     def __init__(
         self,
         dim,
         straight_through = True,
         n_iters = 50,           # 50 iterations in the paper
         fetch_k_ratio = 9 / 8,  # in the paper, they do a bit slightly higher k (times this ratio) for better learning
-        eps = 1.                # the epsilon for coordinate descent. in CoLT5 paper they used 1. apparently
+        eps = 1.,               # the epsilon for coordinate descent. in CoLT5 paper they used 1. apparently
+        num_routing_tokens = 1
     ):
         super().__init__()
         assert fetch_k_ratio >= 1.
         self.eps = eps
 
         self.n_iters = n_iters
         self.fetch_k_ratio = fetch_k_ratio
 
-        self.routing_token = nn.Parameter(torch.randn(dim))
+        self.is_one_routing_token = num_routing_tokens == 1
+        self.num_routing_tokens = num_routing_tokens
+        self.routing_token = nn.Parameter(torch.randn(num_routing_tokens, dim))
         self.straight_through = straight_through
 
     def forward(
         self,
         x,
         *,
         num_tokens,
         mask = None
     ):
-        n, device, eps = x.shape[-2], x.device, self.eps
+        n, device, eps, num_routes = x.shape[-2], x.device, self.eps, self.num_routing_tokens
 
         # s stands for eventual normalized score
 
-        s = einsum('b n d, d -> b n', x, self.routing_token)
+        s = einsum('b n d, r d -> b r n', x, self.routing_token)
+
+        # merge routing dimension into batch
+
+        x = repeat(x, 'b ... -> (b r) ...', r = num_routes)
+        s, ps = pack_one(s, '* n')
+
+        if exists(mask):
+            mask = repeat(mask, 'b ... -> (b r) ...', r = num_routes)
 
         # k, which controls the sparsity of the outputted scores from iterative coordinate descent
 
         effective_k = min(num_tokens * self.fetch_k_ratio, n)
 
         k = torch.tensor([effective_k], device = device)
 
@@ -272,14 +378,20 @@
             selected_scores = selected_scores + (1. - selected_scores).detach()
 
             if exists(mask):
                 batch_range = create_batch_range(x)
                 selected_mask = mask[batch_range, selected_indices]
                 selected_scores = selected_scores.masked_fill(~selected_mask, 0.)
 
+        # split out routing dimension again if need be
+
+        if not self.is_one_routing_token:
+            selected_scores = unpack_one(selected_scores, ps, '* n')
+            selected_indices = unpack_one(selected_indices, ps, '* n')
+
         return selected_scores, selected_indices
 
 # all router types
 
 ROUTERS = dict(
     cum_softmax = DifferentiableTopKRouter,
     sinkhorn = SinkhornRouter,
@@ -478,19 +590,21 @@
 class ConditionalRoutedCrossAttention(nn.Module):
     def __init__(
         self,
         dim,
         *,
         num_tokens_q,
         num_tokens_kv,
+        num_sets_kv = 1,                # setting this greater than 1 would route multiple sets of key / values, each of size num_tokens_kv, using this many routing tokens
         dim_head = 64,
         heads = 8,
         router_straight_through = True, # would make sure all normalized scores are 1., still differentiable
         router_type = 'coor_descent',
-        router_kwargs: dict = {}
+        router_kwargs: dict = {},
+        kv_routing_tokens = 1
     ):
         super().__init__()
         assert router_type in ROUTERS.keys()
 
         self.router_type = router_type
 
         router_klass = ROUTERS.get(router_type)
@@ -503,14 +617,15 @@
             straight_through = router_straight_through,
             **router_kwargs
         )
 
         self.kv_router = router_klass(
             dim = dim,
             straight_through = router_straight_through,
+            num_routing_tokens = kv_routing_tokens,
             **router_kwargs
         )
 
         self.heavy_attn = Attention(
             dim = dim,
             dim_head = dim_head,
             heads = heads
```

### Comparing `CoLT5-attention-0.2.1/setup.py` & `CoLT5-attention-0.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.2.1',
+  version = '0.2.2',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

