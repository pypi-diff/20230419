# Comparing `tmp/powergridsim-0.0.1.tar.gz` & `tmp/powergridsim-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powergridsim-0.0.1.tar", last modified: Mon Mar  6 18:00:01 2023, max compression
+gzip compressed data, was "powergridsim-1.0.0.tar", last modified: Wed Apr 19 18:30:26 2023, max compression
```

## Comparing `powergridsim-0.0.1.tar` & `powergridsim-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-03-06 18:00:01.827771 powergridsim-0.0.1/
--rw-r--r--   0 jf3375     (502) staff       (20)      586 2023-03-06 18:00:01.827622 powergridsim-0.0.1/PKG-INFO
-drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-03-06 18:00:01.824482 powergridsim-0.0.1/powergridsim/
--rw-r--r--   0 jf3375     (502) staff       (20)      742 2023-03-06 17:49:23.000000 powergridsim-0.0.1/powergridsim/__init__.py
-drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-03-06 18:00:01.827092 powergridsim-0.0.1/powergridsim/models_gurobi/
--rw-r--r--   0 jf3375     (502) staff       (20)      797 2023-02-21 21:44:18.000000 powergridsim-0.0.1/powergridsim/models_gurobi/__init__.py
--rw-r--r--   0 jf3375     (502) staff       (20)     2112 2023-02-21 01:25:18.000000 powergridsim-0.0.1/powergridsim/models_gurobi/_status_vars_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)    12518 2023-02-21 01:25:18.000000 powergridsim-0.0.1/powergridsim/models_gurobi/generation_limits_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)      727 2023-02-21 01:25:18.000000 powergridsim-0.0.1/powergridsim/models_gurobi/non_dispatchable_vars_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)     7686 2023-03-03 16:59:44.000000 powergridsim-0.0.1/powergridsim/models_gurobi/objective_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)    68183 2023-02-20 19:39:14.000000 powergridsim-0.0.1/powergridsim/models_gurobi/params_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)    29651 2023-03-03 18:01:23.000000 powergridsim-0.0.1/powergridsim/models_gurobi/power_balance_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)     5932 2023-02-21 01:58:56.000000 powergridsim-0.0.1/powergridsim/models_gurobi/power_vars_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)    10913 2023-03-03 17:28:27.000000 powergridsim-0.0.1/powergridsim/models_gurobi/production_costs_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)     8107 2023-02-21 01:25:18.000000 powergridsim-0.0.1/powergridsim/models_gurobi/ramping_limits_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)     2461 2023-03-03 14:18:54.000000 powergridsim-0.0.1/powergridsim/models_gurobi/reserve_requirement_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)     3726 2023-02-21 01:25:18.000000 powergridsim-0.0.1/powergridsim/models_gurobi/reserve_vars_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)     3485 2023-02-17 20:11:06.000000 powergridsim-0.0.1/powergridsim/models_gurobi/services_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)     6395 2023-03-03 17:34:08.000000 powergridsim-0.0.1/powergridsim/models_gurobi/startup_costs_gurobi.py
-drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-03-06 18:00:01.827453 powergridsim-0.0.1/powergridsim/models_gurobi/transmission_gurobi/
--rw-r--r--   0 jf3375     (502) staff       (20)        0 2023-02-21 01:06:17.000000 powergridsim-0.0.1/powergridsim/models_gurobi/transmission_gurobi/__init__.py
--rw-r--r--   0 jf3375     (502) staff       (20)    20325 2023-02-21 18:47:40.000000 powergridsim-0.0.1/powergridsim/models_gurobi/transmission_gurobi/branch.py
--rw-r--r--   0 jf3375     (502) staff       (20)     3967 2023-02-21 18:43:42.000000 powergridsim-0.0.1/powergridsim/models_gurobi/transmission_gurobi/bus.py
--rw-r--r--   0 jf3375     (502) staff       (20)     5138 2023-03-03 17:16:42.000000 powergridsim-0.0.1/powergridsim/models_gurobi/uptime_downtime_gurobi.py
--rw-r--r--   0 jf3375     (502) staff       (20)      167 2023-02-21 00:45:59.000000 powergridsim-0.0.1/powergridsim/models_gurobi/utils_gurobi.py
-drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-03-06 18:00:01.825085 powergridsim-0.0.1/powergridsim.egg-info/
--rw-r--r--   0 jf3375     (502) staff       (20)      586 2023-03-06 18:00:01.000000 powergridsim-0.0.1/powergridsim.egg-info/PKG-INFO
--rw-r--r--   0 jf3375     (502) staff       (20)     1181 2023-03-06 18:00:01.000000 powergridsim-0.0.1/powergridsim.egg-info/SOURCES.txt
--rw-r--r--   0 jf3375     (502) staff       (20)        1 2023-03-06 18:00:01.000000 powergridsim-0.0.1/powergridsim.egg-info/dependency_links.txt
--rw-r--r--   0 jf3375     (502) staff       (20)        7 2023-03-06 18:00:01.000000 powergridsim-0.0.1/powergridsim.egg-info/requires.txt
--rw-r--r--   0 jf3375     (502) staff       (20)       13 2023-03-06 18:00:01.000000 powergridsim-0.0.1/powergridsim.egg-info/top_level.txt
--rw-r--r--   0 jf3375     (502) staff       (20)       38 2023-03-06 18:00:01.827825 powergridsim-0.0.1/setup.cfg
--rw-r--r--   0 jf3375     (502) staff       (20)      753 2023-03-06 17:59:28.000000 powergridsim-0.0.1/setup.py
+drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-04-19 18:30:26.345930 powergridsim-1.0.0/
+-rw-r--r--   0 jf3375     (502) staff       (20)      304 2023-04-19 18:30:26.345764 powergridsim-1.0.0/PKG-INFO
+drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-04-19 18:30:26.341953 powergridsim-1.0.0/powergridsim/
+-rw-r--r--   0 jf3375     (502) staff       (20)      175 2023-04-19 16:40:27.000000 powergridsim-1.0.0/powergridsim/__init__.py
+drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-04-19 18:30:26.345189 powergridsim-1.0.0/powergridsim/models_gurobi/
+-rw-r--r--   0 jf3375     (502) staff       (20)      948 2023-04-11 14:55:10.000000 powergridsim-1.0.0/powergridsim/models_gurobi/__init__.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     2112 2023-04-11 18:37:45.000000 powergridsim-1.0.0/powergridsim/models_gurobi/_status_vars_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)    32848 2023-04-19 18:20:18.000000 powergridsim-1.0.0/powergridsim/models_gurobi/_utils_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)    14779 2023-04-17 18:10:36.000000 powergridsim-1.0.0/powergridsim/models_gurobi/generation_limits_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)      727 2023-04-11 14:55:10.000000 powergridsim-1.0.0/powergridsim/models_gurobi/non_dispatchable_vars_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     7686 2023-04-11 14:55:10.000000 powergridsim-1.0.0/powergridsim/models_gurobi/objective_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)    68225 2023-04-19 17:28:16.000000 powergridsim-1.0.0/powergridsim/models_gurobi/params_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)    29757 2023-04-18 19:03:17.000000 powergridsim-1.0.0/powergridsim/models_gurobi/power_balance_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     5930 2023-04-12 18:21:14.000000 powergridsim-1.0.0/powergridsim/models_gurobi/power_vars_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)    11371 2023-04-18 18:14:51.000000 powergridsim-1.0.0/powergridsim/models_gurobi/production_costs_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)    44296 2023-04-19 18:20:07.000000 powergridsim-1.0.0/powergridsim/models_gurobi/ptdf_utils_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     8107 2023-04-17 17:36:33.000000 powergridsim-1.0.0/powergridsim/models_gurobi/ramping_limits_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     4119 2023-04-18 18:27:51.000000 powergridsim-1.0.0/powergridsim/models_gurobi/reserve_requirement_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     6624 2023-04-18 20:05:12.000000 powergridsim-1.0.0/powergridsim/models_gurobi/reserve_vars_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     3487 2023-04-18 20:05:53.000000 powergridsim-1.0.0/powergridsim/models_gurobi/services_gurobi.py
+-rw-r--r--   0 jf3375     (502) staff       (20)    11355 2023-04-11 18:51:47.000000 powergridsim-1.0.0/powergridsim/models_gurobi/startup_costs_gurobi.py
+drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-04-19 18:30:26.345588 powergridsim-1.0.0/powergridsim/models_gurobi/transmission_gurobi/
+-rw-r--r--   0 jf3375     (502) staff       (20)        0 2023-04-11 14:55:10.000000 powergridsim-1.0.0/powergridsim/models_gurobi/transmission_gurobi/__init__.py
+-rw-r--r--   0 jf3375     (502) staff       (20)    18238 2023-04-12 15:33:57.000000 powergridsim-1.0.0/powergridsim/models_gurobi/transmission_gurobi/branch.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     3993 2023-04-11 14:55:10.000000 powergridsim-1.0.0/powergridsim/models_gurobi/transmission_gurobi/bus.py
+-rw-r--r--   0 jf3375     (502) staff       (20)     5118 2023-04-11 14:55:10.000000 powergridsim-1.0.0/powergridsim/models_gurobi/uptime_downtime_gurobi.py
+drwxr-xr-x   0 jf3375     (502) staff       (20)        0 2023-04-19 18:30:26.342666 powergridsim-1.0.0/powergridsim.egg-info/
+-rw-r--r--   0 jf3375     (502) staff       (20)      304 2023-04-19 18:30:26.000000 powergridsim-1.0.0/powergridsim.egg-info/PKG-INFO
+-rw-r--r--   0 jf3375     (502) staff       (20)     1245 2023-04-19 18:30:26.000000 powergridsim-1.0.0/powergridsim.egg-info/SOURCES.txt
+-rw-r--r--   0 jf3375     (502) staff       (20)        1 2023-04-19 18:30:26.000000 powergridsim-1.0.0/powergridsim.egg-info/dependency_links.txt
+-rw-r--r--   0 jf3375     (502) staff       (20)       49 2023-04-19 18:30:26.000000 powergridsim-1.0.0/powergridsim.egg-info/requires.txt
+-rw-r--r--   0 jf3375     (502) staff       (20)       13 2023-04-19 18:30:26.000000 powergridsim-1.0.0/powergridsim.egg-info/top_level.txt
+-rw-r--r--   0 jf3375     (502) staff       (20)      106 2023-04-19 17:04:21.000000 powergridsim-1.0.0/pyproject.toml
+-rw-r--r--   0 jf3375     (502) staff       (20)       38 2023-04-19 18:30:26.345970 powergridsim-1.0.0/setup.cfg
+-rw-r--r--   0 jf3375     (502) staff       (20)      617 2023-04-19 18:30:16.000000 powergridsim-1.0.0/setup.py
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/_status_vars_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/_status_vars_gurobi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from gurobipy import GRB
 
 def _is_relaxed(model):
