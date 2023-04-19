# Comparing `tmp/fast_pq-0.2.tar.gz` & `tmp/fast_pq-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_pq-0.2.tar", last modified: Fri Apr 14 22:11:28 2023, max compression
+gzip compressed data, was "fast_pq-0.3.tar", last modified: Wed Apr 19 19:28:24 2023, max compression
```

## Comparing `fast_pq-0.2.tar` & `fast_pq-0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ahle       (501) staff       (20)        0 2023-04-14 22:11:28.542777 fast_pq-0.2/
--rw-r--r--   0 ahle       (501) staff       (20)    34523 2023-04-10 23:48:36.000000 fast_pq-0.2/LICENSE
--rw-r--r--   0 ahle       (501) staff       (20)     6519 2023-04-14 22:11:28.542364 fast_pq-0.2/PKG-INFO
--rw-r--r--   0 ahle       (501) staff       (20)     5883 2023-04-14 20:47:37.000000 fast_pq-0.2/README.md
-drwxr-xr-x   0 ahle       (501) staff       (20)        0 2023-04-14 22:11:28.531291 fast_pq-0.2/fast_pq/
--rw-r--r--   0 ahle       (501) staff       (20)      163 2023-04-12 21:03:18.000000 fast_pq-0.2/fast_pq/__init__.py
--rw-r--r--   0 ahle       (501) staff       (20)   881113 2023-04-14 22:00:56.000000 fast_pq-0.2/fast_pq/_fast_pq.cpp
--rw-r--r--   0 ahle       (501) staff       (20)     5210 2023-04-12 21:03:18.000000 fast_pq-0.2/fast_pq/_transform.py
--rw-r--r--   0 ahle       (501) staff       (20)    10039 2023-04-13 02:30:47.000000 fast_pq-0.2/fast_pq/fast_pq.py
--rw-r--r--   0 ahle       (501) staff       (20)     9438 2023-04-14 19:58:15.000000 fast_pq-0.2/fast_pq/ivf.py
-drwxr-xr-x   0 ahle       (501) staff       (20)        0 2023-04-14 22:11:28.536666 fast_pq-0.2/fast_pq.egg-info/
--rw-r--r--   0 ahle       (501) staff       (20)     6519 2023-04-14 22:11:28.000000 fast_pq-0.2/fast_pq.egg-info/PKG-INFO
--rw-r--r--   0 ahle       (501) staff       (20)      395 2023-04-14 22:11:28.000000 fast_pq-0.2/fast_pq.egg-info/SOURCES.txt
--rw-r--r--   0 ahle       (501) staff       (20)        1 2023-04-14 22:11:28.000000 fast_pq-0.2/fast_pq.egg-info/dependency_links.txt
--rw-r--r--   0 ahle       (501) staff       (20)       55 2023-04-14 22:11:28.000000 fast_pq-0.2/fast_pq.egg-info/requires.txt
--rw-r--r--   0 ahle       (501) staff       (20)        8 2023-04-14 22:11:28.000000 fast_pq-0.2/fast_pq.egg-info/top_level.txt
--rw-r--r--   0 ahle       (501) staff       (20)      854 2023-04-14 22:00:49.000000 fast_pq-0.2/pyproject.toml
--rw-r--r--   0 ahle       (501) staff       (20)       38 2023-04-14 22:11:28.542890 fast_pq-0.2/setup.cfg
--rw-r--r--   0 ahle       (501) staff       (20)      692 2023-04-14 21:45:39.000000 fast_pq-0.2/setup.py
-drwxr-xr-x   0 ahle       (501) staff       (20)        0 2023-04-14 22:11:28.541677 fast_pq-0.2/tests/
--rw-r--r--   0 ahle       (501) staff       (20)     2705 2023-04-13 08:03:59.000000 fast_pq-0.2/tests/test_heap.py
--rw-r--r--   0 ahle       (501) staff       (20)     3530 2023-04-14 19:51:24.000000 fast_pq-0.2/tests/test_ivf.py
--rw-r--r--   0 ahle       (501) staff       (20)     1363 2023-04-14 20:47:37.000000 fast_pq-0.2/tests/test_multiprobe.py
--rw-r--r--   0 ahle       (501) staff       (20)     3454 2023-04-13 02:30:38.000000 fast_pq-0.2/tests/test_pq.py
--rw-r--r--   0 ahle       (501) staff       (20)     2579 2023-04-12 21:03:18.000000 fast_pq-0.2/tests/test_transform.py
+drwxr-xr-x   0 ahle       (501) staff       (20)        0 2023-04-19 19:28:24.222358 fast_pq-0.3/
+-rw-r--r--   0 ahle       (501) staff       (20)    34523 2023-04-10 23:48:36.000000 fast_pq-0.3/LICENSE
+-rw-r--r--   0 ahle       (501) staff       (20)     6685 2023-04-19 19:28:24.221701 fast_pq-0.3/PKG-INFO
+-rw-r--r--   0 ahle       (501) staff       (20)     6049 2023-04-19 19:28:13.000000 fast_pq-0.3/README.md
+drwxr-xr-x   0 ahle       (501) staff       (20)        0 2023-04-19 19:28:24.208605 fast_pq-0.3/fast_pq/
+-rw-r--r--   0 ahle       (501) staff       (20)      186 2023-04-19 00:19:30.000000 fast_pq-0.3/fast_pq/__init__.py
+-rw-r--r--   0 ahle       (501) staff       (20)   881113 2023-04-14 22:00:56.000000 fast_pq-0.3/fast_pq/_fast_pq.cpp
+-rw-r--r--   0 ahle       (501) staff       (20)     5099 2023-04-18 20:57:19.000000 fast_pq-0.3/fast_pq/_transform.py
+-rw-r--r--   0 ahle       (501) staff       (20)    10198 2023-04-18 20:57:19.000000 fast_pq-0.3/fast_pq/fast_pq.py
+-rw-r--r--   0 ahle       (501) staff       (20)    10623 2023-04-19 00:37:43.000000 fast_pq-0.3/fast_pq/ivf.py
+drwxr-xr-x   0 ahle       (501) staff       (20)        0 2023-04-19 19:28:24.213764 fast_pq-0.3/fast_pq.egg-info/
+-rw-r--r--   0 ahle       (501) staff       (20)     6685 2023-04-19 19:28:24.000000 fast_pq-0.3/fast_pq.egg-info/PKG-INFO
+-rw-r--r--   0 ahle       (501) staff       (20)      395 2023-04-19 19:28:24.000000 fast_pq-0.3/fast_pq.egg-info/SOURCES.txt
+-rw-r--r--   0 ahle       (501) staff       (20)        1 2023-04-19 19:28:24.000000 fast_pq-0.3/fast_pq.egg-info/dependency_links.txt
+-rw-r--r--   0 ahle       (501) staff       (20)       55 2023-04-19 19:28:24.000000 fast_pq-0.3/fast_pq.egg-info/requires.txt
+-rw-r--r--   0 ahle       (501) staff       (20)        8 2023-04-19 19:28:24.000000 fast_pq-0.3/fast_pq.egg-info/top_level.txt
+-rw-r--r--   0 ahle       (501) staff       (20)      854 2023-04-19 19:28:13.000000 fast_pq-0.3/pyproject.toml
+-rw-r--r--   0 ahle       (501) staff       (20)       38 2023-04-19 19:28:24.222524 fast_pq-0.3/setup.cfg
+-rw-r--r--   0 ahle       (501) staff       (20)      692 2023-04-14 21:45:39.000000 fast_pq-0.3/setup.py
+drwxr-xr-x   0 ahle       (501) staff       (20)        0 2023-04-19 19:28:24.220583 fast_pq-0.3/tests/
+-rw-r--r--   0 ahle       (501) staff       (20)     2708 2023-04-18 20:57:19.000000 fast_pq-0.3/tests/test_heap.py
+-rw-r--r--   0 ahle       (501) staff       (20)     4273 2023-04-19 00:37:43.000000 fast_pq-0.3/tests/test_ivf.py
+-rw-r--r--   0 ahle       (501) staff       (20)     1374 2023-04-18 20:57:19.000000 fast_pq-0.3/tests/test_multiprobe.py
+-rw-r--r--   0 ahle       (501) staff       (20)     3495 2023-04-18 20:57:19.000000 fast_pq-0.3/tests/test_pq.py
+-rw-r--r--   0 ahle       (501) staff       (20)     2592 2023-04-18 20:57:19.000000 fast_pq-0.3/tests/test_transform.py
```

### Comparing `fast_pq-0.2/LICENSE` & `fast_pq-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_pq-0.2/PKG-INFO` & `fast_pq-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_pq
-Version: 0.2
+Version: 0.3
 Summary: Approximate Nearest Neighbors in Python.
 Author-email: Thomas Dybdahl Ahle <lobais@gmail.com>
 License: AGPL-3.0-or-later
 Project-URL: homepage, https://github.com/thomasahle/fast_pq/
 Keywords: nns,approximate nearest neighbor search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Fast PQ
 FastPQ is a lightweight Python Vector Database specifically designed to offer high performance and be easy to read.
 The main ingredient is an optimized implementation of 4bit Product Quantization (PQ) which enables fast approximate distance computations, 50 times faster than NumPy/BLAS.
 
