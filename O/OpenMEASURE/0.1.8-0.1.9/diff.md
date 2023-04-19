# Comparing `tmp/OpenMEASURE-0.1.8.tar.gz` & `tmp/OpenMEASURE-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OpenMEASURE-0.1.8.tar", last modified: Wed Sep 21 10:03:42 2022, max compression
+gzip compressed data, was "dist/OpenMEASURE-0.1.9.tar", last modified: Fri Sep 23 09:31:35 2022, max compression
```

## Comparing `OpenMEASURE-0.1.8.tar` & `OpenMEASURE-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alberto    (501) staff       (20)        0 2022-09-21 10:03:42.000000 OpenMEASURE-0.1.8/
--rw-r--r--   0 alberto    (501) staff       (20)     1519 2021-12-25 14:43:59.000000 OpenMEASURE-0.1.8/LICENSE.txt
--rw-r--r--   0 alberto    (501) staff       (20)       14 2021-12-25 15:32:30.000000 OpenMEASURE-0.1.8/MANIFEST.in
--rw-r--r--   0 alberto    (501) staff       (20)     6836 2022-09-21 10:03:42.000000 OpenMEASURE-0.1.8/PKG-INFO
--rw-r--r--   0 alberto    (501) staff       (20)     6499 2022-09-20 12:28:57.000000 OpenMEASURE-0.1.8/README.md
--rw-r--r--   0 alberto    (501) staff       (20)       38 2022-09-21 10:03:42.000000 OpenMEASURE-0.1.8/setup.cfg
--rwxr-xr-x   0 alberto    (501) staff       (20)      655 2022-09-21 10:02:17.000000 OpenMEASURE-0.1.8/setup.py
-drwxr-xr-x   0 alberto    (501) staff       (20)        0 2022-09-21 10:03:42.000000 OpenMEASURE-0.1.8/src/
-drwxr-xr-x   0 alberto    (501) staff       (20)        0 2022-09-21 10:03:42.000000 OpenMEASURE-0.1.8/src/OpenMEASURE.egg-info/
--rw-r--r--   0 alberto    (501) staff       (20)     6836 2022-09-21 10:03:41.000000 OpenMEASURE-0.1.8/src/OpenMEASURE.egg-info/PKG-INFO
--rw-r--r--   0 alberto    (501) staff       (20)      269 2022-09-21 10:03:41.000000 OpenMEASURE-0.1.8/src/OpenMEASURE.egg-info/SOURCES.txt
--rw-r--r--   0 alberto    (501) staff       (20)        1 2022-09-21 10:03:41.000000 OpenMEASURE-0.1.8/src/OpenMEASURE.egg-info/dependency_links.txt
--rw-r--r--   0 alberto    (501) staff       (20)       54 2022-09-21 10:03:41.000000 OpenMEASURE-0.1.8/src/OpenMEASURE.egg-info/requires.txt
--rw-r--r--   0 alberto    (501) staff       (20)       19 2022-09-21 10:03:41.000000 OpenMEASURE-0.1.8/src/OpenMEASURE.egg-info/top_level.txt
--rw-r--r--   0 alberto    (501) staff       (20)    18185 2022-09-21 09:42:47.000000 OpenMEASURE-0.1.8/src/gpr.py
--rwxr-xr-x   0 alberto    (501) staff       (20)    34704 2022-09-21 10:02:04.000000 OpenMEASURE-0.1.8/src/sparse_sensing.py
+drwxr-xr-x   0 alberto    (501) staff       (20)        0 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/
+-rw-r--r--   0 alberto    (501) staff       (20)     1519 2021-12-25 14:43:59.000000 OpenMEASURE-0.1.9/LICENSE.txt
+-rw-r--r--   0 alberto    (501) staff       (20)       14 2021-12-25 15:32:30.000000 OpenMEASURE-0.1.9/MANIFEST.in
+-rw-r--r--   0 alberto    (501) staff       (20)     6835 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/PKG-INFO
+-rw-r--r--   0 alberto    (501) staff       (20)     6498 2022-09-23 09:28:41.000000 OpenMEASURE-0.1.9/README.md
+-rw-r--r--   0 alberto    (501) staff       (20)       38 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/setup.cfg
+-rwxr-xr-x   0 alberto    (501) staff       (20)      655 2022-09-23 09:29:58.000000 OpenMEASURE-0.1.9/setup.py
+drwxr-xr-x   0 alberto    (501) staff       (20)        0 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/src/
+drwxr-xr-x   0 alberto    (501) staff       (20)        0 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/src/OpenMEASURE.egg-info/
+-rw-r--r--   0 alberto    (501) staff       (20)     6835 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/src/OpenMEASURE.egg-info/PKG-INFO
+-rw-r--r--   0 alberto    (501) staff       (20)      269 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/src/OpenMEASURE.egg-info/SOURCES.txt
+-rw-r--r--   0 alberto    (501) staff       (20)        1 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/src/OpenMEASURE.egg-info/dependency_links.txt
+-rw-r--r--   0 alberto    (501) staff       (20)       54 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/src/OpenMEASURE.egg-info/requires.txt
+-rw-r--r--   0 alberto    (501) staff       (20)       19 2022-09-23 09:31:35.000000 OpenMEASURE-0.1.9/src/OpenMEASURE.egg-info/top_level.txt
+-rw-r--r--   0 alberto    (501) staff       (20)    18185 2022-09-21 09:42:47.000000 OpenMEASURE-0.1.9/src/gpr.py
+-rwxr-xr-x   0 alberto    (501) staff       (20)    35057 2022-09-23 09:28:37.000000 OpenMEASURE-0.1.9/src/sparse_sensing.py
```

### Comparing `OpenMEASURE-0.1.8/LICENSE.txt` & `OpenMEASURE-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OpenMEASURE-0.1.8/PKG-INFO` & `OpenMEASURE-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenMEASURE
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for soft sensing applications
 Home-page: https://github.com/albertoprocacci/OpenMEASURE
 Author: Alberto Procacci
 Author-email: alberto.procacci@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -172,19 +172,19 @@
     index = np.argmax(C_qr[i,:])
     xz_sensors[i,:2] = xz[index % n_cells, :]
     xz_sensors[i,2] = index // n_cells
 
 plot_sensors(xz_sensors, features, mesh_outline)
 
 # Sample a test simulation using the optimal qr matrix
