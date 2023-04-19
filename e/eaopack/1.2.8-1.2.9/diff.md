# Comparing `tmp/eaopack-1.2.8.tar.gz` & `tmp/eaopack-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eaopack-1.2.8.tar", last modified: Sat Apr  1 11:06:09 2023, max compression
+gzip compressed data, was "eaopack-1.2.9.tar", last modified: Wed Apr 19 21:16:39 2023, max compression
```

## Comparing `eaopack-1.2.8.tar` & `eaopack-1.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:06:09.644648 eaopack-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-01 11:06:09.644648 eaopack-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-01 11:05:57.000000 eaopack-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:06:09.640648 eaopack-1.2.8/eaopack/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   132279 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/basic_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/network_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    29189 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-04-01 11:05:57.000000 eaopack-1.2.8/eaopack/stoch_lin_prog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:06:09.644648 eaopack-1.2.8/eaopack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-01 11:06:09.000000 eaopack-1.2.8/eaopack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-01 11:06:09.000000 eaopack-1.2.8/eaopack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 11:06:09.000000 eaopack-1.2.8/eaopack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-01 11:06:09.000000 eaopack-1.2.8/eaopack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-01 11:06:09.644648 eaopack-1.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 11:06:09.644648 eaopack-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    38397 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_CHP_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_MIP.py
--rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_asset_freq.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_new_asset_fnct.py
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_periodicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-01 11:05:57.000000 eaopack-1.2.8/tests/test_tz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:16:39.717579 eaopack-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-19 21:16:39.717579 eaopack-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-19 21:16:31.000000 eaopack-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:16:39.713579 eaopack-1.2.9/eaopack/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138235 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14592 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/basic_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/network_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29189 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-04-19 21:16:31.000000 eaopack-1.2.9/eaopack/stoch_lin_prog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:16:39.713579 eaopack-1.2.9/eaopack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-19 21:16:39.000000 eaopack-1.2.9/eaopack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-19 21:16:39.000000 eaopack-1.2.9/eaopack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:16:39.000000 eaopack-1.2.9/eaopack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 21:16:39.000000 eaopack-1.2.9/eaopack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-19 21:16:39.717579 eaopack-1.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:16:39.717579 eaopack-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    45099 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_CHP_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10704 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_MIP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27455 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_asset_freq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_new_asset_fnct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_periodicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-04-19 21:16:31.000000 eaopack-1.2.9/tests/test_tz.py
```

### Comparing `eaopack-1.2.8/PKG-INFO` & `eaopack-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaopack
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Framework for Optimizing Decentralized Portfolios and Green Supply
 Home-page: https://github.com/EnergyAssetOptimization/EAO
 Author: The EAO development Team
 Project-URL: Bug Tracker, https://github.com/EnergyAssetOptimization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `eaopack-1.2.8/README.md` & `eaopack-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/eaopack/assets.py` & `eaopack-1.2.9/eaopack/assets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1129,14 +1129,18 @@
                  min_downtime: float = 0,
                  time_already_off: float = 0,
                  last_dispatch: float = 0,
                  start_ramp_lower_bounds: Sequence = None,
                  start_ramp_upper_bounds: Sequence = None,
                  shutdown_ramp_lower_bounds: Sequence = None,
                  shutdown_ramp_upper_bounds: Sequence = None,
