# Comparing `tmp/preliz-0.2.0.tar.gz` & `tmp/preliz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preliz-0.2.0.tar", last modified: Tue Feb 14 00:24:37 2023, max compression
+gzip compressed data, was "preliz-0.3.0.tar", last modified: Wed Apr 19 00:58:29 2023, max compression
```

## Comparing `preliz-0.2.0.tar` & `preliz-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0     2933 2023-02-14 00:24:30.001869 preliz-0.2.0/README.md
--rw-r--r--   0        0        0      649 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/__init__.py
--rw-r--r--   0        0        0      757 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/distributions/__init__.py
--rw-r--r--   0        0        0    83467 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/distributions/continuous.py
--rw-r--r--   0        0        0    25145 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/distributions/discrete.py
--rw-r--r--   0        0        0    18095 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/distributions/distributions.py
--rw-r--r--   0        0        0       64 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/internal/__init__.py
--rw-r--r--   0        0        0     4232 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/internal/distribution_helper.py
--rw-r--r--   0        0        0     6391 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/internal/optimization.py
--rw-r--r--   0        0        0     3043 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/internal/parser.py
--rw-r--r--   0        0        0    14933 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/internal/plot_helper.py
--rw-r--r--   0        0        0      114 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/predictive/__init__.py
--rw-r--r--   0        0        0    14161 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/predictive/ppa.py
--rw-r--r--   0        0        0     1347 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/predictive/predictive_sliders.py
--rw-r--r--   0        0        0     1946 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/check_inside_notebook.ipynb
--rw-r--r--   0        0        0     1799 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/plot_interactive.ipynb
--rw-r--r--   0        0        0     2244 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/predictive_sliders.ipynb
--rw-r--r--   0        0        0     1472 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/roulette.ipynb
--rw-r--r--   0        0        0     6366 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_distributions.py
--rw-r--r--   0        0        0      626 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_helper.py
--rw-r--r--   0        0        0      338 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_internals.py
--rw-r--r--   0        0        0     5750 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_maxent.py
--rw-r--r--   0        0        0     2586 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_mle.py
--rw-r--r--   0        0        0     1309 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_plots.py
--rw-r--r--   0        0        0      115 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_predictive_sliders.py
--rw-r--r--   0        0        0     2971 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_quartile.py
--rw-r--r--   0        0        0      905 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/tests/test_roulette.py
--rw-r--r--   0        0        0      164 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/unidimensional/__init__.py
--rw-r--r--   0        0        0     3894 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/unidimensional/maxent.py
--rw-r--r--   0        0        0     1681 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/unidimensional/mle.py
--rw-r--r--   0        0        0     3261 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/unidimensional/quartile.py
--rw-r--r--   0        0        0     9632 2023-02-14 00:24:30.169868 preliz-0.2.0/preliz/unidimensional/roulette.py
--rw-r--r--   0        0        0     1298 2023-02-14 00:24:30.169868 preliz-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3932 1970-01-01 00:00:00.000000 preliz-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2802 2023-04-19 00:58:22.162966 preliz-0.3.0/README.md
+-rw-r--r--   0        0        0      649 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/__init__.py
+-rw-r--r--   0        0        0     1016 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/__init__.py
+-rw-r--r--   0        0        0    89157 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/continuous.py
+-rw-r--r--   0        0        0    14095 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/continuous_multivariate.py
+-rw-r--r--   0        0        0    39411 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/discrete.py
+-rw-r--r--   0        0        0    18095 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/distributions.py
+-rw-r--r--   0        0        0     6516 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/distributions/distributions_multivariate.py
+-rw-r--r--   0        0        0       64 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/__init__.py
+-rw-r--r--   0        0        0     4611 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/distribution_helper.py
+-rw-r--r--   0        0        0     7289 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/optimization.py
+-rw-r--r--   0        0        0     3043 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/parser.py
+-rw-r--r--   0        0        0    14995 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/plot_helper.py
+-rw-r--r--   0        0        0     8168 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/internal/plot_helper_multivariate.py
+-rw-r--r--   0        0        0      114 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/predictive/__init__.py
+-rw-r--r--   0        0        0    14107 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/predictive/ppa.py
+-rw-r--r--   0        0        0     1345 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/predictive/predictive_sliders.py
+-rw-r--r--   0        0        0     1946 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/check_inside_notebook.ipynb
+-rw-r--r--   0        0        0     1799 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/plot_interactive.ipynb
+-rw-r--r--   0        0        0     2244 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/predictive_sliders.ipynb
+-rw-r--r--   0        0        0     1472 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/roulette.ipynb
+-rw-r--r--   0        0        0     7310 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_distributions.py
+-rw-r--r--   0        0        0      626 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_helper.py
+-rw-r--r--   0        0        0      338 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_internals.py
+-rw-r--r--   0        0        0     6488 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_maxent.py
+-rw-r--r--   0        0        0     2859 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_mle.py
+-rw-r--r--   0        0        0     2789 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_plots.py
+-rw-r--r--   0        0        0      115 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_predictive_sliders.py
+-rw-r--r--   0        0        0     3455 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_quartile.py
+-rw-r--r--   0        0        0      906 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/tests/test_roulette.py
+-rw-r--r--   0        0        0      164 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/unidimensional/__init__.py
+-rw-r--r--   0        0        0     3898 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/unidimensional/maxent.py
+-rw-r--r--   0        0        0     1681 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/unidimensional/mle.py
+-rw-r--r--   0        0        0     3263 2023-04-19 00:58:22.334967 preliz-0.3.0/preliz/unidimensional/quartile.py
+-rw-r--r--   0        0        0     9633 2023-04-19 00:58:22.338967 preliz-0.3.0/preliz/unidimensional/roulette.py
+-rw-r--r--   0        0        0     1298 2023-04-19 00:58:22.338967 preliz-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3801 1970-01-01 00:00:00.000000 preliz-0.3.0/PKG-INFO
```

### Comparing `preliz-0.2.0/README.md` & `preliz-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 <img src="https://raw.githubusercontent.com/arviz-devs/preliz/main/docs/logos/PreliZ.png#gh-light-mode-only" width=200></img>
 <img src="https://raw.githubusercontent.com/arviz-devs/preliz/main/docs/logos/PreliZ_white.png#gh-dark-mode-only" width=200></img>
 
