# Comparing `tmp/multiPrime-2.3.9.tar.gz` & `tmp/multiPrime-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.3.9.tar", last modified: Fri Apr 14 05:17:30 2023, max compression
+gzip compressed data, was "multiPrime-2.4.1.tar", last modified: Wed Apr 19 07:57:44 2023, max compression
```

## Comparing `multiPrime-2.3.9.tar` & `multiPrime-2.4.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-14 05:17:30.014961 multiPrime-2.3.9/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-02-16 10:00:29.000000 multiPrime-2.3.9/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12953 2023-04-14 05:17:30.014961 multiPrime-2.3.9/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12800 2023-04-14 05:12:54.000000 multiPrime-2.3.9/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-14 05:17:29.575922 multiPrime-2.3.9/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    12953 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-14 05:17:26.000000 multiPrime-2.3.9/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-14 05:17:30.014961 multiPrime-2.3.9/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-02-16 10:00:57.000000 multiPrime-2.3.9/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-14 05:17:30.013960 multiPrime-2.3.9/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-02-16 10:00:29.000000 multiPrime-2.3.9/src/__init__.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-14 05:17:21.000000 multiPrime-2.3.9/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-13 01:45:21.000000 multiPrime-2.3.9/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    84525 2023-04-13 01:45:21.000000 multiPrime-2.3.9/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    24918 2023-04-13 01:45:21.000000 multiPrime-2.3.9/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 07:57:44.588568 multiPrime-2.4.1/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-04-19 07:54:42.000000 multiPrime-2.4.1/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    15921 2023-04-19 07:57:44.588568 multiPrime-2.4.1/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    15768 2023-04-19 07:54:42.000000 multiPrime-2.4.1/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 07:57:44.586568 multiPrime-2.4.1/multiPrime/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-04-19 07:57:18.000000 multiPrime-2.4.1/multiPrime/__init__.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 07:57:44.587568 multiPrime-2.4.1/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    15921 2023-04-19 07:57:43.000000 multiPrime-2.4.1/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      274 2023-04-19 07:57:43.000000 multiPrime-2.4.1/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-19 07:57:43.000000 multiPrime-2.4.1/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-19 07:57:43.000000 multiPrime-2.4.1/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-19 07:57:43.000000 multiPrime-2.4.1/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-19 07:57:44.588568 multiPrime-2.4.1/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1798 2023-04-19 07:54:42.000000 multiPrime-2.4.1/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 07:57:44.587568 multiPrime-2.4.1/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-19 07:57:28.000000 multiPrime-2.4.1/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-19 07:54:42.000000 multiPrime-2.4.1/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    85987 2023-04-19 07:54:42.000000 multiPrime-2.4.1/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    25219 2023-04-19 07:54:42.000000 multiPrime-2.4.1/src/utils.py
```

### Comparing `multiPrime-2.3.9/LICENSE` & `multiPrime-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.9/PKG-INFO` & `multiPrime-2.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.9
+Version: 2.4.1
 License: MIT
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
 
 `multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
 It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).` 
@@ -38,28 +38,28 @@
 | Errors        | Extract primer-contained sequences with errors.             |
 ```
 multiPrime DPrime -i input -o output
            Options: { -l [18] -n [4] -d [10] -v [1] -g [0.2,0.7] -f [0.8] -c [4] -p [10] -a [4] }
 ```
 Parameters：
 
