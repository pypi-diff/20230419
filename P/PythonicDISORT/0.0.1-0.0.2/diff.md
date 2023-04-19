# Comparing `tmp/PythonicDISORT-0.0.1.tar.gz` & `tmp/PythonicDISORT-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonicDISORT-0.0.1.tar", last modified: Mon Apr 17 22:16:18 2023, max compression
+gzip compressed data, was "PythonicDISORT-0.0.2.tar", last modified: Wed Apr 19 15:08:40 2023, max compression
```

## Comparing `PythonicDISORT-0.0.1.tar` & `PythonicDISORT-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:16:18.085624 PythonicDISORT-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-17 22:16:18.085624 PythonicDISORT-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-04-17 22:15:59.000000 PythonicDISORT-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-17 22:16:00.000000 PythonicDISORT-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 22:16:18.085624 PythonicDISORT-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:16:18.085624 PythonicDISORT-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:16:18.085624 PythonicDISORT-0.0.1/src/PythonicDISORT/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-17 22:16:00.000000 PythonicDISORT-0.0.1/src/PythonicDISORT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12375 2023-04-17 22:16:00.000000 PythonicDISORT-0.0.1/src/PythonicDISORT/_loop_and_assemble_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-17 22:16:00.000000 PythonicDISORT-0.0.1/src/PythonicDISORT/_one_Fourier_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19831 2023-04-17 22:16:00.000000 PythonicDISORT-0.0.1/src/PythonicDISORT/pydisort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-04-17 22:16:00.000000 PythonicDISORT-0.0.1/src/PythonicDISORT/subroutines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 22:16:18.085624 PythonicDISORT-0.0.1/src/PythonicDISORT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-17 22:16:18.000000 PythonicDISORT-0.0.1/src/PythonicDISORT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-17 22:16:18.000000 PythonicDISORT-0.0.1/src/PythonicDISORT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 22:16:18.000000 PythonicDISORT-0.0.1/src/PythonicDISORT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-17 22:16:18.000000 PythonicDISORT-0.0.1/src/PythonicDISORT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-17 22:16:18.000000 PythonicDISORT-0.0.1/src/PythonicDISORT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:08:40.684362 PythonicDISORT-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-19 15:08:40.684362 PythonicDISORT-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-04-19 15:08:22.000000 PythonicDISORT-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 15:08:40.684362 PythonicDISORT-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:08:40.680362 PythonicDISORT-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:08:40.680362 PythonicDISORT-0.0.2/src/PythonicDISORT/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/_loop_and_assemble_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/_one_Fourier_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20045 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/pydisort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-04-19 15:08:23.000000 PythonicDISORT-0.0.2/src/PythonicDISORT/subroutines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:08:40.684362 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 15:08:40.000000 PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/top_level.txt
```

### Comparing `PythonicDISORT-0.0.1/PKG-INFO` & `PythonicDISORT-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.0.1
+Version: 0.0.2
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
-Author-email: Dion Ho <dh3065@columbia.edu>
+Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pytest
 Provides-Extra: notebook_dependencies
 
 # Introduction
 The PythonicDISORT package is a Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 It is coded entirely in Python 3 and in as "Pythonic" a manner as possible: we vectorize as well as use list comprehension and `map` as much as possible. 
 
-It is based on Stamnes' FORTRAN DISORT (see References, in particular [2, 3, 8]) and has its main features: 
+PythonicDISORT is based on Stamnes' FORTRAN DISORT (see References, in particular [2, 3, 8]) and has its main features: 
 delta-M scaling, Nakajima-Tanaka (NT) corrections, only flux option, isotropic internal sources (thermal source),
 Bi-Directional Reflectance Function (BDRF) and more.
 
 This repository also includes our F2PY-wrapped Stamnes DISORT (version 4.0.99) in the `disort4.0.99_f2py` directory.
 The original was downloaded from http://www.rtatmocn.com/disort/. The wrapper was inspired by https://github.com/kconnour/pyRT_DISORT.
 
 # Documentation
 https://pythonic-disort.readthedocs.io/en/latest/
 
-Also see the accompanying Jupyter Notebook: `Pythonic-DISORT.ipynb` in the `docs` directory.
+Also see the accompanying Jupyter Notebook: `Pythonic-DISORT.ipynb` in the `docs` directory 
+at https://github.com/LDEO-CREW/Pythonic-DISORT.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest
 