-Tools to help you pick a prior.
+A tool-box for prior elicitation.
 
 [![PyPi version](https://badge.fury.io/py/preliz.svg)](https://badge.fury.io/py/preliz)
 [![Build Status](https://github.com/arviz-devs/preliz/actions/workflows/test.yml/badge.svg)](https://github.com/arviz-devs/preliz/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/arviz-devs/preliz/branch/master/graph/badge.svg?token=SLJIK2O4C5 )](https://codecov.io/gh/arviz-devs/preliz/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 
-**This package is very new and many of its features are experimental, or not yet well tested, or subject to change without notice.**
 
 
 ## Documentation
 
 The PreliZ documentation can be found in the [official docs](https://preliz.readthedocs.io/en/latest/).
 
 ## Installation
```

### Comparing `preliz-0.2.0/preliz/__init__.py` & `preliz-0.3.0/preliz/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .distributions import *
 from .predictive import *
 from .unidimensional import *
 
 
 __all__ = ["maxent", "mle", "ppa", "roulette", "quartile"]
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 _log = logging.getLogger("preliz")
 
 if not logging.root.handlers:
     _log.setLevel(logging.INFO)
     if len(_log.handlers) == 0:
         handler = logging.StreamHandler()
```

### Comparing `preliz-0.2.0/preliz/distributions/__init__.py` & `preliz-0.3.0/preliz/distributions/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 from .continuous import *
 from .discrete import *
+from .continuous_multivariate import *
 
 all_continuous = [
     AsymmetricLaplace,
     Beta,
     BetaScaled,
     Cauchy,
     ChiSquared,
     ExGaussian,
     Exponential,
     Gamma,
     Gumbel,
     HalfCauchy,
     HalfNormal,
-    HalfStudent,
+    HalfStudentT,
     InverseGamma,
+    Kumaraswamy,
     Laplace,
     Logistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
-    Student,
+    StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
 ]
 all_discrete = [
     Bernoulli,
     BetaBinomial,
     Binomial,
     Categorical,
     DiscreteUniform,
     Geometric,
+    HyperGeometric,
     NegativeBinomial,
     Poisson,
+    ZeroInflatedBinomial,
+    ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
 ]
 
+all_continuous_multivariate = [Dirichlet, MvNormal]
 
-__all__ = [s.__name__ for s in all_continuous] + [s.__name__ for s in all_discrete]
+
+__all__ = (
+    [s.__name__ for s in all_continuous]
+    + [s.__name__ for s in all_discrete]
+    + [s.__name__ for s in all_continuous_multivariate]
+)
```

### Comparing `preliz-0.2.0/preliz/distributions/continuous.py` & `preliz-0.3.0/preliz/distributions/continuous.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 Continuous probability distributions.
 """
 from copy import copy
 
 import numpy as np
 from scipy import stats
 from scipy.special import gamma as gammaf
+from scipy.special import beta as betaf  # pylint: disable=no-name-in-module
 from scipy.special import logit, expit  # pylint: disable=no-name-in-module
 
-from ..internal.optimization import optimize_ml
-from ..internal.distribution_helper import garcia_approximation, all_not_none
+from ..internal.optimization import optimize_ml, optimize_moments
+from ..internal.distribution_helper import garcia_approximation, all_not_none, any_not_none
 from .distributions import Continuous
 
 eps = np.finfo(float).eps
 
 
 def from_precision(precision):
     sigma = 1 / precision**0.5
@@ -87,43 +88,43 @@
     def __init__(self, kappa=None, mu=None, b=None, q=None):
         super().__init__()
         self.dist = copy(stats.laplace_asymmetric)
         self.support = (-np.inf, np.inf)
         self._parametrization(kappa, mu, b, q)
 
     def _parametrization(self, kappa=None, mu=None, b=None, q=None):
-        if kappa is not None and q is not None:
+        if all_not_none(kappa, q):
             raise ValueError("Incompatible parametrization. Either use kappa or q.")
 
         self.param_names = ("kappa", "mu", "b")
         self.params_support = ((eps, np.inf), (-np.inf, np.inf), (eps, np.inf))
 
         if q is not None:
             self.q = q
             kappa = self._from_q(q)
             self.param_names = ("q", "mu", "b")
             self.params_support = ((eps, 1 - eps), (-np.inf, np.inf), (eps, np.inf))
 
         self.kappa = kappa
         self.mu = mu
         self.b = b
-        if (kappa and mu and b) is not None:
+        if all_not_none(kappa, mu, b):
             self._update(kappa, mu, b)
 
     def _from_q(self, q):
         kappa = (q / (1 - q)) ** 0.5
         return kappa
 
     def _to_q(self, kappa):
         q = kappa**2 / (1 + kappa**2)
         return q
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(kappa=self.kappa, loc=self.mu, scale=self.b)
         return frozen
 
     def _update(self, kappa, mu, b):
         self.kappa = np.float64(kappa)
         self.mu = np.float64(mu)
         self.b = np.float64(b)
@@ -206,44 +207,44 @@
         super().__init__()
         self.dist = copy(stats.beta)
         self.support = (0, 1)
         self._parametrization(alpha, beta, mu, sigma, kappa)
 
     def _parametrization(self, alpha=None, beta=None, mu=None, sigma=None, kappa=None):
         if (
-            (alpha or beta) is not None
-            and (mu or sigma or kappa) is not None
-            or (sigma and kappa) is not None
+            any_not_none(alpha, beta)
+            and any_not_none(mu, sigma, kappa)
+            or all_not_none(sigma, kappa)
         ):
             raise ValueError(
                 "Incompatible parametrization. Either use alpha " "and beta, or mu and sigma."
             )
 
         self.param_names = ("alpha", "beta")
         self.params_support = ((eps, np.inf), (eps, np.inf))
 
-        if (mu or sigma) is not None:
+        if any_not_none(mu, sigma):
             self.mu = mu
             self.sigma = sigma
             self.param_names = ("mu", "sigma")
             self.params_support = ((eps, 1 - eps), (eps, 1 - eps))
-            if (mu and sigma) is not None:
+            if all_not_none(mu, sigma):
                 alpha, beta = self._from_mu_sigma(mu, sigma)
 
-        if (mu or kappa) is not None:
+        if any_not_none(mu, kappa):
             self.mu = mu
             self.kappa = kappa
             self.param_names = ("mu", "kappa")
             self.params_support = ((eps, 1 - eps), (eps, np.inf))
-            if (mu and kappa) is not None:
+            if all_not_none(mu, kappa):
                 alpha, beta = self._from_mu_kappa(mu, kappa)
 
         self.alpha = alpha
         self.beta = beta
-        if (self.alpha and self.beta) is not None:
+        if all_not_none(self.alpha, self.beta):
             self._update(self.alpha, self.beta)
 
     def _from_mu_sigma(self, mu, sigma):
         kappa = mu * (1 - mu) / sigma**2 - 1
         alpha = mu * kappa
         beta = (1 - mu) * kappa
         return alpha, beta
@@ -257,15 +258,15 @@
         alpha_plus_beta = alpha + beta
         mu = alpha / alpha_plus_beta
         sigma = (alpha * beta) ** 0.5 / alpha_plus_beta / (alpha_plus_beta + 1) ** 0.5
         return mu, sigma
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.alpha, self.beta)
         return frozen
 
     def _update(self, alpha, beta):
         self.alpha = np.float64(alpha)
         self.beta = np.float64(beta)
         self.mu, self.sigma = self._to_mu_sigma(self.alpha, self.beta)
@@ -343,20 +344,20 @@
         self.dist = copy(stats.beta)
         self.support = (lower, upper)
         self._parametrization(self.alpha, self.beta, self.lower, self.upper)
 
     def _parametrization(self, alpha=None, beta=None, lower=None, upper=None):
         self.param_names = ("alpha", "beta", "lower", "upper")
         self.params_support = ((eps, np.inf), (eps, np.inf), (-np.inf, np.inf), (-np.inf, np.inf))
-        if (alpha and beta) is not None:
+        if all_not_none(alpha, beta):
             self._update(alpha, beta, lower, upper)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.alpha, self.beta, loc=self.lower, scale=self.upper - self.lower)
         return frozen
 
     def _update(self, alpha, beta, lower=None, upper=None):
         if lower is not None:
             self.lower = np.float64(lower)
         if upper is not None:
@@ -425,20 +426,20 @@
 
     def _parametrization(self, alpha=None, beta=None):
         self.alpha = alpha
         self.beta = beta
         self.param_names = ("alpha", "beta")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf))
         self.params = (self.alpha, self.beta)
-        if (alpha and beta) is not None:
+        if all_not_none(alpha, beta):
             self._update(alpha, beta)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.alpha, self.beta)
         return frozen
 
     def _update(self, alpha, beta):
         self.alpha = np.float64(alpha)
         self.beta = np.float64(beta)
         self.params = (self.alpha, self.beta)
@@ -452,15 +453,15 @@
     def _fit_mle(self, sample, **kwargs):
         alpha, beta = self.dist.fit(sample, **kwargs)
         self._update(alpha, beta)
 
 
 class ChiSquared(Continuous):
     r"""
-    Chi squared  log-likelihood.
+    Chi squared  distribution.
 
     The pdf of this distribution is
 
     .. math::
 
        f(x \mid \nu) =
                 \frac{x^{(\nu-2)/2}e^{-x/2}}{2^{\nu/2}\Gamma(\nu/2)}
@@ -501,15 +502,15 @@
         self.params_support = ((eps, np.inf),)
         self.params = (self.nu,)
         if self.nu is not None:
             self._update(self.nu)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.nu)
         return frozen
 
     def _update(self, nu):
         self.nu = np.float64(nu)
         self.params = (self.nu,)
         self._update_rv_frozen()
@@ -579,20 +580,20 @@
     def _parametrization(self, mu=None, sigma=None, nu=None):
         self.nu = nu
         self.mu = mu
         self.sigma = sigma
         self.param_names = ("mu", "sigma", "nu")
         self.params = (mu, sigma, nu)
         self.params_support = ((-np.inf, np.inf), (eps, np.inf), (eps, np.inf))
-        if (mu and sigma and nu) is not None:
+        if all_not_none(mu, sigma, nu):
             self._update(mu, sigma, nu)
 
     def _get_frozen(self):
         frozen = None
-        if self.nu is not None and self.sigma is not None:
+        if all_not_none(self.nu, self.sigma):
             frozen = self.dist(K=self.nu / self.sigma, loc=self.mu, scale=self.sigma)
         return frozen
 
     def _update(self, mu, sigma, nu):
         self.nu = np.float64(nu)
         self.mu = np.float64(mu)
         self.sigma = np.float64(sigma)
@@ -630,44 +631,68 @@
 
     ========  ============================
     Support   :math:`x \in [0, \infty)`
     Mean      :math:`\dfrac{1}{\lambda}`
     Variance  :math:`\dfrac{1}{\lambda^2}`
     ========  ============================
 
+    Exponential distribution has 2 alternative parametrizations. In terms of lambda (rate)
+    or in terms of beta (scale).
+
+    The link between the two alternatives is given by:
+
+    .. math::
+
+        \beta = \dfrac{1}{\lambda}
+
     Parameters
     ----------
     lam : float
         Rate or inverse scale (lam > 0).
+    beta : float
+        Scale (beta > 0).
     """
 
-    def __init__(self, lam=None):
+    def __init__(self, lam=None, beta=None):
         super().__init__()
-        self.lam = lam
         self.dist = copy(stats.expon)
         self.support = (0, np.inf)
-        self._parametrization(lam)
+        self._parametrization(lam, beta)
+
+    def _parametrization(self, lam=None, beta=None):
+        if all_not_none(lam, beta):
+            raise ValueError("Incompatible parametrization. Either use 'lam' or 'beta'.")
 
-    def _parametrization(self, lam=None):
-        self.lam = lam
-        self.params = (self.lam,)
         self.param_names = ("lam",)
         self.params_support = ((eps, np.inf),)
+
+        if beta is not None:
+            lam = 1 / beta
+            self.param_names = ("beta",)
+
+        self.lam = lam
+        self.beta = beta
         if self.lam is not None:
             self._update(self.lam)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(scale=1 / self.lam)
         return frozen
 
     def _update(self, lam):
         self.lam = np.float64(lam)
-        self.params = (self.lam,)
+        self.beta = 1 / lam
+
+        if self.param_names[0] == "lam":
+            self.params = (self.lam,)
+        elif self.param_names[0] == "beta":
+            self.params = (self.beta,)
+
         self._update_rv_frozen()
 
     def _fit_moments(self, mean, sigma=None):  # pylint: disable=unused-argument
         lam = 1 / mean
         self._update(lam)
 
     def _fit_mle(self, sample, **kwargs):
@@ -731,47 +756,47 @@
     def __init__(self, alpha=None, beta=None, mu=None, sigma=None):
         super().__init__()
         self.dist = copy(stats.gamma)
         self.support = (0, np.inf)
         self._parametrization(alpha, beta, mu, sigma)
 
     def _parametrization(self, alpha=None, beta=None, mu=None, sigma=None):
-        if (alpha or beta) is not None and (mu or sigma) is not None:
+        if any_not_none(alpha, beta) and any_not_none(mu, sigma):
             raise ValueError(
                 "Incompatible parametrization. Either use alpha and beta or mu and sigma."
             )
 
         self.param_names = ("alpha", "beta")
         self.params_support = ((eps, np.inf), (eps, np.inf))
 
-        if (mu or sigma) is not None:
+        if any_not_none(mu, sigma):
             self.mu = mu
             self.sigma = sigma
             self.param_names = ("mu", "sigma")
-            if (mu and sigma) is not None:
+            if all_not_none(mu, sigma):
                 alpha, beta = self._from_mu_sigma(mu, sigma)
 
         self.alpha = alpha
         self.beta = beta
-        if self.alpha is not None and self.beta is not None:
+        if all_not_none(self.alpha, self.beta):
             self._update(self.alpha, self.beta)
 
     def _from_mu_sigma(self, mu, sigma):
         alpha = mu**2 / sigma**2
         beta = mu / sigma**2
         return alpha, beta
 
     def _to_mu_sigma(self, alpha, beta):
         mu = alpha / beta
         sigma = alpha**0.5 / beta
         return mu, sigma
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(a=self.alpha, scale=1 / self.beta)
         return frozen
 
     def _update(self, alpha, beta):
         self.alpha = np.float64(alpha)
         self.beta = np.float64(beta)
         self.mu, self.sigma = self._to_mu_sigma(self.alpha, self.beta)
@@ -841,20 +866,20 @@
 
     def _parametrization(self, mu=None, beta=None):
         self.mu = mu
         self.beta = beta
         self.params = (self.mu, self.beta)
         self.param_names = ("mu", "beta")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf))
-        if (self.mu and self.beta) is not None:
+        if all_not_none(self.mu, self.beta):
             self._update(self.mu, self.beta)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(loc=self.mu, scale=self.beta)
         return frozen
 
     def _update(self, mu, beta):
         self.mu = np.float64(mu)
         self.beta = np.float64(beta)
         self.params = (self.mu, self.beta)
@@ -914,15 +939,15 @@
         self.param_names = ("beta",)
         self.params_support = ((eps, np.inf),)
         if self.beta is not None:
             self._update(self.beta)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(scale=self.beta)
         return frozen
 
     def _update(self, beta):
         self.beta = np.float64(beta)
         self.params = (self.beta,)
         self._update_rv_frozen()
@@ -983,15 +1008,15 @@
     def __init__(self, sigma=None, tau=None):
         super().__init__()
         self.dist = copy(stats.halfnorm)
         self.support = (0, np.inf)
         self._parametrization(sigma, tau)
 
     def _parametrization(self, sigma=None, tau=None):
-        if sigma is not None and tau is not None:
+        if all_not_none(sigma, tau):
             raise ValueError("Incompatible parametrization. Either use sigma or tau.")
 
         self.param_names = ("sigma",)
         self.params_support = ((eps, np.inf),)
 
         if tau is not None:
             sigma = from_precision(tau)
@@ -1000,15 +1025,15 @@
         self.sigma = sigma
         self.tau = tau
         if self.sigma is not None:
             self._update(self.sigma)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(scale=self.sigma)
         return frozen
 
     def _update(self, sigma):
         self.sigma = np.float64(sigma)
         self.tau = to_precision(sigma)
 
@@ -1024,52 +1049,52 @@
         self._update(sigma)
 
     def _fit_mle(self, sample, **kwargs):
         _, sigma = self.dist.fit(sample, **kwargs)
         self._update(sigma)
 
 
-class HalfStudent(Continuous):
+class HalfStudentT(Continuous):
     r"""
-    HalfStudent Distribution
+    HalfStudentT Distribution
 
     The pdf of this distribution is
 
     .. math::
 
         f(x \mid \sigma,\nu) =
             \frac{2\;\Gamma\left(\frac{\nu+1}{2}\right)}
             {\Gamma\left(\frac{\nu}{2}\right)\sqrt{\nu\pi\sigma^2}}
             \left(1+\frac{1}{\nu}\frac{x^2}{\sigma^2}\right)^{-\frac{\nu+1}{2}}
 
     .. plot::
         :context: close-figs
 
         import arviz as az
-        from preliz import HalfStudent
+        from preliz import HalfStudentT
         az.style.use('arviz-white')
         sigmas = [1., 2., 2.]
         nus = [3, 3., 10.]
         for sigma, nu in zip(sigmas, nus):
-            HalfStudent(nu, sigma).plot_pdf(support=(0,10))
+            HalfStudentT(nu, sigma).plot_pdf(support=(0,10))
 
     ========  ==========================================
     Support   :math:`x \in [0, \infty)`
     Mean      .. math::
                   2\sigma\sqrt{\frac{\nu}{\pi}}\
                   \frac{\Gamma\left(\frac{\nu+1}{2}\right)}\
                   {\Gamma\left(\frac{\nu}{2}\right)(\nu-1)}\, \text{for } \nu > 2
     Variance  .. math::
                   \sigma^2\left(\frac{\nu}{\nu - 2}-\
                   \frac{4\nu}{\pi(\nu-1)^2}\left(\frac{\Gamma\left(\frac{\nu+1}{2}\right)}\
                   {\Gamma\left(\frac{\nu}{2}\right)}\right)^2\right) \text{for } \nu > 2\, \infty\
                   \text{for } 1 < \nu \le 2\, \text{otherwise undefined}
     ========  ==========================================
 
-    HalfStudent distribution has 2 alternative parameterizations. In terms of nu and
+    HalfStudentT distribution has 2 alternative parameterizations. In terms of nu and
     sigma (standard deviation as nu increases) or nu lam (precision as nu increases).
 
     The link between the 2 alternatives is given by
 
     .. math::
 
         \lambda = \frac{1}{\sigma^2}
@@ -1083,40 +1108,40 @@
         increases.
     lam : float
         Scale parameter (lam > 0). Converges to the precision as nu increases.
     """
 
     def __init__(self, nu=None, sigma=None, lam=None):
         super().__init__()
-        self.dist = _HalfStudent
+        self.dist = _HalfStudentT
         self.support = (0, np.inf)
         self._parametrization(nu, sigma, lam)
 
     def _parametrization(self, nu=None, sigma=None, lam=None):
-        if sigma is not None and lam is not None:
+        if all_not_none(sigma, lam):
             raise ValueError(
                 "Incompatible parametrization. Either use nu and sigma, or nu and lam."
             )
 
         self.param_names = ("nu", "sigma")
         self.params_support = ((eps, np.inf), (eps, np.inf))
 
         if lam is not None:
             self.lam = lam
             sigma = from_precision(lam)
             self.param_names = ("nu", "lam")
 
         self.nu = nu
         self.sigma = sigma
-        if self.nu is not None and self.sigma is not None:
+        if all_not_none(self.nu, self.sigma):
             self._update(self.nu, self.sigma)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(nu=self.nu, sigma=self.sigma)
         return frozen
 
     def _update(self, nu, sigma):
         self.nu = np.float64(nu)
         self.sigma = np.float64(sigma)
         self.lam = to_precision(sigma)
@@ -1149,15 +1174,15 @@
             sigma = sigma / (1 - 2 / np.pi) ** 0.5
         self._update(nu, sigma)
 
     def _fit_mle(self, sample, **kwargs):
         optimize_ml(self, sample)
 
 
-class _HalfStudent(stats.rv_continuous):
+class _HalfStudentT(stats.rv_continuous):
     def __init__(self, nu=None, sigma=None):
         super().__init__()
         self.nu = nu
         self.sigma = sigma
         self.dist = stats.t(loc=0, df=self.nu, scale=self.sigma)
 
     def support(self, *args, **kwd):  # pylint: disable=unused-argument
@@ -1210,15 +1235,15 @@
 
     def rvs(self, size=1, random_state=None):  # pylint: disable=arguments-differ
         return np.abs(self.dist.rvs(size=size, random_state=random_state))
 
 
 class InverseGamma(Continuous):
     r"""
-    Inverse gamma log-likelihood, the reciprocal of the gamma distribution.
+    Inverse gamma distribution, the reciprocal of the gamma distribution.
 
     The pdf of this distribution is
 
     .. math::
 
        f(x \mid \alpha, \beta) =
            \frac{\beta^{\alpha}}{\Gamma(\alpha)} x^{-\alpha - 1}
@@ -1266,32 +1291,32 @@
     def __init__(self, alpha=None, beta=None, mu=None, sigma=None):
         super().__init__()
         self.dist = copy(stats.invgamma)
         self.support = (0, np.inf)
         self._parametrization(alpha, beta, mu, sigma)
 
     def _parametrization(self, alpha=None, beta=None, mu=None, sigma=None):
-        if (alpha or beta) is not None and (mu or sigma) is not None:
+        if any_not_none(alpha, beta) and any_not_none(mu, sigma):
             raise ValueError(
                 "Incompatible parametrization. Either use alpha and beta or mu and sigma."
             )
 
         self.param_names = ("alpha", "beta")
         self.params_support = ((eps, np.inf), (eps, np.inf))
 
-        if (mu or sigma) is not None:
+        if any_not_none(mu, sigma):
             self.mu = mu
             self.sigma = sigma
             self.param_names = ("mu", "sigma")
-            if (mu and sigma) is not None:
+            if all_not_none(mu, sigma):
                 alpha, beta = self._from_mu_sigma(mu, sigma)
 
         self.alpha = alpha
         self.beta = beta
-        if self.alpha is not None and self.beta is not None:
+        if all_not_none(self.alpha, self.beta):
             self._update(self.alpha, self.beta)
 
     def _from_mu_sigma(self, mu, sigma):
         alpha = mu**2 / sigma**2 + 2
         beta = mu**3 / sigma**2 + mu
         return alpha, beta
 
@@ -1304,15 +1329,15 @@
             sigma = beta / ((alpha - 1) * (alpha - 2) ** 0.5)
         else:
             sigma = None
         return mu, sigma
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(a=self.alpha, scale=self.beta)
         return frozen
 
     def _update(self, alpha, beta):
         self.alpha = np.float64(alpha)
         self.beta = np.float64(beta)
         self.mu, self.sigma = self._to_mu_sigma(self.alpha, self.beta)
@@ -1329,14 +1354,133 @@
         self._update(alpha, beta)
 
     def _fit_mle(self, sample, **kwargs):
         alpha, _, beta = self.dist.fit(sample, **kwargs)
         self._update(alpha, beta)
 
 
+class Kumaraswamy(Continuous):
+    r"""
+    Kumaraswamy distribution.
+
+    The pdf of this distribution is
+
+    .. math::
+
+         f(x \mid a, b) = a b x^{a - 1} (1 - x^a)^{b - 1}
+
+    .. plot::
+        :context: close-figs
+
+        import arviz as az
+        from preliz import Kumaraswamy
+        az.style.use('arviz-white')
+        a_s = [.5, 5., 1., 2., 2.]
+        b_s = [.5, 1., 3., 2., 5.]
+        for a, b in zip(a_s, b_s):
+            ax = Kumaraswamy(a, b).plot_pdf()
+            ax.set_ylim(0, 3.)
+
+    ========  ==============================================================
+    Support   :math:`x \in (0, 1)`
+    Mean      :math:`b B(1 + \tfrac{1}{a}, b)`
+    Variance  :math:`b B(1 + \tfrac{2}{a}, b) - (b B(1 + \tfrac{1}{a}, b))^2`
+    ========  ==============================================================
+
+    Parameters
+    ----------
+    a : float
+        a > 0.
+    b : float
+        b > 0.
+    """
+
+    def __init__(self, a=None, b=None):
+        super().__init__()
+        self.dist = _Kumaraswamy
+        self.support = (0, 1)
+        self._parametrization(a, b)
+
+    def _parametrization(self, a=None, b=None):
+        self.a = a
+        self.b = b
+        self.params = (self.a, self.b)
+        self.param_names = ("a", "b")
+        self.params_support = ((eps, np.inf), (eps, np.inf))
+        if (a and b) is not None:
+            self._update(a, b)
+
+    def _get_frozen(self):
+        frozen = None
+        if all_not_none(self.params):
+            frozen = self.dist(self.a, self.b)
+        return frozen
+
+    def _update(self, a, b):
+        self.a = np.float64(a)
+        self.b = np.float64(b)
+        self.params = (self.a, self.b)
+        self._update_rv_frozen()
+
+    def _fit_moments(self, mean, sigma):
+        optimize_moments(self, mean, sigma)
+
+    def _fit_mle(self, sample, **kwargs):
+        optimize_ml(self, sample, **kwargs)
+
+
+class _Kumaraswamy(stats.rv_continuous):
+    def __init__(self, a=None, b=None):
+        super().__init__()
+        self.a = a
+        self.b = b
+
+    def support(self, *args, **kwds):  # pylint: disable=unused-argument
+        return (0, 1)
+
+    def cdf(self, x, *args, **kwds):  # pylint: disable=unused-argument
+        return 1 - (1 - x**self.a) ** self.b
+
+    def pdf(self, x, *args, **kwds):  # pylint: disable=unused-argument
+        return (self.a * self.b * x ** (self.a - 1)) * ((1 - x**self.a) ** (self.b - 1))
+
+    def logpdf(self, x, *args, **kwds):  # pylint: disable=unused-argument
+        return (
+            np.log(self.a * self.b)
+            + (self.a - 1) * np.log(x)
+            + (self.b - 1) * np.log(1 - x**self.a)
+        )
+
+    def ppf(self, q, *args, **kwds):  # pylint: disable=unused-argument
+        return (1 - (1 - q) ** (1 / self.b)) ** (1 / self.a)
+
+    def _stats(self, *args, **kwds):  # pylint: disable=unused-argument
+        mean = self.b * betaf(1 + 1 / self.a, self.b)
+        var = self.b * betaf(1 + 2 / self.a, self.b) - self.b * betaf(1 + 2 / self.a, self.b) ** 2
+        return (mean, var, np.nan, np.nan)
+
+    def entropy(self, *args, **kwds):  # pylint: disable=unused-argument
+        # https://www.ijicc.net/images/vol12/iss4/12449_Nassir_2020_E_R.pdf
+        return (
+            (1 - 1 / self.b)
+            + (1 - 1 / self.a) * sum(1 / i for i in range(1, int(self.b) + 1))
+            - np.log(self.a * self.b)
+        )
+
+    def rvs(self, size=1, random_state=None):  # pylint: disable=arguments-differ
+        if random_state is None:
+            q = np.random.rand(size)
+        elif isinstance(random_state, int):
+            q = np.random.default_rng(random_state).random(size)
+        else:
+            q = random_state.random(size)
+
+        return self.ppf(q)
+
+
 class Laplace(Continuous):
     r"""
     Laplace distribution.
 
     The pdf of this distribution is
 
     .. math::
@@ -1377,20 +1521,20 @@
 
     def _parametrization(self, mu=None, b=None):
         self.mu = mu
         self.b = b
         self.params = (self.mu, self.b)
         self.param_names = ("mu", "b")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf))
-        if (mu and b) is not None:
+        if all_not_none(mu, b):
             self._update(mu, b)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(loc=self.mu, scale=self.b)
         return frozen
 
     def _update(self, mu, b):
         self.mu = np.float64(mu)
         self.b = np.float64(b)
         self.params = (self.mu, self.b)
@@ -1451,20 +1595,20 @@
 
     def _parametrization(self, mu=None, s=None):
         self.mu = mu
         self.s = s
         self.params = (self.mu, self.s)
         self.param_names = ("mu", "s")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf))
-        if (self.mu and self.s) is not None:
+        if all_not_none(self.mu, self.s):
             self._update(self.mu, self.s)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(loc=self.mu, scale=self.s)
         return frozen
 
     def _update(self, mu, s):
         self.mu = np.float64(mu)
         self.s = np.float64(s)
         self.params = (self.mu, self.s)
@@ -1530,20 +1674,20 @@
 
     def _parametrization(self, mu=None, sigma=None):
         self.mu = mu
         self.sigma = sigma
         self.params = (self.mu, self.sigma)
         self.param_names = ("mu", "sigma")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf))
-        if (mu and sigma) is not None:
+        if all_not_none(mu, sigma):
             self._update(mu, sigma)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.sigma, scale=np.exp(self.mu))
         return frozen
 
     def _update(self, mu, sigma):
         self.mu = np.float64(mu)
         self.sigma = np.float64(sigma)
         self.params = (self.mu, self.sigma)
@@ -1557,15 +1701,15 @@
     def _fit_mle(self, sample, **kwargs):
         sigma, _, mu = self.dist.fit(sample, **kwargs)
         self._update(np.log(mu), sigma)
 
 
 class LogitNormal(Continuous):
     r"""
-    Logit-Normal log-likelihood.
+    Logit-Normal distribution.
 
     The pdf of this distribution is
 
     .. math::
        f(x \mid \mu, \tau) =
            \frac{1}{x(1-x)} \sqrt{\frac{\tau}{2\pi}}
            \exp\left\{ -\frac{\tau}{2} (logit(x)-\mu)^2 \right\}
@@ -1601,15 +1745,15 @@
     def __init__(self, mu=None, sigma=None, tau=None):
         super().__init__()
         self.dist = _LogitNormal
         self.support = (0, 1)
         self._parametrization(mu, sigma, tau)
 
     def _parametrization(self, mu=None, sigma=None, tau=None):
-        if sigma is not None and tau is not None:
+        if all_not_none(sigma, tau):
             raise ValueError(
                 "Incompatible parametrization. Either use mu and sigma, or mu and tau."
             )
 
         names = ("mu", "sigma")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf))
 
@@ -1617,20 +1761,20 @@
             self.tau = tau
             sigma = from_precision(tau)
             names = ("mu", "tau")
 
         self.mu = mu
         self.sigma = sigma
         self.param_names = names
-        if mu is not None and sigma is not None:
+        if all_not_none(mu, sigma):
             self._update(mu, sigma)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.mu, self.sigma)
         return frozen
 
     def _update(self, mu, sigma):
         self.mu = np.float64(mu)
         self.sigma = np.float64(sigma)
         self.tau = to_precision(sigma)
@@ -1654,15 +1798,15 @@
 
 class _LogitNormal(stats.rv_continuous):
     def __init__(self, mu=None, sigma=None):
         super().__init__()
         self.mu = mu
         self.sigma = sigma
 
-    def support(self, *args, **kwd):  # pylint: disable=unused-argument
+    def support(self, *args, **kwds):  # pylint: disable=unused-argument
         return (0, 1)
 
     def cdf(self, x, *args, **kwds):
         return stats.norm(self.mu, self.sigma, *args, **kwds).cdf(logit(x))
 
     def pdf(self, x, *args, **kwds):
         x = np.asarray(x)
@@ -1758,20 +1902,20 @@
 
     def _parametrization(self, mu=None, sigma=None):
         self.mu = mu
         self.sigma = sigma
         self.params = (self.mu, self.sigma)
         self.param_names = ("mu", "sigma")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf))