-![Queries / Recall](https://raw.githubusercontent.com/thomasahle/fast_pq/main/plot.png)
+![Queries / Recall](https://raw.githubusercontent.com/thomasahle/fast_pq/main/static/plot.png)
 
 <p align="center">
 (Performance tradeoff on <a href="http://ann-benchmarks.com/glove-100-angular_10_angular.html">ANN Benchmarks</a>. Up and to the right is better.)
 </p>
 
 ## Features
 
@@ -71,18 +71,18 @@
 This will perform approximate nearest neighbor search using Inverted File Indexing, with 10 probes for each query. Note that we first have to call the `fit` method to build the codebook, and then the `build` method to populate the inverted file.
 
 See also `examples/` for more detailed examples of usage.
 
 ## Installing
 
 You need to build `fast_pq` before you can run it, as it contains Cython code.
+The easiest way to do this is to simply run
 
 ```bash
-$ pip install -r requirements.txt
-$ python setup.py build_ext --inplace
+$ pip install .
 ```
 
 To test it we can run an example:
 
 ```bash
 $ python -m examples.example
 n=16000, d=128, queries=1000, dims_per_block=2
@@ -100,14 +100,19 @@
 Scipy speed for comparison: 2.249645948410034
 ```
 
 In this example Fast PQ is about 16 times faster than optmized scipy/numpy.
 The reason is that Fast PQ uses a trick called [Accelerated Nearest Neighbor Search with Qick ADC](https://dl.acm.org/doi/abs/10.1145/3078971.3078992)
 with which SIMD instructions are used to perform 16 inner product operations in a single instruction.
 
+### Developing
+If you are helping develop fast_pq, and need to test a change to the Cython code, you can rebuild it with
+```bash
+$ python setup.py build_ext --inplace
+```
 
 ## Class Overview
 
 The project consists of two main classes: IVF and FastPQ. The IVF class is used to build an IVF index with cluster centers, fit a product quantizer on the data, and perform queries on the index. The FastPQ class is used to create a product quantizer that can quickly transform data and compute distance tables.
 
 IVF: This class is responsible for creating an IVF index using clustering (either Euclidean or angular) and FastPQ for quantization. It provides methods to fit the index on data, build the index with quantized data, and query the index for nearest neighbors.
 Main methods:
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: fast_pq Version: 0.2 Summary: Approximate Nearest
+Metadata-Version: 2.1 Name: fast_pq Version: 0.3 Summary: Approximate Nearest
 Neighbors in Python. Author-email: Thomas Dybdahl Ahle
 gmail.com> License: AGPL-3.0-or-later Project-URL: homepage, https://
 github.com/thomasahle/fast_pq/ Keywords: nns,approximate nearest neighbor
 search Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
 Content-Type: text/markdown License-File: LICENSE # Fast PQ FastPQ is a
 lightweight Python Vector Database specifically designed to offer high
 performance and be easy to read. The main ingredient is an optimized
 implementation of 4bit Product Quantization (PQ) which enables fast approximate
 distance computations, 50 times faster than NumPy/BLAS. ![Queries / Recall]
-(https://raw.githubusercontent.com/thomasahle/fast_pq/main/plot.png)
+(https://raw.githubusercontent.com/thomasahle/fast_pq/main/static/plot.png)
    (Performance tradeoff on ANN_Benchmarks. Up and to the right is better.)
 ## Features FastPQ is a very lightweight index, much smaller than the dataset
 itself. It is also quick to build, requiring only a single pass of sklearn's
 KMeans over the dataset. ## Example Let's generate some random data ```python
 import numpy as np X = np.random.rand(10000, 128) queries = np.random.rand(100,
 128) ``` We can use the `FastPQ` class to quantize the data and perform nearest
 neighbor search. ```python from fast_pq import FastPQ # Initialize PQ with 64
@@ -31,26 +31,28 @@
 perform approximate nearest neighbor search with Inverted File Indexing.
 ```python from fast_pq import IVF ivf = IVF("euclidean", n_clusters=100).fit
 (X).build(X) neighbors = ivf.query(queries, k=10, n_probes=10) ``` This will
 perform approximate nearest neighbor search using Inverted File Indexing, with
 10 probes for each query. Note that we first have to call the `fit` method to
 build the codebook, and then the `build` method to populate the inverted file.
 See also `examples/` for more detailed examples of usage. ## Installing You
-need to build `fast_pq` before you can run it, as it contains Cython code.
-```bash $ pip install -r requirements.txt $ python setup.py build_ext --inplace
-``` To test it we can run an example: ```bash $ python -m examples.example
-n=16000, d=128, queries=1000, dims_per_block=2 Sampling Computing true
-neighbours Fitting PQ Querying Median place of true nearest neighbor: 1.0 90%
-quantile: 19.0 Queries/second: 7101.262693814528 Total time spent on
-preprocess: 0.09025406837463379 Total time spent on search: 0.05056595802307129
-Scipy speed for comparison: 2.249645948410034 ``` In this example Fast PQ is
-about 16 times faster than optmized scipy/numpy. The reason is that Fast PQ
-uses a trick called [Accelerated Nearest Neighbor Search with Qick ADC](https:/
-/dl.acm.org/doi/abs/10.1145/3078971.3078992) with which SIMD instructions are
-used to perform 16 inner product operations in a single instruction. ## Class
+need to build `fast_pq` before you can run it, as it contains Cython code. The
+easiest way to do this is to simply run ```bash $ pip install . ``` To test it
+we can run an example: ```bash $ python -m examples.example n=16000, d=128,
+queries=1000, dims_per_block=2 Sampling Computing true neighbours Fitting PQ
+Querying Median place of true nearest neighbor: 1.0 90% quantile: 19.0 Queries/
+second: 7101.262693814528 Total time spent on preprocess: 0.09025406837463379
+Total time spent on search: 0.05056595802307129 Scipy speed for comparison:
+2.249645948410034 ``` In this example Fast PQ is about 16 times faster than
+optmized scipy/numpy. The reason is that Fast PQ uses a trick called
+[Accelerated Nearest Neighbor Search with Qick ADC](https://dl.acm.org/doi/abs/
+10.1145/3078971.3078992) with which SIMD instructions are used to perform 16
+inner product operations in a single instruction. ### Developing If you are
+helping develop fast_pq, and need to test a change to the Cython code, you can
+rebuild it with ```bash $ python setup.py build_ext --inplace ``` ## Class
 Overview The project consists of two main classes: IVF and FastPQ. The IVF
 class is used to build an IVF index with cluster centers, fit a product
 quantizer on the data, and perform queries on the index. The FastPQ class is
 used to create a product quantizer that can quickly transform data and compute
 distance tables. IVF: This class is responsible for creating an IVF index using
 clustering (either Euclidean or angular) and FastPQ for quantization. It
 provides methods to fit the index on data, build the index with quantized data,
```

### Comparing `fast_pq-0.2/README.md` & `fast_pq-0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Fast PQ
 FastPQ is a lightweight Python Vector Database specifically designed to offer high performance and be easy to read.
 The main ingredient is an optimized implementation of 4bit Product Quantization (PQ) which enables fast approximate distance computations, 50 times faster than NumPy/BLAS.
 
-![Queries / Recall](https://raw.githubusercontent.com/thomasahle/fast_pq/main/plot.png)
+![Queries / Recall](https://raw.githubusercontent.com/thomasahle/fast_pq/main/static/plot.png)
 
 <p align="center">
 (Performance tradeoff on <a href="http://ann-benchmarks.com/glove-100-angular_10_angular.html">ANN Benchmarks</a>. Up and to the right is better.)
 </p>
 
 ## Features
 
@@ -54,18 +54,18 @@
 This will perform approximate nearest neighbor search using Inverted File Indexing, with 10 probes for each query. Note that we first have to call the `fit` method to build the codebook, and then the `build` method to populate the inverted file.
 
 See also `examples/` for more detailed examples of usage.
 
 ## Installing
 
 You need to build `fast_pq` before you can run it, as it contains Cython code.
+The easiest way to do this is to simply run
 
 ```bash
-$ pip install -r requirements.txt
-$ python setup.py build_ext --inplace
+$ pip install .
 ```
 
 To test it we can run an example:
 
 ```bash
 $ python -m examples.example
 n=16000, d=128, queries=1000, dims_per_block=2
@@ -83,14 +83,19 @@
 Scipy speed for comparison: 2.249645948410034
 ```
 
 In this example Fast PQ is about 16 times faster than optmized scipy/numpy.
 The reason is that Fast PQ uses a trick called [Accelerated Nearest Neighbor Search with Qick ADC](https://dl.acm.org/doi/abs/10.1145/3078971.3078992)
 with which SIMD instructions are used to perform 16 inner product operations in a single instruction.
 
+### Developing
+If you are helping develop fast_pq, and need to test a change to the Cython code, you can rebuild it with
+```bash
+$ python setup.py build_ext --inplace
+```
 
 ## Class Overview
 
 The project consists of two main classes: IVF and FastPQ. The IVF class is used to build an IVF index with cluster centers, fit a product quantizer on the data, and perform queries on the index. The FastPQ class is used to create a product quantizer that can quickly transform data and compute distance tables.
 
 IVF: This class is responsible for creating an IVF index using clustering (either Euclidean or angular) and FastPQ for quantization. It provides methods to fit the index on data, build the index with quantized data, and query the index for nearest neighbors.
 Main methods:
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
 # Fast PQ FastPQ is a lightweight Python Vector Database specifically designed
 to offer high performance and be easy to read. The main ingredient is an
 optimized implementation of 4bit Product Quantization (PQ) which enables fast
 approximate distance computations, 50 times faster than NumPy/BLAS. ![Queries /
-Recall](https://raw.githubusercontent.com/thomasahle/fast_pq/main/plot.png)
+Recall](https://raw.githubusercontent.com/thomasahle/fast_pq/main/static/
+plot.png)
    (Performance tradeoff on ANN_Benchmarks. Up and to the right is better.)
 ## Features FastPQ is a very lightweight index, much smaller than the dataset
 itself. It is also quick to build, requiring only a single pass of sklearn's
 KMeans over the dataset. ## Example Let's generate some random data ```python
 import numpy as np X = np.random.rand(10000, 128) queries = np.random.rand(100,
 128) ``` We can use the `FastPQ` class to quantize the data and perform nearest
 neighbor search. ```python from fast_pq import FastPQ # Initialize PQ with 64
@@ -22,26 +23,28 @@
 perform approximate nearest neighbor search with Inverted File Indexing.
 ```python from fast_pq import IVF ivf = IVF("euclidean", n_clusters=100).fit
 (X).build(X) neighbors = ivf.query(queries, k=10, n_probes=10) ``` This will
 perform approximate nearest neighbor search using Inverted File Indexing, with
 10 probes for each query. Note that we first have to call the `fit` method to
 build the codebook, and then the `build` method to populate the inverted file.
 See also `examples/` for more detailed examples of usage. ## Installing You
-need to build `fast_pq` before you can run it, as it contains Cython code.
-```bash $ pip install -r requirements.txt $ python setup.py build_ext --inplace
-``` To test it we can run an example: ```bash $ python -m examples.example
-n=16000, d=128, queries=1000, dims_per_block=2 Sampling Computing true
-neighbours Fitting PQ Querying Median place of true nearest neighbor: 1.0 90%
-quantile: 19.0 Queries/second: 7101.262693814528 Total time spent on
-preprocess: 0.09025406837463379 Total time spent on search: 0.05056595802307129
-Scipy speed for comparison: 2.249645948410034 ``` In this example Fast PQ is
-about 16 times faster than optmized scipy/numpy. The reason is that Fast PQ
-uses a trick called [Accelerated Nearest Neighbor Search with Qick ADC](https:/
-/dl.acm.org/doi/abs/10.1145/3078971.3078992) with which SIMD instructions are
-used to perform 16 inner product operations in a single instruction. ## Class
+need to build `fast_pq` before you can run it, as it contains Cython code. The
+easiest way to do this is to simply run ```bash $ pip install . ``` To test it
+we can run an example: ```bash $ python -m examples.example n=16000, d=128,
+queries=1000, dims_per_block=2 Sampling Computing true neighbours Fitting PQ
+Querying Median place of true nearest neighbor: 1.0 90% quantile: 19.0 Queries/
+second: 7101.262693814528 Total time spent on preprocess: 0.09025406837463379
+Total time spent on search: 0.05056595802307129 Scipy speed for comparison:
+2.249645948410034 ``` In this example Fast PQ is about 16 times faster than
+optmized scipy/numpy. The reason is that Fast PQ uses a trick called
+[Accelerated Nearest Neighbor Search with Qick ADC](https://dl.acm.org/doi/abs/
+10.1145/3078971.3078992) with which SIMD instructions are used to perform 16
+inner product operations in a single instruction. ### Developing If you are
+helping develop fast_pq, and need to test a change to the Cython code, you can
+rebuild it with ```bash $ python setup.py build_ext --inplace ``` ## Class
 Overview The project consists of two main classes: IVF and FastPQ. The IVF
 class is used to build an IVF index with cluster centers, fit a product
 quantizer on the data, and perform queries on the index. The FastPQ class is
 used to create a product quantizer that can quickly transform data and compute
 distance tables. IVF: This class is responsible for creating an IVF index using
 clustering (either Euclidean or angular) and FastPQ for quantization. It
 provides methods to fit the index on data, build the index with quantized data,
```

### Comparing `fast_pq-0.2/fast_pq/_fast_pq.cpp` & `fast_pq-0.3/fast_pq/_fast_pq.cpp`

 * *Files identical despite different names*

### Comparing `fast_pq-0.2/fast_pq/_transform.py` & `fast_pq-0.3/fast_pq/_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,18 +66,18 @@
     n, d = data0.shape
     assert d % 2 == 0  # Because we load two rows at a time (128bits)
     assert np.all(data0 < 16) and np.all(0 <= data0)
     # Convert data to Quick-ADC format
     data = data0.reshape(n // 16, 16, d)
     data = data.transpose(0, 2, 1)
     # Interleave rows two by two
-    data = (                                     # [0,1,2,3,4,5,6,7]
-        data.reshape(n // 16, d // 2, 2, 16)     # [0,1,2,3], [4,5,6,7]
-        .reshape(n // 16, d // 2, 32, order="F") # [0,4,1,5,2,6,3,7]
-        .reshape(n // 16, d, 16)                 # [0,4,1,5], [2,6,3,7]
+    data = (  # [0,1,2,3,4,5,6,7]
+        data.reshape(n // 16, d // 2, 2, 16)  # [0,1,2,3], [4,5,6,7]
+        .reshape(n // 16, d // 2, 32, order="F")  # [0,4,1,5,2,6,3,7]
+        .reshape(n // 16, d, 16)  # [0,4,1,5], [2,6,3,7]
     )
     # Reversing last dimension for endianess
     data = data[:, :, ::-1]
     # Extra tests for required format
     assert data[0, 0, -1] == data0[0][0]
     assert data[0, 0, -2] == data0[0][1]
     assert data[0, 0, -3] == data0[1][0]
@@ -127,16 +127,16 @@
     """
     chunks, d = transformed_data.shape
     n = chunks * 16
 
     shifts = np.arange(15, -1, -1, dtype=np.uint64) * 4
     data = (transformed_data[..., np.newaxis] >> shifts) & 0xF
 
-    data = data[:, :, ::-1]                               # [0,4,1,5], [2,6,3,7]
-    data = data.reshape(chunks, d // 2, 32)               # [0,4,1,5,2,6,3,7]
-    data = data.reshape(chunks, d // 2, 2, 16, order='F') # [0,1,2,3], [4,5,6,7]
-    data = data.reshape(chunks, d, 16)                    # [0,1,2,3], [4,5,6,7]
+    data = data[:, :, ::-1]  # [0,4,1,5], [2,6,3,7]
+    data = data.reshape(chunks, d // 2, 32)  # [0,4,1,5,2,6,3,7]
+    data = data.reshape(chunks, d // 2, 2, 16, order="F")  # [0,1,2,3], [4,5,6,7]
+    data = data.reshape(chunks, d, 16)  # [0,1,2,3], [4,5,6,7]
 
     data = data.transpose(0, 2, 1)
     data = data.reshape(n, d)
 
     return data
```

### Comparing `fast_pq-0.2/fast_pq/fast_pq.py` & `fast_pq-0.3/fast_pq/fast_pq.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,18 +4,25 @@
 
 import warnings
 from sklearn.exceptions import ConvergenceWarning
 
 from ._transform import transform_data, transform_tables
 from ._fast_pq import query_pq_sse, estimate_pq_sse, init_heap
 
+from numpy.core._methods import _amax, _mean
+
 warnings.simplefilter("error", category=ConvergenceWarning)
 
 TransformedData = namedtuple("TransformedData", "size packed")
 
+import os
+
+os.environ["NUMPY_EXPERIMENTAL_ARRAY_FUNCTION"] = "0"
+
+
 def pad1(arr, m):
     (s,) = arr.shape
     new_shape = (s + (-s) % m,)
     padded_arr = np.zeros(new_shape, dtype=arr.dtype)
     padded_arr[:s] = arr
     return padded_arr
 
@@ -48,15 +55,15 @@
         Parameters
         ----------
         dims_per_block : int
             The number of dimensions per block.
         """
         self.dims_per_block = dims_per_block
         self.centers = None  # Shape: (n_blocks, 16, dims_per_block)
-        self.center_norms_sq = None  # Shape: (n_blocks, 16)
+        self.sqrt_n_blocks = None
 
     def fit(self, data, verbose=False):
         """
         Fits the FastPQ model to the given data.
 
         Parameters
         ----------
@@ -94,19 +101,23 @@
             try:
                 cl.fit(data[:, i * dpb : (i + 1) * dpb])
             except ConvergenceWarning:
                 pass
             # It doesn't give too much precision to do separate centers for each block,
             # but durnig queries we need seperate distance tables per block anyway, so
             # it doesn't cost us much.
+            # We .copy() the centers because we are reusing the KMeans object.
             centers.append(cl.cluster_centers_.copy())
             # Might as well grab the labels (transformed column) while we have it.
             transformed.append(cl.labels_[:, None])
-        self.centers = np.array(centers, dtype=np.float32)
-        self.center_norms_sq = np.linalg.norm(centers, axis=2) ** 2
+        # (d / dpb, 16, dpb) -> (16, d)
+        self.centers = (
+            np.array(centers, dtype=np.float32).transpose(1, 0, 2).reshape(16, d)
+        )
+        self.sqrt_n_blocks = np.sqrt(d // dpb)
 
         labels = np.hstack(transformed).astype(np.uint8)
         return TransformedData(true_n, transform_data(labels))
 
     def transform(self, data):
         """
         Transforms the given data using the FastPQ model.
@@ -124,19 +135,23 @@
         assert self.centers is not None, "PQ has not been fitted"
         if data.size == 0:
             return data
         true_n = data.shape[0]
         data = pad2(data, 16, 2 * self.dims_per_block)
         n, d = data.shape
         assert n % 16 == 0
-        parts = data.reshape(n, -1, self.dims_per_block)
-        ips = np.einsum("ijk,jlk->ijl", parts, self.centers)  # Shape: (n, n_blocks, 16)
-        labels = np.argmin(self.center_norms_sq - 2 * ips, axis=2)
-        assert labels.shape == (n, d // self.dims_per_block)
-        labels = np.array(labels, dtype=np.uint8)
+        dpb = self.dims_per_block
+        blocks = d // dpb
+        dists = (
+            np.square(self.centers[None] - data[:, None])
+            .reshape(n, 16, blocks, dpb)
+            .sum(axis=-1)
+        )
+        labels = np.argmin(dists, axis=1).astype(np.uint8)
+        assert labels.shape == (n, blocks)
         return TransformedData(true_n, transform_data(labels))
 
     def distance_table(self, q):
         """
         Computes the distance table for the given query vector q.
 
         Parameters
@@ -145,36 +160,33 @@
             The query vector.
 
         Returns
         -------
         _FastDistanceTable
             The FastDistanceTable object containing the computed distance table.
         """
-        q = pad1(q, 2 * self.dims_per_block)
         dpb = self.dims_per_block
-        n_blocks = q.size / dpb
-
-        parts = q.reshape(-1, dpb)
+        q = pad1(q, 2 * dpb)
 
-        # Center the data in the range [-128, 128]
-        dists = self.center_norms_sq - 2 * np.einsum("ijk,ik->ij", self.centers, parts)
+        diff = (self.centers - q).reshape(16, -1, dpb)
+        dists = np.einsum("ijk,ijk->ij", diff, diff)
 
         # We do this by shifting by the mean value and scaling by the nuber of blocks.
         # The idea is that we don't want to have an overflow as we add together
-        # distances in uint8 format.
-        # The median also works well here, maybe even a bit better, but it takes longer to compute.
-        shift = np.median(dists)
-        scale = 128 / (np.max(np.abs(dists - shift)) * np.sqrt(n_blocks))
-
-        # Round to nearest integer towards zero.
-        table = np.round((dists - shift) * scale)
+        # distances in uint8 format. The median seems to work better here than the mean,
+        # even though it's a bit more expensive to compute. It turns out the squared distances
+        # are roughly exponentially distributed, so the median is ~ mean * log(2).
+        shift = _mean(dists) * 0.6931471806
+        dists -= shift
+        scale = 128 / (_amax(dists) * self.sqrt_n_blocks)
+        table = np.round(dists * scale)
 
         # The transformation doesn't care about the sign, so we just use uint
         table = table.astype(np.uint8)
-        trans = transform_tables(table)
+        trans = transform_tables(table.T)
         return _FastDistanceTable(q, trans, shift, scale, signed=True)
 
     def udistance_table(self, q):
         """
         Computes the unsigned distance table for the given query vector q.
         Currently experimental.
 
@@ -184,25 +196,24 @@
             The query vector.
 
         Returns
         -------
         _FastDistanceTable
             The FastDistanceTable object containing the computed unsigned distance table.
         """
-        q = pad1(q, 2 * self.dims_per_block)
         dpb = self.dims_per_block
-        n_blocks = q.size / dpb
-        parts = q.reshape(-1, dpb)
-        dists = self.center_norms_sq - 2 * np.einsum("ijk,ik->ij", self.centers, parts)
+        q = pad1(q, 2 * dpb)
+        n_blocks = q.size // dpb
+        dists = np.square(self.centers - q).reshape(16, n_blocks, dpb).sum(axis=-1)
         shift = np.min(dists)
         dists -= shift
-        scale = 255 / (np.max(dists) * np.sqrt(n_blocks))
-        table *= scale
+        scale = 255 / (np.max(dists) * np.log(n_blocks) * np.sqrt(n_blocks))
+        table = np.round(dists * scale)
         table = table.astype(np.uint8)
-        trans = transform_tables(table)
+        trans = transform_tables(table.T)
         return _FastDistanceTable(q, trans, shift, scale, signed=False)
 
 
 class _FastDistanceTable:
     def __init__(self, q, transformed_tables, mean, scale, signed):
         self.q = q
         self.tables = transformed_tables
@@ -216,19 +227,18 @@
             "scale={self.scale}, signed={self.signed})"
         )
 
     def estimate_distances(self, transformed_data, out=None, rescale=False):
         true_n, transformed_data = transformed_data
         if out is None:
             out = np.zeros(2 * len(transformed_data), dtype=np.uint64)
-        estimate_pq_sse(transformed_data, self.tables, out, True)
+        estimate_pq_sse(transformed_data, self.tables, out, self.signed)
         res = out.view(np.int8)
         res = res[:true_n]  # Trim padding elements
         if not rescale:
-            # TODO: Would sorting actually be faster if we casted to float?
             return res
         # The center_norm is already built into res, so we just need to add
         # the norm of q and rescale.
         as_float = np.ascontiguousarray(res, dtype=np.float32)
         return self.q @ self.q + (as_float / self.scale + self.mean)
 
     def top(self, transformed_data, data, k=1, rescore=None):
@@ -242,16 +252,18 @@
         # In the first pass we collect `rescore` many rows
         if not rescore:
             rescore = min(2 * k + 10, true_n)
         assert true_n >= rescore >= k
 
         indices = np.zeros((rescore,), dtype=np.int64)
         values = np.zeros((rescore,), dtype=np.int32)
-        init_heap(indices, values, True)
-        query_pq_sse(transformed_data, true_n, self.tables, indices, values, True)
+        init_heap(indices, values, self.signed)
+        query_pq_sse(
+            transformed_data, true_n, self.tables, indices, values, self.signed
+        )
 
         # In a second pass we compute the true distances and return the actually
         # closest points. If we got fewer or exactly k outputs, there is no need
         # to compute the true distaneces.
         if rescore <= k:
             return indices, values
```

### Comparing `fast_pq-0.2/fast_pq/ivf.py` & `fast_pq-0.3/fast_pq/ivf.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,58 @@
     between X and Y.
     """
     diff = Y - x
     dists = np.einsum("ij,ij->i", diff, diff)
     return dists.argpartition(kth=k)[:k]
 
 
+def group_data_by_indices(X, indices, k):
+    """
+    Given a 2D array `X` of shape (N, d), a 2D array `indices` of shape (N, c) with integers in [0, k),
+    and an integer `k`, return a list `parts` of k arrays, such that all rows X[i] are in parts[indices[i, j]] for some j.
+
+    Args:
+    X (np.ndarray): A 2D numpy array of shape (N, d) containing the data points.
+    indices (np.ndarray): A 2D numpy array of shape (N, c) containing integers in the range [0, k).
+    k (int): The number of groups.
+
+    Returns:
+    list: A list of k numpy arrays, where each array contains the rows of X that belong to the corresponding group.
+    """
+    # Initialize an empty list to store the data points for each group
+    assert 0 <= np.min(indices) and np.max(indices) < k
+    parts = [[] for _ in range(k)]
+    ids = [[] for _ in range(k)]
+
+    # Iterate over each column in indices
+    for i in range(indices.shape[1]):
+        # Get the current column of indices
+        col = indices[:, i]
+
+        # Sort X by the current column of indices
+        sorted_indices = np.argsort(col)
+        sorted_X = X[sorted_indices]
+
+        # Compute the length of the runs in the current column of indices (sorted)
+        sorted_indices_unique, run_lengths = np.unique(
+            col[sorted_indices], return_counts=True
+        )
+        # Use a loop only over j = 0 to k - 1 that selects the runs of X and adds them to the corresponding group in parts
+        start = 0
+        for i, run_length in enumerate(run_lengths):
+            end = start + run_length
+            parts[sorted_indices_unique[i]].append(sorted_X[start:end])
+            ids[sorted_indices_unique[i]].append(sorted_indices[start:end])
+            start = end
+
+    parts = [np.vstack(part) for part in parts]
+    ids = [np.hstack(id_list) for id_list in ids]
+    return parts, ids
+
+
 class IVF:
     def __init__(self, metric, n_clusters, pq=None):
         assert metric in ["euclidean", "angular"]
         self.metric = metric
         self.pq = FastPQ(dims_per_block=2) if pq is None else pq
         assert self.pq.centers is None, "PQ should not be pre-fitted"
         self.pq_transformed_points = [None] * n_clusters
@@ -103,15 +147,17 @@
 
             elif self.metric == "angular":
                 # For angular we use kmeans clustering, but normalize the norm of the centers
                 # as to make inner product equivalent to angular similarity.
                 X = X / np.linalg.norm(X, axis=1, keepdims=True)
                 cl.fit(X)
                 self.all_centers = cl.cluster_centers_
-                self.all_centers /= np.linalg.norm(self.all_centers, axis=1, keepdims=True)
+                self.all_centers /= np.linalg.norm(
+                    self.all_centers, axis=1, keepdims=True
+                )
 
         with timer(verbose, "Fitting PQ to data..."):
             self.pq.fit(X, verbose=verbose)
 
         return self
 
     def build(self, X, n_probes=2, verbose=False):
@@ -129,19 +175,21 @@
 
         Returns:
         --------
         self : object
             Returns the instance itself, with the index structure built and data points assigned to the nearest n_probes cluster centers.
         """
 
-        assert n_probes <= self.n_clusters, f"Can't assign points to {n_probes} clusters, as index only has {self.n_clusters}"
+        assert (
+            n_probes <= self.n_clusters
+        ), f"Can't assign points to {n_probes} clusters, as index only has {self.n_clusters}"
         self.data = data = X.copy()
 
         with timer(verbose, "Computing nearest clusters..."):
-            # TODO: Use compression here, somehow.
+            # TODO: Use the compression here, somehow.
 
             if self.metric == "euclidean":
                 distances = cdist(data, self.all_centers)
             elif self.metric == "angular":
                 data /= np.linalg.norm(data, axis=1, keepdims=True)
                 distances = -data @ self.all_centers.T
 
@@ -152,40 +200,20 @@
         # in the IVF, or if the query is OOD.
         with timer(verbose, "PQ Transforming active centers..."):
             self.active_centers = np.ascontiguousarray(
                 self.all_centers[np.unique(nearest_indices)], dtype=np.float32
             )
             self.pq_transformed_centers = self.pq.transform(self.active_centers)
 
-        t0, t1, t2 = 0, 0, 0
-        with timer(verbose, "Transforming points and adding them to their nearest centers..."):
+        with timer(verbose, "Transforming points..."):
+            groups, self.ids = group_data_by_indices(
+                data, nearest_indices, self.active_centers.shape[0]
+            )
             for i in range(self.active_centers.shape[0]):
-                # TODO: This is a lot slower than it needs to be.
-                s = time.time()
-                mask = np.any(nearest_indices == i, axis=1)
-                t0 += time.time() - s
-
-                # TODO: We should be able to extract the relevant data
-                # directly from a previously transformed X.
-                # However, that would require slicing into the compressed QuickADC format,
-                # which is annoying.
-                s = time.time()
-                self.pq_transformed_points[i] = self.pq.transform(
-                    np.ascontiguousarray(data[mask])
-                )
-                t1 += time.time() - s
-
-                s = time.time()
-                self.ids[i] = np.arange(data.shape[0], dtype=np.int64)[mask]
-                t2 += time.time() - s
-
-        if verbose:
-            print(f"Finding any: {t0:.1f}")
-            print(f"Transforming: {t1:.1f}")
-            print(f"Computing ids: {t2:.1f}")
+                self.pq_transformed_points[i] = self.pq.transform(groups[i])
 
         return self
 
     def query(self, q, k, n_probes=1, pass_1=None):
         """
         Queries the data structure to find the top k closest elements to the given query vector q.
 
@@ -220,15 +248,21 @@
             pass_1 = (n_probes + 1) * k + 1
         indices = np.full(pass_1, -1, dtype=np.int64)
         values = np.full(pass_1, 127, dtype=np.int32)
 
         for i, cl in enumerate(top):
             true_n, transformed_data = self.pq_transformed_points[cl]
             query_pq_sse(
-                transformed_data, true_n, dtable.tables, indices, values, True, labels=self.ids[cl]
+                transformed_data,
+                true_n,
+                dtable.tables,
+                indices,
+                values,
+                True,
+                labels=self.ids[cl],
             )
 
         # We may have gotten some heap padding elements mixed in. This is very rarely an issue,
         # so we check before we spend time building a mask and indexing.
         if -1 in indices:
             indices = indices[indices != -1]
```

### Comparing `fast_pq-0.2/fast_pq.egg-info/PKG-INFO` & `fast_pq-0.3/fast_pq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-pq
-Version: 0.2
+Version: 0.3
 Summary: Approximate Nearest Neighbors in Python.
 Author-email: Thomas Dybdahl Ahle <lobais@gmail.com>
 License: AGPL-3.0-or-later
 Project-URL: homepage, https://github.com/thomasahle/fast_pq/
 Keywords: nns,approximate nearest neighbor search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Fast PQ
 FastPQ is a lightweight Python Vector Database specifically designed to offer high performance and be easy to read.
 The main ingredient is an optimized implementation of 4bit Product Quantization (PQ) which enables fast approximate distance computations, 50 times faster than NumPy/BLAS.
 
-![Queries / Recall](https://raw.githubusercontent.com/thomasahle/fast_pq/main/plot.png)
+![Queries / Recall](https://raw.githubusercontent.com/thomasahle/fast_pq/main/static/plot.png)
 
 <p align="center">
 (Performance tradeoff on <a href="http://ann-benchmarks.com/glove-100-angular_10_angular.html">ANN Benchmarks</a>. Up and to the right is better.)
 </p>
 
 ## Features
 
@@ -71,18 +71,18 @@
 This will perform approximate nearest neighbor search using Inverted File Indexing, with 10 probes for each query. Note that we first have to call the `fit` method to build the codebook, and then the `build` method to populate the inverted file.
 
 See also `examples/` for more detailed examples of usage.
 
 ## Installing
 
 You need to build `fast_pq` before you can run it, as it contains Cython code.
+The easiest way to do this is to simply run
 
 ```bash
-$ pip install -r requirements.txt
-$ python setup.py build_ext --inplace
+$ pip install .
 ```
 
 To test it we can run an example:
 
 ```bash
 $ python -m examples.example
 n=16000, d=128, queries=1000, dims_per_block=2
@@ -100,14 +100,19 @@
 Scipy speed for comparison: 2.249645948410034
 ```
 
 In this example Fast PQ is about 16 times faster than optmized scipy/numpy.
 The reason is that Fast PQ uses a trick called [Accelerated Nearest Neighbor Search with Qick ADC](https://dl.acm.org/doi/abs/10.1145/3078971.3078992)
 with which SIMD instructions are used to perform 16 inner product operations in a single instruction.
 
+### Developing
+If you are helping develop fast_pq, and need to test a change to the Cython code, you can rebuild it with
+```bash
+$ python setup.py build_ext --inplace
+```
 
 ## Class Overview
 
 The project consists of two main classes: IVF and FastPQ. The IVF class is used to build an IVF index with cluster centers, fit a product quantizer on the data, and perform queries on the index. The FastPQ class is used to create a product quantizer that can quickly transform data and compute distance tables.
 
 IVF: This class is responsible for creating an IVF index using clustering (either Euclidean or angular) and FastPQ for quantization. It provides methods to fit the index on data, build the index with quantized data, and query the index for nearest neighbors.
 Main methods:
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: fast-pq Version: 0.2 Summary: Approximate Nearest
+Metadata-Version: 2.1 Name: fast-pq Version: 0.3 Summary: Approximate Nearest
 Neighbors in Python. Author-email: Thomas Dybdahl Ahle
 gmail.com> License: AGPL-3.0-or-later Project-URL: homepage, https://
 github.com/thomasahle/fast_pq/ Keywords: nns,approximate nearest neighbor
 search Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
 Content-Type: text/markdown License-File: LICENSE # Fast PQ FastPQ is a
 lightweight Python Vector Database specifically designed to offer high
 performance and be easy to read. The main ingredient is an optimized
 implementation of 4bit Product Quantization (PQ) which enables fast approximate
 distance computations, 50 times faster than NumPy/BLAS. ![Queries / Recall]
-(https://raw.githubusercontent.com/thomasahle/fast_pq/main/plot.png)
+(https://raw.githubusercontent.com/thomasahle/fast_pq/main/static/plot.png)
    (Performance tradeoff on ANN_Benchmarks. Up and to the right is better.)
 ## Features FastPQ is a very lightweight index, much smaller than the dataset
 itself. It is also quick to build, requiring only a single pass of sklearn's
 KMeans over the dataset. ## Example Let's generate some random data ```python
 import numpy as np X = np.random.rand(10000, 128) queries = np.random.rand(100,
 128) ``` We can use the `FastPQ` class to quantize the data and perform nearest
 neighbor search. ```python from fast_pq import FastPQ # Initialize PQ with 64
@@ -31,26 +31,28 @@
 perform approximate nearest neighbor search with Inverted File Indexing.
 ```python from fast_pq import IVF ivf = IVF("euclidean", n_clusters=100).fit
 (X).build(X) neighbors = ivf.query(queries, k=10, n_probes=10) ``` This will
 perform approximate nearest neighbor search using Inverted File Indexing, with
 10 probes for each query. Note that we first have to call the `fit` method to
 build the codebook, and then the `build` method to populate the inverted file.
 See also `examples/` for more detailed examples of usage. ## Installing You
-need to build `fast_pq` before you can run it, as it contains Cython code.
-```bash $ pip install -r requirements.txt $ python setup.py build_ext --inplace
-``` To test it we can run an example: ```bash $ python -m examples.example
-n=16000, d=128, queries=1000, dims_per_block=2 Sampling Computing true
-neighbours Fitting PQ Querying Median place of true nearest neighbor: 1.0 90%
-quantile: 19.0 Queries/second: 7101.262693814528 Total time spent on
-preprocess: 0.09025406837463379 Total time spent on search: 0.05056595802307129
-Scipy speed for comparison: 2.249645948410034 ``` In this example Fast PQ is
-about 16 times faster than optmized scipy/numpy. The reason is that Fast PQ
-uses a trick called [Accelerated Nearest Neighbor Search with Qick ADC](https:/
-/dl.acm.org/doi/abs/10.1145/3078971.3078992) with which SIMD instructions are
-used to perform 16 inner product operations in a single instruction. ## Class
+need to build `fast_pq` before you can run it, as it contains Cython code. The
+easiest way to do this is to simply run ```bash $ pip install . ``` To test it
+we can run an example: ```bash $ python -m examples.example n=16000, d=128,
+queries=1000, dims_per_block=2 Sampling Computing true neighbours Fitting PQ
+Querying Median place of true nearest neighbor: 1.0 90% quantile: 19.0 Queries/
+second: 7101.262693814528 Total time spent on preprocess: 0.09025406837463379
+Total time spent on search: 0.05056595802307129 Scipy speed for comparison:
+2.249645948410034 ``` In this example Fast PQ is about 16 times faster than
+optmized scipy/numpy. The reason is that Fast PQ uses a trick called
+[Accelerated Nearest Neighbor Search with Qick ADC](https://dl.acm.org/doi/abs/
+10.1145/3078971.3078992) with which SIMD instructions are used to perform 16
+inner product operations in a single instruction. ### Developing If you are
+helping develop fast_pq, and need to test a change to the Cython code, you can
+rebuild it with ```bash $ python setup.py build_ext --inplace ``` ## Class
 Overview The project consists of two main classes: IVF and FastPQ. The IVF
 class is used to build an IVF index with cluster centers, fit a product
 quantizer on the data, and perform queries on the index. The FastPQ class is
 used to create a product quantizer that can quickly transform data and compute
 distance tables. IVF: This class is responsible for creating an IVF index using
 clustering (either Euclidean or angular) and FastPQ for quantization. It
 provides methods to fit the index on data, build the index with quantized data,
```

### Comparing `fast_pq-0.2/pyproject.toml` & `fast_pq-0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fast_pq"
-version = "0.2"
+version = "0.3"
 description = "Approximate Nearest Neighbors in Python."
 authors = [
     {name="Thomas Dybdahl Ahle", email="lobais@gmail.com"}
 ]
 license = {text = "AGPL-3.0-or-later"}
 #license-file = "LICENSE"
 readme = "README.md"
```

### Comparing `fast_pq-0.2/setup.py` & `fast_pq-0.3/setup.py`

 * *Files identical despite different names*

### Comparing `fast_pq-0.2/tests/test_heap.py` & `fast_pq-0.3/tests/test_heap.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import heapq
 
 np.random.seed(10)
 
 from fast_pq._fast_pq import estimate_pq_sse
 from fast_pq._fast_pq import insert, init_heap
 
+
 class Heap:
     def __init__(self, size):
         self.indices = np.empty((size,), dtype=np.int64)
         self.vals = np.empty((size,), dtype=np.int32)
         init_heap(self.indices, self.vals, signd=True)
 
     def insert(self, i, v):
@@ -53,15 +54,15 @@
 def test_random():
     heap = Heap(10)
     pyheap = [(-127, -1)] * 10
     for t in range(1000):
         top_pyheap = -pyheap[0][0]
         assert top_pyheap == heap.peek()
 
-        v = np.random.randint(10000 // (t+1))
+        v = np.random.randint(10000 // (t + 1))
         heap.insert(t, v)
         if v < top_pyheap:
             heapq.heappop(pyheap)
             heapq.heappush(pyheap, (-v, t))
         assert set(heap.vals) == set(-vi for vi, _ in pyheap)
```

### Comparing `fast_pq-0.2/tests/test_ivf.py` & `fast_pq-0.3/tests/test_ivf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 
 from fast_pq import FastPQ, DummyPQ
-from fast_pq import IVF, cdist, brute
+from fast_pq import IVF, cdist, brute, group_data_by_indices
 
 
 def test_cdist():
     n1, n2, d = 10, 8, 5
     np.random.seed(10)
     for chunk in [1, 10, 100]:
         X = np.random.randn(n1, d)
@@ -44,15 +44,15 @@
 def test_small_n():
     d = 10
     for metric in ["euclidean", "angular"]:
         for n in range(1, 5):
             X = np.random.randn(n, d).astype(np.float32)
             q = np.random.randn(d).astype(np.float32)
             ivf = IVF(metric, 1, FastPQ(2))
-            ivf.fit(X).build(X,n_probes=1)
+            ivf.fit(X).build(X, n_probes=1)
             res = ivf.query(q, n)
             print(res)
             assert all(0 <= i < n for i in res)
 
 
 def test_far_small_n():
     d = 10
@@ -100,7 +100,32 @@
     return recall_at / nq / at
 
 
 @pytest.mark.filterwarnings("ignore:Number of distinct clusters")
 def test_small():
     np.random.seed(10)
     assert _test_recall_inner(15, 10, 30, 2, 10, "euclidean", 1) > 0.05
+
+
+def test_group_data_by_indices():
+    N, d, c, k = 100, 5, 6, 3
+    X = np.random.rand(N, d)
+    Q = np.random.randn(c, d)
+    indices = np.argpartition(-X @ Q.T, k, axis=1)[:, :k]
+
+    # Using the group_data_by_indices function
+    parts, _ = group_data_by_indices(X, indices, c)
+
+    # Using the alternative method with masks
+    mask_parts = []
+    for i in range(c):
+        mask = np.any(indices == i, axis=1)
+        mask_parts.append(X[mask])
+
+    # Compare the results
+    for i in range(c):
+        # Sort so we can compare
+        A = parts[i]
+        sorted_A = A[np.lexsort(A.T), :]
+        B = mask_parts[i]
+        sorted_B = B[np.lexsort(B.T), :]
+        np.testing.assert_allclose(sorted_A, sorted_B)
```

### Comparing `fast_pq-0.2/tests/test_multiprobe.py` & `fast_pq-0.3/tests/test_multiprobe.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,48 +8,51 @@
 nq = 30
 at = 10
 dpb = 2
 
 X = np.random.randn(n, d).astype(np.float32)
 qs = np.random.randn(nq, d).astype(np.float32)
 
+
 def compute_recall(metric, build_probes, query_probes):
     if at < n:
         trus = brute(qs, X, k=at, metric=metric)
     else:
         trus = np.broadcast_to(np.arange(n), (nq, n))
     ivf = IVF(metric, int(n**0.5), FastPQ(2))
     ivf.fit(X).build(X, n_probes=build_probes)
     recall_at = 0
     for q, tru in zip(qs, trus):
         guess = ivf.query(q, k=at, n_probes=query_probes)
         recall_at += len(set(guess) & set(tru))
     return recall_at / nq / at
 
+
 def _test_monotone(metric):
     n = 4
     table = []
-    for build_probes in range(1, n+1):
+    for build_probes in range(1, n + 1):
         table.append([])
-        for query_probes in range(1, n+1):
+        for query_probes in range(1, n + 1):
             recall = compute_recall(metric, build_probes, query_probes)
             table[-1].append(recall)
 
     for row in table:
         print(row)
 
     # Test rows monotone
     for i in range(1, n):
         for j in range(n):
-            assert table[i][j] >= table[i-1][j] - 0.1
+            assert table[i][j] >= table[i - 1][j] - 0.1
 
     # Test cols monotone
     for i in range(n):
         for j in range(1, n):
-            assert table[i][j] >= table[i][j-1] - 0.1
+            assert table[i][j] >= table[i][j - 1] - 0.1
+
 
 def test_euclidean():
     _test_monotone("euclidean")
 
+
 def test_angular():
     _test_monotone("angular")
-
```

### Comparing `fast_pq-0.2/tests/test_pq.py` & `fast_pq-0.3/tests/test_pq.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 import numpy as np
 import pytest
+from itertools import product
 
 from fast_pq._fast_pq import estimate_pq_sse, query_pq_sse, init_heap
 from fast_pq import FastPQ, cdist
 
+np.random.seed(10)
 
-def test_recall():
-    np.random.seed(10)
-    for i in range(1, 5):
-        for method in ["argpartition", "top"]:
-            n = np.random.randint(16 * i, 16 * (i + 1))
-            recall_at_10 = _test_recall_inner(n, 8 * i, 100, 2, method)
-            assert recall_at_10 > 0.8
 
+@pytest.mark.parametrize(
+    "i, method, signed", product(range(1, 5), ["argpartition", "top"], [True, False])
+)
+def test_recall(i, method, signed):
+    n = np.random.randint(16 * i, 16 * (i + 1))
+    _test_recall_inner(n, 8 * i, 100, 2, method, signed)
 
-def _test_recall_inner(n, d, k, dpb, method):
+
+def _test_recall_inner(n, d, k, dpb, method, signed):
     X = np.random.randn(n, d).astype(np.float32)
     qs = np.random.randn(k, d).astype(np.float32)
     trus = cdist(qs, X).argmin(axis=1)
 
     pq = FastPQ(dims_per_block=dpb)
     data = pq.fit_transform(X)
     recall_at_10 = 0
     for q, tru in zip(qs, trus):
-        dtable = pq.distance_table(q)
+        dtable = pq.distance_table(q) if signed else pq.udistance_table(q)
         if method == "argpartition":
             top10 = dtable.estimate_distances(data).argpartition(10)[:10]
         elif method == "top":
             top10, _ = dtable.top(data, X, 10)
         if tru in top10:
             recall_at_10 += 1
-    return recall_at_10 / k
+    recall_at_10 /= k
+    assert recall_at_10 > 0.8
 
 
 @pytest.mark.filterwarnings("ignore:Number of distinct clusters")
-def test_topk():
-    np.random.seed(11)
-    for n in tuple(range(1, 10)) + (20, 30, 50):
-        for dpb in [1, 2]:
-            for signed in [True, False]:
-                _test_topk_inner(n, 3, 11, dpb, signed)
+@pytest.mark.parametrize(
+    "n, dpb, signed", product(tuple(range(1, 10)) + (20, 30, 50), [1, 2], [True, False])
+)
+def test_topk(n, dpb, signed):
+    _test_topk_inner(n, 3, 11, dpb, signed)
 
 
 @pytest.mark.filterwarnings("ignore:Number of distinct clusters")
-def test_topk_0():
-    np.random.seed(11)
-    for signed in [True, False]:
-        with pytest.raises(AssertionError):
-            _test_topk_inner(0, 3, 11, 2, signed)
+@pytest.mark.parametrize("signed", [True, False])
+def test_topk_0(signed):
+    with pytest.raises(AssertionError):
+        _test_topk_inner(0, 3, 11, 2, signed)
 
 
 def test_fit_transform():
-    np.random.seed(11)
     n, d = 100, 10
     X = np.random.randn(n, d).astype(np.float32)
 
     pq = FastPQ(2)
     n0, tdata0 = pq.fit_transform(X)
     n1, tdata1 = pq.transform(X)
     assert n0 == n1
@@ -70,15 +70,15 @@
 
     for q in qs:
         dtable = pq.distance_table(q)
 
         out = np.zeros(2 * len(data), dtype=np.uint64)
         estimate_pq_sse(data, dtable.tables, out, signed)
         est = out.view(np.int8 if signed else np.uint8)
-        est = est[:n] # Remove padding
+        est = est[:n]  # Remove padding
 
         k = n
         indices = np.zeros((k,), dtype=np.int64)
         values = np.zeros((k,), dtype=np.int32)
         init_heap(indices, values, signed)
         query_pq_sse(data, n, dtable.tables, indices, values, signed)
 
@@ -106,8 +106,7 @@
     indices = np.empty((k,), dtype=np.int64)
     values = np.empty((k,), dtype=np.int32)
     labels = np.arange(n, dtype=np.int64) + 10**12
     init_heap(indices, values, True)
     query_pq_sse(data, n, dtable.tables, indices, values, True, labels)
     indices.sort()
     np.testing.assert_array_equal(indices, labels)
-
```

### Comparing `fast_pq-0.2/tests/test_transform.py` & `fast_pq-0.3/tests/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 
 def _test_rand_inner_unsigned(n, d):
     dat = [[random.randrange(16) for _ in range(d)] for _ in range(n)]
     # We saturate at 255, so no reason to have numbers much bigger than 1/d of that.
     tab = [[random.randrange(256 // d * 2) for _ in range(16)] for _ in range(d)]
     expected = np.array([sum(tab[j][dat[i][j]] for j in range(d)) for i in range(n)])
     expected = np.minimum(expected, 255)
-    out = _slow_pq(np.array(dat).astype(np.uint8), np.array(tab).astype(np.uint8), False)
+    out = _slow_pq(
+        np.array(dat).astype(np.uint8), np.array(tab).astype(np.uint8), False
+    )
     assert np.all(expected == out)
 
 
 def sat8_add(x, y):
     if x + y > 127:
         return 127
     if x + y < -128:
@@ -69,8 +71,7 @@
 def test_unpack():
     np.random.seed(10)
     n, d = 16 * 13, 2 * 7
     data = np.random.randint(16, size=(n, d)).astype(np.uint8)
     t_data = transform_data(data)
     data1 = unpack(t_data)
     np.testing.assert_array_equal(data, data1)
-
```

