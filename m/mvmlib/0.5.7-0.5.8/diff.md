# Comparing `tmp/mvmlib-0.5.7.tar.gz` & `tmp/mvmlib-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvmlib-0.5.7.tar", last modified: Tue Mar  7 04:18:54 2023, max compression
+gzip compressed data, was "mvmlib-0.5.8.tar", last modified: Tue Apr 18 23:42:22 2023, max compression
```

## Comparing `mvmlib-0.5.7.tar` & `mvmlib-0.5.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     3444 2023-03-07 04:18:17.271483 mvmlib-0.5.7/.github/workflows/release.yml
--rw-r--r--   0        0        0      930 2023-03-07 04:18:17.271483 mvmlib-0.5.7/.github/workflows/tests_dev.yml
--rw-r--r--   0        0        0     2183 2023-03-07 04:18:17.271483 mvmlib-0.5.7/.github/workflows/tests_master.yml
--rw-r--r--   0        0        0     2072 2023-03-07 04:18:17.271483 mvmlib-0.5.7/.gitignore
--rw-r--r--   0        0        0      633 2023-03-07 04:18:17.271483 mvmlib-0.5.7/docs/Makefile
--rw-r--r--   0        0        0      162 2023-03-07 04:18:17.271483 mvmlib-0.5.7/docs/_static/css/custom.css
--rw-r--r--   0        0        0     1834 2023-03-07 04:18:17.271483 mvmlib-0.5.7/docs/api.rst
--rw-r--r--   0        0        0    16325 2023-03-07 04:18:17.271483 mvmlib-0.5.7/docs/background.rst
--rw-r--r--   0        0        0     2488 2023-03-07 04:18:17.271483 mvmlib-0.5.7/docs/conf.py
--rw-r--r--   0        0        0      317 2023-03-07 04:18:17.271483 mvmlib-0.5.7/docs/examples.rst
--rw-r--r--   0        0        0     1675 2023-03-07 04:18:17.271483 mvmlib-0.5.7/docs/getting_started.rst
--rw-r--r--   0        0        0      444 2023-03-07 04:18:17.271483 mvmlib-0.5.7/docs/glossary.rst
--rw-r--r--   0        0        0    16999 2023-03-07 04:18:17.275483 mvmlib-0.5.7/docs/history.rst
--rw-r--r--   0        0        0   403031 2023-03-07 04:18:17.275483 mvmlib-0.5.7/docs/images/TRS_example/load_case.png
--rw-r--r--   0        0        0    31511 2023-03-07 04:18:17.275483 mvmlib-0.5.7/docs/images/efm_example.png
--rw-r--r--   0        0        0   344431 2023-03-07 04:18:17.279483 mvmlib-0.5.7/docs/images/strut_example/MAN.png
--rw-r--r--   0        0        0   122730 2023-03-07 04:18:17.279483 mvmlib-0.5.7/docs/images/strut_example/simplified_strut_model.png
--rw-r--r--   0        0        0   806946 2023-03-07 04:18:17.287483 mvmlib-0.5.7/docs/images/strut_example/strut_overview.png
--rw-r--r--   0        0        0     3117 2023-03-07 04:18:17.287483 mvmlib-0.5.7/docs/index.rst
--rw-r--r--   0        0        0      799 2023-03-07 04:18:17.287483 mvmlib-0.5.7/docs/make.bat
--rw-r--r--   0        0        0   132133 2023-03-07 04:18:17.287483 mvmlib-0.5.7/docs/notebooks/PDF_examples.ipynb
--rw-r--r--   0        0        0   176595 2023-03-07 04:18:17.287483 mvmlib-0.5.7/docs/notebooks/TRS_example.ipynb
--rw-r--r--   0        0        0   229076 2023-03-07 04:18:17.291483 mvmlib-0.5.7/docs/notebooks/strut_example.ipynb
--rw-r--r--   0        0        0      847 2023-03-07 04:18:17.291483 mvmlib-0.5.7/docs/refs.bib
--rw-r--r--   0        0        0      674 2023-03-07 04:18:17.291483 mvmlib-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      157 2023-03-07 04:18:17.291483 mvmlib-0.5.7/pytest.ini
--rw-r--r--   0        0        0     1786 2023-03-07 04:18:17.291483 mvmlib-0.5.7/readme.md
--rw-r--r--   0        0        0      102 2023-03-07 04:18:17.291483 mvmlib-0.5.7/requirements.txt
--rw-r--r--   0        0        0      407 2023-03-07 04:18:17.291483 mvmlib-0.5.7/requirements_dev.txt
--rw-r--r--   0        0        0     5131 2023-03-07 04:18:17.291483 mvmlib-0.5.7/src/mvm/DOELib.py
--rw-r--r--   0        0        0      964 2023-03-07 04:18:17.291483 mvmlib-0.5.7/src/mvm/__init__.py
--rw-r--r--   0        0        0   134203 2023-03-07 04:18:17.291483 mvmlib-0.5.7/src/mvm/designMarginsLib.py
--rw-r--r--   0        0        0    13107 2023-03-07 04:18:17.291483 mvmlib-0.5.7/src/mvm/fuzzyLib.py
--rw-r--r--   0        0        0    28992 2023-03-07 04:18:17.291483 mvmlib-0.5.7/src/mvm/uncertaintyLib.py
--rw-r--r--   0        0        0     3299 2023-03-07 04:18:17.291483 mvmlib-0.5.7/src/mvm/utilities.py
--rw-r--r--   0        0        0      129 2023-03-07 04:18:17.291483 mvmlib-0.5.7/tests/__init__.py
--rw-r--r--   0        0        0      539 2023-03-07 04:18:17.291483 mvmlib-0.5.7/tests/test_doe.py
--rw-r--r--   0        0        0    14496 2023-03-07 04:18:17.291483 mvmlib-0.5.7/tests/test_fuzzy.py
--rw-r--r--   0        0        0    73185 2023-03-07 04:18:17.291483 mvmlib-0.5.7/tests/test_marginNetwork.py
--rw-r--r--   0        0        0    14717 2023-03-07 04:18:17.291483 mvmlib-0.5.7/tests/test_probFunction.py
--rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 mvmlib-0.5.7/setup.py
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 mvmlib-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     3444 2023-04-18 23:41:39.325292 mvmlib-0.5.8/.github/workflows/release.yml
+-rw-r--r--   0        0        0      930 2023-04-18 23:41:39.325292 mvmlib-0.5.8/.github/workflows/tests_dev.yml
+-rw-r--r--   0        0        0     2183 2023-04-18 23:41:39.325292 mvmlib-0.5.8/.github/workflows/tests_master.yml
+-rw-r--r--   0        0        0     2072 2023-04-18 23:41:39.325292 mvmlib-0.5.8/.gitignore
+-rw-r--r--   0        0        0      633 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/Makefile
+-rw-r--r--   0        0        0      162 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     1834 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/api.rst
+-rw-r--r--   0        0        0    16325 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/background.rst
+-rw-r--r--   0        0        0     2488 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/conf.py
+-rw-r--r--   0        0        0      317 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/examples.rst
+-rw-r--r--   0        0        0     1675 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/getting_started.rst
+-rw-r--r--   0        0        0      444 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/glossary.rst
+-rw-r--r--   0        0        0    17166 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/history.rst
+-rw-r--r--   0        0        0   403031 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/images/TRS_example/load_case.png
+-rw-r--r--   0        0        0    31511 2023-04-18 23:41:39.329292 mvmlib-0.5.8/docs/images/efm_example.png
+-rw-r--r--   0        0        0   344431 2023-04-18 23:41:39.333292 mvmlib-0.5.8/docs/images/strut_example/MAN.png
+-rw-r--r--   0        0        0   122730 2023-04-18 23:41:39.333292 mvmlib-0.5.8/docs/images/strut_example/simplified_strut_model.png
+-rw-r--r--   0        0        0   806946 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/images/strut_example/strut_overview.png
+-rw-r--r--   0        0        0     3117 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/index.rst
+-rw-r--r--   0        0        0      799 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/make.bat
+-rw-r--r--   0        0        0   132133 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/notebooks/PDF_examples.ipynb
+-rw-r--r--   0        0        0   176595 2023-04-18 23:41:39.341292 mvmlib-0.5.8/docs/notebooks/TRS_example.ipynb
+-rw-r--r--   0        0        0   229076 2023-04-18 23:41:39.345293 mvmlib-0.5.8/docs/notebooks/strut_example.ipynb
+-rw-r--r--   0        0        0      847 2023-04-18 23:41:39.345293 mvmlib-0.5.8/docs/refs.bib
+-rw-r--r--   0        0        0      674 2023-04-18 23:41:39.345293 mvmlib-0.5.8/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-04-18 23:41:39.345293 mvmlib-0.5.8/pytest.ini
+-rw-r--r--   0        0        0     1786 2023-04-18 23:41:39.345293 mvmlib-0.5.8/readme.md
+-rw-r--r--   0        0        0      102 2023-04-18 23:41:39.345293 mvmlib-0.5.8/requirements.txt
+-rw-r--r--   0        0        0      407 2023-04-18 23:41:39.345293 mvmlib-0.5.8/requirements_dev.txt
+-rw-r--r--   0        0        0     5131 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/DOELib.py
+-rw-r--r--   0        0        0      964 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/__init__.py
+-rw-r--r--   0        0        0   134203 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/designMarginsLib.py
+-rw-r--r--   0        0        0    13107 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/fuzzyLib.py
+-rw-r--r--   0        0        0    29002 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/uncertaintyLib.py
+-rw-r--r--   0        0        0     3299 2023-04-18 23:41:39.345293 mvmlib-0.5.8/src/mvm/utilities.py
+-rw-r--r--   0        0        0      129 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/__init__.py
+-rw-r--r--   0        0        0      539 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/test_doe.py
+-rw-r--r--   0        0        0    14496 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/test_fuzzy.py
+-rw-r--r--   0        0        0    73185 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/test_marginNetwork.py
+-rw-r--r--   0        0        0    14717 2023-04-18 23:41:39.345293 mvmlib-0.5.8/tests/test_probFunction.py
+-rw-r--r--   0        0        0      928 1970-01-01 00:00:00.000000 mvmlib-0.5.8/setup.py
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 mvmlib-0.5.8/PKG-INFO
```

### Comparing `mvmlib-0.5.7/.github/workflows/release.yml` & `mvmlib-0.5.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/.github/workflows/tests_dev.yml` & `mvmlib-0.5.8/.github/workflows/tests_dev.yml`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/.github/workflows/tests_master.yml` & `mvmlib-0.5.8/.github/workflows/tests_master.yml`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/.gitignore` & `mvmlib-0.5.8/.gitignore`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/Makefile` & `mvmlib-0.5.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/api.rst` & `mvmlib-0.5.8/docs/api.rst`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/background.rst` & `mvmlib-0.5.8/docs/background.rst`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/conf.py` & `mvmlib-0.5.8/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'mvmlib'
 copyright = '2021, Khalil Al Handawi'
 author = 'Khalil Al Handawi'
 
 # The full version, including alpha/beta/rc tags
-release = '0.5.7'
+release = '0.5.8'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `mvmlib-0.5.7/docs/getting_started.rst` & `mvmlib-0.5.8/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/history.rst` & `mvmlib-0.5.8/docs/history.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 .. toctree::
    :titlesonly:
 
 *********
 Changelog
 *********
 
