# Comparing `tmp/phenotype_cover-0.7.tar.gz` & `tmp/phenotype_cover-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenotype_cover-0.7.tar", last modified: Sat Nov 12 19:28:15 2022, max compression
+gzip compressed data, was "phenotype_cover-0.8.tar", last modified: Wed Apr 19 15:22:52 2023, max compression
```

## Comparing `phenotype_cover-0.7.tar` & `phenotype_cover-0.8.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:28:15.163200 phenotype_cover-0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-11-12 19:28:07.000000 phenotype_cover-0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-12 19:28:07.000000 phenotype_cover-0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-11-12 19:28:15.163200 phenotype_cover-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-11-12 19:28:07.000000 phenotype_cover-0.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:28:15.159200 phenotype_cover-0.7/phenotype_cover.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-11-12 19:28:15.000000 phenotype_cover-0.7/phenotype_cover.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-11-12 19:28:15.000000 phenotype_cover-0.7/phenotype_cover.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-12 19:28:15.000000 phenotype_cover-0.7/phenotype_cover.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-11-12 19:28:15.000000 phenotype_cover-0.7/phenotype_cover.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-11-12 19:28:15.000000 phenotype_cover-0.7/phenotype_cover.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-12 19:28:15.163200 phenotype_cover-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-11-12 19:28:07.000000 phenotype_cover-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:28:15.159200 phenotype_cover-0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-12 19:28:15.163200 phenotype_cover-0.7/src/phenotype_cover/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-11-12 19:28:07.000000 phenotype_cover-0.7/src/phenotype_cover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2332 2022-11-12 19:28:07.000000 phenotype_cover-0.7/src/phenotype_cover/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    16346 2022-11-12 19:28:07.000000 phenotype_cover-0.7/src/phenotype_cover/_gci_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-12 19:28:07.000000 phenotype_cover-0.7/src/phenotype_cover/_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4096 2022-11-12 19:28:07.000000 phenotype_cover-0.7/src/phenotype_cover/_operations.py
--rw-r--r--   0 runner    (1001) docker     (121)    15848 2022-11-12 19:28:07.000000 phenotype_cover-0.7/src/phenotype_cover/_phenotype_cover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.250129 phenotype_cover-0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-19 15:22:40.000000 phenotype_cover-0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-19 15:22:40.000000 phenotype_cover-0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 15:22:52.250129 phenotype_cover-0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-04-19 15:22:40.000000 phenotype_cover-0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.246129 phenotype_cover-0.8/phenotype_cover.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-19 15:22:52.000000 phenotype_cover-0.8/phenotype_cover.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:22:52.250129 phenotype_cover-0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-19 15:22:40.000000 phenotype_cover-0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.246129 phenotype_cover-0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.250129 phenotype_cover-0.8/src/phenotype_cover/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16346 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_gci_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-04-19 15:22:40.000000 phenotype_cover-0.8/src/phenotype_cover/_phenotype_cover.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:22:52.250129 phenotype_cover-0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-19 15:22:40.000000 phenotype_cover-0.8/tests/test_pairmat_construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-04-19 15:22:40.000000 phenotype_cover-0.8/tests/test_phenotype_cover.py
```

### Comparing `phenotype_cover-0.7/LICENSE.txt` & `phenotype_cover-0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.7/PKG-INFO` & `phenotype_cover-0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenotype_cover
-Version: 0.7
+Version: 0.8
 Summary: phenotype_cover is a package for biomarker discovery using multiset multicover.
 Home-page: https://github.com/euxhenh/phenotype-cover
 Author: Euxhen Hasanaj
 Author-email: ehasanaj@cs.cmu.edu
 License: MIT
 Keywords: biomarker,marker,phenotype,scRNA-seq,set,cover,multiset,multicover
 Platform: ALL
```

### Comparing `phenotype_cover-0.7/README.rst` & `phenotype_cover-0.8/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 Other packages that phenotype-cover depends on are numpy, matplotlib, and scikit-learn.
 
 Import `GreedyPC` or `CEMPC` from `phenotype_cover`.
 
 Example
 
     >>> from phenotype_cover import GreedyPC
+    >>> from sklearn.datasets import make_classification
 
-    >>> # X is the data matrix (log transformed) and y are class labels
-    >>> X = np.log1p(np.random.randint(0, 1000, (1000, 200)))
-    >>> y = np.random.randint(0, 5, 1000)  # class labels
+    >>> # You may need to log-transform X if working with raw counts
+    >>> X, y = make_classification(1000, 200, n_informative=5, n_classes=5, scale=100)
 
     >>> gpc = GreedyPC()
     >>> gpc.fit(X, y)
-    >>> features = gpc.select(10)  # coverage of 10
+    >>> features = gpc.select(100)  # coverage of 100
 
 Some other functionality implemented in GreedyPC
 
     >>> # Number of elements reamining and coverage attained after every iteration
     >>> gpc.plot_progress()
     >>> gpc.n_elements_remaining_per_iter_
     >>> gpc.coverage_per_iter_
```

### Comparing `phenotype_cover-0.7/phenotype_cover.egg-info/PKG-INFO` & `phenotype_cover-0.8/phenotype_cover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenotype-cover
-Version: 0.7
+Version: 0.8
 Summary: phenotype_cover is a package for biomarker discovery using multiset multicover.
 Home-page: https://github.com/euxhenh/phenotype-cover
 Author: Euxhen Hasanaj
 Author-email: ehasanaj@cs.cmu.edu
 License: MIT
 Keywords: biomarker,marker,phenotype,scRNA-seq,set,cover,multiset,multicover
 Platform: ALL
```

### Comparing `phenotype_cover-0.7/setup.py` & `phenotype_cover-0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 options = {
     'name': 'phenotype_cover',
     'description': 'phenotype_cover is a package for biomarker discovery using multiset multicover.',
     'long_description': 'Implements the greedy and cross-entropy-method phenotype cover algorithms.',
     'license': 'MIT',
-    'version': '0.7',
+    'version': '0.8',
     'author': 'Euxhen Hasanaj',
     'author_email': 'ehasanaj@cs.cmu.edu',
     'url': 'https://github.com/euxhenh/phenotype-cover',
     'provides': ['phenotype_cover'],
     'package_dir': {'phenotype_cover': 'src/phenotype_cover'},
     'packages': find_packages(where='src'),
     'cmdclass': cmdclass,
```

### Comparing `phenotype_cover-0.7/src/phenotype_cover/_base.py` & `phenotype_cover-0.8/src/phenotype_cover/_base.py`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.7/src/phenotype_cover/_gci_wrapper.py` & `phenotype_cover-0.8/src/phenotype_cover/_gci_wrapper.py`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.7/src/phenotype_cover/_operations.py` & `phenotype_cover-0.8/src/phenotype_cover/_operations.py`

 * *Files identical despite different names*

### Comparing `phenotype_cover-0.7/src/phenotype_cover/_phenotype_cover.py` & `phenotype_cover-0.8/src/phenotype_cover/_phenotype_cover.py`

 * *Files identical despite different names*

