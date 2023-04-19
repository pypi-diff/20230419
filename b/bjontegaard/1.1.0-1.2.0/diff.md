# Comparing `tmp/bjontegaard-1.1.0.tar.gz` & `tmp/bjontegaard-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bjontegaard-1.1.0.tar", last modified: Thu Sep  8 09:15:52 2022, max compression
+gzip compressed data, was "bjontegaard-1.2.0.tar", last modified: Wed Apr 19 12:31:24 2023, max compression
```

## Comparing `bjontegaard-1.1.0.tar` & `bjontegaard-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 regensky (1928359471) lms-mitarbeiter (1928340378)        0 2022-09-08 09:15:52.219080 bjontegaard-1.1.0/
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     1551 2022-09-06 06:51:33.000000 bjontegaard-1.1.0/LICENSE
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     7200 2022-09-08 09:15:52.219080 bjontegaard-1.1.0/PKG-INFO
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     6296 2022-09-08 09:15:06.000000 bjontegaard-1.1.0/README.md
-drwxr-xr-x   0 regensky (1928359471) lms-mitarbeiter (1928340378)        0 2022-09-08 09:15:52.219080 bjontegaard-1.1.0/bjontegaard/
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     1706 2022-09-08 09:12:58.000000 bjontegaard-1.1.0/bjontegaard/__init__.py
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     4477 2022-09-06 06:51:33.000000 bjontegaard-1.1.0/bjontegaard/bd_akima.py
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     4693 2022-09-06 06:51:33.000000 bjontegaard-1.1.0/bjontegaard/bd_cubic.py
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     4371 2022-09-06 06:51:33.000000 bjontegaard-1.1.0/bjontegaard/bd_piecewise_cubic.py
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     5412 2022-09-06 06:51:33.000000 bjontegaard-1.1.0/bjontegaard/evaluate.py
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     6913 2022-09-08 09:13:58.000000 bjontegaard-1.1.0/bjontegaard/functions.py
-drwxr-xr-x   0 regensky (1928359471) lms-mitarbeiter (1928340378)        0 2022-09-08 09:15:52.219080 bjontegaard-1.1.0/bjontegaard.egg-info/
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     7200 2022-09-08 09:15:52.000000 bjontegaard-1.1.0/bjontegaard.egg-info/PKG-INFO
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)      371 2022-09-08 09:15:52.000000 bjontegaard-1.1.0/bjontegaard.egg-info/SOURCES.txt
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)        1 2022-09-08 09:15:52.000000 bjontegaard-1.1.0/bjontegaard.egg-info/dependency_links.txt
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)       23 2022-09-08 09:15:52.000000 bjontegaard-1.1.0/bjontegaard.egg-info/requires.txt
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)       12 2022-09-08 09:15:52.000000 bjontegaard-1.1.0/bjontegaard.egg-info/top_level.txt
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)      104 2022-09-06 06:51:33.000000 bjontegaard-1.1.0/pyproject.toml
--rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)      969 2022-09-08 09:15:52.219080 bjontegaard-1.1.0/setup.cfg
+drwxr-xr-x   0 regensky (1928359471) lms-mitarbeiter (1928340378)        0 2023-04-19 12:31:24.899068 bjontegaard-1.2.0/
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     1557 2023-04-19 12:29:32.000000 bjontegaard-1.2.0/LICENSE
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     7521 2023-04-19 12:31:24.899068 bjontegaard-1.2.0/PKG-INFO
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     6617 2023-04-19 12:24:58.000000 bjontegaard-1.2.0/README.md
+drwxr-xr-x   0 regensky (1928359471) lms-mitarbeiter (1928340378)        0 2023-04-19 12:31:24.898069 bjontegaard-1.2.0/bjontegaard/
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     1721 2023-04-19 12:29:23.000000 bjontegaard-1.2.0/bjontegaard/__init__.py
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     5068 2023-04-19 12:29:23.000000 bjontegaard-1.2.0/bjontegaard/bd_akima.py
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     4701 2023-04-19 11:21:18.000000 bjontegaard-1.2.0/bjontegaard/bd_cubic.py
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     4376 2023-04-19 12:29:23.000000 bjontegaard-1.2.0/bjontegaard/bd_piecewise_cubic.py
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     5391 2023-04-19 12:29:23.000000 bjontegaard-1.2.0/bjontegaard/evaluate.py
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)    11751 2023-04-19 12:29:23.000000 bjontegaard-1.2.0/bjontegaard/functions.py
+drwxr-xr-x   0 regensky (1928359471) lms-mitarbeiter (1928340378)        0 2023-04-19 12:31:24.899068 bjontegaard-1.2.0/bjontegaard.egg-info/
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)     7521 2023-04-19 12:31:24.000000 bjontegaard-1.2.0/bjontegaard.egg-info/PKG-INFO
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)      371 2023-04-19 12:31:24.000000 bjontegaard-1.2.0/bjontegaard.egg-info/SOURCES.txt
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)        1 2023-04-19 12:31:24.000000 bjontegaard-1.2.0/bjontegaard.egg-info/dependency_links.txt
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)       23 2023-04-19 12:31:24.000000 bjontegaard-1.2.0/bjontegaard.egg-info/requires.txt
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)       12 2023-04-19 12:31:24.000000 bjontegaard-1.2.0/bjontegaard.egg-info/top_level.txt
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)      104 2022-09-05 11:35:37.000000 bjontegaard-1.2.0/pyproject.toml
+-rw-r--r--   0 regensky (1928359471) lms-mitarbeiter (1928340378)      969 2023-04-19 12:31:24.899068 bjontegaard-1.2.0/setup.cfg
```

### Comparing `bjontegaard-1.1.0/LICENSE` & `bjontegaard-1.2.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Friedrich-Alexander-Universität Erlangen-Nürnberg.
+Copyright (c) 2022-2023, Friedrich-Alexander-Universität Erlangen-Nürnberg.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
@@ -22,8 +22,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `bjontegaard-1.1.0/PKG-INFO` & `bjontegaard-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bjontegaard
-Version: 1.1.0
+Version: 1.2.0
 Summary: Calculate the Bjonteegard-Delta metric with different interpolation methods
 Home-page: https://github.com/FAU-LMS/bjontegaard
 Author: bjontegaard contributors
 Author-email: christian.herglotz@fau.de
 Project-URL: Bug Tracker, https://github.com/FAU-LMS/bjontegaard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -76,14 +76,20 @@
 * `'cubic'`: Cubic spline interpolation
 * `'pchip'`: Piecewise cubic hermite interpolation (used in standardizations [[2]](http://phenix.int-evry.fr/jct/doc_end_user/documents/12_Geneva/wg11/JCTVC-L1100-v1.zip), [[3]]((https://jvet-experts.org/doc_end_user/documents/20_Teleconference/wg11/JVET-T2010-v2.zip)))
 * `'akima'`: Akima interpolation [[4]](https://doi.org/10.48550/arXiv.2202.12565)
 
 If `require_matching_points=True` (default), the number of rate-distortion points for anchor and test must match.
 If `interpolators=True` is given, the functions additionally return the internal interpolation objects that can be used to check the behaviour of the value interpolation.
 
+## Relative curve difference plots (RCD-plots)
+
+For in-depth evaluation of codec comparison results, we recommend to take relative curve difference plots (RCD-plots) into account.
+They can be created using:
+* `plot_rcd(rate_anchor, dist_anchor, rate_test, dist_test, method, require_matching_points=True, samples=1000)`
+
 ## Comparison behind the scenes
 The function `compare_methods` generates a plot that compares the internal interpolation behaviour of the three variants.
 The parameters `rate_label`, `distortion_label`, and `figure_label` control the figure and axis labels of the plot.
 If `filepath` is given, the final figure is saved to this file.
 
 ```python
 import bjontegaard as bd
