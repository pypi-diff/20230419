# Comparing `tmp/mdfs-1.5.0.tar.gz` & `tmp/mdfs-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdfs-1.5.0.tar", last modified: Mon Mar 13 15:19:59 2023, max compression
+gzip compressed data, was "mdfs-1.5.2.tar", last modified: Wed Apr 19 08:12:30 2023, max compression
```

## Comparing `mdfs-1.5.0.tar` & `mdfs-1.5.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-13 15:19:59.488052 mdfs-1.5.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-01-23 17:39:31.000000 mdfs-1.5.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3865 2023-03-13 15:19:59.488052 mdfs-1.5.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2970 2023-01-31 09:42:06.000000 mdfs-1.5.0/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-13 15:19:59.480052 mdfs-1.5.0/mdfs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      269 2023-01-30 19:42:40.000000 mdfs-1.5.0/mdfs/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1075 2023-01-29 19:26:29.000000 mdfs-1.5.0/mdfs/c.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5454 2023-01-30 19:42:30.000000 mdfs-1.5.0/mdfs/compute_max_ig.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-01-30 19:32:21.000000 mdfs-1.5.0/mdfs/compute_tuples.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2122 2023-01-29 19:18:57.000000 mdfs-1.5.0/mdfs/fit_p_value.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      133 2023-01-29 18:33:33.000000 mdfs-1.5.0/mdfs/internal_common.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2440 2023-01-29 18:11:44.000000 mdfs-1.5.0/mdfs/run.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2790 2023-03-06 17:09:18.000000 mdfs-1.5.0/mdfs/utils.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-13 15:19:59.484052 mdfs-1.5.0/mdfs.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3865 2023-03-13 15:19:59.000000 mdfs-1.5.0/mdfs.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-03-13 15:19:59.000000 mdfs-1.5.0/mdfs.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-03-13 15:19:59.000000 mdfs-1.5.0/mdfs.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2023-03-13 15:19:59.000000 mdfs-1.5.0/mdfs.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-03-13 15:19:59.000000 mdfs-1.5.0/mdfs.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1054 2023-03-13 15:18:18.000000 mdfs-1.5.0/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-03-13 15:19:59.488052 mdfs-1.5.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-01-30 17:59:12.000000 mdfs-1.5.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-13 15:19:59.476052 mdfs-1.5.0/shared/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-13 15:19:59.484052 mdfs-1.5.0/shared/interface/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      111 2023-01-24 11:42:53.000000 mdfs-1.5.0/shared/interface/common.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9675 2023-03-13 13:59:43.000000 mdfs-1.5.0/shared/interface/compute_max_ig.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10715 2023-03-13 14:04:04.000000 mdfs-1.5.0/shared/interface/compute_tuples.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1655 2023-01-30 18:42:16.000000 mdfs-1.5.0/shared/interface/discretize.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10562 2023-01-30 18:43:57.000000 mdfs-1.5.0/shared/interface/fit_p_value.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-01-24 11:43:51.000000 mdfs-1.5.0/shared/interface/free_helpers.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3100 2023-01-30 18:48:06.000000 mdfs-1.5.0/shared/interface/gen_contrast_variables.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      716 2023-01-30 17:50:58.000000 mdfs-1.5.0/shared/interface/get_suggested_range.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      189 2023-03-13 13:55:26.000000 mdfs-1.5.0/shared/interface/get_suggested_range.h
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-13 15:19:59.476052 mdfs-1.5.0/shared/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-13 15:19:59.488052 mdfs-1.5.0/shared/src/cpu/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6610 2023-01-28 22:07:04.000000 mdfs-1.5.0/shared/src/cpu/common.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4024 2023-01-28 22:07:04.000000 mdfs-1.5.0/shared/src/cpu/common.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1227 2023-01-28 22:04:34.000000 mdfs-1.5.0/shared/src/cpu/dataset.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-01-28 22:04:34.000000 mdfs-1.5.0/shared/src/cpu/discretize.cpp
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-01-28 22:04:34.000000 mdfs-1.5.0/shared/src/cpu/discretize.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      852 2021-05-23 14:53:14.000000 mdfs-1.5.0/shared/src/cpu/entropy.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19647 2023-01-31 12:59:09.000000 mdfs-1.5.0/shared/src/cpu/mdfs.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2037 2022-05-30 19:43:52.000000 mdfs-1.5.0/shared/src/cpu/mdfs_count_counters.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6574 2023-01-28 21:53:38.000000 mdfs-1.5.0/shared/src/cpu/mdfs_cpu_kernel.h
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      480 2020-09-23 14:21:13.000000 mdfs-1.5.0/shared/src/cpu/mdfs_reduce_counters.h
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-19 08:12:30.463573 mdfs-1.5.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-01-23 17:39:31.000000 mdfs-1.5.2/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3873 2023-04-19 08:12:30.463573 mdfs-1.5.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2974 2023-03-13 15:25:39.000000 mdfs-1.5.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-19 08:12:30.455572 mdfs-1.5.2/mdfs/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      269 2023-01-30 19:42:40.000000 mdfs-1.5.2/mdfs/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1075 2023-01-29 19:26:29.000000 mdfs-1.5.2/mdfs/c.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5454 2023-01-30 19:42:30.000000 mdfs-1.5.2/mdfs/compute_max_ig.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6535 2023-01-30 19:32:21.000000 mdfs-1.5.2/mdfs/compute_tuples.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2122 2023-01-29 19:18:57.000000 mdfs-1.5.2/mdfs/fit_p_value.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      133 2023-01-29 18:33:33.000000 mdfs-1.5.2/mdfs/internal_common.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2440 2023-01-29 18:11:44.000000 mdfs-1.5.2/mdfs/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2790 2023-03-06 17:09:18.000000 mdfs-1.5.2/mdfs/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-19 08:12:30.455572 mdfs-1.5.2/mdfs.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3873 2023-04-19 08:12:30.000000 mdfs-1.5.2/mdfs.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      936 2023-04-19 08:12:30.000000 mdfs-1.5.2/mdfs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-19 08:12:30.000000 mdfs-1.5.2/mdfs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2023-04-19 08:12:30.000000 mdfs-1.5.2/mdfs.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-04-19 08:12:30.000000 mdfs-1.5.2/mdfs.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1058 2023-04-19 08:04:21.000000 mdfs-1.5.2/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-19 08:12:30.463573 mdfs-1.5.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1730 2023-01-30 17:59:12.000000 mdfs-1.5.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-19 08:12:30.451573 mdfs-1.5.2/shared/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-19 08:12:30.459573 mdfs-1.5.2/shared/interface/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      111 2023-01-24 11:42:53.000000 mdfs-1.5.2/shared/interface/common.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9675 2023-03-13 13:59:43.000000 mdfs-1.5.2/shared/interface/compute_max_ig.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10715 2023-03-13 14:04:04.000000 mdfs-1.5.2/shared/interface/compute_tuples.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1655 2023-01-30 18:42:16.000000 mdfs-1.5.2/shared/interface/discretize.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10562 2023-01-30 18:43:57.000000 mdfs-1.5.2/shared/interface/fit_p_value.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      328 2023-01-24 11:43:51.000000 mdfs-1.5.2/shared/interface/free_helpers.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3100 2023-01-30 18:48:06.000000 mdfs-1.5.2/shared/interface/gen_contrast_variables.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      738 2023-04-19 08:04:03.000000 mdfs-1.5.2/shared/interface/get_suggested_range.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      189 2023-03-13 13:55:26.000000 mdfs-1.5.2/shared/interface/get_suggested_range.h
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-19 08:12:30.451573 mdfs-1.5.2/shared/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-19 08:12:30.463573 mdfs-1.5.2/shared/src/cpu/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6610 2023-01-28 22:07:04.000000 mdfs-1.5.2/shared/src/cpu/common.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4024 2023-01-28 22:07:04.000000 mdfs-1.5.2/shared/src/cpu/common.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1227 2023-01-28 22:04:34.000000 mdfs-1.5.2/shared/src/cpu/dataset.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2243 2023-01-28 22:04:34.000000 mdfs-1.5.2/shared/src/cpu/discretize.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      407 2023-01-28 22:04:34.000000 mdfs-1.5.2/shared/src/cpu/discretize.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      852 2021-05-23 14:53:14.000000 mdfs-1.5.2/shared/src/cpu/entropy.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19647 2023-01-31 12:59:09.000000 mdfs-1.5.2/shared/src/cpu/mdfs.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2037 2022-05-30 19:43:52.000000 mdfs-1.5.2/shared/src/cpu/mdfs_count_counters.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6574 2023-01-28 21:53:38.000000 mdfs-1.5.2/shared/src/cpu/mdfs_cpu_kernel.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      480 2020-09-23 14:21:13.000000 mdfs-1.5.2/shared/src/cpu/mdfs_reduce_counters.h
```

### Comparing `mdfs-1.5.0/PKG-INFO` & `mdfs-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mdfs
-Version: 1.5.0
+Version: 1.5.2
 Summary: A library for MultiDimensional Feature Selection (MDFS)
 Author-email: Radosław Piliszek <r.piliszek@uwb.edu.pl>
 Maintainer-email: Radosław Piliszek <r.piliszek@uwb.edu.pl>
 Project-URL: homepage, https://www.mdfs.it/