-| Parameters      | Description                                                                                                                                                                                                                                                                              |
-|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| -i/--input      | Input file: Result of multi-alignment. (muscle, mafft or others)                                                                                                                                                                                                                         |
-| -l/--plen       | Length of primer. Default: 18                                                                                                                                                                                                                                                            |
-| -n/--dnum       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                        |
-| -v/--variation  | Max mismatch number of primer. Default: 1.                                                                                                                                                                                                                                               |
-| -e/--entropy    | Entropy is actually a measure of disorder. This parameter is used to judge whether the window is conservation. Entropy of primer-length window. Default: 3.6.                                                                                                                            |
-| -g/--gc         | Filter primers by GC content. Default [0.2,0.7].                                                                                                                                                                                                                                         |
-| -s/--size       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                        |
-| -f/--fraction   | Filter primers by match fraction (Coverage with errors). Default: 0.8.                                                                                                                                                                                                                   |
-| -c/--coordinate | Mismatch index is not allowed to locate in start or stop. otherwise, it won't be regard as the mis-coverage. With this param, you can control the index of Y-distance (number=variation and position of mismatch) when calculate coverage with error.Default: 4.                         |
-| -p/--proc       | Number of process to launch. Default: 20.                                                                                                                                                                                                                                                |
-| -a/--away       | Filter hairpin structure, which means distance of the minimal paired bases. Default: 4. Example:(number of X) AGCT[XXXX]AGCT. Primers should not have complementary sequences (no consecutive 4 bp complementarities),otherwise the primers themselves will fold into hairpin structure. |
-| -o/--out        | Output file: candidate primers. e.g.  [*].candidate.primers.out.                                                                                                                                                                                                                         |
+| Parameters      | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| -i/--input      | Input file: Result of multi-alignment. (muscle, mafft or others)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| -l/--plen       | Length of primer. Default: 18                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+| -n/--dnum       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| -v/--variation  | Max mismatch number of primer. Default: 1.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| -e/--entropy    | Entropy is actually a measure of disorder. This parameter is used to judge whether the window is conservation. Entropy of primer-length window. Default: 3.6.                                                                                                                                                                                                                                                                                                                                                |
+| -g/--gc         | Filter primers by GC content. Default [0.2,0.7].                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| -s/--size       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| -f/--fraction   | Filter primers by match fraction (Coverage with errors). Default: 0.8.                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| -c/--coordinate | Mismatch index is not allowed to locate in your specific positions. otherwise, it won't be regard as the mis-coverage. With this param, you can control the index of Y-distance (number=variation and position of mismatch). when calculate coverage with error. coordinate>0: 5'==>3'; coordinate<0: 3'==>5'. You can set this param to any value that you prefer. Default: 1,-1. 1:  I dont want mismatch at the 2nd position, start from 0. -1: I dont want mismatch at the -1st position, start from -1. |
+| -p/--proc       | Number of process to launch. Default: 20.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| -a/--away       | Filter hairpin structure, which means distance of the minimal paired bases. Default: 4. Example:(number of X) AGCT[XXXX]AGCT. Primers should not have complementary sequences (no consecutive 4 bp complementarities),otherwise the primers themselves will fold into hairpin structure.                                                                                                                                                                                                                     |
+| -o/--out        | Output file: candidate primers. e.g.  [*].candidate.primers.out.                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 ```
 multiPrime Ppair -i input -r reference -o output
            Options: {-f [0.6] -m [500] -n [200] -e [4] -p [9] -s [250,500] -g [0.4,0.6] -d [4] -a ","}
 ```
 Parameters：
 
 | Parameters    | Description                                                                                                                                                                                                         |
```

### Comparing `multiPrime-2.3.9/README.md` & `multiPrime-2.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -30,28 +30,28 @@
 | Errors        | Extract primer-contained sequences with errors.             |
 ```
 multiPrime DPrime -i input -o output
            Options: { -l [18] -n [4] -d [10] -v [1] -g [0.2,0.7] -f [0.8] -c [4] -p [10] -a [4] }
 ```
 Parameters：
 