-        if (mu and sigma) is not None:
+        if all_not_none(mu, sigma):
             self._update(self.mu, self.sigma)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(loc=self.mu, scale=self.sigma)
         return frozen
 
     def _update(self, mu, sigma):
         self.mu = np.float64(mu)
         self.sigma = np.float64(sigma)
         self.params = (self.mu, self.sigma)
@@ -1838,15 +1982,15 @@
     def __init__(self, mu=None, sigma=None, tau=None):
         super().__init__()
         self.dist = copy(stats.norm)
         self.support = (-np.inf, np.inf)
         self._parametrization(mu, sigma, tau)
 
     def _parametrization(self, mu=None, sigma=None, tau=None):
-        if sigma is not None and tau is not None:
+        if all_not_none(sigma, tau):
             raise ValueError(
                 "Incompatible parametrization. Either use mu and sigma, or mu and tau."
             )
 
         names = ("mu", "sigma")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf))
 
@@ -1854,20 +1998,20 @@
             self.tau = tau
             sigma = from_precision(tau)
             names = ("mu", "tau")
 
         self.mu = mu
         self.sigma = sigma
         self.param_names = names
-        if mu is not None and sigma is not None:
+        if all_not_none(mu, sigma):
             self._update(mu, sigma)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.mu, self.sigma)
         return frozen
 
     def _update(self, mu, sigma):
         self.mu = np.float64(mu)
         self.sigma = np.float64(sigma)
         self.tau = to_precision(sigma)
@@ -1885,15 +2029,15 @@
     def _fit_mle(self, sample, **kwargs):
         mu, sigma = self.dist.fit(sample, **kwargs)
         self._update(mu, sigma)
 
 
 class Pareto(Continuous):
     r"""
-    Pareto log-likelihood.
+    Pareto distribution.
 
     The pdf of this distribution is
 
     .. math::
 
        f(x \mid \alpha, m) = \frac{\alpha m^{\alpha}}{x^{\alpha+1}}
 
@@ -1930,20 +2074,20 @@
 
     def _parametrization(self, alpha=None, m=None):
         self.alpha = alpha
         self.m = m
         self.params = (self.alpha, self.m)
         self.param_names = ("alpha", "m")
         self.params_support = ((eps, np.inf), (eps, np.inf))
-        if (alpha and m) is not None:
+        if all_not_none(alpha, m):
             self._update(alpha, m)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.alpha, scale=self.m)
         return frozen
 
     def _update(self, alpha, m):
         self.alpha = np.float64(alpha)
         self.m = np.float64(m)
         self.support = (self.m, np.inf)
@@ -2014,45 +2158,45 @@
         super().__init__()
         self.name = "rice"
         self.dist = copy(stats.rice)
         self.support = (0, np.inf)
         self._parametrization(nu, sigma, b)
 
     def _parametrization(self, nu=None, sigma=None, b=None):
-        if nu is not None and b is not None:
+        if all_not_none(nu, b):
             raise ValueError(
                 "Incompatible parametrization. Either use nu and sigma or b and sigma."
             )
 
         self.param_names = ("nu", "sigma")
         self.params_support = ((eps, np.inf), (eps, np.inf))
 
         if b is not None:
             self.b = b
             self.sigma = sigma
             self.param_names = ("b", "sigma")
-            if (b and sigma) is not None:
+            if all_not_none(b, sigma):
                 nu = self._from_b(b, sigma)
 
         self.nu = nu
         self.sigma = sigma
-        if self.nu is not None and self.sigma is not None:
+        if all_not_none(self.nu, self.sigma):
             self._update(self.nu, self.sigma)
 
     def _from_b(self, b, sigma):
         nu = b * sigma
         return nu
 
     def _to_b(self, nu, sigma):
         b = nu / sigma
         return b
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             b_ = self._to_b(self.nu, self.sigma)
             frozen = self.dist(b=b_, scale=self.sigma)
         return frozen
 
     def _update(self, nu, sigma):
         self.nu = np.float64(nu)
         self.sigma = np.float64(sigma)
@@ -2062,15 +2206,16 @@
             self.params = (self.nu, self.sigma)
         elif self.param_names[0] == "b":
             self.params = (self.b, self.sigma)
 
         self._update_rv_frozen()
 
     def _fit_moments(self, mean, sigma):
-        self._update(mean, sigma)
+        params = mean, sigma
+        optimize_moments(self, mean, sigma, params)
 
     def _fit_mle(self, sample, **kwargs):
         b, _, sigma = self.dist.fit(sample, **kwargs)
         nu = self._from_b(b, sigma)
         self._update(nu, sigma)
 
 
@@ -2130,15 +2275,15 @@
     def __init__(self, mu=None, sigma=None, alpha=None, tau=None):
         super().__init__()
         self.dist = copy(stats.skewnorm)
         self.support = (-np.inf, np.inf)
         self._parametrization(mu, sigma, alpha, tau)
 
     def _parametrization(self, mu=None, sigma=None, alpha=None, tau=None):
-        if sigma is not None and tau is not None:
+        if all_not_none(sigma, tau):
             raise ValueError(
                 "Incompatible parametrization. Either use mu, sigma and alpha,"
                 " or mu, tau and alpha."
             )
 
         self.param_names = ("mu", "sigma", "alpha")
         self.params_support = ((-np.inf, np.inf), (eps, np.inf), (-np.inf, np.inf))
@@ -2147,20 +2292,20 @@
             self.tau = tau
             sigma = from_precision(tau)
             self.param_names = ("mu", "tau", "alpha")
 
         self.mu = mu
         self.sigma = sigma
         self.alpha = alpha
-        if self.mu is not None and self.sigma is not None and self.alpha is not None:
+        if all_not_none(self.mu, self.sigma, self.alpha):
             self._update(self.mu, self.sigma, self.alpha)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.alpha, self.mu, self.sigma)
         return frozen
 
     def _update(self, mu, sigma, alpha):
         self.mu = np.float64(mu)
         self.sigma = np.float64(sigma)
         self.alpha = np.float64(alpha)
@@ -2178,17 +2323,17 @@
         self._update(mean, sigma, 0)
 
     def _fit_mle(self, sample, **kwargs):
         alpha, mu, sigma = self.dist.fit(sample, **kwargs)
         self._update(mu, sigma, alpha)
 
 
-class Student(Continuous):
+class StudentT(Continuous):
     r"""
-    Student's T log-likelihood.
+    StudentT's distribution.
 
     Describes a normal variable whose precision is gamma distributed.
 
     The pdf of this distribution is
 
     .. math::
 
@@ -2196,30 +2341,30 @@
            \frac{\Gamma \left(\frac{\nu+1}{2} \right)} {\sqrt{\nu\pi}\
            \Gamma \left(\frac{\nu}{2} \right)} \left(1+\frac{x^2}{\nu} \right)^{-\frac{\nu+1}{2}}
 
     .. plot::
         :context: close-figs
 
         import arviz as az
-        from preliz import Student
+        from preliz import StudentT
         az.style.use('arviz-white')
         nus = [2., 5., 5.]
         mus = [0., 0.,  -4.]
         sigmas = [1., 1., 2.]
         for nu, mu, sigma in zip(nus, mus, sigmas):