-Separate from the verification tests in the notebook, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
+Separate from the notebook verification tests, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
 With PyTest installed, execute the console command `pytest` in the `pydisotest` directory to run these tests.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
-* From Conda-forge: (TODO: need to first publish on Conda-forge)
+* From Conda-forge: (TODO: we need to first publish on Conda-forge)
 * By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.17.3`
 * `scipy >= 1.8.0`
 * (OPTIONAL) `pytest >= 6.2.5`
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
 * (OPTIONAL) `ipympl >= 0.8.8`
 
-Our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must also be set up to run the last section (section 6).
+In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must be set up to run the last section (section 6).
 
 ## Compatibility
 
-The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code.
-We are not sure if the Jupyter Notebook or our F2PY-wrapped Stamnes' DISORT will run without issues on non-Windows systems.
+The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code, 
+but we cannot say the same for our Jupyter Notebook and F2PY-wrapped Stamnes' DISORT.
 Everything was built and tested on Windows 11 and not yet tested on other systems.
 
 # References
 1) S. Chandrasekhar. 1960. *Radiative Transfer.*
 
 2) Knut Stamnes and S-Chee Tsay and Warren Wiscombe and Kolf Jayaweera. 1988. *Numerically stable algorithm for discrete-ordinate-method radiative transfer in multiple scattering and emitting layered media.* http://opg.optica.org/ao/abstract.cfm?URI=ao-27-12-2502.
```

### Comparing `PythonicDISORT-0.0.1/README.md` & `PythonicDISORT-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 # Introduction
 The PythonicDISORT package is a Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 It is coded entirely in Python 3 and in as "Pythonic" a manner as possible: we vectorize as well as use list comprehension and `map` as much as possible. 
 
-It is based on Stamnes' FORTRAN DISORT (see References, in particular [2, 3, 8]) and has its main features: 
+PythonicDISORT is based on Stamnes' FORTRAN DISORT (see References, in particular [2, 3, 8]) and has its main features: 
 delta-M scaling, Nakajima-Tanaka (NT) corrections, only flux option, isotropic internal sources (thermal source),
 Bi-Directional Reflectance Function (BDRF) and more.
 
 This repository also includes our F2PY-wrapped Stamnes DISORT (version 4.0.99) in the `disort4.0.99_f2py` directory.
 The original was downloaded from http://www.rtatmocn.com/disort/. The wrapper was inspired by https://github.com/kconnour/pyRT_DISORT.
 
 # Documentation
 https://pythonic-disort.readthedocs.io/en/latest/
 
-Also see the accompanying Jupyter Notebook: `Pythonic-DISORT.ipynb` in the `docs` directory.
+Also see the accompanying Jupyter Notebook: `Pythonic-DISORT.ipynb` in the `docs` directory 
+at https://github.com/LDEO-CREW/Pythonic-DISORT.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest
 
-Separate from the verification tests in the notebook, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
+Separate from the notebook verification tests, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
 With PyTest installed, execute the console command `pytest` in the `pydisotest` directory to run these tests.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
-* From Conda-forge: (TODO: need to first publish on Conda-forge)
+* From Conda-forge: (TODO: we need to first publish on Conda-forge)
 * By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.17.3`
 * `scipy >= 1.8.0`
 * (OPTIONAL) `pytest >= 6.2.5`
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
 * (OPTIONAL) `ipympl >= 0.8.8`
 
-Our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must also be set up to run the last section (section 6).
+In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must be set up to run the last section (section 6).
 
 ## Compatibility
 
-The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code.
-We are not sure if the Jupyter Notebook or our F2PY-wrapped Stamnes' DISORT will run without issues on non-Windows systems.
+The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code, 
+but we cannot say the same for our Jupyter Notebook and F2PY-wrapped Stamnes' DISORT.
 Everything was built and tested on Windows 11 and not yet tested on other systems.
 
 # References
 1) S. Chandrasekhar. 1960. *Radiative Transfer.*
 
 2) Knut Stamnes and S-Chee Tsay and Warren Wiscombe and Kolf Jayaweera. 1988. *Numerically stable algorithm for discrete-ordinate-method radiative transfer in multiple scattering and emitting layered media.* http://opg.optica.org/ao/abstract.cfm?URI=ao-27-12-2502.
```