+.. _release-0.5.8:
+
+0.5.8
+=====
+
+:Date: April 18, 2023
+
+Fixes
+-----
+* Fix the ``compute_volume`` method to avoid float object TypeError on call to ``math.factorial``
+
 .. _release-0.5.7:
 
 0.5.7
 =====
 
 :Date: March 04, 2023
```

### Comparing `mvmlib-0.5.7/docs/images/TRS_example/load_case.png` & `mvmlib-0.5.8/docs/images/TRS_example/load_case.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/images/efm_example.png` & `mvmlib-0.5.8/docs/images/efm_example.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/images/strut_example/MAN.png` & `mvmlib-0.5.8/docs/images/strut_example/MAN.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/images/strut_example/simplified_strut_model.png` & `mvmlib-0.5.8/docs/images/strut_example/simplified_strut_model.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/images/strut_example/strut_overview.png` & `mvmlib-0.5.8/docs/images/strut_example/strut_overview.png`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/index.rst` & `mvmlib-0.5.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/make.bat` & `mvmlib-0.5.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/notebooks/PDF_examples.ipynb` & `mvmlib-0.5.8/docs/notebooks/PDF_examples.ipynb`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/notebooks/TRS_example.ipynb` & `mvmlib-0.5.8/docs/notebooks/TRS_example.ipynb`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/notebooks/strut_example.ipynb` & `mvmlib-0.5.8/docs/notebooks/strut_example.ipynb`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/docs/refs.bib` & `mvmlib-0.5.8/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/pyproject.toml` & `mvmlib-0.5.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/readme.md` & `mvmlib-0.5.8/readme.md`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/src/mvm/DOELib.py` & `mvmlib-0.5.8/src/mvm/DOELib.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/src/mvm/__init__.py` & `mvmlib-0.5.8/src/mvm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 A library based on the margin value method for computing design 
 margins using fuzzy logic and probabilistic methods for 
 uncertainty modelling
 
 """
 
-__version__ = '0.5.7'
+__version__ = '0.5.8'
 __all__ = ['TriangularFunc', 'FuzzySet', 'FuzzyRule', 'FuzzySystem', 'GaussianFunc', 'UniformFunc', 'Distribution',
            'VisualizeDist', 'compute_cdf', 'Design', 'MarginNode', 'InputSpec', 'FixedParam', 'DesignParam',
            'Behaviour', 'MatrixParam', 'ScalarParam', 'VectorParam', 'Performance', 'MarginNetwork', 'Decision', 'nearest']
 
 from .fuzzyLib import TriangularFunc, FuzzySet, FuzzyRule, FuzzySystem
 from .uncertaintyLib import GaussianFunc, UniformFunc, Distribution, VisualizeDist, compute_cdf
 from .DOELib import Design
```