-| Parameters      | Description                                                                                                                                                                                                                                                                              |
-|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| -i/--input      | Input file: Result of multi-alignment. (muscle, mafft or others)                                                                                                                                                                                                                         |
-| -l/--plen       | Length of primer. Default: 18                                                                                                                                                                                                                                                            |
-| -n/--dnum       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                        |
-| -v/--variation  | Max mismatch number of primer. Default: 1.                                                                                                                                                                                                                                               |
-| -e/--entropy    | Entropy is actually a measure of disorder. This parameter is used to judge whether the window is conservation. Entropy of primer-length window. Default: 3.6.                                                                                                                            |
-| -g/--gc         | Filter primers by GC content. Default [0.2,0.7].                                                                                                                                                                                                                                         |
-| -s/--size       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                        |
-| -f/--fraction   | Filter primers by match fraction (Coverage with errors). Default: 0.8.                                                                                                                                                                                                                   |
-| -c/--coordinate | Mismatch index is not allowed to locate in start or stop. otherwise, it won't be regard as the mis-coverage. With this param, you can control the index of Y-distance (number=variation and position of mismatch) when calculate coverage with error.Default: 4.                         |
-| -p/--proc       | Number of process to launch. Default: 20.                                                                                                                                                                                                                                                |
-| -a/--away       | Filter hairpin structure, which means distance of the minimal paired bases. Default: 4. Example:(number of X) AGCT[XXXX]AGCT. Primers should not have complementary sequences (no consecutive 4 bp complementarities),otherwise the primers themselves will fold into hairpin structure. |
-| -o/--out        | Output file: candidate primers. e.g.  [*].candidate.primers.out.                                                                                                                                                                                                                         |
+| Parameters      | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| -i/--input      | Input file: Result of multi-alignment. (muscle, mafft or others)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| -l/--plen       | Length of primer. Default: 18                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+| -n/--dnum       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| -v/--variation  | Max mismatch number of primer. Default: 1.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| -e/--entropy    | Entropy is actually a measure of disorder. This parameter is used to judge whether the window is conservation. Entropy of primer-length window. Default: 3.6.                                                                                                                                                                                                                                                                                                                                                |
+| -g/--gc         | Filter primers by GC content. Default [0.2,0.7].                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| -s/--size       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| -f/--fraction   | Filter primers by match fraction (Coverage with errors). Default: 0.8.                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| -c/--coordinate | Mismatch index is not allowed to locate in your specific positions. otherwise, it won't be regard as the mis-coverage. With this param, you can control the index of Y-distance (number=variation and position of mismatch). when calculate coverage with error. coordinate>0: 5'==>3'; coordinate<0: 3'==>5'. You can set this param to any value that you prefer. Default: 1,-1. 1:  I dont want mismatch at the 2nd position, start from 0. -1: I dont want mismatch at the -1st position, start from -1. |
+| -p/--proc       | Number of process to launch. Default: 20.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| -a/--away       | Filter hairpin structure, which means distance of the minimal paired bases. Default: 4. Example:(number of X) AGCT[XXXX]AGCT. Primers should not have complementary sequences (no consecutive 4 bp complementarities),otherwise the primers themselves will fold into hairpin structure.                                                                                                                                                                                                                     |
+| -o/--out        | Output file: candidate primers. e.g.  [*].candidate.primers.out.                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 ```
 multiPrime Ppair -i input -r reference -o output
            Options: {-f [0.6] -m [500] -n [200] -e [4] -p [9] -s [250,500] -g [0.4,0.6] -d [4] -a ","}
 ```
 Parameters：
 
 | Parameters    | Description                                                                                                                                                                                                         |
```

### Comparing `multiPrime-2.3.9/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.4.1/multiPrime.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.3.9
+Version: 2.4.1
 License: MIT
-Requires-Python: >=3.9
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
 
 `multiPrime is an error-tolerant primer design tool for broad-spectrum pathogens detection. 
 It proposes a solution for the maximal coverage degenerate primer design with error (MD-EDPD).` 
@@ -38,28 +38,28 @@
 | Errors        | Extract primer-contained sequences with errors.             |
 ```
 multiPrime DPrime -i input -o output
            Options: { -l [18] -n [4] -d [10] -v [1] -g [0.2,0.7] -f [0.8] -c [4] -p [10] -a [4] }
 ```
 Parameters：
 