### Comparing `PythonicDISORT-0.0.1/pyproject.toml` & `PythonicDISORT-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 [project]
 dependencies = [
   "numpy>=1.17.3",
   "scipy>=1.8.0",
 ]
 name = "PythonicDISORT"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Dion Ho", email="dh3065@columbia.edu" },
+  { name="Dion HO Jia Xu", email="dh3065@columbia.edu" },
 ]
 description = "Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `PythonicDISORT-0.0.1/src/PythonicDISORT/_loop_and_assemble_results.py` & `PythonicDISORT-0.0.2/src/PythonicDISORT/_loop_and_assemble_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,17 +178,16 @@
                     ) + B_collect[-1, l, :].T * np.exp(-scaled_tau[None, :] / mu0)
                 else:
                     ulast = np.einsum(
                         "tij, tj -> it", GC_collect[-1, l, :, :], np.exp(exponent), optimize=True
                     )
                 Fourier_error = np.max(
                     np.abs(
-                        (ulast[:, :, None]
-                        * np.cos((NLoops - 1) * (phi0 - phi))[None, None, :])
-                        / np.clip(intensities, a_min = 1e-15, a_max = None)
+                        (ulast[:, :, None] * np.cos((NLoops - 1) * (phi0 - phi))[None, None, :])
+                        / np.clip(intensities, a_min=1e-15, a_max=None)
                     )
                 )
                 return intensities, Fourier_error
             else:
                 return intensities
         # --------------------------------------------------------------------------------------------------------------------------
```

### Comparing `PythonicDISORT-0.0.1/src/PythonicDISORT/_one_Fourier_mode.py` & `PythonicDISORT-0.0.2/src/PythonicDISORT/_one_Fourier_mode.py`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.0.1/src/PythonicDISORT/pydisort.py` & `PythonicDISORT-0.0.2/src/PythonicDISORT/pydisort.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     Leg_coeffs_BDRF=np.array([]),
     s_poly_coeffs=np.array([[]]),
     use_sparse_NLayers=6
 ):
     """Solves the 1D RTE for the fluxes, and optionally intensity,
     of a multi-layer atmosphere with the specified optical properties, boundary conditions
     and sources. Optionally performs delta-M scaling and NT corrections. 
-    See https://pythonic-disort.readthedocs.io/en/latest/PythonicDISORT.html#1.-USER-INPUT-REQUIRED:-Choose-parameters 
-    for a more detailed explanation of each parameter.
-
+    
+        See https://pythonic-disort.readthedocs.io/en/latest/Pythonic-DISORT.html#1.-USER-INPUT-REQUIRED:-Choose-parameters
+        for a more detailed explanation of each parameter.
+        See https://pythonic-disort.readthedocs.io/en/latest/Pythonic-DISORT.html#2.-PythonicDISORT-modules-and-outputs
+        for a more detailed explanation of each output.
 
     Parameters
     ----------
     tau_arr : array
         Optical depth of the lower boundary of each atmospheric layer.
     omega_arr : array
         Single-scattering albedo of each atmospheric layer.
@@ -54,15 +56,15 @@
     NLoops : optional, int
         Number of outermost loops to perform, also number of Fourier modes in the numerical solution.
     b_pos : optional, 2darray or float
         Dirichlet boundary condition for the upward direction.
     b_neg : optional, 2darray or float
         Dirichlet boundary condition for the downward direction.
     only_flux : optional, bool
-        Do NOT compute the intensity function?.
+        Do NOT compute the intensity function?
     f_arr : optional, array
         Fractional scattering into peak for each atmospheric layer.
     NT_cor : optional, bool
         Perform Nakajima-Tanaka intensity corrections?
     Leg_coeffs_BDRF : optional, array
         Unweighted BDRF Legendre coefficients.
     s_poly_coeffs : optional, array
@@ -96,17 +98,17 @@
     s_poly_coeffs = np.atleast_2d(s_poly_coeffs)
     f_arr = np.atleast_1d(f_arr)
     # --------------------------------------------------------------------------------------------------------------------------
     
     # Setup
     # --------------------------------------------------------------------------------------------------------------------------
     NLayers = len(tau_arr)
-    if NLeg == None:
+    if NLeg is None:
         NLeg = NQuad
-    if NLoops == None:
+    if NLoops is None:
         NLoops = NQuad
     scalar_b_pos = False
     scalar_b_neg = False
     thickness_arr = np.concatenate([[tau_arr[0]], np.diff(tau_arr)])
     Nscoeffs = np.shape(s_poly_coeffs)[1]
     NLeg_all = np.shape(Leg_coeffs_all)[1]
     # --------------------------------------------------------------------------------------------------------------------------
@@ -386,22 +388,24 @@
 
         # The corrected intensity
         # --------------------------------------------------------------------------------------------------------------------------
         def u_corrected(tau, phi, return_Fourier_error=False):
             tau = np.atleast_1d(tau)
             phi = np.atleast_1d(phi)
             NT_corrections = TMS_correction(tau, phi)
-            
+
+            # We provide two options below, comment and uncomment as desired.
+            # Option 1 is more computationally efficient but would prevent the use of autograd for testing.
+
             NT_corrections = NT_corrections + np.concatenate(
                 [np.zeros((N, len(tau), len(phi))), IMS_correction(tau, phi)], axis=0
-            )
-            ## The line below is a more computationally efficient implementation of the
-            ## line above but would prevent the use of autograd for testing.
-            #NT_corrections[N:, :, :] += IMS_correction(tau, phi)
-            
+            )  # Option 1
+
+            #NT_corrections[N:, :, :] += IMS_correction(tau, phi)  # Option 2
+
             if return_Fourier_error:
                 u_star_outputs = u_star(tau, phi, True)
                 return (
                     u_star_outputs[0] + np.squeeze(NT_corrections),
                     u_star_outputs[1],
                 )
             else:
```