### Comparing `mvmlib-0.5.7/src/mvm/designMarginsLib.py` & `mvmlib-0.5.8/src/mvm/designMarginsLib.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/src/mvm/fuzzyLib.py` & `mvmlib-0.5.8/src/mvm/fuzzyLib.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/src/mvm/uncertaintyLib.py` & `mvmlib-0.5.8/src/mvm/uncertaintyLib.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,18 +547,18 @@
         -------
         V : float
             volume of hyperellipsoid for Mahalanobis distance r
 
         """
 
         if (self.ndim % 2) == 0:
-            v_d = (np.pi ** (self.ndim / 2)) / np.math.factorial(self.ndim / 2)  # if self.ndim is even
+            v_d = (np.pi ** (self.ndim / 2)) / np.math.factorial(int(self.ndim / 2))  # if self.ndim is even
         else:
             v_d = (2 ** self.ndim) * (np.pi ** ((self.ndim - 1) / 2)) / \
-                  (np.math.factorial((self.ndim - 1) / 2) / np.math.factorial(self.ndim))  # if self.ndim is odd
+                  (np.math.factorial(int((self.ndim - 1) / 2)) / np.math.factorial(self.ndim))  # if self.ndim is odd
 
         return v_d * np.power(np.linalg.det(self.Sigma), 0.5) * (r ** self.ndim)
 
     def compute_density_r(self, r=3):
         """
         Returns the value of probability density at given Mahalanobis distance r