-| Parameters      | Description                                                                                                                                                                                                                                                                              |
-|-----------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| -i/--input      | Input file: Result of multi-alignment. (muscle, mafft or others)                                                                                                                                                                                                                         |
-| -l/--plen       | Length of primer. Default: 18                                                                                                                                                                                                                                                            |
-| -n/--dnum       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                        |
-| -v/--variation  | Max mismatch number of primer. Default: 1.                                                                                                                                                                                                                                               |
-| -e/--entropy    | Entropy is actually a measure of disorder. This parameter is used to judge whether the window is conservation. Entropy of primer-length window. Default: 3.6.                                                                                                                            |
-| -g/--gc         | Filter primers by GC content. Default [0.2,0.7].                                                                                                                                                                                                                                         |
-| -s/--size       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                        |
-| -f/--fraction   | Filter primers by match fraction (Coverage with errors). Default: 0.8.                                                                                                                                                                                                                   |
-| -c/--coordinate | Mismatch index is not allowed to locate in start or stop. otherwise, it won't be regard as the mis-coverage. With this param, you can control the index of Y-distance (number=variation and position of mismatch) when calculate coverage with error.Default: 4.                         |
-| -p/--proc       | Number of process to launch. Default: 20.                                                                                                                                                                                                                                                |
-| -a/--away       | Filter hairpin structure, which means distance of the minimal paired bases. Default: 4. Example:(number of X) AGCT[XXXX]AGCT. Primers should not have complementary sequences (no consecutive 4 bp complementarities),otherwise the primers themselves will fold into hairpin structure. |
-| -o/--out        | Output file: candidate primers. e.g.  [*].candidate.primers.out.                                                                                                                                                                                                                         |
+| Parameters      | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
+|-----------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| -i/--input      | Input file: Result of multi-alignment. (muscle, mafft or others)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| -l/--plen       | Length of primer. Default: 18                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
+| -n/--dnum       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| -v/--variation  | Max mismatch number of primer. Default: 1.                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+| -e/--entropy    | Entropy is actually a measure of disorder. This parameter is used to judge whether the window is conservation. Entropy of primer-length window. Default: 3.6.                                                                                                                                                                                                                                                                                                                                                |
+| -g/--gc         | Filter primers by GC content. Default [0.2,0.7].                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| -s/--size       | Number of degenerate. Default: 4.                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| -f/--fraction   | Filter primers by match fraction (Coverage with errors). Default: 0.8.                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| -c/--coordinate | Mismatch index is not allowed to locate in your specific positions. otherwise, it won't be regard as the mis-coverage. With this param, you can control the index of Y-distance (number=variation and position of mismatch). when calculate coverage with error. coordinate>0: 5'==>3'; coordinate<0: 3'==>5'. You can set this param to any value that you prefer. Default: 1,-1. 1:  I dont want mismatch at the 2nd position, start from 0. -1: I dont want mismatch at the -1st position, start from -1. |
+| -p/--proc       | Number of process to launch. Default: 20.                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| -a/--away       | Filter hairpin structure, which means distance of the minimal paired bases. Default: 4. Example:(number of X) AGCT[XXXX]AGCT. Primers should not have complementary sequences (no consecutive 4 bp complementarities),otherwise the primers themselves will fold into hairpin structure.                                                                                                                                                                                                                     |
+| -o/--out        | Output file: candidate primers. e.g.  [*].candidate.primers.out.                                                                                                                                                                                                                                                                                                                                                                                                                                             |
 ```
 multiPrime Ppair -i input -r reference -o output
            Options: {-f [0.6] -m [500] -n [200] -e [4] -p [9] -s [250,500] -g [0.4,0.6] -d [4] -a ","}
 ```
 Parameters：
 
 | Parameters    | Description                                                                                                                                                                                                         |
```

### Comparing `multiPrime-2.3.9/setup.py` & `multiPrime-2.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,32 +41,33 @@
 
 def getdes():
     des = ""
     with open(os.path.join(os.getcwd(), "README.md")) as fi:
         des = fi.read()
     return des
 
+
 def get_requirement():
     requires = []
     with open(os.path.join(os.path.dirname(__file__), "requirements.txt")) as fi:
         for line in fi:
             line = line.strip()
             requires.append(line)
     return requires
 
 
 setup(
     name=PKG,
     version=get_version(),
     packages=[PKG],
     license="MIT",
-    package_dir={PKG: "src"},
-    #install_requires=get_requirement(),
-    python_requires='>=3.9',
-    #ext_modules=getExtension(),
+    #package_dir={PKG: "src"},
+    # install_requires=get_requirement(),
+    python_requires='>=3.6',
+    ext_modules=getExtension(),
     long_description=getdes(),
     long_description_content_type='text/markdown',
     entry_points={
         'console_scripts': [
             '%s = %s.main:main' % (PKG, PKG),
         ]
     }
```

### Comparing `multiPrime-2.3.9/src/main.py` & `multiPrime-2.4.1/src/main.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.3.9/src/src.py` & `multiPrime-2.4.1/src/src.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,30 +13,34 @@
 from bisect import bisect_left
 from pathlib import Path
 import multiprocessing
 
 
 class NN_degenerate(object):
     def __init__(self, seq_file, primer_length=18, coverage=0.8, number_of_dege_bases=18, score_of_dege_bases=1000,
-                 product_len=250, position=4, variation=2, entropy_threshold=3.6, distance=4, GC="0.2,0.7", nproc=10,
-                 outfile=""):
+                 product_len=250, position="2,-1", variation=2, raw_entropy_threshold=3.6, distance=4, GC="0.4,0.6",
+                 nproc=10, outfile=""):
         self.primer_length = primer_length  # primer length
         self.coverage = coverage  # min coverage
         self.number_of_dege_bases = number_of_dege_bases
         self.score_of_dege_bases = score_of_dege_bases
         self.product = product_len
         self.position = position  # gap position