-    if hasattr(model, 'relax_binaries') and model._relax_binaries:
+    if hasattr(model, '_relax_binaries') and model._relax_binaries:
         return True
     else:
         return False
 
 # @add_model_attr(component_name, requires = {'data_loader': None} )
 def garver_3bin_vars(model):
     '''
@@ -44,12 +44,12 @@
         model._UnitStart = model.addVars(model._ThermalGenerators, model._TimePeriods, lb = 0, ub =1, name = 'UnitStart')
     else:
         model._UnitStart = model.addVars(model._ThermalGenerators, model._TimePeriods, vtype=GRB.BINARY, name = 'UnitStart')
     return model
 
 def _add_unit_stop_vars(model, relaxed=False):
     if relaxed:
-        model._UnitStop = model.addVars(model._ThermalGenerators, model._TimePeriods, lb = 0, ub =1, name = 'UnitStoop')
+        model._UnitStop = model.addVars(model._ThermalGenerators, model._TimePeriods, lb = 0, ub =1, name = 'UnitStop')
     else:
         model._UnitStop = model.addVars(model._ThermalGenerators, model._TimePeriods, vtype=GRB.BINARY, name = 'UnitStop')
     return model
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/generation_limits_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/generation_limits_gurobi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 from gurobipy import LinExpr, quicksum
 ##LinExpr works faster than quicksum
 
 component_name = 'generation_limits'
 
+def _get_initial_maximum_power_available_upperbound_lists(m,g,t):
+    linear_vars, linear_coefs = m._get_maximum_power_available_lists(m,g,t)
+    linear_vars.append(m._UnitOn[g,t])
+    linear_coefs.append(-m._MaximumPowerOutput[g,t])
+    return linear_vars, linear_coefs
+
 ## generate new time periods by looking forward
 def _get_look_forward_periods(m,g,t,UT_end):
     expr = 0.
     p_max_gt = m._MaximumPowerOutput[g,t]
     if UT_end is not None:
         end = min(UT_end, m._NumTimePeriods-t-1)
     else:
@@ -56,15 +62,15 @@
     return linear_vars, linear_coefs
 
 
 def _CA_lower_limit(model):
     def enforce_generator_output_limits_rule_part_a(m, g, t):
         return m._MinimumPowerOutput[g, t] * m._UnitOn[g, t] <= m._PowerGenerated[g, t]
 
-    model.addConstrs((enforce_generator_output_limits_rule_part_a(model, g, t) for g in model._ThermalGenerators
+    model._EnforceGeneratorOutputLimitsPartA = model.addConstrs((enforce_generator_output_limits_rule_part_a(model, g, t) for g in model._ThermalGenerators
                      for t in model._TimePeriods), name = 'EnforceGeneratorOutputLimitsPartA')
 
 def _MLR_generation_limits_uptime_1(model, tightened=False):
     ## equations (9), (10) in ME:
     def power_limit_from_start_rule(m, g, t):
         if m._ScaledMinimumUpTime[g] > 1:
             return None
@@ -152,27 +158,27 @@
     for g in model._ThermalGenerators:
         for t in model._TimePeriods:
             cons = power_limit_from_start_stop_rule(model, g, t)
             if cons != None:
                 _power_limit_from_start_stop_cons[(g,t)] = cons
 
     if len(_power_limit_from_start_stop_cons)!= 0:
-        model._power_limit_from_start_stop = model.addConstrs((_power_limit_from_start_stop_cons[g_t] for g_t in _power_limit_from_start_stop_cons.keys()), name = '_power_limit_from_start_stop')
+        model._power_limit_from_start_stop_pan_guan_gentile = model.addConstrs((_power_limit_from_start_stop_cons[g_t] for g_t in _power_limit_from_start_stop_cons.keys()), name = '_power_limit_from_start_stop_pan_guan_gentile')
 
     model.update()
 
 def _KOW_generation_limits(model):
     ## We'll assume _MLR_generation_limits_uptime_1 and _pan_guan_generation_limits are included
     def max_power_limit_from_starts_rule(m,g,t):
         time_RU = _get_look_back_periods(m,g,t,None)
         if time_RU <= 0:
             return None
         UT = m._ScaledMinimumUpTime[g]
         ## this case is handled better above
-        if time_RU <= UT - 2 or t == m.NumTimePeriods:
+        if time_RU <= UT - 2 or t == m._NumTimePeriods:
             return None
         Start = m._UnitStart
         Pmax = m._MaximumPowerOutput[g,t]
         SU = m._ScaledStartupRampLimit
         RU = m._ScaledNominalRampUpLimit
 
         linear_vars, linear_coefs = _get_initial_maximum_power_available_upperbound_lists(m,g,t)
@@ -190,15 +196,15 @@
     for g in model._ThermalGenerators:
         for t in model._TimePeriods:
             cons = max_power_limit_from_starts_rule(model, g, t)
             if cons != None:
                 _max_power_limit_from_starts_cons[(g,t)] = cons
 
     if len(_max_power_limit_from_starts_cons)!= 0:
-        model._power_limit_from_start_stop = model.addConstrs((_max_power_limit_from_starts_cons[g_t] for g_t in _max_power_limit_from_starts_cons.keys()), name = '_max_power_limit_from_starts')
+        model._max_power_limit_from_starts = model.addConstrs((_max_power_limit_from_starts_cons[g_t] for g_t in _max_power_limit_from_starts_cons.keys()), name = '_max_power_limit_from_starts')
 
     ## NOTE: it seems this tightening should really be done on the p^l variables, when they exist
     def power_limit_from_start_stops_rule(m,g,t):
         UT = m._ScaledMinimumUpTime[g]
         SD_time_limit = _get_look_forward_periods(m,g,t,UT-1)
         if SD_time_limit <= 0: ## this is handled by the _MLR_generation_limits or _pan_guan_generation_limits
                                ## and this is needed so this number isn't negative in the computation of SU_time_limit below
@@ -237,15 +243,15 @@
     for g in model._ThermalGenerators:
         for t in model._TimePeriods:
             cons = power_limit_from_start_stops_rule(model, g, t)
             if cons != None:
                 _power_limit_from_start_stop_cons[(g,t)] = cons
 
     if len(_power_limit_from_start_stop_cons)!= 0:
-        model._power_limit_from_start_stop = model.addConstrs((_power_limit_from_start_stop_cons[g_t] for g_t in _power_limit_from_start_stop_cons.keys()), name = '_power_limit_from_start_stop')
+        model._power_limit_from_start_stop_KOW = model.addConstrs((_power_limit_from_start_stop_cons[g_t] for g_t in _power_limit_from_start_stop_cons.keys()), name = '_power_limit_from_start_stop_KOW')
 
 def pan_guan_gentile_KOW_generation_limits(model):
     model._generation_limits = 'pan_guan_gentile_KOW_generation_limits'
     if model._power_vars in ['garver_power_vars', ]:
         pass
     else:
         _CA_lower_limit(model)
@@ -268,8 +274,57 @@
 
     def reactive_lower_limit(m,g,t):
         return m._MinimumReactivePowerOutput[g,t]*m._UnitOn[g,t] <= m._ReactivePowerGenerated[g,t]
 
     model._EnforceReactiveLowerLimit = model.addConstrs(
         (reactive_lower_limit(model, g, t) for g in model._ThermalGenerators
             for t in model._TimePeriods),
-        name = 'EnforceReactiveLowerLimit')
+        name = 'EnforceReactiveLowerLimit')
+
+def MLR_generation_limits(model):
+    '''
+    Equations (9)--(11) from
+
+    G. Morales-Espana, J. M. Latorre, and A. Ramos. Tight and compact MILP
+    formulation for the thermal unit commitment problem. IEEE Transactions on
+    Power Systems, 28(4):4897–4908, 2013.
+
+    with lower limits if required
+    '''
+    model._generation_limits = 'MLR_generation_limits'
+    if model._power_vars in ['garver_power_vars',]:
+        pass
+    else:
+        _CA_lower_limit(model)
+    _MLR_generation_limits(model, False)
+    model.update()
+    return model
+
+
+def _MLR_generation_limits(model, tightened=False):
+    _MLR_generation_limits_uptime_1(model, tightened)
+
+    ## equation (11) in ME:
+    def power_limit_from_start_stop_rule(m, g, t):
+        if m._ScaledMinimumUpTime[g] <= 1:
+            return None
+        linear_vars, linear_coefs = _get_initial_maximum_power_available_upperbound_lists(
+            m, g, t)
+        linear_vars.append(m._UnitStart[g, t])
+        linear_coefs.append(
+            m._MaximumPowerOutput[g, t] - m._ScaledStartupRampLimit[g, t])
+        if t == m._NumTimePeriods:
+            return (LinExpr(linear_coefs, linear_vars) <= 0)
+        linear_vars.append(m._UnitStop[g, t + 1])
+        linear_coefs.append(
+            m._MaximumPowerOutput[g, t] - m._ScaledShutdownRampLimit[g, t])
+        return (LinExpr(linear_coefs, linear_vars) <= 0)
+
+    _power_limit_from_start_stop_cons = {}
+    for g in model._ThermalGenerators:
+        for t in model._TimePeriods:
+            cons = power_limit_from_start_stop_rule(model, g, t)
+            if cons != None:
+                _power_limit_from_start_stop_cons[(g,t)] = cons
+
+    if len(_power_limit_from_start_stop_cons)!= 0:
+        model._power_limit_from_start_stop = model.addConstrs((_power_limit_from_start_stop_cons[g_t] for g_t in _power_limit_from_start_stop_cons.keys()), name = '_power_limit_from_start_stop')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/non_dispatchable_vars_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/non_dispatchable_vars_gurobi.py`

 * *Files identical despite different names*

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/objective_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/objective_gurobi.py`

 * *Files identical despite different names*

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/params_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/params_gurobi.py`

 * *Files 2% similar despite different names*

```diff
@@ -562,19 +562,19 @@
 
         if startup_curve is None:
             return ()
 
         min_down_time = int(math.ceil(m._MinimumDownTime[g]
                                       / m._TimePeriodLengthHours))
 
-        if len(startup_curve) > min_down_time:
-            logger.warn(
-                "Truncating startup_curve longer than scaled minimum down "
-                "time {} for generator {}".format(min_down_time, g)
-            )
+        # if len(startup_curve) > min_down_time:
+        #     logger.warn(
+        #         "Truncating startup_curve longer than scaled minimum down "
+        #         "time {} for generator {}".format(min_down_time, g)
+        #     )
 
         return startup_curve[0:min_down_time]
 
     model._StartupCurve = {g: startup_curve_init_rule(model, g) for g in model._ThermalGenerators}
 
 
     def shutdown_curve_init_rule(m, g):
@@ -582,19 +582,19 @@
 
         if shutdown_curve is None:
             return ()
 
         min_down_time = int(math.ceil(m._MinimumDownTime[g]
                                       / m._TimePeriodLengthHours))
 
-        if len(shutdown_curve) > min_down_time:
-            logger.warn(
-                "Truncating shutdown_curve longer than scaled minimum down "
-                "time {} for generator {}".format(min_down_time, g)
-            )
+        # if len(shutdown_curve) > min_down_time:
+        #     logger.warn(
+        #         "Truncating shutdown_curve longer than scaled minimum down "
+        #         "time {} for generator {}".format(min_down_time, g)
+        #     )
 
         return shutdown_curve[0:min_down_time]
 
     model._ShutdownCurve = {g: shutdown_curve_init_rule(model, g) for g in model._ThermalGenerators}
 
     ####################################################################
     # generator power output at t=0 (initial condition). units are MW. #
@@ -731,15 +731,15 @@
 
         if temp > (m._MaximumPowerOutput[g, t]
                                       - m._MinimumPowerOutput[g, t]):
             return m._MaximumPowerOutput[g, t]
         else:
             return temp + m._MinimumPowerOutput[g, t]
 
-    model._ScaledShutdownRampLimit = tupledict({(g, t): scale_startup_limit(model, g, t) for g in model._ThermalGenerators for t in model._TimePeriods})
+    model._ScaledShutdownRampLimit = tupledict({(g, t): scale_shutdown_limit(model, g, t) for g in model._ThermalGenerators for t in model._TimePeriods})
 
 
     ramp_limit_validator(model)
 
     ## Some additional ramping parameters to
     ## deal with shutdowns at time=1
 
@@ -796,17 +796,17 @@
             return [i[0] for i in startup]
 
 
     def startup_lags_init_rule(m, g):
         startup_cost = thermal_gens[g].get('startup_cost')
         startup_fuel = thermal_gens[g].get('startup_fuel')
 
-        if startup_cost is not None and startup_fuel is not None:
-            logger.warning("WARNING: found startup_fuel for generator }, "
-                           "ignoring startup_cost".format(g))
+        # if startup_cost is not None and startup_fuel is not None:
+        #     logger.warning("WARNING: found startup_fuel for generator }, "
+        #                    "ignoring startup_cost".format(g))
 
         if startup_fuel is None and startup_cost is None:
             return [model.__MinimumDownTime[g]]
 
         elif startup_cost is None:
             return _get_startup_lag(startup_fuel,
                                     model.__MinimumDownTime[g])
@@ -910,15 +910,14 @@
     # for purposes of defining constraints, it is useful to have a set to index the various startup costs parameters.
     # entries are 1-based indices, because they are used as indicies into Pyomo sets - which use 1-based indexing.
     #change to 0-based indices when rewriting it directly in Gurobi
 
     def startup_cost_indices_init_rule(m, g):
         return range(0, len(m._StartupLags[g]))
 
-
     model._StartupCostIndices = {g: startup_cost_indices_init_rule(model, g) for g in model._ThermalGenerators}
 
     ## scale the startup lags
     ## Again, assert that this must be at least one in the time units of the model
     def scaled_startup_lags_rule(m, g):
         return [max(int(round(this_lag / m._TimePeriodLengthHours)), 1)
                 for this_lag in m._StartupLags[g]]
@@ -1009,17 +1008,17 @@
                 gen_name=g, t=_t
             )
 
             # if no curve_type+'_type' is specified, we assume piecewise
             # (for backwards compatibility with no 'fuel_curve_type')
             if (curve_type + '_type' in curve
                     and curve_t[curve_type + '_type'] == 'polynomial'):
-                if not _check_curve.warn_piecewise_approx:
-                    logger.warning("WARNING: Polynomial cost curves will be "
-                                   "approximated using piecewise segments")
+                # if not _check_curve.warn_piecewise_approx:
+                #     logger.warning("WARNING: Polynomial cost curves will be "
+                #                    "approximated using piecewise segments")
                     _check_curve.warn_piecewise_approx = True
 
             if curve['data_type'] != 'time_series':
                 break
 
 
     ## set "static" variable for this function
@@ -1029,21 +1028,21 @@
     def validate_cost_rule(m, g):
         gen_dict = thermal_gens[g]
         cost = gen_dict.get('p_cost')
         fuel = gen_dict.get('p_fuel')
         fuel_cost = gen_dict.get('fuel_cost')
 
         if cost is None and fuel is None:
-            logger.warning("WARNING: Generator {} has no cost information "
-                           "associated with it".format(g))
+            # logger.warning("WARNING: Generator {} has no cost information "
+            #                "associated with it".format(g))
             return True
 
-        if cost is not None and fuel is not None:
-            logger.warning("WARNING: ignoring provided p_cost and using fuel "
-                           "cost data from p_fuel for generator {}".format(g))
+        # if cost is not None and fuel is not None:
+        #     logger.warning("WARNING: ignoring provided p_cost and using fuel "
+        #                    "cost data from p_fuel for generator {}".format(g))
 
         ## look at p_cost through time
         if fuel is None:
             _check_curve(m, g, cost, 'cost_curve')
 
         else:
             if fuel_cost is None:
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/power_balance_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/power_balance_gurobi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from gurobipy import tupledict, LinExpr, GRB, quicksum
 import gurobipy as gp
 
 import egret.model_library.transmission.branch as libbranch
-import egret.data.ptdf_utils as ptdf_utils
 import egret.common.lazy_ptdf_utils as lpu
 from egret.model_library.defn import BasePointType, CoordinateType, ApproximationType
 
+import vatic.models_gurobi.ptdf_utils_gurobi as ptdf_utils
 from .power_vars_gurobi import _add_reactive_power_vars
 from .generation_limits_gurobi import _add_reactive_limits
 import vatic.models_gurobi.transmission_gurobi.bus as libbus
 import vatic.models_gurobi.transmission_gurobi.branch as libbranch
 from vatic.models_gurobi.power_vars_gurobi import _add_power_generated_startup_shutdown
 from vatic.models_gurobi.non_dispatchable_vars_gurobi import file_non_dispatchable_vars
 
@@ -140,17 +140,23 @@
     def define_pos_neg_load_generate_mismatch_rule(m, b, t):
         if b == m._ReferenceBus:
             return m._posLoadGenerateMismatch[t]-m._negLoadGenerateMismatch[t]
 
         else:
             return 0
 
-    model._LoadGenerateMismatch = {(b, t): define_pos_neg_load_generate_mismatch_rule(model, b, t)
-                                                for b in model._Buses for t in model._TimePeriods}
-
+    model._LoadGenerateMismatch_atT = {}
+    model._LoadGenerateMismatch = {}
+    for t in model._TimePeriods:
+        total = 0
+        for b in model._Buses:
+            mismatch =  define_pos_neg_load_generate_mismatch_rule(model, b, t)
+            model._LoadGenerateMismatch[(b, t)] = mismatch
+            total += mismatch
+        model._LoadGenerateMismatch_atT[t] = total
 
     # the following constraints are necessarily, at least in the case of CPLEX 12.4, to prevent
     # the appearance of load generation mismatch component values in the range of *negative* e-5.
     # what these small negative values do is to cause the optimal objective to be a very large negative,
     # due to obviously large penalty values for under or over-generation. JPW would call this a heuristic
     # at this point, but it does seem to work broadly. we tried a single global constraint, across all
     # buses, but that failed to correct the problem, and caused the solve times to explode.
@@ -182,20 +188,21 @@
             linear_vars)
         return LinExpr(linear_coefs, linear_vars)
 
     model._LoadMismatchCost = {t: compute_load_mismatch_cost_rule(t)
                                 for t in model._TimePeriods}
 
 def _add_load_mismatch(model):
-    over_gen_maxes = {}
-    over_gen_times_per_bus = {b: list() for b in model._Buses}
 
-    load_shed_maxes = {}
+    over_gen_times_per_bus = {b: list() for b in model._Buses}
     load_shed_times_per_bus = {b: list() for b in model._Buses}
 
+    model._OverGeneration = {}
+    model._LoadShedding = {}
+
     for b in model._Buses:
 
         # storage, for now, does not
         # have time-vary parameters
         storage_max_injections = 0.
         storage_max_withdraws = 0.
 
@@ -228,36 +235,24 @@
             load = model._Demand[b, t]
             if load > 0:
                 max_withdrawls += load
             elif load < 0:
                 max_injections += -load
 
             if max_injections > 0:
-                over_gen_maxes[b, t] = max_injections
+                model._OverGeneration[(b,t)] = model.addVar(lb = 0, ub = max_injections, name = 'OverGeneration[{},{}]'.format(b,t))
                 over_gen_times_per_bus[b].append(t)
             else:
-                over_gen_maxes[b, t] = GRB.INFINITY
+                model._OverGeneration[(b,t)] = model.addVar(lb = 0, ub = GRB.INFINITY, name = 'OverGeneration[{},{}]'.format(b,t))
 
             if max_withdrawls > 0:
-                load_shed_maxes[b, t] = max_withdrawls
+                model._LoadShedding[(b,t)] = model.addVar(lb = 0, ub = max_withdrawls, name = 'LoadShedding[{},{}]'.format(b,t))
                 load_shed_times_per_bus[b].append(t)
             else:
-                load_shed_maxes[b, t] = GRB.INFINITY
-
-    model._OverGenerationBusTimes = list(over_gen_maxes.keys())
-    model._LoadSheddingBusTimes = list(load_shed_maxes.keys())
-
-    model._OverGeneration = model.addVars(model._OverGenerationBusTimes,
-                                          lb = 0, ub = [over_gen_maxes[key] for key in model._OverGenerationBusTimes],
-                                          name = 'OverGeneration') # over generation
-
-    model._LoadShedding = model.addVars(model._LoadSheddingBusTimes,
-                                        lb=0, ub= [load_shed_maxes[key] for key in model._LoadSheddingBusTimes],
-                                        name='LoadShedding'
-                                        )
+                model._LoadShedding[(b,t)] = model.addVar(lb = 0, ub = GRB.INFINITY, name = 'LoadShedding[{},{}]'.format(b,t))
 
     # the following constraints are necessarily, at least in the case of CPLEX 12.4, to prevent
     # the appearance of load generation mismatch component values in the range of *negative* e-5.
     # what these small negative values do is to cause the optimal objective to be a very large negative,
     # due to obviously large penalty values for under or over-generation. JPW would call this a heuristic
     # at this point, but it does seem to work broadly. we tried a single global constraint, across all
     # buses, but that failed to correct the problem, and caused the solve times to explode.
@@ -291,75 +286,73 @@
         if const != None:
             model.addConstr(
                 const, name = 'NegLoadGenerateMismatchTolerance[{}]'.format(bus))
 
     #####################################################
     # load "shedding" can be both positive and negative #
     #####################################################
+    model._LoadGenerateMismatch_atT = {}
     model._LoadGenerateMismatch = {}
-    for b in model._Buses:
-        for t in model._TimePeriods:
-            model._LoadGenerateMismatch[b, t] = 0.
-    for b, t in model._LoadSheddingBusTimes:
-        model._LoadGenerateMismatch[b, t] += model._LoadShedding[b, t]
-    for b, t in model._OverGenerationBusTimes:
-        model._LoadGenerateMismatch[b, t] -= model._OverGeneration[b, t]
+    for t in model._TimePeriods:
+        total = 0
+        for b in model._Buses:
+            mismatch = model._LoadShedding[b,t]-model._OverGeneration[b,t]
+            model._LoadGenerateMismatch[b,t] = mismatch
+            total += mismatch
+        model._LoadGenerateMismatch_atT[t] = total
 
     model._LoadMismatchCost = {}
     for t in model._TimePeriods:
-        model._LoadMismatchCost[t] = 0.
-    for b, t in model._LoadSheddingBusTimes:
-        model._LoadMismatchCost[
-            t] += model._LoadMismatchPenalty * model._TimePeriodLengthHours * \
-                       model._LoadShedding[b, t]
-    for b, t in model._OverGenerationBusTimes:
-        model._LoadMismatchCost[
-            t] += model._LoadMismatchPenalty * model._TimePeriodLengthHours * \
+        total = 0
+        for b in model._Buses:
+            total = total + model._LoadMismatchPenalty * model._TimePeriodLengthHours * \
+                       model._LoadShedding[b, t]+ model._LoadMismatchPenalty * model._TimePeriodLengthHours * \
                        model._OverGeneration[b, t]
+        model._LoadMismatchCost[t] = total
 
 def _copperplate_network_model(block, tm, relax_balance=None):
 
     m, gens_by_bus, bus_p_loads, bus_gs_fixed_shunts = \
             _setup_egret_network_model(block, tm)
 
     ### declare the p balance
-    libbus.declare_eq_p_balance_ed(model=block,
+    libbus.declare_eq_p_balance_ed(model=block, parent_model = parent_model,
                                    index_set=m._Buses,
                                    bus_p_loads=bus_p_loads,
                                    gens_by_bus=gens_by_bus,
                                    bus_gs_fixed_shunts=bus_gs_fixed_shunts,
                                    relax_balance = relax_balance,
                                    )
 
 
 def _copperplate_relax_network_model(block,tm):
     _copperplate_network_model(block, tm, relax_balance=True)
 
 def _copperplate_approx_network_model(block,tm):
     _copperplate_network_model(block, tm, relax_balance=False)
 
-def _setup_branch_slacks(m,block,tm):
+def _setup_branch_slacks(m,block):
     # declare the branch slack variables
     # they have a sparse index set
     block._pf_slack_pos = block.addVars(m._BranchesWithSlack, lb = 0, ub = GRB.INFINITY,
                     name = 'pf_slack_pos')
 
     block._pf_slack_pos = block.addVars(m._BranchesWithSlack, lb = 0, ub = GRB.INFINITY,
                     name = 'pf_slack_neg')
 
-def _setup_interface_slacks(m,block,tm):
+def _setup_interface_slacks(m, block):
     # declare the interface slack variables
     # they have a sparse index set
     block._pfi_slack_pos = block.addVars(m._InterfacesWithSlack, lb = 0, ub = GRB.INFINITY,
                     name = 'pfi_slack_pos')
 
     block._pfi_slac_neg =  block.addVars(m._InterfacesWithSlack, lb = 0, ub = GRB.INFINITY,
                     name = 'pfi_slack_neg')
 
-def _setup_contingency_slacks(m,block,tm):
+def _setup_contingency_slacks(m, block):
     # declare the interface slack variables
     # they have a sparse index set
 
     block._pfc_slack_pos = block.addVars(m._Contingencies, m._TransmissionLines, lb=0, ub=GRB.INFINITY,
                   name='pfc_slack_pos')
 
     block._pfc_slack_neg = block.addVars(m._Contingencies, m._TransmissionLines, lb=0, ub=GRB.INFINITY,
@@ -376,77 +369,77 @@
     ## this will serve as a key into our dict of PTDF matricies,
     ## so that we can avoid recalculating them each time step
     ## with the same network topology
     branches_out_service = tuple(l for l in m._TransmissionLines if m._LineOutOfService[l,tm])
 
     return buses, branches, branches_in_service, branches_out_service, interfaces, contingencies
 
-def _setup_egret_network_model(block, tm):
-    m = block._parent
+def _setup_egret_network_model(block, tm, parent_model):
+    m = parent_model
 
     ## this is not the "real" gens by bus, but the
     ## index of net injections from the UC model
     gens_by_bus = block._gens_by_bus
 
     ### declare (and fix) the loads at the buses
     bus_p_loads = {b: m._Demand[b,tm] for b in m._Buses}
 
     block._pl = bus_p_loads
 
     bus_gs_fixed_shunts = m._bus_gs_fixed_shunts
 
     return m, gens_by_bus, bus_p_loads, bus_gs_fixed_shunts
 
-def _ptdf_dcopf_network_model(block, tm):
+def _ptdf_dcopf_network_model(block, tm, parent_model = None):
     # m is our main model, the parent of block
     m, gens_by_bus, bus_p_loads, bus_gs_fixed_shunts = \
-        _setup_egret_network_model(block, tm)
+        _setup_egret_network_model(block, tm, parent_model)
 
     buses, branches, \
     branches_in_service, branches_out_service, \
     interfaces, contingencies = _setup_egret_network_topology(m, tm)
 
     ptdf_options = m._ptdf_options
 
     block._p_nw_tm = m.addVars(m._Buses, lb = -GRB.INFINITY, ub = GRB.INFINITY, name='p_nw_{}'.format(tm))
 
     # libbus.declare_var_p_nw(block, m._Buses)
 
     ### declare net withdraw expression for use in PTDF power flows
-    libbus.declare_eq_p_net_withdraw_at_bus(model=block,
+    libbus.declare_eq_p_net_withdraw_at_bus(model=block, parent_model = parent_model,
                                             index_set=m._Buses,
                                             bus_p_loads=bus_p_loads,
                                             gens_by_bus=gens_by_bus,
                                             bus_gs_fixed_shunts=bus_gs_fixed_shunts,
                                             )
 
     ### declare the p balance
-    libbus.declare_eq_p_balance_ed(model=block,
+    libbus.declare_eq_p_balance_ed(model=block, parent_model = parent_model,
                                    index_set=m._Buses,
                                    bus_p_loads=bus_p_loads,
                                    gens_by_bus=gens_by_bus,
                                    bus_gs_fixed_shunts=bus_gs_fixed_shunts,
                                    )
 
     ### add "blank" power flow expressions
     block._branches_inservice = branches_in_service
 
-    _setup_branch_slacks(m, block, tm)
+    _setup_branch_slacks(m, block)
 
     ### interface setup
     block._interfae_keys = interfaces.keys()
 
-    _setup_interface_slacks(m, block, tm)
+    _setup_interface_slacks(m, block)
 
     ### contingency setup
     ### NOTE: important that this not be dense, we'll add elements
     ###       as we find violations
     block._contingency_set = [(c, i) for c in m._Contingencies for i in m._TransmissionLines]
     # block._pfc = Expression(block._contingency_set)
-    _setup_contingency_slacks(m, block, tm)
+    _setup_contingency_slacks(m, block)
 
     ### Get the PTDF matrix from cache, from file, or create a new one
     ### m._PTDFs set in uc_model_generator
     if branches_out_service not in m._PTDFs:
         buses_idx = tuple(buses.keys())
 
         reference_bus = m._ReferenceBus
@@ -468,35 +461,35 @@
     ### attach the current PTDF object to this block
     block._PTDF = PTDF
     rel_ptdf_tol = m._ptdf_options['rel_ptdf_tol']
     abs_ptdf_tol = m._ptdf_options['abs_ptdf_tol']
 
     if ptdf_options['lazy']:
         ### add "blank" real power flow limits
-        libbranch.declare_ineq_p_branch_thermal_bounds(model=block, period = tm,
+        libbranch.declare_ineq_p_branch_thermal_bounds(model=block, parent_model = parent_model, period = tm,
                                                        index_set=branches_in_service,
                                                        branches=branches,
                                                        p_thermal_limits=None,
                                                        approximation_type=None,
                                                        slacks=True,
                                                        slack_cost_expr=
                                                        m._BranchViolationCost[
                                                            tm]
                                                        )
         ### declare the "blank" interface flow limits
-        libbranch.declare_ineq_p_interface_bounds(model=block, period = tm,
+        libbranch.declare_ineq_p_interface_bounds(model=block, parent_model = parent_model, period = tm,
                                                   index_set=interfaces.keys(),
                                                   interfaces=interfaces,
                                                   approximation_type=None,
                                                   slacks=True,
                                                   slack_cost_expr=
                                                   m._InterfaceViolationCost[tm]
                                                   )
         ### declare the "blank" interface flow limits
-        libbranch.declare_ineq_p_contingency_branch_thermal_bounds(model=block, period = tm,
+        libbranch.declare_ineq_p_contingency_branch_thermal_bounds(model=block, parent_model = parent_model, period = tm,
                                                                    index_set=block._contingency_set,
                                                                    pc_thermal_limits=None,
                                                                    approximation_type=None,
                                                                    slacks=True,
                                                                    slack_cost_expr=
                                                                    m._ContingencyViolationCost[
                                                                        tm]
@@ -518,42 +511,42 @@
         if contingencies:
             raise RuntimeError(
                 "Contingency constraints only supported in lazy mode")
         p_max = {k: branches[k]['rating_long_term'] for k in
                  branches_in_service}
 
         ### declare the branch power flow approximation constraints
-        libbranch.declare_eq_branch_power_ptdf_approx(model=block, period = tm,
+        libbranch.declare_eq_branch_power_ptdf_approx(model=block, parent_model = parent_model, period = tm,
                                                       index_set=branches_in_service,
                                                       PTDF=PTDF,
                                                       abs_ptdf_tol=abs_ptdf_tol,
                                                       rel_ptdf_tol=rel_ptdf_tol
                                                       )
         ### declare the real power flow limits
-        libbranch.declare_ineq_p_branch_thermal_bounds(model=block, period = tm,
+        libbranch.declare_ineq_p_branch_thermal_bounds(model=block, parent_model = parent_model, period = tm,
                                                        index_set=branches_in_service,
                                                        branches=branches,
                                                        p_thermal_limits=p_max,
                                                        approximation_type=ApproximationType.PTDF,
                                                        slacks=True,
                                                        slack_cost_expr=
                                                        m._BranchViolationCost[
                                                            tm]
                                                        )
 
         ### declare the branch power flow approximation constraints
-        libbranch.declare_eq_interface_power_ptdf_approx(model=block, period = tm,
+        libbranch.declare_eq_interface_power_ptdf_approx(model=block, parent_model = parent_model, period = tm,
                                                          index_set=interfaces.keys(),
                                                          PTDF=PTDF,
                                                          abs_ptdf_tol=abs_ptdf_tol,
                                                          rel_ptdf_tol=rel_ptdf_tol
                                                          )
 
         ### declare the interface flow limits
-        libbranch.declare_ineq_p_interface_bounds(model=block, period = tm,
+        libbranch.declare_ineq_p_interface_bounds(model=block, parent_model = parent_model, period = tm,
                                                   index_set=interfaces.keys(),
                                                   interfaces=interfaces,
                                                   approximation_type=ApproximationType.PTDF,
                                                 slacks=True,
                                                   slack_cost_expr=
                                                   m._InterfaceViolationCost[tm]
                                                   )
@@ -604,20 +597,22 @@
     # for interface violation costs at a time step
     model._InterfaceViolationCost = {t: 0 for t in model._TimePeriods}
 
     # for contingency violation costs at a time step
     model._ContingencyViolationCost = {t: 0 for t in model._TimePeriods}
 
     # set up the empty model block for each time period to add constraints
+    model._TransmissionBlock = {}
     block = gp.Model()
 
     block._gens_by_bus = {bus: [bus] for bus in model._Buses}
-    block._parent = model
+    parent_model = model
     for tm in model._TimePeriods:
         block._tm = tm
         block._pg = {bus: _get_pg_expr_rule(tm, model, bus) for bus in
                      model._Buses}
         if reactive_power:
             block._qg = {bus: _get_qg_expr_rule(tm, model, bus) for bus in
                          model._Buses}
-        network_model_builder(block, tm)
+        network_model_builder(block, tm, parent_model)
+        model._TransmissionBlock[tm] = block
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/power_vars_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/power_vars_gurobi.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,26 +33,26 @@
         startup_curve = model._StartupCurve[g]
         shutdown_curve = model._ShutdownCurve[g]
         time_periods_before_startup = model._TimePeriodsBeforeStartup[g]
         time_periods_since_shutdown = model._TimePeriodsSinceShutdown[g]
 
         future_startup_past_shutdown_production = 0.
         future_startup_power_index = time_periods_before_startup + model._NumTimePeriods - t
-        if future_startup_power_index <= len(startup_curve):
+        if future_startup_power_index <= len(startup_curve)-1:
             future_startup_past_shutdown_production += startup_curve[future_startup_power_index]
 
         past_shutdown_power_index = time_periods_since_shutdown + t
-        if past_shutdown_power_index <= len(shutdown_curve):
+        if past_shutdown_power_index <= len(shutdown_curve)-1:
             future_startup_past_shutdown_production += shutdown_curve[past_shutdown_power_index]
 
         linear_vars, linear_coefs = model._get_power_generated_lists(model,g,t)
-        for startup_idx in range(1, min( len(startup_curve)+1, model._NumTimePeriods+1-t )):
+        for startup_idx in range(1, min(len(startup_curve), model._NumTimePeriods+1-t)):
             linear_vars.append(model._UnitStart[g,t+startup_idx])
             linear_coefs.append(startup_curve[startup_idx])
-        for shutdown_idx in range(1, min( len(shutdown_curve)+1, t+1 )):
+        for shutdown_idx in range(1, min(len(shutdown_curve), t+1)):
             linear_vars.append(model._UnitStop[g,t-shutdown_idx+1])
             linear_coefs.append(shutdown_curve[shutdown_idx])
         return LinExpr(linear_coefs, linear_vars) + future_startup_past_shutdown_production
 
         ## if we're here, then we can use 1-bin models
         ## and no need to do the additional work
     return LinExpr(linear_coefs, linear_vars)
@@ -83,17 +83,17 @@
                                                       name='PowerGeneratedAboveMinimum')
 
     model._get_power_generated_above_minimum_lists = lambda m, g, t: ([model._PowerGeneratedAboveMinimum[g, t]], [1.])
     model._get_negative_power_generated_above_minimum_lists = lambda m, g, t: (
     [model._PowerGeneratedAboveMinimum[g, t]], [-1.])
 
     model._get_power_generated_lists = lambda m, g, t: (
-    [model._PowerGeneratedAboveMinimum[g, t], model.UnitOn[g, t]], [1., model._MinimumPowerOutput[g, t]])
+    [model._PowerGeneratedAboveMinimum[g, t], model._UnitOn[g, t]], [1., model._MinimumPowerOutput[g, t]])
     model._get_negative_power_generated_lists = lambda m, g, t: (
-    [model._PowerGeneratedAboveMinimum[g, t], model.UnitOn[g, t]], [-1., -model._MinimumPowerOutput[g, t]])
+    [model._PowerGeneratedAboveMinimum[g, t], model._UnitOn[g, t]], [-1., -model._MinimumPowerOutput[g, t]])
 
     def power_generated_expr_rule(model, g, t):
         return model._PowerGeneratedAboveMinimum[g, t] + model._MinimumPowerOutput[g, t] * model._UnitOn[g, t]
 
     model._PowerGenerated = tupledict({(g, t): power_generated_expr_rule(model, g, t) for g in model._ThermalGenerators
                              for t in model._TimePeriods})
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/production_costs_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/production_costs_gurobi.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,45 +102,39 @@
         name = 'ProductionCost')
 
     def piecewise_production_costs_rule(m, g, t):
         if (g, t) in m._PiecewiseGeneratorTimeIndexSet:
             points = m._PowerGenerationPiecewisePoints[g, t]
             costs = m._PowerGenerationPiecewiseCostValues[g, t]
             time_scale = m._TimePeriodLengthHours
-            linear_coefs = [
-                (time_scale * costs[i + 1] - time_scale * costs[i]) / (
-                            points[i + 1] - points[i]) \
-                for i in range(len(points) - 1)]
-            linear_vars = [m._PiecewiseProduction[g, t, i] for i in
-                           range(len(points) - 1)]
-            linear_coefs.append(-1.)
-            linear_vars.append(m._ProductionCost[g, t])
-            return LinExpr(linear_coefs, linear_vars) == 0
+            linear_coefs = [None]*(len(points)-1)
+            linear_vars = [None]*(len(points)-1)
+            for i in range(len(points)-1):
+                linear_coefs[i] =  (time_scale * costs[i + 1] - time_scale * costs[i]) / (points[i + 1] - points[i])
+                linear_vars[i] = m._PiecewiseProduction[g, t, i]
+            return LinExpr(linear_coefs, linear_vars)-m._ProductionCost[g,t]== 0
         elif (g, t) in m._LinearGeneratorTimeIndexSet:
             i = 0
             points = m._PowerGenerationPiecewisePoints[g, t]
             costs = m._PowerGenerationPiecewiseCostValues[g, t]
             time_scale = m._TimePeriodLengthHours
             slope = (time_scale * costs[i + 1] - time_scale * costs[i]) / (
                         points[i + 1] - points[i])
             linear_vars, linear_coefs = m._get_power_generated_above_minimum_lists(
                 m, g, t)
             linear_coefs = [slope * coef for coef in linear_coefs]
-            linear_vars.append(m._ProductionCost[g, t])
-            linear_coefs.append(-1.)
-            return LinExpr(linear_coefs, linear_vars) == 0
+            return LinExpr(linear_coefs, linear_vars)-m._ProductionCost[g, t] == 0
         else:
-            return m.ProductionCost[g, t] == 0.
-
-    model._ProductionCostConstr = \
-        model.addConstrs((piecewise_production_costs_rule(model, g, t)
-                            for g in model._SingleFuelGenerators
-                            for t in model._TimePeriods),
-                          name = 'ProductionCostConstr')
+            return (m._ProductionCost[g, t] == 0)
 
+    model._ProductionCostConstr = {}
+    for g in model._SingleFuelGenerators:
+        for t in model._TimePeriods:
+            piecewise_production_costs_rule(model, g, t)
+            model._ProductionCostConstr[(g,t)] = model.addConstr(piecewise_production_costs_rule(model, g, t), name = 'ProductionCostConstr[{},{}]'.format(g,t))
     _compute_total_production_cost(model)
 
 def KOW_production_costs_tightened(model):
 
     '''
     this is the (more ideal) production cost model introducted by:
 
