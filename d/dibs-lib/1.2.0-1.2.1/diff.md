# Comparing `tmp/dibs-lib-1.2.0.tar.gz` & `tmp/dibs-lib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dibs-lib-1.2.0.tar", last modified: Mon Sep 26 07:06:31 2022, max compression
+gzip compressed data, was "/Users/larslorch/PycharmProjects/dibs/dist/.tmp-h6ih1p0u/dibs-lib-1.2.1.tar", last modified: Wed Apr 19 16:11:53 2023, max compression
```

## Comparing `dibs-lib-1.2.0.tar` & `dibs-lib-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2022-09-26 07:06:31.503759 dibs-lib-1.2.0/
--rw-r--r--   0 larslorch   (501) staff       (20)     1067 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/LICENCE
--rw-r--r--   0 larslorch   (501) staff       (20)      379 2022-09-26 07:06:31.503609 dibs-lib-1.2.0/PKG-INFO
--rw-r--r--   0 larslorch   (501) staff       (20)     5309 2022-09-26 07:04:03.000000 dibs-lib-1.2.0/README.md
-drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2022-09-26 07:06:31.500069 dibs-lib-1.2.0/dibs/
--rw-r--r--   0 larslorch   (501) staff       (20)        0 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/dibs/__init__.py
--rw-r--r--   0 larslorch   (501) staff       (20)     2654 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/dibs/graph_utils.py
-drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2022-09-26 07:06:31.500939 dibs-lib-1.2.0/dibs/inference/
--rw-r--r--   0 larslorch   (501) staff       (20)       65 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/dibs/inference/__init__.py
--rw-r--r--   0 larslorch   (501) staff       (20)    28549 2022-09-26 06:53:03.000000 dibs-lib-1.2.0/dibs/inference/dibs.py
--rw-r--r--   0 larslorch   (501) staff       (20)    36378 2022-09-26 07:01:05.000000 dibs-lib-1.2.0/dibs/inference/svgd.py
--rw-r--r--   0 larslorch   (501) staff       (20)     2536 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/dibs/kernel.py
--rw-r--r--   0 larslorch   (501) staff       (20)     9279 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/dibs/metrics.py
-drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2022-09-26 07:06:31.502081 dibs-lib-1.2.0/dibs/models/
--rw-r--r--   0 larslorch   (501) staff       (20)      204 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/dibs/models/__init__.py
--rw-r--r--   0 larslorch   (501) staff       (20)     8307 2022-09-26 06:53:03.000000 dibs-lib-1.2.0/dibs/models/graph.py
--rw-r--r--   0 larslorch   (501) staff       (20)    15798 2022-09-26 06:53:03.000000 dibs-lib-1.2.0/dibs/models/linearGaussian.py
--rw-r--r--   0 larslorch   (501) staff       (20)    12885 2022-09-26 07:01:05.000000 dibs-lib-1.2.0/dibs/models/nonlinearGaussian.py
--rw-r--r--   0 larslorch   (501) staff       (20)    10814 2022-03-14 09:52:09.000000 dibs-lib-1.2.0/dibs/target.py
-drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2022-09-26 07:06:31.502841 dibs-lib-1.2.0/dibs/utils/
--rw-r--r--   0 larslorch   (501) staff       (20)       64 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/dibs/utils/__init__.py
--rw-r--r--   0 larslorch   (501) staff       (20)     2246 2022-09-26 06:53:03.000000 dibs-lib-1.2.0/dibs/utils/func.py
--rw-r--r--   0 larslorch   (501) staff       (20)     1897 2022-09-26 06:53:03.000000 dibs-lib-1.2.0/dibs/utils/tree.py
--rw-r--r--   0 larslorch   (501) staff       (20)     1795 2022-03-04 10:55:31.000000 dibs-lib-1.2.0/dibs/utils/visualize.py
-drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2022-09-26 07:06:31.503458 dibs-lib-1.2.0/dibs_lib.egg-info/
--rw-r--r--   0 larslorch   (501) staff       (20)      379 2022-09-26 07:06:31.000000 dibs-lib-1.2.0/dibs_lib.egg-info/PKG-INFO
--rw-r--r--   0 larslorch   (501) staff       (20)      534 2022-09-26 07:06:31.000000 dibs-lib-1.2.0/dibs_lib.egg-info/SOURCES.txt
--rw-r--r--   0 larslorch   (501) staff       (20)        1 2022-09-26 07:06:31.000000 dibs-lib-1.2.0/dibs_lib.egg-info/dependency_links.txt
--rw-r--r--   0 larslorch   (501) staff       (20)       86 2022-09-26 07:06:31.000000 dibs-lib-1.2.0/dibs_lib.egg-info/requires.txt
--rw-r--r--   0 larslorch   (501) staff       (20)        5 2022-09-26 07:06:31.000000 dibs-lib-1.2.0/dibs_lib.egg-info/top_level.txt
--rw-r--r--   0 larslorch   (501) staff       (20)       38 2022-09-26 07:06:31.503803 dibs-lib-1.2.0/setup.cfg
--rw-r--r--   0 larslorch   (501) staff       (20)      688 2022-09-26 07:05:41.000000 dibs-lib-1.2.0/setup.py
+drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2023-04-19 16:11:53.264414 dibs-lib-1.2.1/
+-rw-r--r--   0 larslorch   (501) staff       (20)     1067 2022-03-04 10:55:31.000000 dibs-lib-1.2.1/LICENCE
+-rw-r--r--   0 larslorch   (501) staff       (20)      379 2023-04-19 16:11:53.264252 dibs-lib-1.2.1/PKG-INFO
+-rw-r--r--   0 larslorch   (501) staff       (20)     5309 2022-11-04 13:58:55.000000 dibs-lib-1.2.1/README.md
+drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2023-04-19 16:11:53.260747 dibs-lib-1.2.1/dibs/
+-rw-r--r--   0 larslorch   (501) staff       (20)        0 2022-03-04 10:55:31.000000 dibs-lib-1.2.1/dibs/__init__.py
+-rw-r--r--   0 larslorch   (501) staff       (20)     2654 2022-03-04 10:55:31.000000 dibs-lib-1.2.1/dibs/graph_utils.py
+drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2023-04-19 16:11:53.261572 dibs-lib-1.2.1/dibs/inference/
+-rw-r--r--   0 larslorch   (501) staff       (20)       65 2022-03-04 10:55:31.000000 dibs-lib-1.2.1/dibs/inference/__init__.py
+-rw-r--r--   0 larslorch   (501) staff       (20)    27067 2023-04-19 16:04:35.000000 dibs-lib-1.2.1/dibs/inference/dibs.py
+-rw-r--r--   0 larslorch   (501) staff       (20)    36346 2023-04-19 16:04:35.000000 dibs-lib-1.2.1/dibs/inference/svgd.py
+-rw-r--r--   0 larslorch   (501) staff       (20)     2413 2023-04-19 16:04:35.000000 dibs-lib-1.2.1/dibs/kernel.py
+-rw-r--r--   0 larslorch   (501) staff       (20)     9279 2022-03-04 10:55:31.000000 dibs-lib-1.2.1/dibs/metrics.py
+drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2023-04-19 16:11:53.262324 dibs-lib-1.2.1/dibs/models/
+-rw-r--r--   0 larslorch   (501) staff       (20)      204 2022-03-04 10:55:31.000000 dibs-lib-1.2.1/dibs/models/__init__.py
+-rw-r--r--   0 larslorch   (501) staff       (20)     8119 2023-04-19 16:04:35.000000 dibs-lib-1.2.1/dibs/models/graph.py
+-rw-r--r--   0 larslorch   (501) staff       (20)    14980 2023-04-19 16:04:35.000000 dibs-lib-1.2.1/dibs/models/linearGaussian.py
+-rw-r--r--   0 larslorch   (501) staff       (20)    12829 2023-04-19 16:04:35.000000 dibs-lib-1.2.1/dibs/models/nonlinearGaussian.py
+-rw-r--r--   0 larslorch   (501) staff       (20)    10814 2022-11-04 13:58:55.000000 dibs-lib-1.2.1/dibs/target.py
+drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2023-04-19 16:11:53.263205 dibs-lib-1.2.1/dibs/utils/
+-rw-r--r--   0 larslorch   (501) staff       (20)       64 2022-03-04 10:55:31.000000 dibs-lib-1.2.1/dibs/utils/__init__.py
+-rw-r--r--   0 larslorch   (501) staff       (20)     3188 2023-04-19 16:11:11.000000 dibs-lib-1.2.1/dibs/utils/func.py
+-rw-r--r--   0 larslorch   (501) staff       (20)     1897 2022-09-26 06:53:03.000000 dibs-lib-1.2.1/dibs/utils/tree.py
+-rw-r--r--   0 larslorch   (501) staff       (20)     1795 2022-03-04 10:55:31.000000 dibs-lib-1.2.1/dibs/utils/visualize.py
+drwxr-xr-x   0 larslorch   (501) staff       (20)        0 2023-04-19 16:11:53.264057 dibs-lib-1.2.1/dibs_lib.egg-info/
+-rw-r--r--   0 larslorch   (501) staff       (20)      379 2023-04-19 16:11:53.000000 dibs-lib-1.2.1/dibs_lib.egg-info/PKG-INFO
+-rw-r--r--   0 larslorch   (501) staff       (20)      534 2023-04-19 16:11:53.000000 dibs-lib-1.2.1/dibs_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 larslorch   (501) staff       (20)        1 2023-04-19 16:11:53.000000 dibs-lib-1.2.1/dibs_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 larslorch   (501) staff       (20)       86 2023-04-19 16:11:53.000000 dibs-lib-1.2.1/dibs_lib.egg-info/requires.txt
+-rw-r--r--   0 larslorch   (501) staff       (20)        5 2023-04-19 16:11:53.000000 dibs-lib-1.2.1/dibs_lib.egg-info/top_level.txt
+-rw-r--r--   0 larslorch   (501) staff       (20)       38 2023-04-19 16:11:53.264466 dibs-lib-1.2.1/setup.cfg
+-rw-r--r--   0 larslorch   (501) staff       (20)      688 2023-04-19 16:11:11.000000 dibs-lib-1.2.1/setup.py
```

### Comparing `dibs-lib-1.2.0/LICENCE` & `dibs-lib-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `dibs-lib-1.2.0/README.md` & `dibs-lib-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dibs-lib-1.2.0/dibs/graph_utils.py` & `dibs-lib-1.2.1/dibs/graph_utils.py`

 * *Files identical despite different names*

