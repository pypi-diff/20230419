# Comparing `tmp/eQTac-1.0.2.tar.gz` & `tmp/eQTac-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eQTac-1.0.2.tar", last modified: Wed Apr 19 07:25:18 2023, max compression
+gzip compressed data, was "eQTac-1.0.3.tar", last modified: Wed Apr 19 07:50:30 2023, max compression
```

## Comparing `eQTac-1.0.2.tar` & `eQTac-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 07:25:18.406832 eQTac-1.0.2/
--rw-rw-rw-   0        0        0     3877 2023-04-19 07:25:18.403815 eQTac-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3428 2023-04-19 06:43:03.000000 eQTac-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 07:25:18.386859 eQTac-1.0.2/eQTac.egg-info/
--rw-rw-rw-   0        0        0     3877 2023-04-19 07:25:18.000000 eQTac-1.0.2/eQTac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-19 07:25:18.000000 eQTac-1.0.2/eQTac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:25:18.000000 eQTac-1.0.2/eQTac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-19 07:25:18.000000 eQTac-1.0.2/eQTac.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 07:25:18.000000 eQTac-1.0.2/eQTac.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 07:25:18.410823 eQTac-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      769 2023-04-19 07:25:00.000000 eQTac-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:50:30.259463 eQTac-1.0.3/
+-rw-rw-rw-   0        0        0     1539 2023-04-19 07:30:51.000000 eQTac-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0       17 2023-04-19 07:47:38.000000 eQTac-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3900 2023-04-19 07:50:30.257470 eQTac-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3428 2023-04-19 06:43:03.000000 eQTac-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 07:50:30.151752 eQTac-1.0.3/eQTac/
+-rw-rw-rw-   0        0        0     1860 2023-04-18 09:28:48.000000 eQTac-1.0.3/eQTac/control_FDR.py
+-rw-rw-rw-   0        0        0     4343 2023-04-17 11:42:17.000000 eQTac-1.0.3/eQTac/eQTac_correlation.py
+-rw-rw-rw-   0        0        0     2260 2023-04-17 11:42:17.000000 eQTac-1.0.3/eQTac/eQTac_permutation.py
+-rw-rw-rw-   0        0        0     2644 2023-04-17 11:42:17.000000 eQTac-1.0.3/eQTac/filter_bkg.py
+-rw-rw-rw-   0        0        0     4744 2023-04-17 11:42:17.000000 eQTac-1.0.3/eQTac/generate_PRE.py
+-rw-rw-rw-   0        0        0     2594 2023-04-17 11:42:17.000000 eQTac-1.0.3/eQTac/generate_mut_fa.py
+-rw-rw-rw-   0        0        0      910 2023-04-17 11:42:17.000000 eQTac-1.0.3/eQTac/generate_snp_dict.py
+-rw-rw-rw-   0        0        0     3832 2023-04-17 11:42:17.000000 eQTac-1.0.3/eQTac/geno2score.py
+-rw-rw-rw-   0        0        0     2480 2023-04-17 11:42:17.000000 eQTac-1.0.3/eQTac/get_nullseq.py
+drwxrwxrwx   0        0        0        0 2023-04-19 07:50:30.241541 eQTac-1.0.3/eQTac.egg-info/
+-rw-rw-rw-   0        0        0     3900 2023-04-19 07:50:29.000000 eQTac-1.0.3/eQTac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-19 07:50:30.000000 eQTac-1.0.3/eQTac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:50:29.000000 eQTac-1.0.3/eQTac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-04-19 07:50:29.000000 eQTac-1.0.3/eQTac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 07:50:29.000000 eQTac-1.0.3/eQTac.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 07:50:30.262455 eQTac-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-04-19 07:48:50.000000 eQTac-1.0.3/setup.py
```

### Comparing `eQTac-1.0.2/PKG-INFO` & `eQTac-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.2
+Version: 1.0.3
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8.3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # eQTac
 ---
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Dependence
 ### Python packages
 ```
```

### Comparing `eQTac-1.0.2/README.md` & `eQTac-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `eQTac-1.0.2/eQTac.egg-info/PKG-INFO` & `eQTac-1.0.3/eQTac.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: eQTac
-Version: 1.0.2
+Version: 1.0.3
 Summary: The eQTac method.
 Home-page: https://github.com/JFF1594032292/eQTac
 Author: Jiang Feng
 Author-email: 1594032292@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8.3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # eQTac
 ---
 EQTac is a method to predict the potential regulatory elements (PREs) and their target genes, based on the eQTL datasets, The only additional data was ATAC-seq or ChIP-seq peak data. 
 ## Dependence
 ### Python packages
 ```
```

### Comparing `eQTac-1.0.2/setup.py` & `eQTac-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f1:
     long_description = f1.read()
 
 setuptools.setup(
     name="eQTac",
-    version="1.0.2",
+    version="1.0.3",
     author="Jiang Feng",
     author_email="1594032292@qq.com",
     description="The eQTac method.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JFF1594032292/eQTac",
     packages=setuptools.find_packages(),
```

