# Comparing `tmp/Seq2SeqSharp-2.7.3.tar.gz` & `tmp/Seq2SeqSharp-2.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Seq2SeqSharp-2.7.3.tar", last modified: Wed Apr 19 08:01:05 2023, max compression
+gzip compressed data, was "Seq2SeqSharp-2.7.4.tar", last modified: Wed Apr 19 08:11:46 2023, max compression
```

## Comparing `Seq2SeqSharp-2.7.3.tar` & `Seq2SeqSharp-2.7.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        0 2023-04-19 08:01:05.907730 Seq2SeqSharp-2.7.3/
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)     1512 2023-04-19 03:18:59.000000 Seq2SeqSharp-2.7.3/LICENSE
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      687 2023-04-19 08:01:05.907730 Seq2SeqSharp-2.7.3/PKG-INFO
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    47511 2023-04-19 03:19:22.000000 Seq2SeqSharp-2.7.3/README.md
-drwxr-xr-x   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        0 2023-04-19 08:01:05.903730 Seq2SeqSharp-2.7.3/Seq2SeqSharp/
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    27648 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/AdvUtils.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    21712 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/AdvUtils.pdb
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   129536 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/CudaBlas.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    33384 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/CudaBlas.pdb
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    16896 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/CudaRand.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    14572 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/CudaRand.pdb
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)  1324032 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/ManagedCuda.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   730264 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/ManagedCuda.pdb
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    27264 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Caching.Abstractions.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    38016 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Caching.Memory.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    43632 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    62064 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Logging.Abstractions.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    59008 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Options.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    40048 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Primitives.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    11264 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/NVRTC.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    12972 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/NVRTC.pdb
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   695336 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Newtonsoft.Json.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   252416 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Seq2SeqSharp.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      427 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Seq2SeqSharp.dll.config
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   103972 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/Seq2SeqSharp.pdb
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   317440 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.CUDA.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      513 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.CUDA.dll.config
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    54796 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.CUDA.pdb
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   140288 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    62060 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.pdb
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      653 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/__init__.py
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   262656 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/protobuf-net.Core.dll
--rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   259584 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp/protobuf-net.dll
-drwxr-xr-x   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        0 2023-04-19 08:01:05.907730 Seq2SeqSharp-2.7.3/Seq2SeqSharp.egg-info/
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      687 2023-04-19 08:01:05.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp.egg-info/PKG-INFO
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)     1203 2023-04-19 08:01:05.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp.egg-info/SOURCES.txt
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        1 2023-04-19 08:01:05.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp.egg-info/dependency_links.txt
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)       17 2023-04-19 08:01:05.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp.egg-info/requires.txt
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)       13 2023-04-19 08:01:05.000000 Seq2SeqSharp-2.7.3/Seq2SeqSharp.egg-info/top_level.txt
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)       38 2023-04-19 08:01:05.907730 Seq2SeqSharp-2.7.3/setup.cfg
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)     1904 2023-04-19 08:00:54.000000 Seq2SeqSharp-2.7.3/setup.py
-drwxr-xr-x   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        0 2023-04-19 08:01:05.907730 Seq2SeqSharp-2.7.3/tests/
--rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      655 2023-04-19 02:50:57.000000 Seq2SeqSharp-2.7.3/tests/test.py
+drwxr-xr-x   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        0 2023-04-19 08:11:46.049080 Seq2SeqSharp-2.7.4/
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)     1512 2023-04-19 03:18:59.000000 Seq2SeqSharp-2.7.4/LICENSE
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    48239 2023-04-19 08:11:46.049080 Seq2SeqSharp-2.7.4/PKG-INFO
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    47511 2023-04-19 03:19:22.000000 Seq2SeqSharp-2.7.4/README.md
+drwxr-xr-x   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        0 2023-04-19 08:11:46.045080 Seq2SeqSharp-2.7.4/Seq2SeqSharp/
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    27648 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/AdvUtils.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    21712 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/AdvUtils.pdb
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   129536 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/CudaBlas.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    33384 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/CudaBlas.pdb
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    16896 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/CudaRand.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    14572 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/CudaRand.pdb
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)  1324032 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/ManagedCuda.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   730264 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/ManagedCuda.pdb
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    27264 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Caching.Abstractions.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    38016 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Caching.Memory.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    43632 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    62064 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Logging.Abstractions.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    59008 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Options.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    40048 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Primitives.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    11264 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/NVRTC.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    12972 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/NVRTC.pdb
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   695336 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Newtonsoft.Json.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   252416 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Seq2SeqSharp.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      427 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Seq2SeqSharp.dll.config
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   103972 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/Seq2SeqSharp.pdb
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   317440 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.CUDA.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      513 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.CUDA.dll.config
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    54796 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.CUDA.pdb
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   140288 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    62060 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.pdb
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      543 2023-04-19 08:09:30.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/__init__.py
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   262656 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/protobuf-net.Core.dll
+-rwxr-x---   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)   259584 2023-04-19 07:20:59.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp/protobuf-net.dll
+drwxr-xr-x   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        0 2023-04-19 08:11:46.045080 Seq2SeqSharp-2.7.4/Seq2SeqSharp.egg-info/
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)    48239 2023-04-19 08:11:46.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp.egg-info/PKG-INFO
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)     1203 2023-04-19 08:11:46.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp.egg-info/SOURCES.txt
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        1 2023-04-19 08:11:46.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp.egg-info/dependency_links.txt
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)       17 2023-04-19 08:11:46.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp.egg-info/requires.txt
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)       13 2023-04-19 08:11:46.000000 Seq2SeqSharp-2.7.4/Seq2SeqSharp.egg-info/top_level.txt
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)       38 2023-04-19 08:11:46.049080 Seq2SeqSharp-2.7.4/setup.cfg
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)     2063 2023-04-19 08:11:31.000000 Seq2SeqSharp-2.7.4/setup.py
+drwxr-xr-x   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)        0 2023-04-19 08:11:46.045080 Seq2SeqSharp-2.7.4/tests/
+-rw-r--r--   0 REDMOND.zhongfu (515443620) REDMOND.domain users (500000513)      655 2023-04-19 02:50:57.000000 Seq2SeqSharp-2.7.4/tests/test.py
```

### Comparing `Seq2SeqSharp-2.7.3/LICENSE` & `Seq2SeqSharp-2.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/README.md` & `Seq2SeqSharp-2.7.4/README.md`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/AdvUtils.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/AdvUtils.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/AdvUtils.pdb` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/AdvUtils.pdb`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/CudaBlas.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/CudaBlas.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/CudaBlas.pdb` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/CudaBlas.pdb`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/CudaRand.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/CudaRand.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/CudaRand.pdb` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/CudaRand.pdb`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/ManagedCuda.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/ManagedCuda.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/ManagedCuda.pdb` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/ManagedCuda.pdb`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Caching.Abstractions.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Caching.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Caching.Memory.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Caching.Memory.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Logging.Abstractions.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Options.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Microsoft.Extensions.Primitives.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/NVRTC.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/NVRTC.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/NVRTC.pdb` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/NVRTC.pdb`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Newtonsoft.Json.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Seq2SeqSharp.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Seq2SeqSharp.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/Seq2SeqSharp.pdb` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/Seq2SeqSharp.pdb`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.CUDA.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.CUDA.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.CUDA.dll.config` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.CUDA.dll.config`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.CUDA.pdb` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.CUDA.pdb`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/TensorSharp.pdb` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/TensorSharp.pdb`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/protobuf-net.Core.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/protobuf-net.Core.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp/protobuf-net.dll` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp/protobuf-net.dll`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/Seq2SeqSharp.egg-info/SOURCES.txt` & `Seq2SeqSharp-2.7.4/Seq2SeqSharp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Seq2SeqSharp-2.7.3/setup.py` & `Seq2SeqSharp-2.7.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from setuptools import setup
 
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
 setup(
     name='Seq2SeqSharp',
-    version='2.7.3',
+    version='2.7.4',
     author='Zhongkai Fu',
     author_email='fuzhongkai@gmail.com',
     description='Seq2SeqSharp is a tensor based fast & flexible encoder-decoder deep neural network framework written by .NET (C#). It has many highlighted features, such as automatic differentiation, many different types of encoders/decoders(Transformer, LSTM, BiLSTM and so on), multi-GPUs supported, cross-platforms (Windows, Linux, x86, x64, ARM) and so on.',
     url='https://github.com/zhongkaifu/Seq2SeqSharp',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     packages=['Seq2SeqSharp'],
     install_requires=['pythonnet>=3.0.1'],
```

### Comparing `Seq2SeqSharp-2.7.3/tests/test.py` & `Seq2SeqSharp-2.7.4/tests/test.py`

 * *Files identical despite different names*