### Comparing `dibs-lib-1.2.0/dibs/inference/dibs.py` & `dibs-lib-1.2.1/dibs/inference/dibs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from jax import vmap, random, grad
 from jax.scipy.special import logsumexp
 from jax.nn import sigmoid, log_sigmoid
 import jax.lax as lax
 from jax.tree_util import tree_map
 
 from dibs.graph_utils import acyclic_constr_nograd
-from dibs.utils.func import expand_by
+from dibs.utils.func import expand_by, zero_diagonal
 
 
 class DiBS:
     """
     This class implements the backbone for DiBS, i.e. all gradient estimators and sampling
     components. Any inference method in the DiBS framework should inherit from this class.
 
@@ -58,16 +58,14 @@
                  tau=1.0,
                  n_grad_mc_samples=128,
                  n_acyclicity_mc_samples=32,
                  grad_estimator_z='reparam',
                  score_function_baseline=0.0,
                  latent_prior_std=None,
                  verbose=False):
-        super(DiBS, self).__init__()
-
         self.x = x
         self.interv_mask = interv_mask
         self.n_vars = x.shape[-1]
         self.log_graph_prior = log_graph_prior
         self.log_joint_prob = log_joint_prob
         self.alpha = lambda t: (alpha_linear * t)
         self.beta = lambda t: (beta_linear * t)
@@ -79,58 +77,30 @@
         self.latent_prior_std = latent_prior_std
         self.verbose = verbose
 
     """
     Backbone functionality
     """
 
-    def vec_to_mat(self, z, n_vars):
-        """
-        Reshapes particle to latent adjacency matrix form. Last dim gets shaped into matrix
-
-        Args:
-            z (ndarray): flattened matrix of shape ``[..., n_vars * n_vars]``
-
-        Returns:
-            matrix of shape ``[..., d, d]``
-        """
-        return z.reshape(*z.shape[:-1], n_vars, n_vars)
-
-
-    def mat_to_vec(self, w):
-        """
-        Reshapes latent adjacency matrix form to particle. Last two dims get flattened into vector
-
-        Args:
-            w (ndarray): matrix of shape ``[..., d, d]``
-
-        Returns:
-            flattened matrix of shape ``[..., d * d]``
-        """
-        n_vars = w.shape[-1]
-        return w.reshape(*w.shape[:-2], n_vars * n_vars)
-
-
     def particle_to_g_lim(self, z):
         """
         Returns :math:`G` corresponding to :math:`\\alpha = \\infty` for particles `z`
 
         Args:
             z (ndarray): latent variables ``[..., d, k, 2]``
 
         Returns:
             graph adjacency matrices of shape ``[..., d, d]``
         """
         u, v = z[..., 0], z[..., 1]
         scores = jnp.einsum('...ik,...jk->...ij', u, v)
         g_samples = (scores > 0).astype(jnp.int32)
 
-        # zero diagonal
-        g_samples = g_samples.at[..., jnp.arange(scores.shape[-1]), jnp.arange(scores.shape[-1])].set(0)
-        return g_samples
+        # mask diagonal since it is explicitly not modeled
+        return zero_diagonal(g_samples)
 
 
     def sample_g(self, p, subk, n_samples):
         """
         Sample Bernoulli matrix according to matrix of probabilities
 
         Args:
@@ -138,20 +108,19 @@
             n_samples (int): number of samples
             subk (ndarray): rng key
 
         Returns:
             an array of matrices sampled according to ``p`` of shape ``[n_samples, d, d]``
         """
         n_vars = p.shape[-1]
-        g_samples = self.vec_to_mat(random.bernoulli(
-            subk, p=self.mat_to_vec(p), shape=(n_samples, n_vars * n_vars)), n_vars).astype(jnp.int32)
+        g_samples = random.bernoulli(
+            subk, p=p, shape=(n_samples, n_vars, n_vars)).astype(jnp.int32)
 
         # mask diagonal since it is explicitly not modeled
-        g_samples = g_samples.at[..., jnp.arange(p.shape[-1]), jnp.arange(p.shape[-1])].set(0)
-        return g_samples
+        return zero_diagonal(g_samples)
 
     def particle_to_soft_graph(self, z, eps, t):
         """
         Gumbel-softmax / concrete distribution using Logistic(0,1) samples ``eps``
 
         Args:
             z (ndarray): a single latent tensor :math:`Z` of shape ``[d, k, 2]```
@@ -164,17 +133,15 @@
         scores = jnp.einsum('...ik,...jk->...ij', z[..., 0], z[..., 1])
 
         # soft reparameterization using gumbel-softmax/concrete distribution
         # eps ~ Logistic(0,1)
         soft_graph = sigmoid(self.tau * (eps + self.alpha(t) * scores))
 
         # mask diagonal since it is explicitly not modeled
-        n_vars = soft_graph.shape[-1]
-        soft_graph = soft_graph.at[..., jnp.arange(n_vars), jnp.arange(n_vars)].set(0.0)
-        return soft_graph
+        return zero_diagonal(soft_graph)
 
 
     def particle_to_hard_graph(self, z, eps, t):
         """
         Bernoulli sample of :math:`G` using probabilities implied by latent ``z``
 
         Args:
@@ -184,20 +151,18 @@
 
         Returns:
             Gumbel-max (hard) sample of adjacency matrix ``[d, d]``
         """
         scores = jnp.einsum('...ik,...jk->...ij', z[..., 0], z[..., 1])
 
         # simply take hard limit of sigmoid in gumbel-softmax/concrete distribution
-        hard_graph = ((self.tau * (eps + self.alpha(t) * scores)) > 0.0).astype(jnp.float32)
+        hard_graph = ((eps + self.alpha(t) * scores) > 0.0).astype(jnp.float32)
 
         # mask diagonal since it is explicitly not modeled
-        n_vars = hard_graph.shape[-1]
-        hard_graph = hard_graph.at[..., jnp.arange(n_vars), jnp.arange(n_vars)].set(0.0)
-        return hard_graph
+        return zero_diagonal(hard_graph)
 
 
     """
     Generative graph model p(G | Z)
     """
 
     def edge_probs(self, z, t):
@@ -212,16 +177,15 @@
             edge probabilities of shape ``[..., d, d]``
         """
         u, v = z[..., 0], z[..., 1]
         scores = jnp.einsum('...ik,...jk->...ij', u, v)
         probs = sigmoid(self.alpha(t) * scores)
 
         # mask diagonal since it is explicitly not modeled
-        probs = probs.at[..., jnp.arange(probs.shape[-1]), jnp.arange(probs.shape[-1])].set(0.0)
-        return probs
+        return zero_diagonal(probs)
 
 
     def edge_log_probs(self, z, t):
         """
         Edge log probabilities encoded by latent representation
 
         Args:
@@ -233,17 +197,15 @@
         """
         u, v = z[..., 0], z[..., 1]
         scores = jnp.einsum('...ik,...jk->...ij', u, v)
         log_probs, log_probs_neg = log_sigmoid(self.alpha(t) * scores), log_sigmoid(self.alpha(t) * -scores)
 
         # mask diagonal since it is explicitly not modeled
         # NOTE: this is not technically log(p), but the way `edge_log_probs_` is used, this is correct
-        log_probs = log_probs.at[..., jnp.arange(log_probs.shape[-1]), jnp.arange(log_probs.shape[-1])].set(0.0)
-        log_probs_neg = log_probs_neg.at[..., jnp.arange(log_probs_neg.shape[-1]), jnp.arange(log_probs_neg.shape[-1])].set(0.0)
-        return log_probs, log_probs_neg
+        return zero_diagonal(log_probs), zero_diagonal(log_probs_neg)
 
 
 
     def latent_log_prob(self, single_g, single_z, t):
         """
         Log likelihood of generative graph model
 
@@ -723,8 +685,8 @@
                 f'iteration {kwargs["t"]:6d}'
                 f' | alpha {self.alpha(kwargs["t"]):6.1f}'
                 f' | beta {self.beta(kwargs["t"]):6.1f}'
                 f' | #cyclic {(constraint(gs, self.n_vars) > 0).sum().item():3d}'
             )
             return
 
-        return callback
+        return callback
```