+                 start_ramp_lower_bounds_heat: Sequence = None,
+                 start_ramp_upper_bounds_heat: Sequence = None,
+                 shutdown_ramp_lower_bounds_heat: Sequence = None,
+                 shutdown_ramp_upper_bounds_heat: Sequence = None,
                  ramp_freq: str = None,
                  start_fuel: Union[float, Dict, str] = 0.,
                  fuel_efficiency: Union[float, Dict, str] = 1.,
                  consumption_if_on: Union[float, Dict, str] = 0.
                  ):
         """ CHPContract: Generate heat and power
             Restrictions
@@ -1193,14 +1197,18 @@
             shutdown_ramp_lower_bounds (Sequence): The i-th element of this sequence specifies a lower bound of the
                                                    virtual dispatch (power + conversion_factor_power_heat * heat) at i timesteps
                                                    of freq ramp_freq before turning off. Defaults to None.
             shutdown_ramp_upper_bounds (Sequence): The i-th element of this sequence specifies an upper bound of the
                                                    virtual dispatch (power + conversion_factor_power_heat * heat) at i timesteps
                                                    of freq ramp_freq before turning off. If it is None, it is set equal to shutdown_ramp_upper_bounds.
                                                    Defaults to None.
+            start_ramp_lower_bounds_heat (Sequence): The i-th element of this sequence specifies a lower bound of heat dispatch at i timesteps
+            start_ramp_upper_bounds_heat (Sequence): as above
+            shutdown_ramp_lower_bounds_heat (Sequence): as above
+            shutdown_ramp_upper_bounds_heat (Sequence): as above
             ramp_freq (str): A string specifying the frequency of the start-and shutdown ramp specification.
                              If this is None, the timegrids main_time_unit is used. Otherwise the start and shutdown ramps are
                              interpolated to get values in the timegrids freq.
 
 
             Optional: Explicit fuel consumption (e.g. gas) for multi-commodity simulation
                  start_fuel (float, dict, str): detaults to  0
@@ -1243,14 +1251,28 @@
         self.shutdown_ramp_lower_bounds = shutdown_ramp_lower_bounds
         self.shutdown_ramp_upper_bounds = shutdown_ramp_upper_bounds
         if self.shutdown_ramp_upper_bounds is None:
             self.shutdown_ramp_upper_bounds = self.shutdown_ramp_lower_bounds
         assert self.shutdown_ramp_lower_bounds is None or len(self.shutdown_ramp_lower_bounds) == len(self.shutdown_ramp_upper_bounds), "start_ramp_lower_bounds and start_ramp_upper_bounds cannot have different lengths. Asset: " + self.name
         self.shutdown_ramp_time = len(self.shutdown_ramp_lower_bounds) if self.shutdown_ramp_lower_bounds is not None else 0
         assert np.all([self.shutdown_ramp_lower_bounds[i] <= self.shutdown_ramp_upper_bounds[i] for i in range(self.shutdown_ramp_time)]), "shutdown_ramp_lower_bounds is higher than shutdown_ramp_upper bounds at some point. Asset: " + self.name
+
+        # heat start and shutdown ramps
+        self.start_ramp_lower_bounds_heat = start_ramp_lower_bounds_heat
+        self.start_ramp_upper_bounds_heat = start_ramp_upper_bounds_heat
+        self.shutdown_ramp_lower_bounds_heat = shutdown_ramp_lower_bounds_heat
+        self.shutdown_ramp_upper_bounds_heat = shutdown_ramp_upper_bounds_heat
+        ### Asserts
+        if shutdown_ramp_upper_bounds_heat is not None:
+            assert len(shutdown_ramp_lower_bounds_heat) == len(shutdown_ramp_lower_bounds), 'shutdown lower ramp needs to habe same length for heat and power'
+            assert len(shutdown_ramp_upper_bounds_heat) == len(shutdown_ramp_upper_bounds), 'shutdown upper ramp needs to habe same length for heat and power'
+        if start_ramp_upper_bounds_heat is not None:
+            assert len(start_ramp_upper_bounds_heat) == len(start_ramp_upper_bounds), 'start upper ramp needs to habe same length for heat and power'        
+            assert len(start_ramp_lower_bounds_heat) == len(start_ramp_lower_bounds), 'start lower ramp needs to habe same length for heat and power'        
+
         self.ramp_freq = ramp_freq
 
         if len(nodes) >= 3:
             self.fuel_efficiency      = fuel_efficiency
             self.consumption_if_on    = consumption_if_on
             self.start_fuel           = start_fuel
 
@@ -1287,30 +1309,51 @@
         # Convert start ramp and shutdown ramp from ramp_freq to timegrid.freq
         ramp_freq = self.ramp_freq
         if ramp_freq is None:
             ramp_freq = timegrid.main_time_unit
         start_ramp_time = self.start_ramp_time
         start_ramp_lower_bounds = self.start_ramp_lower_bounds
         start_ramp_upper_bounds = self.start_ramp_upper_bounds
-        shutdown_ramp_time = self.shutdown_ramp_time
+        start_ramp_lower_bounds_heat = self.start_ramp_lower_bounds_heat
+        start_ramp_upper_bounds_heat = self.start_ramp_upper_bounds_heat
+        shutdown_ramp_time = self.shutdown_ramp_time        
         shutdown_ramp_lower_bounds = self.shutdown_ramp_lower_bounds
         shutdown_ramp_upper_bounds = self.shutdown_ramp_upper_bounds
+        shutdown_ramp_lower_bounds_heat = self.shutdown_ramp_lower_bounds_heat
+        shutdown_ramp_upper_bounds_heat = self.shutdown_ramp_upper_bounds_heat
         conversion_factor = convert_time_unit(value=1, old_freq=timegrid.freq, new_freq=timegrid.main_time_unit)
         if self.start_ramp_time:
+            # power
             start_ramp_lower_bounds = self._convert_ramp(self.start_ramp_lower_bounds, ramp_freq)
             start_ramp_upper_bounds = self._convert_ramp(self.start_ramp_upper_bounds, ramp_freq)
             start_ramp_time = len(start_ramp_lower_bounds)
             start_ramp_lower_bounds = start_ramp_lower_bounds * conversion_factor
             start_ramp_upper_bounds = start_ramp_upper_bounds * conversion_factor
+            # heat
+            if start_ramp_lower_bounds_heat is not None:
+                start_ramp_lower_bounds_heat = self._convert_ramp(self.start_ramp_lower_bounds_heat, ramp_freq)
+                start_ramp_upper_bounds_heat = self._convert_ramp(self.start_ramp_upper_bounds_heat, ramp_freq)
+                # start_ramp_time = len(start_ramp_lower_bounds)
+                start_ramp_lower_bounds_heat = start_ramp_lower_bounds_heat * conversion_factor
+                start_ramp_upper_bounds_heat = start_ramp_upper_bounds_heat * conversion_factor
+
         if self.shutdown_ramp_time:
+            # power
             shutdown_ramp_lower_bounds = self._convert_ramp(self.shutdown_ramp_lower_bounds, ramp_freq)
             shutdown_ramp_upper_bounds = self._convert_ramp(self.shutdown_ramp_upper_bounds, ramp_freq)
             shutdown_ramp_time = len(shutdown_ramp_lower_bounds)
             shutdown_ramp_lower_bounds = shutdown_ramp_lower_bounds * conversion_factor
             shutdown_ramp_upper_bounds = shutdown_ramp_upper_bounds * conversion_factor
+            # heat
+            if shutdown_ramp_lower_bounds_heat is not None:
+                shutdown_ramp_lower_bounds_heat = self._convert_ramp(self.shutdown_ramp_lower_bounds_heat, ramp_freq)
+                shutdown_ramp_upper_bounds_heat = self._convert_ramp(self.shutdown_ramp_upper_bounds_heat, ramp_freq)
+                # shutdown_ramp_time = len(shutdown_ramp_lower_bounds)
+                shutdown_ramp_lower_bounds_heat = shutdown_ramp_lower_bounds_heat * conversion_factor
+                shutdown_ramp_upper_bounds_heat = shutdown_ramp_upper_bounds_heat * conversion_factor
 
         min_runtime += start_ramp_time + shutdown_ramp_time
 
         # scale ramp and last dispatch in case timegrid.freq and timegrid.main_time_unit are not equal
         ramp = self.ramp * self.timegrid.restricted.dt[0] if self.ramp is not None else None
         last_dispatch = self.last_dispatch * self.timegrid.restricted.dt[0]
 
@@ -1376,15 +1419,17 @@
         # Add on-, start-, and shutdown-variables:
         op = self._add_bool_variables(op, include_on_variables, include_start_variables, include_shutdown_variables)
 
         # Minimum and maximum capacity:
         op = self._add_constraints_for_min_and_max_cap(op, min_cap, max_cap, time_already_running,
                                                        conversion_factor_power_heat, include_on_variables, start_ramp_time,
                                                        start_ramp_lower_bounds, start_ramp_upper_bounds, shutdown_ramp_time,
-                                                       shutdown_ramp_lower_bounds, shutdown_ramp_upper_bounds)
+                                                       shutdown_ramp_lower_bounds, shutdown_ramp_upper_bounds,
+                                                       start_ramp_lower_bounds_heat, start_ramp_upper_bounds_heat, 
+                                                       shutdown_ramp_lower_bounds_heat, shutdown_ramp_upper_bounds_heat)
 
         # Ramp constraints:
         op = self._add_constraints_for_ramp(op, ramp, conversion_factor_power_heat, time_already_running,
                                             include_on_variables, max_cap, start_ramp_time, shutdown_ramp_time, last_dispatch)
 
         # Start and shutdown constraints:
         op = self._add_constrains_for_start_and_shutdown(op, time_already_running, include_start_variables, include_shutdown_variables)
@@ -1525,15 +1570,17 @@
                 op.u = np.hstack((op.u, np.ones(self.timegrid.restricted.T)))
 
         return op
 
     def _add_constraints_for_min_and_max_cap(self, op, min_cap, max_cap, time_already_running,
                                              conversion_factor_power_heat, include_on_variables, start_ramp_time,
                                              start_ramp_lower_bounds, start_ramp_upper_bounds, shutdown_ramp_time,
-                                             shutdown_ramp_lower_bounds, shutdown_ramp_upper_bounds):
+                                             shutdown_ramp_lower_bounds, shutdown_ramp_upper_bounds,
+                                             start_ramp_lower_bounds_heat, start_ramp_upper_bounds_heat, 
+                                             shutdown_ramp_lower_bounds_heat, shutdown_ramp_upper_bounds_heat):
         """ Add the constraints for the minimum and maximum capacity to op.
 
             These ensure that the virtual dispatch
             (power + conversion_factor_power_heat * heat) is 0 when the asset is "off",
             it is bounded by the start or shutdown specifications during the start and shutdown ramp,
             and otherwise it is between minimum and maximum capacity"""
         # Minimum and maximum capacity:
@@ -1541,20 +1588,20 @@
         A_lower_bounds = sp.lil_matrix((self.n, op.A.shape[1]))
         A_upper_bounds = sp.lil_matrix((self.n, op.A.shape[1]))
         starting_timestep = self.timegrid.restricted.I[0]
         for i in range(start, self.n):
             var = op.mapping.iloc[i]
 
             A_lower_bounds[i, i] = 1
-            A_lower_bounds[i, self.heat_idx + i] = conversion_factor_power_heat[i]
+            A_lower_bounds[i, self.heat_idx + i] = conversion_factor_power_heat[i] 
             if include_on_variables:
                 A_lower_bounds[i, self.on_idx + var["time_step"] - starting_timestep] = - min_cap[i]
 
             A_upper_bounds[i, i] = 1
-            A_upper_bounds[i, self.heat_idx + i] = conversion_factor_power_heat[i]
+            A_upper_bounds[i, self.heat_idx + i] = conversion_factor_power_heat[i] 
             if include_on_variables:
                 A_upper_bounds[i, self.on_idx + var["time_step"] - starting_timestep] = - max_cap[i]
 
             for j in range(start_ramp_time):
                 if i - j < 0:
                     continue
                 A_lower_bounds[i, self.start_idx + i - j] = min_cap[i] - start_ramp_lower_bounds[j]
@@ -1573,14 +1620,55 @@
         op.A = sp.vstack((op.A, A_upper_bounds[start:]))
         op.cType += 'U' * (self.n - start)
         if include_on_variables:
             op.b = np.hstack((op.b, np.zeros(self.n - start)))
         else:
             op.b = np.hstack((op.b, max_cap[start:]))
 
+        # Minimum and maximum capacity for HEAT during start:
+        if shutdown_ramp_lower_bounds_heat is not None:
+            start = max(0, start_ramp_time - time_already_running) if time_already_running > 0 else 0
+            A_lower_bounds = sp.lil_matrix((self.n, op.A.shape[1]))
+            A_upper_bounds = sp.lil_matrix((self.n, op.A.shape[1]))
+            starting_timestep = self.timegrid.restricted.I[0]
+            for i in range(start, self.n):
+                var = op.mapping.iloc[i]
+
+                #A_lower_bounds[i, i] = 1
+                A_lower_bounds[i, self.heat_idx + i] = 1 # conversion_factor_power_heat[i]  
+                A_lower_bounds[i, self.on_idx + var["time_step"] - starting_timestep] = - 0
+
+                #A_upper_bounds[i, i] = 1
+                A_upper_bounds[i, self.heat_idx + i] = 1 # conversion_factor_power_heat[i] 
+                A_upper_bounds[i, self.on_idx + var["time_step"] - starting_timestep] = - max_cap[i]/conversion_factor_power_heat[i] 
+
+                for j in range(start_ramp_time):
+                    if i - j < 0:
+                        continue
+                    A_lower_bounds[i, self.start_idx + i - j] = 0 -start_ramp_lower_bounds_heat[j]
+                    A_upper_bounds[i, self.start_idx + i - j] = max_cap[i]/conversion_factor_power_heat[i] -start_ramp_upper_bounds_heat[j]
+
+                for j in range(shutdown_ramp_time):
+                    if i + j + 1 >= self.timegrid.restricted.T:
+                        break
+                    A_lower_bounds[i, self.shutdown_idx + i + j + 1] = 0 -shutdown_ramp_lower_bounds_heat[j]
+                    A_upper_bounds[i, self.shutdown_idx + i + j + 1] = max_cap[i]/conversion_factor_power_heat[i] -shutdown_ramp_upper_bounds_heat[j]
+
+            op.A = sp.vstack((op.A, A_lower_bounds[start:]))
+            op.cType += 'L' * (self.n - start)
+            op.b = np.hstack((op.b, np.zeros(self.n - start)))
+
+            op.A = sp.vstack((op.A, A_upper_bounds[start:]))
+            op.cType += 'U' * (self.n - start)
+            if include_on_variables:
+                op.b = np.hstack((op.b, np.zeros(self.n - start)))
+            else:
+                op.b = np.hstack((op.b, max_cap[start:]))
+
+
         # Enforce start_ramp if asset is in the starting process at time 0
         if time_already_running > 0 and time_already_running < start_ramp_time:
             for i in range(start_ramp_time - time_already_running):
                 # Upper Bound:
                 a = sp.lil_matrix((1, op.A.shape[1]))
                 a[0, i] = 1
                 a[0, self.heat_idx + i] = conversion_factor_power_heat[i]
@@ -1594,19 +1682,20 @@
                 a[0, self.heat_idx + i] = conversion_factor_power_heat[i]
                 op.A = sp.vstack((op.A, a))
                 op.cType += 'L'
                 op.b = np.hstack((op.b, start_ramp_lower_bounds[time_already_running + i]))
 
         return op
 
-    def _add_constraints_for_ramp(self, op: OptimProblem, ramp, conversion_factor_power_heat, time_already_running, include_on_variables, max_cap, start_ramp_time, shutdown_ramp_time, last_dispatch):
+    def _add_constraints_for_ramp(self, op: OptimProblem, ramp, conversion_factor_power_heat, 
+                                  time_already_running, include_on_variables, max_cap, 
+                                  start_ramp_time, shutdown_ramp_time, last_dispatch):
         """ Add ramp constraints to the OptimProblem op.