-y_qr = np.zeros((n_sensors,2))
+y_qr = np.ones((n_sensors,3))
 y_qr[:,0] = C_qr @ X_test[:,3]
 
 for i in range(n_sensors):
-    y_qr[i,1] = np.argmax(C_qr[i,:]) // n_cells
+    y_qr[i,2] = np.argmax(C_qr[i,:]) // n_cells
 
 # Fit the model and predict the low-dim vector (ap) and the high-dim solution (xp)
 ap, xp = spr.fit_predict(C_qr, y_qr)
 
 # Select the feature to plot
 str_ind = 'T'
 ind = features.index(str_ind)
```

### Comparing `OpenMEASURE-0.1.8/README.md` & `OpenMEASURE-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -160,19 +160,19 @@
     index = np.argmax(C_qr[i,:])
     xz_sensors[i,:2] = xz[index % n_cells, :]
     xz_sensors[i,2] = index // n_cells
 
 plot_sensors(xz_sensors, features, mesh_outline)
 
 # Sample a test simulation using the optimal qr matrix
-y_qr = np.zeros((n_sensors,2))
+y_qr = np.ones((n_sensors,3))
 y_qr[:,0] = C_qr @ X_test[:,3]
 
 for i in range(n_sensors):
-    y_qr[i,1] = np.argmax(C_qr[i,:]) // n_cells
+    y_qr[i,2] = np.argmax(C_qr[i,:]) // n_cells
 
 # Fit the model and predict the low-dim vector (ap) and the high-dim solution (xp)
 ap, xp = spr.fit_predict(C_qr, y_qr)
 
 # Select the feature to plot
 str_ind = 'T'
 ind = features.index(str_ind)
```

### Comparing `OpenMEASURE-0.1.8/setup.py` & `OpenMEASURE-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
       name='OpenMEASURE',
-      version='0.1.8',
+      version='0.1.9',
       description='Python package for soft sensing applications',
       py_modules=['sparse_sensing', 'gpr'],
       package_dir={'':'src'},
       long_description=long_description,
       long_description_content_type='text/markdown',
       install_requires=['numpy>=1.19', 'scipy>=1.7.1', 'gpytorch>=1.5.1', 
                         'cvxpy>=1.1.3'],
