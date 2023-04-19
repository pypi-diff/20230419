# Comparing `tmp/emantis-1.0.2.tar.gz` & `tmp/emantis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emantis-1.0.2.tar", last modified: Wed Mar 15 18:27:33 2023, max compression
+gzip compressed data, was "emantis-1.0.3.tar", last modified: Wed Apr 19 09:28:27 2023, max compression
```

## Comparing `emantis-1.0.2.tar` & `emantis-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-03-15 18:27:33.905525 emantis-1.0.2/
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)      109 2023-03-10 11:06:15.000000 emantis-1.0.2/MANIFEST.in
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     3427 2023-03-15 18:27:33.905525 emantis-1.0.2/PKG-INFO
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     2528 2023-03-15 18:24:43.000000 emantis-1.0.2/README.rst
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     1264 2023-03-15 09:50:02.000000 emantis-1.0.2/pyproject.toml
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)       38 2023-03-15 18:27:33.905525 emantis-1.0.2/setup.cfg
-drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-03-15 18:27:33.897525 emantis-1.0.2/src/
-drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-03-15 18:27:33.897525 emantis-1.0.2/src/emantis/
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)       44 2023-03-10 08:51:23.000000 emantis-1.0.2/src/emantis/__init__.py
-drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-03-15 18:27:33.897525 emantis-1.0.2/src/emantis/data/
-drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-03-15 18:27:33.901525 emantis-1.0.2/src/emantis/data/fofr_matter_power_boost/
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     8309 2023-03-10 08:51:23.000000 emantis-1.0.2/src/emantis/data/fofr_matter_power_boost/cosmo_params.txt
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     3496 2023-03-10 08:51:23.000000 emantis-1.0.2/src/emantis/data/fofr_matter_power_boost/kbins.h5
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)  1515040 2023-03-10 08:51:23.000000 emantis-1.0.2/src/emantis/data/fofr_matter_power_boost/power_boosts_train.h5
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)    23119 2023-03-15 09:45:35.000000 emantis-1.0.2/src/emantis/powerspectrum_matter.py
-drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-03-15 18:27:33.901525 emantis-1.0.2/src/emantis.egg-info/
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     3427 2023-03-15 18:27:33.000000 emantis-1.0.2/src/emantis.egg-info/PKG-INFO
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)      442 2023-03-15 18:27:33.000000 emantis-1.0.2/src/emantis.egg-info/SOURCES.txt
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)        1 2023-03-15 18:27:33.000000 emantis-1.0.2/src/emantis.egg-info/dependency_links.txt
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)       71 2023-03-15 18:27:33.000000 emantis-1.0.2/src/emantis.egg-info/requires.txt
--rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)        8 2023-03-15 18:27:33.000000 emantis-1.0.2/src/emantis.egg-info/top_level.txt
+drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-04-19 09:28:27.348382 emantis-1.0.3/
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)    35149 2023-03-10 08:51:23.000000 emantis-1.0.3/COPYING
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)      109 2023-03-10 11:06:15.000000 emantis-1.0.3/MANIFEST.in
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     3571 2023-04-19 09:28:27.348382 emantis-1.0.3/PKG-INFO
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     2650 2023-03-20 13:48:30.000000 emantis-1.0.3/README.rst
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     1264 2023-04-19 09:20:24.000000 emantis-1.0.3/pyproject.toml
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)       38 2023-04-19 09:28:27.348382 emantis-1.0.3/setup.cfg
+drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-04-19 09:28:27.340382 emantis-1.0.3/src/
+drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-04-19 09:28:27.344382 emantis-1.0.3/src/emantis/
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)       44 2023-03-10 08:51:23.000000 emantis-1.0.3/src/emantis/__init__.py
+drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-04-19 09:28:27.344382 emantis-1.0.3/src/emantis/data/
+drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-04-19 09:28:27.344382 emantis-1.0.3/src/emantis/data/fofr_matter_power_boost/
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     8309 2023-03-10 08:51:23.000000 emantis-1.0.3/src/emantis/data/fofr_matter_power_boost/cosmo_params.txt
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     3496 2023-03-10 08:51:23.000000 emantis-1.0.3/src/emantis/data/fofr_matter_power_boost/kbins.h5
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)  1515040 2023-03-10 08:51:23.000000 emantis-1.0.3/src/emantis/data/fofr_matter_power_boost/power_boosts_train.h5
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)    23134 2023-04-19 09:15:33.000000 emantis-1.0.3/src/emantis/powerspectrum_matter.py
+drwxrwxr-x   0 isaezcasares  (1001) isaezcasares  (1001)        0 2023-04-19 09:28:27.344382 emantis-1.0.3/src/emantis.egg-info/
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)     3571 2023-04-19 09:28:27.000000 emantis-1.0.3/src/emantis.egg-info/PKG-INFO
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)      450 2023-04-19 09:28:27.000000 emantis-1.0.3/src/emantis.egg-info/SOURCES.txt
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)        1 2023-04-19 09:28:27.000000 emantis-1.0.3/src/emantis.egg-info/dependency_links.txt
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)       71 2023-04-19 09:28:27.000000 emantis-1.0.3/src/emantis.egg-info/requires.txt
+-rw-rw-r--   0 isaezcasares  (1001) isaezcasares  (1001)        8 2023-04-19 09:28:27.000000 emantis-1.0.3/src/emantis.egg-info/top_level.txt
```

### Comparing `emantis-1.0.2/PKG-INFO` & `emantis-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: emantis
-Version: 1.0.2
+Version: 1.0.3
 Summary: A cosmological emulator for non-linear large-scale structure formation studies in extended dark energy and gravity theories.
 Author-email: Iñigo Sáez-Casares <inigo.saez-casares@obspm.fr>
 License: GNU GPLv3
 Project-URL: documentation, https://e-mantis.pages.obspm.fr/e-mantis/index.html
 Project-URL: repository, https://gitlab.obspm.fr/e-mantis/e-mantis.git
 Project-URL: tracker, https://gitlab.obspm.fr/e-mantis/e-mantis/-/issues
 Keywords: cosmology,emulator,large-scale structure,dark energy,modified gravity,non-linear
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
+License-File: COPYING
 
 |PyPI|_ |DOI|_
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/emantis
 .. _PyPI: https://pypi.org/project/emantis/
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7738363.svg
@@ -33,16 +34,16 @@
 -----------
 
 e-MANTIS is an emulator for the study of the non-linear large-scale structure formation in the context
 of alternative dark energy and gravity theories.
 It uses Gaussian Processes to perform a fast and accurate interpolation between the outputs of
 high resolution cosmological N-body simulations.
 Currently, e-MANTIS is able to give predictions for the following quantities:
-   
-* Matter power spectrum boost in :math:`f(R)` gravity (described in <cite paper>).
+
+* Matter power spectrum boost in :math:`f(R)` gravity, described in `The e-MANTIS emulator: fast predictions of the non-linear matter power spectrum in f(R)CDM cosmology <https://arxiv.org/abs/2303.08899>`_.
 
 Please cite the corresponding papers if you use e-MANTIS in your work.
 
 More observables and cosmological models will be added in the future. Stay tuned!
 
 Installation
 ------------
```

### Comparing `emantis-1.0.2/README.rst` & `emantis-1.0.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 -----------
 
 e-MANTIS is an emulator for the study of the non-linear large-scale structure formation in the context
 of alternative dark energy and gravity theories.
 It uses Gaussian Processes to perform a fast and accurate interpolation between the outputs of
 high resolution cosmological N-body simulations.
 Currently, e-MANTIS is able to give predictions for the following quantities:
-   
-* Matter power spectrum boost in :math:`f(R)` gravity (described in <cite paper>).
+
+* Matter power spectrum boost in :math:`f(R)` gravity, described in `The e-MANTIS emulator: fast predictions of the non-linear matter power spectrum in f(R)CDM cosmology <https://arxiv.org/abs/2303.08899>`_.
 
 Please cite the corresponding papers if you use e-MANTIS in your work.
 
 More observables and cosmological models will be added in the future. Stay tuned!
 
 Installation
 ------------
```

### Comparing `emantis-1.0.2/pyproject.toml` & `emantis-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "emantis"
 
 authors = [
     {name = "Iñigo Sáez-Casares", email = "inigo.saez-casares@obspm.fr"},
 ]
 
