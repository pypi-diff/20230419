# Comparing `tmp/pymCADRE-1.2.3.tar.gz` & `tmp/pymCADRE-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymCADRE-1.2.3.tar", last modified: Wed Apr 19 09:43:29 2023, max compression
+gzip compressed data, was "dist/pymCADRE-1.2.4.tar", last modified: Wed Apr 19 11:40:30 2023, max compression
```

## Comparing `pymCADRE-1.2.3.tar` & `pymCADRE-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,48 @@
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:43:29.430107 pymCADRE-1.2.3/
--rw-rw-r--   0 leonidou   (501) staff       (20)    35149 2021-10-13 11:22:14.000000 pymCADRE-1.2.3/LICENSE
--rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-19 09:43:29.429482 pymCADRE-1.2.3/PKG-INFO
--rw-rw-r--   0 leonidou   (501) staff       (20)     4648 2023-04-19 09:38:15.000000 pymCADRE-1.2.3/README.md
-drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 09:43:29.428569 pymCADRE-1.2.3/pymCADRE.egg-info/
--rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/PKG-INFO
--rw-r--r--   0 leonidou   (501) staff       (20)      200 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/SOURCES.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/dependency_links.txt
--rw-r--r--   0 leonidou   (501) staff       (20)       28 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/requires.txt
--rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 09:43:29.000000 pymCADRE-1.2.3/pymCADRE.egg-info/top_level.txt
--rw-rw-r--   0 leonidou   (501) staff       (20)      104 2021-10-13 11:22:14.000000 pymCADRE-1.2.3/pyproject.toml
--rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 09:43:29.430441 pymCADRE-1.2.3/setup.cfg
--rw-rw-r--   0 leonidou   (501) staff       (20)      978 2023-04-19 09:42:53.000000 pymCADRE-1.2.3/setup.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.359646 pymCADRE-1.2.4/
+-rw-rw-r--   0 leonidou   (501) staff       (20)    35149 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/LICENSE
+-rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-19 11:40:30.358168 pymCADRE-1.2.4/PKG-INFO
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4648 2023-04-19 09:38:15.000000 pymCADRE-1.2.4/README.md
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.342632 pymCADRE-1.2.4/pymCADRE.egg-info/
+-rw-r--r--   0 leonidou   (501) staff       (20)     5318 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/PKG-INFO
+-rw-r--r--   0 leonidou   (501) staff       (20)     1511 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/SOURCES.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)        1 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/dependency_links.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       28 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/requires.txt
+-rw-r--r--   0 leonidou   (501) staff       (20)       14 2023-04-19 11:40:30.000000 pymCADRE-1.2.4/pymCADRE.egg-info/top_level.txt
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.339295 pymCADRE-1.2.4/pymCADRE_code/
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.343194 pymCADRE-1.2.4/pymCADRE_code/code/
+-rw-rw-r--   0 leonidou   (501) staff       (20)       52 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/__init__.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.346224 pymCADRE-1.2.4/pymCADRE_code/code/check/
+-rw-rw-r--   0 leonidou   (501) staff       (20)       52 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/__init__.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     5053 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/check_model_function.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3429 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/check_rxn_flux.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)      636 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/find_ex_reactions.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2066 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/find_organic_ex_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3035 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/find_required_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1361 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/check/set_metabolite_bounds.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.348511 pymCADRE-1.2.4/pymCADRE_code/code/prune/
+-rw-rw-r--   0 leonidou   (501) staff       (20)       52 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/__init__.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3773 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/check_core_deadends.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3915 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/check_model_consistency.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4021 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/check_salvage_path.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3084 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/find_inactive_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     7430 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/prune/prune_model.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2473 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/pymcadre.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.352217 pymCADRE-1.2.4/pymCADRE_code/code/rank/
+-rw-rw-r--   0 leonidou   (501) staff       (20)       52 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/__init__.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2148 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/calc_conn_evidence.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2078 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/calc_expr_evidence.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2886 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/initialize_generic_model.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2159 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/map_gene_scores_to_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3235 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/map_high_conf_to_rxns.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3096 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/parse_gprs.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4504 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/code/rank/rank_reactions.py
+drwxr-xr-x   0 leonidou   (501) staff       (20)        0 2023-04-19 11:40:30.356791 pymCADRE-1.2.4/pymCADRE_code/pre_processing/
+-rw-rw-r--   0 leonidou   (501) staff       (20)      948 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/consistent_conf_scores.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     4931 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/data_preprocessing.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     2298 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/entrez_ids.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1433 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/format_model_matlab.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     3703 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/get_conf_scores.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1151 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pymCADRE_code/pre_processing/ubiquity_scores.py
+-rw-rw-r--   0 leonidou   (501) staff       (20)      104 2021-10-13 11:22:14.000000 pymCADRE-1.2.4/pyproject.toml
+-rw-r--r--   0 leonidou   (501) staff       (20)       38 2023-04-19 11:40:30.360093 pymCADRE-1.2.4/setup.cfg
+-rw-rw-r--   0 leonidou   (501) staff       (20)     1311 2023-04-19 11:40:14.000000 pymCADRE-1.2.4/setup.py
```

### Comparing `pymCADRE-1.2.3/LICENSE` & `pymCADRE-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.3/PKG-INFO` & `pymCADRE-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymCADRE
-Version: 1.2.3
+Version: 1.2.4
 Summary: The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 Home-page: https://github.com/draeger-lab/pymCADRE
 Author: Nantia Leonidou
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: pymCADRE,systems biology,tissue-specific metabolic models
 Platform: UNKNOWN
```

### Comparing `pymCADRE-1.2.3/README.md` & `pymCADRE-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pymCADRE-1.2.3/pymCADRE.egg-info/PKG-INFO` & `pymCADRE-1.2.4/pymCADRE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymCADRE
-Version: 1.2.3
+Version: 1.2.4
 Summary: The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.
 Home-page: https://github.com/draeger-lab/pymCADRE
 Author: Nantia Leonidou
 Author-email: nantia.leonidou@uni-tuebingen.de
 License:  GPL-3.0
 Keywords: pymCADRE,systems biology,tissue-specific metabolic models
 Platform: UNKNOWN
```

### Comparing `pymCADRE-1.2.3/setup.py` & `pymCADRE-1.2.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pymCADRE',
-    version='1.2.3',
+    version='1.2.4',
     description='The pymCADRE tool is an advanced re-implementation of the metabolic Context-specificity Assessed by Deterministic Reaction Evaluation (mCADRE) algorithm in Python. It constructs tissue-specific metabolic models by leveraging gene expression data and literature-based evidence, along with network topology information.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/draeger-lab/pymCADRE',
     author='Nantia Leonidou',
     author_email='nantia.leonidou@uni-tuebingen.de',
     license=' GPL-3.0',
     keywords=['pymCADRE', 'systems biology', 'tissue-specific metabolic models'],
+    #packages=find_packages(include=['pymCADRE_code']),
+    #py_modules=['SBOannotator', 'main'],
+    #packages=find_packages(),
+    packages=['pymCADRE_code','pymCADRE_code.code','pymCADRE_code.pre_processing',
+        'pymCADRE_code.code.check','pymCADRE_code.code.prune','pymCADRE_code.code.rank'],
+    include_package_data=True,
     install_requires=['pandas',
                       'numpy',
                       'cobra',
                       'requests']
 )
```