### Comparing `PythonicDISORT-0.0.1/src/PythonicDISORT/subroutines.py` & `PythonicDISORT-0.0.2/src/PythonicDISORT/subroutines.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,16 +146,16 @@
     full_weights_phi = np.hstack((weights_phi_pos, np.flip(weights_phi_pos[:-1])))
 
     return transform_interval(phi_arr, c, d), transform_weights(full_weights_phi, c, d)
 
 
 def generate_FD_mat(Ntau, a, b):
     """Generates a sparse first derivative matrix in `csr` format with second-order accuracy
-    on [a,b] with Ntau grid points.
-    We use second order forward and backward differences at the boundaries.
+    on [a,b] with `Ntau` grid points.
+    We use second order forward or backward differences at the boundaries.
 
     Parameters
     ----------
     Nphi : int
         Number of grid nodes.
     a : float, optional
         Start of diffentiation interval.
@@ -184,15 +184,16 @@
     first_deriv[-1, -2] = -2 / h
     first_deriv[-1, -3] = 1 / (2 * h)
 
     return tau_arr, first_deriv.asformat("csr")
   
 
 def atleast_2d_append(*arys):
-    """View inputs as arrays with at least two dimensions. Dimensions are added, when necessary, to the back of the shape tuple rather than to the front.
+    """View inputs as arrays with at least two dimensions. 
+    Dimensions are added, when necessary, to the back of the shape tuple rather than to the front.
         
         This is exactly NumPy's `atleast_2d` function but altered to add dimensions to the back of the shape tuple rather than to the front.
         View the documentation for NumPy's `atleast_2d` function at https://numpy.org/doc/stable/reference/generated/numpy.atleast_2d.html.
 
     Parameters
     ----------
     arys1, arys2, ... : array_like
@@ -251,16 +252,16 @@
         G_inv[l, :, :],
         1 / mu_arr,
         optimize=True,
     )
     
     
 def _compare(results, mu_to_compare, reorder_mu, flux_up, flux_down, u):
-    """Performs the pointwise comparisons between results from Stamnes' DISORT
-    which are stored in .npz files against results from PythonicDISORT. Used in our PyTests.
+    """Performs pointwise comparisons between results from Stamnes' DISORT,
+    which are stored in .npz files, against results from PythonicDISORT. Used in our PyTests.
 
     """
     uu = results["uu"]
     flup = results["flup"]
     rfldn = results["rfldn"]
     rfldir = results["rfldir"]
