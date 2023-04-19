# Comparing `tmp/sapiens-1.0.3.tar.gz` & `tmp/sapiens-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapiens-1.0.3.tar", last modified: Mon Jan  2 20:47:55 2023, max compression
+gzip compressed data, was "sapiens-1.0.4.tar", last modified: Wed Apr 19 13:15:29 2023, max compression
```

## Comparing `sapiens-1.0.3.tar` & `sapiens-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-01-02 20:47:55.978412 sapiens-1.0.3/
--rw-r--r--   0 prihodad   (501) staff       (20)     1141 2023-01-02 11:19:50.000000 sapiens-1.0.3/LICENSE
--rw-r--r--   0 prihodad   (501) staff       (20)     1835 2023-01-02 11:19:50.000000 sapiens-1.0.3/LICENSES_THIRD_PARTY
--rw-r--r--   0 prihodad   (501) staff       (20)       44 2023-01-02 11:19:50.000000 sapiens-1.0.3/MANIFEST.in
--rw-r--r--   0 prihodad   (501) staff       (20)     5699 2023-01-02 20:47:55.977835 sapiens-1.0.3/PKG-INFO
--rw-r--r--   0 prihodad   (501) staff       (20)     5248 2023-01-02 11:19:50.000000 sapiens-1.0.3/README.md
-drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-01-02 20:47:55.947115 sapiens-1.0.3/sapiens/
--rw-r--r--   0 prihodad   (501) staff       (20)      305 2023-01-02 11:19:50.000000 sapiens-1.0.3/sapiens/__init__.py
-drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-01-02 20:47:55.959102 sapiens-1.0.3/sapiens/__pycache__/
--rw-r--r--   0 prihodad   (501) staff       (20)      489 2023-01-02 12:11:18.000000 sapiens-1.0.3/sapiens/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 prihodad   (501) staff       (20)      184 2023-01-02 12:11:18.000000 sapiens-1.0.3/sapiens/__pycache__/__version__.cpython-39.pyc
--rw-r--r--   0 prihodad   (501) staff       (20)     2978 2023-01-02 12:11:27.000000 sapiens-1.0.3/sapiens/__pycache__/predict.cpython-39.pyc
--rw-r--r--   0 prihodad   (501) staff       (20)     4532 2023-01-02 12:11:27.000000 sapiens-1.0.3/sapiens/__pycache__/roberta.cpython-39.pyc
--rw-r--r--   0 prihodad   (501) staff       (20)     3841 2023-01-02 12:11:29.000000 sapiens-1.0.3/sapiens/__pycache__/smooth_masked_lm.cpython-39.pyc
--rw-r--r--   0 prihodad   (501) staff       (20)       22 2023-01-02 20:47:42.000000 sapiens-1.0.3/sapiens/__version__.py
-drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-01-02 20:47:55.935460 sapiens-1.0.3/sapiens/models/
-drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-01-02 20:47:55.977340 sapiens-1.0.3/sapiens/models/v1/
--rw-r--r--   0 prihodad   (501) staff       (20)  4590491 2023-01-02 11:19:50.000000 sapiens-1.0.3/sapiens/models/v1/checkpoint_vh.pt
--rw-r--r--   0 prihodad   (501) staff       (20)  4573875 2023-01-02 11:19:50.000000 sapiens-1.0.3/sapiens/models/v1/checkpoint_vl.pt
--rw-r--r--   0 prihodad   (501) staff       (20)       80 2023-01-02 11:19:50.000000 sapiens-1.0.3/sapiens/models/v1/dict.txt
--rw-r--r--   0 prihodad   (501) staff       (20)     2670 2023-01-02 11:19:50.000000 sapiens-1.0.3/sapiens/predict.py
--rw-r--r--   0 prihodad   (501) staff       (20)     4218 2023-01-02 11:19:50.000000 sapiens-1.0.3/sapiens/roberta.py
--rw-r--r--   0 prihodad   (501) staff       (20)     3637 2023-01-02 11:19:50.000000 sapiens-1.0.3/sapiens/smooth_masked_lm.py
-drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-01-02 20:47:55.950209 sapiens-1.0.3/sapiens.egg-info/
--rw-r--r--   0 prihodad   (501) staff       (20)     5699 2023-01-02 20:47:55.000000 sapiens-1.0.3/sapiens.egg-info/PKG-INFO
--rw-r--r--   0 prihodad   (501) staff       (20)      648 2023-01-02 20:47:55.000000 sapiens-1.0.3/sapiens.egg-info/SOURCES.txt
--rw-r--r--   0 prihodad   (501) staff       (20)        1 2023-01-02 20:47:55.000000 sapiens-1.0.3/sapiens.egg-info/dependency_links.txt
--rw-r--r--   0 prihodad   (501) staff       (20)       36 2023-01-02 20:47:55.000000 sapiens-1.0.3/sapiens.egg-info/requires.txt
--rw-r--r--   0 prihodad   (501) staff       (20)        8 2023-01-02 20:47:55.000000 sapiens-1.0.3/sapiens.egg-info/top_level.txt
--rw-r--r--   0 prihodad   (501) staff       (20)       38 2023-01-02 20:47:55.978468 sapiens-1.0.3/setup.cfg
--rw-r--r--   0 prihodad   (501) staff       (20)     1384 2023-01-02 20:44:45.000000 sapiens-1.0.3/setup.py
+drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-04-19 13:15:29.503973 sapiens-1.0.4/
+-rw-r--r--   0 prihodad   (501) staff       (20)     1141 2023-01-02 11:19:50.000000 sapiens-1.0.4/LICENSE
+-rw-r--r--   0 prihodad   (501) staff       (20)     1835 2023-01-02 11:19:50.000000 sapiens-1.0.4/LICENSES_THIRD_PARTY
+-rw-r--r--   0 prihodad   (501) staff       (20)       44 2023-01-02 11:19:50.000000 sapiens-1.0.4/MANIFEST.in
+-rw-r--r--   0 prihodad   (501) staff       (20)     5699 2023-04-19 13:15:29.503642 sapiens-1.0.4/PKG-INFO
+-rw-r--r--   0 prihodad   (501) staff       (20)     5248 2023-01-02 11:19:50.000000 sapiens-1.0.4/README.md
+drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-04-19 13:15:29.464417 sapiens-1.0.4/sapiens/
+-rw-r--r--   0 prihodad   (501) staff       (20)      305 2023-01-02 11:19:50.000000 sapiens-1.0.4/sapiens/__init__.py
+drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-04-19 13:15:29.481845 sapiens-1.0.4/sapiens/__pycache__/
+-rw-r--r--   0 prihodad   (501) staff       (20)      489 2023-01-02 12:11:18.000000 sapiens-1.0.4/sapiens/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 prihodad   (501) staff       (20)      184 2023-01-02 12:11:18.000000 sapiens-1.0.4/sapiens/__pycache__/__version__.cpython-39.pyc
+-rw-r--r--   0 prihodad   (501) staff       (20)     2978 2023-01-02 12:11:27.000000 sapiens-1.0.4/sapiens/__pycache__/predict.cpython-39.pyc
+-rw-r--r--   0 prihodad   (501) staff       (20)     4532 2023-01-02 12:11:27.000000 sapiens-1.0.4/sapiens/__pycache__/roberta.cpython-39.pyc
+-rw-r--r--   0 prihodad   (501) staff       (20)     3841 2023-01-02 12:11:29.000000 sapiens-1.0.4/sapiens/__pycache__/smooth_masked_lm.cpython-39.pyc
+-rw-r--r--   0 prihodad   (501) staff       (20)       22 2023-04-19 13:14:43.000000 sapiens-1.0.4/sapiens/__version__.py
+drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-04-19 13:15:29.440421 sapiens-1.0.4/sapiens/models/
+drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-04-19 13:15:29.499578 sapiens-1.0.4/sapiens/models/v1/
+-rw-r--r--   0 prihodad   (501) staff       (20)  4590491 2023-01-02 11:19:50.000000 sapiens-1.0.4/sapiens/models/v1/checkpoint_vh.pt
+-rw-r--r--   0 prihodad   (501) staff       (20)  4573875 2023-01-02 11:19:50.000000 sapiens-1.0.4/sapiens/models/v1/checkpoint_vl.pt
+-rw-r--r--   0 prihodad   (501) staff       (20)       80 2023-01-02 11:19:50.000000 sapiens-1.0.4/sapiens/models/v1/dict.txt
+-rw-r--r--   0 prihodad   (501) staff       (20)     2670 2023-01-02 11:19:50.000000 sapiens-1.0.4/sapiens/predict.py
+-rw-r--r--   0 prihodad   (501) staff       (20)     4218 2023-01-02 11:19:50.000000 sapiens-1.0.4/sapiens/roberta.py
+-rw-r--r--   0 prihodad   (501) staff       (20)     3637 2023-01-02 11:19:50.000000 sapiens-1.0.4/sapiens/smooth_masked_lm.py
+drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-04-19 13:15:29.469851 sapiens-1.0.4/sapiens.egg-info/
+-rw-r--r--   0 prihodad   (501) staff       (20)     5699 2023-04-19 13:15:29.000000 sapiens-1.0.4/sapiens.egg-info/PKG-INFO
+-rw-r--r--   0 prihodad   (501) staff       (20)      670 2023-04-19 13:15:29.000000 sapiens-1.0.4/sapiens.egg-info/SOURCES.txt
+-rw-r--r--   0 prihodad   (501) staff       (20)        1 2023-04-19 13:15:29.000000 sapiens-1.0.4/sapiens.egg-info/dependency_links.txt
+-rw-r--r--   0 prihodad   (501) staff       (20)       15 2023-04-19 13:15:29.000000 sapiens-1.0.4/sapiens.egg-info/requires.txt
+-rw-r--r--   0 prihodad   (501) staff       (20)        8 2023-04-19 13:15:29.000000 sapiens-1.0.4/sapiens.egg-info/top_level.txt
+-rw-r--r--   0 prihodad   (501) staff       (20)       38 2023-04-19 13:15:29.504070 sapiens-1.0.4/setup.cfg
+-rw-r--r--   0 prihodad   (501) staff       (20)     1223 2023-04-19 12:56:57.000000 sapiens-1.0.4/setup.py
+drwxr-xr-x   0 prihodad   (501) staff       (20)        0 2023-04-19 13:15:29.503047 sapiens-1.0.4/tests/
+-rw-r--r--   0 prihodad   (501) staff       (20)      787 2023-01-02 11:19:50.000000 sapiens-1.0.4/tests/test_predict.py
```

### Comparing `sapiens-1.0.3/LICENSE` & `sapiens-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/LICENSES_THIRD_PARTY` & `sapiens-1.0.4/LICENSES_THIRD_PARTY`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/PKG-INFO` & `sapiens-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapiens
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sapiens: Human antibody language model based on BERT
 Home-page: https://github.com/Merck/Sapiens
 Author: David Prihoda
 Author-email: david.prihoda@gmail.com
 License: MIT
 Keywords: sapiens,antibody humanization,bert,biophi
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sapiens Version: 1.0.3 Summary: Sapiens: Human
+Metadata-Version: 2.1 Name: sapiens Version: 1.0.4 Summary: Sapiens: Human
 antibody language model based on BERT Home-page: https://github.com/Merck/
 Sapiens Author: David Prihoda Author-email: david.prihoda@gmail.com License:
 MIT Keywords: sapiens,antibody humanization,bert,biophi Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE License-File: LICENSES_THIRD_PARTY # Sapiens:
 Human antibody language model ``` ____ _ / ___| __ _ _ __ (_) ___ _ __ ___ \___
 \ / _` | '_ \| |/ _ \ '_ \/ __| ___| | |_| | |_| | | __/ | | \__ \ |____/
```