-
             These ensure that the increase/decrease of the virtual dispatch (power + conversion_factor_power_heat * heat)
-            is bounded by ramp, except during timesteps that belong to the start or shutdown ramp"""
+            is bounded by ramp, except during timesteps that belong to the start or shutdown ramp """
         # Ramp constraints:
         if ramp is not None:
             for t in range(1, self.timegrid.restricted.T):
                 # Lower Bound
                 a = sp.lil_matrix((1, op.A.shape[1]))
                 a[0, t] = 1
                 a[0, self.heat_idx + t] = conversion_factor_power_heat[t]
```

### Comparing `eaopack-1.2.8/eaopack/basic_classes.py` & `eaopack-1.2.9/eaopack/basic_classes.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/eaopack/io.py` & `eaopack-1.2.9/eaopack/io.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/eaopack/network_graphs.py` & `eaopack-1.2.9/eaopack/network_graphs.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/eaopack/optimization.py` & `eaopack-1.2.9/eaopack/optimization.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/eaopack/portfolio.py` & `eaopack-1.2.9/eaopack/portfolio.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/eaopack/serialization.py` & `eaopack-1.2.9/eaopack/serialization.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/eaopack/stoch_lin_prog.py` & `eaopack-1.2.9/eaopack/stoch_lin_prog.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/eaopack.egg-info/PKG-INFO` & `eaopack-1.2.9/eaopack.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eaopack
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Framework for Optimizing Decentralized Portfolios and Green Supply
 Home-page: https://github.com/EnergyAssetOptimization/EAO
 Author: The EAO development Team
 Project-URL: Bug Tracker, https://github.com/EnergyAssetOptimization/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `eaopack-1.2.8/eaopack.egg-info/SOURCES.txt` & `eaopack-1.2.9/eaopack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/setup.cfg` & `eaopack-1.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eaopack