-Project-URL: changelog, https://mdfs.it/CHANGELOG
+Project-URL: changelog, https://www.mdfs.it/CHANGELOG
 Keywords: feature selection,classification,machine learning,information theory
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
@@ -95,8 +95,8 @@
 data elsewhere as necessary.
 This quirk might be lifted in the future.
 
 
 [mdfs-web]: https://www.mdfs.it/
 [mdfs-r]: https://cran.r-project.org/package=MDFS
 [gpl-3]: https://www.gnu.org/licenses/gpl-3.0.en.html
-[changelog]: https://mdfs.it/CHANGELOG
+[changelog]: https://www.mdfs.it/CHANGELOG
```

### Comparing `mdfs-1.5.0/README.md` & `mdfs-1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -76,8 +76,8 @@
 data elsewhere as necessary.
 This quirk might be lifted in the future.
 
 
 [mdfs-web]: https://www.mdfs.it/
 [mdfs-r]: https://cran.r-project.org/package=MDFS
 [gpl-3]: https://www.gnu.org/licenses/gpl-3.0.en.html
-[changelog]: https://mdfs.it/CHANGELOG
+[changelog]: https://www.mdfs.it/CHANGELOG
```

### Comparing `mdfs-1.5.0/mdfs/c.py` & `mdfs-1.5.2/mdfs/c.py`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/mdfs/compute_max_ig.py` & `mdfs-1.5.2/mdfs/compute_max_ig.py`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/mdfs/compute_tuples.py` & `mdfs-1.5.2/mdfs/compute_tuples.py`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/mdfs/fit_p_value.py` & `mdfs-1.5.2/mdfs/fit_p_value.py`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/mdfs/run.py` & `mdfs-1.5.2/mdfs/run.py`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/mdfs/utils.py` & `mdfs-1.5.2/mdfs/utils.py`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/mdfs.egg-info/PKG-INFO` & `mdfs-1.5.2/mdfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: mdfs
-Version: 1.5.0
+Version: 1.5.2
 Summary: A library for MultiDimensional Feature Selection (MDFS)
 Author-email: Radosław Piliszek <r.piliszek@uwb.edu.pl>
 Maintainer-email: Radosław Piliszek <r.piliszek@uwb.edu.pl>
 Project-URL: homepage, https://www.mdfs.it/