### Comparing `sapiens-1.0.3/README.md` & `sapiens-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens/__pycache__/predict.cpython-39.pyc` & `sapiens-1.0.4/sapiens/__pycache__/predict.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens/__pycache__/roberta.cpython-39.pyc` & `sapiens-1.0.4/sapiens/__pycache__/roberta.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens/__pycache__/smooth_masked_lm.cpython-39.pyc` & `sapiens-1.0.4/sapiens/__pycache__/smooth_masked_lm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens/models/v1/checkpoint_vh.pt` & `sapiens-1.0.4/sapiens/models/v1/checkpoint_vh.pt`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens/models/v1/checkpoint_vl.pt` & `sapiens-1.0.4/sapiens/models/v1/checkpoint_vl.pt`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens/predict.py` & `sapiens-1.0.4/sapiens/predict.py`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens/roberta.py` & `sapiens-1.0.4/sapiens/roberta.py`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens/smooth_masked_lm.py` & `sapiens-1.0.4/sapiens/smooth_masked_lm.py`

 * *Files identical despite different names*

### Comparing `sapiens-1.0.3/sapiens.egg-info/PKG-INFO` & `sapiens-1.0.4/sapiens.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapiens
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sapiens: Human antibody language model based on BERT
 Home-page: https://github.com/Merck/Sapiens
 Author: David Prihoda
 Author-email: david.prihoda@gmail.com
 License: MIT
 Keywords: sapiens,antibody humanization,bert,biophi
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sapiens Version: 1.0.3 Summary: Sapiens: Human
+Metadata-Version: 2.1 Name: sapiens Version: 1.0.4 Summary: Sapiens: Human
 antibody language model based on BERT Home-page: https://github.com/Merck/
 Sapiens Author: David Prihoda Author-email: david.prihoda@gmail.com License:
 MIT Keywords: sapiens,antibody humanization,bert,biophi Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/
 markdown License-File: LICENSE License-File: LICENSES_THIRD_PARTY # Sapiens:
 Human antibody language model ``` ____ _ / ___| __ _ _ __ (_) ___ _ __ ___ \___
 \ / _` | '_ \| |/ _ \ '_ \/ __| ___| | |_| | |_| | | __/ | | \__ \ |____/