@@ -235,7 +229,23 @@
     model._PiecewiseProductionLimits2 = \
         model.addConstrs((piecewise_production_limits_rule2_cons[g_t_i]
                             for g_t_i in piecewise_production_limits_rule2_cons.keys()),
                          name = 'piecewise_production_limits_rule2')
 
     _basic_production_costs_constr(model)
 
+
+def CA_production_costs(model):
+    '''
+    This is a production cost model with additional variables for each
+    piecewise linear segment, equations (7)--(11) in
+
+    M. Carrion and J. M. Arroyo. A computationally efficient mixed-integer
+    linear formulation for the thermal unit commitment problem. IEEE
+    Transactions on Power Systems, 21(3):1371–1378, Aug 2006. ISSN 0885-8950.
+    doi: 10.1109/TPWRS.2006.876672.
+    '''
+
+    _basic_production_costs_vars(model)
+    _basic_production_costs_constr(model)
+    model.update()
+    return model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/ramping_limits_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/ramping_limits_gurobi.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                 -m._ScaledStartupRampLimit[g, t] + 0 +
                 m._ScaledNominalRampUpLimit[g, t]]
 
             linear_vars = [*linear_vars_power_t, *rhs_linear_vars]
             linear_coefs = [*linear_coefs_power_t, *rhs_neg_linear_coefs]
 
             RHS = m._PowerGeneratedT0[g]