```

### Comparing `OpenMEASURE-0.1.8/src/OpenMEASURE.egg-info/PKG-INFO` & `OpenMEASURE-0.1.9/src/OpenMEASURE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenMEASURE
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for soft sensing applications
 Home-page: https://github.com/albertoprocacci/OpenMEASURE
 Author: Alberto Procacci
 Author-email: alberto.procacci@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -172,19 +172,19 @@
     index = np.argmax(C_qr[i,:])
     xz_sensors[i,:2] = xz[index % n_cells, :]
     xz_sensors[i,2] = index // n_cells
 
 plot_sensors(xz_sensors, features, mesh_outline)
 
 # Sample a test simulation using the optimal qr matrix
-y_qr = np.zeros((n_sensors,2))
+y_qr = np.ones((n_sensors,3))
 y_qr[:,0] = C_qr @ X_test[:,3]
 
 for i in range(n_sensors):
-    y_qr[i,1] = np.argmax(C_qr[i,:]) // n_cells
+    y_qr[i,2] = np.argmax(C_qr[i,:]) // n_cells
 
 # Fit the model and predict the low-dim vector (ap) and the high-dim solution (xp)
 ap, xp = spr.fit_predict(C_qr, y_qr)
 
 # Select the feature to plot
 str_ind = 'T'
 ind = features.index(str_ind)
```

### Comparing `OpenMEASURE-0.1.8/src/gpr.py` & `OpenMEASURE-0.1.9/src/gpr.py`

 * *Files identical despite different names*

### Comparing `OpenMEASURE-0.1.8/src/sparse_sensing.py` & `OpenMEASURE-0.1.9/src/sparse_sensing.py`

 * *Files 2% similar despite different names*

```diff
@@ -442,35 +442,36 @@
     def scale_vector(self, y):
         '''
         Return the scaled measurement vector.
 
         Parameters
         ----------
         y : numpy array
-            Measurement vector to scale, size (s,2). The first column contains
-            the measurements, the second column contains which feature is 
-            measured.
+            The measurement vector, size (s,3). The first column contains
+            the measurements, the second column contains the uncertainty (std deviation), 
+            and the third column contains which feature is measured.
 
         Returns
         -------
         y0: numpy array
-            The scaled measurement vector.
+            The scaled measurement vector, size (s,2).
 
         '''
         
-        y0 = np.zeros((y.shape[0],))
+        y0 = np.zeros((y.shape[0],2))
         cnt_vector = np.zeros((self.n_features))
         scl_vector = np.zeros((self.n_features))
         
         for i in range(self.n_features):
             cnt_vector[i] = self.X_cnt[i*self.n_points,0]
             scl_vector[i] = self.X_scl[i*self.n_points,0]
         
         for i in range(y0.shape[0]):
-            y0[i] = (y[i,0] - cnt_vector[int(y[i,1])]) / scl_vector[int(y[i,1])]
+            y0[i,0] = (y[i,0] - cnt_vector[int(y[i,2])]) / scl_vector[int(y[i,2])]
+            y0[i,1] = y[i,1] / scl_vector[int(y[i,2])]
         
         return y0
 
     def gem(self, Ur, n_sensors, mask, d_min, verbose):
         '''
         Selects the best sensors' placement based on a greedy entropy maximization
         algorithm.
@@ -674,17 +675,17 @@
 
         Parameters
         ----------
         C : numpy array
             The measurement matrix, size (s,n).
         
         y : numpy array
-            The measurement vector, size (s,2). The first column contains
-            the measurements, the second column contains which feature is 
-            measured.
+            The measurement vector, size (s,3). The first column contains
+            the measurements, the second column contains the uncertainty (std deviation), 
+            and the third column contains which feature is measured.
         
         scale_type : str, optional
             Type of scaling method. The default is 'std'. Standard scaling is the 
             only scaling implemented for the 'COLS' method.
         
         select_modes : str, optional
             Type of mode selection. The default is 'variance'. The available 
@@ -695,20 +696,23 @@
             99, which represents 99% of the variance. If select_modes='number',
             n_modes represents the number of modes retained.
 
         method : str, optional
             Method used to comupte the solution of the y0 = Theta * a linear 
             system. The choice are 'OLS' or 'COLS' which is constrained OLS. The
             default is 'OLS'.
+            
         solver : str, optional
             Solver used for the constrained optimization problem. Only used if 
             the method selected is 'COLS'. The default is 'ECOS'.
+            
         abstol : float, optional
             The absolute tolerance used to terminate the constrained optimization
             problem. The default is 1e-3.
+            
         verbose : bool, optional
             If True, it displays the output from the constrained optimiziation 
             solver. The default is False
 
         Returns
         -------
         
@@ -721,15 +725,15 @@
         '''
         if C.shape[0] != y.shape[0]:
             raise ValueError('The number of rows of C does not match the number' \
                              ' of rows of y.')
         if C.shape[1] != self.X.shape[0]:
             raise ValueError('The number of columns of C does not match the number' \
                               ' of rows of X.')