```

### Comparing `sapiens-1.0.3/sapiens.egg-info/SOURCES.txt` & `sapiens-1.0.4/sapiens.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 sapiens/__pycache__/__init__.cpython-39.pyc
 sapiens/__pycache__/__version__.cpython-39.pyc
 sapiens/__pycache__/predict.cpython-39.pyc
 sapiens/__pycache__/roberta.cpython-39.pyc
 sapiens/__pycache__/smooth_masked_lm.cpython-39.pyc
 sapiens/models/v1/checkpoint_vh.pt
 sapiens/models/v1/checkpoint_vl.pt
-sapiens/models/v1/dict.txt
+sapiens/models/v1/dict.txt
+tests/test_predict.py
```

### Comparing `sapiens-1.0.3/setup.py` & `sapiens-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,15 @@
     author='David Prihoda',
     packages=find_packages(include=['sapiens.*', 'sapiens']),
     author_email='david.prihoda@gmail.com',
     license='MIT',
     python_requires=">=3.7",
     install_requires=[
         'pandas',
-        'fairseq == 0.10.2', # using old fairseq version until latest version is on conda-forge
-        'numpy < 1.24.0' # use old numpy version because of fairseq incompatibility
+        'fairseq',
     ],
     keywords='sapiens, antibody humanization, bert, biophi',
     classifiers=[
         'Programming Language :: Python :: 3',
     ],
     include_package_data=True,
     package_data={'': ['*.pt', '*.txt']},
```