+        self.Y_strict, self.Y_strict_R = self.get_Y()
         self.variation = variation  # coverage of n-nt variation and max_gap_number
         self.distance = distance  # haripin
         self.GC = GC.split(",")
-        self.entropy_threshold = entropy_threshold
         self.nproc = nproc  # GC content
         self.seq_dict, self.total_sequence_number = self.parse_seq(seq_file)
-        self.start_position = self.seq_attribute(self.seq_dict)[0]
-        self.stop_position = self.seq_attribute(self.seq_dict)[1]
+        self.position_list = self.seq_attribute(self.seq_dict)
+        self.start_position = self.position_list[0]
+        self.stop_position = self.position_list[1]
+        self.length = self.position_list[2]
+        self.raw_entropy_threshold = raw_entropy_threshold
+        self.entropy_threshold = self.entropy_threshold_adjust(self.length)
         self.outfile = outfile
         self.resQ = Manager().Queue()
 
     # expand degenerate primer into a list.
     @staticmethod
     def degenerate_seq(primer):
         seq = []
@@ -165,16 +169,17 @@
 
     def deltaG(self, sequence):
         Delta_G_list = []
         Na = 50
         for seq in self.degenerate_seq(sequence):
             Delta_G = 0
             for n in range(len(seq) - 1):
-                i, j = base2bit[seq[n + 1]], base2bit[seq[n]]
-                Delta_G += freedom_of_H_37_table[i][j] * H_bonds_number[i][j] + penalty_of_H_37_table[i][j]
+                base_i, base_j = base2bit[seq[n + 1]], base2bit[seq[n]]
+                Delta_G += freedom_of_H_37_table[base_i][base_j] * H_bonds_number[base_i][base_j] + \
+                           penalty_of_H_37_table[base_i][base_j]
             term5 = sequence[-2:]
             if term5 == "TA":
                 Delta_G += adjust_initiation[seq[0]] + adjust_initiation[seq[-1]] + adjust_terminal_TA
             else:
                 Delta_G += adjust_initiation[seq[0]] + adjust_initiation[seq[-1]]
             # adjust by concentration of Na+
             Delta_G -= (0.175 * math.log(Na / 1000, math.e) + 0.20) * len(seq)
@@ -302,45 +307,61 @@
         sort_cover = sorted(cover_for_MM.items(), key=lambda x: x[1], reverse=True)
         L_seq = list(sort_cover[0][0])
         best_primer_index = [base2bit[x] for x in L_seq]
         # Return the maximum of an array or maximum along an axis. axis=0 代表列 , axis=1 代表行
         return best_primer_index
 
     def entropy(self, cover, cover_number, gap_sequence, gap_sequence_number):
+        # cBit: entropy of cover sequences
+        # tBit: entropy of total sequences
         cBit = 0
+        tBit = 0
         for c in cover.keys():
             cBit += (cover[c] / cover_number) * math.log((cover[c] / cover_number), 2)
-        tBit = cBit
+            tBit += (cover[c] / (cover_number + gap_sequence_number)) * \
+                    math.log((cover[c] / (cover_number + gap_sequence_number)), 2)
         for t in gap_sequence.keys():
-            tBit += (gap_sequence[t] / gap_sequence_number) * math.log((gap_sequence[t] / gap_sequence_number), 2)
+            tBit += (gap_sequence[t] / (cover_number + gap_sequence_number)) * \
+                    math.log((gap_sequence[t] / (cover_number + gap_sequence_number)), 2)
         return round(-cBit, 2), round(-tBit, 2)
 
     # Sequence processing. Return a list contains sequence length, start and stop position of each sequence.
     def seq_attribute(self, Input_dict):
         start_dict = {}
         stop_dict = {}