-version = "1.0.2"
+version = "1.0.3"
 description = "A cosmological emulator for non-linear large-scale structure formation studies in extended dark energy and gravity theories."
 readme = "README.rst"
 license = {text = "GNU GPLv3"}
 
 dependencies = [
     "numpy",
     "h5py",
```

### Comparing `emantis-1.0.2/src/emantis/data/fofr_matter_power_boost/cosmo_params.txt` & `emantis-1.0.3/src/emantis/data/fofr_matter_power_boost/cosmo_params.txt`

 * *Files identical despite different names*

### Comparing `emantis-1.0.2/src/emantis/data/fofr_matter_power_boost/kbins.h5` & `emantis-1.0.3/src/emantis/data/fofr_matter_power_boost/kbins.h5`

 * *Files identical despite different names*

### Comparing `emantis-1.0.2/src/emantis/data/fofr_matter_power_boost/power_boosts_train.h5` & `emantis-1.0.3/src/emantis/data/fofr_matter_power_boost/power_boosts_train.h5`

 * *Files identical despite different names*

### Comparing `emantis-1.0.2/src/emantis/powerspectrum_matter.py` & `emantis-1.0.3/src/emantis/powerspectrum_matter.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,26 +245,26 @@
                 # linearly interpolate between the two closest
                 # precomputed scale factor nodes.
                 aexp_low, aexp_up = aexp_neighbours[a][0], aexp_neighbours[a][1]
                 boost_pred[i] = self._lin_interp(
                     a,
                     aexp_low,
                     aexp_up,
-                    boost_pred[aexp_low],
-                    boost_pred[aexp_up],
+                    boost_aexp_nodes[aexp_low],
+                    boost_aexp_nodes[aexp_up],
                 )
 
         # If a single cosmological model and a single scale factor have been requested return a 1D array.
         if nmodels * naexp == 1:
             return np.ravel(boost_pred)
         else:
             return boost_pred
 
     # TODO maybe move this to a separate "utils" module.
-    def _lin_interp(x0, x1, x2, y1, y2):
+    def _lin_interp(self, x0, x1, x2, y1, y2):
         """Performs a linear interpolation.
 
         Linearly interpolates at location *x0* between two nodes *x1* and *x2*, with
         values *y1* and *y2* respectively.
 
         It assumes that *x1* < *x0* < *x2*.
 
@@ -316,15 +316,15 @@
         # Loop over all the requested scale factors.
         for a in aexp:
             # If the scale factor is an emulator node add it to the list of required nodes.
             if a in self.aexp_nodes:
                 aexp_nodes.append(a)
             # Otherwise find the two closest nodes and add them to the list of required nodes and to the neighbours dict.
             else:
-                aexp_low, aexp_up = self._find_neighbour_aexp_nodes(aexp)
+                aexp_low, aexp_up = self._find_neighbour_aexp_nodes(a)
                 aexp_nodes.extend([aexp_low, aexp_up])
                 aexp_neighbours[a] = [aexp_low, aexp_up]
 
         # Sort and remove duplicate entries in the required nodes list.
         aexp_nodes = np.unique(aexp_nodes)
 
         return aexp_nodes, aexp_neighbours
```

### Comparing `emantis-1.0.2/src/emantis.egg-info/PKG-INFO` & `emantis-1.0.3/src/emantis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: emantis
-Version: 1.0.2
+Version: 1.0.3
 Summary: A cosmological emulator for non-linear large-scale structure formation studies in extended dark energy and gravity theories.
 Author-email: Iñigo Sáez-Casares <inigo.saez-casares@obspm.fr>
 License: GNU GPLv3
 Project-URL: documentation, https://e-mantis.pages.obspm.fr/e-mantis/index.html
 Project-URL: repository, https://gitlab.obspm.fr/e-mantis/e-mantis.git
 Project-URL: tracker, https://gitlab.obspm.fr/e-mantis/e-mantis/-/issues
 Keywords: cosmology,emulator,large-scale structure,dark energy,modified gravity,non-linear
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/x-rst
+License-File: COPYING
 
 |PyPI|_ |DOI|_
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/emantis
 .. _PyPI: https://pypi.org/project/emantis/
 
 .. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7738363.svg
@@ -33,16 +34,16 @@
 -----------
 
 e-MANTIS is an emulator for the study of the non-linear large-scale structure formation in the context
 of alternative dark energy and gravity theories.
 It uses Gaussian Processes to perform a fast and accurate interpolation between the outputs of
 high resolution cosmological N-body simulations.
 Currently, e-MANTIS is able to give predictions for the following quantities:
-   
-* Matter power spectrum boost in :math:`f(R)` gravity (described in <cite paper>).
+
+* Matter power spectrum boost in :math:`f(R)` gravity, described in `The e-MANTIS emulator: fast predictions of the non-linear matter power spectrum in f(R)CDM cosmology <https://arxiv.org/abs/2303.08899>`_.
 
 Please cite the corresponding papers if you use e-MANTIS in your work.
 
 More observables and cosmological models will be added in the future. Stay tuned!
 
 Installation
 ------------
```