### Comparing `dibs-lib-1.2.0/dibs/inference/svgd.py` & `dibs-lib-1.2.1/dibs/inference/svgd.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             optimizer_param = {"stepsize": 0.005}
 
         # handle interv mask in observational case
         if interv_mask is None:
             interv_mask = jnp.zeros_like(x, dtype=jnp.int32)
 
         # init DiBS superclass methods
-        super(MarginalDiBS, self).__init__(
+        super().__init__(
             x=x,
             interv_mask=interv_mask,
             log_graph_prior=inference_model.log_graph_prior,
             log_joint_prob=inference_model.interventional_log_marginal_prob,
             alpha_linear=alpha_linear,
             beta_linear=beta_linear,
             tau=tau,
@@ -100,15 +100,15 @@
             verbose=verbose,
         )
 
         self.inference_model = inference_model
 
         # functions for post-hoc likelihood evaluations
         self.eltwise_log_marginal_likelihood_observ = vmap(lambda g, x_ho:
-             inference_model.interventional_log_marginal_prob(g, None, x_ho, jnp.zeros_like(self.x), None), (0, None), 0)
+             inference_model.interventional_log_marginal_prob(g, None, x_ho, jnp.zeros_like(x_ho), None), (0, None), 0)
         self.eltwise_log_marginal_likelihood_interv = vmap(lambda g, x_ho, interv_msk_ho:
              inference_model.interventional_log_marginal_prob(g, None, x_ho, interv_msk_ho, None), (0, None, None), 0)
 
         self.kernel = kernel(**kernel_param)
 
         if optimizer == 'gd':
             self.opt = optimizers.sgd(optimizer_param['stepsize'])