-        if y.shape[1] != 2:
+        if y.shape[1] != 3:
             raise ValueError('The y array has the wrong number of columns. y has' \
                               ' to have dimensions (s,2).')
         
         self.scale_type = scale_type
         X0 = SPR.scale_data(self, scale_type)
         U, A, exp_variance = SPR.decomposition(self, X0)
         Ur, Ar = SPR.reduction(self, U, A, exp_variance, select_modes, n_modes)
@@ -758,42 +762,43 @@
         '''
         Return the prediction vector. 
         This method has to be used after fit_predict.
 
         Parameters
         ----------
         y : numpy array
-            The measurement vector, size (s,2). The first column contains
-            the measurements, the second column contains which feature is 
-            measured.
+            The measurement vector, size (s,3). The first column contains
+            the measurements, the second column contains the uncertainty (std deviation), 
+            and the third column contains which feature is measured.
 
         Returns
         -------
         ar : numpy array
             The low-dimensional projection of the state of the system, size (r,)
         x_rec : numpy array
             The reconstructed error, size (n,).
 
         '''
         if hasattr(self, 'Theta'):
             y0 = SPR.scale_vector(self, y)
+            W = np.diag(1/y0[:,1])  #Weights used for the weighted OLS and COLS
             
             if self.method == 'OLS':
                 
-                ar, res, rank, s = la.lstsq(self.Theta, y0)
+                ar, res, rank, s = la.lstsq(W @ self.Theta, W @ y0[:,0])
                 x0_rec = self.Ur @ ar
         
             elif self.method == 'COLS':
                 r = self.Theta.shape[1]
                 g = cp.Variable(r)
                 
                 x0_tilde = self.Ur @ g
                 x_tilde = SPR.unscale_data(self, x0_tilde)
                 
-                objective = cp.Minimize(cp.pnorm(y0 - self.Theta @ g, p=2))
+                objective = cp.Minimize(cp.pnorm(W @ (y0[:,0] - self.Theta @ g), p=2))
                 constrs = [x_tilde >= 0]
                 prob = cp.Problem(objective, constrs)
                 min_value = prob.solve(solver=self.solver, abstol=self.abstol, 
                                         verbose=self.verbose)
                 ar = g.value
                 x0_rec = self.Ur @ ar
             
@@ -927,36 +932,35 @@
 
     #---------------------------------Sparse sensing--------------------------------------------------
 
     spr = SPR(X_train, n_features, xyz) # Create the spr object
 
     # Compute the optimal measurement matrix using qr decomposition
     n_sensors = 14
-    C_qr = spr.optimal_placement(select_modes='number', n_modes=n_sensors, scale_type='pareto')
+    C_qr = spr.optimal_placement(select_modes='number', n_modes=n_sensors)
 
     # Get the sensors positions and features
     xz_sensors = np.zeros((n_sensors, 4))
     for i in range(n_sensors):
         index = np.argmax(C_qr[i,:])
         xz_sensors[i,:2] = xz[index % n_cells, :]
         xz_sensors[i,2] = index // n_cells
 
     plot_sensors(xz_sensors, features, mesh_outline)
 
     # Sample a test simulation using the optimal qr matrix
-    y_qr = np.zeros((n_sensors,2))
+    y_qr = np.ones((n_sensors,3))
     y_qr[:,0] = C_qr @ X_test[:,3]
 
     for i in range(n_sensors):
-        y_qr[i,1] = np.argmax(C_qr[i,:]) // n_cells
+        y_qr[i,2] = np.argmax(C_qr[i,:]) // n_cells
 
     # Fit the model and predict the low-dim vector (ap) and the high-dim solution (xp)
-    ap, xp = spr.fit_predict(C_qr, y_qr, scale_type='pareto')
+    ap, xp = spr.fit_predict(C_qr, y_qr)
 
     # Select the feature to plot
     str_ind = 'T'
     ind = features.index(str_ind)
 
     plot_contours_tri(xz[:,0], xz[:,1], [X_test[ind*n_cells:(ind+1)*n_cells, 3], 
                     xp[ind*n_cells:(ind+1)*n_cells]], cbar_label=str_ind)
-
```