```

### Comparing `mvmlib-0.5.7/src/mvm/utilities.py` & `mvmlib-0.5.8/src/mvm/utilities.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/tests/test_doe.py` & `mvmlib-0.5.8/tests/test_doe.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/tests/test_fuzzy.py` & `mvmlib-0.5.8/tests/test_fuzzy.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/tests/test_marginNetwork.py` & `mvmlib-0.5.8/tests/test_marginNetwork.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/tests/test_probFunction.py` & `mvmlib-0.5.8/tests/test_probFunction.py`

 * *Files identical despite different names*

### Comparing `mvmlib-0.5.7/setup.py` & `mvmlib-0.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 {'doc': ['sphinx', 'sphinx-autobuild', 'nbsphinx'],
  'test': ['pytest>=6.2.5',
           'pytest-cov==3.0.0',
           'pytest-dependency==0.5.1',
           'pandoc']}
 
 setup(name='mvmlib',
-      version='0.5.7',
+      version='0.5.8',
       description='Margin Value Method Library',
       author=None,
       author_email='Khalil Al Handawi <khalil.alhandawi@mail.mcgill.ca>',
       url=None,
       packages=packages,
       package_data=package_data,
       package_dir=package_dir,
```

### Comparing `mvmlib-0.5.7/PKG-INFO` & `mvmlib-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvmlib
-Version: 0.5.7
+Version: 0.5.8
 Summary: Margin Value Method Library
 Author-email: Khalil Al Handawi <khalil.alhandawi@mail.mcgill.ca>
 Requires-Python: >=3.7
 Requires-Dist: matplotlib==3.4.3
 Requires-Dist: pyDOE==0.3.8
 Requires-Dist: scikit-fuzzy==0.4.2
 Requires-Dist: smt==1.1.0
```