-version = 1.2.8
+version = 1.2.9
 author = The EAO development Team
 description = A Framework for Optimizing Decentralized Portfolios and Green Supply
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/EnergyAssetOptimization/EAO
 project_urls = 
 	Bug Tracker = https://github.com/EnergyAssetOptimization/issues
```

### Comparing `eaopack-1.2.8/tests/test_CHP_asset.py` & `eaopack-1.2.9/tests/test_CHP_asset.py`

 * *Files 7% similar despite different names*

```diff
@@ -233,15 +233,15 @@
                                 max_cap=10.,
                                 start_costs=1.,
                                 running_costs=5.,
                                 conversion_factor_power_heat= 0.2,
                                 max_share_heat= 1,
                                 start_fuel = 10,
                                 fuel_efficiency= .5,
-                                consumption_if_on= .1)
+                                consumption_if_on= .1) 
         b = eao.assets.SimpleContract(name = 'powerMarket', price='price', nodes = node_power, min_cap=-100, max_cap=100)
         c = eao.assets.SimpleContract(name = 'gasMarket', price='priceGas', nodes = node_gas, min_cap=-100, max_cap=100)
         d = eao.assets.SimpleContract(name = 'heatMarket', price='priceGas', nodes = node_heat, min_cap=-100, max_cap=100)
         prices ={'price': 50.*np.ones(timegrid.T), 'priceGas': 0.1*np.ones(timegrid.T)}
         prices['price'][0:5] = -100.
         portf = eao.portfolio.Portfolio([a, b, c, d])
         op = portf.setup_optim_problem(prices, timegrid=timegrid)