-        pattern_start = re.compile('[A-Z]')
-        pattern_stop = re.compile("-*$")
+        # pattern_start = re.compile('[A-Z]')
+        # pattern_stop = re.compile("-*$")
         for acc_id in Input_dict.keys():
-            # len_dict[acc_id] = len(Input_dict[acc_id])
-            start_dict[acc_id] = pattern_start.search(Input_dict[acc_id]).span()[0]
-            stop_dict[acc_id] = pattern_stop.search(Input_dict[acc_id]).span()[0] - 1
-        # start position should contain [coverage] sequences at least.
+            # start_dict[acc_id] = pattern_start.search(Input_dict[acc_id]).span()[0]
+            # stop_dict[acc_id] = pattern_stop.search(Input_dict[acc_id]).span()[0] - 1
+            t_length = len(Input_dict[acc_id])
+            start_dict[acc_id] = t_length - len(Input_dict[acc_id].lstrip("-"))
+            stop_dict[acc_id] = len(Input_dict[acc_id].rstrip("-"))
+            # start position should contain [coverage] sequences at least.
         start = np.quantile(np.array(list(start_dict.values())).reshape(1, -1), self.coverage, interpolation="higher")
         # for python 3.9.9
         # start = np.quantile(np.array(list(start_dict.values())).reshape(1, -1), self.coverage, method="higher")
         # stop position should contain [coverage] sequences at least.
         stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, interpolation="lower")
         # stop = np.quantile(np.array(list(stop_dict.values())).reshape(1, -1), self.coverage, method="lower")
         if stop - start < int(self.product):
             print("Error: max length of PCR product is shorter than the default min Product length with {} "
                   "coverage! Non candidate primers !!!".format(self.coverage))
             sys.exit(1)
         else:
-            return [start, stop]
+            return [start, stop, stop - start]
+
+    def entropy_threshold_adjust(self, length):
+        if length < 5000:
+            return self.raw_entropy_threshold
+        else:
+            if length < 10000:
+                return self.raw_entropy_threshold * 0.95
+            else:
+                return self.raw_entropy_threshold * 0.9
 
     def get_primers(self, sequence_dict, primer_start):  # , primer_info, non_cov_primer_out
         # record sequence and acc id
         non_gap_seq_id = defaultdict(list)
         # record sequence (no gap) and number
         cover = defaultdict(int)
         cover_for_MM = defaultdict(int)
@@ -349,42 +370,47 @@
         # record sequence (> variation gap) and number
         gap_sequence = defaultdict(int)
         gap_seq_id = defaultdict(list)
         # record total sequence (> variation gap) number
         gap_sequence_number = 0
         primers_db = []
         for seq_id in sequence_dict.keys():
-            # sequence
             sequence = sequence_dict[seq_id][primer_start:primer_start + self.primer_length].upper()
             # replace "-" which in start or stop position with nucleotides
-            if sequence.startswith("-"):
-                sequence_narrow = sequence.lstrip("-")
-                append_base_length = len(sequence) - len(sequence_narrow)
-                left_seq = sequence_dict[seq_id][0:primer_start].replace("-", "")
-                if len(left_seq) >= append_base_length:
-                    sequence = left_seq[len(left_seq) - append_base_length:] + sequence_narrow
-            if sequence.endswith("-"):
-                sequence_narrow = sequence.rstrip("-")
-                append_base_length = len(sequence) - len(sequence_narrow)
-                right_seq = sequence_dict[seq_id][primer_start + self.primer_length:].replace("-", "")
-                if len(right_seq) >= append_base_length:
-                    sequence = sequence_narrow + right_seq[0:append_base_length]
+            if sequence == "-" * self.primer_length:
+                pass
+            else:
+                if sequence.startswith("-"):
+                    sequence_narrow = sequence.lstrip("-")
+                    append_base_length = len(sequence) - len(sequence_narrow)
+                    left_seq = sequence_dict[seq_id][0:primer_start].replace("-", "")
+                    if len(left_seq) >= append_base_length:
+                        sequence = left_seq[len(left_seq) - append_base_length:] + sequence_narrow
+                if sequence.endswith("-"):
+                    sequence_narrow = sequence.rstrip("-")
+                    append_base_length = len(sequence) - len(sequence_narrow)
+                    right_seq = sequence_dict[seq_id][primer_start + self.primer_length:].replace("-", "")
+                    if len(right_seq) >= append_base_length:
+                        sequence = sequence_narrow + right_seq[0:append_base_length]
             if len(sequence) < self.primer_length:
                 append_base_length = self.primer_length - len(sequence)
                 left_seq = sequence_dict[seq_id][0:primer_start].replace("-", "")
                 if len(left_seq) >= append_base_length:
                     sequence = left_seq[len(left_seq) - append_base_length:] + sequence
             # gap number. number of gap > 2
             if list(sequence).count("-") > self.variation:
                 gap_sequence[sequence] += 1
                 gap_sequence_number += 1