-            return LinExpr(linear_coefs, linear_vars <= RHS)
+            return LinExpr(linear_coefs, linear_vars) <= RHS
 
         else:
             linear_vars_power_t, linear_coefs_power_t = m._get_maximum_power_available_above_minimum_lists(
                 m, g, t)
             linear_vars_power_t_1, linear_coefs_power_t_1 = m._get_negative_power_generated_above_minimum_lists(
                 m, g, t - 1)
 
@@ -99,15 +99,15 @@
             ]
 
             linear_vars = [*linear_vars_power_t, *linear_vars_power_t_1,
                            *rhs_linear_vars]
             linear_coefs = [*linear_coefs_power_t, *linear_coefs_power_t_1,
                             *rhs_neg_linear_coefs]
 
-            return LinExpr(linear_coefs, linear_vars <= 0)
+            return LinExpr(linear_coefs, linear_vars) <= 0
 
     enforce_max_available_ramp_up_rates_cons = {}
     for g in model._ThermalGenerators:
         for t in model._TimePeriods:
             cons = enforce_max_available_ramp_up_rates_rule(model, g, t)
             if cons != None:
                 enforce_max_available_ramp_up_rates_cons[g, t] = cons
@@ -134,15 +134,15 @@
             linear_vars = [*linear_vars_power_t, *lhs_linear_vars]
             linear_coefs = [*linear_coefs_power_t, *lhs_neg_linear_coefs]
 
             LHS = m._PowerGeneratedT0[g] - (m._ScaledNominalRampDownLimit[g, t] +
                                            m._MinimumPowerOutput[g, t] - 0) * \
                   m._UnitOnT0[g]
 