-Project-URL: changelog, https://mdfs.it/CHANGELOG
+Project-URL: changelog, https://www.mdfs.it/CHANGELOG
 Keywords: feature selection,classification,machine learning,information theory
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
@@ -95,8 +95,8 @@
 data elsewhere as necessary.
 This quirk might be lifted in the future.
 
 
 [mdfs-web]: https://www.mdfs.it/
 [mdfs-r]: https://cran.r-project.org/package=MDFS
 [gpl-3]: https://www.gnu.org/licenses/gpl-3.0.en.html
-[changelog]: https://mdfs.it/CHANGELOG
+[changelog]: https://www.mdfs.it/CHANGELOG
```

### Comparing `mdfs-1.5.0/mdfs.egg-info/SOURCES.txt` & `mdfs-1.5.2/mdfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/pyproject.toml` & `mdfs-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mdfs"
-version = "1.5.0"
+version = "1.5.2"
 description = "A library for MultiDimensional Feature Selection (MDFS)"
 readme = "README.md"
 dependencies = ["numpy", "scipy", "statsmodels"]
 keywords = ["feature selection", "classification", "machine learning", "information theory"]
 authors = [
   {name = "Radosław Piliszek", email = "r.piliszek@uwb.edu.pl"},
 ]
@@ -28,8 +28,8 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [project.urls]
 homepage = "https://www.mdfs.it/"
-changelog = "https://mdfs.it/CHANGELOG"
+changelog = "https://www.mdfs.it/CHANGELOG"
```

### Comparing `mdfs-1.5.0/setup.py` & `mdfs-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/interface/compute_max_ig.cpp` & `mdfs-1.5.2/shared/interface/compute_max_ig.cpp`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/interface/compute_tuples.cpp` & `mdfs-1.5.2/shared/interface/compute_tuples.cpp`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/interface/discretize.cpp` & `mdfs-1.5.2/shared/interface/discretize.cpp`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/interface/fit_p_value.cpp` & `mdfs-1.5.2/shared/interface/fit_p_value.cpp`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/interface/gen_contrast_variables.cpp` & `mdfs-1.5.2/shared/interface/gen_contrast_variables.cpp`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/interface/get_suggested_range.cpp` & `mdfs-1.5.2/shared/interface/get_suggested_range.cpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #include "get_suggested_range.h"
 
 
 #include <cmath>
 
+#include <algorithm>
+
 using std::pow;
 using std::min;
 using std::max;
 
 
 const double REASONABLE_RANGE = 0.25;
```

### Comparing `mdfs-1.5.0/shared/src/cpu/common.cpp` & `mdfs-1.5.2/shared/src/cpu/common.cpp`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/src/cpu/common.h` & `mdfs-1.5.2/shared/src/cpu/common.h`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/src/cpu/dataset.h` & `mdfs-1.5.2/shared/src/cpu/dataset.h`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/src/cpu/discretize.cpp` & `mdfs-1.5.2/shared/src/cpu/discretize.cpp`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/src/cpu/entropy.h` & `mdfs-1.5.2/shared/src/cpu/entropy.h`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/src/cpu/mdfs.h` & `mdfs-1.5.2/shared/src/cpu/mdfs.h`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/src/cpu/mdfs_count_counters.h` & `mdfs-1.5.2/shared/src/cpu/mdfs_count_counters.h`

 * *Files identical despite different names*

### Comparing `mdfs-1.5.0/shared/src/cpu/mdfs_cpu_kernel.h` & `mdfs-1.5.2/shared/src/cpu/mdfs_cpu_kernel.h`

 * *Files identical despite different names*