@@ -340,15 +340,15 @@
         """
         N, _, _ = g.shape
         unique, counts = onp.unique(g, axis=0, return_counts=True)
 
         # empirical distribution using counts
         logp = jnp.log(counts) - jnp.log(N)
 
-        return ParticleDistribution(logp=logp, g=g)
+        return ParticleDistribution(logp=logp, g=unique)
 
     def get_mixture(self, g):
         """
         Converts batch of binary (adjacency) matrices into *mixture* particle distribution,
         where mixture weights correspond to unnormalized target (i.e. posterior) probabilities
 
         Args:
@@ -440,15 +440,15 @@
             optimizer_param = {"stepsize": 0.005}
 
         # handle interv mask in observational case
         if interv_mask is None:
             interv_mask = jnp.zeros_like(x, dtype=jnp.int32)
 
         # init DiBS superclass methods
-        super(JointDiBS, self).__init__(
+        super().__init__(
             x=x,
             interv_mask=interv_mask,
             log_graph_prior=inference_model.log_graph_prior,
             log_joint_prob=inference_model.interventional_log_joint_prob,
             alpha_linear=alpha_linear,
             beta_linear=beta_linear,
             tau=tau,
@@ -460,15 +460,15 @@
             verbose=verbose,
         )
 
         self.inference_model = inference_model
 
         # functions for post-hoc likelihood evaluations
         self.eltwise_log_likelihood_observ = vmap(lambda g, theta, x_ho:
-            inference_model.interventional_log_joint_prob(g, theta, x_ho, jnp.zeros_like(self.x), None), (0, 0, None), 0)
+            inference_model.interventional_log_joint_prob(g, theta, x_ho, jnp.zeros_like(x_ho), None), (0, 0, None), 0)
         self.eltwise_log_likelihood_interv = vmap(lambda g, theta, x_ho, interv_msk_ho:
             inference_model.interventional_log_joint_prob(g, theta, x_ho, interv_msk_ho, None), (0, 0, None, None), 0)
 
         self.kernel = kernel(**kernel_param)
 
         if optimizer == 'gd':
             self.opt = optimizers.sgd(optimizer_param['stepsize'])