```

### Comparing `bjontegaard-1.1.0/README.md` & `bjontegaard-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 * `'cubic'`: Cubic spline interpolation
 * `'pchip'`: Piecewise cubic hermite interpolation (used in standardizations [[2]](http://phenix.int-evry.fr/jct/doc_end_user/documents/12_Geneva/wg11/JCTVC-L1100-v1.zip), [[3]]((https://jvet-experts.org/doc_end_user/documents/20_Teleconference/wg11/JVET-T2010-v2.zip)))
 * `'akima'`: Akima interpolation [[4]](https://doi.org/10.48550/arXiv.2202.12565)
 
 If `require_matching_points=True` (default), the number of rate-distortion points for anchor and test must match.
 If `interpolators=True` is given, the functions additionally return the internal interpolation objects that can be used to check the behaviour of the value interpolation.
 
+## Relative curve difference plots (RCD-plots)
+
+For in-depth evaluation of codec comparison results, we recommend to take relative curve difference plots (RCD-plots) into account.
+They can be created using:
+* `plot_rcd(rate_anchor, dist_anchor, rate_test, dist_test, method, require_matching_points=True, samples=1000)`
+
 ## Comparison behind the scenes
 The function `compare_methods` generates a plot that compares the internal interpolation behaviour of the three variants.
 The parameters `rate_label`, `distortion_label`, and `figure_label` control the figure and axis labels of the plot.
 If `filepath` is given, the final figure is saved to this file.
 
 ```python
 import bjontegaard as bd
```

### Comparing `bjontegaard-1.1.0/bjontegaard/__init__.py` & `bjontegaard-1.2.0/bjontegaard/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 3-Clause License
 #
-# Copyright (c) 2022, Friedrich-Alexander-Universität Erlangen-Nürnberg.
+# Copyright (c) 2022-2023, Friedrich-Alexander-Universität Erlangen-Nürnberg.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -24,11 +24,11 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
-from .functions import bd_rate, bd_psnr
+from .functions import bd_rate, bd_psnr, plot_rcd
 from .evaluate import compare_methods
```

### Comparing `bjontegaard-1.1.0/bjontegaard/bd_akima.py` & `bjontegaard-1.2.0/bjontegaard/bd_akima.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 3-Clause License
 #
-# Copyright (c) 2022, Friedrich-Alexander-Universität Erlangen-Nürnberg.
+# Copyright (c) 2022-2023, Friedrich-Alexander-Universität Erlangen-Nürnberg.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -43,16 +43,23 @@
 
     if rateB[-1] < rateB[0]:
         assert (distB[-1] < distB[0])
         rateB = np.flipud(rateB)
         distB = np.flipud(distB)
 
     # computes interpolating polynomial via the Akima Interpolation method
-    interp1 = scipy.interpolate.Akima1DInterpolator(distA, np.log10(rateA))
-    interp2 = scipy.interpolate.Akima1DInterpolator(distB, np.log10(rateB))
+    # (fallback to linear for less than 3 supporting points)
+    if len(rateA) > 2:
+        interp1 = scipy.interpolate.Akima1DInterpolator(distA, np.log10(rateA))
+    else:
+        interp1 = scipy.interpolate.make_interp_spline(distA, np.log10(rateA), k=1)
+    if len(rateB) > 2:
+        interp2 = scipy.interpolate.Akima1DInterpolator(distB, np.log10(rateB))
+    else:
+        interp2 = scipy.interpolate.make_interp_spline(distB, np.log10(rateB), k=1)
 
     # compute the integration interval
     min_dist = max(distA.min(), distB.min())
     max_dist = min(distA.max(), distB.max())
 
     # if min_dist is bigger than max_, the curves of both sequences don't overlap - BD cannot be calculated!
     if min_dist > max_dist:
@@ -88,16 +95,23 @@
         rateB = np.flipud(rateB)
         distB = np.flipud(distB)
 
     rateA = np.log10(rateA)
     rateB = np.log10(rateB)
 
     # computes interpolating polynomial via the Akima Interpolation method
-    interp1 = scipy.interpolate.Akima1DInterpolator(rateA, distA)
-    interp2 = scipy.interpolate.Akima1DInterpolator(rateB, distB)
+    # (fallback to linear for less than 3 supporting points)
+    if len(rateA) > 2:
+        interp1 = scipy.interpolate.Akima1DInterpolator(rateA, distA)
+    else:
+        interp1 = scipy.interpolate.make_interp_spline(rateA, distA, k=1)
+    if len(rateB) > 2:
+        interp2 = scipy.interpolate.Akima1DInterpolator(rateB, distB)
+    else:
+        interp2 = scipy.interpolate.make_interp_spline(rateB, distB, k=1)
 
     # compute the integration interval
     min_rate = max(rateA.min(), rateB.min())
     max_rate = min(rateA.max(), rateB.max())
 
     # if min_ is bigger than max_, the curves of both sequences don't overlap - BD cannot be calculated!
     if min_rate > max_rate:
```

### Comparing `bjontegaard-1.1.0/bjontegaard/bd_cubic.py` & `bjontegaard-1.2.0/bjontegaard/bd_cubic.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,16 @@
     # numpy seems to do tricks with its exports.
     # pylint: disable=no-member
     # map() is recommended against.
     # pylint: disable=bad-builtin
 
     # log_rate1 = map(math.log, rate1)
     # log_rate2 = map(math.log, rate1)
-    log_rate1 = numpy.log(rate1)
-    log_rate2 = numpy.log(rate2)
+    log_rate1 = numpy.log10(rate1)
+    log_rate2 = numpy.log10(rate2)
 
     # Best cubic poly fit for graph represented by log_ratex, psrn_x.
     poly1 = numpy.polyfit(log_rate1, dist1, 3)
     poly2 = numpy.polyfit(log_rate2, dist2, 3)
 
     # Integration interval.
     min_int = max([min(log_rate1), min(log_rate2)])
@@ -97,16 +97,16 @@
     # numpy plays games with its exported functions.
     # pylint: disable=no-member
     # pylint: disable=too-many-locals
     # pylint: disable=bad-builtin
 
     # log_rate1 = map(math.log, rate1)
     # log_rate2 = map(math.log, rate1)
-    log_rate1 = numpy.log(rate1)
-    log_rate2 = numpy.log(rate2)
+    log_rate1 = numpy.log10(rate1)
+    log_rate2 = numpy.log10(rate2)
 
     # Best cubic poly fit for graph represented by log_ratex, psrn_x.
     poly1 = numpy.polyfit(dist1, log_rate1, 3)
     poly2 = numpy.polyfit(dist2, log_rate2, 3)
 
     # Integration interval.
     min_int = max([min(dist1), min(dist2)])
```

### Comparing `bjontegaard-1.1.0/bjontegaard/bd_piecewise_cubic.py` & `bjontegaard-1.2.0/bjontegaard/bd_piecewise_cubic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 3-Clause License
 #
-# Copyright (c) 2022, Friedrich-Alexander-Universität Erlangen-Nürnberg.
+# Copyright (c) 2022-2023, Friedrich-Alexander-Universität Erlangen-Nürnberg.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
```

### Comparing `bjontegaard-1.1.0/bjontegaard/evaluate.py` & `bjontegaard-1.2.0/bjontegaard/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 3-Clause License
 #
-# Copyright (c) 2022, Friedrich-Alexander-Universität Erlangen-Nürnberg.
+# Copyright (c) 2022-2023, Friedrich-Alexander-Universität Erlangen-Nürnberg.
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -66,40 +66,40 @@
     dist_test = np.asarray(dist_test)
 
     dists1 = np.linspace(dist_anchor.min(), dist_anchor.max(), num=10, endpoint=True)
     dists2 = np.linspace(dist_test.min(), dist_test.max(), num=10, endpoint=True)
 
     # Plot interpolation curves for each method
     methods = {
-        'cubic': ('Cubic interpolation (non-piece-wise)', np.log),
-        'pchip': ('Piece-wise cubic interpolation', np.log10),
-        'akima': ('BD Calculation with Akima Interpolation', np.log10)
+        'cubic': 'Cubic interpolation (non-piece-wise)',
+        'pchip': 'Piece-wise cubic interpolation',
+        'akima': 'BD Calculation with Akima Interpolation'
     }
     fig, axs = plt.subplots(2, 2, figsize=(16, 10))
     fig.suptitle(figure_label)
-    for ax, (method, (label, log)) in zip(axs.flat, methods.items()):
+    for ax, (method, label) in zip(axs.flat, methods.items()):
         bd_rate, interp1, interp2 = bd.bd_rate(rate_anchor, dist_anchor, rate_test, dist_test,
                                                method=method,
                                                require_matching_points=require_matching_points,
                                                interpolators=True)
         bd_psnr = bd.bd_psnr(rate_anchor, dist_anchor, rate_test, dist_test, method=method, require_matching_points=require_matching_points)
 
         # Plot rate1 and dist1
         rates1 = interp1(dists1)
-        ax.plot(log(rate_anchor), dist_anchor, '-o', color='tab:blue', label='anchor')
+        ax.plot(np.log10(rate_anchor), dist_anchor, '-o', color='tab:blue', label='anchor')
         ax.plot(rates1, dists1, '--', color='tab:blue')
 
         # Plot rate2 and dist1
         rates2 = interp2(dists2)
-        ax.plot(log(rate_test), dist_test, '-o', color='tab:orange', label='test')
+        ax.plot(np.log10(rate_test), dist_test, '-o', color='tab:orange', label='test')
         ax.plot(rates2, dists2, '--', color='tab:orange')
 
         # Set axis properties
         ax.set_title(label)
-        ax.set_xlabel('{}({})'.format(log.__name__, rate_label))
+        ax.set_xlabel('{}({})'.format(np.log10.__name__, rate_label))
         ax.set_ylabel(distortion_label)
         ax.grid()
         ax.legend()
 
         # Add bd metrics table
         cell_text = [
             ["{:.10f} %".format(bd_rate)],
```

### Comparing `bjontegaard-1.1.0/bjontegaard.egg-info/PKG-INFO` & `bjontegaard-1.2.0/bjontegaard.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bjontegaard
-Version: 1.1.0
+Version: 1.2.0
 Summary: Calculate the Bjonteegard-Delta metric with different interpolation methods
 Home-page: https://github.com/FAU-LMS/bjontegaard
 Author: bjontegaard contributors
 Author-email: christian.herglotz@fau.de
 Project-URL: Bug Tracker, https://github.com/FAU-LMS/bjontegaard/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -76,14 +76,20 @@
 * `'cubic'`: Cubic spline interpolation
 * `'pchip'`: Piecewise cubic hermite interpolation (used in standardizations [[2]](http://phenix.int-evry.fr/jct/doc_end_user/documents/12_Geneva/wg11/JCTVC-L1100-v1.zip), [[3]]((https://jvet-experts.org/doc_end_user/documents/20_Teleconference/wg11/JVET-T2010-v2.zip)))
 * `'akima'`: Akima interpolation [[4]](https://doi.org/10.48550/arXiv.2202.12565)
 
 If `require_matching_points=True` (default), the number of rate-distortion points for anchor and test must match.
 If `interpolators=True` is given, the functions additionally return the internal interpolation objects that can be used to check the behaviour of the value interpolation.
 
+## Relative curve difference plots (RCD-plots)
+
+For in-depth evaluation of codec comparison results, we recommend to take relative curve difference plots (RCD-plots) into account.
+They can be created using:
+* `plot_rcd(rate_anchor, dist_anchor, rate_test, dist_test, method, require_matching_points=True, samples=1000)`
+
 ## Comparison behind the scenes
 The function `compare_methods` generates a plot that compares the internal interpolation behaviour of the three variants.
 The parameters `rate_label`, `distortion_label`, and `figure_label` control the figure and axis labels of the plot.
 If `filepath` is given, the final figure is saved to this file.
 
 ```python
 import bjontegaard as bd
```

### Comparing `bjontegaard-1.1.0/setup.cfg` & `bjontegaard-1.2.0/setup.cfg`

 * *Files identical despite different names*