-            Student(nu, mu, sigma).plot_pdf(support=(-10,6))
+            StudentT(nu, mu, sigma).plot_pdf(support=(-10,6))
 
     ========  ========================
     Support   :math:`x \in \mathbb{R}`
     Mean      :math:`\mu` for :math:`\nu > 1`, otherwise undefined
     Variance  :math:`\frac{\nu}{\nu-2}` for :math:`\nu > 2`,
               :math:`\infty` for :math:`1 < \nu \le 2`, otherwise undefined
     ========  ========================
 
-    Student's T distribution has 2 alternative parameterizations. In terms of nu, mu and
+    StudentT distribution has 2 alternative parameterizations. In terms of nu, mu and
     sigma (standard deviation as nu increases) or nu, mu and lam (precision as nu increases).
 
     The link between the 2 alternatives is given by
 
     .. math::
 
         \lambda = \frac{1}{\sigma^2}
@@ -2241,15 +2386,15 @@
         super().__init__()
         self.dist = copy(stats.t)
         self.support = (-np.inf, np.inf)
         self.params_support = ((eps, np.inf), (-np.inf, np.inf), (eps, np.inf))
         self._parametrization(nu, mu, sigma, lam)
 
     def _parametrization(self, nu=None, mu=None, sigma=None, lam=None):
-        if sigma is not None and lam is not None:
+        if all_not_none(sigma, lam):
             raise ValueError(
                 "Incompatible parametrization. Either use nu, mu and sigma, or nu, mu and lam."
             )
 
         self.param_names = ("nu", "mu", "sigma")
         self.params_support = ((eps, np.inf), (-np.inf, np.inf), (eps, np.inf))
 
@@ -2258,20 +2403,20 @@
             sigma = from_precision(lam)
             self.param_names = ("nu", "mu", "lam")
 
         self.nu = nu
         self.mu = mu
         self.sigma = sigma
 
-        if self.nu is not None and self.mu is not None and self.sigma is not None:
+        if all_not_none(self.nu, self.mu, self.sigma):
             self._update(self.nu, self.mu, self.sigma)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.nu, self.mu, self.sigma)
         return frozen
 
     def _update(self, nu, mu, sigma):
         self.nu = np.float64(nu)
         self.mu = np.float64(mu)
         self.sigma = np.float64(sigma)
@@ -2357,20 +2502,20 @@
     def _parametrization(self, lower=None, c=None, upper=None):
         self.lower = lower
         self.c = c
         self.upper = upper
         self.params = (self.lower, self.c, self.upper)
         self.param_names = ("lower", "c", "upper")
         self.params_support = ((-np.inf, np.inf), (-np.inf, np.inf), (-np.inf, np.inf))
-        if (lower and c and upper) is not None:
+        if all_not_none(lower, c, upper):
             self._update(lower, c, upper)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             scale = self.upper - self.lower
             c_ = (self.c - self.lower) / scale
             frozen = self.dist(c=c_, loc=self.lower, scale=scale)
         return frozen
 
     def _update(self, lower, c, upper):
         self.lower = np.float64(lower)
@@ -2456,20 +2601,20 @@
             (-np.inf, np.inf),
         )
         if lower is None:
             self.lower = -np.inf
         if upper is None:
             self.upper = np.inf
         self.support = (self.lower, self.upper)
-        if (mu and sigma and lower and upper) is not None:
+        if all_not_none(mu, sigma, lower, upper):
             self._update(mu, sigma, lower, upper)
 
     def _get_frozen(self):
         frozen = None
-        if self.mu is not None or self.sigma is not None:
+        if any_not_none(self.mu, self.sigma):
             a, b = (self.lower - self.mu) / self.sigma, (self.upper - self.mu) / self.sigma
             frozen = self.dist(a, b, self.mu, self.sigma)
         return frozen
 
     def _update(self, mu, sigma, lower=None, upper=None):
         if lower is not None:
             self.lower = np.float64(lower)
@@ -2538,25 +2683,25 @@
         self.param_names = ("lower", "upper")
         self.params_support = ((-np.inf, np.inf), (-np.inf, np.inf))
         if lower is None:
             self.lower = -np.inf
         if upper is None:
             self.upper = np.inf
         self.support = (self.lower, self.upper)
-        if (lower and upper) is not None:
+        if all_not_none(lower, upper):
             self._update(lower, upper)
             self.dist.a = self.lower
             self.dist.b = self.upper
         else:
             self.lower = lower
             self.upper = upper
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.lower, self.upper - self.lower)
         return frozen
 
     def _update(self, lower, upper):
         self.lower = np.float64(lower)
         self.upper = np.float64(upper)
         self.params = (self.lower, self.upper)
@@ -2572,15 +2717,15 @@
         lower = np.min(sample)
         upper = np.max(sample)
         self._update(lower, upper)
 
 
 class VonMises(Continuous):
     r"""
-    Univariate VonMises log-likelihood.
+    Univariate VonMises distribution.
 
     The pdf of this distribution is
 
     .. math::
 
         f(x \mid \mu, \kappa) =
             \frac{e^{\kappa\cos(x-\mu)}}{2\pi I_0(\kappa)}
@@ -2619,20 +2764,20 @@
 
     def _parametrization(self, mu=None, kappa=None):
         self.mu = mu
         self.kappa = kappa
         self.param_names = ("mu", "kappa")
         self.params_support = ((-np.pi, np.pi), (eps, np.inf))
         self.support = (-np.pi, np.pi)
-        if (mu and kappa) is not None:
+        if all_not_none(mu, kappa):
             self._update(mu, kappa)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(kappa=self.kappa, loc=self.mu)
         return frozen
 
     def _update(self, mu, kappa):
         self.mu = np.float64(mu)
         self.kappa = np.float64(kappa)
         self.params = (self.mu, self.kappa)
@@ -2675,46 +2820,93 @@
 
     ========  =============================
     Support   :math:`x \in (0, \infty)`
     Mean      :math:`\mu`
     Variance  :math:`\dfrac{\mu^3}{\lambda}`
     ========  =============================
 
+    Wald distribution has 3 alternative parametrizations. In terms of mu and lam,
+    mu and phi or lam and phi.
+
+    The link between the 3 alternatives is given by
+
+    .. math::
+
+       \phi = \dfrac{\lambda}{\mu}
+
     Parameters
     ----------
     mu : float
         Mean of the distribution (mu > 0).
     lam : float
         Relative precision (lam > 0).
+    phi : float
+        Shape parameter (phi > 0).
     """
 
-    def __init__(self, mu=None, lam=None):
+    def __init__(self, mu=None, lam=None, phi=None):
         super().__init__()
         self.dist = copy(stats.invgauss)
         self.support = (0, np.inf)
-        self._parametrization(mu, lam)
+        self._parametrization(mu, lam, phi)
+
+    def _parametrization(self, mu=None, lam=None, phi=None):
+        if (mu and lam and phi) is not None:
+            raise ValueError(
+                "Incompatible parametrization. Either use mu and lam or mu and phi or lam and phi."
+            )
 
-    def _parametrization(self, mu=None, lam=None):
-        self.mu = mu
-        self.lam = lam
         self.param_names = ("mu", "lam")
         self.params_support = ((eps, np.inf), (eps, np.inf))
-        if (mu and lam) is not None:
-            self._update(mu, lam)
+
+        if phi is not None:
+            self.phi = phi
+            if (mu and phi) is not None:
+                lam = self._from_mu_phi(mu, phi)
+                self.param_names = ("mu", "phi")
+
+            elif (lam and phi) is not None:
+                mu = self._from_lam_phi(lam, phi)
+                self.param_names = ("lam", "phi")
+
+        self.mu = mu
+        self.lam = lam
+        if all_not_none(self.mu, self.lam):
+            self._update(self.mu, self.lam)
+
+    def _from_mu_phi(self, mu, phi):
+        lam = mu * phi
+        return lam
+
+    def _from_lam_phi(self, lam, phi):
+        mu = lam / phi
+        return mu
+
+    def _to_phi(self, mu, lam):
+        phi = lam / mu
+        return phi
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.mu / self.lam, scale=self.lam)
         return frozen
 
     def _update(self, mu, lam):
         self.mu = np.float64(mu)
         self.lam = np.float64(lam)
-        self.params = (self.mu, self.lam)
+        self.phi = self._to_phi(mu, lam)
+
+        if self.param_names == ("mu", "lam"):
+            self.params = (self.mu, self.lam)
+        elif self.param_names == ("mu", "phi"):
+            self.params = (self.mu, self.phi)
+        elif self.param_names == ("lam", "phi"):
+            self.params = (self.lam, self.phi)
+
         self._update_rv_frozen()
 
     def _fit_moments(self, mean, sigma):
         lam = mean**3 / sigma**2
         self._update(mean, lam)
 
     def _fit_mle(self, sample, **kwargs):
@@ -2766,20 +2958,20 @@
         self._parametrization(alpha, beta)
 
     def _parametrization(self, alpha=None, beta=None):
         self.alpha = alpha
         self.beta = beta
         self.param_names = ("alpha", "beta")
         self.params_support = ((eps, np.inf), (eps, np.inf))
-        if (alpha and beta) is not None:
+        if all_not_none(alpha, beta):
             self._update(alpha, beta)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.alpha, scale=self.beta)
         return frozen
 
     def _update(self, alpha, beta):
         self.alpha = np.float64(alpha)
         self.beta = np.float64(beta)
         self.params = (self.alpha, self.beta)
```

### Comparing `preliz-0.2.0/preliz/distributions/discrete.py` & `preliz-0.3.0/preliz/distributions/discrete.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # pylint: disable=too-many-lines
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=attribute-defined-outside-init
 # pylint: disable=invalid-unary-operand-type
+# pylint: disable=invalid-name
 """
 Discrete probability distributions.
 """
 from copy import copy
 import logging
 from math import ceil
 
 import numpy as np
 from scipy import stats
 from scipy.special import logit, expit  # pylint: disable=no-name-in-module
 
 
 from .distributions import Discrete
-from ..internal.optimization import optimize_ml
-from ..internal.distribution_helper import all_not_none
+from ..internal.optimization import optimize_ml, optimize_moments
+from ..internal.distribution_helper import all_not_none, any_not_none
 
 
 _log = logging.getLogger("preliz")
 
 eps = np.finfo(float).eps
 
 
@@ -67,15 +68,15 @@
     def __init__(self, p=None, logit_p=None):
         super().__init__()
         self.dist = copy(stats.bernoulli)
         self.support = (0, 1)
         self._parametrization(p, logit_p)
 
     def _parametrization(self, p=None, logit_p=None):
-        if p is not None and logit_p is not None:
+        if all_not_none(p, logit_p):
             raise ValueError("Incompatible parametrization. Either use p or logit_p.")
 
         self.param_names = "p"
         self.params_support = ((eps, 1),)
 
         if logit_p is not None:
             p = self._from_logit_p(logit_p)
@@ -90,15 +91,15 @@
         return expit(logit_p)
 
     def _to_logit_p(self, p):
         return logit(p)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.p)
         return frozen
 
     def _update(self, p):
         self.p = np.float64(p)
         self.logit_p = self._to_logit_p(p)
 
@@ -169,20 +170,20 @@
     def _parametrization(self, alpha=None, beta=None, n=None):
         self.alpha = alpha
         self.beta = beta
         self.n = n
         self.params = (self.alpha, self.beta, self.n)
         self.param_names = ("alpha", "beta", "n")
         self.params_support = ((eps, np.inf), (eps, np.inf), (eps, np.inf))
-        if (alpha and beta) is not None:
+        if all_not_none(alpha, beta):
             self._update(alpha, beta, n)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(n=self.n, a=self.alpha, b=self.beta)
         return frozen
 
     def _update(self, alpha, beta, n):
         self.alpha = np.float64(alpha)
         self.beta = np.float64(beta)
         self.n = np.int64(n)
@@ -195,15 +196,16 @@
         # For alpha and beta see:
         # https://en.wikipedia.org/wiki/Beta-binomial_distribution#Method_of_moments
         n = mean + sigma * 2
         p = mean / n
         rho = ((sigma**2 / (mean * (1 - p))) - 1) / (n - 1)
         alpha = max(0.5, (p / rho) - p)
         beta = max(0.5, (alpha / p) - alpha)