-            return LinExpr(linear_coefs, linear_vars >= LHS)
+            return LinExpr(linear_coefs, linear_vars) >= LHS
         else:
             linear_vars_power_t, linear_coefs_power_t = m._get_power_generated_above_minimum_lists(
                 m, g, t)
             linear_vars_power_t_1, linear_coefs_power_t_1 = m._get_negative_power_generated_above_minimum_lists(
                 m, g, t - 1)
 
             lhs_linear_vars = [m._UnitOn[g, t - 1], m._UnitStop[g, t]]
@@ -153,15 +153,15 @@
                     g, t] - m._ScaledNominalRampDownLimit[g, t]
             ]
             linear_vars = [*linear_vars_power_t, *linear_vars_power_t_1,
                            *lhs_linear_vars]
             linear_coefs = [*linear_coefs_power_t, *linear_coefs_power_t_1,
                             *lhs_neg_linear_coefs]
 
-            return LinExpr(linear_coefs, linear_vars >= 0)
+            return LinExpr(linear_coefs, linear_vars) >= 0
 
 
     enforce_ramp_down_limits_cons = {}
     for g in model._ThermalGenerators:
         for t in model._TimePeriods:
             cons = enforce_ramp_down_limits_rule(model, g, t)
             if cons != None:
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/reserve_requirement_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/reserve_requirement_gurobi.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,14 +12,26 @@
     else:
         # the reserve shortfall can't be more than the reserve requirement in any given time period.
         model._ReserveShortfall = model.addVars(
                 model._TimePeriods, lb = 0,
                 ub = [model._ReserveRequirement[t] for t in model._TimePeriods],
                 name = 'ReserveShortfall')
 