```

### Comparing `dibs-lib-1.2.0/dibs/kernel.py` & `dibs-lib-1.2.1/dibs/kernel.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     Args:
         h (float): bandwidth parameter
         scale (float): scale parameter
 
     """
 
     def __init__(self, *, h=20.0, scale=1.0):
-        super(AdditiveFrobeniusSEKernel, self).__init__()
-
         self.h = h
         self.scale = scale
 
     def eval(self, *, x, y):
         """Evaluates kernel function
 
         Args:
@@ -42,16 +40,14 @@
         h_latent (float): bandwidth parameter for :math:`Z` term
         h_theta (float): bandwidth parameter for :math:`\\Theta` term
         scale_latent (float): scale parameter for :math:`Z` term
         scale_theta (float): scale parameter  for :math:`\\Theta` term
     """
 
     def __init__(self, *, h_latent=5.0, h_theta=500.0, scale_latent=1.0, scale_theta=1.0):
-        super(JointAdditiveFrobeniusSEKernel, self).__init__()
-
         self.h_latent = h_latent
         self.h_theta = h_theta
         self.scale_latent = scale_latent
         self.scale_theta = scale_theta
 
     def eval(self, *, x_latent, x_theta, y_latent, y_theta):
         """Evaluates kernel function k(x, y)
```

### Comparing `dibs-lib-1.2.0/dibs/metrics.py` & `dibs-lib-1.2.1/dibs/metrics.py`

 * *Files identical despite different names*

### Comparing `dibs-lib-1.2.0/dibs/models/graph.py` & `dibs-lib-1.2.1/dibs/models/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import igraph as ig
 import random as pyrandom
 import jax.numpy as jnp
 from jax import random
 
 from dibs.graph_utils import mat_to_graph, graph_to_mat, mat_is_dag
+from dibs.utils.func import zero_diagonal
 
 
 class ErdosReniDAGDistribution:
     """
     Randomly oriented Erdos-Reni random graph model with i.i.d. edge probability.
     The pmf is defined as
 
@@ -20,16 +21,14 @@
     Args:
         n_vars (int): number of variables in DAG
         n_edges_per_node (int): number of edges sampled per variable in expectation
 
     """
 
     def __init__(self, n_vars, n_edges_per_node=2):
-        super(ErdosReniDAGDistribution, self).__init__()
-
         self.n_vars = n_vars
         self.n_edges = n_edges_per_node * n_vars
         self.p = self.n_edges / ((self.n_vars * (self.n_vars - 1)) / 2)
 
     def sample_G(self, key, return_mat=False):
         """Samples DAG
 
@@ -121,16 +120,14 @@
     Args:
         n_vars (int): number of variables in DAG
         n_edges_per_node (int): number of edges sampled per variable
 
     """
 
     def __init__(self, n_vars, verbose=False, n_edges_per_node=2):
-        super(ScaleFreeDAGDistribution, self).__init__()
-
         self.n_vars = n_vars
         self.n_edges_per_node = n_edges_per_node
         self.verbose = verbose
 
 
     def sample_G(self, key, return_mat=False):
         """Samples DAG
@@ -208,15 +205,14 @@
 
     Args:
         n_vars (int): number of variables in DAG
 
     """
 
     def __init__(self, n_vars):