-                # record acc ID of gap sequences
-                expand_sequence = self.degenerate_seq(sequence)
-                for i in expand_sequence:
-                    gap_seq_id[i].append(seq_id)
+                if round(gap_sequence_number / self.total_sequence_number, 2) >= (1 - self.coverage):
+                    break
+                else:
+                    # record acc ID of gap sequences
+                    expand_sequence = self.degenerate_seq(sequence)
+                    for i in expand_sequence:
+                        gap_seq_id[i].append(seq_id)
             # # accepted gap, number of gap <= variation
             else:
                 expand_sequence = self.degenerate_seq(sequence)
                 cover_number += 1
                 for i in expand_sequence:
                     cover[i] += 1
                     primers_db.append(list(i))
@@ -392,40 +418,50 @@
                     non_gap_seq_id[i].append(seq_id)
                     if re.search("-", i):
                         pass
                     else:
                         cover_for_MM[i] += 1
         # number of sequences with too many gaps greater than (1 - self.coverage)
         if round(gap_sequence_number / self.total_sequence_number, 2) >= (1 - self.coverage):
+            # print("Gap fail")
             self.resQ.put(None)
         elif len(cover) < 1:
             self.resQ.put(None)
+            # print("Cover fail")
         else:
+            # cBit: entropy of cover sequences
+            # tBit: entropy of total sequences
             cBit, tBit = self.entropy(cover, cover_number, gap_sequence, gap_sequence_number)
             if tBit > self.entropy_threshold:
+                # print("Entropy fail")
                 # This window is not a conserved region, and not proper to design primers
                 self.resQ.put(None)
             else:
                 primers_db = pd.DataFrame(primers_db)
                 # frequency matrix
                 freq_matrix = self.state_matrix(primers_db)
+                colSum = np.sum(freq_matrix, axis=0)
                 a, b = freq_matrix.shape
                 # a < 4 means base composition of this region is less than 4 (GC bias).
                 # It's not a proper region for primer design.
                 if a < 4:
                     self.resQ.put(None)
+                elif (colSum == 0).any():
+                    # print(colSum)  # if 0 in array; pass
+                    self.resQ.put(None)
                 else:
                     gap_seq_id_info = [primer_start, gap_seq_id]
                     mismatch_coverage, non_cov_primer_info = \
                         self.degenerate_by_NN_algorithm(primer_start, freq_matrix, cover, non_gap_seq_id,
                                                         cover_for_MM, cover_number, cBit, tBit)
                     # self.resQ.put([mismatch_coverage, non_cov_primer_info, gap_seq_id_info])
                     # F, R = mismatch_coverage[1][6], mismatch_coverage[1][7]
                     sequence = mismatch_coverage[1][2]
                     if self.dimer_check(sequence):
+                        # print("Dimer fail")
                         self.resQ.put(None)
                     else:
                         self.resQ.put([mismatch_coverage, non_cov_primer_info, gap_seq_id_info])
                     # if F < cover_number * 0.5 or R < cover_number * 0.5:
                     #     self.resQ.put(None)
                     # else:
                     #     self.resQ.put([mismatch_coverage, non_cov_primer_info, gap_seq_id_info])
@@ -749,48 +785,48 @@
         # optimal_primer_update, coverage_update,
         # NN_coverage_update, NN array_update,
         # degeneracy_update, degenerate_update
         return primer_update_list[optimal_idx], coverage_update_list[optimal_idx], \
                NN_coverage_update[optimal_idx], NN_array_update_list[optimal_idx], \
                degeneracy_update, degenerate_number_update
 