+
+def _MLR_reserve_constraint(model):
+    def enforce_reserve_requirements_rule(m, t):
+        linear_vars = list(
+            m._ReserveProvided[g, t] for g in m._ThermalGenerators)
+        linear_vars.append(m._ReserveShortfall[t])
+        linear_coefs = [1.] * len(linear_vars)
+        return (LinExpr(linear_coefs, linear_vars) >= m._ReserveRequirement[t])
+
+    model._EnforceReserveRequirements = model.addConstrs((enforce_reserve_requirements_rule(model, t) for t in model._TimePeriods),
+                                                         name = 'EnforceReserveRequirements')
+
 def CA_reserve_constraints(model):
     '''
     This is the reserve requirement with slacks given by equation (3) in
 
     Carrion, M. and Arroyo, J. (2006) A Computationally Efficient Mixed-Integer
     Liner Formulation for the Thermal Unit Commitment Problem. IEEE Transactions
     on Power Systems, Vol. 21, No. 3, Aug 2006.
@@ -34,19 +46,23 @@
     # demand and the spinning reserve requirements in each time period.
     # encodes Constraint 3 in Carrion and Arroyo.
 
     # IMPT: In contrast to power balance, reserves are (1) not per-bus and (2) expressed in terms of
     #       maximum power available, and not actual power generated.
 
     def enforce_reserve_requirements_rule(m, t):
-        m._LoadGenerateMismatch = tupledict(m._LoadGenerateMismatch)
-        linear_expr = (quicksum(m._MaximumPowerAvailable.select('*', t))
+        # linear_expr = (quicksum(m._MaximumPowerAvailable.select('*', t))
+        #             + quicksum(m._NondispatchablePowerUsed.select('*', t))
+        #             +  quicksum(m._LoadGenerateMismatch.select('*', t))
+        #             + m._ReserveShortfall[t])
+
+        linear_expr = (m._MaximumPowerAvailable_atT[t]
                     + quicksum(m._NondispatchablePowerUsed.select('*', t))
-                    +  quicksum(m._LoadGenerateMismatch.select('*', t))
-                    + quicksum(m._ReserveShortfall.select(t)))
+                    +  m._LoadGenerateMismatch_atT[t]
+                    + m._ReserveShortfall[t])
 
         if hasattr(model, '_PowerOutputStorage'):
             linear_expr += quicksum(m._PowerOutputStorage.select('*', t))
 
         if hasattr(model, '_PowerInputStorage'):
             linear_expr -= quicksum(m._PowerInputStorage.select('*', t))
 
@@ -54,8 +70,34 @@
 
     model._EnforceReserveRequirements = model.addConstrs(
             (enforce_reserve_requirements_rule(model, t) for t in model._TimePeriods),
             name = 'EnforceReserveRequirements')
 
 
     model.update()
+    return model
+
+
+def MLR_reserve_constraints(model):
+    '''
+    This is the reserve requirement with slacks given by equation (5) in
+
+    G. Morales-Espana, J. M. Latorre, and A. Ramos. Tight and compact MILP
+    formulation for the thermal unit commitment problem. IEEE Transactions on
+    Power Systems, 28(4):4897–4908, 2013.
+    '''
+
+    if not check_reserve_requirement(model):
+        _add_reserve_shortfall(model, fixed=True)
+        return
+
+    _add_reserve_shortfall(model)
+    # ensure there is sufficient maximal power output available to meet both the
+    # demand and the spinning reserve requirements in each time period.
+    # encodes Constraint 3 in Carrion and Arroyo.
+
+    # IMPT: In contrast to power balance, reserves are (1) not per-bus and (2) expressed in terms of
+    #       maximum power available, and not actual power generated.
+    _MLR_reserve_constraint(model)
+
+    model.update()
     return model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/services_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/services_gurobi.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     Defines ancillary services: regulation, spinning reserve, nonspinning reserve, operational reserve, flexible ramp
     ## NOTE: As in most markets, the value of ancillary services from high to low is regulation, spinning reserve, nonspinning reserve, and supplemental reserve.
     ##       We allow for a higher-quality ancillary service to be subtituted for a lower-quality one
     ##       Flexible ramp is treated differently, again as it is in most markets. There is no bid for flexible ramp, and it is priced at opportunity cost
     '''
     md = model._model_data
 