-        super(UniformDAGDistributionRejection, self).__init__()
         self.n_vars = n_vars 
 
     def sample_G(self, key, return_mat=False):
         """Samples DAG
 
         Args:
             key (ndarray): rng
@@ -225,15 +221,15 @@
         Returns:
             ``iGraph.graph`` / ``jnp.array``:
             DAG
         """
         while True:
             key, subk = random.split(key)
             mat = random.bernoulli(subk, p=0.5, shape=(self.n_vars, self.n_vars)).astype(jnp.int32)
-            mat = mat.at[..., jnp.arange(self.n_vars), jnp.arange(self.n_vars)].set(0)
+            mat = zero_diagonal(mat)
 
             if mat_is_dag(mat):
                 if return_mat:
                     return mat
                 else:
                     return mat_to_graph(mat)
```

### Comparing `dibs-lib-1.2.0/dibs/models/linearGaussian.py` & `dibs-lib-1.2.1/dibs/models/linearGaussian.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import jax.numpy as jnp
 from jax import random, vmap
 from jax.scipy.stats import norm as jax_normal
 from jax.scipy.special import gammaln
+from dibs.utils.func import _slogdet_jax
 
 
 class BGe:
     """
     Linear Gaussian BN model corresponding to linear structural equation model (SEM) with additive Gaussian noise.
     Uses Normal-Wishart conjugate parameter prior to allow for closed-form marginal likelihood
     :math:`\\log p(D | G)` and thus allows inference of the marginal posterior :math:`p(G | D)`
@@ -36,16 +37,14 @@
 
     def __init__(self, *,
                  graph_dist,
                  mean_obs=None,
                  alpha_mu=None,
                  alpha_lambd=None,
                  ):
-        super(BGe, self).__init__()
-
         self.graph_dist = graph_dist
         self.n_vars = graph_dist.n_vars
 
         self.mean_obs = mean_obs or jnp.zeros(self.n_vars)
         self.alpha_mu = alpha_mu or 1.0
         self.alpha_lambd = alpha_lambd or (self.n_vars + 2)
 
@@ -61,33 +60,14 @@
     def sample_obs(self, *, key, n_samples, g, theta, toporder=None, interv=None):
         raise NotImplementedError("Not available for BGe score; use `LinearGaussian` model instead.")
 
     """
     The following functions need to be functionally pure and jax.jit-compilable
     """
 
-    def _slogdet_jax(self, m, parents):
-        """
-        Log determinant of a submatrix. Made ``jax.jit``-compilable and ``jax.grad``-differentiable
-        by masking everything but the submatrix and adding a diagonal of ones everywhere else
-        to obtain the valid determinant
-
-        Args:
-            m (ndarray): matrix of shape ``[d, d]``
-            parents (ndarray): boolean indicator of parents of shape ``[d, ]``
-
-        Returns:
-            natural log of determinant of submatrix ``m`` indexed by ``parents`` on both dimensions
-        """
-
-        n_vars = parents.shape[0]
-        mask = jnp.einsum('...i,...j->...ij', parents, parents)
-        submat = mask * m + (1 - mask) * jnp.eye(n_vars)
-        return jnp.linalg.slogdet(submat)[1]
-
     def _log_marginal_likelihood_single(self, j, n_parents, g, x, interv_targets):
         """
         Computes node-specific score of BGe marginal likelihood. ``jax.jit``-compilable
 
         Args:
             j (int): node index for score
             n_parents (int): number of parents of node ``j``
@@ -129,17 +109,17 @@
                 + 0.5 * (self.alpha_lambd - d + 2 * n_parents + 1) *
                 jnp.log(small_t)
         )
 
         log_term_r = (
             # log det(R_II)^(..) / det(R_JJ)^(..)
                 0.5 * (N + self.alpha_lambd - d + n_parents) *
-                self._slogdet_jax(R, parents)
+                _slogdet_jax(R, parents)
                 - 0.5 * (N + self.alpha_lambd - d + n_parents + 1) *
-                self._slogdet_jax(R, parents_and_j)
+                _slogdet_jax(R, parents_and_j)
         )
 
         # return neutral sum element (0) if no observations (N=0)
         return jnp.where(jnp.isclose(N, 0), 0.0, log_gamma_term + log_term_r)
 
     def log_marginal_likelihood(self, *, g, x, interv_targets):
         """Computes BGe marginal likelihood :math:`\\log p(D | G)`` in closed-form;
@@ -223,16 +203,14 @@
         mean_edge (float, optional): mean of Gaussian edge weight
         sig_edge (float, optional): std dev of Gaussian edge weight
         min_edge (float, optional): minimum linear effect of parent on child
 
     """
 
     def __init__(self, *, graph_dist, obs_noise=0.1, mean_edge=0.0, sig_edge=1.0, min_edge=0.5):