+    def get_Y(self):
+        Y_strict, Y_strict_R = [], []
+        for y in self.position.split(","):
+            y_index = int(y.strip())
+            if y_index > 0:
+                Y_strict.append(y_index)
+                Y_strict_R.append(self.primer_length - y_index)
+            else:
+                Y_strict.append(self.primer_length + y_index + 1)
+                Y_strict_R.append(-y_index + 1)
+        return Y_strict, Y_strict_R
+
     def mis_primer_check(self, all_primers, optimal_primer, cover, non_gap_seq_id):
         # uncoverage sequence in cover dict
         optimal_primer_set = set(self.degenerate_seq(optimal_primer))
         uncover_primer_set = all_primers - optimal_primer_set
         F_non_cover, R_non_cover = {}, {}
         F_mis_cover, R_mis_cover = 0, 0
         for uncover_primer in uncover_primer_set:
             Y_dist = Y_distance(optimal_primer, uncover_primer)
             if len(Y_dist) > self.variation:
                 # record sequence and acc_ID which will never mis-coverage. too many mismatch!
                 F_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
                 R_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
             # if len(Y_dist) <= self.variation:
             else:
-                # print(Y_dist)
-                if min(Y_dist) < self.position:
-                    # record sequence and acc_ID which will never mis-coverage.
-                    # mismatch position located in start region!
+                if len(set(Y_dist).intersection(self.Y_strict)) > 0:
+                    F_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
+                else:
+                    F_mis_cover += cover[uncover_primer]
+                if len(set(Y_dist).intersection(self.Y_strict_R)) > 0:
                     R_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
-                    if max(Y_dist) > len(optimal_primer) - self.position:
-                        # record sequence and acc_ID which will never mis-coverage.
-                        # mismatch popsition located in stop region!
-                        F_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
-                    else:
-                        F_mis_cover += cover[uncover_primer]
                 else:
-                    if max(Y_dist) > len(optimal_primer) - self.position:
-                        # record sequence and acc_ID which will never mis-coverage.
-                        # mismatch popsition located in stop region!
-                        F_non_cover[uncover_primer] = non_gap_seq_id[uncover_primer]
-                        R_mis_cover += cover[uncover_primer]
-                    else:
-                        F_mis_cover += cover[uncover_primer]
-                        R_mis_cover += cover[uncover_primer]
+                    R_mis_cover += cover[uncover_primer]
         # print(F_mis_cover)
         # print(R_mis_cover)
         return F_mis_cover, F_non_cover, R_mis_cover, R_non_cover
 
     ################# get_primers #####################
     def run(self):
         p = ProcessPoolExecutor(self.nproc)  #
```

### Comparing `multiPrime-2.3.9/src/utils.py` & `multiPrime-2.4.1/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,21 +69,23 @@
                       help="Filter primers by match fraction. If you set -s lower than 0.8, make sure that "
                            "--entropy greater than 3.6, because disorder region (entropy > 3.6) will not be processed "
                            "in multiPrime. Even these regions can design coverage with error greater than your "
                            "threshold, it wont be processed. Default: 0.8.")
 
     parser.add_option('-c', '--coordinate',
                       dest='coordinate',
-                      default="4",
-                      type="int",
-                      help="Mismatch index is not allowed to locate in start or stop. "
+                      default="2,-1",
+                      type="str",
+                      help="Mismatch index is not allowed to locate in your specific positions."
                            "otherwise, it won't be regard as the mis-coverage. "
                            "With this param, you can control the index of Y-distance (number=variation and position of mismatch) "
-                           "when calculate coverage with error."
-                           "Default: 4.")
+                           "when calculate coverage with error. coordinate>0: 5\'==>3\'; coordinate<0: 3\'==>5\'."
+                           "You can set this param to any value that you prefer. Default: 1,-1. "
+                           "1:  I dont want mismatch at the 2nd position, start from 0."
+                           "-1: I dont want mismatch at the -1st position, start from -1.")
 
     parser.add_option('-p', '--proc',
                       dest='proc',
                       default="20",
                       type="int",
                       help="Number of process to launch. Default: 20.")
```