-    system = md.data['system']
-    elements = md.data['elements']
+    system = md._data['system']
+    elements = md._data['elements']
 
     ## list of possible ancillary services coming
     ## from model_data
     ancillary_service_list = ['spinning_reserve_requirement',
                               'non_spinning_reserve_requirement',
                               'regulation_up_requirement',
                               'regulation_down_requirement',
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/startup_costs_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/startup_costs_gurobi.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,123 @@
 from gurobipy import tupledict, LinExpr, quicksum, GRB
 
 from ._status_vars_gurobi import _is_relaxed
 
 component_name = 'startup_costs'
 
 
+def MLR_startup_costs(model, add_startup_cost_var=True):
+    '''
+    Start-up cost formulation in equations (2)--(3) from
+
+    G. Morales-Espana, J. M. Latorre, and A. Ramos. Tight and compact MILP
+    formulation for the thermal unit commitment problem. IEEE Transactions on
+    Power Systems, 28(4):4897–4908, 2013.
+    '''
+
+    # begin latorre startup costs
+
+    ############################################################
+    # compute the per-generator, per-time period startup costs #
+    ############################################################
+    ## BK -- replace with delta's
+    def startup_costs_index_set_generator(m):
+        return ((g, s, t) for t in m._TimePeriods for g in m._ThermalGenerators
+                for s in m._StartupCostIndices[g])
+
+    model._StartupCostsIndexSet = [(g, s, t) for g in model._ThermalGenerators
+                for s in model._StartupCostIndices[g] for t in model._TimePeriods]
+
+    if _is_relaxed(model):
+        model._delta = model.addVars(model._StartupCostsIndexSet, lb = 0, ub = 1, name = 'delta')
+    else:
+        model._delta = model.addVars(model._StartupCostsIndexSet, vtype=GRB.BINARY, name = 'delta')
+    model.update()
+
+    def delta_eq_rule(m, g, t):
+        linear_vars = [m._delta[g, s, t] for s in m._StartupCostIndices[g]]
+        linear_coefs = [1.] * len(linear_vars)
+        linear_vars.append(m._UnitStart[g, t])
+        linear_coefs.append(-1.)
+        return (LinExpr(linear_coefs, linear_vars) == 0)
+
+    model._delta_eq = model.addConstrs((delta_eq_rule(model, g, t) for g in
+                                       model._ThermalGenerators for t in model._TimePeriods),
+                                       name = 'delta_eq')
+
+    ## BK -- updated to reflect previous generator condition
+    ## BK -- assumes initial time is 1
+    def delta_ineq_rule(m, g, s, t):
+        assert (m._InitialTime == 1)
+        ## the last startup indicator doesn't have a lag
+        if s == len(m._StartupCostIndices[g])-1:
+            return None
+        this_lag = m._ScaledStartupLags[g][s]
+        next_lag = m._ScaledStartupLags[g][s+1]
+        ## this is negative if the generator has previously been off
+        generator_t0_state = int(round(m._UnitOnT0State[g] / m._TimePeriodLengthHours))
+
+        ## equation (15) in ME
+        if next_lag + generator_t0_state < t < next_lag:
+            m._delta[(g, s, t)].lb = 0
+            m._delta[(g, s, t)].ub = 0
+            return None
+
+        if m._status_vars == 'garver_2bin_vars':
+            linear_vars = [m._UnitStart[g, t - i] for i in
+                           range(this_lag, next_lag)]
+            linear_coefs = [-1.] * len(linear_vars)
+            linear_vars += [m._delta[g, s, t], m._UnitOn[g, t - this_lag]]
+            linear_coefs += [1., 1.]
+            if t == next_lag:
+                return (LinExpr(linear_coefs, linear_vars) <= m._UnitOnT0[g])
+                # return m.delta[g,s,t] <= m.UnitOnT0[g] - m.UnitOn[g,t-this_lag] + sum(m.UnitStart[g,t-i] for i in range(this_lag, next_lag))
+            elif t > next_lag:
+                linear_vars.append(m._UnitOn[g, t - next_lag])
+                linear_coefs.apppend(-1.)
+                return (LinExpr(linear_coefs, linear_vars) <= 0)
+                # return m.delta[g,s,t] <= m.UnitOn[g,t-next_lag] - m.UnitOn[g,t-this_lag] + sum(m.UnitStart[g,t-i] for i in range(this_lag, next_lag))
+        else:
+            ## equation (2) in ME
+            if t >= next_lag:
+                linear_vars = [m._UnitStop[g, t - i] for i in
+                               range(this_lag, next_lag)]
+                linear_coefs = [-1.] * len(linear_vars)
+                linear_vars.append(m._delta[g, s, t])
+                linear_coefs.append(1.)
+                return (LinExpr(linear_coefs, linear_vars) <= 0)
+
+        return None
+
+    delta_ineq_constrs = {}
+    for set in model._StartupCostsIndexSet:
+        constr = delta_ineq_rule(model, set[0], set[1], set[2])
+        if constr != None:
+            delta_ineq_constrs[set] = constr
+
+    model._delta_ineq = model.addConstrs((delta_ineq_constrs[g_s_t] for g_s_t in delta_ineq_constrs.keys()),
+                                         name = 'delta_ineq')
+
+    if add_startup_cost_var:
+        model._StartupCost = model.addVars(model._SingleFuelGenerators, model._TimePeriods, name = 'StartupCost')
+
+    def ComputeStartupCost2_rule(m, g, t):
+        linear_vars = [m._delta[g, s, t] for s in m._StartupCostIndices[g]]
+        linear_coefs = [m._StartupCosts[g][s] for s in m._StartupCostIndices[g]]
+        linear_vars.append(m._StartupCost[g, t])
+        linear_coefs.append(-1.)
+        return (LinExpr(linear_coefs, linear_vars) == 0)
+
+    model._ComputeStartupCosts = model.addConstrs((ComputeStartupCost2_rule(model, g, t)
+                                                    for g in model._SingleFuelGenerators for t in model._TimePeriods), name = 'ComputeStartupCosts')
+    model.update()
+    return model
+
+
+
 def KOW_startup_costs(model, add_startup_cost_var=True):
     '''
     Start-up cost formulation "Match" from
 
     Ben Knueven, Jim Ostrowski, and Jean-Paul Watson. A novel matching
     formulation for startup costs in unit commitment, 2017.
     URL http://www.optimization-online.org/DB_FILE/2017/03/5897.pdf.
@@ -142,10 +251,10 @@
                     break
 
         return LinExpr(linear_coefs, linear_vars) == 0
 
     model._ComputeStartupCosts = model.addConstrs(
         (ComputeStartupCost2_rule(model, g, t)
             for g in model._SingleFuelGenerators for t in model._TimePeriods)
-                                           ,name='ComputeStartupCost2_rule')
+                                           ,name='ComputeStartupCosts')
     model.update()
     return model
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/transmission_gurobi/branch.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/transmission_gurobi/branch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from gurobipy import LinExpr, quicksum
+from gurobipy import LinExpr, tupledict
 
 from egret.model_library.defn import FlowType, CoordinateType, ApproximationType, RelaxationType
 
 def get_power_flow_interface_expr_ptdf(model, interface_name, PTDF, rel_ptdf_tol=None, abs_ptdf_tol=None):
     """
     Create a pyomo power flow expression from PTDF matrix for an interface
     """
@@ -88,36 +88,35 @@
         expr = pf
         if neg_slack is not None:
             expr += neg_slack
         if pos_slack is not None:
             expr -= pos_slack
     return (llimit, expr, ulimit)
 
-def declare_ineq_p_branch_thermal_bounds(model, period, index_set,
+def declare_ineq_p_branch_thermal_bounds(model, parent_model, period, index_set,
                                         branches, p_thermal_limits,
                                         approximation_type=ApproximationType.BTHETA,
                                         slacks=False, slack_cost_expr=None):
     """
     Create an inequality constraint for the branch thermal limits
     based on the power variables or expressions.
     """
-    m = model._parent
+    m = parent_model
     # con_set = decl.declare_set('_con_ineq_p_branch_thermal_bounds',
     #                            model=model, index_set=index_set)
     # flag for if slacks are on the model
     # if slacks:
     #     if not hasattr(model, 'pf_slack_pos'):
     #         raise Exception('No positive slack branch variables on model, but slacks=True')
     #     if not hasattr(model, 'pf_slack_neg'):
     #         raise Exception('No negative slack branch variables on model, but slacks=True')
     #     if slack_cost_expr is None:
     #         raise Exception('No cost expression for slacks, but slacks=True')
-
-    # m._ineq_pf_branch_thermal_bounds = pe.Constraint(con_set)
-
+    m._ineq_pf_branch_thermal_ub = tupledict()
+    m._ineq_pf_branch_thermal_lb = tupledict()
     if approximation_type == ApproximationType.BTHETA or \
             approximation_type == ApproximationType.PTDF:
         for branch_name in index_set:
             limit = p_thermal_limits[branch_name]
             if limit is None:
                 continue
 
@@ -131,44 +130,46 @@
                 assert len(model._pf_slack_pos) == len(model._pf_slack_neg)
             else:
                 neg_slack = None
                 pos_slack = None
 
             lb, expr, ub = generate_thermal_bounds(model.pf[branch_name], -limit, limit,
                                     neg_slack, pos_slack)
-            m.addConstr(
+            m._ineq_pf_branch_thermal_ub[(branch_name, period)] = m.addConstr(
                     (expr <= ub),
                     name = 'ineq_pf_branch_thermal_upper_bounds_branch[{}]_period[{}]'.format(branch_name, period))
-            m.addConstr(
+            m._ineq_pf_branch_thermal_lb[(branch_name, period)] = m.addConstr(
                     (-expr <= -lb),
                     name = 'ineq_pf_branch_thermal_lower_bounds_branch[{}]_period[{}]'.format(branch_name, period))
 
-def declare_ineq_p_interface_bounds(model, period, index_set, interfaces,
+def declare_ineq_p_interface_bounds(model, parent_model, period, index_set, interfaces,
                                         approximation_type=ApproximationType.BTHETA,
                                         slacks=False, slack_cost_expr=None):
     """
     Create the inequality constraints for the interface limits
     based on the power variables or expressions.
 
     p_interface_limits should be (lower, upper) tuple
     """
-    m = model._parent
+    m = parent_model
     # con_set = decl.declare_set('_con_ineq_p_interface_bounds',
     #                            model=model, index_set=index_set)
     #
     # m._ineq_pf_interface_bounds = pe.Constraint(con_set)
     #
     # # flag for if slacks are on the model
     # if slacks:
     #     if not hasattr(model, 'pfi_slack_pos'):
     #         raise Exception('No positive slack interface variables on model, but slacks=True')
     #     if not hasattr(model, 'pfi_slack_neg'):
     #         raise Exception('No negative slack interface variables on model, but slacks=True')
     #     if slack_cost_expr is None:
     #         raise Exception('No cost expression for slacks, but slacks=True')
+    m._ineq_p_interface_ub = tupledict()
+    m._ineq_p_interface_lb = tupledict()
 
     if approximation_type == ApproximationType.BTHETA or \
             approximation_type == ApproximationType.PTDF:
         for interface_name in index_set:
             interface = interfaces[interface_name]
             if interface['minimum_limit'] is None and \
                     interface['maximum_limit'] is None:
@@ -184,30 +185,30 @@
                 assert len(model._pfi_slack_pos) == len(model._pfi_slack_neg)
             else:
                 neg_slack = None
                 pos_slack = None
 
             lb, expr, ub =  generate_thermal_bounds(model._pfi[interface_name], interface['minimum_limit'], interface['maximum_limit'],
                                         neg_slack, pos_slack)
-            m.addConstr(
+            m._ineq_p_interface_ub[(interface_name, period)] = m.addConstr(
                     (expr <= ub),
                     name = 'ineq_pf_interface_upper_bounds_interface[{}]_peiord[{}]'.format(interface_name, period))
-            m.addConstr(
+            m._ineq_p_interface_lb[(interface_name, period)] = m.addConstr(
                     (-expr <= -lb),
                     name = 'ineq_pf_interface_lower_bounds_interface[{}]_period[{}]'.format(interface_name, period))
 
-def declare_ineq_p_contingency_branch_thermal_bounds(model, period, index_set,
+def declare_ineq_p_contingency_branch_thermal_bounds(model, parent_model, period, index_set,
                                                      pc_thermal_limits,
                                                      approximation_type=ApproximationType.PTDF,
                                                      slacks=False, slack_cost_expr=None):
     """
     Create an inequality constraint for the branch thermal limits
     based on the power variables or expressions.
     """
-    m = model._parent
+    m = parent_model
     # # flag for if slacks are on the model
     # if slacks:
     #     if not hasattr(model, 'pfc_slack_pos'):
     #         raise Exception('No positive slack branch variables on model, but slacks=True')
     #     if not hasattr(model, 'pfc_slack_neg'):
     #         raise Exception('No negative slack branch variables on model, but slacks=True')
     #     if slack_cost_expr is None:
@@ -240,21 +241,21 @@
                     (expr <= ub),
                     name = 'ineq_pf_interface_upper_bounds_branch[{}]_peiord[{}]'.format(branch_name, period))
             m.addConstr(
                     (-expr <= -lb),
                     name = 'ineq_pf_interface_lower_bounds_branch[{}]_period[{}]'.format(branch_name, period))
 
 
-def declare_eq_branch_power_ptdf_approx(model, period, index_set, PTDF, rel_ptdf_tol=None, abs_ptdf_tol=None):
+def declare_eq_branch_power_ptdf_approx(model, parent_model, period, index_set, PTDF, rel_ptdf_tol=None, abs_ptdf_tol=None):
     """
     Create the equality constraints or expressions for power (from PTDF
     approximation) in the branch
     """
 
-    m = model._parent
+    m = parent_model
 
     # con_set = decl.declare_set("_con_eq_branch_power_ptdf_approx_set", model, index_set)
 
 
     # if pf_is_var:
     #     m._eq_pf_branch = pe.Constraint(con_set)
     # else:
@@ -263,73 +264,21 @@
 
     for branch_name in index_set:
         expr = \
             get_power_flow_expr_ptdf_approx(m, branch_name, PTDF, rel_ptdf_tol=rel_ptdf_tol, abs_ptdf_tol=abs_ptdf_tol)
 
         m.addConstr((model._pf[branch_name] == expr), name = '_eq_pf_branch[{}]_period[{}]'.format(branch_name, period))
 
-
-
-def declare_ineq_p_branch_thermal_bounds(model, period, index_set,
-                                        branches, p_thermal_limits,
-                                        approximation_type=ApproximationType.BTHETA,
-                                        slacks=False, slack_cost_expr=None):
-    """
-    Create an inequality constraint for the branch thermal limits
-    based on the power variables or expressions.
-    """
-    m = model._parent
-    # con_set = decl.declare_set('_con_ineq_p_branch_thermal_bounds',
-    #                            model=model, index_set=index_set)
-    # # flag for if slacks are on the model
-    # if slacks:
-    #     if not hasattr(model, 'pf_slack_pos'):
-    #         raise Exception('No positive slack branch variables on model, but slacks=True')
-    #     if not hasattr(model, 'pf_slack_neg'):
-    #         raise Exception('No negative slack branch variables on model, but slacks=True')
-    #     if slack_cost_expr is None:
-    #         raise Exception('No cost expression for slacks, but slacks=True')
-
-    # m._ineq_pf_branch_thermal_bounds = pe.Constraint(con_set)
-
-    if approximation_type == ApproximationType.BTHETA or \
-            approximation_type == ApproximationType.PTDF:
-        for branch_name in index_set:
-            limit = p_thermal_limits[branch_name]
-            if limit is None:
-                continue
-
-            if slacks and branch_name in model._pf_slack_neg.index_set():
-                assert branch_name in model._pf_slack_pos.index_set()
-                neg_slack = model._pf_slack_neg[branch_name]
-                pos_slack = model._pf_slack_pos[branch_name]
-                uc_model = slack_cost_expr.parent_block()
-                slack_cost_expr.expr += (uc_model._TimePeriodLengthHours*uc_model._BranchLimitPenalty[branch_name] *
-                                    (neg_slack + pos_slack) )
-                assert len(model._pf_slack_pos) == len(model._pf_slack_neg)
-            else:
-                neg_slack = None
-                pos_slack = None
-
-            lb, expr, ub = generate_thermal_bounds(model._pf[branch_name], -limit, limit, neg_slack, pos_slack)
-            model.addConstrs(
-                (expr >= ub), name = 'ineq_pf_branch_thermal_upper-bounds_branch[{}]_period[{}]'.format(branch_name, period)
-            )
-            model.addConstrs(
-                (-expr >= -lb), name = 'ineq_pf_branch_thermal_lower_bounds_branch[{}]_period[{}]'.format(branch_name, period)
-            )
-
-
-def declare_eq_interface_power_ptdf_approx(model, period, index_set, PTDF, rel_ptdf_tol=None, abs_ptdf_tol=None):
+def declare_eq_interface_power_ptdf_approx(model, parent_model, period, index_set, PTDF, rel_ptdf_tol=None, abs_ptdf_tol=None):
     """
     Create equality constraints or expressions for power (from PTDF
     approximation) across the interface
     """
 
-    m = model._parent
+    m = parent_model
     # con_set = decl.declare_set("_con_eq_interface_power_ptdf_approx_set", model, index_set)
     #
     # pfi_is_var = isinstance(m._pfi, pe.Var)
     #
     # if pfi_is_var:
     #     m._eq_pf_interface = pe.Constraint(con_set)
     # else:
@@ -345,22 +294,22 @@
         #     m._eq_pf_interface[interface_name] = \
         #             m._pfi[interface_name] == expr
         # else:
     m.addConstr((expr), name = 'pfi_interface_[{}]_period[{}]'.format(interface_name, period))
 
 
 
-def declare_ineq_s_branch_thermal_limit(model, period, index_set,
+def declare_ineq_s_branch_thermal_limit(model, parent_model, period, index_set,
                                         branches, s_thermal_limits,
                                         flow_type=FlowType.POWER):
     """
     Create the inequality constraints for the branch thermal limits
     based on the power variables.
     """
-    m = model._parent
+    m = parent_model
     # con_set = decl.declare_set('_con_ineq_s_branch_thermal_limit',
     #                            model=model, index_set=index_set)
     #
     # m._ineq_sf_branch_thermal_limit = pe.Constraint(con_set)
     # m._ineq_st_branch_thermal_limit = pe.Constraint(con_set)
 
     if flow_type == FlowType.CURRENT:
@@ -391,24 +340,24 @@
                 name = '_ineq_sf_branch_thermal_limit_branch[{}]_period[{}]'.format(branch_name, period))
             m.addConstr(
                 (model._pt[branch_name] ** 2 + model._qt[branch_name] ** 2 \
                 <= s_thermal_limits[branch_name] ** 2),
                 name='_ineq_st_branch_thermal_limit_branch[{}]_period[{}]'.format(branch_name, period)
             )
 
-def declare_ineq_p_interface_bounds(model, period, index_set, interfaces,
+def declare_ineq_p_interface_bounds(model, parent_model, period, index_set, interfaces,
                                         approximation_type=ApproximationType.BTHETA,
                                         slacks=False, slack_cost_expr=None):
     """
     Create the inequality constraints for the interface limits
     based on the power variables or expressions.
 
     p_interface_limits should be (lower, upper) tuple
     """
-    m = model._parent
+    m = parent_model
     # con_set = decl.declare_set('_con_ineq_p_interface_bounds',
     #                            model=model, index_set=index_set)
     #
     # m._ineq_pf_interface_bounds = pe.Constraint(con_set)
     #
     # # flag for if slacks are on the model
     # if slacks:
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/transmission_gurobi/bus.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/transmission_gurobi/bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,20 +26,20 @@
     relaxed_balance = False
 
     if relaxed_balance:
         m.addConstr((p_expr >= 0.0), name = 'eq_p_balance_at_period_[{}]'.format(model._tm))
     else:
         m.addConstr((p_expr == 0.0), name = 'eq_p_balance_at_period_[{}]'.formar(model._tm))
 
-def declare_eq_p_net_withdraw_at_bus(model, index_set, bus_p_loads, gens_by_bus, bus_gs_fixed_shunts,
+def declare_eq_p_net_withdraw_at_bus(model, parent_model, index_set, bus_p_loads, gens_by_bus, bus_gs_fixed_shunts,
                                      dc_inlet_branches_by_bus=None, dc_outlet_branches_by_bus=None):
     """
     Create a named pyomo expression for bus net withdraw
     """
-    m = model._parent
+    m = parent_model
     dc_inlet_branches_by_bus, dc_outlet_branches_by_bus = _get_dc_dicts(dc_inlet_branches_by_bus,
                                                                         dc_outlet_branches_by_bus,
                                                                         index_set)
 
     for b in index_set:
         rhs = ( bus_gs_fixed_shunts[b]+ (model._pl[b] if bus_p_loads[b] != 0.0 else 0.0 )
                                             - quicksum(model._pg[g] for g in gens_by_bus[b] )
@@ -47,22 +47,22 @@
                                                    in dc_outlet_branches_by_bus[b])
                                             - quicksum(model._dcpf[branch_name] for branch_name
                                                    in dc_inlet_branches_by_bus[b])
                                             )
 
         m.addConstr((model._p_nw_tm[b] == rhs) , name =  '_eq_p_net_withdraw_at_bus[{}]_at_period[{}]'.format(b, model._tm))
 
-def declare_eq_p_balance_ed(model, index_set, bus_p_loads, gens_by_bus, bus_gs_fixed_shunts, **rhs_kwargs):
+def declare_eq_p_balance_ed(model, parent_model, index_set, bus_p_loads, gens_by_bus, bus_gs_fixed_shunts, **rhs_kwargs):
     """
     Create the equality constraints for the real power balance
     at a bus using the variables for real power flows, respectively.
 
     NOTE: Equation build orientates constants to the RHS in order to compute the correct dual variable sign
     """
-    m = model._parent
+    m = parent_model
     p_expr = quicksum(model._pg[gen_name] for bus_name in index_set for gen_name in gens_by_bus[bus_name])
     p_expr -= quicksum(model._pl[bus_name] for bus_name in index_set if bus_p_loads[bus_name] is not None)
     p_expr -= quicksum(bus_gs_fixed_shunts[bus_name] for bus_name in index_set if bus_gs_fixed_shunts[bus_name] != 0.0)
 
     relaxed_balance = False
 
     if relaxed_balance:
```

### Comparing `powergridsim-0.0.1/powergridsim/models_gurobi/uptime_downtime_gurobi.py` & `powergridsim-1.0.0/powergridsim/models_gurobi/uptime_downtime_gurobi.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,32 +27,32 @@
                                        name = 'logical')
 
 def _add_initial(model):
     # constraint due to initial conditions.
     def enforce_up_time_constraints_initial(m, g):
         if m._InitialTimePeriodsOnLine[g] == 0:
             return
-        for t in range(m._TimePeriods.first(),
-                m._InitialTimePeriodsOnLine[g]) + m._TimePeriods.first():
+        for t in range(m._TimePeriods[0],
+                m._InitialTimePeriodsOnLine[g] + m._TimePeriods[0]):
             if m._status_vars == 'ALS_state_transition_vars':
                 m._UnitStayOn[g, t].ub = 1
                 m._UnitStayOn[g, t].lb = 1
             else:
                 m._UnitOn[g, t].ub = 1
                 m._UnitOn[g, t].lb = 1
 
     model._EnforceUpTimeConstraintsInitial = [enforce_up_time_constraints_initial(model, g)
                                                 for g in model._ThermalGenerators]
 
     # constraint due to initial conditions.
     def enforce_down_time_constraints_initial(m, g):
         if m._InitialTimePeriodsOffLine[g] == 0:
             return
-        for t in range(m._TimePeriods.first(),
-                m._InitialTimePeriodsOffLine[g]) + m._TimePeriods.first():
+        for t in range(m._TimePeriods[0],
+                m._InitialTimePeriodsOffLine[g] + m._TimePeriods[0]):
             if m._status_vars == 'ALS_state_transition_vars':
                 m._UnitStayOn[g, t].lb = 0
                 m._UnitStayOn[g, t].ub = 0
             else:
                 m._UnitOn[g, t].lb = 0
                 m._UnitOn[g, t].ub = 0
```

### Comparing `powergridsim-0.0.1/powergridsim.egg-info/SOURCES.txt` & `powergridsim-1.0.0/powergridsim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+pyproject.toml
 setup.py
 powergridsim/__init__.py
 powergridsim.egg-info/PKG-INFO
 powergridsim.egg-info/SOURCES.txt
 powergridsim.egg-info/dependency_links.txt
 powergridsim.egg-info/requires.txt
 powergridsim.egg-info/top_level.txt
 powergridsim/models_gurobi/__init__.py
 powergridsim/models_gurobi/_status_vars_gurobi.py
+powergridsim/models_gurobi/_utils_gurobi.py
 powergridsim/models_gurobi/generation_limits_gurobi.py
 powergridsim/models_gurobi/non_dispatchable_vars_gurobi.py
 powergridsim/models_gurobi/objective_gurobi.py
 powergridsim/models_gurobi/params_gurobi.py
 powergridsim/models_gurobi/power_balance_gurobi.py
 powergridsim/models_gurobi/power_vars_gurobi.py
 powergridsim/models_gurobi/production_costs_gurobi.py
+powergridsim/models_gurobi/ptdf_utils_gurobi.py
 powergridsim/models_gurobi/ramping_limits_gurobi.py
 powergridsim/models_gurobi/reserve_requirement_gurobi.py
 powergridsim/models_gurobi/reserve_vars_gurobi.py
 powergridsim/models_gurobi/services_gurobi.py
 powergridsim/models_gurobi/startup_costs_gurobi.py
 powergridsim/models_gurobi/uptime_downtime_gurobi.py
-powergridsim/models_gurobi/utils_gurobi.py
 powergridsim/models_gurobi/transmission_gurobi/__init__.py
 powergridsim/models_gurobi/transmission_gurobi/branch.py
 powergridsim/models_gurobi/transmission_gurobi/bus.py
```