-        self._update(alpha, beta, n)
+        params = alpha, beta, n
+        optimize_moments(self, mean, sigma, params)
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
 
 
 class Binomial(Discrete):
     R"""
@@ -250,35 +252,36 @@
 
     def _parametrization(self, n=None, p=None):
         self.n = n
         self.p = p
         self.params = (self.n, self.p)
         self.param_names = ("n", "p")
         self.params_support = ((eps, np.inf), (eps, 1 - eps))
-        if (n and p) is not None:
+        if all_not_none(n, p):
             self._update(n, p)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.n, self.p)
         return frozen
 
     def _update(self, n, p):
         self.n = np.int64(n)
         self.p = np.float64(p)
         self.params = (self.n, self.p)
         self.support = (0, self.n)
         self._update_rv_frozen()
 
     def _fit_moments(self, mean, sigma):
         # crude approximation for n and p
         n = mean + sigma * 2
         p = mean / n
-        self._update(n, p)
+        params = n, p
+        optimize_moments(self, mean, sigma, params)
 
     def _fit_mle(self, sample):
         # see https://doi.org/10.1016/j.jspi.2004.02.019 for details
         x_bar = np.mean(sample)
         x_std = np.std(sample)
         x_max = np.max(sample)
         n = ceil(x_max ** (1.5) * x_std / (x_bar**0.5 * (x_max - x_bar) ** 0.5))
@@ -337,15 +340,15 @@
         return cdf
 
     def ppf(self, q):  # pylint: disable=arguments-differ
         cumsum = np.cumsum(self.p)
         return np.searchsorted(cumsum, q)
 
     def _parametrization(self, p=None, logit_p=None):
-        if p is not None and logit_p is not None:
+        if all_not_none(p, logit_p):
             raise ValueError("Incompatible parametrization. Either use p or logit_p.")
 
         self.param_names = "p"
         self.params_support = ((eps, np.inf),)
 
         if logit_p is not None:
             p = self._from_logit_p(logit_p)
@@ -361,15 +364,15 @@
         return expit(logit_p)
 
     def _to_logit_p(self, p):
         return logit(p)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(n=1, p=self.p)
         return frozen
 
     def _update(self, p):
         self.p = np.array(p)
         self.logit_p = self._to_logit_p(p)
 
@@ -432,23 +435,23 @@
         if lower is None:
             self.lower = -np.inf
         if upper is None:
             self.upper = np.inf
         self.support = (self.lower, self.upper)
         self.dist.a = self.lower
         self.dist.b = self.upper
-        if (lower and upper) is not None:
+        if all_not_none(lower, upper):
             self._update(lower, upper)
         else:
             self.lower = lower
             self.upper = upper
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.lower, self.upper + 1)
         return frozen
 
     def _update(self, lower, upper):
         self.lower = np.floor(lower)
         self.upper = np.ceil(upper)
         self.params = (self.lower, self.upper)
@@ -510,15 +513,15 @@
         self.param_names = "p"
         self.params_support = ((eps, 1),)
         if self.p is not None:
             self._update(self.p)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.p)
         return frozen
 
     def _update(self, p):
         self.p = np.float64(p)
         self.params = (self.p,)
         self._update_rv_frozen()
@@ -529,14 +532,92 @@
 
     def _fit_mle(self, sample):
         mean = np.mean(sample)
         p = 1 / mean
         self._update(p)
 
 
+class HyperGeometric(Discrete):
+    R"""
+    Discrete hypergeometric distribution.
+
+    The probability of :math:`x` successes in a sequence of :math:`n` bernoulli
+    trials taken without replacement from a population of :math:`N` objects,
+    containing :math:`k` good (or successful or Type I) objects.
+    The pmf of this distribution is
+
+    .. math:: f(x \mid N, n, k) = \frac{\binom{k}{x}\binom{N-k}{n-x}}{\binom{N}{n}}
+
+    .. plot::
+        :context: close-figs
+
+        import arviz as az
+        from preliz import HyperGeometric
+        az.style.use('arviz-white')
+        N = 50
+        k = 10
+        for n in [20, 25]:
+            HyperGeometric(N, k, n).plot_pdf(support=(1,15))
+
+    ========  =============================
+    Support   :math:`x \in \left[\max(0, n - N + k), \min(k, n)\right]`
+    Mean      :math:`\dfrac{nk}{N}`
+    Variance  :math:`\dfrac{(N-n)nk(N-k)}{(N-1)N^2}`
+    ========  =============================
+
+    Parameters
+    ----------
+    N : int
+        Total size of the population (N > 0)
+    k : int
+        Number of successful individuals in the population (0 <= k <= N)
+    n : int
+        Number of samples drawn from the population (0 <= n <= N)
+    """
+
+    def __init__(self, N=None, k=None, n=None):
+        super().__init__()
+        self.dist = copy(stats.hypergeom)
+        self._parametrization(N, k, n)
+        self.support = (0, np.inf)
+
+    def _parametrization(self, N=None, k=None, n=None):
+        self.N = N
+        self.k = k
+        self.n = n
+        self.param_names = ("N", "k", "n")
+        self.params_support = ((eps, np.inf), (eps, self.N), (eps, self.N))
+        if all_not_none(self.N, self.k, self.n):
+            self._update(N, k, n)
+
+    def _get_frozen(self):
+        frozen = None
+        if all_not_none(self.params):
+            frozen = self.dist(M=self.N, N=self.n, n=self.k)
+        return frozen
+
+    def _update(self, N, k, n):
+        self.N = np.int64(N)
+        self.k = np.int64(k)
+        self.n = np.int64(n)
+        self.params = (self.N, self.k, self.n)
+        self.support = (max(0, n - N + k), min(k, n))
+        self._update_rv_frozen()
+
+    def _fit_moments(self, mean, sigma):
+        n = mean + sigma * 4
+        k = n
+        N = k * n / mean
+        params = N, k, n
+        optimize_moments(self, mean, sigma, params)
+
+    def _fit_mle(self, sample):
+        optimize_ml(self, sample)
+
+
 class NegativeBinomial(Discrete):
     R"""
     Negative binomial distribution.
 
     The negative binomial distribution describes a Poisson random variable
     whose rate parameter is gamma distributed.
     Its pmf, parametrized by the parameters alpha and mu of the gamma distribution, is
@@ -598,45 +679,45 @@
     def __init__(self, mu=None, alpha=None, p=None, n=None):
         super().__init__()
         self.dist = copy(stats.nbinom)
         self.support = (0, np.inf)
         self._parametrization(mu, alpha, p, n)
 
     def _parametrization(self, mu=None, alpha=None, p=None, n=None):
-        if (mu or alpha) is not None and (p or n) is not None:
+        if any_not_none(mu, alpha) and any_not_none(p, n):
             raise ValueError("Incompatible parametrization. Either use mu and alpha, or p and n.")
 
         self.param_names = ("mu", "alpha")
         self.params_support = ((eps, np.inf), (eps, np.inf))
 
-        if (p or n) is not None:
+        if any_not_none(p, n):
             self.p = p
             self.n = n
             self.param_names = ("p", "n")
-            if (p and n) is not None:
+            if all_not_none(p, n):
                 mu, alpha = self._from_p_n(p, n)
 
         self.mu = mu
         self.alpha = alpha
-        if (mu and alpha) is not None:
+        if all_not_none(mu, alpha):
             self._update(mu, alpha)
 
     def _from_p_n(self, p, n):
         alpha = n
         mu = n * (1 / p - 1)
         return mu, alpha
 
     def _to_p_n(self, mu, alpha):
         p = alpha / (mu + alpha)
         n = alpha
         return p, n
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.n, self.p)
         return frozen
 
     def _update(self, mu, alpha):
         self.mu = np.float64(mu)
         self.alpha = np.float64(alpha)
         self.p, self.n = self._to_p_n(self.mu, self.alpha)