@@ -570,14 +570,135 @@
         start_variables_true[5] = 1
         self.assertAlmostEqual(abs(start_variables_true - start_variables).sum(), 0, 4)
         shutdown_variables_true = np.zeros(timegrid.T)
         shutdown_variables_true[5 + len(start_ramp_interpolated) + len(shutdown_ramp_interpolated)] = 1
         self.assertAlmostEqual(abs(shutdown_variables_true - shutdown_variables).sum(), 0, 4)
 
 
+    def test_start_and_shutdown_ramp_heat_1(self):
+        """ Testing heat start ramp
+        """
+        node_power = eao.assets.Node('node_power')
+        node_heat = eao.assets.Node('node_heat')
+        node_gas = eao.assets.Node('node_gas')
+
+        Start = dt.date(2021, 1, 1)
+        End = dt.date(2021, 1, 2)
+        timegrid = eao.assets.Timegrid(Start, End, freq='h')
+        # start ramps
+        start_ramp_lower_bounds = [10, 20, 30, 40]
+        start_ramp_upper_bounds = [10, 20, 30, 40]
+        shutdown_ramp_lower_bounds = [10, 40, 45, 50, 50]
+        shutdown_ramp_upper_bounds = [10, 40, 45, 50, 50]
+
+        # heat ... NEW
+        start_ramp_lower_bounds_heat = [0, 0, 0, 0]
+        start_ramp_upper_bounds_heat = [0, 100, 100, 100]
+        shutdown_ramp_lower_bounds_heat = [0, 0, 0, 0, 0]
+        shutdown_ramp_upper_bounds_heat = [0, 100, 100, 100, 100]
+
+        a = eao.assets.CHPAsset(name='CHP',
+                                nodes=(node_power, node_heat, node_gas),
+                                min_cap=1.,
+                                max_cap=50.,
+                                start_costs=1.,
+                                running_costs=5.,
+                                conversion_factor_power_heat= 0.2,
+                                max_share_heat= 1,
+                                start_fuel = 10,
+                                fuel_efficiency= .5,
+                                consumption_if_on= .1,
+                                start_ramp_lower_bounds=start_ramp_lower_bounds,
+                                start_ramp_upper_bounds=start_ramp_upper_bounds,
+                                shutdown_ramp_lower_bounds=shutdown_ramp_lower_bounds,
+                                shutdown_ramp_upper_bounds=shutdown_ramp_upper_bounds,                                
+                                start_ramp_lower_bounds_heat=start_ramp_lower_bounds_heat,
+                                start_ramp_upper_bounds_heat=start_ramp_upper_bounds_heat,
+                                shutdown_ramp_lower_bounds_heat=shutdown_ramp_lower_bounds_heat,
+                                shutdown_ramp_upper_bounds_heat=shutdown_ramp_upper_bounds_heat 
+
+                                )
+        b = eao.assets.SimpleContract(name = 'powerMarket', price='price', nodes = node_power, min_cap=-100, max_cap=100)
+        c = eao.assets.SimpleContract(name = 'gasMarket', price='priceGas', nodes = node_gas, min_cap=-100, max_cap=100)
+        d = eao.assets.SimpleContract(name = 'heatMarket', nodes = node_heat, min_cap='heat_demand', max_cap='heat_demand')
+        prices ={'price': -50.*np.ones(timegrid.T), 
+                 'priceGas': 10*np.ones(timegrid.T),
+                 'heat_demand': np.zeros(timegrid.T)}
+        prices['heat_demand'][10:20] = -1
+        portf = eao.portfolio.Portfolio([a, b, c, d])
+        op = portf.setup_optim_problem(prices, timegrid=timegrid)
+        res = op.optimize()
+        out = eao.io.extract_output(portf, op, res, prices)
+        # need to start power an hour before heat
+        self.assertAlmostEqual(out['dispatch']['CHP (node_power)'][9], 10, 4)
+
+    def test_start_and_shutdown_ramp_heat_2(self):
+        """ Testing heat start ramp
+        """
+        node_power = eao.assets.Node('node_power')
+        node_heat = eao.assets.Node('node_heat')
+        node_gas = eao.assets.Node('node_gas')
+
+        Start = dt.date(2021, 1, 1)
+        End = dt.date(2021, 1, 2)
+        timegrid = eao.assets.Timegrid(Start, End, freq='h')
+        # start ramps
+        start_ramp_lower_bounds = [10, 20, 30, 40]
+        start_ramp_upper_bounds = [10, 20, 30, 40]
+        shutdown_ramp_lower_bounds = [10, 40, 45, 50, 50]
+        shutdown_ramp_upper_bounds = [10, 40, 45, 50, 50]
+
+        # heat ... NEW
+        start_ramp_lower_bounds_heat = [1, 2, 3, 4]
+        start_ramp_upper_bounds_heat = [1, 2, 3, 4]
+        shutdown_ramp_lower_bounds_heat = [1, 2, 3, 4, 5]
+        shutdown_ramp_upper_bounds_heat = [1, 2, 3, 4, 5]
+        cr = .2
+        a = eao.assets.CHPAsset(name='CHP',
+                                nodes=(node_power, node_heat, node_gas),
+                                min_cap=1.,
+                                max_cap=50.,
+                                start_costs=0.,
+                                running_costs=5.,
+                                conversion_factor_power_heat= cr,
+                                max_share_heat= 1,
+                                start_fuel = 10,
+                                fuel_efficiency= .5,
+                                consumption_if_on= .1,                     
+                                start_ramp_lower_bounds=start_ramp_lower_bounds,
+                                start_ramp_upper_bounds=start_ramp_upper_bounds,
+                                shutdown_ramp_lower_bounds=shutdown_ramp_lower_bounds,
+                                shutdown_ramp_upper_bounds=shutdown_ramp_upper_bounds,                                
+                                start_ramp_lower_bounds_heat=start_ramp_lower_bounds_heat,
+                                start_ramp_upper_bounds_heat=start_ramp_upper_bounds_heat,
+                                shutdown_ramp_lower_bounds_heat=shutdown_ramp_lower_bounds_heat,
+                                shutdown_ramp_upper_bounds_heat=shutdown_ramp_upper_bounds_heat 
+                                )
+        b = eao.assets.SimpleContract(name = 'powerMarket', price='price', nodes = node_power, min_cap=-100, max_cap=100)
+        c = eao.assets.SimpleContract(name = 'gasMarket', price='priceGas', nodes = node_gas, min_cap=-500, max_cap=500)
+        d = eao.assets.SimpleContract(name = 'heatMarket', nodes = node_heat, min_cap=-100, max_cap=100)
+        prices ={'price': 0.*np.ones(timegrid.T), 
+                 'priceGas': 10*np.ones(timegrid.T)}
+#                 'heat_demand': np.zeros(timegrid.T)}
+#        prices['heat_demand'][10:20] = -1
+        prices['price'][10:20] = 1000
+        portf = eao.portfolio.Portfolio([a, b, c, d])
+        op = portf.setup_optim_problem(prices, timegrid=timegrid)
+        res = op.optimize()
+        out = eao.io.extract_output(portf, op, res, prices)
+        # need to start power an hour before heat
+        myr = out['dispatch']['CHP (node_heat)'][6:10].values
+        myrp = out['dispatch']['CHP (node_power)'][6:10].values
+        myrt = myr*cr+myrp # total
+        # check start ramps are fulfilled
+        for i in range(0,4):
+             self.assertAlmostEqual(myr[i], start_ramp_lower_bounds_heat[i], 4)
+                # check power side ... total virtual dispatch
+             self.assertAlmostEqual(myrt[i], start_ramp_lower_bounds[i], 4)        
+
 class CHPAssetTest_with_threshhold(unittest.TestCase):
 
     def test_basics(self):
         """ Unit test. Test inheritance of CHPAsset class
         """
         node_power = eao.assets.Node('node_power')
         node_heat = eao.assets.Node('node_heat')
```

### Comparing `eaopack-1.2.8/tests/test_MIP.py` & `eaopack-1.2.9/tests/test_MIP.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_asset.py` & `eaopack-1.2.9/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_asset_freq.py` & `eaopack-1.2.9/tests/test_asset_freq.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_io.py` & `eaopack-1.2.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_new_asset_fnct.py` & `eaopack-1.2.9/tests/test_new_asset_fnct.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_optimization.py` & `eaopack-1.2.9/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_periodicity.py` & `eaopack-1.2.9/tests/test_periodicity.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_portfolio.py` & `eaopack-1.2.9/tests/test_portfolio.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_solvers.py` & `eaopack-1.2.9/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `eaopack-1.2.8/tests/test_tz.py` & `eaopack-1.2.9/tests/test_tz.py`

 * *Files identical despite different names*