```

### Comparing `PythonicDISORT-0.0.1/src/PythonicDISORT.egg-info/PKG-INFO` & `PythonicDISORT-0.0.2/src/PythonicDISORT.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,69 +1,70 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.0.1
+Version: 0.0.2
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
-Author-email: Dion Ho <dh3065@columbia.edu>
+Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: pytest
 Provides-Extra: notebook_dependencies
 
 # Introduction
 The PythonicDISORT package is a Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 It is coded entirely in Python 3 and in as "Pythonic" a manner as possible: we vectorize as well as use list comprehension and `map` as much as possible. 
 
-It is based on Stamnes' FORTRAN DISORT (see References, in particular [2, 3, 8]) and has its main features: 
+PythonicDISORT is based on Stamnes' FORTRAN DISORT (see References, in particular [2, 3, 8]) and has its main features: 
 delta-M scaling, Nakajima-Tanaka (NT) corrections, only flux option, isotropic internal sources (thermal source),
 Bi-Directional Reflectance Function (BDRF) and more.
 
 This repository also includes our F2PY-wrapped Stamnes DISORT (version 4.0.99) in the `disort4.0.99_f2py` directory.
 The original was downloaded from http://www.rtatmocn.com/disort/. The wrapper was inspired by https://github.com/kconnour/pyRT_DISORT.
 
 # Documentation
 https://pythonic-disort.readthedocs.io/en/latest/
 
-Also see the accompanying Jupyter Notebook: `Pythonic-DISORT.ipynb` in the `docs` directory.
+Also see the accompanying Jupyter Notebook: `Pythonic-DISORT.ipynb` in the `docs` directory 
+at https://github.com/LDEO-CREW/Pythonic-DISORT.
 The Jupyter Notebook provides comprehensive documentation, suggested inputs, explanations, 
 mathematical derivations and verification tests.
 We highly recommend reading the non-optional parts of sections 1 and 2 before use.
 
 ## PyTest
 
-Separate from the verification tests in the notebook, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
+Separate from the notebook verification tests, we used PyTest to recreate most of the test problems from Stamnes et. al.'s `disotest.f90`.
 With PyTest installed, execute the console command `pytest` in the `pydisotest` directory to run these tests.
 
 # Installation
 
 * From PyPI: `pip install PythonicDISORT`
-* From Conda-forge: (TODO: need to first publish on Conda-forge)
+* From Conda-forge: (TODO: we need to first publish on Conda-forge)
 * By cloning repository: `pip install .` in the `Pythonic-DISORT` directory; `pip install -r all_optional_dependencies.txt` to install all optional dependencies
 
 ## Requirements to run PythonicDISORT
 * Python 3.8+
 * `numpy >= 1.17.3`
 * `scipy >= 1.8.0`
 * (OPTIONAL) `pytest >= 6.2.5`
 
 ## Additional requirements to run the Jupyter Notebook
 * `autograd >= 1.5`
 * `jupyter > 1.0.0`
 * `notebook > 6.5.2`
 * (OPTIONAL) `ipympl >= 0.8.8`
 
-Our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must also be set up to run the last section (section 6).
+In addition, our F2PY-wrapped Stamnes' DISORT (in the `disort4.0.99_f2py` directory) must be set up to run the last section (section 6).
 
 ## Compatibility
 
-The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code.
-We are not sure if the Jupyter Notebook or our F2PY-wrapped Stamnes' DISORT will run without issues on non-Windows systems.
+The PythonicDISORT package should be system agnostic given its minimal dependencies and pure Python code, 
+but we cannot say the same for our Jupyter Notebook and F2PY-wrapped Stamnes' DISORT.
 Everything was built and tested on Windows 11 and not yet tested on other systems.
 
 # References
 1) S. Chandrasekhar. 1960. *Radiative Transfer.*
 
 2) Knut Stamnes and S-Chee Tsay and Warren Wiscombe and Kolf Jayaweera. 1988. *Numerically stable algorithm for discrete-ordinate-method radiative transfer in multiple scattering and emitting layered media.* http://opg.optica.org/ao/abstract.cfm?URI=ao-27-12-2502.
```