@@ -655,15 +736,15 @@
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
 
 
 class Poisson(Discrete):
     R"""
-    Poisson log-likelihood.
+    Poisson distribution.
 
     Often used to model the number of events occurring in a fixed period
     of time when the times at which events occur are independent.
     The pmf of this distribution is
 
     .. math:: f(x \mid \mu) = \frac{e^{-\mu}\mu^x}{x!}
 
@@ -702,20 +783,20 @@
         self._parametrization(mu)
 
     def _parametrization(self, mu=None):
         self.mu = mu
         self.params = (self.mu,)
         self.param_names = ("mu",)
         self.params_support = ((eps, np.inf),)
-        if (mu) is not None:
+        if mu is not None:
             self._update(mu)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.mu)
         return frozen
 
     def _update(self, mu):
         self.mu = np.float64(mu)
         self.params = (self.mu,)
         self._update_rv_frozen()
@@ -724,17 +805,241 @@
         self._update(mean)
 
     def _fit_mle(self, sample):
         mu = np.mean(sample)
         self._update(mu)
 
 
+class ZeroInflatedBinomial(Discrete):
+    R"""
+    Zero-inflated Binomial distribution.
+
+    The pmf of this distribution is
+
+    .. math::
+
+        f(x \mid \psi, n, p) = \left\{ \begin{array}{l}
+            (1-\psi) + \psi (1-p)^{n}, \text{if } x = 0 \\
+            \psi {n \choose x} p^x (1-p)^{n-x}, \text{if } x=1,2,3,\ldots,n
+            \end{array} \right.
+
+    .. plot::
+        :context: close-figs
+
+        import arviz as az
+        from preliz import ZeroInflatedBinomial
+        az.style.use('arviz-white')
+        ns = [10, 20]
+        ps = [0.5, 0.7]
+        psis = [0.7, 0.4]
+        for n, p, psi in zip(ns, ps, psis):
+            ZeroInflatedBinomial(psi, n, p).plot_pdf(support=(0,25))
+
+    ========  ==========================
+    Support   :math:`x \in \mathbb{N}_0`
+    Mean      :math:`\psi n p`
+    Variance  :math:`(1-\psi) n p [1 - p(1 - \psi n)].`
+    ========  ==========================
+
+    Parameters
+    ----------
+    psi : float
+        Expected proportion of Binomial variates (0 < psi < 1)
+    n : int
+        Number of Bernoulli trials (n >= 0).
+    p : float
+        Probability of success in each trial (0 < p < 1).
+    """
+
+    def __init__(self, psi=None, n=None, p=None):
+        super().__init__()
+        self.psi = psi
+        self.n = n
+        self.p = p
+        self.dist = ZIBinomial
+        self.support = (0, np.inf)
+        self._parametrization(psi, n, p)
+
+    def _parametrization(self, psi=None, n=None, p=None):
+        self.psi = psi
+        self.n = n
+        self.p = p
+        self.params = (self.psi, self.n, self.p)
+        self.param_names = ("psi", "n", "p")
+        self.params_support = ((eps, 1 - eps), (eps, np.inf), (eps, 1 - eps))
+        if all_not_none(psi, n, p):
+            self._update(psi, n, p)
+
+    def _get_frozen(self):
+        frozen = None
+        if all_not_none(self.params):
+            frozen = self.dist(self.psi, self.n, self.p)
+        return frozen
+
+    def _update(self, psi, n, p):
+        self.psi = np.float64(psi)
+        self.n = np.int64(n)
+        self.p = np.float64(p)
+        self.params = (self.psi, self.n, self.p)
+        self._update_rv_frozen()
+
+    def _fit_moments(self, mean, sigma):
+        # crude approximation for n and p (same as Binomial)
+        n = mean + sigma * 2
+        p = mean / n
+        psi = 0.9
+        params = psi, n, p
+        optimize_moments(self, mean, sigma, params)
+
+    def _fit_mle(self, sample):
+        optimize_ml(self, sample)
+
+
+class ZeroInflatedNegativeBinomial(Discrete):
+    R"""
+    Zero-Inflated Negative binomial distribution.
+
+    The Zero-inflated version of the Negative Binomial (NB).
+    The NB distribution describes a Poisson random variable
+    whose rate parameter is gamma distributed.
+    The pmf of this distribution is
+
+    .. math::
+
+       f(x \mid \psi, \mu, \alpha) = \left\{
+         \begin{array}{l}
+           (1-\psi) + \psi \left (
+             \frac{\alpha}{\alpha+\mu}
+           \right) ^\alpha, \text{if } x = 0 \\
+           \psi \frac{\Gamma(x+\alpha)}{x! \Gamma(\alpha)} \left (
+             \frac{\alpha}{\mu+\alpha}
+           \right)^\alpha \left(
+             \frac{\mu}{\mu+\alpha}
+           \right)^x, \text{if } x=1,2,3,\ldots
+         \end{array}
+       \right.
+
+    .. plot::
+        :context: close-figs
+
+        import arviz as az
+        from preliz import ZeroInflatedNegativeBinomial
+        az.style.use('arviz-white')
+        psis = [0.7, 0.7]
+        mus = [2, 8]
+        alphas = [2, 4]
+        for psi, mu, alpha in zip(psis, mus, alphas):
+        ZeroInflatedNegativeBinomial(psi, mu=mu, alpha=alpha).plot_pdf(support=(0,25))
+
+    ========  ==========================
+    Support   :math:`x \in \mathbb{N}_0`
+    Mean      :math:`\psi\mu`
+    Var       :math:`\psi\mu +  \left (1 + \frac{\mu}{\alpha} + \frac{1-\psi}{\mu} \right)`
+    ========  ==========================
+
+    The zero inflated negative binomial distribution can be parametrized
+    either in terms of mu and alpha, or in terms of n and p.
+    The link between the parametrizations is given by
+
+    .. math::
+
+        \mu &= \frac{n(1-p)}{p} \\
+        \alpha &= n
+
+    Parameters
+    ----------
+    psi : float
+        Expected proportion of NegativeBinomial variates (0 < psi < 1)
+    mu : float
+        Poisson distribution parameter (mu > 0).
+    alpha : float
+        Gamma distribution parameter (alpha > 0).
+    p : float
+        Alternative probability of success in each trial (0 < p < 1).
+    n : float
+        Alternative number of target success trials (n > 0)
+    """
+
+    def __init__(self, psi=None, mu=None, alpha=None, p=None, n=None):
+        super().__init__()
+        self.psi = psi
+        self.n = n
+        self.p = p
+        self.alpha = alpha
+        self.mu = mu
+        self.dist = ZINegativeBinomial
+        self.support = (0, np.inf)
+        self._parametrization(psi, mu, alpha, p, n)
+
+    def _parametrization(self, psi=None, mu=None, alpha=None, p=None, n=None):
+        if any_not_none(mu, alpha) and any_not_none(p, n):
+            raise ValueError(
+                "Incompatible parametrization. Either use psi, mu and alpha, or psi, p and n."
+            )
+
+        self.psi = psi
+        self.param_names = ("psi", "mu", "alpha")
+        self.params_support = ((eps, 1 - eps), (eps, np.inf), (eps, np.inf))
+
+        if any_not_none(p, n):
+            self.p = p
+            self.n = n
+            self.param_names = ("psi", "p", "n")
+            if all_not_none(p, n):
+                mu, alpha = self._from_p_n(p, n)
+
+        self.mu = mu
+        self.alpha = alpha
+        self.params = (self.psi, self.mu, self.alpha)
+        if all_not_none(mu, alpha):
+            self._update(psi, mu, alpha)
+
+    def _from_p_n(self, p, n):
+        alpha = n
+        mu = n * (1 / p - 1)
+        return mu, alpha
+
+    def _to_p_n(self, mu, alpha):
+        p = alpha / (mu + alpha)
+        n = alpha
+        return p, n
+
+    def _get_frozen(self):
+        frozen = None
+        if all_not_none(self.params):
+            frozen = self.dist(self.psi, self.p, self.n)
+        return frozen
+
+    def _update(self, psi, mu, alpha):
+        self.psi = np.float64(psi)
+        self.mu = np.float64(mu)
+        self.alpha = np.float64(alpha)
+        self.p, self.n = self._to_p_n(self.mu, self.alpha)
+
+        if self.param_names[1] == "mu":
+            self.params = (self.psi, self.mu, self.alpha)
+        elif self.param_names[1] == "p":
+            self.params = (self.psi, self.p, self.n)
+
+        self._update_rv_frozen()
+
+    def _fit_moments(self, mean, sigma):
+        psi = 0.9
+        mu = mean / psi
+        alpha = mean**2 / (sigma**2 - mean)
+        params = psi, mu, alpha
+        optimize_moments(self, mean, sigma, params)
+
+    def _fit_mle(self, sample):
+        optimize_ml(self, sample)
+
+
 class ZeroInflatedPoisson(Discrete):
     R"""
-    Zero-inflated Poisson log-likelihood.
+    Zero-inflated Poisson distribution.
 
     Often used to model the number of events occurring in a fixed period
     of time when the times at which events occur are independent.
     The pmf of this distribution is
 
     .. math::
 
@@ -779,20 +1084,20 @@
 
     def _parametrization(self, psi=None, mu=None):
         self.psi = psi
         self.mu = mu
         self.params = (self.psi, self.mu)
         self.param_names = ("psi", "mu")
         self.params_support = ((eps, 1 - eps), (eps, np.inf))
-        if (psi and mu) is not None:
+        if all_not_none(psi, mu):
             self._update(psi, mu)
 
     def _get_frozen(self):
         frozen = None
-        if all_not_none(self):
+        if all_not_none(self.params):
             frozen = self.dist(self.psi, self.mu)
         return frozen
 
     def _update(self, psi, mu):
         self.psi = np.float64(psi)
         self.mu = np.float64(mu)
         self.params = (self.psi, self.mu)
@@ -803,14 +1108,131 @@
         mean = mean / psi
         self._update(psi, mean)
 
     def _fit_mle(self, sample):
         optimize_ml(self, sample)
 
 
+class ZIBinomial(stats.rv_continuous):
+    def __init__(self, psi=None, n=None, p=None):
+        super().__init__()
+        self.psi = psi
+        self.n = n
+        self.p = p
+
+    def support(self, *args, **kwd):  # pylint: disable=unused-argument
+        return (0, np.inf)
+
+    def cdf(self, x, *args, **kwds):
+        return (1 - self.psi) + self.psi * stats.binom(self.n, self.p, *args, **kwds).cdf(x)
+
+    def pmf(self, x, *args, **kwds):
+        x = np.array(x, ndmin=1)
+        result = np.zeros_like(x, dtype=float)
+        result[x == 0] = (1 - self.psi) + self.psi * (1 - self.p) ** self.n
+        result[x != 0] = self.psi * stats.binom(self.n, self.p, *args, **kwds).pmf(x[x != 0])
+        return result
+
+    def logpmf(self, x, *args, **kwds):
+        result = np.zeros_like(x, dtype=float)
+        result[x == 0] = np.log((1 - self.psi) + self.psi * (1 - self.p) ** self.n)
+        result[x != 0] = np.log(self.psi) + stats.binom(self.n, self.p, *args, **kwds).logpmf(
+            x[x != 0]
+        )
+        return result
+
+    def ppf(self, q, *args, **kwds):
+        return np.round(
+            (1 - self.psi) + self.psi * stats.binom(self.n, self.p, *args, **kwds).ppf(q)
+        )
+
+    def _stats(self, *args, **kwds):  # pylint: disable=unused-argument
+        mean = self.psi * self.n * self.p
+        var = (1 - self.psi) * self.n * self.p * (1 - self.p * (1 - self.psi * self.n))
+        return (mean, var, np.nan, np.nan)
+
+    def entropy(self):  # pylint: disable=arguments-differ
+        binomial_entropy = stats.binom.entropy(self.n, self.p)
+        if self.psi < 0.00001:
+            return 0
+        elif self.psi > 0.99999:
+            return binomial_entropy
+        else:
+            # The variable can be 0 with probability 1-psi or something else with probability psi
+            zero_entropy = -(1 - self.psi) * np.log(1 - self.psi) - self.psi * np.log(self.psi)
+            # The total entropy is the weighted sum of the two entropies
+            return (1 - self.psi) * zero_entropy + self.psi * binomial_entropy
+
+    def rvs(self, size=1):  # pylint: disable=arguments-differ
+        samples = np.zeros(size, dtype=int)
+        non_zero_indices = np.where(np.random.uniform(size=size) < (self.psi))[0]
+        samples[~non_zero_indices] = 0
+        samples[non_zero_indices] = stats.binom.rvs(self.n, self.p, size=len(non_zero_indices))
+        return samples
+
+
+class ZINegativeBinomial(stats.rv_continuous):
+    def __init__(self, psi=None, p=None, n=None):
+        super().__init__()
+        self.psi = psi
+        self.n = n
+        self.p = p
+        self.mu = self.n * (1 / self.p - 1)
+
+    def support(self, *args, **kwd):  # pylint: disable=unused-argument
+        return (0, np.inf)
+
+    def cdf(self, x, *args, **kwds):
+        return (1 - self.psi) + self.psi * stats.nbinom(self.n, self.p, *args, **kwds).cdf(x)
+
+    def pmf(self, x, *args, **kwds):
+        x = np.array(x, ndmin=1)
+        result = np.zeros_like(x, dtype=float)
+        result[x == 0] = (1 - self.psi) + self.psi * (self.n / (self.n + self.mu)) ** self.n
+        result[x != 0] = self.psi * stats.nbinom(self.n, self.p, *args, **kwds).pmf(x[x != 0])
+        return result
+
+    def logpmf(self, x, *args, **kwds):
+        result = np.zeros_like(x, dtype=float)
+        result[x == 0] = np.log((1 - self.psi) + self.psi * (self.n / (self.n + self.mu)) ** self.n)
+        result[x != 0] = np.log(self.psi) + stats.nbinom(self.n, self.p, *args, **kwds).logpmf(
+            x[x != 0]
+        )
+        return result
+
+    def ppf(self, q, *args, **kwds):
+        return np.round(
+            (1 - self.psi) + self.psi * stats.nbinom(self.n, self.p, *args, **kwds).ppf(q)
+        )
+
+    def _stats(self, *args, **kwds):  # pylint: disable=unused-argument
+        mean = self.psi * self.mu
+        var = self.psi * self.mu + (1 + (self.mu / self.n) + ((1 - self.psi) / self.mu))
+        return (mean, var, np.nan, np.nan)
+
+    def entropy(self):  # pylint: disable=arguments-differ
+        negative_binomial_entropy = stats.nbinom.entropy(self.n, self.p)
+        if self.psi < 0.00001:
+            return 0
+        elif self.psi > 0.99999:
+            return negative_binomial_entropy
+        else:
+            # The variable can be 0 with probability 1-psi or something else with probability psi
+            zero_entropy = -(1 - self.psi) * np.log(1 - self.psi) - self.psi * np.log(self.psi)
+            # The total entropy is the weighted sum of the two entropies
+            return (1 - self.psi) * zero_entropy + self.psi * negative_binomial_entropy
+
+    def rvs(self, size=1):  # pylint: disable=arguments-differ
+        samples = np.zeros(size, dtype=int)
+        non_zero_indices = np.where(np.random.uniform(size=size) < (self.psi))[0]
+        samples[~non_zero_indices] = 0
+        samples[non_zero_indices] = stats.nbinom.rvs(self.n, self.p, size=len(non_zero_indices))
+        return samples
+
+
 class ZIPoisson(stats.rv_continuous):
     def __init__(self, psi=None, mu=None):
         super().__init__()
         self.psi = psi
         self.mu = mu
 
     def support(self, *args, **kwd):  # pylint: disable=unused-argument
@@ -843,15 +1265,15 @@
     def entropy(self):  # pylint: disable=arguments-differ
         poisson_entropy = stats.poisson.entropy(self.mu)
         if self.psi < 0.00001:
             return 0
         elif self.psi > 0.99999:
             return poisson_entropy
         else:
-            # The vriable can be 0 with probability 1-psi or something else with probability psi
+            # The variable can be 0 with probability 1-psi or something else with probability psi
             zero_entropy = -(1 - self.psi) * np.log(1 - self.psi) - self.psi * np.log(self.psi)
             # The total entropy is the weighted sum of the two entropies
             return (1 - self.psi) * zero_entropy + self.psi * poisson_entropy
 
     def rvs(self, size=1):  # pylint: disable=arguments-differ
         samples = np.zeros(size, dtype=int)
         non_zero_indices = np.where(np.random.uniform(size=size) < (self.psi))[0]
```

### Comparing `preliz-0.2.0/preliz/distributions/distributions.py` & `preliz-0.3.0/preliz/distributions/distributions.py`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/preliz/internal/distribution_helper.py` & `preliz-0.3.0/preliz/internal/distribution_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,16 +46,26 @@
         poly += k * z**idx
 
     alpha = 1 / (z * (1 + (1 - z) ** 2 * poly))
     beta = 1 / (gamma(1 + 1 / alpha) / (mean))
     return alpha, beta
 
 
-def all_not_none(self):
-    return all(x is not None for x in self.params)
+def all_not_none(*args):
+    for arg in args:
+        if arg is None:
+            return False
+    return True
+
+
+def any_not_none(*args):
+    for arg in args:
+        if arg is not None:
+            return True
+    return False
 
 
 def valid_scalar_params(self, check_frozen=True):
     if not self.is_frozen:
         if check_frozen:
             raise ValueError(
                 "Undefined distribution, "
@@ -90,35 +100,39 @@
     "ChiSquared": {"nu": 5.0},
     "ExGaussian": {"mu": 0.0, "sigma": 1, "nu": 2},
     "Exponential": {"lam": 1},
     "Gamma": {"alpha": 2.0, "beta": 5.0},
     "Gumbel": {"mu": 2.0, "beta": 5.0},
     "HalfCauchy": {"beta": 1.0},
     "HalfNormal": {"sigma": 1.0},
-    "HalfStudent": {"nu": 7.0, "sigma": 1.0},
+    "HalfStudentT": {"nu": 7.0, "sigma": 1.0},
     "InverseGamma": {"alpha": 3.0, "beta": 5.0},
+    "Kumaraswamy": {"a": 2.0, "b": 2.0},
     "Laplace": {"mu": 0.0, "b": 1.0},
     "Logistic": {"mu": 0.0, "s": 1},
     "LogNormal": {"mu": 0.0, "sigma": 0.5},
     "LogitNormal": {"mu": 0.0, "sigma": 0.5},
     "Moyal": {"mu": 0.0, "sigma": 1.0},
     "Normal": {"mu": 0.0, "sigma": 1.0},
     "Pareto": {"alpha": 5, "m": 2.0},
     "Rice": {"nu": 2.0, "sigma": 1.0},
     "SkewNormal": {"mu": 0.0, "sigma": 1, "alpha": 6.0},
-    "Student": {"nu": 7, "mu": 0.0, "sigma": 1},
+    "StudentT": {"nu": 7, "mu": 0.0, "sigma": 1},
     "Triangular": {"lower": -2, "c": 0.0, "upper": 2.0},
     "TruncatedNormal": {"mu": 0.0, "sigma": 1, "lower": -2, "upper": 3.0},
     "Uniform": {"lower": 0.0, "upper": 1.0},
     "VonMises": {"mu": 0.0, "kappa": 1.0},
     "Wald": {"mu": 1, "lam": 3.0},
     "Weibull": {"alpha": 5.0, "beta": 2.0},
     "Bernoulli": {"p": 0.5},
     "BetaBinomial": {"alpha": 2, "beta": 2, "n": 10},
     "Binomial": {"n": 5, "p": 0.5},
     "Categorical": {"p": [0.5, 0.1, 0.4]},
     "DiscreteUniform": {"lower": -2.0, "upper": 2.0},
     "Geometric": {"p": 0.5},
+    "HyperGeometric": {"N": 50, "k": 10, "n": 20},
     "NegativeBinomial": {"mu": 5.0, "alpha": 2.0},
     "Poisson": {"mu": 4.5},
+    "ZeroInflatedBinomial": {"psi": 0.7, "n": 10, "p": 0.5},
+    "ZeroInflatedNegativeBinomial": {"psi": 0.7, "mu": 5, "alpha": 8},
     "ZeroInflatedPoisson": {"psi": 0.8, "mu": 4.5},
 }
```

### Comparing `preliz-0.2.0/preliz/internal/optimization.py` & `preliz-0.3.0/preliz/internal/optimization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Optimization routines and utilities
 """
 from sys import modules
 import numpy as np
 from scipy.optimize import minimize, least_squares
+from .distribution_helper import init_vals as default_vals
 
 
 def optimize_max_ent(dist, lower, upper, mass, none_idx, fixed):
     def prob_bound(params, dist, lower, upper, mass):
         params = get_params(dist, params, none_idx, fixed)
         dist._parametrization(**params)
         if dist.kind == "discrete":
@@ -81,14 +82,40 @@
 
     opt = least_squares(func, x0=init_vals, args=(dist, x_vals, ecdf))
     dist._update(*opt["x"])
     loss = opt["cost"]
     return loss
 
 
+def optimize_moments(dist, mean, sigma, params=None):
+    def func(params, dist, mean, sigma):
+        params = get_params(dist, params, none_idx, fixed)
+        dist._parametrization(**params)
+        loss = abs(dist.rv_frozen.mean() - mean) + abs(dist.rv_frozen.std() - sigma)
+        return loss
+
+    none_idx, fixed = get_fixed_params(dist)
+
+    if params is not None:
+        dist._update(*params)
+    else:
+        dist._update(**default_vals[dist.__class__.__name__])
+
+    init_vals = np.array(dist.params)[none_idx]
+
+    if dist == "HyperGeometric":
+        opt = minimize(func, x0=init_vals, args=(dist, mean, sigma), method="Powell")
+    else:
+        opt = least_squares(func, x0=init_vals, args=(dist, mean, sigma))
+
+    params = get_params(dist, opt["x"], none_idx, fixed)
+    dist._parametrization(**params)
+    return opt
+
+
 def optimize_ml(dist, sample):
     def negll(params, dist, sample):
         dist._update(*params)
         if dist.kind == "continuous":
             neg = -dist.rv_frozen.logpdf(sample).sum()
         else:
             neg = -dist.rv_frozen.logpmf(sample).sum()
```

### Comparing `preliz-0.2.0/preliz/internal/parser.py` & `preliz-0.3.0/preliz/internal/parser.py`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/preliz/internal/plot_helper.py` & `preliz-0.3.0/preliz/internal/plot_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 import traceback
 import sys
 
 from IPython import get_ipython
 from ipywidgets import FloatSlider, IntSlider
 from arviz import plot_kde, plot_ecdf, hdi
+from arviz.stats.density_utils import _kde_linear
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import _pylab_helpers, get_backend
 from matplotlib.ticker import MaxNLocator
 from scipy.interpolate import interp1d, PchipInterpolator
 
 _log = logging.getLogger("preliz")
@@ -351,16 +352,16 @@
                 bins=bins,
                 color="k",
                 ls="--",
                 histtype="step",
             )
         elif kind_plot == "kde":
             for result in results:
-                plot_kde(result, plot_kwargs={"alpha": alpha})
-            plot_kde(np.concatenate(results), plot_kwargs={"color": "k", "ls": "--"})
+                plt.plot(*_kde_linear(result, grid_len=100), "C0", alpha=alpha)
+            plt.plot(*_kde_linear(np.concatenate(results), grid_len=100), "k--")
         elif kind_plot == "ecdf":
             plt.plot(
                 np.sort(results, axis=1).T,
                 np.linspace(0, 1, len(results[0]), endpoint=False),
                 color="C0",
             )
             a = np.concatenate(results)
```

### Comparing `preliz-0.2.0/preliz/predictive/ppa.py` & `preliz-0.3.0/preliz/predictive/ppa.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,15 @@
     init : tuple or PreliZ distribtuion
         Initial distribution. The first shown distributions will be selected to be as close
         as possible to `init`. Available options are, a PreliZ distribution or a 2-tuple with
         the first element representing the mean and the second the standard deviation.
     """
     check_inside_notebook(need_widget=True)
 
-    _log.info(
-        """Enter at your own risk. """
-        """This is highly experimental code and not recommended for regular use."""
-    )
+    _log.info(""""This is an experimental method under development, use with caution.""")
 
     if isinstance(references, (float, int)):
         references = [references]
 
     source, _ = inspect_source(fmodel)
 
     pp_samples, prior_samples, obs_rv = get_prior_pp_samples(fmodel, draws)
```

### Comparing `preliz-0.2.0/preliz/predictive/predictive_sliders.py` & `preliz-0.3.0/preliz/predictive/predictive_sliders.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from ipywidgets import interactive
 from preliz.internal.parser import inspect_source, parse_function_for_pred_sliders
 from preliz.internal.plot_helper import get_sliders, plot_decorator
 
 
-def predictive_sliders(fmodel, samples=50, kind_plot="hist"):
+def predictive_sliders(fmodel, samples=50, kind_plot="kde"):
     """
     Create sliders and plot a set of samples returned by a function relating one or more
     PreliZ distributions.
 
     Use this function to interactively explore how a prior predictive distribution changes when the
     priors are changed.
 
     Parameters
     ----------
     fmodel : callable
         A function with PreliZ distributions. The distributions should call their rvs methods.
     samples : int, optional
         The number of samples to draw from the prior predictive distribution (default is 50).
     kind_plot : str, optional
-        The type of plot to display. Defaults to "hist". Options are "hist" (histogram),
+        The type of plot to display. Defaults to "kde". Options are "hist" (histogram),
         "kde" (kernel density estimate), "ecdf" (empirical cumulative distribution function),
         or None (no plot).
     """
     source, signature = inspect_source(fmodel)
 
     model = parse_function_for_pred_sliders(source, signature)
     sliders = get_sliders(signature, model)
```

### Comparing `preliz-0.2.0/preliz/tests/check_inside_notebook.ipynb` & `preliz-0.3.0/preliz/tests/check_inside_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/preliz/tests/plot_interactive.ipynb` & `preliz-0.3.0/preliz/tests/plot_interactive.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/preliz/tests/predictive_sliders.ipynb` & `preliz-0.3.0/preliz/tests/predictive_sliders.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/preliz/tests/roulette.ipynb` & `preliz-0.3.0/preliz/tests/roulette.ipynb`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/preliz/tests/test_distributions.py` & `preliz-0.3.0/preliz/tests/test_distributions.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,71 +12,81 @@
     ChiSquared,
     Gamma,
     Gumbel,
     ExGaussian,
     Exponential,
     HalfCauchy,
     HalfNormal,
-    HalfStudent,
+    HalfStudentT,
     InverseGamma,
+    Kumaraswamy,
     Laplace,
     Logistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
-    Student,
+    StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
     Bernoulli,
     BetaBinomial,
     Binomial,
     DiscreteUniform,
     Geometric,
     NegativeBinomial,
     Poisson,
+    ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
+    Dirichlet,
+    MvNormal,
 )
 
 
 @pytest.fixture(scope="session")
 def a_few_poissons():
     return Poisson(), Poisson([1.0, 2.0]), Poisson(4.5)
 
 
+@pytest.fixture(scope="session")
+def multivariates():
+    return Dirichlet(), Dirichlet([1.0, 2.0, 1.0]), MvNormal(np.zeros(2), np.eye(2))
+
+
 @pytest.mark.parametrize(
     "distribution, params",
     [
         (AsymmetricLaplace, (1, 0, 1)),
         (Beta, (2, 5)),
         (ChiSquared, (1,)),
         (ExGaussian, (0, 1, 1e-6)),
         (Exponential, (0.5,)),
         (Gamma, (1, 0.5)),
         (Gumbel, (1, 2)),
         (HalfNormal, (1,)),
-        (HalfStudent, (100, 1)),
+        (HalfStudentT, (100, 1)),
         (InverseGamma, (3, 1)),
+        (Kumaraswamy, (5, 2)),
         (Laplace, (0, 1)),
         (Logistic, (1, 2)),
         (LogNormal, (0, 0.5)),
         (LogitNormal, (0, 0.5)),
         (Moyal, (1, 2)),
         (Normal, (0, 1)),
         (Pareto, (5, 1)),
         (Rice, (4, 1)),
         (SkewNormal, (0, 1, 0)),
-        (Student, (100, 0, 1)),
+        (StudentT, (100, 0, 1)),
         (Triangular, (-2, 3, 7)),
         (TruncatedNormal, (0, 1, -np.inf, np.inf)),
         (Uniform, (0, 1)),
         (VonMises, (0, 1000)),
         (Wald, (1, 1)),
         (Weibull, (2, 1)),
         (Bernoulli, (0.8,)),
@@ -99,15 +109,22 @@
 def test_moments(distribution, params):
     dist = distribution(*params)
     dist_ = distribution()
 
     dist_._fit_moments(dist.rv_frozen.mean(), dist.rv_frozen.std())
 
     tol = 5
-    if dist.__class__.__name__ in ["BetaBinomial", "Binomial", "LogitNormal", "Rice", "Student"]:
+    if dist.__class__.__name__ in [
+        "BetaBinomial",
+        "Binomial",
+        "Kumaraswamy",
+        "LogitNormal",
+        "Rice",
+        "StudentT",
+    ]:
         tol = 0
     assert_almost_equal(dist.rv_frozen.mean(), dist_.rv_frozen.mean(), tol)
     assert_almost_equal(dist.rv_frozen.std(), dist_.rv_frozen.std(), tol)
     assert_almost_equal(params, dist_.params, 0)
 
 
 @pytest.mark.parametrize(
@@ -119,42 +136,44 @@
         (ChiSquared, (1,)),
         (ExGaussian, (0, 1, 3)),
         (Exponential, (0.5,)),
         (Gamma, (1, 0.5)),
         (Gumbel, (0, 1)),
         (HalfCauchy, (1,)),
         (HalfNormal, (1,)),
-        (HalfStudent, (100, 1)),
+        (HalfStudentT, (100, 1)),
         (InverseGamma, (3, 0.5)),
+        (Kumaraswamy, (2, 3)),
         (Laplace, (0, 1)),
         (Logistic, (0, 1)),
         (LogNormal, (0, 0.5)),
         (LogitNormal, (0, 0.5)),
         (Moyal, (0, 2)),
         (Normal, (0, 1)),
         (Pareto, (5, 1)),
         (Rice, (1, 2)),
         (SkewNormal, (0, 1, 0)),
         (SkewNormal, (0, 1, -1)),
-        (Student, (4, 0, 1)),
-        (Student, (1000, 0, 1)),
+        (StudentT, (4, 0, 1)),
+        (StudentT, (1000, 0, 1)),
         (Triangular, (-3, 0, 5)),
         (TruncatedNormal, (0, 1, -1, 1)),
         (Uniform, (0, 1)),
         (VonMises, (0, 1)),
         (Wald, (1, 1)),
         (Weibull, (2, 1)),
         (Bernoulli, (0.4,)),
         (BetaBinomial, (2, 2, 10)),
         (Binomial, (2, 0.5)),
         (Binomial, (2, 0.1)),
         (DiscreteUniform, (0, 1)),
         (Geometric, (0.5,)),
         (NegativeBinomial, (8, 4)),
         (Poisson, (4.5,)),
+        (ZeroInflatedNegativeBinomial, (0.7, 8, 4)),
         (
             ZeroInflatedPoisson,
             (
                 0.8,
                 4.5,
             ),
         ),
@@ -168,42 +187,56 @@
 
     if dist.__class__.__name__ == "Pareto":
         tol = 0
     else:
         tol = 1
     assert_almost_equal(dist.rv_frozen.mean(), dist_.rv_frozen.mean(), tol)
     assert_almost_equal(dist.rv_frozen.std(), dist_.rv_frozen.std(), tol)
-    if dist.__class__.__name__ == "Student":
+    if dist.__class__.__name__ == "StudentT":
         assert_almost_equal(params[1:], dist_.params[1:], 0)
     else:
         assert_almost_equal(params, dist_.params, 0)
 
 
 @pytest.mark.parametrize("fmt", (".2f", ".1g"))
 @pytest.mark.parametrize("mass", (0.5, 0.95))
 def test_summary_args(fmt, mass):
     result = Normal(0, 1).summary(fmt, mass)
     assert result.mean == 0
     assert result.std == 1
 
 
-def test_summary_valid(a_few_poissons):
+def test_summary_univariate_valid(a_few_poissons):
     d_0, d_1, d_2 = a_few_poissons
     with pytest.raises(ValueError):
         d_0.summary()
     with pytest.raises(ValueError):
         d_1.summary()
     result = d_2.summary()
     assert result.__class__.__name__ == "Poisson"
     assert result.mean == 4.5
     assert result.std == 2.12
     assert result.lower == 1.0
     assert result.upper == 9.0
 
 
+def test_summary_multivariate_valid(multivariates):
+    d_0, d_1, m_0 = multivariates
+    with pytest.raises(ValueError):
+        d_0.summary()
+    result = d_1.summary()
+    assert result.__class__.__name__ == "Dirichlet"
+    assert_almost_equal(result.mean, [0.25, 0.5, 0.25])
+    assert_almost_equal(result.std, [0.193, 0.223, 0.193], decimal=3)
+    result = m_0.summary()
+    assert result.__class__.__name__ == "MvNormal"
+    assert_almost_equal(result.mean, [0, 0])
+    assert_almost_equal(result.std, [1, 1])
+
+
 def test_eti(a_few_poissons):
     d_0, d_1, d_2 = a_few_poissons
     with pytest.raises(ValueError):
         d_0.eti()
     with pytest.raises(ValueError):
         d_1.eti()
     result = d_2.eti()
```

### Comparing `preliz-0.2.0/preliz/tests/test_helper.py` & `preliz-0.3.0/preliz/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/preliz/tests/test_maxent.py` & `preliz-0.3.0/preliz/tests/test_maxent.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,39 +13,43 @@
     ChiSquared,
     ExGaussian,
     Exponential,
     Gamma,
     Gumbel,
     HalfCauchy,
     HalfNormal,
-    HalfStudent,
+    HalfStudentT,
     InverseGamma,
+    Kumaraswamy,
     Laplace,
     Logistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
-    Student,
+    StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
     # Bernoulli, maxent is not useful for Bernoulli distribution as we only have two states
     BetaBinomial,
     Binomial,
     DiscreteUniform,
     Geometric,
+    HyperGeometric,
     NegativeBinomial,
     Poisson,
+    ZeroInflatedBinomial,
+    ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
 )
 
 
 @pytest.mark.parametrize(
     "dist, lower, upper, mass, support, result",
     [
@@ -75,37 +79,38 @@
         (Exponential(), 0, 4, 0.9, (0, np.inf), (0.575)),
         (Gamma(), 0, 10, 0.7, (0, np.inf), (0.868, 0.103)),
         (Gamma(mu=9), 0, 10, 0.7, (0, np.inf), (2.170)),
         (Gumbel(), 0, 10, 0.9, (-np.inf, np.inf), (3.557, 2.598)),
         (Gumbel(mu=9), 0, 10, 0.9, (-np.inf, np.inf), (0.444)),
         (HalfCauchy(), 0, 10, 0.7, (0, np.inf), (5.095)),
         (HalfNormal(), 0, 10, 0.7, (0, np.inf), (9.648)),
-        (HalfStudent(), 1, 10, 0.7, (0, np.inf), (99.997, 7.697)),
-        (HalfStudent(nu=7), 1, 10, 0.7, (0, np.inf), (2.541)),
+        (HalfStudentT(), 1, 10, 0.7, (0, np.inf), (99.997, 7.697)),
+        (HalfStudentT(nu=7), 1, 10, 0.7, (0, np.inf), (2.541)),
         (InverseGamma(), 0, 1, 0.99, (0, np.inf), (8.889, 3.439)),
+        (Kumaraswamy(), 0.1, 0.6, 0.9, (0, 1), (2.246, 7.426)),
         (Laplace(), -1, 1, 0.9, (-np.inf, np.inf), (0, 0.435)),
         (Laplace(mu=0.5), -1, 1, 0.9, (-np.inf, np.inf), (0.303)),
         (Logistic(), -1, 1, 0.5, (-np.inf, np.inf), (0, 0.91)),
         (LogNormal(), 1, 4, 0.5, (0, np.inf), (1.216, 0.859)),
         (LogNormal(mu=1), 1, 4, 0.5, (0, np.inf), (0.978)),
         (LogitNormal(), 0.3, 0.8, 0.9, (0, 1), (0.226, 0.677)),
         (LogitNormal(mu=0.7), 0.3, 0.8, 0.9, (0, 1), (0.531)),
         (Moyal(), 0, 10, 0.9, (-np.inf, np.inf), (2.935, 1.6)),
         (Moyal(mu=4), 0, 10, 0.9, (-np.inf, np.inf), (1.445)),
         (Normal(), -1, 1, 0.683, (-np.inf, np.inf), (0, 1)),
         (Normal(), 10, 12, 0.99, (-np.inf, np.inf), (11, 0.388)),
         (Normal(mu=0.5), -1, 1, 0.8, (-np.inf, np.inf), (0.581)),
         (Pareto(), 1, 4, 0.9, (1, np.inf), (1.660, 1)),
         (Pareto(m=2), 1, 4, 0.9, (2, np.inf), (3.321)),
-        (Rice(), 0, 4, 0.7, (0, np.inf), (0.027, 2.577)),
+        (Rice(), 0, 4, 0.7, (0, np.inf), (0.0139, 2.577)),
         (Rice(nu=4), 0, 6, 0.9, (0, np.inf), (1.402)),
         (SkewNormal(), -2, 10, 0.9, (-np.inf, np.inf), (3.999, 3.647, 0)),
         (SkewNormal(mu=-1), -2, 10, 0.9, (-np.inf, np.inf), (6.2924, 4.905)),
-        (Student(), -1, 1, 0.683, (-np.inf, np.inf), (99.999, 0, 0.994)),
-        (Student(nu=7), -1, 1, 0.683, (-np.inf, np.inf), (0, 0.928)),
+        (StudentT(), -1, 1, 0.683, (-np.inf, np.inf), (99.999, 0, 0.994)),
+        (StudentT(nu=7), -1, 1, 0.683, (-np.inf, np.inf), (0, 0.928)),
         (
             Triangular(),
             0,
             4,
             0.8,
             (-1.618, 5.618),
             (-1.6180, 1.9999, 5.6180),
@@ -130,31 +135,42 @@
         (Uniform(), -2, 10, 0.9, (-2.666, 10.666), (-2.666, 10.666)),
         (VonMises(), -1, 1, 0.9, (-np.pi, np.pi), (0.0, 3.294)),
         (VonMises(mu=0.5), -1, 1, 0.9, (-np.pi, np.pi), (6.997)),
         (Wald(), 0, 10, 0.9, (0, np.inf), (5.061, 7.937)),
         (Wald(mu=5), 0, 10, 0.9, (0, np.inf), (7.348)),
         (Weibull(), 0, 10, 0.9, (0, np.inf), (1.411, 5.537)),
         (Weibull(alpha=2), 0, 10, 0.9, (0, np.inf), (6.590)),
-        (BetaBinomial(), 2, 8, 0.9, (0, 8), (1.95, 1.344, 8)),
+        (BetaBinomial(), 2, 8, 0.9, (0, 8), (1.951, 1.345, 8)),
         (BetaBinomial(n=10), 2, 6, 0.6, (0, 10), (1.837, 2.181)),
         # results for binomial are close to the correct result, but still off
         (Binomial(), 3, 9, 0.9, (0, 9), (9, 0.490)),
         (Binomial(n=12), 3, 9, 0.9, (0, 12), (0.612)),
         (DiscreteUniform(), -2, 10, 0.9, (-3, 11), (-2, 10)),
         (Geometric(), 1, 4, 0.99, (0, np.inf), (0.6837)),
+        (HyperGeometric(), 2, 14, 0.9, (0, 21), (56, 21, 21)),
         (NegativeBinomial(), 0, 15, 0.9, (0, np.inf), (7.546, 2.041)),
         (NegativeBinomial(p=0.2), 0, 15, 0.9, (0, np.inf), (1.847)),
         (Poisson(), 0, 3, 0.7, (0, np.inf), (2.763)),
+        (ZeroInflatedBinomial(), 1, 10, 0.9, (0, np.inf), (0.901, 10, 0.493)),
+        (ZeroInflatedBinomial(psi=0.7), 1, 10, 0.7, (0, np.inf), (11, 0.5)),
+        (ZeroInflatedNegativeBinomial(), 2, 15, 0.8, (0, np.inf), (1.0, 9.851, 3.416)),
+        (ZeroInflatedNegativeBinomial(psi=0.9), 2, 15, 0.8, (0, np.inf), (8.775, 5.709)),
         (ZeroInflatedPoisson(), 0, 3, 0.7, (0, np.inf), (1, 2.763)),
         (ZeroInflatedPoisson(psi=0.8), 0, 3, 0.7, (0, np.inf), (1.898)),
     ],
 )
 def test_maxent(dist, lower, upper, mass, support, result):
     _, opt = maxent(dist, lower, upper, mass)
 
     assert_almost_equal(dist.support, support, 0.3)
 
-    if (
-        dist.__class__.__name__ != "DiscreteUniform"
-    ):  # optimization fails to converge, but results are reasonable
+    if dist.__class__.__name__ not in [
+        "DiscreteUniform",
+        "HyperGeometric",
+        "ZeroInflatedBinomial",
+    ]:  # optimization fails to converge, but results are reasonable
         assert opt.success
     assert_allclose(opt.x, result, atol=0.001)
+
+
+def test_maxent_plot():
+    maxent(Normal(), plot_kwargs={"support": "restricted", "pointinterval": True})
```

### Comparing `preliz-0.2.0/preliz/tests/test_mle.py` & `preliz-0.3.0/preliz/tests/test_mle.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,39 +12,43 @@
     ChiSquared,
     ExGaussian,
     Exponential,
     Gamma,
     Gumbel,
     HalfCauchy,
     HalfNormal,
-    HalfStudent,
+    HalfStudentT,
     InverseGamma,
+    Kumaraswamy,
     Laplace,
     Logistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
     SkewNormal,
-    Student,
+    StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
     Bernoulli,
     BetaBinomial,
     Binomial,
     DiscreteUniform,
     Geometric,
+    HyperGeometric,
     NegativeBinomial,
     Poisson,
+    ZeroInflatedBinomial,
+    ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
 )
 
 
 @pytest.mark.parametrize(
     "distribution, params",
     [
@@ -55,40 +59,44 @@
         (ChiSquared, (1,)),
         (ExGaussian, (0, 1, 3)),
         (Exponential, (5,)),
         (Gamma, (2, 5)),
         (Gumbel, (0, 2)),
         (HalfCauchy, (1,)),
         (HalfNormal, (1,)),
-        (HalfStudent, (3, 1)),
+        (HalfStudentT, (3, 1)),
         (HalfNormal, (2,)),
         (InverseGamma, (3, 5)),
+        (Kumaraswamy, (2, 3)),
         (Laplace, (0, 2)),
         (Logistic, (0, 1)),
         (LogNormal, (0, 1)),
         (LogitNormal, (0, 0.5)),
         (Moyal, (0, 2)),
         (Normal, (0, 1)),
         (Pareto, (5, 1)),
         (Rice, (0, 2)),
         (SkewNormal, (0, 1, 6)),
-        (Student, (4, 0, 1)),
+        (StudentT, (4, 0, 1)),
         (Triangular, (0, 2, 4)),
         (TruncatedNormal, (0, 1, -1, 1)),
         (Uniform, (2, 5)),
         (VonMises, (1, 2)),
         (Wald, (2, 1)),
         (Weibull, (2, 1)),
         (Bernoulli, (0.5,)),
         (BetaBinomial, (1, 2, 10)),
         (Binomial, (5, 0.5)),
         (DiscreteUniform, (-2, 2)),
         (Geometric, (0.75,)),
+        (HyperGeometric, (50, 20, 10)),
         (NegativeBinomial, (10, 0.5)),
         (Poisson, (4.2,)),
+        (ZeroInflatedBinomial, (0.5, 10, 0.8)),
+        (ZeroInflatedNegativeBinomial, (0.7, 8, 4)),
         (
             ZeroInflatedPoisson,
             (
                 0.8,
                 4.2,
             ),
         ),
```

### Comparing `preliz-0.2.0/preliz/tests/test_quartile.py` & `preliz-0.3.0/preliz/tests/test_quartile.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,37 +11,41 @@
     ChiSquared,
     ExGaussian,
     Exponential,
     Gamma,
     Gumbel,
     HalfCauchy,
     HalfNormal,
-    HalfStudent,
+    HalfStudentT,
     InverseGamma,
+    Kumaraswamy,
     Laplace,
     Logistic,
     LogNormal,
     LogitNormal,
     Moyal,
     Normal,
     Pareto,
     Rice,
-    Student,
+    StudentT,
     Triangular,
     TruncatedNormal,
     Uniform,
     VonMises,
     Wald,
     Weibull,
     # Bernoulli, quartile is not useful for Bernoulli distribution as we only have two states
     BetaBinomial,
     # DiscreteUniform,
     Geometric,
+    HyperGeometric,
     NegativeBinomial,
     Poisson,
+    ZeroInflatedBinomial,
+    ZeroInflatedNegativeBinomial,
     ZeroInflatedPoisson,
 )
 
 
 @pytest.mark.parametrize(
     "distribution, q1, q2, q3, result",
     [
@@ -52,46 +56,52 @@
         (ExGaussian(), 8, 9, 10, (8.996, 1.482, 0.003)),
         (ExGaussian(mu=8.5), 8, 9, 10, (1.401, 0.513)),
         (Exponential(), 0.5, 1, 2.5, (0.611)),
         (Gamma(), 0.5, 1, 2.5, (0.894, 0.523)),
         (Gumbel(), 0.5, 1, 2.5, (0.751, 1.265)),
         (HalfCauchy(), 0.5, 1, 3, (1.105)),
         (HalfNormal(), 0.5, 1, 2, (1.613)),
-        (HalfStudent(), 0.5, 1, 2, (2.393, 1.311)),
+        (HalfStudentT(), 0.5, 1, 2, (2.393, 1.311)),
         (InverseGamma(), 0.2, 0.3, 0.4, (3.881, 1.019)),
+        (Kumaraswamy(), 0.2, 0.3, 0.4, (2.199, 9.598)),
         (Laplace(), -1, 0, 1, (0, 1.442)),
         (Logistic(), -1, 0, 1, (0, 0.910)),
         (LogNormal(), 0.5, 1, 2, (0, 1.027)),
         (LogitNormal(), 0.3, 0.45, 0.6, (-0.212, 0.929)),
         (Moyal(), 0.5, 1, 2, (0.620, 0.567)),
         (Normal(), -1, 0, 1, (0, 1.482)),
         (Pareto(), 0.5, 1, 4, (0.541, 0.289)),
         (Rice(), 2, 4, 6, (0.03566, 3.395)),
         pytest.param(
-            Student(),
+            StudentT(),
             -1,
             0,
             1,
             (84576.43, 0, 1.482),
             marks=pytest.mark.skipif(
                 sys.version_info >= (3, 8), reason="third party implementations details"
             ),
         ),
-        (Student(nu=4), -1, 0, 1, (0, 1.350)),
+        (StudentT(nu=4), -1, 0, 1, (0, 1.350)),
         (Triangular(), 0, 1, 2, (-2.414, 1.0, 4.414)),
         (TruncatedNormal(), -1, 0, 1, (0, 1.482)),
         (Uniform(), -1, 0, 1, (-2, 2)),
         (VonMises(), -1, 0, 1, (0, 0.656)),
         (Wald(), 0.5, 1, 2, (1.698, 1.109)),
         (Weibull(), 0.5, 1, 2, (1.109, 1.456)),
         (BetaBinomial(), 2, 5, 8, (1.59, 4.49, 23)),
         # (DiscreteUniform(), -1, 0, 1, (-5, 5)), # the mass is 0.27 instead of 0.5
         (Geometric(), 2, 4, 6, (0.17)),
+        (HyperGeometric(), 2, 3, 4, (75, 15, 15)),
         (NegativeBinomial(), 3, 5, 10, (7.283, 2.167)),
         (Poisson(), 4, 5, 6, (5.641)),
+        (ZeroInflatedBinomial(), 3, 4, 7, (0.726, 17.001, 0.375)),
+        (ZeroInflatedBinomial(psi=0.7), 2, 4, 6, (16, 0.362)),
+        (ZeroInflatedNegativeBinomial(), 2, 4, 6, (0.87, 5.24, 17.49)),
+        (ZeroInflatedNegativeBinomial(psi=0.9), 2, 4, 6, (5.16, 11.32)),
         (ZeroInflatedPoisson(), 4, 5, 6, (1, 5.641)),
         (ZeroInflatedPoisson(psi=0.8), 2, 4, 6, (5.475)),
     ],
 )
 def test_quartile(distribution, q1, q2, q3, result):
     _, opt = quartile(distribution, q1, q2, q3)
```

### Comparing `preliz-0.2.0/preliz/tests/test_roulette.py` & `preliz-0.3.0/preliz/tests/test_roulette.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     nrows = 10
 
     fig, ax_grid, ax_fit = create_figure((10, 9))
     coll = create_grid(x_min, x_max, nrows, ncols, ax=ax_grid)
     grid = Rectangles(fig, coll, nrows, ncols, ax_grid)
     grid.weights = {0: 2, 1: 6, 2: 10, 3: 10, 4: 7, 5: 3, 6: 1, 7: 1, 8: 1, 9: 1}
     w_repr = "kde"
-    distributions = ["Gamma", "LogNormal", "Student", "BetaScaled", "Normal"]
+    distributions = ["Gamma", "LogNormal", "StudentT", "BetaScaled", "Normal"]
 
     for idx, dist in enumerate(distributions):
         w_distributions = distributions[idx:]
 
         fitted_dist = on_leave_fig(
             fig.canvas, grid, w_distributions, w_repr, x_min, x_max, ncols, ax_fit
         )
```

### Comparing `preliz-0.2.0/preliz/unidimensional/maxent.py` & `preliz-0.3.0/preliz/unidimensional/maxent.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,25 +55,25 @@
         :include-source: true
 
         >>> import arviz as az
         >>> import preliz as pz
         >>> az.style.use('arviz-white')
         >>> pz.maxent(pz.Gamma(), 1, 8, 0.9)
 
-    Calculate the maxent HalfStudent T distribution with 90 % of the mass between 0 and 12
+    Calculate the maxent HalfStudentT T distribution with 90 % of the mass between 0 and 12
     and a value of nu=4:
 
     .. plot::
         :context: close-figs
         :include-source: true
 
         >>> import arviz as az
         >>> import preliz as pz
         >>> az.style.use('arviz-white')
-        >>> pz.maxent(pz.HalfStudent(nu=4), 0, 12, 0.9)
+        >>> pz.maxent(pz.HalfStudentT(nu=4), 0, 12, 0.9)
 
     """
     valid_distribution(distribution)
     if not 0 < mass <= 1:
         raise ValueError("mass should be larger than 0 and smaller or equal to 1")
 
     if upper <= lower:
@@ -112,15 +112,15 @@
         _log.info(
             " The requested mass is %.3g, but the computed one is %.3g",
             mass,
             computed_mass,
         )
 
     if plot:
-        ax = distribution.plot_pdf(plot_kwargs)
+        ax = distribution.plot_pdf(**plot_kwargs)
         if plot_kwargs.get("pointinterval"):
             cid = -4
         else:
             cid = -1
         ax.plot([lower, upper], [0, 0], "o", color=ax.get_lines()[cid].get_c(), alpha=0.5)
     return ax, opt
```

### Comparing `preliz-0.2.0/preliz/unidimensional/mle.py` & `preliz-0.3.0/preliz/unidimensional/mle.py`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/preliz/unidimensional/quartile.py` & `preliz-0.3.0/preliz/unidimensional/quartile.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,25 +54,25 @@
         :include-source: true
 
         >>> import arviz as az
         >>> import preliz as pz
         >>> az.style.use('arviz-white')
         >>> pz.quartile(pz.Gamma(), 3, 6, 8)
 
-    Calculate the HalfStudent T distribution with quartiles 2, 9 and 12
+    Calculate the HalfStudentT T distribution with quartiles 2, 9 and 12
     and a value of nu=7:
 
     .. plot::
         :context: close-figs
         :include-source: true
 
         >>> import arviz as az
         >>> import preliz as pz
         >>> az.style.use('arviz-white')
-        >>> pz.quartile(pz.HalfStudent(nu=7), 2, 9, 12)
+        >>> pz.quartile(pz.HalfStudentT(nu=7), 2, 9, 12)
 
     """
     valid_distribution(distribution)
 
     if plot_kwargs is None:
         plot_kwargs = {}
```

### Comparing `preliz-0.2.0/preliz/unidimensional/roulette.py` & `preliz-0.3.0/preliz/unidimensional/roulette.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,14 +346,14 @@
         options=["pdf", "cdf", "ppf"],
         value="pdf",
         description="",
         disabled=False,
         layout=width_entry_text,
     )
 
-    dist_names = ["Normal", "BetaScaled", "Gamma", "LogNormal", "Student"]
+    dist_names = ["Normal", "BetaScaled", "Gamma", "LogNormal", "StudentT"]
 
     w_distributions = widgets.SelectMultiple(
         options=dist_names, value=dist_names, description="", disabled=False
     )
 
     return w_x_min, w_x_max, w_ncols, w_nrows, w_repr, w_distributions
```

### Comparing `preliz-0.2.0/pyproject.toml` & `preliz-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `preliz-0.2.0/PKG-INFO` & `preliz-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preliz
-Version: 0.2.0
+Version: 0.3.0
 Summary: The place for all your prior elicitation needs.
 Author-email: ArviZ team <arviz.devs@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: Apache Software License
@@ -23,23 +23,22 @@
 Requires-Dist: ipympl
 Project-URL: source, https://github.com/arviz-devs/preliz
 Project-URL: tracker, https://github.com/arviz-devs/preliz/issues
 
 <img src="https://raw.githubusercontent.com/arviz-devs/preliz/main/docs/logos/PreliZ.png#gh-light-mode-only" width=200></img>
 <img src="https://raw.githubusercontent.com/arviz-devs/preliz/main/docs/logos/PreliZ_white.png#gh-dark-mode-only" width=200></img>
 
-Tools to help you pick a prior.
+A tool-box for prior elicitation.
 
 [![PyPi version](https://badge.fury.io/py/preliz.svg)](https://badge.fury.io/py/preliz)
 [![Build Status](https://github.com/arviz-devs/preliz/actions/workflows/test.yml/badge.svg)](https://github.com/arviz-devs/preliz/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/arviz-devs/preliz/branch/master/graph/badge.svg?token=SLJIK2O4C5 )](https://codecov.io/gh/arviz-devs/preliz/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
 
-**This package is very new and many of its features are experimental, or not yet well tested, or subject to change without notice.**
 
 
 ## Documentation
 
 The PreliZ documentation can be found in the [official docs](https://preliz.readthedocs.io/en/latest/).
 
 ## Installation
```