-        super(LinearGaussian, self).__init__()
-
         self.graph_dist = graph_dist
         self.n_vars = graph_dist.n_vars
         self.obs_noise = obs_noise
         self.mean_edge = mean_edge
         self.sig_edge = sig_edge
         self.min_edge = min_edge
```

### Comparing `dibs-lib-1.2.0/dibs/models/nonlinearGaussian.py` & `dibs-lib-1.2.1/dibs/models/nonlinearGaussian.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,14 @@
         obs_noise (float, optional): variance of additive observation noise at nodes
         sig_param (float, optional): std dev of Gaussian parameter prior
         activation (str, optional): identifier for activation function.
             Choices: ``sigmoid``, ``tanh``, ``relu``, ``leakyrelu``
 
     """
     def __init__(self, *, graph_dist, hidden_layers, obs_noise=0.1, sig_param=1.0, activation='relu', bias=True):
-        super(DenseNonlinearGaussian, self).__init__()
-
         self.graph_dist = graph_dist
         self.n_vars = graph_dist.n_vars
         self.obs_noise = obs_noise
         self.sig_param = sig_param
         self.hidden_layers = hidden_layers
         self.activation = activation
         self.bias = bias
```

### Comparing `dibs-lib-1.2.0/dibs/target.py` & `dibs-lib-1.2.1/dibs/target.py`

 * *Files identical despite different names*

### Comparing `dibs-lib-1.2.0/dibs/utils/func.py` & `dibs-lib-1.2.1/dibs/utils/func.py`

 * *Files 16% similar despite different names*

```diff
@@ -110,7 +110,36 @@
 
     diff = tree_map(jnp.subtract, x, y)
     squared_norm_ind = tree_map(lambda leaf: jnp.square(leaf).sum(), diff)
     squared_norm = tree_reduce(jnp.add, squared_norm_ind)
     return squared_norm
 
 
+def zero_diagonal(g):
+    """
+    Returns the argument matrix with its diagonal set to zero.
+
+    Args:
+        g (ndarray): matrix of shape ``[..., d, d]``
+    """
+    d = g.shape[-1]
+    return g.at[..., jnp.arange(d), jnp.arange(d)].set(0)
+
+
+def _slogdet_jax(m, parents):
+    """
+    Log determinant of a submatrix. Made ``jax.jit``-compilable and ``jax.grad``-differentiable
+    by masking everything but the submatrix and adding a diagonal of ones everywhere else
+    to obtain the valid determinant
+
+    Args:
+        m (ndarray): matrix of shape ``[d, d]``
+        parents (ndarray): boolean indicator of parents of shape ``[d, ]``
+
+    Returns:
+        natural log of determinant of submatrix ``m`` indexed by ``parents`` on both dimensions
+    """
+
+    n_vars = parents.shape[0]
+    mask = jnp.einsum('...i,...j->...ij', parents, parents)
+    submat = mask * m + (1 - mask) * jnp.eye(n_vars)
+    return jnp.linalg.slogdet(submat)[1]
```

### Comparing `dibs-lib-1.2.0/dibs/utils/tree.py` & `dibs-lib-1.2.1/dibs/utils/tree.py`

 * *Files identical despite different names*

### Comparing `dibs-lib-1.2.0/dibs/utils/visualize.py` & `dibs-lib-1.2.1/dibs/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `dibs-lib-1.2.0/dibs_lib.egg-info/SOURCES.txt` & `dibs-lib-1.2.1/dibs_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dibs-lib-1.2.0/setup.py` & `dibs-lib-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='dibs-lib',
-    version='1.2.0',
+    version='1.2.1',
     description='DiBS: Differentiable Bayesian Structure Learning',
     author='Lars Lorch',
     author_email='lars.lorch@inf.ethz.ch',
     url="https://github.com/larslorch/dibs",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

